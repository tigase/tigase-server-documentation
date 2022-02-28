========================================================
Tigase Administration Guide
========================================================

Version:  V8.2.0

1. Tigase XMPP Server 8.2.0 Release Notes
==========================================

Welcome to Tigase XMPP Server 8.2.0! This is a feature release a number of fixes and updates. Here is the list of most important features and changes and below the list of all release notes from all included components

1.1. Highlights
----------------

Version 8.2.0 brings in MIX support. Tigase MIX component is a component extending Tigase PubSub Component and providing support for XEP-0369: MIX protocol extensions being part of MIX specification family.

MIX stands for Mediated Information eXchange (MIX) and it’s basics are defined in XEP-0369: Mediated Information eXchange (MIX):

"an XMPP protocol extension for the exchange of information among multiple users through a mediating service. The protocol can be used to provide human group communication and communication between non-human entities using channels, although with greater flexibility and extensibility than existing groupchat technologies such as Multi-User Chat (MUC). MIX uses Publish-Subscribe to provide flexible access and publication, and uses Message Archive Management (MAM) to provide storage and archiving."

MIX Works in cluster (with ACS-MIX component, requires licence) and with all database, including MongoDB.

1.1.2. Improvements to s2s connection
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Version 8.2.0 brings a lot of improvements related to s2s connectivity: support for TLS1.3, improved logic during authentication and stream negotiation solving connectivity issues with various deployments.

1.1.3. Better handling of certificates
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

It’s now possible to store certificates in the database making it easier to manage them, especially in clustered environment.

1.2. Other significant changes
------------------------------

- Improved performance: reduced memory usage and decrease startup time

- Add publishing executor with rate limiting in PubSub

- Bring MUC specification support up to date

- Improve handling of multiple user session using same nickname in MUC

- Fixes and improvements to MUC ad-hoc scripts

- Enable HTTP File Upload by default with additional, optional, AWS S3 compatible backend

- Improvements to Web Setup to make installation even more straightforward

- Allow exposing .well-known in the root context to facilitate XEP-0156: Discovering Alternative XMPP Connection Methods

- Add option to redirect requests from http to https internally by Tigase XMPP Server

- Added support for sending VoIP push notifications using PushKit

- Support for storing APNS certificates in repository instead of filesystem for easier cluster deployments

- Add priority detection for push notifications to avoid excessive pushes to devices

- Inclusion of APNS certificate validity task that notifies if it’s about to expire

- Add support for urn:xmpp:mam:2

- Add support for XEP-0308: Last Message Correction

- Deprecation of Element based events in favour of Object based events

- Deprecate Deprecate PartitionedStrategy in ACS-PubSub

1.3. Per-component changes
--------------------------

1.3.1. Tigase XMPP Server 8.2.0 release notes
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Tigase XMPP Server 8.2.0 Change notes


Major Change
~~~~~~~~~~~~

- **Improvements to s2s connection**: Version 8.2.0 brings a lot of improvements related to s2s connectivity: support for TLS1.3, improved logic during authentication and stream
  negotiation solving connectivity issues with various deployments

- **Better handling of certificates**: It’s now possible to store certificates in the database making it easier to manage them in clustered environment.

- Deprecation of Element based events in favour of Object based events

- Improved performance: reduced memory usage and decrease startup time

All Minor Features & Behavior Changes

- '#server-1050<https://projects.tigase.net/issue/server-1050>'_: Database installation without root credentials

- "#server-1062<https://projects.tigase.net/issue/server-1062>'_: Deprecate Element based Event-bus

- #server-1097: It’s not possible to configure additional PacketFilters

- #server-1101: Enabling TLS1.3 causes s2s connections to fail

- #server-1102: Add possibility to extend MAM to MAM:2

- #server-1105: Enhance Add SSL Certificate ad-hoc with option to set default

- #server-1119: Use database for certificate storage instead of filesystem

- #server-1120: JabberIqRegister should allow enforcing both CAPTCHA and e-mail

- #server-1132: Don’t use s2s socket if only one-direction works

- #server-1142: After registration inform the client that the account activation (email) is required

- #server-1158: Establishing JMX connection to the server causes excessive memory allocation

- #server-1162: Allow interfaces in @ConfigField

- #server-1170: TLS infinity loop impacts Tigase XMPP Server performance

- #server-1175: Connection with diebesban.de stopped with invalid-namespace error

- #server-1177: Ability to change log level during runtime

- #server-1178: Remove online_status from the repository

- #server-1179: Add support for {clusterNode} in XEP-0215 host field

- #server-1181: NoSuchElementException in MaxDailyCounterQueue

- #server-1182: NPE while processing <iq type="result"/> without existing session

- #server-1187: SchemaLoader should not print passwords in the logs (URL logs)

- #server-1192: Obfuscate repository passwords

- #server-1190: Executing EditUser on non-existen’t user causes creation of the user

- #server-1193: Push notifications are sent for groupchat messages without <body/>

- #server-1197: Infinite loop while cutting body of encrypted push notification to fit the push notifications limit

- #server-1199: Don’t send any packets until s2s stream negotiation is finished

- #server-1200: Use proper size of network buffers for high-throughput connections

- #server-1203: Handing error packets in CIDConnections.sendPacketsBack

- #server-1217: Prevent performing schema upgrade concurrently

- #server-1219: Use all JDBC URI parameters from config.tdsl when performing database upgrade.

- #server-1222: Add support for XEP-0377: Spam Reporting

- #server-1229: Enabling CAPTCHA or e-mail for JabberIqRegister breaks password changing functionality.

- #server-1229: Enabling CAPTCHA or e-mail for JabberIqRegister breaks password changing functionality.

- #server-1233: Add option to CertificateRepository to load certificates from the filesystem

- #server-1234: Roster API improvements

- #server-1237: Rework CertificateRepository so items are stored individually

- #server-1238: Can’t set MOTD via ad-hoc.

- #server-1243: Include wait-for-it.sh script in base distribution

- #server-1245: MethodStatistics doesn’t work well for interfaces with overloaded methods

- #server-1251: Can’t initialise MAM processor with default installation

- #server-1252: Remove select row_count() from Tig_OfflineMessages_DeleteMessage

- #server-1253: It seems that 'expired-processor' doesn’t remove periodically expired messages

- #server-1254: Fix slow startup and shutdown

- #server-1258: Allow beans to be instantiated without the requirement to reference/inject them

- #server-1260: UserConnectedEvent should be a cluster event

- #server-1261: Revise and improve EventBus developer guide

- #server-1269: SSL issues are hidden by default making it difficult to identify

- #server-1273: Add option to limit number of concurrently connected resources

- #server-1277: Fix HUGE out queue in StreamManagementIOProcessor

- #server-1278: NPE in StreamManagementIOProcessor.serviceStopped

- #server-1282: XMPPProcessorAbstract.processToUserPacket() responds to IQ result with error

- #server-1284: Add validation to JabberIqAuth

- #server-1285: Wrong field type for XEP-0157 entries

- #server-1290: Improve StringPrep to actually forbid space in localpart/domain as per rfc7622

- #server-1292: TLS connectivity issue with search.jabber.network

- #server-1297: Add option to push plugin that would allow to overwrite unencrypted part in (OMEMO) encrypted messages

- #server-1303: Better handling of "The target is unavailable at this time." / PacketInvalidTypeException

- #server-1305: Allow creation of admin user (if not exist) during upgrade-schema task

- #server-1306: Fix farge amount of direct memory being used.

- #server-1307: Fix disconnection on MAM sync

- #extras-3: Add AWS logback and documentation how to use it

- #extras-4: Unescape and normalise logs in mail notifications before sending them

- #extras-7: Add email validation during in-band-registration; better handling of mail sending exceptions regarding to non-existent addresses

- #extras-9: Deprecate mDNS implementation

- #serverdist-8: Remove DNS resolution part from XEP-0156 implementation

1.3.2. Tigase MIX 1.0.0 Release Notes
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Major Changes
~~~~~~~~~~~~

This is the introductory version of MIX specification 'family<https://xmpp.org/extensions/xep-0369.html#family>'_

All Changes
~~~~~~~~~~~~

- #mix-2:Implement XEP-0369: Mediated Information eXchange (MIX)

- #mix-3:Implement XEP-0406: Mediated Information eXchange (MIX): MIX Administration

- #mix-6:Create tests for MIX CORE & Participants Server Requirements

- #mix-8:Improve caching

- #mix-9:Add support for MIX-MUC integration

- #mix-10:Invalid response for disco#items

- #mix-14:Add configuration to limit who can create channels in component

- #mix-15:NPE in MAMItemHandler

- #mix-16:Add MIX to installer as option.

- #mix-17:Could not parse new configuration of channel: PubSubException: Only participants and information nodes are supported!

- #mix-18:NPE when sending requests to removed channel nodes

- #mix-19:MAM:2 is not advertised

- #mix-20:MIX component is broadcasting messages with bare JID

- #mix-21:Possibility of duplicated subscription of a node

- #mix-22:Nickname not returned in response after being set

- #mix-23:Remove banned participants from participants list and subscriptions

- #mix-24:NPE in MIXProcessor

- #mix-25:Create MIX component documentation and publish it

- #mix-26:Allow installation admins to manager MIX channels if domain admins are allowed

- #mix-27:MIX-MUC message duplication

- #mix-28:NPE in Affiliations.getSubscriberAffiliation

- #mix-29:Weird "open channel" behaviour

1.3.3. Tigase PubSub 5.0.0 Release Notes
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Major Changes
~~~~~~~~~~~~~


- Add publishing executor with rate limiting

- Optimisations and fixes

All Changes
~~~~~~~~~~~

- #pubsub-102: Add publishing executor with rate limiting

- #pubsub-103: Empty message notification id attribute

- #pubsub-105: NPE in RetrieveItemsModule

- #pubsub-106: NPE in PubsubPublishModule?Eventbus

- #pubsub-107: disco#items feature returned on disco#info request for PubSub node item

- #pubsub-108: Fix Missing notification for published events

- #pubsub-110: Fix Deadlock in TigPubSubRemoveService SP on MySQL

- #pubsub-111: Fix SQLException: At least one parameter to the current statement is uninitialized.

- #pubsub-113: Fix StackOverflowError in LRUCacheWithFuture

- #pubsub-114: Fix pubsub#persist_items is not advertised

- #pubsub-115: Fix Cannot add or update a child row: a foreign key constraint fails (tigasedb.tig_pubsub_items, CONSTRAINT tig_pubsub_items_ibfk_1 FOREIGN KEY (node_id) REFERENCES tig_pubsub_nodes (node_id))

- #pubsub-119: Fix NPE in DiscoveryModule

- #pubsub-120: Fix Empty element in POST payload is incorrectly parsed

- #pubsub-121: Use String.intern() for PEP CAPS nodes string

- #pubsub-124: Fix PubSub sends notifications about last published item on each presence received from subscriber.

- #pubsub-125: Reported features pubsub#metadata should be pubsub#meta-data

- #pubsub-126: Fix Deadlocks in MySQL schema

- #pubsub-127: Fix NPE in UserEntry.remove

- #pubsub-128: Fix PatternSyntaxException for users with emoticons in resource

1.3.4. Tigase MUC 3.2.0 Release Notes
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Major Changes
~~~~~~~~~~~~~

- Bring MUC specification support up to date

- Improve handling of multiple user session using same nickname

- Fixes and improvements to ad-hoc scripts

All Changes
~~~~~~~~~~~

- #muc-133: Add component option to let only admins create rooms

- #muc-134: Better MUC Converter log

- #muc-136: MUC specification supported by Tigase MUC is out of data

- #muc-137: Add support for <iq/> forwarding with multiple resources joined

- #muc-138: tigase@muc.tigase.org kicks my clients if I use them both

- #muc-139: Create script to (mass) delete MUC rooms

- #muc-140: There is no empty <subject/> element for persistent room sent after re-joining

- #muc-141: StringIndexOutOfBoundsException in IqStanzaForwarderModule

- #muc-142: NullPointerException when processing message with subject

- #muc-143: Fix MUC scripts: "No such property: mucRepository for class: tigase.admin.Script151"

- #muc-144: No signature of method: tigase.muc.cluster.RoomClustered.addAffiliationByJid()

1.3.5. Tigase HTTP-API 2.2.0 Release Notes
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Major Changes
~~~~~~~~~~~~~

- Enable HTTP File Upload by default with additional, optional, AWS S3 compatible backend

- Improvements to Web Setup to make installation even more straightforward

- Allow exposing *.well-known* in the root context to facilitate 'XEP-0156: Discovering Alternative XMPP Connection Methods<https://xmpp.org/extensions/xep-0156.html>'_

- Add option to redirect requests from http to https

All Changes
~~~~~~~~~~~
- #http-65: More detailed logs

- #http-86: Add s3 backend for http-upload

- #http-91: Items in setup on Features screen are misaligned

- #http-93: Update web-installer documentation

- #http-95: Enable HTTP File Upload by default

- #http-96: Enabling cluster mode / ACS doesn’t add it to resulting configuration file

- #http-98: Setup tests are failing since Septempter

- #http-99: Enforce max-file-size limit

- #http-100: Prevent enabling all Message* plugins

- #http-101: Prevent enabling all Mobile* plugins

- #http-102: Last activity plugins handling should be improved

- #http-103: Enabling http-upload should give an info about requirement to set domain/store

- #http-105: Handle forbidden characters in filenames

- #http-106: Can’t remove user for non-existent VHost

- #http-107: Allow exposing .well-known in the root context

- #http-108: Add option to redirect requests from http to https

- #http-109: openAccess option is missing after migrating the component to TK

- #http-110: Add support for querying and managing uploaded files

- #http-111: DefaultLogic.removeExpired removal of slot failed

- #http-113: Add condition to redirect only if the X-Forwarded-Proto has certain value

- #http-114: TigaseDBException: Could not allocate slot

- #http-116: Limiting list of VHosts doesn’t work for JDK based http-server

- #http-117: Http redirection doesn’t work in docker

- #http-119: Can’t change VHost configuration via Admin WebUI

- #http-120: Improve S3 support for HTTP File Upload to accept custom URL and credentials for S3 storage configuration

- #http-121: Deprecate DnsWebService and rewrite /.well-known/host-meta generator

1.3.6. Tigase Push 1.2.0 Release Notes
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Major Changes
~~~~~~~~~~~~~

- Added support for sending VoIP push notifications using PushKit

- Support for storing APNS certificates in repository instead of filesystem for easier cluster deployments

- Add priority detection for push notifications to avoid excessive pushes to devices

- Inclusion of APNS certificate validity task that notifies if it’s about to expire

All Changes
~~~~~~~~~~~

- #push-29 Added support for sending VoIP push notifications using PushKit

- #push-30 Added REST API handler for quick unregistration of a device

- #push-32 Fixed issue with APNS certificate validation

- #push-33 Added statistics gathering

- #push-35 Added support for APNS certificate in PEM

- #push-36 Improved priority detection of push notifications

- #push-37 Enable APNS certificates to be stored in UserRepository - management is done via ad-hoc command;

- #push-39 Changes to improve error handling

- #push-41 Fixed issue with ApnsService exceptions not being thown logged

- #push-42 Fixed error type reported back on tooManyRequestsForDeviceToken

- #push-47 Added task to periodically validate SSL certificates for Push notifications

- #push-48 Fixed handling events by APNsBinaryApiProvider

- #push-49 Added enforcement to use HTTP/2 protocol (with use of ALPN)

1.3.7. Tigase Message Archiving 3.0.0 Release Notes
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Major Changes
~~~~~~~~~~~~~

- Add support for urn:xmpp:mam:2

- Add support for XEP-0308: Last Message Correction

All Changes
~~~~~~~~~~~
- #mam-47: Add support for urn:xmpp:mam:2

- #mam-49: Historical message duplication

- #mam-50: XEP-0308: Last Message Correction

- #mam-51: Fix OMEMO encrypted messages are not stored by MA or MAM

- #mam-54: Fix NPE in MAM/Message Archiving

- #mam-55: Fix IllegalArgumentException in MessageArchiveVHostItemExtension

- #mam-56: Fix upgrade-schema failes

- #mam-58: Change message archiving rules

- #mam-60: Fix Message carbons stored in MAM

- #mam-61: Adjust schema to use new primary keys

- #mam-65: Fix archiveMessage: Data truncation: Data too long for column _body

- #mam-66: Fix NPE in AbstractMAMProcessor.updatePrefrerences()

- #mam-67: Fix Incorrect datetime value in JDBCMessageArchiveRepository

- #mam-68: Add option to disable local MAM archive

- #mam-69: Fix Data truncation: Data too long for column '_stanzaId'

- #mam-70: Fix Schema is inconsistent (tigase.org mysql vs clean postgresql)

- #mam-72: Fix Deadlock on inserting message

1.3.8. Tigase Advanced Clustering Strategy (ACS) 3.2.0 Release Note
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Major Changes
~~~~~~~~~~~~~

- Deprecate Deprecate PartitionedStrategy in ACS-PubSub

All Changes
~~~~~~~~~~~~~

- #acs-8: Fix NotAuthorizedException: Session has not been yet authorised. in OnlineUsersCachingStrategy

- #acsmix-1: Implement clustering support for MIX

- #acsmix-3: Fix NPE in DefaultPubSubLogic

- #acsmix-4: Fix NPE in DefaultPubSubLogic.subscribersOfNotifications()

- #acsmuc-23: Fix NPE in ClusteredRoomStrategyV2

- #acsmuc-25: Fix NPE in OccupantChangedPresenceCmd

- #acspubsub-20: Fix NPE in pubsub-nodes-changed-cmd

- #acspubsub-21: Fix Multiple notifications for single publication

- #acspubsub-22: Fix Presences informations are kept indefinitely

- #acspubsub-24: Fix caps-changed-cmd not processed correctly

- #acspubsub-25: Deprecate PartitionedStrategy

- #acspubsub-27: Review and improve clustering documentation