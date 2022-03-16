9. Tigase PubSub Component
===========================

Welcome to Tigase PubSub component guide

9.1. PubSub Component
----------------------

Tigase’s Publish Subscribe component is an `XEP-0060 <http://www.xmpp.org/extensions/xep-0060.html>`__ compliant plugin handling all publish and subscribe activity within Tigase server. This is enabled as default with the pubsub name, however you may include the following line if you wish to customize it’s configuration.

.. code:: dsl

   pubsub () {}

You may change the name so long as you specify the pubsub class within parenthesis.

9.1.1. Tigase Pubsub Release Notes
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Welcome to Tigase Pubsub 5.0.0! This is a feature release for with a number of fixes and updates.

Tigase PubSub 5.0.0 Release Notes
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Major Changes
''''''''''''''

-  Add publishing executor with rate limiting

-  Optimisations and fixes


All Changes
''''''''''''

-  `#pubsub-102 <https://projects.tigase.net/issue/pubsub-102>`__: Add publishing executor with rate limiting

-  `#pubsub-103 <https://projects.tigase.net/issue/pubsub-103>`__: Empty message notification id attribute

-  `#pubsub-105 <https://projects.tigase.net/issue/pubsub-105>`__: NPE in RetrieveItemsModule

-  `#pubsub-106 <https://projects.tigase.net/issue/pubsub-106>`__: NPE in PubsubPublishModule?Eventbus

-  `#pubsub-107 <https://projects.tigase.net/issue/pubsub-107>`__: disco#items feature returned on disco#info request for PubSub node item

-  `#pubsub-108 <https://projects.tigase.net/issue/pubsub-108>`__: Fix Missing notification for published events

-  `#pubsub-110 <https://projects.tigase.net/issue/pubsub-110>`__: Fix Deadlock in TigPubSubRemoveService SP on MySQL

-  `#pubsub-111 <https://projects.tigase.net/issue/pubsub-111>`__: Fix SQLException: At least one parameter to the current statement is uninitialized.

-  `#pubsub-113 <https://projects.tigase.net/issue/pubsub-113>`__: Fix StackOverflowError in LRUCacheWithFuture

-  `#pubsub-114 <https://projects.tigase.net/issue/pubsub-114>`__: Fix pubsub#persist_items is not advertised

-  `#pubsub-115 <https://projects.tigase.net/issue/pubsub-115>`__: Fix Cannot add or update a child row: a foreign key constraint fails (``tigasedb``.\ ``tig_pubsub_items``, CONSTRAINT ``tig_pubsub_items_ibfk_1`` FOREIGN KEY (``node_id``) REFERENCES ``tig_pubsub_nodes`` (``node_id``))

-  `#pubsub-119 <https://projects.tigase.net/issue/pubsub-119>`__: Fix NPE in DiscoveryModule

-  `#pubsub-120 <https://projects.tigase.net/issue/pubsub-120>`__: Fix Empty element in POST payload is incorrectly parsed

-  `#pubsub-121 <https://projects.tigase.net/issue/pubsub-121>`__: Use String.intern() for PEP CAPS nodes string

-  `#pubsub-124 <https://projects.tigase.net/issue/pubsub-124>`__: Fix PubSub sends notifications about last published item on each presence received from subscriber.

-  `#pubsub-125 <https://projects.tigase.net/issue/pubsub-125>`__: Reported features ``pubsub#metadata`` should be ``pubsub#meta-data``

-  `#pubsub-126 <https://projects.tigase.net/issue/pubsub-126>`__: Fix Deadlocks in MySQL schema

-  `#pubsub-127 <https://projects.tigase.net/issue/pubsub-127>`__: Fix NPE in UserEntry.remove

-  `#pubsub-128 <https://projects.tigase.net/issue/pubsub-128>`__: Fix PatternSyntaxException for users with emoticons in resource

Previous Releases
~~~~~~~~~~~~~~~~~~~

Announcement
'''''''''''''

Major changes

Tigase pubsub component has undergone a few major changes to our code and structure. To continue to use Tigase pubsub component, a few changes may be needed to be made to your systems. Please see them below:

Database schema changes

Current version comes with changes to database schema to improve JID comparison during lookup of nodes, subscriptions, affiliations, etc.

To continue usage of new versions of pubsub component it is required to manually load new component database schema, see `database preparation <#databasePreparation>`__ section for more information.

.. Warning::

    Loading of new database schema is required to use new version of pubsub component.

Changes in REST API

We continuously work on improving usability and making our REST API easier to use we added support for handling JSON requests in REST API for pubsub. At the same time we decided to slightly modify responses in XML sent by REST API to make responses in JSON and XML similar.

For more informations about current REST API please look into `Rest API <#restAPI>`__ section.

New features
Support for using separate database for different domains

Since this version it is possible to use separate pubsub nodes and items based on domains. This allows you to configure component to store informations about nodes and items for particular domain to different database.

For more informations please look into `using multiple databases <#multidb>`__.

Support for MAM

In this version we added support for `XEP-0313: Message Archive Management <http://xmpp.org/extensions/xep-0313.html:>`__ protocol which allows any MAM compatible XMPP client with pubsub support to retrieve items published on pubsub nodes using MAM protocol for querying.

9.1.2. Configuration
^^^^^^^^^^^^^^^^^^^^

Pubsub naming
~~~~~~~~~~~~~

Within Tigase, all pubsub component address MUST be domain-based address and not a JID style address. This was made to simplify communications structure. Tigase will automatically set component names to pubsub.domain, however any messages send to pubsub@domain will result in a ``SERVICE_UNAVAILABLE`` error.

Pubsub nodes within Tigase can be found as a combination of JID and node where nodes will be identified akin to service discovery. For example, to address a friendly node, use the following structure:

.. code:: xml

   <iq to='pubsub.domain'>
     <query node='friendly node'/>
   </iq>


Configure Roster Maximum size
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Administrators can configure the maximum allowable roster size per user via the config.tdsl file.

.. code:: dsl

   'sess-man' {
       'jabber:iqa:roster' {
           max_roster_size = '100'
       }
   }

This sets the roster limit to 100 entries per user. It can be set to any integer, however by default no limit is set and no configuration is set in ``config.tdsl`` file.

Store Full XML of Last Presence
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Tigase can store a more detailed ``<unavailable/>`` presence stanza to include timestamps and other information.

Requirements
''''''''''''

Ensure that ``presence-offline`` plugin is enabled in config.tdsl. To do this, add be sure ``presence-offline`` is listed under ``sess-man``

.. code:: dsl

   'sess-man' {
       'presence-offline' () {}
   }

The following two lines in ``sess-man`` configure options to broadcast probes to offline users.

.. code:: dsl

   'sess-man' {
       'skip-offline' = 'false'
       'skip-offline-sys' = 'false'
   }

Without these lines, Tigase will not send presence probes to users that the server knows to be offline.

The full XML presence is stored under the tig_pairs table with a pkey of ``last-unavailable-presence`` will look like this:

.. code:: xml

   <presence from="user@example.com" xmlns="jabber:client" type="unavailable">
   <status>Logged out</status>
   <delay stamp="2015-12-29T16:51:50.748Z" xmlns="urn:xmpp:delay"/></presence>

As you can see, the plugin has added a delay stamp which indicates the last time they were seen online. This may be suppressed by using the following line in your config.tdsl file.

.. code:: dsl

   'sess-man' {
       'delay-stamp' = 'false'
   }

You may also limit probe responses only to newly connected resources.

.. code:: dsl

   'sess-man' {
       'probe-full-jid' = 'true'
   }

When a user logs on, they will receive the same full unavailable presence statements from contacts not logged in. Also the repository entry containing their last unavailable presence will be removed.

**NOTE: This will increase traffic with users with many people on their rosters.**

Using separate store
~~~~~~~~~~~~~~~~~~~~~~

As mentioned above, by default Tigase pubsub component uses default data source configured for Tigase XMPP Server. It is possible to use separate store by pubsub component. To do so you need to configure new ``DataSource`` in ``dataSource`` section. Here we will use ``pubsub-store`` as name of newly configured data source. Additionally you need to pass name of newly configured data source to ``dataSourceName`` property of default DAO of pubsub component.

::

   dataSource {
       pubsub-store () {
           uri = 'jdbc:postgresql://server/pubsub-database'
       }
   }

   pubsub () {
       dao {
           default () {
               dataSourceName = 'pubsub-store'
           }
       }
   }

It is also possible to configure separate store for particular domain, ie. ``pubsub.example.com``. Here we will configure data source with name ``pubsub.example.com`` and use it to store data for pubsub nodes and items at ``pubsub.example.com``:

::

   dataSource {
       'pubsub.example.com' () {
           uri = 'jdbc:postgresql://server/example-database'
       }
   }

   pubsub () {
       dao {
           'pubsub.example.com' () {
             # we may not set dataSourceName as it matches name of domain
           }
       }
   }

.. Note::

   With this configuration, data for other domains than ``pubsub.example.com`` will be stored in default data source.


Enabling PEP support
~~~~~~~~~~~~~~~~~~~~~

To enable `XEP-0163: Personal Eventing Protocol <http://xmpp.org/extensions/xep-0163.html>`__ support it is required to set ``persistent-pep`` property of pubsub component to ``true``, set ``send-last-published-item-on-presence`` property of component to ``true`` and enable ``pep`` SessionManager processor.

::

   pubsub () {
       persistent-pep = true
       send-last-published-item-on-presence = true
   }

   sess-man () {
       pep () {
       }
   }

.. Note::

   If your pubsub component uses different name than ``pubsub`` then you need to set ``pubsub-jid`` property of ``pep`` processor to JID of pubsub component make it aware of a different name of a pubsub component.

**Example with pubsub component named ``events`` hosted at server named ``servername.com`` and enabled PEP.**

::

   events () {
       persistent-pep = true
       send-last-published-item-on-presence = true
   }
   sess-man () {
       pep () {
           'pubsub-jid' = 'events@servername.com'
       }
   }


Enabling REST API
~~~~~~~~~~~~~~~~~~

To use REST API for pubsub component it is required that:

-  Tigase HTTP API component is installed and configured properly. For information about HTTP API component installation please look into `HTTP component documentation <#compHTTPAPI>`__.

-  Tigase pubsub REST scripts are copied to HTTP API REST scripts directory In installation package this is already done and scripts are in proper locations. dd\* JID of HTTP API component needs to be added to list of trusted jids of Tigase pubsub component ``trusted`` property (if ``http`` is name of HTTP API component)

::

   pubsub () {
       trusted = [ 'http@{clusterNode}' ];
   }

Changing nodes cache size
~~~~~~~~~~~~~~~~~~~~~~~~~~

By default Tigase pubsub component caches node configuration of 2000 last loaded nodes. If there are many requests to database to load node configuration and your installation contains many nodes it may be a good idea to increase number of cached nodes.

To do this you need to set ``pubsub-repository-cache-size`` property of pubsub component to new size.

::

   pubsub () {
       pubsub-repository-cache-size = 4000
   }


Enable sending last published item on presence
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

By default it is not possible to use delivery of last published item when users broadcasts initial presence. To do so you need to set ``send-last-published-item-on-presence`` of pubsub component to ``true``. This will allow you to configure nodes to send last published item on presence.

::

   pubsub () {
       send-last-published-item-on-presence = true
   }


Throttling sending notifications
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Notifications sent by PubSub component may be sent in large batches, if you have a nodes with a lot of subscribers. In those cases, it is useful to throttle publications to improve behaviour and performance of other parts of Tigase XMPP Server.

To achieve that, PubSub throttles generate notifications to specified throughput. By default it is set to 5k packets for each CPU core available per second.

To set it to a different value, you can set ``limit`` property of ``publishExecutor`` bean to the expected number of publications per second, ie. 100000;

.. Note::

   This value is a number of total throughput, and will not be adjusted by the number of available CPU cores.

::

   pubsub () {
       publishExecutor () {
           limit = 10000
       }
   }

Publication rate is also adjusted to current memory usage on a 4 point scale adjusted to the value of two configuration options: ``highMemoryUsageLimit`` and ``criticalMemoryUsageLimit`` (with default values: 90% and 98% respectively): \* ``normal`` - if memory usage is below ``highMemoryUsageLimit`` (i.e. below 90%) \* ``high`` - memory usage less than halfway between ``highMemoryUsageLimit`` and ``veryHigh`` (i.e. between 90% and 94%) \* ``veryHigh`` - memory usage more than halfway between ``highMemoryUsageLimit`` and ``veryHigh`` (i.e. between 94% and 98%) \* ``critical`` - if memory usage is above ``criticalMemoryUsageLimit`` (i.e. above 98%)

It’s possible to adjust values of the high and critical limits in publisher bean:

::

   pubsub () {
       publishExecutor () {
           highMemoryUsageLimit = 90
           criticalMemoryUsageLimit = 98
       }
   }


Disable automatic subscription of node creator
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

During creation of node pubsub component subscribes creator to pubsub node and delivers notifications to creator. If in your case you do not want this behavior, you may set ``auto-subscribe-node-creator`` property of pubsub component to ``false``.

::

   pubsub () {
       auto-subscribe-node-creator = false
   }

9.1.3. Database
^^^^^^^^^^^^^^^^

Preparation of database
~~~~~~~~~~~~~~~~~~~~~~~~~~

Before you will be able to use Tigase PubSub Component you need to initialize database. We provide few schemas for this component for MySQL, PostgreSQL, SQLServer and DerbyDB.

They are placed in ``database/`` directory of installation package and named in ``dbtype-pubsub-version.sql``, where ``dbname`` in name of database type which this schema supports and ``version`` is version of a PubSub component for which this schema is designed.

You need to manually select schema for correct database and component and load this schema to database. For more information about loading database schema look into `database preperation <#databasePreperation>`__ section of this guide.

Upgrade of database schema
~~~~~~~~~~~~~~~~~~~~~~~~~~

Database schema for our components may change between versions and if so it needs to be updated before new version may be started. To upgrade schema please follow instructions from the `database preperation <#databasePreperation>`__ section.

.. Note::

   If you use SNAPSHOT builds then schema may change for same version as this are versions we are still working on.

Schema description
~~~~~~~~~~~~~~~~~~~~~~~~~~

Tigase PubSub component uses few tables and stored procedures. To make it easier to identify tables and stored procedures used by PubSub component they are prefixed with ``tig_pubsub_``.

Table ``tig_pubsub_service_jids``
''''''''''''''''''''''''''''''''''

This table stores all jids for which PubSub component contains nodes.

+------------------+--------------------------------------+----------------------------------------------------+
| Field            | Description                          | Comments                                           |
+==================+======================================+====================================================+
| service_id       | Database ID of a service JID         |                                                    |
+------------------+--------------------------------------+----------------------------------------------------+
| service_jid      | Value of a service JID               |                                                    |
+------------------+--------------------------------------+----------------------------------------------------+
| service_jid_sha1 | SHA1 value of lowercased service JID | Used for proper bare JID comparison during lookup. |
|                  |                                      |                                                    |
|                  |                                      | (N/A to PostgreSQL schema)                         |
+------------------+--------------------------------------+----------------------------------------------------+

Table ``tig_pubsub_jids``
''''''''''''''''''''''''''

This table stores all jids related to PubSub nodes, ie. subscriber, affiliates, creators, publishers, etc.

+----------+-----------------------------------+----------------------------------------------------+
| Field    | Description                       | Comments                                           |
+==========+===================================+====================================================+
| jid_id   | Database ID of a bare JID         |                                                    |
+----------+-----------------------------------+----------------------------------------------------+
| jid      | Value of a bare JID               |                                                    |
+----------+-----------------------------------+----------------------------------------------------+
| jid_sha1 | SHA1 value of lowercased bare JID | Used for proper bare JID comparison during lookup. |
|          |                                   |                                                    |
|          |                                   | (N/A to PostgreSQL schema)                         |
+----------+-----------------------------------+----------------------------------------------------+

Table ``tig_pubsub_nodes``
'''''''''''''''''''''''''''

Table stores nodes tree structure and node configuration.

+---------------+-----------------------------------------+------------------------------------------------------------+
| Field         | Description                             | Comments                                                   |
+===============+=========================================+============================================================+
| node_id       | Database ID of a node                   |                                                            |
+---------------+-----------------------------------------+------------------------------------------------------------+
| service_id    | ID of service JID                       | References ``service_id`` from ``tig_pubsub_service_jids`` |
+---------------+-----------------------------------------+------------------------------------------------------------+
| name          | Name of PubSub node                     |                                                            |
+---------------+-----------------------------------------+------------------------------------------------------------+
| name_sha1     | SHA1 of PubSub node name                | Used for indexing and faster lookup.                       |
|               |                                         |                                                            |
|               |                                         | (N/A to PostgreSQL schema)                                 |
+---------------+-----------------------------------------+------------------------------------------------------------+
| type          | Type of PubSub node                     | 0 - collection                                             |
|               |                                         |                                                            |
|               |                                         | 1 - leaf                                                   |
+---------------+-----------------------------------------+------------------------------------------------------------+
| title         | Title of PubSub node                    |                                                            |
+---------------+-----------------------------------------+------------------------------------------------------------+
| description   | Description of a node                   |                                                            |
+---------------+-----------------------------------------+------------------------------------------------------------+
| creator_id    | ID of JID of creator                    | References ``jid_id`` from ``tig_pubsub_jids``             |
+---------------+-----------------------------------------+------------------------------------------------------------+
| creation_date | Timestamp of creation time              |                                                            |
+---------------+-----------------------------------------+------------------------------------------------------------+
| configuration | Serialized configuration of PubSub node |                                                            |
+---------------+-----------------------------------------+------------------------------------------------------------+
| collection_id | Points collection (parent node)         | References ``node_id`` from ``tig_pubsub_nodes``           |
+---------------+-----------------------------------------+------------------------------------------------------------+

Table ``tig_pubsub_affiliations``
'''''''''''''''''''''''''''''''''''

Table stores affiliations between PubSub nodes and jids.

+-------------+-------------------+--------------------------------------------------+
| Field       | Description       | Comments                                         |
+=============+===================+==================================================+
| node_id     | ID of a node      | References ``node_id`` from ``tig_pubsub_nodes`` |
+-------------+-------------------+--------------------------------------------------+
| jid_id      | ID of a user JID  | References ``jid_id`` from ``tig_pubsub_jids``   |
+-------------+-------------------+--------------------------------------------------+
| affiliation | Affiliation value |                                                  |
+-------------+-------------------+--------------------------------------------------+

Table ``tig_pubsub_subscriptions``
'''''''''''''''''''''''''''''''''''

Table stores subscriptions of jids to PubSub nodes.

+-----------------+----------------------+--------------------------------------------------+
| Field           | Description          | Comments                                         |
+=================+======================+==================================================+
| node_id         | ID of a node         | References ``node_id`` from ``tig_pubsub_nodes`` |
+-----------------+----------------------+--------------------------------------------------+
| jid_id          | ID of a user JID     | References ``jid_id`` from ``tig_pubsub_jids``   |
+-----------------+----------------------+--------------------------------------------------+
| subscription    | Subscription value   |                                                  |
+-----------------+----------------------+--------------------------------------------------+
| subscription_id | Id of a subscription |                                                  |
+-----------------+----------------------+--------------------------------------------------+

Table ``tig_pubsub_items``
''''''''''''''''''''''''''''

Table stores items of PubSub nodes.

+---------------+-------------------------------------+--------------------------------------------------+
| Field         | Description                         | Comments                                         |
+---------------+-------------------------------------+--------------------------------------------------+
| node_id       | ID of a node                        | References ``node_id`` from ``tig_pubsub_nodes`` |
+---------------+-------------------------------------+--------------------------------------------------+
| id            | Id of an items                      |                                                  |
+---------------+-------------------------------------+--------------------------------------------------+
| id_sha1       | SHA1 of item id                     | Indexed and used for faster lookup               |
|               |                                     |                                                  |
|               |                                     | (N/A to PostgreSQL schema)                       |
+---------------+-------------------------------------+--------------------------------------------------+
| creation_date | Creation date                       |                                                  |
+---------------+-------------------------------------+--------------------------------------------------+
| publisher_id  | ID of publisher JID                 | References ``jid_id`` from ``tig_pubsub_jids``   |
+---------------+-------------------------------------+--------------------------------------------------+
| update_date   | Timestamp of last item modification |                                                  |
+---------------+-------------------------------------+--------------------------------------------------+
| data          | Item payload                        |                                                  |
+---------------+-------------------------------------+--------------------------------------------------+

PubSub Schema Changes
~~~~~~~~~~~~~~~~~~~~~~

Tigase PubSub Component is currently version 3.3.0 which is introduced in Tigase server v8.0.0.

PubSub 3.2.0 Changes
'''''''''''''''''''''

PubSub v 3.2.0 adds a new procedure TigPubSubGetNodeMeta which supports PubSub metadata retrieval while conducting a disco#info query on nodes.

You will need to upgrade your database if you are not using v3.2.0 schema. Tigase will report being unable to load PubSub component if you do not have this schema version.

The MySQL schema can be found `Here <https://projects.tigase.org/projects/tigase-pubsub/repository/revisions/master/entry/database/mysql-pubsub-schema-3.2.0.sql>`__.

The Derby schema can be found `Here <https://projects.tigase.org/projects/tigase-pubsub/repository/changes/database/derby-pubsub-schema-3.2.0.sql>`__.

The PostGRESQL schema can be found `Here <https://projects.tigase.org/projects/tigase-pubsub/repository/changes/database/postgresql-pubsub-schema-3.2.0.sql>`__.

The MS SQL schema can be found `Here <https://projects.tigase.org/projects/tigase-pubsub/repository/changes/database/sqlserver-pubsub-schema-3.2.0.sql>`__.

The same files are also included in all distributions of v8.0.0 in ``[tigaseroot]/database/`` . All changes to database schema are meant to be backward compatible.

For instructions how to manually upgrade the databases, please refer to `Tigase v7.1.0 Schema Updates section <#tigaseServer71>`__.

Upgrading older installations (pre-v3.0.0 Schema)
''''''''''''''''''''''''''''''''''''''''''''''''''

To update older installations of Tigase to the PubSub Schema v3.0.0 follow these instructions. Note this should be done before upgrading to PubSub v3.1.0.

Step by Step guide.

Prepare Old Database for Upgrade

In ``database`` directory of Tigase installation you will find SQL files which will prepare old database schema for upgrade using following this naming pattern: ``<database_type>-pubsub-schema-3.0.0-pre-upgrade.sql`` Where ``<database_type>`` can be one of the following: ``mysql``, ``sqlserver``, ie. for MySQL you will find the file ``mysql-pubsub-schema-3.0.0-pre-upgrade.sql``. You need to execute statements from this file on your source database, which will drop old procedures and functions used to access database and also this statements will rename old tables by adding suffix \_1 to each of old tables. Example:

**MySQL**
   ``mysql -u tigase -p tigase_pubsub < database/mysql-pubsub-schema-3.0.0-pre-upgrade.sql``

**MS SQL**
   ``sqlcmd -S %servername% -U %root_user% -P %root_pass% -d %database% -i database\sqlserver-pubsub-schema-3.0.0-pre-upgrade.sql``

Update Tigase PubSub Component

For this you need to copy the Tigase PubSub Component jar file to jars directory inside Tigase XMPP Server installation directory. It is also recommended to copy files from database directory of Tigase PubSub Component to database directory in Tigase XMPP Server installation directory.

If you happen to use one of the the distribution packaged (either installer or -dist-max flavored archive) then all required files are already available - both new schema files will be available in ``database/`` directory as well as both versions of PubSub component will be present in ``jars/`` directory - PubSub3 as tigase-pubsub.jar and PubSub2 as tigase-pubsub-2.2.0.jar.old (provided for compatibility reasons).

Load New Schema

In the ``database`` directory you will find files containing new schemas for:

-  MySQL - ``mysql-pubsub-schema-3.0.0.sql``

-  PostgreSQL - ``postgresql-pubsub-schema-3.0.0.sql``

-  MSSQL - ``sqlserver-pubsub-schema-3.0.0.sql``

-  DerbyDB - ``derby-pubsub-schema-3.0.0.sql`` and ``pubsub-db-create-derby.sh``

For most databases, with the exception of Derby, you only need to execute statements from the proper file. For example:

**MySQL**
   ``mysql -u tigase -p tigase_pubsub < database/mysql-pubsub-schema-3.0.0.sql``

**MS SQL**
   ``sqlcmd -S %servername% -U %root_user% -P %root_pass% -d %database% -i database\sqlserver-pubsub-schema-3.0.0.sql``

**PostgreSQL**
   ``psql -h $DB_HOST -q -U ${USR_NAME} -d $DB_NAME -f database/sqlserver-pubsub-schema-3.0.0.sql``

For DerbyDB you need to execute the ``pubsub-db-create-derby.sh`` script and pass proper JDBC URI to database to which you want to load schema (if database does not exist, it will be created).

::

   database/pubsub-db-create-derby.sh

**NOTE:** It is possible to use same database which was used before - then after upgrade you will have new tables and old tables with \_1 suffix.

Execute Migration Utility

In the ``/database`` directory you will find the ``pubsub-db-migrate.sh`` file which you need to execute and pass arguments with JDBC URIs needed to connect to source and destination database. If you used dedicated tables for PubSub you will also need to pass a class name used to access database (value of ``pubsub-repo-class`` variable from ``etc/config.tdsl`` file).

Example for dedicated table used for PubSub:

.. code:: sql

   database/pubsub-db-migrate.sh -in-repo-class tigase.pubsub.repository.PubSubDAO
   -in 'jdbc:mysql://localhost/tigase_pubsub?user=tigase&password=passwd'
   -out 'jdbc:mysql://localhost/tigase_pubsub?user=tigase&password=passwd'

Example for use without dedicated PubSub tables:

.. code:: sql

   database/pubsub-db-migrate.sh
   -in 'jdbc:mysql://localhost/tigase?user=tigase&password=passwd'
   -out 'jdbc:mysql://localhost/tigase?user=tigase&password=passwd'

Example for use with dedicated tables in a Windows environment:

.. code:: sql

   database/pubsub-db-migrate.cmd -in-repo-class tigase.pubsub.repository.PubSubDAO
   -in 'jdbc:sqlserver://<hostname>\\<instance>:<port>;databaseName=<name>;user=tigase;password=tigase;schema=dbo;lastUpdateCount=false'
   -out 'jdbc:sqlserver://<hostname>\\<instance>:<port>;databaseName=<name>;user=tigase;password=tigase;schema=dbo;lastUpdateCount=false'

During execution this utility will report information about migration of PubSub data to the new schema, and the same information will be store in ``pubsub_db_migration.log``.

Finish

After successful migration you will have all data copied to new tables. Old tables will be renamed by adding suffix \_1. After verification that everything works OK, you can delete old tables and it’s content as it want be used any more.

9.1.4. Features
^^^^^^^^^^^^^^^^

9.1.5. AdHoc Commands
^^^^^^^^^^^^^^^^^^^^^^