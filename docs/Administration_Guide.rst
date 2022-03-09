
2. Tigase XMPP Server Distribution Administration Guide
=======================================================

2.1. Tigase User Guide
-----------------------

2.1.1. Jabber/XMPP introduction
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Jabber/XMPP is Instant Messaging Technology
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
All federated **XMPP** servers are connected in one global communications network allowing you to send messages to friends who have accounts on other Jabber servers.

This is very much like sending e-mail but the difference between Jabber and e-mail is the same as the difference between sending a traditional mail and talking on the phone.

All messages sent through Jabber are sent instantly and you also receive responses instantly. More over you can see whether your mate is online and available for talking or not.

There exists similar technologies to Jabber like WhatsApp Messenger, Facebook Messenger, Signal, Telegram, WeChat, QQ and other. There are, however, quite a few differences.

XMPP is an open standard which means everybody can know how it works, everybody can implement their own software connecting to the network both client and server side.

The server side is actually the biggest difference and advantage. Many companies have offices in different locations, and such instant messaging technology could be very useful to employees for communication. Companies are not inclined to allow confidential discussions to go outside the company’s network. Especially if it is not very secure to leave such information on third party public servers.

XMPP servers on the other hand, allows you to deploy server software on your own company network. Employees can then talk securely and all information remains on the company’s secure network. Of course if offices are located in different locations or countries then all messages are transmitted over the public network - the Internet. This is not a problem since XMPP supports SSL/TLS - secure encrypted connections which helps you protect your discussion.

Then if your employees need to contact customers outside your company, the whole discussion can go through your server and a server located on the customer side.

There are many other scenarios and use cases but I hope this brief introduction gives you an idea of the differences and advantages of XMPP technology.

2.1.2. How to Use Tigase Service
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^


This Article Describes How to use **tigase.im** Service for Instant Communications
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

You have to install and run a Jabber client application to use the service.

There are multiple domains available: tigase.im, sure.im, xmpp.cloud (and you can host your own domain as well)


Short instructions:
~~~~~~~~~~~~~~~~~~~

Usually you just need to enter the user name of the form: user@tigase.im. Your XMPP client should take care of all other things as our service doesn’t need any special settings. If you don’t have an account on tigase.im server yet just tick the option to register new account. That’s it!


**Long Instructions:**
~~~~~~~~~~~~~~~~~~~~~~

Good news is that there are many programs to choose from which allow you to communicate through our server. So you can pick up your favorite application or use an existing one that is compatible and start using our service.

All clients presented below support multiple accounts on Jabber servers. What this means is that you can have a few Jabber accounts on different Jabber servers and you can still use just one program to connect to all of them at the same time.

The `full list of all known XMPP clients <https://xmpp.org/software/clients.html>`__ is very long. You can obviously try them all but below is a selection which is recommended by the Tigase team. The selected programs might not be the best choice for you, but these programs have been tested and we can offer help with using them. Here is a list of recommended instant messaging clients:

-  `Beagle.im <https://beagle.im/>`__ - macOS desktop client developed by Tigase team supporting all the latest and greatest features

-  `Tigase Messenger for iOS <https://itunes.apple.com/us/app/tigase-messenger/id1153516838>`__ - lightweight, powerful XMPP client developed by Tigase, Inc. It provides an easy way to start using the XMPP Protocol (formerly known as Jabber) if you’ve never used it before. Veterans of the protocol will find many features here they are familiar with along with enhancements to reduce data use and extend battery life.

-  `Tigase Messenger for Android <https://play.google.com/store/apps/details?id=org.tigase.messenger.phone.pro>`__ - mobile chat client to use with XMPP services and servers. The totally revamped v3.0 now has new features, a better design, and Google integration. Application supports any XMPP server, from free services like sure.im or Tigase.im, to a server you may host on your own.

-  tigase.im[Tigase.im] - web-based client allowing to easily chat with friends independently of platform.

-  `Psi <http://psi-im.org/>`__ Pure Jabber client. Although it supports only Jabber network it is a very user friendly and comfortable program. It works on most popular operating systems like Linux, MS Windows, and Apple MacOS X.

-  `Gajim <http://www.gajim.org/>`__ This is another Jabber only client. Very user friendly and works on most of Linux distributions, FreeBSD, and MS Windows.

-  `Pidgin <http://www.pidgin.im/>`__ (previously `Gaim <http://gaim.sourceforge.net/>`__) This is not just a Jabber client. This type of application is called multicommunicator as apart from Jabber it supports many other instant messaging networks/protocols such as: AIM/ICQ, MSN, Yahoo, Gadu-Gadu, IRC, and a few others. So it is especially convenient if you have friends using other messaging networks. Pidgin works on most Linux distributions, and on MS Windows.

-  `Kopete <http://kopete.kde.org/>`__ This is a `KDE <http://www.kde.org/>`__ component and although it only works on Linux based system it also supports many of the most popular instant messaging protocols apart from Jabber like: AIM, Gadu-Gadu, ICQ, IRC, MSN, Yahoo.

Install the Jabber client of your choice and set up for a Tigase account:


2.1.3. Configuration instructions for Psi
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Psi - Initial configuration
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

The first time you run Psi you see a screen like this:

|Psi First Run|

To connect to tigase.org server we need to configure the program. Below are step-by-step instructions for novice users on how to setup Psi.

1. Psi can connect to many Jabber servers at the same time so we have to identify each connection somehow. The first thing to do is assign a name to the connection we just created. As we are going to define connection to tigase.org server let’s just name it: **Tigase**.

   |Psi Add Account|

   **Note!** At the moment you can register an account through the Web site only. This is a single account for both services: The Drupal website and Jabber/XMPP service on the tigase.org domain. If you want to have a Jabber account on the tigase.org server go to the registration page, un-tick "Register new account", and go to the point no 5. You can use guide points 2-4 to register a Jabber account on any other Jabber server.

2. When you press the Add button you will see next window where you can enter your Jabber account details:

   |Psi Empty Account|

3. Invent your user name for the account on Tigase server. Let’s assume your user name is: **frank**. Jabber ID’s however consist of 2 parts - your user name and server address. Exactly the same as an e-mail address. As you are registering an account on tigase.org server, you will have to enter in this field: **frank@tigase.org**. Next enter the password of your choice and click the Register button.

   |Psi Register Account|

4. On successful registration you will receive a confirmation message and you should see a window like this:

   |Register Account Success|

   It may happen that somebody earlier registered an account with the same name you’ve selected for yourself. If so, you will receive error message. You will then have to select another user name and try to register again.

5. After clicking the **OK** button you will see a window with your connection and account setup. You can stick with default values for now.

   |PSI After Registration|

   Just click the **Save** button and this window closes.

6. Now you have your account configured and ready to use but you are still off-line. You can find out whether you are on-line or off-line by looking at the bottom of main Psi window. There you can see **Offline** text.

   Click on this **Offline** text and you will see a list of possible options. Just select **Online**.

   |PSI Connected|

   Now you are connected!

Well, you are now connected but how to talk to other people? How to add friends to the contact list? You can send a message to your friends straight away using the **Psi menu** option **New blank message**. It is much more convenient however, if you could see which of your friends is online and available for chatting and if you could start talking to your friend just by clicking on his name.


Short Instructions How to Add Your First Contact
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

1. Click on Psi menu - the button next to the **Online** text. You will see something like this:

   |PSI Menu|

   From all menu options select the top one - Add a contact:

   |PSI Menu add Contact|

2. The next window will display where you can enter your contact details:

   |PSI Add User Empty|

   You have to know the Jabber ID of the person you want to add to your contact list. Let’s assume, for example, you want to add Tigase server administrator’s Jabber ID to your contact list. So, after you enter these details the window will look like this:

   |PSI Add User Filled|

   Click the **Add** button.

3. Now you will see a confirmation window that a new person has been added to your contact list:

   |PSI Kobit Added|

   But there is more behind the scenes. Adding a contact to your **Roster** (contact list) usually means you can see whether the person is online and available to talk or not. The person however, may not wish you to see his presence. So, to make sure the other person accepts you as a friend Psi sent a request to the address you just entered with the question of whether he agrees to show his presence to you.

   You won’t be able to see the users availability until he sends confirmation.

4. Once the other user sends confirmation back, you will usually receive 2 system events:

   |PSI Kobit Auth Received|

5. Click on the contact to see a window with these messages:

   |PSI Authorized Window|

6. One message just says you have been authorized by the other user:

   |PSI Authorized Window 2|

   So you simply click **Next** to see the second message.

7. The second message is a bit more interesting. It contains the question of whether you also authorize the other user to see your presence. If you want to accept this request just click **Add/Auth**.

   |PSI Authorized Window 3|

8. Finally main Psi window with your new contact:

   |PSI Kobit Added Authorized|

Well done!

You are ready to start Jabbering. Good luck.

Where to go next? For detailed Psi documentation refer to the program Wiki page: http://psi-im.org/wiki/Main_Page

Welcome to the Tigase Administration Guide.

.. |Psi First Run| image:: images/user/psi-first-run.png
.. |Psi Add Account| image:: images/user/psi-add-account.png
.. |Psi Empty Account| image:: images/user/psi-register-account-empty.png
.. |Psi Register Account| image:: images/user/psi-register-account-nossl.png
.. |Register Account Success| image:: images/user/psi-register-account-success.png
.. |PSI After Registration| image:: images/user/psi-after-registration.png
.. |PSI Connected| image:: images/user/psi-connected.png
.. |PSI Menu| image:: images/user/psi-menu.png
.. |PSI Menu add Contact| image:: images/user/psi-menu-add-contact.png
.. |PSI Add User Empty| image:: images/user/psi-add-user-empty.png
.. |PSI Add User Filled| image:: images/user/psi-add-user-filled.png
.. |PSI Kobit Added| image:: images/user/psi-kobit-added.png
.. |PSI Kobit Auth Received| image:: images/user/psi-kobit-auth-received.png
.. |PSI Authorized Window| image:: images/user/psi-authorized-window.png
.. |PSI Authorized Window 2| image:: images/user/psi-authorized-window-2.png
.. |PSI Authorized Window 3| image:: images/user/psi-authorized-window-3.png
.. |PSI Kobit Added Authorized| image:: images/user/psi-kobit-added-authorized.png


2.2. About Tigase XMPP Server
-----------------------------

**Tigase XMPP Server** is an **Open Source and Free (AGPLv3)** Java based server. The goals behind its design and implementation of the server are:

1. Make the server robust and reliable.

2. Make the server a secure communication platform.

3. Make a flexible server which can be applied to different use cases.

4. Make an extensible server which takes full advantage of XMPP protocol extensibility.

5. Make the server easy to setup and maintain.

2.2.1. Robust and reliable
^^^^^^^^^^^^^^^^^^^^^^^^^^

This means that the server can handle many concurrent requests/connections and can run for a long time reliably. The server is designed and implemented to handle millions of simultaneous connections.

It is not enough however to design and implement a high load server and hope it will run well. The main focus of the project is put in into testing. Tests are taken so seriously that a dedicated testing framework has been implemented. All server functions are considered as implemented only when they pass a rigorous testing cycle. The testing cycle consists of 3 fundamental tests:

1. **Functional tests** - Checking whether the function works at all.

2. **Performance tests** - Checking whether the function performs well enough.

3. **Stability tests** - Checking whether the function behaves well in long term run. It must handle hundreds of requests a second in a several hour server run.


2.2.2. Security
^^^^^^^^^^^^^^^^

There are a few elements of the security related to XMPP servers: secure data transmissions which is met by the implementation of **SSL** or **TLS** protocol, secure user authorization which is met by the implementation of **DIGEST** or **SASL** user authorization and secure deployment which is met by component architecture.

**Secure deployment** Tigase software installation does not impact network security. Companies usually have their networks divided into 2 parts: **DMZ** which is partially open to the outside world and the **Private network** which is closed to the outside world.

If the XMPP server is to provide an effective way of communication between company employees regardless if they are in a secure company office or outside (perhaps at a customer site), it needs to accept both internal and external connections. So the natural location for the server deployment is the **DMZ**. However, this solution has some considerations: each company has normally established network users base and integrated authorization mechanisms. However, that information should be stored outside the DMZ to protect internal security, so how to maintain ease of installation and system security?

**Tigase server** offers a solution for such a case. With it’s component structure, Tigase can be easily deployed on any number machines and from the user’s point of view it is seen as a one logical XMPP server. In this case we can install a Session Manager module in the **private** network, and a Client Connection Manager with Server Connection Manager in the **DMZ**.

Session Manager connects to **DMZ** and receives all packets from external users. Thus is can securely realize users authorization based on company authorization mechanisms.


2.2.3. Flexibility
^^^^^^^^^^^^^^^^^^
There are many different XMPP server implementations. The most prevalent are:

-  Used as a business communication platform in small and medium companies where the server is not under a heavy load. For such deployments security is a key feature.

-  For huge community websites or internet portal servers is, on the other hand, usually under very heavy load and has to support thousands or millions of simultaneous connections. For such a deployment we need a different level of security as most of the service is open to the public.

-  For very small community deployments or for small home networks the key factor is ease to deploy and maintain.

Architecture based on components provides the ability to run selected modules on separate machines so the server can be easily applied in any scenario.

For simple installation the server generates a config file which can be used straight away with very few modifications or none at all. For complex deployments though, you can tweak configurations to your needs and setup XMPP server on as many physical machines as you need.

2.2.4. Extensibility
^^^^^^^^^^^^^^^^^^^^^

The world changes all the time as does user’s needs. The XMPP protocol has been designed to be extensible to make it easy to add new features and apply it to those different user’s needs. As a result, XMPP is a very effective platform not only for sending messages to other users, it can also be extended for sending instant notifications about events, a useful platform for on-line customer service, voice communication, and other cases where sending information instantly to other people is needed.

**Tigase server** has been designed to be extensible using a modular architecture. You can easily replace components which do not fulfill your requirements with others better fitting your needs. But that is not all, another factor of extensibility is how easy is to replace or add new extensions. A great deal of focus has been put into the server design API to make it easy for other software developers to create extensions and implement new features.


2.2.5. Ease of Use
^^^^^^^^^^^^^^^^^^^

Complex computer networks consisting of many servers with different services are hard to maintain. This requires employing professional staff to operate and maintain the network.

Not all networks are so complex however, most small companies have just a few servers for their needs with services like e-mail and a HTTP server. They might want to add an XMPP server to the collection of their services and don’t want to dedicate resources on setup and maintenance. For such users our default configuration is exactly what they need. If the operating system on the server is well configured, then Tigase should automatically pickup the correct hostname and be ready to operate immediately.

Tigase server is designed and implemented to allow dynamic reconfiguration during runtime so there is no need to restart the server each time you want to change configuration settings.

There are also interfaces and handlers available to make it easy to implement a web user interface for server monitoring and configuring.

2.2.6. XMPP Supported Extensions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Based on `XEP-0387: XMPP Compliance Suites 2018 <https://xmpp.org/extensions/xep-0387.html>`__


Core Compliance Suite
~~~~~~~~~~~~~~~~~~~~~~

.. table:: Table 1.Core Compliance Suite
   :widths: grid

   +---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+-----------------------------------------------------------+
   | Support | Specification                                            | Name                                                                                           | Comment                                                   |
   +---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+-----------------------------------------------------------+
   | ✓       | `RFC6120 <https://tools.ietf.org/html/rfc6120>`__        | Extensible Messaging and Presence Protocol (XMPP): Core                                        |                                                           |
   +---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+-----------------------------------------------------------+
   | ⍻       | `RFC7622 <https://tools.ietf.org/html/rfc7622>`__        | Extensible Messaging and Presence Protocol (XMPP): Address Format                              | We support previous version of the specification: RFC6122 |
   +---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+-----------------------------------------------------------+
   | ✓       | `RFC7590 <https://tools.ietf.org/html/rfc7590>`__        | Use of Transport Layer Security (TLS) in the Extensible Messaging and Presence Protocol (XMPP) |                                                           |
   +---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+-----------------------------------------------------------+
   | ✓       | `XEP-0368 <https://xmpp.org/extensions/xep-0368.html>`__ | SRV records for XMPP over TLS                                                                  | Requires adding DNS entries pointing to port 5223         |
   +---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+-----------------------------------------------------------+
   | ✓       | `XEP-0030 <https://xmpp.org/extensions/xep-0030.html>`__ | Service Discovery                                                                              |                                                           |
   +---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+-----------------------------------------------------------+
   | ✓       | `XEP-0115 <https://xmpp.org/extensions/xep-0115.html>`__ | Entity Capabilities                                                                            |                                                           |
   +---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+-----------------------------------------------------------+
   | ✓       | `XEP-0114 <https://xmpp.org/extensions/xep-0114.html>`__ | Jabber Component Protocol                                                                      |                                                           |
   +---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+-----------------------------------------------------------+
   | ✓       | `XEP-0163 <https://xmpp.org/extensions/xep-0163.html>`__ | Personal Eventing Protocol                                                                     |                                                           |
   +---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+-----------------------------------------------------------+

Web Compliance Suite
~~~~~~~~~~~~~~~~~~~~~

.. table:: Table 2.Web Compliance Suite

   +---------+----------------------------------------------------------+--------------------------------------------------------------------------------+---------+
   | Support | Specification                                            | Name                                                                           | Comment |
   +---------+----------------------------------------------------------+--------------------------------------------------------------------------------+---------+
   | ✓       | `RFC7395 <https://tools.ietf.org/html/rfc7395>`__        | An Extensible Messaging and Presence Protocol (XMPP) Subprotocol for WebSocket |         |
   +---------+----------------------------------------------------------+--------------------------------------------------------------------------------+---------+
   | ✓       | `XEP-0206 <https://xmpp.org/extensions/xep-0206.html>`__ | XMPP Over BOSH                                                                 |         |
   +---------+----------------------------------------------------------+--------------------------------------------------------------------------------+---------+
   | ✓       | `XEP-0124 <https://xmpp.org/extensions/xep-0124.html>`__ | Bidirectional-streams Over Synchronous HTTP (BOSH)                             |         |
   +---------+----------------------------------------------------------+--------------------------------------------------------------------------------+---------+

IM Compliance Suite
~~~~~~~~~~~~~~~~~~~~~

.. table:: Table 3.Web Compliance Suite

   +---------+----------------------------------------------------------+-----------------------------------------------------------------------------------+-------------------------------------------------------------+
   | Support | Specification                                            | Name                                                                              | Comment                                                     |
   +---------+----------------------------------------------------------+-----------------------------------------------------------------------------------+-------------------------------------------------------------+
   | ✓       | `RFC6120 <https://tools.ietf.org/html/rfc6120>`__        | Extensible Messaging and Presence Protocol (XMPP): Instant Messaging and Presence |                                                             |
   +---------+----------------------------------------------------------+-----------------------------------------------------------------------------------+-------------------------------------------------------------+
   | ✓       | `XEP-0084 <https://xmpp.org/extensions/xep-0084.html>`__ | User Avatar                                                                       |                                                             |
   +---------+----------------------------------------------------------+-----------------------------------------------------------------------------------+-------------------------------------------------------------+
   | ✓       | `XEP-0153 <https://xmpp.org/extensions/xep-0153.html>`__ | vCard-Based Avatars                                                               |                                                             |
   +---------+----------------------------------------------------------+-----------------------------------------------------------------------------------+-------------------------------------------------------------+
   | ✓       | `XEP-0054 <https://xmpp.org/extensions/xep-0054.html>`__ | vcard-temp                                                                        |                                                             |
   +---------+----------------------------------------------------------+-----------------------------------------------------------------------------------+-------------------------------------------------------------+
   | ✓       | `XEP-0280 <https://xmpp.org/extensions/xep-0280.html>`__ | Message Carbons                                                                   |                                                             |
   +---------+----------------------------------------------------------+-----------------------------------------------------------------------------------+-------------------------------------------------------------+
   | ✓       | `XEP-0191 <https://xmpp.org/extensions/xep-0191.html>`__ | Blocking Command                                                                  |                                                             |
   +---------+----------------------------------------------------------+-----------------------------------------------------------------------------------+-------------------------------------------------------------+
   | ✓       | `XEP-0045 <https://xmpp.org/extensions/xep-0045.html>`__ | Multi-User Chat                                                                   |                                                             |
   +---------+----------------------------------------------------------+-----------------------------------------------------------------------------------+-------------------------------------------------------------+
   | ✓       | `XEP-0249 <https://xmpp.org/extensions/xep-0249.html>`__ | Direct MUC Invitations                                                            |                                                             |
   +---------+----------------------------------------------------------+-----------------------------------------------------------------------------------+-------------------------------------------------------------+
   | ✓       | `XEP-0048 <https://xmpp.org/extensions/xep-0048.html>`__ | Bookmarks                                                                         |                                                             |
   +---------+----------------------------------------------------------+-----------------------------------------------------------------------------------+-------------------------------------------------------------+
   | ✓       | `XEP-0223 <https://xmpp.org/extensions/xep-0223.html>`__ | Persistent Storage of Private Data via PubSub                                     |                                                             |
   +---------+----------------------------------------------------------+-----------------------------------------------------------------------------------+-------------------------------------------------------------+
   | ✓       | `XEP-0049 <https://xmpp.org/extensions/xep-0049.html>`__ | Private XML Storage                                                               |                                                             |
   +---------+----------------------------------------------------------+-----------------------------------------------------------------------------------+-------------------------------------------------------------+
   | ✓       | `XEP-0198 <https://xmpp.org/extensions/xep-0198.html>`__ | Stream Management                                                                 | Both ``Session Resumption`` and ``Stanza Acknowledgements`` |
   +---------+----------------------------------------------------------+-----------------------------------------------------------------------------------+-------------------------------------------------------------+
   | ✓       | `XEP-0313 <https://xmpp.org/extensions/xep-0313.html>`__ | Message Archive Management                                                        |                                                             |
   +---------+----------------------------------------------------------+-----------------------------------------------------------------------------------+-------------------------------------------------------------+

Mobile Compliance Suite
~~~~~~~~~~~~~~~~~~~~~~~~

.. table:: Table 4.Web Compliance Suite

   +---------+----------------------------------------------------------+--------------------------------------------------------------------------------+-------------------------------------------------------------+
   | Support | Specification                                            | Name                                                                           | Comment                                                     |
   +---------+----------------------------------------------------------+--------------------------------------------------------------------------------+-------------------------------------------------------------+
   | ✓       | `RFC7395 <https://tools.ietf.org/html/rfc7395>`__        | An Extensible Messaging and Presence Protocol (XMPP) Subprotocol for WebSocket |                                                             |
   +---------+----------------------------------------------------------+--------------------------------------------------------------------------------+-------------------------------------------------------------+
   | ✓       | `XEP-0198 <https://xmpp.org/extensions/xep-0198.html>`__ | Stream Management                                                              | Both ``Session Resumption`` and ``Stanza Acknowledgements`` |
   +---------+----------------------------------------------------------+--------------------------------------------------------------------------------+-------------------------------------------------------------+
   | ✓       | `XEP-0352 <https://xmpp.org/extensions/xep-0352.html>`__ | Client State Indication                                                        |                                                             |
   +---------+----------------------------------------------------------+--------------------------------------------------------------------------------+-------------------------------------------------------------+
   | ✓       | `XEP-0357 <https://xmpp.org/extensions/xep-0357.html>`__ | Push Notifications                                                             |                                                             |
   +---------+----------------------------------------------------------+--------------------------------------------------------------------------------+-------------------------------------------------------------+

Non-Compliance Suite Extensions
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. table:: Table 5.Core Compliance Suite

   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | Support | Specification                                            | Name                                                      | Comment                                                      |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0004 <https://xmpp.org/extensions/xep-0004.html>`__ | Data Forms                                                |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0008 <https://xmpp.org/extensions/xep-0004.html>`__ | IQ-Based Avatars                                          |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0012 <https://xmpp.org/extensions/xep-0012.html>`__ | Last Activity                                             |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0013 <https://xmpp.org/extensions/xep-0013.html>`__ | Flexible Offline Message Retrieval                        |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0016 <https://xmpp.org/extensions/xep-0016.html>`__ | Privacy Lists                                             |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0020 <https://xmpp.org/extensions/xep-0020.html>`__ | Feature Negotiation                                       |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0022 <https://xmpp.org/extensions/xep-0022.html>`__ | Message Events                                            |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0047 <https://xmpp.org/extensions/xep-0047.html>`__ | In-Band Bytestreams                                       |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0050 <https://xmpp.org/extensions/xep-0050.html>`__ | Ad-Hoc Commands                                           |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0059 <https://xmpp.org/extensions/xep-0059.html>`__ | Result Set Management                                     |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0060 <https://xmpp.org/extensions/xep-0060.html>`__ | Publish-Subscribe                                         |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0065 <https://xmpp.org/extensions/xep-0065.html>`__ | SOCKS5 Bytestreams                                        |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0066 <https://xmpp.org/extensions/xep-0066.html>`__ | Out of Band Data                                          |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0068 <https://xmpp.org/extensions/xep-0068.html>`__ | Field Standardization for Data Forms                      |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0071 <https://xmpp.org/extensions/xep-0071.html>`__ | XHTML-IM                                                  |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0072 <https://xmpp.org/extensions/xep-0072.html>`__ | SOAP Over XMPP                                            |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0077 <https://xmpp.org/extensions/xep-0077.html>`__ | In-Band Registration                                      |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0078 <https://xmpp.org/extensions/xep-0078.html>`__ | Non-SASL Authentication                                   |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0079 <https://xmpp.org/extensions/xep-0079.html>`__ | Advanced Message Processing                               |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0080 <https://xmpp.org/extensions/xep-0080.html>`__ | User Location                                             |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0082 <https://xmpp.org/extensions/xep-0082.html>`__ | XMPP Date and Time Profiles                               |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0083 <https://xmpp.org/extensions/xep-0083.html>`__ | Nested Roster Groups                                      |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0085 <https://xmpp.org/extensions/xep-0085.html>`__ | Chat State Notifications                                  |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0086 <https://xmpp.org/extensions/xep-0086.html>`__ | Error Condition Mappings                                  |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0091 <https://xmpp.org/extensions/xep-0091.html>`__ | Legacy Delayed Delivery                                   |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0092 <https://xmpp.org/extensions/xep-0092.html>`__ | Software Version                                          |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0096 <https://xmpp.org/extensions/xep-0096.html>`__ | File Transfer                                             |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0100 <https://xmpp.org/extensions/xep-0100.html>`__ | Gateway Interaction                                       |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0106 <https://xmpp.org/extensions/xep-0106.html>`__ | JID Escaping                                              |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0107 <https://xmpp.org/extensions/xep-0107.html>`__ | User Mood                                                 | Server support via ``Personal Eventing Protocol (XEP-0163)`` |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0108 <https://xmpp.org/extensions/xep-0108.html>`__ | User Activity                                             | Server support via ``Personal Eventing Protocol (XEP-0163)`` |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0118 <https://xmpp.org/extensions/xep-0118.html>`__ | User Tune                                                 | Server support via ``Personal Eventing Protocol (XEP-0163)`` |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0127 <https://xmpp.org/extensions/xep-0127.html>`__ | Common Alerting Protocol (CAP) Over XMPP                  |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0128 <https://xmpp.org/extensions/xep-0128.html>`__ | Service Discovery Extensions                              |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0131 <https://xmpp.org/extensions/xep-0131.html>`__ | Stanza Headers and Internet Metadata (SHIM)               |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0133 <https://xmpp.org/extensions/xep-0133.html>`__ | Service Administration                                    |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0136 <https://xmpp.org/extensions/xep-0136.html>`__ | Message Archiving                                         |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0141 <https://xmpp.org/extensions/xep-0141.html>`__ | Data Forms Layout                                         |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓ [1]_  | `XEP-0142 <https://xmpp.org/extensions/xep-0142.html>`__ | Workgroup Queues                                          |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0144 <https://xmpp.org/extensions/xep-0144.html>`__ | Roster Item Exchange                                      |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0145 <https://xmpp.org/extensions/xep-0145.html>`__ | Annotations                                               |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0146 <https://xmpp.org/extensions/xep-0146.html>`__ | Remote Controlling Clients                                |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0152 <https://xmpp.org/extensions/xep-0152.html>`__ | Reachability Addresses                                    |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0155 <https://xmpp.org/extensions/xep-0155.html>`__ | Stanza Session Negotiation                                |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0156 <https://xmpp.org/extensions/xep-0156.html>`__ | Discovering Alternative XMPP Connection Methods           | Uses DNS records, so will work with Tigase XMPP Server       |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0157 <https://xmpp.org/extensions/xep-0157.html>`__ | Contact Addresses for XMPP Services                       |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0160 <https://xmpp.org/extensions/xep-0160.html>`__ | Best Practices for Handling Offline Messages              |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0166 <https://xmpp.org/extensions/xep-0166.html>`__ | Jingle                                                    |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0167 <https://xmpp.org/extensions/xep-0167.html>`__ | Jingle RTP Sessions                                       |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0170 <https://xmpp.org/extensions/xep-0170.html>`__ | Recommended Order of Stream Feature Negotiation           |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0171 <https://xmpp.org/extensions/xep-0171.html>`__ | Language Translation                                      |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0172 <https://xmpp.org/extensions/xep-0172.html>`__ | User Nickname                                             |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0174 <https://xmpp.org/extensions/xep-0174.html>`__ | Serverless Messaging                                      |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0175 <https://xmpp.org/extensions/xep-0175.html>`__ | Best Practices for Use of SASL ANONYMOUS                  |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0176 <https://xmpp.org/extensions/xep-0176.html>`__ | Jingle ICE-UDP Transport Method                           |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0177 <https://xmpp.org/extensions/xep-0177.html>`__ | Jingle Raw UDP Transport Method                           |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0178 <https://xmpp.org/extensions/xep-0178.html>`__ | Best Practices for Use of SASL EXTERNAL with Certificates |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0179 <https://xmpp.org/extensions/xep-0179.html>`__ | Jingle IAX Transport Method                               |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0180 <https://xmpp.org/extensions/xep-0180.html>`__ | Jingle Video via RTP                                      |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0181 <https://xmpp.org/extensions/xep-0181.html>`__ | Jingle DTMF                                               |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0184 <https://xmpp.org/extensions/xep-0184.html>`__ | Message Receipts                                          |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0185 <https://xmpp.org/extensions/xep-0185.html>`__ | Dialback Key Generation and Validation                    |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0190 <https://xmpp.org/extensions/xep-0190.html>`__ | Best Practice for Closing Idle Streams                    |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0199 <https://xmpp.org/extensions/xep-0199.html>`__ | XMPP Ping                                                 |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0201 <https://xmpp.org/extensions/xep-0201.html>`__ | Best Practices for Message Threads                        |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0202 <https://xmpp.org/extensions/xep-0202.html>`__ | Entity Time                                               |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0203 <https://xmpp.org/extensions/xep-0203.html>`__ | Delayed Delivery                                          |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0205 <https://xmpp.org/extensions/xep-0205.html>`__ | Best Practices to Discourage Denial of Service Attacks    |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0209 <https://xmpp.org/extensions/xep-0209.html>`__ | Metacontacts                                              |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0220 <https://xmpp.org/extensions/xep-0220.html>`__ | Server Dialback                                           |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0224 <https://xmpp.org/extensions/xep-0224.html>`__ | Attention                                                 |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0225 <https://xmpp.org/extensions/xep-0225.html>`__ | Component Connections                                     |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0226 <https://xmpp.org/extensions/xep-0226.html>`__ | Message Stanza Profiles                                   |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0231 <https://xmpp.org/extensions/xep-0231.html>`__ | Bits of Binary                                            |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0234 <https://xmpp.org/extensions/xep-0234.html>`__ | Jingle File Transfer                                      |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0245 <https://xmpp.org/extensions/xep-0245.html>`__ | The /me Command                                           |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0246 <https://xmpp.org/extensions/xep-0246.html>`__ | End-to-End XML Streams                                    |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0247 <https://xmpp.org/extensions/xep-0247.html>`__ | Jingle XML Streams                                        |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0250 <https://xmpp.org/extensions/xep-0250.html>`__ | C2C Authentication Using TLS                              |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0251 <https://xmpp.org/extensions/xep-0251.html>`__ | Jingle Session Transfer                                   |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0260 <https://xmpp.org/extensions/xep-0260.html>`__ | Jingle SOCKS5 Bytestreams Transport Method                |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0261 <https://xmpp.org/extensions/xep-0261.html>`__ | Jingle In-Band Bytestreams Transport                      |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0262 <https://xmpp.org/extensions/xep-0262.html>`__ | Use of ZRTP in Jingle RTP Sessions                        |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0277 <https://xmpp.org/extensions/xep-0277.html>`__ | Microblogging over XMPP                                   |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0292 <https://xmpp.org/extensions/xep-0292.html>`__ | vCard4 Over XMPP                                          |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0301 <https://xmpp.org/extensions/xep-0301.html>`__ | In-Band Real Time Text                                    |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0305 <https://xmpp.org/extensions/xep-0305.html>`__ | XMPP Quickstart                                           |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0323 <https://xmpp.org/extensions/xep-0323.html>`__ | Internet of Things - Sensor Data                          |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0324 <https://xmpp.org/extensions/xep-0324.html>`__ | Internet of Things - Provisioning                         |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0325 <https://xmpp.org/extensions/xep-0325.html>`__ | Internet of Things - Control                              |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0326 <https://xmpp.org/extensions/xep-0326.html>`__ | Internet of Things - Concentrators                        |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0333 <https://xmpp.org/extensions/xep-0333.html>`__ | Chat Markers                                              |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0363 <https://xmpp.org/extensions/xep-0363.html>`__ | HTTP File Upload                                          |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+
   | ✓       | `XEP-0387 <https://xmpp.org/extensions/xep-0387.html>`__ | XMPP Compliance Suites 2018                               |                                                              |
   +---------+----------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------+

Full, ordered list of supported RFCs and XEPs:
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| Support | Specification                                            | Name                                                                                           | Comment                                                      |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `RFC6120 <https://tools.ietf.org/html/rfc6120>`__        | Extensible Messaging and Presence Protocol (XMPP): Core                                        |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `RFC6120 <https://tools.ietf.org/html/rfc6120>`__        | Extensible Messaging and Presence Protocol (XMPP): Instant Messaging and Presence              |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ⍻       | `RFC7622 <https://tools.ietf.org/html/rfc7622>`__        | Extensible Messaging and Presence Protocol (XMPP): Address Format                              | We support previous version of the specification: RFC6122    |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `RFC7395 <https://tools.ietf.org/html/rfc7395>`__        | An Extensible Messaging and Presence Protocol (XMPP) Subprotocol for WebSocket                 |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `RFC7395 <https://tools.ietf.org/html/rfc7395>`__        | An Extensible Messaging and Presence Protocol (XMPP) Subprotocol for WebSocket                 |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `RFC7590 <https://tools.ietf.org/html/rfc7590>`__        | Use of Transport Layer Security (TLS) in the Extensible Messaging and Presence Protocol (XMPP) |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0004 <https://xmpp.org/extensions/xep-0004.html>`__ | Data Forms                                                                                     |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0008 <https://xmpp.org/extensions/xep-0004.html>`__ | IQ-Based Avatars                                                                               |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0012 <https://xmpp.org/extensions/xep-0012.html>`__ | Last Activity                                                                                  |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0013 <https://xmpp.org/extensions/xep-0013.html>`__ | Flexible Offline Message Retrieval                                                             |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0016 <https://xmpp.org/extensions/xep-0016.html>`__ | Privacy Lists                                                                                  |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0020 <https://xmpp.org/extensions/xep-0020.html>`__ | Feature Negotiation                                                                            |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0022 <https://xmpp.org/extensions/xep-0022.html>`__ | Message Events                                                                                 |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0030 <https://xmpp.org/extensions/xep-0030.html>`__ | Service Discovery                                                                              |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0045 <https://xmpp.org/extensions/xep-0045.html>`__ | Multi-User Chat                                                                                |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0047 <https://xmpp.org/extensions/xep-0047.html>`__ | In-Band Bytestreams                                                                            |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0048 <https://xmpp.org/extensions/xep-0048.html>`__ | Bookmarks                                                                                      |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0049 <https://xmpp.org/extensions/xep-0049.html>`__ | Private XML Storage                                                                            |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0050 <https://xmpp.org/extensions/xep-0050.html>`__ | Ad-Hoc Commands                                                                                |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0054 <https://xmpp.org/extensions/xep-0054.html>`__ | vcard-temp                                                                                     |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0059 <https://xmpp.org/extensions/xep-0059.html>`__ | Result Set Management                                                                          |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0060 <https://xmpp.org/extensions/xep-0060.html>`__ | Publish-Subscribe                                                                              |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0065 <https://xmpp.org/extensions/xep-0065.html>`__ | SOCKS5 Bytestreams                                                                             |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0066 <https://xmpp.org/extensions/xep-0066.html>`__ | Out of Band Data                                                                               |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0068 <https://xmpp.org/extensions/xep-0068.html>`__ | Field Standardization for Data Forms                                                           |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0071 <https://xmpp.org/extensions/xep-0071.html>`__ | XHTML-IM                                                                                       |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0072 <https://xmpp.org/extensions/xep-0072.html>`__ | SOAP Over XMPP                                                                                 |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0077 <https://xmpp.org/extensions/xep-0077.html>`__ | In-Band Registration                                                                           |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0078 <https://xmpp.org/extensions/xep-0078.html>`__ | Non-SASL Authentication                                                                        |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0079 <https://xmpp.org/extensions/xep-0079.html>`__ | Advanced Message Processing                                                                    |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0080 <https://xmpp.org/extensions/xep-0080.html>`__ | User Location                                                                                  |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0082 <https://xmpp.org/extensions/xep-0082.html>`__ | XMPP Date and Time Profiles                                                                    |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0083 <https://xmpp.org/extensions/xep-0083.html>`__ | Nested Roster Groups                                                                           |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0084 <https://xmpp.org/extensions/xep-0084.html>`__ | User Avatar                                                                                    |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0085 <https://xmpp.org/extensions/xep-0085.html>`__ | Chat State Notifications                                                                       |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0086 <https://xmpp.org/extensions/xep-0086.html>`__ | Error Condition Mappings                                                                       |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0091 <https://xmpp.org/extensions/xep-0091.html>`__ | Legacy Delayed Delivery                                                                        |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0092 <https://xmpp.org/extensions/xep-0092.html>`__ | Software Version                                                                               |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0096 <https://xmpp.org/extensions/xep-0096.html>`__ | File Transfer                                                                                  |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0100 <https://xmpp.org/extensions/xep-0100.html>`__ | Gateway Interaction                                                                            |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0106 <https://xmpp.org/extensions/xep-0106.html>`__ | JID Escaping                                                                                   |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0107 <https://xmpp.org/extensions/xep-0107.html>`__ | User Mood                                                                                      | Server support via ``Personal Eventing Protocol (XEP-0163)`` |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0108 <https://xmpp.org/extensions/xep-0108.html>`__ | User Activity                                                                                  | Server support via ``Personal Eventing Protocol (XEP-0163)`` |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0114 <https://xmpp.org/extensions/xep-0114.html>`__ | Jabber Component Protocol                                                                      |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0115 <https://xmpp.org/extensions/xep-0115.html>`__ | Entity Capabilities                                                                            |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0118 <https://xmpp.org/extensions/xep-0118.html>`__ | User Tune                                                                                      | Server support via ``Personal Eventing Protocol (XEP-0163)`` |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0124 <https://xmpp.org/extensions/xep-0124.html>`__ | Bidirectional-streams Over Synchronous HTTP (BOSH)                                             |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0128 <https://xmpp.org/extensions/xep-0128.html>`__ | Service Discovery Extensions                                                                   |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0127 <https://xmpp.org/extensions/xep-0127.html>`__ | Common Alerting Protocol (CAP) Over XMPP                                                       |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0131 <https://xmpp.org/extensions/xep-0131.html>`__ | Stanza Headers and Internet Metadata (SHIM)                                                    |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0133 <https://xmpp.org/extensions/xep-0133.html>`__ | Service Administration                                                                         |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0136 <https://xmpp.org/extensions/xep-0136.html>`__ | Message Archiving                                                                              |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0141 <https://xmpp.org/extensions/xep-0141.html>`__ | Data Forms Layout                                                                              |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0142 <https://xmpp.org/extensions/xep-0142.html>`__ | Workgroup Queues                                                                               |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0144 <https://xmpp.org/extensions/xep-0144.html>`__ | Roster Item Exchange                                                                           |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0145 <https://xmpp.org/extensions/xep-0145.html>`__ | Annotations                                                                                    |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0146 <https://xmpp.org/extensions/xep-0146.html>`__ | Remote Controlling Clients                                                                     |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0152 <https://xmpp.org/extensions/xep-0152.html>`__ | Reachability Addresses                                                                         |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0153 <https://xmpp.org/extensions/xep-0153.html>`__ | vCard-Based Avatars                                                                            |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0155 <https://xmpp.org/extensions/xep-0155.html>`__ | Stanza Session Negotiation                                                                     |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0156 <https://xmpp.org/extensions/xep-0156.html>`__ | Discovering Alternative XMPP Connection Methods                                                | Uses DNS records, so will work with Tigase XMPP Server       |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0157 <https://xmpp.org/extensions/xep-0157.html>`__ | Contact Addresses for XMPP Services                                                            |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0160 <https://xmpp.org/extensions/xep-0160.html>`__ | Best Practices for Handling Offline Messages                                                   |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0163 <https://xmpp.org/extensions/xep-0163.html>`__ | Personal Eventing Protocol                                                                     |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0166 <https://xmpp.org/extensions/xep-0166.html>`__ | Jingle                                                                                         |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0167 <https://xmpp.org/extensions/xep-0167.html>`__ | Jingle RTP Sessions                                                                            |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0170 <https://xmpp.org/extensions/xep-0170.html>`__ | Recommended Order of Stream Feature Negotiation                                                |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0171 <https://xmpp.org/extensions/xep-0171.html>`__ | Language Translation                                                                           |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0172 <https://xmpp.org/extensions/xep-0172.html>`__ | User Nickname                                                                                  |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0174 <https://xmpp.org/extensions/xep-0174.html>`__ | Serverless Messaging                                                                           |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0175 <https://xmpp.org/extensions/xep-0175.html>`__ | Best Practices for Use of SASL ANONYMOUS                                                       |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0176 <https://xmpp.org/extensions/xep-0176.html>`__ | Jingle ICE-UDP Transport Method                                                                |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0177 <https://xmpp.org/extensions/xep-0177.html>`__ | Jingle Raw UDP Transport Method                                                                |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0178 <https://xmpp.org/extensions/xep-0178.html>`__ | Best Practices for Use of SASL EXTERNAL with Certificates                                      |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0179 <https://xmpp.org/extensions/xep-0179.html>`__ | Jingle IAX Transport Method                                                                    |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0180 <https://xmpp.org/extensions/xep-0180.html>`__ | Jingle Video via RTP                                                                           |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0181 <https://xmpp.org/extensions/xep-0181.html>`__ | Jingle DTMF                                                                                    |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0184 <https://xmpp.org/extensions/xep-0184.html>`__ | Message Receipts                                                                               |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0185 <https://xmpp.org/extensions/xep-0185.html>`__ | Dialback Key Generation and Validation                                                         |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0190 <https://xmpp.org/extensions/xep-0190.html>`__ | Best Practice for Closing Idle Streams                                                         |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0191 <https://xmpp.org/extensions/xep-0191.html>`__ | Blocking Command                                                                               |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0198 <https://xmpp.org/extensions/xep-0198.html>`__ | Stream Management                                                                              | Both ``Session Resumption`` and ``Stanza Acknowledgements``  |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0199 <https://xmpp.org/extensions/xep-0199.html>`__ | XMPP Ping                                                                                      |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0201 <https://xmpp.org/extensions/xep-0201.html>`__ | Best Practices for Message Threads                                                             |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0202 <https://xmpp.org/extensions/xep-0202.html>`__ | Entity Time                                                                                    |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0203 <https://xmpp.org/extensions/xep-0203.html>`__ | Delayed Delivery                                                                               |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0205 <https://xmpp.org/extensions/xep-0205.html>`__ | Best Practices to Discourage Denial of Service Attacks                                         |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0206 <https://xmpp.org/extensions/xep-0206.html>`__ | XMPP Over BOSH                                                                                 |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0209 <https://xmpp.org/extensions/xep-0209.html>`__ | Metacontacts                                                                                   |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0220 <https://xmpp.org/extensions/xep-0220.html>`__ | Server Dialback                                                                                |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0223 <https://xmpp.org/extensions/xep-0223.html>`__ | Persistent Storage of Private Data via PubSub                                                  |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0224 <https://xmpp.org/extensions/xep-0224.html>`__ | Attention                                                                                      |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0225 <https://xmpp.org/extensions/xep-0225.html>`__ | Component Connections                                                                          |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0226 <https://xmpp.org/extensions/xep-0226.html>`__ | Message Stanza Profiles                                                                        |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0231 <https://xmpp.org/extensions/xep-0231.html>`__ | Bits of Binary                                                                                 |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0234 <https://xmpp.org/extensions/xep-0234.html>`__ | Jingle File Transfer                                                                           |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0245 <https://xmpp.org/extensions/xep-0245.html>`__ | The /me Command                                                                                |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0246 <https://xmpp.org/extensions/xep-0246.html>`__ | End-to-End XML Streams                                                                         |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0247 <https://xmpp.org/extensions/xep-0247.html>`__ | Jingle XML Streams                                                                             |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0249 <https://xmpp.org/extensions/xep-0249.html>`__ | Direct MUC Invitations                                                                         |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0250 <https://xmpp.org/extensions/xep-0250.html>`__ | C2C Authentication Using TLS                                                                   |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0251 <https://xmpp.org/extensions/xep-0251.html>`__ | Jingle Session Transfer                                                                        |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0260 <https://xmpp.org/extensions/xep-0260.html>`__ | Jingle SOCKS5 Bytestreams Transport Method                                                     |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0261 <https://xmpp.org/extensions/xep-0261.html>`__ | Jingle In-Band Bytestreams Transport                                                           |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0262 <https://xmpp.org/extensions/xep-0262.html>`__ | Use of ZRTP in Jingle RTP Sessions                                                             |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0277 <https://xmpp.org/extensions/xep-0277.html>`__ | Microblogging over XMPP                                                                        |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0280 <https://xmpp.org/extensions/xep-0280.html>`__ | Message Carbons                                                                                |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0292 <https://xmpp.org/extensions/xep-0292.html>`__ | vCard4 Over XMPP                                                                               |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0301 <https://xmpp.org/extensions/xep-0301.html>`__ | In-Band Real Time Text                                                                         |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0305 <https://xmpp.org/extensions/xep-0305.html>`__ | XMPP Quickstart                                                                                |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0313 <https://xmpp.org/extensions/xep-0313.html>`__ | Message Archive Management                                                                     |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0323 <https://xmpp.org/extensions/xep-0323.html>`__ | Internet of Things - Sensor Data                                                               |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0324 <https://xmpp.org/extensions/xep-0324.html>`__ | Internet of Things - Provisioning                                                              |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0325 <https://xmpp.org/extensions/xep-0325.html>`__ | Internet of Things - Control                                                                   |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0326 <https://xmpp.org/extensions/xep-0326.html>`__ | Internet of Things - Concentrators                                                             |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0333 <https://xmpp.org/extensions/xep-0333.html>`__ | Chat Markers                                                                                   |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0352 <https://xmpp.org/extensions/xep-0352.html>`__ | Client State Indication                                                                        |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0357 <https://xmpp.org/extensions/xep-0357.html>`__ | Push Notifications                                                                             |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0363 <https://xmpp.org/extensions/xep-0363.html>`__ | HTTP File Upload                                                                               |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0368 <https://xmpp.org/extensions/xep-0368.html>`__ | SRV records for XMPP over TLS                                                                  | Requires adding DNS entries pointing to port 5223            |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+
| ✓       | `XEP-0387 <https://xmpp.org/extensions/xep-0387.html>`__ | XMPP Compliance Suites 2018                                                                    |                                                              |
+---------+----------------------------------------------------------+------------------------------------------------------------------------------------------------+--------------------------------------------------------------+

.. [1]
   Requires commercial license

2.2.7. Tigase Custom Extensions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

General features
~~~~~~~~~~~~~~~~~

.. table:: tabel 6.Monitoring

   +---------+--------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | Support | Name                           | Comment                                                                                                                                                                           |
   +---------+--------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | ✓ [1]_  | AuditLog                       | Ability functionality to log important events in a system (loggins, message exchanges, calls)                                                                                     |
   +---------+--------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | ✓       | Anti Abuse                     | Fight stanza SPAM, DoS, brute-force attacks and other threats                                                                                                                     |
   +---------+--------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | ✓       | Virtual domains                | Ability to create and manage multiple virtual domains from a single instance and restart-less management                                                                          |
   +---------+--------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | ✓       | MUC subscribe for offline push | Option to register permanently to the room to receive push notifications about new messages.                                                                                      |
   +---------+--------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | ✓       | Scripting API                  | Supports the Java Scripting API JSR-223                                                                                                                                           |
   +---------+--------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | ✓       | JMX monitoring                 | Advanced monitoring the server via JMX protocol with an API for connecting custom monitors and TCP/IP end-point for connecting general purpose JMX tools                          |
   +---------+--------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | ✓       | HTTP monitoring                | Basic monitoring via HTTP protocol                                                                                                                                                |
   +---------+--------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | ✓       | XMPP Monitoring                | Pluggable, active monitoring via XMPP, retrieving detailed server statistics, receiving automatic notifications about possible problems discovered by the self-monitor mechanisms |
   +---------+--------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | ✓       | SNMP Monitoring                | Advanced server monitoring via SNMP.                                                                                                                                              |
   +---------+--------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | ✓       | Bosh Cache                     | Bosh Session Cache - a feature to quickly reload user data - roster, presences and messages history by the web client (for example after web page reload)                         |
   +---------+--------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | ✓       | Clustering                     | Full clustering support for HA and LB with pluggabble clustering strategies for perfect optimising the cluster to the client’s system                                             |
   +---------+--------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | ✓       | Advanced Clustering Strategy   | Dedicated, specialised clustering strategy for best possible performance                                                                                                          |
   +---------+--------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | ✓       | MUC Clustered                  | Support for clustering group chatrooms with various, pluggable strategies                                                                                                         |
   +---------+--------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | ✓       | PubSub Clustered               | Support for clustering PubSub component with various, pluggable strategies                                                                                                        |
   +---------+--------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | ✓       | Mobile optimisations           | Optimizations designed for Mobile Devices                                                                                                                                         |
   +---------+--------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | ✓       | OSGi                           | Support for running in OSGi environment, i.e. as embedded XMPP server in advanced application server                                                                              |
   +---------+--------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | ✓       | Dynamic rosters                | Ability to create users' rosters entries on the fly based on data retrieved from any sources                                                                                      |
   +---------+--------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | ✓       | Command line admin tools       | Commandline utility to manage server                                                                                                                                              |
   +---------+--------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | ✓       | Unified Archive                | An extension to XEP-0313 Message Archive Management, with greatly improved flexibility in terms of what can be archived.                                                          |
   +---------+--------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+


Repositories/Databases
~~~~~~~~~~~~~~~~~~~~~~~

.. table:: Table 7.Repositories/Databases

   +---------+---------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | Support | Name          | Comment                                                                                                                                                                 |
   +---------+---------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | ✓       | DB per domain | Ability to have multiple databases for specific domains.                                                                                                                |
   +---------+---------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | ✓       | PostgreSQL    | Full support for PostgreSQL database with database schemas excluding dedicated DB schema for PubSub component                                                           |
   +---------+---------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | ✓       | MySQL         | Full support for MySQL database with database schemas, dedicated DB schema for PubSub component                                                                         |
   +---------+---------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | ✓       | SQL Server    | Full support for MS SQL Server database with database schemas excluding dedicated DB schema for PubSub component, only in Tigase server version 3.x                     |
   +---------+---------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | ✓       | Derby DB      | Full support for built-in Derby database with database schemas excluding dedicated DB schema for PubSub component                                                       |
   +---------+---------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | ✓       | JDBC          | Support for all JDBC enabled databases, although the database schemas are available for some databases                                                                  |
   +---------+---------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | ✓       | Drupal Auth   | Drupal authentication - the Tigase server can share user authentication database with Drupal CMS and authenticate users agains Drupal user database                     |
   +---------+---------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | ✓       | Drupal Auth   | Close integration with Drupal CMS, the Tigase can send notifications to subscribed users about new posts, comments and can also publish short news information via XMPP |
   +---------+---------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | ✓       | LDAP-Auth     | LDAP Authentication Connector Supported                                                                                                                                 |
   +---------+---------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

.. [1]
   Requires commercial license

2.3. Licensing and Open Source
-------------------------------

As mentioned previously, Tigase is open source under AGPLv3. If you are not familiar with open source software, or the environment, here are some frequently asked questions that might provide some answers.

| **What does open source mean?**
| This means that Tigase’s source code is available to the public to see how Tigase works. There are no 'black boxes' for packets where things just happen, everything is out in the open, whereas other companies may consider this propitiatory information. In addition, we have the benefit of many talented people working with Tigase to constantly improve Tigase server and related projects. These people not only include the Tigase development team, but other members of the community who submit code improvements, patches, enhancements, or other changes to Tigase.

| **Does this mean that the binaries are open to malicious code?**
| Although we accept patches from contributors, our repository does not accept them directly. Code may be submitted through our `tigase.tech <http://tigase.tech>`__ page and our developers will review the code before it is added. All builds are tested for functionality and security when they are built.

| **Does this mean it is less secure?**
| Not at all. Although anybody can see the source code, and know how Tigase works; your installation, connections, and settings are uniquely yours. Tigase is regularly tested and written to be as secure as possible using the latest encryption and secure connection protocols.

| **Is Tigase free?**
| Tigase is free for download and use in it’s unmodified state. Our commercial grade products such as Advanced Clustering Strategy is available for free use for testing & development.

| **Does this mean I cannot use it in my product or commercial environment?**
| Not necessarily, consult the Affero General Public License Agreement v3 to see if your use qualifies. Tigase is offered under commercial license if your use is not covered by AGPLv3.

| **Are there options for closed code or extensions?**
| Yes! Commercial licenses can be custom made for each client, and software written for your company may be made private or part of our open source distributions at your discretion.

| **Can I contribute code?**
| Sure! We accept code through GitHub pull-requests - submit them to one of our projects listed in our `GitHub organisation <https://github.com/tigase/>`__

2.4. Tigase Server Binary Updates
----------------------------------

Most open source projects try to make sure that the nightly builds compile correctly so that these builds can be used. However, we at Tigase believe that these builds should be separated until they are thoroughly tested and released. Although lots of installations out there we know of just run from our nightly builds, this puts an extra responsibility to make sure all code is functional and will constantly work. Therefore, our general approach is to run all basic functionality tests before each code commit to make sure it works correctly. This does not guarantee that there will never be a problem, but it is a precaution from preventing bad builds from arriving in the hands of our customers.

Some users on the other hand, like to be on the bleeding edge and regularly use our nightly builds exploring new code changes and playing with new features before they are put to a full release. Others prefer to stick to stable and fully tested public releases. Others however, want something from the middle, the most recent features, but bug fixes, something like a beta or a release-candidate state.

Should you choose to use the nightly builds, a few things you should consider:

-  Changes may be made to the code that can negatively affect performance.

-  Changes may be made to the code that can negatively affect security.

We **highly** recommend testing these builds in your environments before upgrading.

With these considerations in mind, we provide nightly builds at `this link <https://build.tigase.net/nightlies/dists/>`__ which provides directories by date.

Standard naming format is ``tigase-server-<version>-SNAPSHOT-b<build>-<type>`` where ``<version>`` is in the form of ``major.minor.bugfix``

.. Note::

   individual days may have the same builds as noted by the byyyy section of the file.\*

Just like the standard distributions, the builds are available with the following extensions (``<type>``):

1. ``javadoc.jar`` - Java installer for javadoc only

2. ``dist.zip`` - Compressed binaries with no dependencies.

3. ``dist.tar.gz`` - tarball compressed binaries with no dependencies.

4. ``dist-max.zip`` - Compressed binaries with all dependencies.

5. ``dist-max.tar.gz`` - tarball compressed binaries with all dependencies.

We also provide automated testing of each of our nightly builds for each supported databases. Tests are done with both functional and low memory parameters in mind, and are available `at this link <https://build.tigase.net/nightlies/tests/>`__. These tests can provide a quick examination of function before upgrading your current build.

2.5. Quick Start Guide
-----------------------

2.5.1. Minimum Requirements
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Before you begin installing Tigase server onto your system, please make sure the minimum requirements are met first:

-  **Java Development Kit (JDK) 11 (LTS)** - We recommend OpenJDK

-  **Administrator access** - We recommend that you install Tigase Server from a user login with administrator access.

..

.. Important::

   You should always run the latest point/bugfix release of the recommended JDK.

.. Note::

   While it should be possible to use newer versions of the JDK, we don’t guarantee it and we recommend using the one mentioned above.


2.5.2. Contents
^^^^^^^^^^^^^^^^

This is a set of documents allowing you to quickly start with our software. Every document provides an introduction to a single topic allowing you to start using/developing or just working on the subject. Please have a look at the documents list below to find a topic you are looking for. If you don’t find a document for the topic you need please `let us know <http://www.tigase.net/contact>`__.

-  `Installation Using Web Installer <#webinstall>`__

-  `Manual installation in console mode <#manualinstall>`__

-  `Installing Tigase on Windows <#windowsInstallation>`__

-  `Network settings for Tigase <#setupTigaseServer>`__

-  `Running Tigase XMPP Server as a service <#tigaseScriptStart>`__

2.5.3. Installation Using Web Installer
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

When Tigase XMPP Server starts up, it looks for the default configuration file: ``etc/config.tdsl``. If this file has not been modified you can run the web installer. Which will step you through the process of configuring Tigase. If you are installing Tigase in a Windows environment, please see the `Windows Installation <#winWebInstall>`__ section.


Download and Extract
~~~~~~~~~~~~~~~~~~~~

First download Tigase XMPP Server and extract it. You can download the `official binaries <https://tigase.net/downloads>`__, or the latest and greatest `nightly builds <https://build.tigase.net/nightlies/dists/>`__. Once you have the distribution binary extract it and navigate to the directory:

.. code:: bash

   $ tar -xf tigase-server-<version>-dist-max.tar.gz
   $ cd tigase-server-<version>



.. Tip::

   Do not run as root user!


Start the Server
~~~~~~~~~~~~~~~~~

.. Note::

   Please make sure ``JAVA_HOME`` is set and points to your JVM installation

.. code:: bash

   scripts/tigase.sh start etc/tigase.conf


Verify Tigase is ready to start installation
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Tigase should start listening on port 8080 - you can check it using ``lsof`` command:

.. code:: bash

   $ lsof -i -P
   COMMAND   PID   USER   FD   TYPE   DEVICE SIZE/OFF NODE NAME
   java    18387 tigase  141u  IPv6 22185825      0t0  TCP *:8080 (LISTEN)

You can also check console log under ``logs/tigase-console.log``, which should point you directly to the installer.


Connect to the Web Installer
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Some points before you can connect:

This setup page is restricted access, however for first setup there is a default account set to setup Tigase: Username: ``admin`` Password: ``tigase``

This combination will only be valid once as it will be removed from ``config.tdsl`` file on completion of setup process. After this point the setup page will only be accessible using the following:

1. JID accounts listed as administrators in admins line in ``config.tdsl`` file.

2. Username and password combinations added to ``config.tdsl`` file manually, or at the last page in this process.

Point your browser to http://localhost:8080/setup/ unless you are working remotely. You can also use the domain name, or IP address.

Enter the username and password above to gain access.


Step Through the Installation Process
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

You will be greeted by the following "About software" page.

|web install 01|

Read it and then click "Next"

The setup consists of several steps that help you configure your installation: selecting features and providing database configuration.

.. Note::

   Order and design of the steps may slightly differ thus we only provide a broad overview of how to proceed:

1. **Advanced Clustering Strategy information**

   You will see some information about our commercial products and licensing. Please read though the agreement, and as a confirmation of agreement type in your name or company and click "Next" to go to the next page.

2. **Basic Tigase server configuration**

   This page will look over your basic configuration settings, those include the server type, domain you wish to use, and gives you a chance to specify an administrator for the domain. Also, you will be selecting what type of database Tigase server will be using (configuration comes later).

   If you do not specify an administrator and password, one is made for you, which will be admin@yourdomain and password is tigase.

3. **Connectivity**

   At this page you will be presented with a list of possible connectivity options supported by Tigase XMPP Server and a way to enable/disable each of them (desktop, mobile, http, websocket, federation, etc.). After making this decisions, click "Next".

4. **Features**

   Now you will be able to select which features of Tigase XMPP Server (such as MUC, PubSub, MIX, MAM, Push Notifications) should be enabled or disabled.

   At this step will also be able to enable clustering on your installation

   When you will be ready, click "Next".

5. **Database configuration**

   This is where the database is configured. The type of database selected in step 3 will influence available options. **BE SURE TO SPECIFY DATABASE ROOT USER ACCOUNT AND PASSWORD**

6. **Database connectivity check**

   After database setup, you should see a page with executed actions and their results. All presented items should be "green", meaning that everything went well. If anything is presented in "red" or "yellow", please read description presented below this header to learn more about this issue. If setup is completed, click "Next".

7. **Setup security**

   The Setup Access Page will be locked from the admin/tigase user as specified above. This is your chance to have the setup pages add a specific user in addition to admin accounts to re-access this setup process later. If left blank, only JIDs listed in admin will be allowed to access.

8. **Saving configuration**

   The installation is almost complete and you will be presented with a page showing what the resulting configuration (stored in ``config.tdsl`` file) will look like.

   If you have a custom setup, or would like to put your own settings in, you may copy and past the contents here to edit the current ``config.tdsl`` file.

   Click "Save" to write the file to disk.

9. **Finished**

   You have now finished the installation, proceed to the next step to restart the server.



Restart the Server
~~~~~~~~~~~~~~~~~~~

It is recommended at this point to stop the server manually and restart it using the proper script for your OS. From the Tigase base directory enter

.. code:: bash

   ./scripts/tigase.sh stop

   ./scripts/tigase.sh start etc/tigase.conf


.. Note::

   In order to make Tigase XMPP Server start automatically during system startup you should setup startup scripts as described in `??? <#tigaseScriptStart>`__

To further fine tune the server you should edit ``etc/tigase.conf``. Ensure ``JAVA_HOME`` path is correct, and increase memory if needed using ``JAVA_OPTIONS`` -Xmx (max), and -Xms (initial). You will need to direct Tigase to read settings from this file on startup as follows.

Everything should be running smooth at this point. Check the logfiles in ``logs/`` if you experience any problems.

Verify Tigase is Running
~~~~~~~~~~~~~~~~~~~~~~~~~

You should see a list of listening ports.

.. code:: bash

   $ lsof -i -P
   COMMAND   PID   USER   FD   TYPE   DEVICE SIZE/OFF NODE NAME
   java    18387 tigase  141u  IPv6 22185825      0t0  TCP *:8080 (LISTEN)
   java    18387 tigase  148u  IPv6 22185834      0t0  TCP *:5222 (LISTEN)
   java    18387 tigase  149u  IPv6 22185835      0t0  TCP *:5223 (LISTEN)
   java    18387 tigase  150u  IPv6 22185836      0t0  TCP *:5290 (LISTEN)
   java    18387 tigase  151u  IPv6 22185837      0t0  TCP *:5280 (LISTEN)
   java    18387 tigase  152u  IPv6 22185838      0t0  TCP *:5269 (LISTEN)


Windows Instructions for using Web Installer
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

There are a few steps involved with setting up Tigase with the web installer in a Windows environment. Please follow this guide.

First step is to extract the distribution archive in it’s entirety to the intended running directory. Once there, run the ``Setup.bat`` file inside the ``win-stuff`` folder. This will move the necessary files to the correct folders before Tigase begins operation.

From here, you have a few options how to run Tigase; ``run.bat`` will operate Tigase using a java command, or ``tigase.bat`` which will start Tigase using the wrapper. You may also install Tigase and run it as a service.

Once this setup is finished, web installer will continue the same from `here <#connecttoWebInstall>`__.

.. |web install 01| image:: images/admin/web-install-01.png

2.5.4. Manual Installation in Console Mode
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Our preferred way to install the Tigase server is using `Web installer <#webinstall>`__ and configuration program which comes with one of the binary packages. Please pick up the latest version of the distribution archive in our `download section <https://tigase.net/downloads>`__.

In many cases however it is not always possible to use the web installer. In many cases you have just an ssh access or even a direct access in console mode only. We are going to provide a text-only installer in one of the next releases but for the time being you can use our binary packages to install the server manually. Please continue reading to learn how to install and setup the server in a few easy steps…​

If you have an old version of the Tigase server running and working and you intend to upgrade it please always backup the old version first.

.. Note::

   Please note that these instructions are for \*nix operating systems, and some modifications may be required for other Operating Systems!


Get the Binary Package
~~~~~~~~~~~~~~~~~~~~~~~

Have a look at our `download area <https://tigase.net/downloads>`__. Always pick the latest version of the package available. For manual installation either ``zip`` or ``tar.gz`` file is available. Pick one of files with filename looking like: ``tigase-server-<version>-b<build>-<type>.<archive>``, where ``<version>`` is in the form of ``major.minor.bugfix``, ``<type>`` can be either ``dist`` (basic package) or ``dist-max`` (extended set of components) and archive type can be eitehr ``tar.gz`` or ``zip``.


Unpack the Package
~~~~~~~~~~~~~~~~~~~~~~~

Unpack the file using command for the tar.gz file:

.. code:: sh

    $ tar -xzvf tigase-server-x.y.z-bv.tar.gz

or for the zip file:

.. code:: sh

    $ unzip tigase-server-x.y.z-bv.zip

A new directory will be created: **tigase-server-x.y.z-bv/**.

Sometimes after unpacking package on unix system startup script doesn’t have execution permissions. To fix the problem you have to run following command:

.. code:: sh

    $ chmod u+x ./scripts/tigase.sh


Prepare Configuration
~~~~~~~~~~~~~~~~~~~~~~~

If you look inside the new directory, it should like this output:

.. code:: sh

    $ ls -l
   total 88
   drwxr-xr-x 2 tigase tigase  4096 Aug 15 18:17 certs
   -rw-r--r-- 1 tigase tigase     0 Aug 15 18:26 ChangeLog
   drwxr-xr-x 2 tigase tigase 12288 Aug 15 18:17 database
   drwxrwxr-x 4 tigase tigase  4096 Oct 12 09:48 docs
   drwxrwxr-x 2 tigase tigase  4096 Oct 12 09:48 etc
   drwxrwxr-x 2 tigase tigase  4096 Oct 12 09:48 jars
   -rw-r--r-- 1 tigase tigase 34203 Aug 15 18:26 License.html
   drwxr-xr-- 2 tigase tigase  4096 Aug 15 18:26 logs
   -rw-r--r-- 1 tigase tigase  3614 Aug 15 18:26 package.html
   -rw-r--r-- 1 tigase tigase  2675 Aug 15 18:26 README
   drwxr-xr-x 9 tigase tigase  4096 Aug 15 18:17 scripts
   drwxr-xr-x 5 tigase tigase  4096 Aug 15 18:17 tigase
   drwxrwxr-x 4 tigase tigase  4096 Oct 12 09:48 win-stuff

At the moment the most important is the etc/ directory with these files:

.. code:: sh

    $ ls -l etc/
   total 36
   -rw-r--r-- 1 tigase tigase  153 Aug 15 18:11 bosh-extra-headers.txt
   -rw-r--r-- 1 tigase tigase  325 Aug 15 18:11 client-access-policy.xml
   -rw-r--r-- 1 tigase tigase  124 Aug 15 18:11 config.tdsl
   -rw-r--r-- 1 tigase tigase  263 Aug 15 18:11 cross-domain-policy.xml
   -rw-r--r-- 1 tigase tigase 2337 Aug 15 18:11 jmx.access
   -rw-r--r-- 1 tigase tigase 2893 Aug 15 18:11 jmx.password
   -rw-r--r-- 1 tigase tigase  735 Aug 15 18:11 logback.xml
   -rw-r--r-- 1 tigase tigase 3386 Aug 15 18:11 snmp.acl
   -rw-r--r-- 1 tigase tigase 1346 Aug 15 18:11 tigase.conf


Configure tigase.conf
'''''''''''''''''''''''

Tigase.conf is a file that contains general program operating parameters, and java settings for Tigase to run. For now, the only setting we need to set is the **JAVA_HOME** directory.

.. code:: sh

   JAVA_HOME="${JDKPath}"

Replace **${JDKPath}** with a path to Java JDK installation on your system.


Configure config.tdsl
''''''''''''''''''''''

You need also to edit the ``config.tdsl`` file. It contains initial parameters normally set by the configuration program. As this is a manual installation, you will have to edit this document yourself. It contains already a few lines:

.. code:: dsl

   'config-type' = 'setup'

   http () {
       setup () {
           'admin-user' = 'admin'
           'admin-password' = 'tigase'
       }
   }

You will need to set a few things in order to get Tigase up and running.



Step 1: Change config-type


Refer to `config-type <#configType>`__ property description for details, but for most operations, change ``setup`` to ``default``.


Step 2: Set virtual host

Without a virtual host, your XMPP server has no domain with which to operate. To set a virtual host use the following configuration:

.. code:: dsl

   'default-virtual-host' = 'hostname'

You have to replace ``hostname`` with a domain name used for your XMPP installation. Let’s say this is **jabber.your-great.net**. Your setting should look like this:

.. code:: dsl

   'default-virtual-host' = 'jabber.your-great.net'

There are many other settings that can be configured `visit this section for details <#tigase41virtualHosts>`__.


Step 3: Set Administrators


At least one administrator is required, and once the database is setup will have the default password of ``tigase``. Be sure to change this once you have finished setting up your server. To add admins, use the following line in the ``config.tdsl`` file:

.. code:: dsl

   admins = [ 'admin@jabber.your-great.net', 'user2jabber.your-great.net' ]


Step 4: Set databases


You will also need to configure connection to the database. First you have to decide what database you want to use: ``Derby``, ``MySQL``, ``PostgreSQL``, ``MSSQL``, or ``MondoDB``. Each database will have slightly different configurations. If we are using derby, in a directory called ``tigasedb``, your configuration would look like this:

.. code:: dsl

   dataSource () {
       default () {
           uri = 'jdbc:derby:tigasedb;create=true'
       }
   }

Consult `dataSource <#dataSource>`__ property for more configuration info.

This is enough basic configuration to have your Tigase server installation running.


Install Database
~~~~~~~~~~~~~~~~~

Creating the database is the next step. Previously, we had scripts to handle this process, but we now have the advantage of functions in the ``tigase.sh`` script that can be used. Setting up the database can now be done using a single command.

.. code:: dsl

   ./scripts/tigase.sh install-schema etc/tigase.conf -T derby -D tigasedb -H localhost -U tigase_user -P tigase_pass -R root -A rootpass -J admin@jabber.your-great.net -N pass

This command will install tigase using a Derby database on one named ``tigasedb`` hosted on ``localhost``. The username and password editing the database is ``tigase_pass`` and ``root``. Note that ``-J`` explicitly adds the administrator, this is highly recommended with the ``-N`` passing the password. You may customize this command as needed, refer to the `install-schema <#install-schema>`__ section of the documentation for more information.

On a windows system, you need to call the program directly:

.. code:: windows

   C:\tigase>java -cp "jars/*" tigase.db.util.SchemaManager "install-schema" -T derby -D tigasedb -H localhost -U tigase_user -P tigase_pass -R root -A rootpass -J admin@jabber.your-great.net -N pass

If this successfully passes, you should see some information printed out

.. code:: bash

   LogLevel: CONFIG
   2017-10-12 20:05:47.987 [main]             DBSchemaLoader.init()                   CONFIG:   Parameters: [ingoreMissingFiles: false, logLevel: CONFIG, adminPassword: pass, admins: [admin@jabber.your-great.net], dbRootPass: rootpass, dbRootUser: root, dbType: derby, dbName: tigasedbx, dbHostname: localhost, dbUser: tigase_user, dbPass: tigase_pass, useSSL: false, useLegacyDatetimeCode: false, serverTimezone: null, file: null, query: null]
   Oct 12, 2017 8:05:48 PM tigase.util.DNSResolverDefault <init>
   WARNING: Resolving default host name: ubuntu took: 7
   Oct 12, 2017 8:05:49 PM tigase.db.util.SchemaManager loadSchemas
   INFO: found 1 data sources to upgrade...
   Oct 12, 2017 8:05:49 PM tigase.db.util.SchemaManager loadSchemas
   INFO: begining upgrade...
   LogLevel: CONFIG
   2017-10-12 20:05:49.877 [main]             DBSchemaLoader.init()                   CONFIG:   Parameters: [ingoreMissingFiles: false, logLevel: CONFIG, adminPassword: pass, admins: [admin@jabber.your-great.net], dbRootPass: rootpass, dbRootUser: root, dbType: derby, dbName: tigasedbx, dbHostname: null, dbUser: null, dbPass: null, useSSL: null, useLegacyDatetimeCode: false, serverTimezone: null, file: null, query: null]
   2017-10-12 20:05:49.877 [main]             DBSchemaLoader.validateDBConnection()   INFO:     Validating DBConnection, URI: jdbc:derby:tigasedbx;create=true
   2017-10-12 20:05:50.932 [main]             DBSchemaLoader.validateDBConnection()   CONFIG:   DriverManager (available drivers): [org.apache.derby.jdbc.AutoloadedDriver@65262308, jTDS 1.3.1, com.mysql.jdbc.Driver@54997f67, com.mysql.fabric.jdbc.FabricMySQLDriver@189633f2, org.postgresql.Driver@76fc5687]
   2017-10-12 20:05:50.932 [main]             DBSchemaLoader.validateDBConnection()   INFO:     Connection OK
   2017-10-12 20:05:50.933 [main]             DBSchemaLoader.validateDBExists()       INFO:     Validating whether DB Exists, URI: jdbc:derby:tigasedbx;create=true
   2017-10-12 20:05:50.936 [main]             DBSchemaLoader.withConnection()         CONFIG:   DriverManager (available drivers): [org.apache.derby.jdbc.AutoloadedDriver@65262308, jTDS 1.3.1, com.mysql.jdbc.Driver@54997f67, com.mysql.fabric.jdbc.FabricMySQLDriver@189633f2, org.postgresql.Driver@76fc5687]
   2017-10-12 20:05:50.937 [main]             DBSchemaLoader.lambda$validateDBExists$283()  INFO: Exists OK
   2017-10-12 20:05:50.939 [main]             DBSchemaLoader.loadSchemaFile()         INFO:     Loading schema from file(s): database/derby-schema-7-2.sql, URI: jdbc:derby:tigasedbx;create=true
   2017-10-12 20:05:50.941 [main]             DBSchemaLoader.withConnection()         CONFIG:   DriverManager (available drivers): [org.apache.derby.jdbc.AutoloadedDriver@65262308, jTDS 1.3.1, com.mysql.jdbc.Driver@54997f67, com.mysql.fabric.jdbc.FabricMySQLDriver@189633f2, org.postgresql.Driver@76fc5687]
   2017-10-12 20:05:51.923 [main]             DBSchemaLoader.lambda$loadSchemaFile$287()  INFO:  completed OK
   2017-10-12 20:05:51.925 [main]             DBSchemaLoader.loadSchemaFile()         INFO:     Loading schema from file(s): database/derby-message-archiving-schema-1.3.0.sql, URI: jdbc:derby:tigasedbx;create=true
   2017-10-12 20:05:51.926 [main]             DBSchemaLoader.withConnection()         CONFIG:   DriverManager (available drivers): [org.apache.derby.jdbc.AutoloadedDriver@65262308, jTDS 1.3.1, com.mysql.jdbc.Driver@54997f67, com.mysql.fabric.jdbc.FabricMySQLDriver@189633f2, org.postgresql.Driver@76fc5687]
   2017-10-12 20:05:52.209 [main]             DBSchemaLoader.lambda$loadSchemaFile$287()  INFO:  completed OK
   2017-10-12 20:05:52.210 [main]             DBSchemaLoader.loadSchemaFile()         INFO:     Loading schema from file(s): database/derby-muc-schema-2.5.0.sql, URI: jdbc:derby:tigasedbx;create=true
   2017-10-12 20:05:52.211 [main]             DBSchemaLoader.withConnection()         CONFIG:   DriverManager (available drivers): [org.apache.derby.jdbc.AutoloadedDriver@65262308, jTDS 1.3.1, com.mysql.jdbc.Driver@54997f67, com.mysql.fabric.jdbc.FabricMySQLDriver@189633f2, org.postgresql.Driver@76fc5687]
   2017-10-12 20:05:52.305 [main]             DBSchemaLoader.lambda$loadSchemaFile$287()  INFO:  completed OK
   2017-10-12 20:05:52.306 [main]             DBSchemaLoader.loadSchemaFile()         INFO:     Loading schema from file(s): database/derby-pubsub-schema-3.3.0.sql, URI: jdbc:derby:tigasedbx;create=true
   2017-10-12 20:05:52.307 [main]             DBSchemaLoader.withConnection()         CONFIG:   DriverManager (available drivers): [org.apache.derby.jdbc.AutoloadedDriver@65262308, jTDS 1.3.1, com.mysql.jdbc.Driver@54997f67, com.mysql.fabric.jdbc.FabricMySQLDriver@189633f2, org.postgresql.Driver@76fc5687]
   2017-10-12 20:05:52.731 [main]             DBSchemaLoader.lambda$loadSchemaFile$287()  INFO:  completed OK
   2017-10-12 20:05:52.732 [main]             DBSchemaLoader.addXmppAdminAccount()    INFO:     Adding XMPP Admin Account, URI: jdbc:derby:tigasedbx;create=true
   2017-10-12 20:05:52.732 [main]             DBSchemaLoader.addXmppAdminAccount()    CONFIG:   RepositoryFactory.getAuthRepository(null, jdbc:derby:tigasedbx;create=true,{data-repo-pool-size=1})
   Oct 12, 2017 8:05:52 PM tigase.db.jdbc.DataRepositoryImpl initialize
   INFO: Table schema found: jdbc:derby:tigasedbx;create=true, database type: derby, database driver: org.apache.derby.jdbc.EmbeddedDriver
   Oct 12, 2017 8:05:52 PM tigase.db.jdbc.DataRepositoryImpl initialize
   INFO: Initialized database connection: jdbc:derby:tigasedbx;create=true
   2017-10-12 20:05:52.884 [main]             DBSchemaLoader.addXmppAdminAccount()    INFO:     All users added
   2017-10-12 20:05:52.884 [main]             DBSchemaLoader.postInstallation()       INFO:     Post Installation, URI: jdbc:derby:tigasedbx;create=true
   2017-10-12 20:05:52.891 [main]             DBSchemaLoader.withConnection()         CONFIG:   DriverManager (available drivers): [org.apache.derby.jdbc.AutoloadedDriver@65262308, jTDS 1.3.1, com.mysql.jdbc.Driver@54997f67, com.mysql.fabric.jdbc.FabricMySQLDriver@189633f2, org.postgresql.Driver@76fc5687]
   2017-10-12 20:05:52.892 [main]             DBSchemaLoader.lambda$postInstallation$286()  INFO: Finalizing...
   2017-10-12 20:05:52.893 [main]             DBSchemaLoader.lambda$postInstallation$286()  INFO:  completed OK
   2017-10-12 20:05:52.895 [main]             DBSchemaLoader.shutdownDerby()          INFO:     Validating DBConnection, URI: jdbc:derby:tigasedbx;create=true
   2017-10-12 20:05:53.129 [main]             DBSchemaLoader.withConnection()         SEVERE:


   =====
   Failure: Database 'tigasedbx' shutdown.
   =====


   Oct 12, 2017 8:05:53 PM tigase.db.util.SchemaManager loadSchemas
   INFO: schema upgrade finished!




     =============================================================================
       Schema installation finished

     Data source: default with uri jdbc:derby:tigasedbx;create=true
       Checking connection to database ok
       Checking if database exists ok
       Loading schema: Tigase XMPP Server (Core), version: 8.0.0   ok
       Loading schema: Tigase Message Archiving Component, version: 1.3.0  ok
       Loading schema: Tigase MUC Component, version: 2.5.0    ok
       Loading schema: Tigase PubSub Component, version: 3.3.0 ok
       Adding XMPP admin accounts  ok
       Post installation action    ok

     Example etc/config.tdsl configuration file:

     'config-type' = 'default'
     debug = [ 'server' ]
     'default-virtual-host' = [ 'ubuntu' ]
     dataSource () {
         default () {
             uri = 'jdbc:derby:tigasedbx;create=true'
         }
     }
     amp () {}
     bosh () {}
     c2s () {}
     eventbus () {}
     http () {}
     'message-archive' () {}
     monitor () {}
     muc () {}
     pubsub () {}
     s2s () {}
     ws2s () {}
     =============================================================================

Note at the end, the script will output a recommended example file. You may use this in conjunction with your written config file, but some settings may not be set using this configuration. Again, it is only an **EXAMPLE**.


Start the Server
~~~~~~~~~~~~~~~~~~

You can start the server using the tigase file found in the scripts sub-directory of Tigase server base directory. There, select the type of linux you have, debian, gentoo, mendriva or redhat. In the root server directory type the following command:

.. code:: bash

   ./scripts/{OS}/init.d/tigase start etc/tigase.conf

Where {OS} is your \*nix operating system.

and you should get the output like this:

.. code:: sh

   Starting Tigase:
   nohup: redirecting stderr to stdout
   Tigase running pid=18103


Check if it is Working
~~~~~~~~~~~~~~~~~~~~~~~

The server is started already but how do you know if it is really working and there were no problems. Have a look in the ``logs/`` directory. There should be a few files in there:

.. code:: sh

    $ ls -l logs/
   total 40K
   -rw-r--r-- 1 20K 2009-02-03 21:48 tigase-console.log
   -rw-r--r-- 1 16K 2009-02-03 21:48 tigase.log.0
   -rw-r--r-- 1   0 2009-02-03 21:48 tigase.log.0.lck
   -rw-r--r-- 1   6 2009-02-03 21:48 tigase.pid

The first 2 files are the most interesting for us: **tigase-console.log** and **tigase.log.0**. The first one contains very limited information and only the most important entries. Have a look inside and check if there are any **WARNING** or **SEVERE** entries. If not everything should be fine.

Now you can connect with an XMPP client of your choice with the administrator account you setup earlier.

2.5.5. Windows Installation
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Tigase XMPP Server can also work on Microsoft Windows systems and servers, although some slight modifications may be necessary to get things ready to run.

Although you may wish to use command line, take note that commands entered in shell may require quotations in some cases.

Make sure that you have Java JDK v8 installed on your system prior to installing Tigase. It will also help to fully setup whatever database software you will be using as well.

Step 1: Initial Setup
~~~~~~~~~~~~~~~~~~~~~~

Download the Tigase XMPP Server archive from `our repository <https://tigase.net/downloads>`__ and extract it to a directory of your choice.

Once that is completed, enter the directory ``win-stuff`` and run the setup.bat program. This program when run, will extract the necessary files to appropriate places on your computer. The bat file should look like the following:

.. code:: bat

   copy "tigase.ico" "..\"
   copy "wrapper\wrapper.jar" "..\jars"
   copy "wrapper\wrapper.dll" "..\jars"
   copy "wrapper\wrapper.exe" "..\"
   copy "wrapper\wrapper.conf" "..\"
   copy "wrapper\wrapper-community-license-1.2.txt" "..\"
   copy "scripts\*.*" "..\"

Step 2: Starting Server
~~~~~~~~~~~~~~~~~~~~~~~~

To start the server you may use a command prompt from the installation directory

.. code:: bash

   java -cp "jars/*" tigase.server.XMPPServer

..

   **Note**

   this may freeze the command window, and will only display output from Tigase.

Or you may run wrapper.exe or tigase.bat from the GUI.


2A: Installing as a service
''''''''''''''''''''''''''''

The cleanest way to operate Tigase in a Windows environment is to install Tigase as a Service by running the InstallTigaseService.bat program. This will install Tigase as a system service, and now the server can be controlled from the services.msc panel. This allows for stopping, starting, and pausing of Tigase XMPP Server and allowing for graceful shutdowns.

For a basic installation, MySQL is recommended over Derby DB. For that purpose, we have included a basic installation guide for MySQL on Windows systems here:


MySQL Database Installation
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

The section describes installation and configuration of the MySQL database to work with Tigase server.

Download the binary package from MySQL download area at `mysql.com <http://dev.mysql.com/downloads/mysql/5.0.html#win32>`__. Make sure you select executable proper for your operating system.

Run the installation program and follow default installation steps. When the installation is complete find the MySQL elements in the Windows Start menu and run the MySQL Configuration Wizard. Follow the wizard and make sure to check settings against the screenshots in the guide below.

In Welcome window just press 'Next'.(pic.1)

|sql1|

In the next window select option: 'Detailed Configuration' and press 'Next' (pic. 2)

|sql2|

On the next screen select option: 'Server Machine' and press 'Next' (pic. 3)

|sql3|

On the forth windows leave the default" 'Multi-functional Database' and press 'Next' (pic. 4)

|sql4|

On the step number five just press 'Next' using defaults. (pic. 5)

|sql5|

Again, on window 6 select the default - 'Decision Support (DSS)/OLAP' and press 'Next' (pic.6)

|sql6|

Make sure you switch OFF the 'Strict mode' and and press 'Next' (pic. 7)

|sql7|

On the character encoding page select: 'Manual Selected Default Character set/ Collation' and 'utf8', press 'Next' (pic.8)

|sql8|

On next window select 'Include Bin Directory in Windows PATH' and press 'Next' (pic.9)

|sql9|

On this window just enter the database super user password and make sure you remember it. When ready press 'Next' (pic. 10)

|sql10|

This is the last screen. Press 'Execute' to save the configuration parameters. (pic. 11)

|sql11|

When the configuration is saved you can repeat all the steps and change settings at any time by running: **START ⇒ Programs ⇒ MYSQL⇒ MYSQL serwer machine⇒ MySQL Server Instance Config Wizard**

Now we have to setup Tigase database. From the Start menu run the MySQL console and enter all commands below finishing them with **<ENTER>**:

1. Create the database:

   .. code:: sql

      mysql>create database tigasedb;

2. Add database user:

   .. code:: bash

      mysql> GRANT ALL ON tigasedb.* TO tigase_user@'%' IDENTIFIED BY 'tigase_passwd';
      mysql> GRANT ALL ON tigasedb.* TO tigase_user@'localhost' IDENTIFIED BY 'tigase_passwd';
      mysql> GRANT ALL ON tigasedb.* TO tigase_user IDENTIFIED BY 'tigase_passwd';
      mysql> FLUSH PRIVILEGES;

3. Load Tigase database schema:

   .. code:: bash

      mysql> use tigasedb;
      mysql> source c:/Program Files/Tigase/database/mysql-schema.sql;

When the system is up and running you can connect with any XMPP client (Psi for example) to your server to see if it is working.

.. |sql1| image:: images/admin/sql1.JPG
.. |sql2| image:: images/admin/sql2.JPG
.. |sql3| image:: images/admin/sql3.JPG
.. |sql4| image:: images/admin/sql4.JPG
.. |sql5| image:: images/admin/sql5.JPG
.. |sql6| image:: images/admin/sql6.JPG
.. |sql7| image:: images/admin/sql7.JPG
.. |sql8| image:: images/admin/sql8.JPG
.. |sql9| image:: images/admin/sql9.JPG
.. |sql10| image:: images/admin/sql10.JPG
.. |sql11| image:: images/admin/sql11.JPG

2.5.6. Tigase Server Network Instructions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

One you have installed Tigase XMPP Server on a machine, you’re going to want to use it. If you are just using for local communications on a network behind a router, you’re all set. Enjoy and use!

However, if you want to have people from other computers outside your network connect to your server, you’re going to have to go through a few more steps to show your server out to the public.

   **Note**

   This guide is merely a recommendation of how to get a local server to be open to incoming communications. Any time you open ports, or take other security measures you risk compromising your network security. These are only recommendations, and may not be appropriate for all installations. Please consult your IT Security expert for securing your own installation.

XMPP, being a decentralized communication method, relies on proper DNS records to figure out where and how an XMPP server is setup. Operating an XMPP Server will require you to properly setup DNS routing so not only can clients connect to you, but if you decide to run a federated server and enable server to server communication, you will need to do the same. If you already have a DNS server already, you should have little issue adding these records. If you do not have a DNS setup pointing to your server, you may use a free dynamic name service such as dynu.com.


A Records
~~~~~~~~~~

You will not be able to use an IP Address or a CNAME record to setup an XMPP Server. While it’s not required, an A record can provide some other benefits such serving as a backup in case the SRV record is not configured right.


SRV Records
~~~~~~~~~~~~

You will need to set SRV records both for client-to-server (c2s) communication and, if you plan to use it, server to server (s2s) communication. We recommend both records are entered for every server as some resources or clients will check for both records. For this example we will use tigase.org is our domain, and xmpp as the xmpp server subdomain.

SRV records have the following form:

::

   _service._protocol.name. TTL class SRV Priority weight port target.

The key is as follows:

-  ``service``: is the symbolic name of the desired service, in this case it would be *xmpp-client* or *xmpp-server*.

-  ``protocol``: is the transport protocol, either TCP or UDP, XMPP traffic will take place over *TCP*.

-  ``name``: the domain name where the server resides, in this case *tigase.org*.

-  ``TTL``: a numeric value for DNS time to live in milliseconds, by default use *86400*.

-  ``class``: DNS class field, this is always *IN*.

-  ``priority``: the priority of the target host with lower numbers being higher priority. Since we are not setting up multiple SRV records, we can use *0*.

-  ``weight``: the relative weight for records with the same priority. We can use *5*.

-  ``port``: the specific TCP or UDP port where the service can be found. In this case it will be *5222* or *5269*.

-  ``target``: the hostname of the machine providing the service, here we will use *xmpp.tigase.org*.

For our example server, the SRV records will then look like this:

::

   _xmpp-client._TCP.tigase.org 86400 IN SRV 0 5 5222 xmpp.tigase.org
   _xmpp-server._TCP.tigase.org 86400 IN SRV 0 5 5269 xmpp.tigase.org


Tigase and Vhosts
''''''''''''''''''

If you are running multiple vhosts or subdomains that you wish to separate, you will need another record. In this case an A record will be all you need if you are using default ports. If you are using custom ports, you will need to have a new SRV record for each subdomain.


Hosting via Tigase.me
~~~~~~~~~~~~~~~~~~~~~~

If you don’t want to do all the hosting yourself, you can still have an XMPP service running in your own domain. The only condition right now is proper DNS service record (SRV) configuration that point to the following DNS address: ``tigase.me``.

We highly encourage using SRV records. If you want to register: **your-domain.tld** on our XMPP service make sure that it resolves correctly:

+----------------------------------------------+----------+--------------------------+--------------------------------------+
| Service                                      | DNS Type | DNS record               | Comment                              |
+----------------------------------------------+----------+--------------------------+--------------------------------------+
| ``_xmpp-client._tcp.your-domain.tld``        | SRV      | ``10 0 5222 tigase.me.`` | Basic XMPP                           |
+----------------------------------------------+----------+--------------------------+--------------------------------------+
| ``_xmpps-client._tcp.your-domain.tld``       | SRV      | ``10 0 5223 tigase.me.`` | DirectTLS                            |
+----------------------------------------------+----------+--------------------------+--------------------------------------+
| ``_xmpp-server._tcp.your-domain.tld``        | SRV      | ``10 0 5269 tigase.me.`` | Federation / s2s connection          |
+----------------------------------------------+----------+--------------------------+--------------------------------------+
| ``_xmpp-server._tcp.muc.your-domain.tld``    | SRV      | ``10 0 5269 tigase.me.`` | Federation / s2s connection (MUC)    |
+----------------------------------------------+----------+--------------------------+--------------------------------------+
| ``_xmpp-server._tcp.mix.your-domain.tld``    | SRV      | ``10 0 5269 tigase.me.`` | Federation / s2s connection (MIX)    |
+----------------------------------------------+----------+--------------------------+--------------------------------------+
| ``_xmpp-server._tcp.pubsub.your-domain.tld`` | SRV      | ``10 0 5269 tigase.me.`` | Federation / s2s connection (PubSub) |
+----------------------------------------------+----------+--------------------------+--------------------------------------+

..

   **Note**

   If you want to have MUC, MIX and PubSub available under your domain as subdomains, you have to setup DNS for your ``muc.your-domain.tld``, ``mix.your-domain.tld`` and ``pubsub.your-domain.tld`` domains too but they are optional.

You can check if the configuration is correct by issuing following commands:

.. code:: sh

   $ host -t SRV _xmpp-client._tcp.your-domain.tld
   $ host -t SRV _xmpps-client._tcp.your-domain.tld
   $ host -t SRV _xmpp-server._tcp.your-domain.tld
   $ host -t SRV _xmpp-server._tcp.muc.your-domain.tld
   $ host -t SRV _xmpp-server._tcp.pubsub.your-domain.tld

Now, how do you register your domain with our service?

There are a few ways. We recommend checking with the `Add and Manage Domains <#addManageDomain>`__ section of the documentation on setting that up. If you cannot or don’t want to do it on your own, the way described in the guide please send us a message, either via XMPP to admin@tigase.im or the contact form requesting new domain. User registration is available via in-band registration protocol. You can also specify whether you want to allow anonymous authentication to be available for your domain and you can specify maximum number of users for your domain.


Providing certificate
''''''''''''''''''''''

It’s also encouraged to provide dedicated SSL certificate - there are various ways to do it and they are described in `??? <#InstallingSSLCertificate>`__. You may want to take advantage of free Let’s Encrypt certificates and automate whole upload and renewal process as described in `??? <#LetsEncryptCertificate>`__


Checking setup
~~~~~~~~~~~~~~~

If you have a cell phone on a separate network with an XMPP client, you can now try to login to test the server. If that is not handy, you can use an online tool to check proper DNS records such as kingant’s: https://kingant.net/check_xmpp_dns/ and it will tell you if anything is missing.


Ports description
~~~~~~~~~~~~~~~~~~~

Once your server is setup, you may need to open at least two ports. By default XMPP communication happens on ports 5222/5269, to which point SRV records. Other ports used by the server are:

-  ``3478`` - TURN or STUN, plain socket, TCP and UDP

-  ``5349`` - TURN or STUN, over TLS, TCP and UDP

-  ``5222`` - incoming client to server XMPP connections

-  ``5223`` - incoming client to server XMPP connections over TLS/SSL, including DirectTLS

-  ``5269`` - default s2s port, i.e.: federation support

-  ``5277`` - inter-cluster communication

-  ``5280`` - default BOSH connections

-  ``5290`` - default WebSocket connections

-  ``5291`` - default WebSocket connections over TLS/SSL

-  ``8080`` - for HTTP server (web-based setup, REST API, file upload extension, etc.)

-  ``9050`` - JMX Monitoring

If for any reason you can’t use default ports and have to change them it’s possible to point SRV records those ports. Please keep in mind, that you have to open those ports for incoming connections in your firewall. In case you are using ``iptables`` you can use following command to include those ports in your rules:

.. code:: bash

   iptables -A INPUT -p tcp -m tcp --dport 5222 -j ACCEPT
   iptables -A INPUT -p tcp -m tcp --dport 5223 -j ACCEPT
   iptables -A INPUT -p tcp -m tcp --dport 5269 -j ACCEPT
   iptables -A INPUT -p tcp -m tcp --dport 5277 -j ACCEPT
   iptables -A INPUT -p tcp -m tcp --dport 5280 -j ACCEPT
   iptables -A INPUT -p tcp -m tcp --dport 5290 -j ACCEPT
   iptables -A INPUT -p tcp -m tcp --dport 8080 -j ACCEPT
   iptables -A INPUT -p tcp -m tcp --dport 9050 -j ACCEPT

Both ports should be setup to use TCP only. If for any reason you want to make service available for different ports you can:

1. change ports in Tigase configuration and update DNS SRV records;

2. forward those ports to default Tigase ports (this is especially useful under \*nix operating system if you want to utilize ports lower than ``1024`` while running, as recommended, Tigase service from user account - there is a limitation and user accounts can bind to ports lower than ``1024``), for example using ``iptables`` rules (in following example we are making available Tigase SSL websocket port available under port ``443``, which is usually opened in corporate firewalls):

   .. code:: bash

      iptables -t nat -A PREROUTING -p tcp --dport 443 -j REDIRECT --to-ports 5291

2.5.7. Tigase Script Selection
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

As mentioned in each of the quick start sections, each distribution of Tigase XMPP server comes with a number of scripts that are customized for different versions of Linux.

.. table:: init.d chart

   +------------------+--------------------------------------------------+-----------------------------------------------------------------------------------------------------------------+
   | Operating system | init.d file path                                 | Types of Operating Systems                                                                                      |
   +==================+==================================================+=================================================================================================================+
   | Systemd          | ``tigase-server/scripts/systemd/*``              | Systemd-based distributions                                                                                     |
   +------------------+--------------------------------------------------+-----------------------------------------------------------------------------------------------------------------+
   | Debian           | ``tigase-server/scripts/debian/tigase.init.d``   | Knoppix, Ubuntu (before v15.04), Raspbian or Duvian                                                             |
   +------------------+--------------------------------------------------+-----------------------------------------------------------------------------------------------------------------+
   | Gentoo           | ``tigase-server/scripts/gentoo/init.d/tigase``   | CoreOS (before v94.0.0), Tin Hat Linux or other \*too based systems                                             |
   +------------------+--------------------------------------------------+-----------------------------------------------------------------------------------------------------------------+
   | Mandriva         | ``tigase-server/scripts/mandriva/init.d/tigase`` | Specific init.d file for Mandriva Linux                                                                         |
   +------------------+--------------------------------------------------+-----------------------------------------------------------------------------------------------------------------+
   | Redhat           | ``tigase-server/scripts/redhat/init.d/tigase``   | RedHat (before v7.0) and other RPM based linux derivatives like CentOS (before v.7.14), openSUSE (before v12.2) |
   +------------------+--------------------------------------------------+-----------------------------------------------------------------------------------------------------------------+



.. Note::

   If your operating system is a systemd-based linux distribution, we recommend to use systemd service scripts. It may be possible to use (in this case legacy) ``init.d`` startup files as before, but usage of systemd startup scripts will allow better control of the startup process and will even allow for automatic restart of the Tigase XMPP Server in the case of JVM crash.


Configuration: For Linux Distributions using systemd
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

To set up Tigase XMPP Server as a system service it is required to copy ``tigase-server.service`` file to ``/etc/systemd/system/`` directory

.. code:: bash

   sudo cp $SCRIPT_FILE_PATH/tigase-server.service /etc/systemd/system/

This file contains following parameters which may need to be adjusted:

-  ``User`` - Specifies the user that will run the program. This should be a user with SU permissions.

-  ``WorkingDirectory`` - Specifies installation directory *(default: ``/home/tigase/tigase-server``)*

-  ``ExecStart`` - Specifies startup command *(default: runs ``scripts/tigase.sh start etc/tigase.conf`` in the Tigase installation directory)*

-  ``ExecStop`` - Specifies shutdown command *(default: runs ``scripts/tigase.sh stop etc/tigase.conf`` in the Tigase installation directory)*

-  ``PIDFile`` - Specifies location of the PID file *(default: ``logs/tigase.pid`` file in the Tigase installation directory)*

It is also required to copy options file ``tigase-server`` to ``/etc/default/`` directory

.. code:: bash

   sudo cp $SCRIPT_FILE_PATH/tigase-server /etc/default/

With those files in place you need to reload ``systemctl`` daemon

.. code:: bash

   sudo systemctl daemon-reload

..

   **Note**

   If you are upgrading from the previous version of the Tigase XMPP Server which was not running as the systemd system service it is required to uninstall old service and remove old service files.


Configuration: For All Linux Distributions
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Once you’ve located the appropriate distribution scripts (please take a look at the table above), copy it to your system’s init.d folder (usually it’s ``/etc/init.d/``):

.. code:: bash

   sudo cp $SCRIPT_FILE_PATH /etc/init.d/tigase

You may also need to make it executable:

.. code:: bash

   sudo chmod +x /etc/init.d/tigase

It is recommended that you open the script files or configuration files as some have some parameters that you will need to specify.


Gentoo
'''''''

The conf.d script must contain the following parameters:

.. code:: conf

   TIGASE_HOME="/home/tigase/tigase-server"
   TIGASE_USER=tigase
   TIGASE_CONF="etc/tigase.conf"

The following should be configured:

-  ``TIGASE_HOME`` - Specifies the Tigase Server installation directory.

-  ``TIGASE_USER`` - Specifies the user that will run the program. This should be a user with SU permissions.

-  ``TIGASE_CONF`` - The location of tigase.conf file, relative to the ``TIGASE_HOME`` directory.


Mandriva
'''''''''

Mandriva has a single init.d file, however it should be configured:

.. code:: bash

   …
   export JAVA_HOME=/usr/java/jdk1.8.0
   export TIGASE_DIR=/opt/tigase/server/
   tigase=$TIGASE_DIR/scripts/tigase.sh
   prog=tigase
   config=$TIGASE_DIR/etc/tigase.conf
   …

The following should be configured:

-  ``JAVA_HOME`` - The location of your JDK Installation.

-  ``TIGASE_DIR`` - Tigase Server installation directory.

-  ``tigase`` - The location of your tigase.sh script. This should not need adjusting if you maintain the default file structure.

-  ``config`` - The location of your tigase.conf file. This should not need adjusting if you maintain the default file structure.

``pid`` file will be stored in ``/var/run/ser.pid``


Redhat
'''''''

Similar to Mandriva, you will need to configure the init.d file:

.. code:: bash

   …
   JAVA_HOME=/usr/lib/jvm/java/

   USERNAME=tigase
   USERGROUP=tigase
   NAME=tigase
   DESC="Tigase XMPP server"

   TIGASE_HOME=/home/tigase/tigase-server
   TIGASE_LIB=${TIGASE_HOME}/jars
   TIGASE_CONFIG=/etc/tigase.conf
   TIGASE_OPTIONS=
   TIGASE_PARAMS=

   PIDFILE=
   TIGASE_CONSOLE_LOG=
   …

-  ``USERNAME`` - Username running Tigase, should have su permissions.

-  ``USERGROUP`` - The usergroup of the username.

-  ``NAME`` - OS name for Tigase program.

-  ``DESC`` - Optional description.

-  ``TIGASE_HOME`` - The location of your Tigase Server installation directory.

-  ``TIGASE_LIB`` - The location of your Tigase Jars folder, you should not need to adjust this if you set ``TIGASE_HOME`` properly, and maintain the default file structure.

-  ``TIGASE_CONFIG`` - The location of your tigase.conf file relative to ``TIGASE_HOME``

-  ``TIGASE_OPTIONS`` - Legacy options for Tigase, most are now handled in ``config.tdsl`` or tigase.conf.

-  ``TIGASE_PARAMS`` - Parameters passed to command line when launching Tigase.

-  ``PIDFILE`` - Location of Tigase PID file if you wish to use custom directory. Default will be located in /logs or /var/temp directory.

-  ``TIGASE_CONSOLE_LOG`` - Location of Tigase Server console log file if you wish to use a custom directory. Default will be located in /logs directory, failing that /dev/null.

After you’ve copied the script, in order to install sysinit script you have to add it to the configuration:

.. code:: bash

   /sbin/chkconfig --add tigase

Service can be enabled or disabled service with:

.. code:: bash

   /sbin/chkconfig tigase <on|off|reset>

Debian
'''''''

As with other distributions you should copy init.d script to the correct location. Afterwards it should be edited and correct values for variables need to be set:

.. code:: bash

   …
   USERNAME=tigase
   USERGROUP=tigase
   NAME=tigase
   DESC="Tigase XMPP server"

   TIGASE_HOME=/usr/share/tigase
   TIGASE_CONFIG=/etc/tigase/tigase.config
   TIGASE_OPTIONS=
   TIGASE_PARAMS=

   PIDFILE=
   TIGASE_CONSOLE_LOG=
   …

-  ``USERNAME`` - Username running Tigase, should have su permissions.

-  ``USERGROUP`` - The usergroup of the username.

-  ``NAME`` - OS name for Tigase program.

-  ``DESC`` - Optional description.

-  ``TIGASE_HOME`` - The location of your Tigase Server installation directory.

-  ``TIGASE_CONFIG`` - The location of your tigase-server.xml file relative (old configuration format)

-  ``TIGASE_OPTIONS`` - command line arguments passed to Tigase server (which may include path to ``init.properies`` (if correct ``tigase.conf`` configuration will be found then it will translate to ``TIGASE_OPTIONS=" --property-file etc/config.tdsl "``

-  ``TIGASE_PARAMS`` - Parameters passed to command line when launching Tigase.

-  ``PIDFILE`` - Location of Tigase PID file if you wish to use custom directory. Default will be located in ``/var/run/tigase/tigase.pid`` or under (in this case relative to tigase home directory)\ ``logs/tigase.pid``.

-  ``TIGASE_CONSOLE_LOG`` - Location of Tigase Server console log file if you wish to use a custom directory. Default will be located in /logs directory, failing that /dev/null.

Afterwards we need to install service in the system with following command:

.. code:: bash

   update-rc.d tigase defaults


Running Tigase as a system service
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

There are a number of benefits to running Tigase as a service, one of which is to ensure that the program will run even in the event of a power outage or accidental server restart, Tigase will always be up and running.


For systemd-based linux distributions
''''''''''''''''''''''''''''''''''''''

Once installation is complete you may start Tigase as a typical systemd service using following command:

.. code:: bash

   sudo systemctl start tigase-server

To stop it, you may run following command:

.. code:: bash

   sudo systemctl stop tigase-server

It is also possible to enable service, to make it start during startup of the operating system:

.. code:: bash

   sudo systemctl enable tigase-server


For other linux distributions
''''''''''''''''''''''''''''''

Once installation is complete, you should be able to start Tigase using the following command:

.. code:: bash

   service tigase start

Tigase should begin running in the background. Since Tigase is now installed as a service, it can be controlled with any of the service commands, such as:

-  ``service tigase stop``

-  ``service tigase restart``

2.5.8. Shutting Down Tigase
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Although Tigase XMPP Server can be terminated by ending the process, it is preferred and recommended to use it’s own shutdown scripts instead. Not only does this allow for a proper purge of Tigase form the system, but allows for all shutdown functions to operate, such as amending logs and completing statistics. To trigger a shutdown of Tigase server, the following command can be used from the tigase directory:

.. code:: bash

   ./scripts/tigase.sh stop

You may specify the config file if you want, but it will make no differences

This will:

-  Begin shutdown thread

-  Stop accepting new connections

-  Close all current connections

-  Collect runtime statistics

-  Write statistics to log

-  Dump full stacktrace to a file

-  Run GC and clear from memory


Shutdown statistics
~~~~~~~~~~~~~~~~~~~~

Upon shutdown, statistics for the server’s runtime will be appended to the log file. For a description of the statistics and what they mean, refer to the `Statistics Description <#statsticsDescription>`__ portion of the documentation.

Shutdown StackTrace Dump
~~~~~~~~~~~~~~~~~~~~~~~~~

To aid with troubleshooting purposes, the full stacktrace will be dumped to a seperate file located at $serverdir/logs/threads-dump.log.# Stacktrace logs will follow the same log file numbering scheme described in `Log file description <#logs>`__.

This feature is enabled by default, however you may disable this by adding the following to your ``config.tdsl`` file:

.. code:: dsl

   'shutdown-thread-dump' = false


Shutting Down Cluster Nodes
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Starting with v8.0.0 you can now shut down individual cluster nodes without shutting down the whole server. This command will use the *SeeOtherHost* strategy to direct traffic to other nodes and update the cluster map to gracefully shut down the single node

Shutting down individual nodes can be done VIA Ad-hoc command and fill out the response forms. The command is available from message-router as http://jabber.org/protocol/admin#shutdown.

2.5.8. Shutting Down Tigase
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Although Tigase XMPP Server can be terminated by ending the process, it is preferred and recommended to use it’s own shutdown scripts instead. Not only does this allow for a proper purge of Tigase form the system, but allows for all shutdown functions to operate, such as amending logs and completing statistics. To trigger a shutdown of Tigase server, the following command can be used from the tigase directory:

.. code:: bash

   ./scripts/tigase.sh stop

You may specify the config file if you want, but it will make no differences

This will:

-  Begin shutdown thread

-  Stop accepting new connections

-  Close all current connections

-  Collect runtime statistics

-  Write statistics to log

-  Dump full stacktrace to a file

-  Run GC and clear from memory


Shutdown statistics
~~~~~~~~~~~~~~~~~~~~

Upon shutdown, statistics for the server’s runtime will be appended to the log file. For a description of the statistics and what they mean, refer to the `Statistics Description <#statsticsDescription>`__ portion of the documentation.


Shutdown StackTrace Dump
~~~~~~~~~~~~~~~~~~~~~~~~~~~

To aid with troubleshooting purposes, the full stacktrace will be dumped to a seperate file located at $serverdir/logs/threads-dump.log.# Stacktrace logs will follow the same log file numbering scheme described in `Log file description <#logs>`__.

This feature is enabled by default, however you may disable this by adding the following to your ``config.tdsl`` file:

.. code:: dsl

   'shutdown-thread-dump' = false


Shutting Down Cluster Nodes
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Starting with v8.0.0 you can now shut down individual cluster nodes without shutting down the whole server. This command will use the *SeeOtherHost* strategy to direct traffic to other nodes and update the cluster map to gracefully shut down the single node

Shutting down individual nodes can be done VIA Ad-hoc command and fill out the response forms. The command is available from message-router as http://jabber.org/protocol/admin#shutdown.

2.5.9. Upgrading to v8.0.0 from v7.1.0
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

There have been a number of changes to the user and auth databases since v7.1.0. As a result, if you are upgrading from older versions, you will need to follow this guide.

.. Note::

   We recommend installing Tigase XMPP Server 8.0.0 in a separate directory.


Backup your data
~~~~~~~~~~~~~~~~~

As with any migration it is highly recommended that you backup your repository before conducting any upgrade operations.

For MySQL databases:

.. code:: bash

   mysqldump [dbname] --routines -u [username] -p [password] > [filename].sql


Setup Tigase XMPP Server 8.0.0
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

After downloading Tigase XMPP Server 8.0.0 from our website, or using wget, extract the files to a separate directory.

Copy the ``tigase.conf`` and ``init.properties`` files from the old directory to v8.0.0 directory.

.. code:: bash

   cd tigase-server-8.0.0
   cp ../tigase-server/etc/tigase.conf etc/
   cp ../tigase-server/etc/init.properties etc/

Import the database.

.. code:: bash

   mysql -h [host address] [dbname] -u [username] -p [password] < [filename].sql
   mysql -h 198.27.120.213 tigase_tpub -u USERNAME -p <../tpub.2017-05-30.sql
   Enter password:


Upgrade configuration file
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Tigase XMPP Server has a utility that can be called using ``upgrade-config`` that will update your old ``init.properties`` file and create a new file using DSL.

.. code:: bash

   ./scripts/tigase.sh upgrade-config etc/tigase.conf

When everything is ready it will printout following information

::

   ===============================================================================
     Configuration file etc/init.properties was converted to DSL format.
     Previous version of a configuration file was saved at etc/init.properties.old
   ===============================================================================


Connect new database
~~~~~~~~~~~~~~~~~~~~~

Edit your new ``config.tdsl`` file to connect to the new database you created during the import step.

.. code:: dsl

   dataSource {
       default () {
           uri = 'jdbc:mysql://localhost/tigase_tpub?user=tigase_user&password=mypass'
       }
   }
   userRepository {
       default () {}
   }
   authRepository {
       default () {}
   }

Upgrade Database schema
~~~~~~~~~~~~~~~~~~~~~~~~

Upgrading database schemas is now possible using the ``upgrade-schema`` option. Do this now.

.. code:: bash

   ./scripts/tigase.sh upgrade-schema etc/tigase.conf


.. Warning::

    Your database schema MUST be v8 or conversion will not occur properly!

You will be asked the following prompts:

.. code:: bash

   Database root account username used to create tigase user and database at 198.27.120.213 :

   Database root account password used to create tigase user and database at 198.27.120.213 :

Upon success, you should see the following:

.. code:: bash

   =============================================================================
           Schema upgrade finished

     Data source: default with uri
   jdbc:mysql://HOST/DATABASE?user=USERNAME&password=PASSWORD
           Checking connection to database ok
           Checking if database exists     ok
           Loading schema: Tigase XMPP Server (Core), version: 8.0.0       ok
           Loading schema: Tigase Message Archiving Component, version: 1.3.0      ok
           Loading schema: Tigase MUC Component, version: 2.5.0    ok
           Loading schema: Tigase PubSub Component, version: 3.3.0 ok
           Adding XMPP admin accounts      warning
                   Message: Error: No admin users entered
           Post installation action        ok

   =============================================================================

Start Tigase!


Help?
~~~~~

Both ``upgrade`` commands also have a build in help function, they can be called if needed from the command line. You can also run these commands for help.

::

   scripts/tigase.sh upgrade-config etc/tigase.conf --help
   scripts/tigase.sh upgrade-schema etc/tigase.conf --help


Upgrade/Restore with a script [experimental!]
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

To make upgrade process easier it’s possible to utilize `tigase-upgrade.sh <files/tigase-upgrade.sh>`__ \*nix shell script. It permits upgrading to new version (supports downloading version from provided URL).

It’s usage is as follows:

.. code:: bash

   ./tigase-upgrade.sh {upgrade|rollback} install_package install_directory [tar|dir]

Where: \* ``{upgrade|rollback}`` - defines whether to perform upgrade or rollback to previous version \* ``install_package`` - package to which perform upgrade (can be URL) in case of upgrade or backed-up installation (from which we want to restore) in case of rollback \* ``install_directory`` - destination directory (both in upgrade and rollback); can be symlink in which case it will be preserved with upgraded/restored path as target \* ``[tar|dir]`` - (optional) type of backup (either simply copy directory or also archive it using ``tar`` command); by default ``dir`` is used.

To upgrade installation to version ``tigase-server-8.0.0-SNAPSHOT-b5285-dist-max.tar.gz`` execute the script as follows:

.. code:: bash

   $ ./tigase-upgrade.sh upgrade tigase-server-8.0.0-SNAPSHOT-b5285-dist-max.tar.gz tigase-server

To rollback from ``tigase-server-8.0.0-SNAPSHOT-b5264_backup-18-11-05_1712`` backup execute script as follows:

.. code:: bash

   bash -x ./tigase-upgrade.sh rollback tigase-server-8.0.0-SNAPSHOT-b5264_backup-18-11-05_1712/ tigase-server

2.6. Configuration
-------------------

When the user tries to setup the client for the first time he comes across 2 configuration files: ``tigase.conf`` and ``config.tdsl`` in the ``/etc`` folder. Here is a brief explanation what all those files are about and in other sections you can learn all the details needed to configure the server.

1. `config.tdsl <#dslConfig>`__ file is a simple text file with server parameters in form: **key** = **value**. When the XML configuration file is missing the Tigase server reads ``config.tdsl`` file and uses parameters found there as defaults for generation of the XML file. Therefore if you change the ``config.tdsl`` file you normally have to stop the server, remove the XML file and start the server again. All the settings from the ``config.tdsl`` are read and applied to the XML configuration. The properties file is easy to read and very safe to modify. At the moment this is the recommended way change the server configuration.

2. `tigase.conf <#manualconfig>`__ is the Tigase server startup configuration. It is actually not used by the server itself. It rather contains operating system settings and environment parameters to correctly run the `Java Virtual Machine <http://java.sun.com/>`__. It is only useful on the unix-like systems with Bash shell. If you run the server on MS Windows systems ``tigase.bat`` and ``wrapper.conf`` files are used instead. The ``tigase.conf`` file is read and loaded by the ``scripts/tigase.sh`` shell script which also scans the operating system environment for Java VM and other tools needed.

2.6.1. DSL file format
^^^^^^^^^^^^^^^^^^^^^^^

In previous Tigase XMPP Server releases configuration was stored in properties based configuration file. From Tigase XMPP Server 8.0.0 release it will be required to use new DSL based configuration file format. This file format was inspired by Groovy language syntax and new core feature of Tigase XMPP Server - Tigase Kernel Framework.

why new format?
~~~~~~~~~~~~~~~~~

In properties configuration format each line contained key and value with optional definition of type of stored value:

.. code::

   c2s/ports[i]=5222,5223

where ``c2s/ports`` was name of property, ``[i]`` defined that type of value is array of integers, and ``5222,5223`` was comma separated list of values.

This format worked but in fact ``c2s/ports`` was not name of property you configured but key which was later split on ``/`` char to parts which defined by names path to property which name was in last part.From that you can see that it was domain based setting of properties.

Except from this multi-part keys we also used properties starting with ``--`` which were global properties accessible for every part of application, i.e.: to add new component and set some properties you needed to write:

.. code::

   --comp-name-1=pubsub
   --comp-class-1=tigase.pubsub.PubSubComponent
   pubsub/test[B]=true
   pubsub/pubsub-repo-url="jdbc:XXXX:XXXX/db_name"

This lead to mistakes like duplicated definition of name and class for same number of component or redefined property value in other place of a configuration file - especially in cases where configuration was big.

In this configuration structure it was hard to tell where is configuration for particular component or what databases this installation uses. This could be defined all over the file.

In this release we are introducing Tigase Kernel Framework, which allows to configure beans in configuration file and even define usage of new beans loaded from external jars which can modify behavior of Tigase components. This would make configuration file even more complex, difficult and less readable.

What is DSL?
~~~~~~~~~~~~~

DSL stands for domain-specific language - in this case language created for storage of configuration.

Now we use domain based configuration which means that our configuration file is not a flat key=value storage but it defines objects, it's properties and assigned values.

To illustrate it better let's start with a simple example. In properties file in order to configure PubSub component named ``pubsub`` you would use following properties:

.. code::

   --comp-name-1=pubsub
   --comp-class-1=tigase.pubsub.PubSubComponent
   pubsub/test[B]=true

In DSL based configuration this would be replaced by following block

.. code::

   pubsub (class: tigase.pubsub.PubSubComponent) {
       # comment
       test = true
   }


in which we define bean with name `pubsub` and set it's class inside ``()`` block to ``tigase.pubsub.PubSubComponent``.
We also use block between ``{}`` chars to define properties which are related to bean.
Which means this properties will be passed only to this instance of Tigase PubSub Component, same as it was before where we needed to add prefix.
Entries after ``\#`` are comments, to pass ``#`` you need to wrap whole part containing it in ``''``, ie. ``'test#242'``

.. WARNING:: 
    If a string value assigned to a property contains any char from a following list ``=:,[]#+-*/`` it needs to be wrapped in a ``''``.

Why DSL?
~~~~~~~~

DSL configuration format provides a number of advantages over the old system of configuration. All configurations for components are related in a single block, so they are not spread out over several different lines. No need for long property names, no longer have to invoke a long string of settings for multiple values. Support is provided for environment variables. No longer need to escape certain characters, making settings far more readable at a glance. Values may be set using basic calculations, such as ``100 * 200 * 2`` rather than ``40000``. Parameter type values are no longer necessary, no more [i], [S], [B] etc.. Comma separated values can now be simplified lists with separate entries being able to be in multiple lines.

Although the format may seem more complex, looking like a section of java code, the formatting is consistent and can be far more readable. After some experience with DSL format, you'll find it's far more intuitive and user friendly than it may appear. Of course if there's any real confusion, Tigase can automatically convert old style properties files to the DSL format using the following command:

.. code-block:: bash

   ./scripts/tigase.sh upgrade-config etc/tigase.conf

Setting property
'''''''''''''''''

To set property you just write property name followed by `=` and value to set. This is always done in context of bean which configuration property you want to set.

.. code-block::

   test=true

It is also possible to set property in main context by placing property outside of any context.
This sets property which value is available to access by any bean.

Setting global property
''''''''''''''''''''''''
Like in properties file it is still possible to use property names starting with ``--`` without any context or any other properties at global scope. Format is the same as in case of setting property but they are defined without scope (in global scope). This properties are global and accessible by any bean but also set as system property in JVM.

Defining bean
''''''''''''''

You can configure bean by using following format:

.. code:: bash

   beanName (class: className, active: activeValue, exportable: exportableValue) {
       # scope of bean properties
   }

where ``beanName`` is name under which you want to configure bean.
`beanName` must be wrapped in ``''``, if ``beanName`` contains characters like ``=:,[]#+-*/`` and is recommended, if ``beanName`` is numeric only.

Inside block between ``(` and `)`` you can define:

* ``class`` which will be used as a bean, in example above we set class as ``className``. *_(default: if you try to configure bean under name which has default class assigned with it in Tigase framework then this assigned class will be used. In other case you need to pass name of class to use as a bean)_*
* ``active`` (boolean) whether you want the bean to be active or not (beans with ``active`` set to ``false`` are not loaded). *_(default: true)_*
* ``exportable`` (boolean) defines if this bean should be exported and available for use for beans in inner scopes. This is advanced option in most cases it is recommended to omit this field in configuration. *_(default: false)_*

Spaces between ``beanName`` and block between ``()`` is optional as well as space between block ``()`` and block ``{}``.
It is recommended that properties of bean would be placed in separate lines with indentation and first property will be placed in new line.

.. important::

   Usage of ``()`` block is very important. When this block is used in configuration it automatically sets ``active`` property of bean definition for bean for which it is used to to `true`. This is done due to fact that default value of ``active`` is ``true``.

   If you omit it in configuration, you will set bean configuration but it may remain ``inactive``. In this state bean will not be loaded and as a result will not be used by Tigase XMPP Server.


Configuring bean
'''''''''''''''''
If you know that bean is defined and you do not want to change it's activity or class then you can just pass properties to configure bean in following way:

.. code::

   beanName {
       # scope of bean properties
       test = true
   }


where ``beanName`` is name of bean to configure and `test` is name of property to set to ``true`` in this bean.

Format of values
'''''''''''''''''

In properties based configuration file every property was defined as a string and only by defining expected format it was properly converted to expected value. In DSL it is possible to set values in two ways:

as an object
   Using this format you set list as a list and integer is set as an integer.

.. table::

+-------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| Type        | Description                                                                                                                                                                                                            |
+=============+========================================================================================================================================================================================================================+
| **string**  | Wrap it in ``''``, ie. to set ``test`` as string you use ``'test'``                                                                                                                                                    |
+-------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| **integer** | Just put value, ie. to set ``543`` use ``543``                                                                                                                                                                         |
+-------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| **long**    | Put value and follow it with ``L``, ie. to set ``23645434`` as long use ``23645434L``                                                                                                                                  |
+-------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| **float**   | Put value and follow it with ``f``, ie. to set ``231.342`` use ``231.342f``                                                                                                                                            |
+-------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| **boolean** | To set value just use ``true`` or ``false``                                                                                                                                                                            |
+-------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| **list**    | Lists can be of many types and to make it simple we decided to use as a comma separated list of values in proper format wrapped in ``[]``.                                                                             |
|             |                                                                                                                                                                                                                        |
|             | -  of strings - ``[ 'alfa', 'beta', 'gamma' ]``                                                                                                                                                                        |
|             |                                                                                                                                                                                                                        |
|             | -  of integers - ``[ 1, 2, 3, 4]``                                                                                                                                                                                     |
|             |                                                                                                                                                                                                                        |
|             | You can write it in multiple lines if you want:                                                                                                                                                                        |
|             |                                                                                                                                                                                                                        |
|             | ::                                                                                                                                                                                                                     |
|             |                                                                                                                                                                                                                        |
|             |    [                                                                                                                                                                                                                   |
|             |        'alfa'                                                                                                                                                                                                          |
|             |        'beta'                                                                                                                                                                                                          |
|             |        'gamma'                                                                                                                                                                                                         |
|             |    ]                                                                                                                                                                                                                   |
+-------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| **map**     | Maps can be written as a block of properties wrapped in ``{}``. This format of map is the same as used for passing configuration to bean properties. Keys and values can be written in separate lines *(recommended)*: |
|             |                                                                                                                                                                                                                        |
|             | ::                                                                                                                                                                                                                     |
|             |                                                                                                                                                                                                                        |
|             |    {                                                                                                                                                                                                                   |
|             |        test = true                                                                                                                                                                                                     |
|             |        ssl = false                                                                                                                                                                                                     |
|             |        ssl-certificate = '/test/cert.pem'                                                                                                                                                                              |
|             |        another-map = {                                                                                                                                                                                                 |
|             |            key = 'value'                                                                                                                                                                                               |
|             |        }                                                                                                                                                                                                               |
|             |    }                                                                                                                                                                                                                   |
|             |                                                                                                                                                                                                                        |
|             | or in single line *(separation with spaces is not required)*:                                                                                                                                                          |
|             |                                                                                                                                                                                                                        |
|             | ::                                                                                                                                                                                                                     |
|             |                                                                                                                                                                                                                        |
|             |    { test = true, ssl = false, ssl-certificate = '/test/cert.pem' }                                                                                                                                                    |
+-------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

as a plain string
   Very similar to properties based configuration, in fact values are passed in same format and later are converted to correct type by checking type expected by bean. *(Not recommended)*

.. table::

+-------------+-----------------------------------------------------------------------------------------------+
| Type        | Description                                                                                   |
+=============+===============================================================================================+
| **string**  | Just put value, ie. to set ``test`` use ``test``                                              |
+-------------+-----------------------------------------------------------------------------------------------+
| **integer** | Just put value, ie. to set ``543`` use ``543``                                                |
+-------------+-----------------------------------------------------------------------------------------------+
| **long**    | Put value, ie. to set ``23645434`` as long use ``23645434``                                   |
+-------------+-----------------------------------------------------------------------------------------------+
| **float**   | Put value, ie. to set ``231.342`` use ``231.342``                                             |
+-------------+-----------------------------------------------------------------------------------------------+
| **boolean** | To set value just use ``true`` or ``false``                                                   |
+-------------+-----------------------------------------------------------------------------------------------+
| **list**    | List needs to be written as comma separated list of values, ie. ``test,abc,efg`` or ``1,2,3`` |
+-------------+-----------------------------------------------------------------------------------------------+
| **map**     | Not possible                                                                                  |
+-------------+-----------------------------------------------------------------------------------------------+


Using values from System Properties and Environment Variables
''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''

Now it is possible to use values of `system properties <https://docs.oracle.com/javase/tutorial/essential/environment/sysprop.html>`__ and `environment variables <https://docs.oracle.com/javase/tutorial/essential/environment/env.html>`__ and assign them to bean properties. For this purpose we added functions which can be used in DSL and which will return values of:

system property
   ``prop('property-name')`` or ``prop('property-name','default value')``

environment variable
   ``env('variable-name')``

**Example of setting value of system property and environment variable to bean ``user``.**

.. code::

   user {
     name = env('USER')
     home = prop('user.home')
     paths = [ prop('user.home'), prop('user.dir') ]
   }

..

.. Warning::

    For properties which accepts lists it is not allowed to set value using variable/property with comma separated values like ``value1,value2`` wrapped in ``[]``, ie. ``property = [ env('some-variable') ]``. It needs to be set in following way ``property = env('some-variable')``
 
Computed values
''''''''''''''''

With DSL configuration format we introduce support for computable values for properties. It is now possible to set value which is result of a computation, ie. concatenation of a strings or very simple mathematical expression. We currently support only following mathematical operations:

-  add

-  subtract

-  multiply

-  divide

**Example of setting environment variable related path and computed timeout.**

.. code::

   bean {
     # setting path to `some-subdirectory` of user home directory
     path = prop('user.home') + '/some-subdirectory/'

     # setting timeout to 5 minutes (setting value in milliseconds)
     timeout = 5L * 60 * 1000
     # previously it would need to be configured in following way:
     # timeout = 300000L
   }

..

   warning::

    For properties which accepts lists it is not allowed to set value using computed values with comma separated values like ``value1,value2`` wrapped in ``[]``, ie. ``property = [ env('some-variable') + ',other-value' ]``. It needs to be set in following way ``property = env('some-variable') + ',other-value'``.


Period / Duration values
'''''''''''''''''''''''''

Some configuration options allow control of execution of tasks with particular period or within certain duration. DSL file format accepts strings denoting particular amount of time, which follows Java’s native structures (see: `Period <https://docs.oracle.com/javase/8/docs/api/java/time/Period.html#parse-java.lang.CharSequence->`__ and `Duration <https://docs.oracle.com/javase/8/docs/api/java/time/Duration.html#parse-java.lang.CharSequence->`__ for detailed explanation).

-  ``Duration`` formats accepted are based on the ISO-8601 duration format ``PnDTnHnMn.nS`` with days considered to be exactly 24 hours, for example:

   -  ``PT20.345S`` - 20.345 seconds

   -  ``PT15M`` - 15 minutes (where a minute is 60 seconds)

   -  ``PT10H`` - 10 hours (where an hour is 3600 seconds)

   -  ``P2D`` - 2 days (where a day is 24 hours or 86400 seconds)

   -  ``P2DT3H4M`` - 2 days, 3 hours and 4 minutes

-  ``Period`` format is based on the ISO-8601 period formats PnYnMnD and PnW, for example, the following are valid inputs:

   -  ``P2Y`` - 2 years

   -  ``P3M`` - 3 months

   -  ``P4W`` - 4 weeks

   -  ``P5D`` - 5 days

   -  ``P1Y2M3D`` - 1 year, 2 months, 3 days

   -  ``P1Y2M3W4D`` - 1 year, 2 months, 3 weeks, 4 days


Example configuration file in DSL
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. code:: dsl

   # Enable cluster mode
   --cluster-mode = true
   # Enable debugging for server and xmpp.impl
   --debug = 'server,xmpp.impl'
   # Set list of virtual hosts (old way)
   --virt-hosts = 'example.com,test-1.example.com,test-2.example.com'

   # Configure list of administrator jids
   admins = [ 'admin@zeus', 'http@macbook-pro-andrzej.local' ]
   # Set config type
   config-type = '--gen-config-def'

   # Configure dataSource bean with database configuration
   dataSource {
       # Configure default data source (using default implementation so class is omitted)
       default () {
           uri = 'jdbc:postgresql://127.0.0.1/tigase?user=test&password=test&autoCreateUser=true'
       }

       # Configure data source with name exaple.com (will be used by domain example.com)
       'example.com' () {
           uri = 'jdbc:mysq://127.0.0.1/example?user=test&password=test&autoCreateUser=true'
       }
   }

   # Configure C2S component
   c2s {
       # Enable Stream Management bean
       'urn:xmpp:sm:3' () {}

       # Register tigase.server.xmppclient.SeeOtherHostDualIP as seeOtherHost bean
       seeOtherHost (class: tigase.server.xmppclient.SeeOtherHostDualIP) {}

       # Add additional port 5224 which is SSL port and disable port 5223
       connections () {
           '5224' () {
                socket = ssl
             }
           '5223' (active: false) {}
       }
   }

   # Configure HTTP API component
   http {
       # Set list of API keys
       api-keys = [ 'test1234', 'test2356' ]
       rest {
           # Set value of environment property as a path to look for REST scripts
           rest-scripts-dir = env('TIGASE_REST_SCRIPTS_DIR')
       }
   }

   # Register pubsub-2 (class is passed as pubsub-2 name do not have default class assigned)
   pubsub-2 (class: tigase.pubsub.cluster.PubSubComponentClustered) {
       # Set configuration bean properties
       pubsubConfig {
           persistentPep = true
       }
       # Use tigase.pubsub.cluster.ClusteredNodeStrategy as advanced clustering strategy
       strategy (class: tigase.pubsub.cluster.ClusteredNodeStrategy) {}
   }

   # Configure Session Manager
   sess-man {
       # Here we enable pep, urn:xmpp:mam:1 processors and disable message-archive-xep-0136 processor
       pep () {}
       'urn:xmpp:mam:1' () {}
       message-archive-xep-0136 (active: false) {}

       # Define class used as clustering strategy (it is different than default so class is required)
       strategy (class: tigase.server.cluster.strategy.OnlineUsersCachingStrategy) {}
   }


Default configuration
~~~~~~~~~~~~~~~~~~~~~~

Tigase XMPP Server is packaged with a basic ``config.tdsl`` file that tells the server to start up in setup mode.

.. code:: dsl

   'config-type' = 'setup'

   http () {
       setup () {
           'admin-user' = 'admin'
       'admin-password' = 'tigase'
       }
   }

This tells Tigase to operate in a setup mode, and tells the http component to allow login with the username and password admin/tigase. With this you can enter the setup process that is covered in `this section <#webinstall>`__.

There are other options for config-type: ``default``, ``session-manager``, ``connection-managers``, and ``component``. For more information, visit `Config Type <#configType>`__ property description.


2.6.2. Startup File for tigase.sh - tigase.conf
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Property file names for ``tigase.sh`` startup script is a second parameter for the startup script. It can be skipped if environmental variables are set in different location or in different way.

Config file for startup script simply sets number of environment variables with the location of required components. Possible variables to set in this file are:

-  ``JAVA_HOME`` - location of Java installation home directory. **Must be set**.

-  ``TIGASE_HOME`` - location of Tigase installation home directory. *By default script try to find this location by searching directories from the location where the script has been run.*

-  ``TIGASE_CONSOLE_LOG`` - file to which all console messages will be redirected if server is run in background. By default it will be: ``TIGASE_HOME/logs/tigase-console.log``. **If this file/directory is not writable by Tigase process all console messages will be redirected to /dev/null**

-  ``TIGASE_PID`` location of the file with server PID number. By default it will be ``TIGASE_HOME/logs/tigase.pid``.

-  ``JAVA_OPTIONS`` - options for JVM like size of RAM allocated for the JVM, properties and so on.

-  ``TIGASE_OPTIONS`` - (optional) additional options for Tigase server program. You can tweak initial parameters for your environment here. If you want to specify custom location of your configuration file you should use ``--config-file <path/to/config.tdsl>`` configuration

Sample file to run **Tigase** with **PostgreSQL** database may look like:

.. code:: bash

   ENC="-Dfile.encoding=UTF-8 -Dsun.jnu.encoding=UTF-8"
   DRV="-Djdbc.drivers=org.postgresql.Driver"
   JAVA_OPTIONS="${ENC} ${DRV} -server -Xms100M -Xmx100M "
   CLASSPATH=""
   TIGASE_CONFIG="tigase-pgsql.xml"
   TIGASE_OPTIONS=" "

Please note encoding settings. JVM by default uses encoding set in operating system environment. XMPP protocol, however uses ``UTF-8`` for all data processing. So the ENC settings enforces ``UTF-8`` encoding for all operations.

Another significant setting is \\'**CLASSPATH**'. It is intentionally set to an empty string. The **tigase.sh** startup script builds the **CLASSPATH** on it’s own from files found in **jars/** and **libs/** directories. It is advised to set the **CLASSPATH** to the empty string because the Tigase server scans all available classes to find all components and plugins implementation. If the **CLASSPATH** contains lots of libraries which are not used anyway it can cause a long startup time and high system loads.

2.6.3. Linux Settings for High Load Systems
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

There are a few basic settings you have to adjust for high load systems to make sure the server has enough resources to handle a big number of network connections.

The main parameter is a maximum number of opened files allowed for the process to keep at the same time. Each network connection uses a file handler, therefore if the limit is too low you can quickly run out of handlers and the server can not accept any more connections.

This limit is set on 2 levels - on the kernel level (``fs.file-max``) and on the system level (``nofile``).

Another kernel property which can be important in certain configurations (like transports installations or when you use proxy for Bosh connections) is: ``net.ipv4.ip_local_port_range``. This parameter can be set the same way as the ``fs.file-max`` property.

fs.file-max
~~~~~~~~~~~~

The ``fs.file-max`` kernel property is set via sysctl command. You can see current settings by executing the command:

.. code:: sh

   # sysctl fs.file-max
   fs.file-max = 358920

If you plan to run high load service with large number of server connections, then this parameter should be at least as twice big as the number of network connections you expect to support. You can change this setting by executing the command:

::

   # sysctl -w fs.file-max=360000
   fs.file-max = 360000


net.ipv4.ip_local_port_range
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

You can see current settings by executing the command:

.. code:: sh

   # sysctl net.ipv4.ip_local_port_range
   net.ipv4.ip_local_port_range = 32768    61000

You can change this setting by executing the command:

.. code:: sh

   # sysctl -w net.ipv4.ip_local_port_range="1024 65000"
   net.ipv4.ip_local_port_range = 1024 65000

TCP_keepalive
~~~~~~~~~~~~~~~

According to `Using TCP keepalive to Detect Network Errors <http://www.gnugk.org/keepalive.html>`__ and `TCP Keepalive HOWTO <https://tldp.org/HOWTO/TCP-Keepalive-HOWTO/usingkeepalive.html>`__ some keepalive settings should be changed to improve reliability - it will enable keep alive functionality (checking if the connection is established and valid) and, by decreasing times and interval - will make detection of broken connections faster.

.. code:: sh

   # sysctl -w net.ipv4.tcp_keepalive_time="60"
   net.ipv4.tcp_keepalive_time = 60
   # sysctl -w net.ipv4.tcp_keepalive_probes="3"
   net.ipv4.tcp_keepalive_probes = 3
   # sysctl -w net.ipv4.tcp_keepalive_intvl="90"
   net.ipv4.tcp_keepalive_intvl = 90
   # sysctl -w net.ipv4.tcp_retries2=4
   net.ipv4.tcp_retries2 = 4


/etc/sysctl.conf
~~~~~~~~~~~~~~~~~~

The above commands let the system remember new settings until the next system restart. If you want to make the change permanent you have to edit the file: ``/etc/sysctl.conf`` and add the property at the end of the file:

.. code:: sh

   fs.file-max=360000
   net.ipv4.ip_local_port_range=1024 65000
   net.ipv4.tcp_keepalive_time=60
   net.ipv4.tcp_keepalive_probes=3
   net.ipv4.tcp_keepalive_intvl=90
   net.ipv4.tcp_retries2=4

It will be automatically loaded next time you start the server.

Command:

.. code:: sh

   # sysctl -p

Causes the ``/etc/systcl.conf`` to be reloaded which is useful when you have added more parameters to the file and don’t want to restart the server.

nofile
~~~~~~~

This is the property used by the system limits. For example running the command ``ulimit -a`` shows you all limits set for the current user:

.. code:: sh

   # ulimit -a
   core file size          (blocks, -c) 0
   data seg size           (kbytes, -d) unlimited
   file size               (blocks, -f) unlimited
   pending signals                 (-i) 38912
   max locked memory       (kbytes, -l) 32
   max memory size         (kbytes, -m) unlimited
   open files                      (-n) 40960
   pipe size            (512 bytes, -p) 8
   POSIX message queues     (bytes, -q) 819200
   stack size              (kbytes, -s) 8192
   cpu time               (seconds, -t) unlimited
   max user processes              (-u) 38912
   virtual memory          (kbytes, -v) unlimited
   file locks                      (-x) unlimited

To make it even more interesting and more complex, there are 2 types of system limits: **soft limit** which can be temporarily exceeded by the user and **hard limit** which can not be exceeded. To see your **hard limit** execute command:

.. code:: sh

   # ulimit -a -H
   core file size          (blocks, -c) unlimited
   data seg size           (kbytes, -d) unlimited
   file size               (blocks, -f) unlimited
   pending signals                 (-i) 38912
   max locked memory       (kbytes, -l) 32
   max memory size         (kbytes, -m) unlimited
   open files                      (-n) 40960
   pipe size            (512 bytes, -p) 8
   POSIX message queues     (bytes, -q) 819200
   stack size              (kbytes, -s) unlimited
   cpu time               (seconds, -t) unlimited
   max user processes              (-u) 38912
   virtual memory          (kbytes, -v) unlimited
   file locks                      (-x) unlimited

The hard limits are usually bigger then the soft limits or sometimes the same.

For us the most important parameter is: **open files**. You can change the property in file: ``/etc/security/limits.conf``. You have to append 2 following lines to the end of the file:

.. code:: sh

   jabber               soft    nofile         350000
   jabber               hard    nofile         350000

Where the ``jabber`` is the user name of the account running you IM service. You can also set the limits for all users on the machine in a following way:

.. code:: sh

   *               soft    nofile         350000
   *               hard    nofile         350000

For those changes to make an effect you have to logout from the modified account and login again. New limits should be applied.


su and init script
~~~~~~~~~~~~~~~~~~~~

If one intends to use init scripts for startup purposes (or simply wants to be able to start the server utilizing su command) it’s necessary to adjust PAM configuration by modifying /etc/pam.d/su file and uncomment following line:

.. code:: sh

   session    required   pam_limits.so

Afterwards the init scripts will respect configured limits.

2.6.4. JVM settings and recommendations
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Tigase configuration file ``tigase.conf`` (described in more detail in `??? <#manualconfig>`__) mentioned a couple of environmental variables which are related to the operation of the JVM. In this guide we would like to expound on those configuration options and provide hints for the optimal settings.

Settings included in the ``etc/tigase.conf`` are as follows:

.. code:: bash

   #GC="-XX:+UseBiasedLocking -XX:+UseConcMarkSweepGC -XX:+UseParNewGC -XX:NewRatio=2 -XX:+CMSIncrementalMode -XX:-ReduceInitialCardMarks -XX:CMSInitiatingOccupancyFraction=70 -XX:+UseCMSInitiatingOccupancyOnly"
   #EX="-XX:+OptimizeStringConcat -XX:+DoEscapeAnalysis -XX:+UseNUMA"

   #GC_DEBUG=" -XX:+PrintTenuringDistribution -XX:+PrintGCDetails -XX:+PrintGCDateStamps -XX:+PrintGCTimeStamps -Xloggc:logs/jvm.log -verbose:gc "

   #PRODUCTION_HEAP_SETTINGS=" -Xms5G -Xmx5G " # heap memory settings must be adjusted on per deployment-base!
   JAVA_OPTIONS="${GC} ${GC_DEBUG} ${EX} ${ENC} ${DRV} ${JMX_REMOTE_IP} -server ${PRODUCTION_HEAP_SETTINGS} ${DNS_RESOLVER} ${INTERNAL_IP} ${EXTERNAL_IP}  -XX:MaxDirectMemorySize=128m "

And while this file utilizes bash variables, JVM configuration options can be used in the same manner on all operating systems.

The guide will consists of two main parts - memory settings and Garbage Collector tweaks descriptions and hints.

We recommend using ``-server`` JVM parameter in all cases.

Heap Sizing
~~~~~~~~~~~~

For the non-production deployments (development or stating environments) we recommend using default memory settings of the JVM (which depends on the underlaying operating system), which result i automatic memory allocation and, by the rule of thumb - are the safest in such environments.

For the production environments we recommend a fixed size HEAP - both initial and maximum size, which can be set with (respectively)``-Xms`` and ``-Xmx`` JVM flags - ideally to the same value (which should be roughly 95% of the available memory, if Tigase will be the only service on the machine) to avoid allocation and deallocation.

For convenience it’s possible to uncomment line with ``PRODUCTION_HEAP_SETTINGS`` and adjust parameters accordingly.

Memory consideration - total usage
'''''''''''''''''''''''''''''''''''

The HEAP size is not the only thing that affects JVM memory usage. When trying to size accordingly for your usage and machine specification you have to consider other factors that count towards total: loaded classes, threads' stack, JIT code cache, garbage collector and others. In principle consider following equation:

::

   Maximum memory usage = [-Xmx] + [-XX:MaxMetaspaceSize] + number_of_threads * [-Xss] + [-XX:MaxDirectMemorySize]
                          (heap)   (classes)                (threads' stack)             (direct memory)

..

   **Note**

   before Java8 memory dedicated to loaded classes was configured with ``-XX:PermSize`` and ``-XX:MaxPermSize`` instead of, respectively, ``-XX:MetaspaceSize`` and ``-XX:MaxMetaspaceSize``

In case of Tigase XMPP Server, apart from heap we limit remaining factors:

-  direct memory to **128** MB

-  loaded classes to **128** MB

-  single thread’s stack size to **228** KB (number of threads depends on number of CPU cores and may vary from 500 to couple of thousands)

In principle, in addition to HEAP’s maximum size defined by ``-Xmx`` you should add roughly **512** MB

If you are interested in detailed tracking of memory take a look at [Memory footprint of the JVM](\ https://spring.io/blog/2019/03/11/memory-footprint-of-the-jvm/), [Native Memory Tracking in JVM](\ https://www.baeldung.com/native-memory-tracking-in-jvm) or [Why does my Java process consume more memory than Xmx?](\ https://plumbr.io/blog/memory-leaks/why-does-my-java-process-consume-more-memory-than-xmx)


GC settings
~~~~~~~~~~~~

Let’s start with stating that there is no "one to rule them all" - each deployment and use-case is different, however we will try to give a couple of pointers and recommendations proceed with short introduction to GC itself.

XMPP is quite specific in terms of memory allocation - short-lived objects (various types of stanzas) usually exceed number of long-lived objects (user connections and related data). This is important bit of information in the context of how usually JVM HEAP is organized and how Garbage Collector works. On the most basic level Heap is separated into couple of regions:

Generations
''''''''''''

-  **Young Generation**, which is further divided in to:

   -  **Eden** - the region when the objects are usually allocated when they are created;

   -  **Survivor Spaces** - (*to* and *from* - one of which is always empty) - responsible for storing all live object remaining after collecting **Young Generation** (process is repeated several times until objects are finally considered *old enough*);

-  **Old Generation** - (*Tenured Space*) - responsible for live objects remaining after running GC on **Survivor Spaces** - those would be *long-lived* objects (usually user connections and associated data);

Minor, Major and Full GC - optimizing
''''''''''''''''''''''''''''''''''''''

General thinking suggests that:

-  **Minor GC** cleans Young generation;

-  **Major GC** cleans Tenured space;

-  **Full GC** cleans all heap.

However, while we can certainly state that Minor GC cleans Young generation it’s a bit more difficult to differentiate Major and Full GC, especially considering that Major GC can be quite often triggered by Minor GC and some garbage collectors can perform cleaning concurrently. Instead of focusing of distinguishing phases one should pay closer attention to actual operations of Garbage Collector itself - uncommenting the line ``GC_DEBUG=" -XX:+PrintTenuringDistribution -XX:+PrintGCDetails -XX:+PrintGCDateStamps -XX:+PrintGCTimeStamps -Xloggc:logs/jvm.log -verbose:gc "`` in ``etc/tigase.conf`` (or adding same properties to the java commandline) and subsequently analyzing the results should prove more helpful. In addition monitoring GC operation using for example VisualVM (with VisualGC plugin) will also be helpful.

Settings for XMPP
''''''''''''''''''

Ideally we should limit both number of GC pauses as well as their duration. After running rather tests following conclusions were made:

-  Garbage Collection is the faster the more dead objects occupies given space, therefore on high-traffic installation it’s better to have rather large YoungGen resulting in lower promotion of the objects to the OldGen;

-  with JVM8 default sizing of Young / Old generation changed, even tho NewRatio is still defaulting to “2” - setting it explicitly to "2" brought back previous sizing;

-  Concurrent Mark and Sweep (CMS) enabled (applies to Tenured space only) with explicit configuration of NewRatio set to default value of 2 (i.e. ``-XX:+UseConcMarkSweepGC -XX:+UseParNewGC -XX:NewRatio=2``) in general behaves best;

-  For small installations (few core CPU, less memory) with low traffic default Parallel collector may be a better solution;

-  Using Heap size adjusted to the actual usage is better as the larger the heap the larger are spaces over which collection needs to be performed thus resulting in longer pauses; in case of huge heaps G1 collector may be better solution to avoid longer pauses;

Considering all of the above using following options should be a good starting point toward further optimizing of Garbage Collection:

``GC="-XX:+UseBiasedLocking -XX:+UseConcMarkSweepGC -XX:+UseParNewGC -XX:+CMSIncrementalMode -XX:-ReduceInitialCardMarks -XX:CMSInitiatingOccupancyFraction=70 -XX:+UseCMSInitiatingOccupancyOnly"``


GC settings worth considering
'''''''''''''''''''''''''''''''

In addition to the general recommendation to use CMS collector, following options (or changes to the options) may be worth considering:

-  ``-XX:NewRatio=2`` - defines the ratio between the young and tenured generation is 1:2. In other words, the combined size of the eden and survivor spaces will be one-third of the total heap size. The parameters NewSize and MaxNewSize bound the young generation size from below and above. Setting these to the same value fixes the young generation, just as setting -Xms and -Xmx to the same value fixes the total heap size.

-  ``-XX:CMSInitiatingOccupancyFraction=percent`` - sets the percentage of the old generation occupancy (0 to 100) at which to start a CMS collection cycle.

-  ``-XX:+UseCMSInitiatingOccupancyOnly`` - instructs the JVM not to base its decision when to start a CMS cycle on run time statistics but instead it uses the value of CMSInitiatingOccupancyFraction for every CMS cycle.

-  ``-XX:ParallelGCThreads=x`` - sets the number of threads used for parallel garbage collection in the young and old generations. The default value depends on the number of CPUs available to the JVM. If the Tigase JMV is the only one running on the installation default value is recommended.

-  ``-XX:ConcGCThreads=x`` - sets the number of threads used for concurrent GC. The default value depends on the number of CPUs available to the JVM. If the Tigase JMV is the only one running on the installation default value is recommended.

-  ``-XX:+UseBiasedLocking`` and ``-XX:+DoEscapeAnalysis`` - designed to eliminate locking overhead, however their effect on performance is unpredictable therefore testing is required; reduced locking should improve concurrency and, on current multi-core hardware, improve throughput.

-  ``-XX:+OptimizeStringConcat`` - enables the optimization of String concatenation operations. This option is enabled by default.

-  ``-XX:+UseNUMA`` - enables performance optimization of an application on a machine with nonuniform memory architecture (NUMA - most modern computers are based on NUMA architecture) by increasing the application’s use of lower latency memory. By default, this option is disabled and no optimization for NUMA is made. The option is only available when the parallel garbage collector is used (-XX:+UseParallelGC).

-  ``-XX:-UseCompressedOops`` — disables the use of compressed pointers. By default, this option is enabled, and compressed pointers are used when Java heap sizes are less than 32 GB. When this option is enabled, object references are represented as 32-bit offsets instead of 64-bit pointers, which typically increases performance when running the application with Java heap sizes less than 32 GB. This option works only for 64-bit JVMs.


What to use with Machine x, y, z?
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


Server class machine (non-VM), > 16GB, >= 8 core CPU
'''''''''''''''''''''''''''''''''''''''''''''''''''''

For such setup enabling CMS garbage collector is recommended. Depending on the traffic usage and particular use-case adjusting NewRatio may be needed. Adjusting Xms and Xms sizes for actual available memory is needed (or better yet, for the actual traffic!). Following should be used:

.. code:: bash

   GC="-XX:+UseBiasedLocking -XX:+UseConcMarkSweepGC -XX:+UseParNewGC -XX:NewRatio=2 -XX:+CMSIncrementalMode -XX:-ReduceInitialCardMarks -XX:CMSInitiatingOccupancyFraction=70 -XX:+UseCMSInitiatingOccupancyOnly"
   EX="-XX:+OptimizeStringConcat -XX:+DoEscapeAnalysis -XX:+UseNUMA"

   #GC_DEBUG=" -XX:+PrintTenuringDistribution -XX:+PrintGCDetails -XX:+PrintGCDateStamps -XX:+PrintGCTimeStamps -Xloggc:logs/jvm.log -verbose:gc "

   PRODUCTION_HEAP_SETTINGS=" -Xms15G -Xmx15G " # heap memory settings must be adjusted on per deployment-base!
   JAVA_OPTIONS="${GC} ${GC_DEBUG} ${EX} ${ENC} ${DRV} ${JMX_REMOTE_IP} -server ${PRODUCTION_HEAP_SETTINGS} ${DNS_RESOLVER} ${INTERNAL_IP} ${EXTERNAL_IP}  -XX:MaxDirectMemorySize=128m "

For installation with lot of available memory and intention to utilize it all, using G1GC collector may be a better idea :

.. code:: bash

   GC="-XX:+UseG1GC -XX:ConcGCThreads=4 -XX:G1HeapRegionSize=2 -XX:InitiatingHeapOccupancyPercent=35 -XX:MaxGCPauseMillis=100"
   EX="-XX:+OptimizeStringConcat -XX:+DoEscapeAnalysis -XX:+UseNUMA"

   #GC_DEBUG=" -XX:+PrintTenuringDistribution -XX:+PrintGCDetails -XX:+PrintGCDateStamps -XX:+PrintGCTimeStamps -Xloggc:logs/jvm.log -verbose:gc "

   PRODUCTION_HEAP_SETTINGS=" -Xms60G -Xmx60G " # heap memory settings must be adjusted on per deployment-base!
   JAVA_OPTIONS="${GC} ${GC_DEBUG} ${EX} ${ENC} ${DRV} ${JMX_REMOTE_IP} -server ${PRODUCTION_HEAP_SETTINGS} ${DNS_RESOLVER} ${INTERNAL_IP} ${EXTERNAL_IP}  -XX:MaxDirectMemorySize=128m "


VM machine, 8GB of RAM, 4 core CPU equivalent
''''''''''''''''''''''''''''''''''''''''''''''

For such setup enabling CMS garbage collector is also recommended. Depending on the traffic usage and particular use-case adjusting NewRatio may be needed (and configuring NewRatio is a must!). Adjusting Xms and Xms sizes for actual available memory is needed (or better yet, for the actual traffic!). Following should be used:

.. code:: bash

   GC="-XX:+UseBiasedLocking -XX:+UseConcMarkSweepGC -XX:+UseParNewGC -XX:NewRatio=2 -XX:+CMSIncrementalMode -XX:-ReduceInitialCardMarks -XX:CMSInitiatingOccupancyFraction=70 -XX:+UseCMSInitiatingOccupancyOnly"
   EX="-XX:+OptimizeStringConcat -XX:+DoEscapeAnalysis -XX:+UseNUMA"

   #GC_DEBUG=" -XX:+PrintTenuringDistribution -XX:+PrintGCDetails -XX:+PrintGCDateStamps -XX:+PrintGCTimeStamps -Xloggc:logs/jvm.log -verbose:gc "

   PRODUCTION_HEAP_SETTINGS=" -Xms7G -Xmx7G " # heap memory settings must be adjusted on per deployment-base!
   JAVA_OPTIONS="${GC} ${GC_DEBUG} ${EX} ${ENC} ${DRV} ${JMX_REMOTE_IP} -server ${PRODUCTION_HEAP_SETTINGS} ${DNS_RESOLVER} ${INTERNAL_IP} ${EXTERNAL_IP}  -XX:MaxDirectMemorySize=128m "


VM machine with 4GB or less of RAM, and less than 4 core CPU equivalent
''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''

Small installations with limited resources could operate better with default (for JVM versions up to 8, which is the most current at the moment of the writing). Again - depending on the traffic usage and particular use-case adjusting NewRatio may be needed. Adjusting Xms and Xms sizes for actual available memory is recommended (or better yet, for the actual traffic!). Following should be used (i.e. ``GC`` line should be commented so the defaults will be used):

.. code:: bash

   #GC="-XX:+UseBiasedLocking -XX:+UseConcMarkSweepGC -XX:+UseParNewGC -XX:NewRatio=2 -XX:+CMSIncrementalMode -XX:-ReduceInitialCardMarks -XX:CMSInitiatingOccupancyFraction=70 -XX:+UseCMSInitiatingOccupancyOnly"
   EX="-XX:+OptimizeStringConcat -XX:+DoEscapeAnalysis -XX:+UseNUMA"

   #GC_DEBUG=" -XX:+PrintTenuringDistribution -XX:+PrintGCDetails -XX:+PrintGCDateStamps -XX:+PrintGCTimeStamps -Xloggc:logs/jvm.log -verbose:gc "

   PRODUCTION_HEAP_SETTINGS=" -Xms3G -Xmx3G " # heap memory settings must be adjusted on per deployment-base!
   JAVA_OPTIONS="${GC} ${GC_DEBUG} ${EX} ${ENC} ${DRV} ${JMX_REMOTE_IP} -server ${PRODUCTION_HEAP_SETTINGS} ${DNS_RESOLVER} ${INTERNAL_IP} ${EXTERNAL_IP}  -XX:MaxDirectMemorySize=128m "


Additional resources
~~~~~~~~~~~~~~~~~~~~~

-  `Sizing the Generations <https://docs.oracle.com/javase/8/docs/technotes/guides/vm/gctuning/sizing.html>`__

-  `About Java, parallel garbage collection and processor sets <http://www.c0t0d0s0.org/archives/6617-About-Java,-parallel-garbage-collection-and-processor-sets.html>`__

-  `GC Threads <http://hiroshiyamauchi.blogspot.cl/2009/12/gc-threads.html>`__

-  `GCViewer readme <https://github.com/chewiebug/GCViewer#readme>`__

-  `Java HotSpot™ Virtual Machine Performance Enhancements <http://docs.oracle.com/javase/7/docs/technotes/guides/vm/performance-enhancements-7.html>`__

-  `Java Garbage Collection handbook <https://plumbr.eu/java-garbage-collection-handbook>`__

-  Useful JVM Flags

   -  `Part 1 - JVM Types and Compiler Modes <https://blog.codecentric.de/en/2012/07/useful-jvm-flags-part-1-jvm-types-and-compiler-modes/>`__

   -  `Part 2 - Flag Categories and JIT Compiler Diagnostics) <https://blog.codecentric.de/en/2012/07/useful-jvm-flags-part-2-flag-categories-and-jit-compiler-diagnostics/>`__

   -  `Part 3 - Printing all XX Flags and their Values <https://blog.codecentric.de/en/2012/07/useful-jvm-flags-part-3-printing-all-xx-flags-and-their-values/>`__

   -  `Part 4 - Heap Tuning <https://blog.codecentric.de/en/2012/07/useful-jvm-flags-part-4-heap-tuning/>`__

   -  `Part 5 - Young Generation Garbage Collection <https://blog.codecentric.de/en/2012/08/useful-jvm-flags-part-5-young-generation-garbage-collection/>`__

   -  `Part 6 - Throughput Collector <https://blog.codecentric.de/en/2013/01/useful-jvm-flags-part-6-throughput-collector/>`__

   -  `Part 7 - CMS Collector <https://blog.codecentric.de/en/2013/10/useful-jvm-flags-part-7-cms-collector/>`__

   -  `Part 8 - GC Logging <https://blog.codecentric.de/en/2014/01/useful-jvm-flags-part-8-gc-logging/>`__

2.6.5. Session Manager
^^^^^^^^^^^^^^^^^^^^^^^

Tigase Session Manager is where most of Tigase basic options can be configured, and where many operations are controlled from. Changes to session manager can effect operations throughout an entire XMPP installation, so care must be made when changing settings here.

.. _sessManMobileOpts:

Mobile Optimizations
~~~~~~~~~~~~~~~~~~~~~

By default, Tigase employs XEP-0352 Client State Indication which allows for a more streamlined mobile experiencing by allowing the XMPP server to suppress or reduce the number of updates sent to a client thereby reducing the number of stanzas sent to a mobile client that is inactive. This employment is contained within the processor ``ClientStateIndication`` and is independent from the MobileV1, MobileV2, MobileV3 settings.

However, this can be fine tuned by using mobile plugins from Tigase which can be used at the same time by adding the following line to the ``config.tdsl`` file:

.. code:: properties

   }
   'sess-man' {
       'urn:xmpp:csi:0' {
           logic = 'tigase.xmpp.impl.MobileV1'
       }
   }

Logic Options are:


MobileV1
'''''''''

Keeps all presence stanzas in queue until client is active.

::

   logic = 'tigase.xmpp.impl.MobileV1'


MobileV2
''''''''

This setting delays delivery of presences while client is in inactive state, but only keeps the last presence for each full jid. **This is the default setting for CSI logic**.

::

   logic = 'tigase.xmpp.impl.MobileV2'


MobileV3
'''''''''

Keeps the same presence logic as MobileV2, but also queues Message Carbons. **Currently not supported by CSI processor, will cause issues**.

::

   logic = 'tigase.xmpp.impl.MobileV3'



Disabling CSI
''''''''''''''

If you wish to not use the ``ClientStateIndication`` processor, set the following in your ``config.tdsl`` file:

.. code:: dsl

   'sess-man' () {
       'urn:xmpp:csi:0' (active: false) {}
   }


A note about Mobile Plugins
''''''''''''''''''''''''''''

Previously, you could enable Mobile optimization logic using by enabling ``Mobile_V1 (){}`` bean to Session Manager: ``sess-man () {}`` bean.

If you have used these in the past, it is recommended you change your system to use the CSI processor with the appropriate mobile processing logic.

If you require v3 logic, or do not wish to use CSI, be sure to disable it using the above option.


threads-pool
~~~~~~~~~~~~~

The ``threadsNo`` property allows you to fine-tune the SM plugin’s (processors) thread pool. With the default settings every plugin gets his own thread pool. This guarantees the best performance and optimal resource usage. The downside of this setting is that packets can arrive out of order if they are processed within different thread pools.

We can even fine tune this packet processing. Let’s say you want most of the plugins to be executed within a single thread pool to preserve packet ordering for them, but for some selected plugins that should execute within separate thread pools to improve performance. Let’s say, authentication packets and user registration can be actually executed in a separate thread pools as we do not worry about an order for them. Users cannot send or receive anything else before they authenticates anyway. The solution is to specify a number of threads for the selected plugin. For example, setting a common thread pool for all plugins but registration and authentication can be done with following configuration:

.. code:: dsl

   'sess-man' () {
       'amp' () {
           threadsNo = 30
       }
       'presence-state' () {
           threadsNo = 27
       }
   }

This replaces the old ``--sm-threads-pool`` property, as well as specifying thread pools in ``--sm-plugins``.


Thread Pool factor
~~~~~~~~~~~~~~~~~~~

Session manager can control the number of available thread pools for each processor. By adding the following line to the ``config.tdsl`` file, the global thread pool can be increased by a specified factor:

.. code:: dsl

   'sess-man' () {
       'sm-threads-factor' = 3
   }

In this case, the global thread pools is increased by a factor or 3.


Strategy
~~~~~~~~

The ``Strategy`` property allows users to specify Clustering Strategy class which should be used for handling clustering environment; by default ``SMNonCachingAllNodes`` is used.

Any class implementing ``tigase.cluster.strategy.ClusteringStrategyIfc`` interface may be used for this setting.

Example:

.. code:: dsl

   'sess-man' () {
       strategy (class: tigase.cluster.strategy.SMCachingAllNodes)
   }

This replaces the old ``--sm-cluster-strategy-class`` setting from v7.1.

2.6.6. Virtual Hosts in Tigase Server
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Tigase server supports multiple virtual hosts in a single server installation. Virtual hosts can be added or removed, enabled or disabled during runtime without restarting the service or disrupting normal operation.

This document describes how virtual hosts work in Tigase server and how to get the most out of this feature in your installation.

The `'default-virtual-host' <#virtHosts>`__ property allows to define name of the single vhost domain which will be considered a default vhost domain for this installation. It allows you just to configure the domain name. Any additional configuration needs to be configured using ad-hoc commands.

Virtual hosts should be managed using ad-hoc commands or admin ui, visit `Add and Manage Domains <#addManageDomain>`__ for description of vhosts management process or visit `Specification for ad-hoc Commands Used to Manage Virtual Domains <#ad-hocCommands>`__ for more information about ad-hoc commands.

If you have components that may not be able to handle multiple vhosts or cluster mode, we have developed a virtual component solution as well, details in the `Virtual Components for the Tigase Cluster <#virtualComponents>`__ section.

You may also want to reference the Vhosts API for additional information: - `API Description for Virtual Domains Management in Tigase Server <#addManageDomain>`__.

   **Tip**

   If you have a Tigase XMPP Server running in the cluster mode hidden behind some load balancer, or if internal IP or hostname of cluster nodes differ from the DNS name under which it is available from the internet, we would suggest setting a property ``installation-dns-address`` of ``vhost-man`` component to the DNS name which allows you to connect to all cluster nodes (ie. to the DNS name of the load balancer). This will allow Tigase XMPP Server to do proper DNS lookups to verify that DNS domain name of the virtual host which you will try to add or update points to your XMPP installation.


Default VHost configuration
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

It’s possible to specify initial default configuration for all Virtual Host in TDSL configuration file (i.e. ``etc/config.tdsl``) for selected parameters. To do so you should specify each configuration option within ``defaults`` bean belonging to ``vhost-man`` bean:

::

   'vhost-man' () {
       'defaults' () {
           'domain-filter-policy' = null
           's2s-secret' = null
           trusted = null
           'vhost-disable-dns-check' = false
           'vhost-max-users' = 0L
           'vhost-message-forward-jid' = null
           'vhost-presence-forward-jid' = null
           'vhost-register-enabled' = true
           'vhost-tls-required' = false
       }
   }

After initial definition of default configuration or after first startup of Tigase XMPP Server it is possible to configure Virtual Host defaults using ad-hoc commands by modifying values for ``default`` using ad-hoc as described in `Specification for ad-hoc Commands Used to Manage Virtual Domains <#ad-hocCommands>`__.

Alternatively, you may edit default Virtual Host configuration (configuration for domain ``default``) using Admin UI which by default is available at ``http://localhost:8080/admin/``.

Specification for ad-hoc Commands Used to Manage Virtual Domains
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

There are 3 ad-hoc commands for virtual domains management in the Tigase server:

1. ``VHOSTS_RELOAD`` used to reload virtual domains list from the repository (database).

2. ``VHOSTS_UPDATE`` used to add a new virtual domain or update information for existing one.

3. ``VHOSTS_REMOVE`` used to remove an existing virtual host from the running server.

Syntax of the commands follows the specification described in `XEP-0050 <http://xmpp.org/extensions/xep-0050.html>`__. Extra information required to complete the command is carried as data forms described in `XEP-0004 <http://xmpp.org/extensions/xep-0004.html>`__.

All commands are accepted by the server only when send by the installation administrator. If the command is sent from any other account ``<not-authorized />`` error is returned. To grant administrator rights to an account you have to set ``admins`` property in the ``config.tdsl`` configuration file.

Commands are sent to the 'vhost-man' server component and the 'to' attribute of the stanza must contain a full JID of the VHostManager on the server. The full **JID** consists of the component name: 'vhost-man' and the local domain, that is domain which is already on the list of virtual domains and is active. Assuming 'existing.domain.com' one of domains already activated for the server installation the **JID** is: 'vhost-man@existing.domain.com'.


Reloading the Domains List from the Database
'''''''''''''''''''''''''''''''''''''''''''''

In order to reload virtual domains from the permanent repository other than configuration file, you have to send ``VHOSTS_RELOAD`` ad-hoc command to the VHostManager on the server.

The reload command request is of the form:

.. code:: xml

   <iq type="set"
       to="vhost-man@existing.domain.com"
       id="aac8a">
     <command xmlns="http://jabber.org/protocol/commands"
              node="VHOSTS_RELOAD" />
   </iq>

The server sends a response upon successful completion of the command with current number of virtual domains server by the installation:

.. code:: xml

   <iq from="vhost-man@existing.domain.com"
       type="result"
       to="cmd-sender-admin@existing.domain.com"
       id="aac8a">
     <command xmlns="http://jabber.org/protocol/commands"
              status="completed"
              node="VHOSTS_RELOAD">
       <x xmlns="jabber:x:data" type="result">
         <field type="fixed" var="Note">
           <value>Current number of VHosts: 123</value>
         </field>
       </x>
     </command>
   </iq>

If the command is sent from an account other than admin, the server returns an error:

.. code:: xml

   <iq from="vhost-man@existing.domain.com"
       type="error"
       to="cmd-sender-admin@existing.domain.com"
       id="aac8a">
     <command xmlns="http://jabber.org/protocol/commands"
              node="VHOSTS_RELOAD" />
     <error type="auth" code="401">
       <not-authorized xmlns="urn:ietf:params:xml:ns:xmpp-stanzas" />
       <text xmlns="urn:ietf:params:xml:ns:xmpp-stanzas"
             xml:lang="en">
         You are not authorized for this action.
       </text>
     </error>
   </iq>

The response doesn’t have any special meaning other then end-user information. The client may ignore the response as it is sent after the command has been executed.

Adding a New Domain or Updating Existing One
'''''''''''''''''''''''''''''''''''''''''''''

In order to add a new domain or update existing one you have to send an ad-hoc command ``VHOSTS_UPDATE`` with at least one domain name in the command data form. You can also specify whether the domain is enabled or disabled but this is optional. Future releases may allow for setting additional parameters for the domain: maximum number of user accounts for this domain, anonymous login enabled/disabled for the domain, registration via XMPP enabled/disabled for this domain and some more parameters not specified yet.

The domain add/update command request is of the form:

.. code:: xml

   <iq type="set"
       to="vhost-man@existing.domain.com"
       id="aacba">
     <command xmlns="http://jabber.org/protocol/commands"
              node="VHOSTS_UPDATE">
       <x xmlns="jabber:x:data" type="submit">
         <field type="text-single"
                var="VHost">
           <value>new-virt.domain.com</value>
         </field>
         <field type="list-single"
                var="Enabled">
           <value>true</value>
         </field>
       </x>
     </command>
   </iq>

Please note: Character case in the command field variable names does matter.

Upon successful completion of the command the server sends a response back to the client with information of the existing number of virtual hosts on the server:

.. code:: xml

   <iq from="vhost-man@existing.domain.com"
       type="result"
       to="cmd-sender-admin@existing.domain.com"
       id="aacba">
     <command xmlns="http://jabber.org/protocol/commands"
              status="completed"
              node="VHOSTS_UPDATE">
       <x xmlns="jabber:x:data" type="result">
         <field type="fixed" var="Note">
           <value>Current number of VHosts: 124</value>
         </field>
       </x>
     </command>
   </iq>



Removing a Virtual Domain From the Server
''''''''''''''''''''''''''''''''''''''''''

In order to remove a virtual domain you have to send ``VHOSTS_REMOVE`` command to the server with the domain name.

The domain remove command is sent by the client:

.. code:: xml

   <iq type="set"
       to="vhost-man@existing.domain.com"
       id="aacba">
     <command xmlns="http://jabber.org/protocol/commands"
              node="VHOSTS_REMOVE">
       <x xmlns="jabber:x:data" type="submit">
         <field type="text-single"
                var="VHost">
           <value>virt-nn.domain.com</value>
         </field>
       </x>
     </command>
   </iq>

Upon successful completion of the command the server sends a response back to the client with information of the existing number of virtual hosts on the server:

.. code:: bash

   <iq from="vhost-man@existing.domain.com"
       type="result"
       to="cmd-sender-admin@existing.domain.com"
       id="aacba">
     <command xmlns="http://jabber.org/protocol/commands"
              status="completed"
              node="VHOSTS_REMOVE">
       <x xmlns="jabber:x:data" type="result">
         <field type="fixed" var="Note">
           <value>Current number of VHosts: 124</value>
         </field>
       </x>
     </command>
   </iq>

Virtual Components for the Cluster Mode
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Let’s assume you have a cluster installation and you want to include a component in your installation which doesn’t support the cluster mode yet. If you put it on all nodes as a separate instances they will work out of sync and overall functionality might be useless. If you put on one node only it will work correctly but it will be visible to users connected to this one node only.

Ideally you would like to have a mechanism to install it on one node and put some redirections on other nodes to forward all packets for this component to a node where this component is working. Redirection on it’s own is not enough because the component must be visible in service discovery list and must be visible somehow to users connected to all nodes.

This is where the virtual components are handy. They are visible to users as a local normal component, they seem to be a real local component but in fact they just forward all requests/packets to a cluster node where the real component is working.

Virtual component is a very lightweight ServerComponent implementation in Tigase server. It can pretend to be any kind of component and can redirect all packets to a given address. They can mimic native Tigase components as well as third-party components connected over external component protocol (XEP-0114).

Configuration is very simple and straightforward, in fact it is very similar to configuration of any Tigase component. You set a real component name as a name of the component and a virtual component class name to load. Let’s say we want to deploy MUC component this way. The MUC component is visible as ``muc.domain.oug`` in the installation. Thus the name of the component is: ``muc``

.. code:: dsl

   muc (class: tigase.cluster.VirtualComponent) {}

This is pretty much all you need to load a virtual component. A few other options are needed to point to correct destination addresses for packets forwarding and to set correct service discovery parameters:

.. code:: dsl

   }
   muc (class: tigase.cluster.VirtualComponent) {
       'disco-category' = 'conference'
       'disco-features' = 'http://jabber.org/protocol/muc'
       'disco-name' = 'Multi User Chat'
       'disco-node' = ''
       'disco-type' = 'text'
       'redirect-to' = 'muc@cluster-node-with-real-muc.domain.our'
   }

That’s it.

2.6.7. Settings for Custom Logging in Tigase
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Logging can be an important tool to monitor your server’s health and performance. Logging may be controlled and customized on a per-component basis.

A ``logging`` bean has been implemented to allow more flexible configuration of logging in the Tigase XMPP Server.


Configuring logging
~~~~~~~~~~~~~~~~~~~~~


In the config file
'''''''''''''''''''

Default logging configuration for your installation is kept in the config file and it may be adjusted there.

.. code:: config

   logging () {
       rootLevel = CONFIG
       'packet-debug-full' = true
       loggers = {
           'tigase.server' = {
               level = ALL
           }
           'tigase.conf' = {
               level = FINEST
           }
       }
       handlers = {
           ' java.util.logging.FileHandler' = {
               level = ALL
               append = true
               count = 5
               formatter = 'tigase.util.LogFormatter'
               limit = 10000000
               pattern = 'logs/tigase.log'
           }
           'java.util.logging.ConsoleHandler' = {
               level = WARNING
               formatter = 'tigase.util.LogFormatter'
           }
       }
   }

You only need to specify the settings you wish to customize, otherwise they will be left as default.

-  ``packet-debug-full`` - controls whether log entries should be obfuscated (all CData of all elements will be replaced by ``CData size: <length in bytes of the replaced string>``) or not; default: ``false``.

-  ``rootLevel`` - Defines the root level of logging for all components not otherwise defined. Default is CONFIG

-  ``loggers`` - Defines the level of logging for packages running in tigase server. This is similar to the --debug setting, however you must use ``tigase.{package}`` format. Default is NONE.

-  ``handlers`` - Defines the level of logging for File output and Console output.

   1. ``FileHandler`` - is the file output for log files, with the following options:

      a. ``level`` - specifies the level of logs to be written, default is ALL.

      b. ``append`` - whether to append to the log or replace it during restart. Default is true.

      c. ``count`` - number of individual log files to keep at set limit. Default is 5. (default settings will continue appending logs until 5 files at 10MB are reached, then the oldest file will be overwritten.)

      d. ``formatter`` - specifies the package to format logging output. Default is tigase.util.LogFormatter.

      e. ``limit`` - Byte limit for each log file. Default is 10000000 or 10MB.

      f. ``pattern`` - Directory and filename of the log file with respect to the Tigase installation directory. Default is logs/tigase.log.

   2. ``ConsoleHandler`` - Determines the formatting for Tigase output to console.

      a. ``level`` - specifies the level of logs to be written, default is WARNING.

      b. ``formatter`` - specifies the package to format logging output. Default is tigase.util.LogFormatter.


Disabling colored output
~~~~~~~~~~~~~~~~~~~~~~~~~

If for some reason you don’t want colored output in the logs you can disable it by setting ``disable_logger_color`` to ``true``. For convenience, you can uncomment in ``etc/tigase.conf`` following line:

.. code:: bash

   #DISABLE_LOGGER_COLOR=" -Ddisable_logger_color=true "


Ad-hoc changes to the logging configuration
''''''''''''''''''''''''''''''''''''''''''''

It is also possible to use ad-hoc command named **Set package logging** with id ``logging-set`` available at ``message-router@domain`` (where domain is your server name) to reconfigure logging level of packets at runtime without requirement of restarting the Tigase XMPP Server.

   **Note**

   Those changes will be applied to this single cluster node.

..

   **Note**

   Those changes will not be saved in the Tigase XMPP Server configuration file and will be lost after restart of Tigase XMPP Server.


Using Admin UI

If your Tigase XMPP Server is running with HTTP server and with Admin UI enabled, then the easiest way to change logging configuration is by using Admin UI. After logging into web interface, open ``Configuration`` section and select ``Set package logging`` command. This will bring to you a form which you need to fill in with following fields:

-  ``Package name`` - should contain Java package or class name for which you wish to change logging level

-  ``Level`` - select a logging level you wish to apply to entered package name *(``OFF`` means that logging will be disabled)*

After pressing ``Submit`` your form will be passed to the server for validation and selected changes will be applied.


Using ad-hoc command

If you have access to the XMPP admin account of Tigase XMPP Server and XMPP client which supports ad-hoc command execution, you may connect with your XMPP client to the Tigase XMPP Server and look for adh-hoc commands available at ``message-router@domain`` (where domain is your server name). Within found ad-hoc commands you should find command named ``Set package logging`` or ``logging-set`` (that depends what your XMPP client is showing, id or name of the command) and you should execute it. Tigase XMPP Server will return a form which you need to fill in with following fields:

-  ``Package name`` - should contain Java package or class name for which you wish to change logging level

-  ``Level`` - select a logging level you wish to apply to entered package name *(``OFF`` means that logging will be disabled)*

After submitting the form, Tigase XMPP Server will validate your request and update logging configuration.


Using REST API

If you have Tigase XMPP Server with REST API enabled, you can use it for configuring logging of Tigase XMPP Server as well.

   **Note**

   As with all HTTP REST API requests you will require a valid API key and in this case a valid admin credentials to authenticate a HTTP request using Basic HTTP Authentication.

All you need to to is to send a HTTP POST request to ``/rest/adhoc/message-router@domain.com`` (where domain is your server name) with ``Contect-Type`` set to ``application/xml`` and a following XML as a payload to set logging level of ``tigase.server`` package to ``ALL``.

.. code:: xml

   <command>
     <node>logging-set</node>
     <fields>
       <item>
         <var>package-name</var>
         <value>tigase.server</value>
       </item>
       <item>
         <var>level</var>
         <value>ALL</value>
       </item>
     </fields>
   </command>

..

   **Tip**

   You can set logging levels also using JSON payload. For more details please refer to `Tigase HTTP API Guide <https://docs.tigase.net/index.html#collapse-tigase-http-api-master-snapshot-head:>`__, to section ``Executing example ad-hoc commands`` in ``REST API - usage examples``.



Alternate loggers in Tigase - Logback
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

It’s possible to use Logback for logging purposes, which offers certain interesting features (async logging, better control over log rotation, on the fly changing logging configuration)

Requirements: \* slf4j-api.jar (provided in ``-dist-max`` package) \* jul-to-slf4j.jar (provided in ``-dist-max`` package) \* desired logger libraries (for logback it’s ``logback-classic.jar`` and ``logback-core.jar`` (provided in -dist-max).

Configuration boils down to adding slf4j bridge handler to the list of build-in Java Logger handlers configuration, which in Tigase translates to adding following line to ``etc/config.tdsl``:

.. code:: bash

   logging () {
       rootHandlers = [ 'java.util.logging.ConsoleHandler', 'java.util.logging.FileHandler', 'org.slf4j.bridge.SLF4JBridgeHandler' ]
   }

After that ``etc/logback.xml`` configuration file will be used.

As stated in [jul-to-slf4j bridge documentation](\ http://www.slf4j.org/legacy.html#jul-to-slf4j) it’s essential to include ``LevelChangePropagator`` to eliminate translation overhead for disabled log statements:

.. code:: xml

   <configuration debug="true">
     <contextListener class="ch.qos.logback.classic.jul.LevelChangePropagator"/>
     ...
   </configuration>

NOTE, that it may be prudent to remove configuration of all old JUL logger by appending following to ``etc/logback.xml`` configuration:

.. code:: xml

   <configuration debug="true">
     <contextListener class="ch.qos.logback.classic.jul.LevelChangePropagator"/>
       <resetJUL>true</resetJUL>
   </configuration>

2.6.8. Tigase Advanced Options
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

This section is designed to include a number of advanced configuration options available within Tigase, but may not have a relevant section yet to house them.

Using CAPTCHA for in-band registration
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

To reduce false or spam registrations to Tigase XMPP Server, there is now the ability to add CAPTCHA forms as a part of the in-band registration. The CAPTCHA will generate a random math equation and ask the user registering a new account to answer it. This may be enabled as a sub-option of enabling registration in config.tdsl:

.. code:: dsl

   'sess-man' {
       'jabber:iq:register' {
           captchaRequired = 'true'
       }
   }

..

   **Note**

   Because some clients do not refresh a registration form after an unsuccessful attempt, this option allows 3 retries with the same CAPTCHA.

3 unsuccessful attempts will result in the captcha being invalidated and a client will receive an error message.


Enabling Empty Nicknames
~~~~~~~~~~~~~~~~~~~~~~~~~

Tigase can now support users with empty nicknames. This can be enabled by adding the following code in config.tdsl.

.. code:: dsl

   'sess-man' {
       'jabber:iq:roster' {
           empty_name_enabled = 'true'
       }
   }


Enable Silent Ignore on Packets Delivered to Unavailable Resources
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

You can now have Tigase ignore packets delivered to unavailable resources to avoid having a packet bounce around and create unnecessary traffic. You may set this globally, within standard message handling only, or within the AMP component using the following settings:

Globally:

.. code:: dsl

   'sess-man' {
       'silently-ignore-message' = 'true'
   }

Message Processing Only:

.. code:: dsl

   'sess-man' {
       message {
           'silently-ignore-message' = 'true'
       }
   }

AMP Component:

.. code:: dsl

   'sess-man' {
       amp () {
           'silently-ignore-message' = 'true'
   }



Mechanism to count errors within Tigase
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

A new processor within statistics has been added to count the number of errors that Tigase returns. This processor, named ``error-counter``, will count all errors returned by Tigase, however by default the number is always zero if it is not enabled. It can be found as an MBean object in JMX under ``ErrorStatistics`` and contains values for packets with ``ERROR`` and grouped by type. To enable counting of these errors, you must ensure the processor is included in your ``sess-man`` configuration:

.. code:: dsl

   'sess-man' {
       'error-counter' () {}
   }

Including stream errors
''''''''''''''''''''''''

Stream ``ERROR`` packets are not included in the above counter by default as they are processed separately. To enable this to be added to the counter, the following line must be in your ``config.tdsl`` file.

.. code:: dsl

   c2s {
       'stream-error-counter' () {
           active = true
       }
   }


Stream resumption default & max-timeout
''''''''''''''''''''''''''''''''''''''''

``SteamManagementIOProcessor`` now has a setting that can be used to change the maximum timeout time it will wait for reconnection if a client does not send a time to wait. Two settings are now available:

.. code:: dsl

   c2s {
       'urn:xmpp:sm:3' {
           'resumption-timeout' = 90
       }
   }

The above setting in ``config.tdsl`` file will change the default timeout period to 90 seconds.

.. code:: dsl

   c2s {
       'urn:xmpp:sm:3' {
           'max-resumption-timeout' = 900
       }
   }

This setting will set the maximum time allowed for stream resumption to 900 seconds. This can be handy if you expect a number of mobile phones to connect to your server and want to avoid duplicate messages being sent back and forth.


Automatic subscription approval
''''''''''''''''''''''''''''''''

You may setup a server to automatically approve presence subscriptions or roster authorizations for all users. Say you were hosting bots and wanted to automate the process. This can be done with the following settings:

.. code:: dsl

   'sess-man' () {
       'jabber:iq:roster' {
           'auto-authorize' = 'true'
       }
       'presence-subscription' () {
           'auto-authorize' = 'true'
       }
   }

Both of these settings are false by default, and you may use them together or separately.

   **Note**

   ``presence-subscription`` is current default plugin. If you are using old ``presence`` then you should configure the option with correct plugin name.

The following behavior is followed when they are both activated:

-  Upon sending a subscription request - Both contacts will each others' subscription and be added to each others' roster. Presence information will immediately be exchanged between both parties.

-  Upon sending presence with type either unsubscribe or unsubscribed follows the rules defined in RFC regarding processing of these stanzas (i.e. adjusting subscription type of user/contact), but without forwarding those stanzas to the receiving entity to avoid any notifications to the client. However, a roster push is generated to reflect changes to presence in user roster in a seamless manner.

-  Simply adding an item to the roster (i.e. with <iq/> stanza with correct semantics) will also cause an automatic subscription between the user and the contact in a matter explained above.

Abuse Contacts
'''''''''''''''

Tigase has support for `XEP-0128: Service Discovery Extensions <https://xmpp.org/extensions/xep-0128.html>`__ for providing additional information to the server and component discovery information. One of the important usages for this feature is `XEP-0157: Contact Addresses for XMPP Services <https://xmpp.org/extensions/xep-0157.html>`__ which describes usage of this feature for providing contact information to server administrators or abuse response team.

To set abuse contact details you should set ``disco-extensions`` in property in ``etc/config.tdsl`` file with subproperty ``abuse-addresses`` set to your abuse address URI (for email you need to prefix it with ``mailto:`` and for XMPP address you need to prefix it with ``xmpp``):

.. code:: dsl

   'disco-extensions' = {
       'abuse-addresses' = [ 'mailto:abuse@localhost', 'xmpp:abuse@localhost' ]
   }

Push Notifications
''''''''''''''''''''

Tigase XMPP Server comes with support for `XEP-0357: Push Notifications <https://xmpp.org/extensions/xep-0357.html>`__ allowing user to receive notifications for messages received while his XMPP client is not connected enabled by default.


Disabling notifications

You can disable this feature with following settings:

.. code:: dsl

   'sess-man' {
       'urn:xmpp:push:0' (active: false) {}
   }


Removing body and sender from notifications

If you wish Tigase XMPP Server not to forward body of the message or sender details in the push notification you can disable that with following settings:

.. code:: dsl

   'sess-man' {
       'urn:xmpp:push:0' () {
           'with-body' = false
           'with-sender' = false
       }
   }

Overriding body of notifications

If you wish Tigase XMPP Server to override forward body of the encrypted message in the push notification (for example to avoid indicating that there is an "error") you can do that with following settings:

.. code:: dsl

   'sess-man' {
       'urn:xmpp:push:0' () {
           'encryptedMessageBody' = "You have a new secure message. Open to see the message"
       }
   }


Enabling push notifications for messages received when all resources are AWAY/XA/DND

Push notifications may also be sent by Tigase XMPP Server when new message is received and all resources of recipient are in AWAY/XA/DND state. To enable this type of notifications you need to enable additional push delivery extension named ``away`` in default push processor:

.. code:: dsl

   'sess-man' () {
       'urn:xmpp:push:0' () {
           'away' () {}
       }
   }

As this behaviour may not be expected by users and users need a compatible XMPP client to properly handle this notifications (XMPP client needs to retrieve message history from server to get actual message), in addition to enabling this plugin on the server, XMPP clients need to explicitly activate this feature. They can do that by including ``away`` attribute with value of ``true`` in push ``enable`` element send to the server, as in following example:

**Enabling Push notifications for away/xa/dnd account.**

.. code:: xml

   <iq type='set' id='x43'>
     <enable xmlns='urn:xmpp:push:0' away='true' jid='push-5.client.example' node='yxs32uqsflafdk3iuqo'>
       <x xmlns='jabber:x:data' type='submit'>
           ....
       </x>
     </enable>
   </iq>

If later on, user decides to disable notification for account in away/xa/dnd state, it may disable push notifications or once again send stanza to enable push notification but without ``away`` attribute being set:

.. code:: xml

   <iq type='set' id='x43'>
     <enable xmlns='urn:xmpp:push:0' away='true' jid='push-5.client.example' node='yxs32uqsflafdk3iuqo'>
       <x xmlns='jabber:x:data' type='submit'>
           ....
       </x>
     </enable>
   </iq>

2.7. Security
---------------

The articles here cover advanced security features built into to Tigase Server, and some options for adding your own levels of security.

2.7.1. XEP-0191: Blocking Command
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

The simplest security feature, however, inside an XMPP server is the ability to block users and JIDS. `XEP-0191 <http://xmpp.org/extensions/xep-0191>`__ specifies the parameters of simple blocking without using privacy lists. Below is a breakdown and some sample commands you may find helpful. To enable this feature, be sure the following is in your ``config.tdsl`` file:

::

   }
   'sess-man' {
       'urn:xmpp:blocking' () {}
   }

If you have other plugins running, then just add ``'urn:xmpp:blocking' () {}`` to the list to activate this feature.

To confirm if your installation of Tigase supports this feature, a quick disco#info of your server should reveal the following feature:

::

   <feature var='urn:xmpp:blocking'/>

Blocked users are stored on the server on a per-JID basis, so one user may only see his or her blocked JIDs. Lists of blocked JIDs will return as an IQ stanza with a list of <item> fields. To retrieve the blocklist, the following command is issued:

.. code:: xml

   <iq type='get' id='blockedjids'>
     <blocklist xmlns='urn:xmpp:blocking'/>
   </iq>

The server responds:

.. code:: xml

   <iq type='result' id='blockedjids'>
     <blocklist xmlns='urn:xmpp:blocking'>
       <item jid='user1@domain.net'/>
       <item jid='admin@example.com'/>
     </blocklist>
   </iq>

To block a JID, a similar stanza to the one above is sent to the server with the items of the blocked JIDs you wish to add:

.. code:: xml

   <iq from='admin@domain.net' type='set' id='block'>
     <block xmlns='urn:xmpp:blocking'>
       <item jid='user2@domain.net'/>
     </block>
   </iq>

The server will then push an unavailable presence to blocked contacts. Communication between a contact that is blocked, and an entity that blocked it will result in a <not-acceptable> error:

.. code:: xml

   <message type='error' from='user2@domain.net' to='admin@domain.net'>
     <body>Hello, are you online?</body>
     <error type='cancel'>
       <not-acceptable xmlns='urn:ietf:params:xml:ns:xmpp-stanzas'/>
       <blocked xmlns='urn:xmpp:blocking:errors'/>
     </error>
   </message>

Unblocking a contact is just as easy as blocking, send an unblock stanza to the server:

.. code:: xml

   <iq from='admin@domain.net' type='set' id='unblock'>
     <unblock xmlns='urn:xmpp:blocking'>
       <item jid='user2@domain.net'/>
     </unblock>
   </iq>

The server will begin pushing presence information to unblocked contacts and resources so long as permissions have not changed between.

You may also opt to unblock all contacts and essentially clear out your blocked list using the following command:

.. code:: xml

   <iq type='set' id='unblockall'>
     <unblock xmlns='urn:xmpp:blocking'/>
   </iq>

2.7.2. Account Registration Limits
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

In order to protect Tigase servers from DOS attacks, a limit on number of account registrations per second has been implemented. This may be configured by adding the following line in the ``config.tdsl`` file:

.. code:: dsl

   'registration-throttling' () {
       limit = 10

This setting allows for 10 registrations from a single IP per second. If the limit is exceeded, a ``NOT_ALLOWED`` error will be returned.

It is possible to create two separate counters as well:

.. code:: dsl

   'registration-throttling' () {
       limit = 10
   }
   c2s {
       'registration-throttling' (class: tigase.server.xmppclient.RegistrationThrottling) {
           limit = 3
       }
   }

Here we have one for c2s with a limit of 3, and a global for all other connection managers set at 10.

You can also set individual components limits as well:

.. code:: dsl

   ws2s {
       'registration-throttling' (class: tigase.server.xmppclient.RegistrationThrottling) {
           limit = 7
       }
   }

2.7.3. Brute-force attack prevention
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Brute-force Prevention is designed to protect Tigase Server against user password guessing. It counts invalid login tries and when it is above limit, it locks login ability for specific time (soft ban). When invalid login counter reaches second level, account will be disabled permanently.

Configuration
~~~~~~~~~~~~~~

Brute-force Prevention is configured by VHost. There is following lis of configuration parameters:

+-------------------------------------+-------------+---------------------------------------------------------------------------+
| ``brute-force-lock-enabled``        | ``boolean`` | Brute Force Prevention Enabled                                            |
+-------------------------------------+-------------+---------------------------------------------------------------------------+
| ``brute-force-lock-after-fails``    | ``long``    | Number of allowed invalid login                                           |
+-------------------------------------+-------------+---------------------------------------------------------------------------+
| ``brute-force-period-time``         | ``long``    | Time [sec] in what failed login tries are counted                         |
+-------------------------------------+-------------+---------------------------------------------------------------------------+
| ``brute-force-disable-after-fails`` | ``long``    | Threshold beyond which account will be permanently disabled               |
+-------------------------------------+-------------+---------------------------------------------------------------------------+
| ``brute-force-lock-time``           | ``long``    | Time [sec] of soft ban (first threshold)                                  |
+-------------------------------------+-------------+---------------------------------------------------------------------------+
| ``brute-force-mode``                | ``string``  | Working mode (see `Working modes <#bruteForcePrevention_WorkingModes>`__) |
+-------------------------------------+-------------+---------------------------------------------------------------------------+

Detailed statistics
''''''''''''''''''''

By default, in order not to pollute statistics, Brute-Force locker will only provide details about number of locker IPs and JIDs (and total number of locked attempts). In order to have detailed information about IPs and JIDs that has been locked in statistics you should use following configuration:

::

   'sess-man' () {
       'brute-force-locker' () {
           detailedStatistics = false
       }
   }


Working modes
'''''''''''''

There are three working modes:

-  ``Ip`` - it counts invalid login tries from IP, and locks login ability (soft ban) for IP what reach the threshold

-  ``IpJid`` - it counts tries from IP to specific user account. Soft ban locks ability of login to specific JID from specific IP.

-  ``Jid``- similar to ``IpJid`` but checks only JID. Soft ban locks ability of login to specific JID from all IPs.

..

   **Note**

   Only in modes ``Jid`` and ``IpJid`` account may be permanently disabled.


Permanent ban
''''''''''''''

In modes ``Jid`` and ``IpJid``, when invalid login counter reach threshold ``brute-force-disable-after-fails``, account status will be set o ``disabled``. To enable it again you should use `Re-Enable User <https://xmpp.org/extensions/xep-0133.html#reenable-users>`__ Ad-hoc Command.

2.7.4. Server Certificates
^^^^^^^^^^^^^^^^^^^^^^^^^^^

-  `Creating and Loading the Server Certificate in pem Files <#certspem>`__

Creating and Loading the Server Certificate in pem Files
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Server Certificates
''''''''''''''''''''

Server certificates are needed when you use secure socket connections - SSL/TLS.

For secure socket connection a proper certificate is needed. You can either generate your own self-signed certificate or obtain certificate from trusted third party organization.

Here are steps how to obtain certificate from a trusted organization.

Generating your Own Certificates

Self-signed certificates can be generated easily on a Linux system. Although it may not be considered a 'trusted' certificate authority, it can be useful to test server installations. **We do not recommend regular use of self-signed certificates**.

.. Note:: 

   that Tigase v5.0 and later can automatically create self signed PEM files if needed. However we will cover doing this process by hand.

This tutorial assumes you are running a Linux-based operating system with access to command shell, and the 'Openssl' package is installed on the system.

| The process takes the following steps:
| 1. Create a local private key. This file ends with .key extension. It is recommended to create a new private key for the process.
| 2. Generate a certificate request. This file ends with the .csr extension and is the file sent to the Certificate Authority to be signed.
| 3. CA signs private key. This can be done by your own computer, but can also be done by private CAs for a fee.
| 4. Results are obtained from the CA. This is a ``.crt`` file which contains a separate public certificate.
| 5. Combine the ``.csr`` and ``.crt`` file into a unified ``.pem`` file. Tigase requires keys to be non-password protected PEM files.

**Generate local private key.**

.. code:: sh

   openssl genrsa -out [domain.com.key] 1024

This command generates a private key using a 1024 bit RSA algorithm. ``-out`` designates the name of the file, in this case it will be ``domain.com.key``. The exact name is not important, and the file will be created in whatever directory you are currently in.

**Generate a certificate request:.**

.. code:: sh

   openssl req -nodes -key domain.com.key -out domain.com.csr

This command generates a certificate request using the file specified after ``-key``, and the result file will be ``domain.com.csr``. You will be asked a series of questions to generate the request.

.. code:: sh

   Country Name (2 letter code) [AU]:AU
   State or Province Name (full name) [Some-State]:Somestate
   Locality Name (eg, city) []:Your city name
   Organization Name (eg, company) [Internet Widgits Pty Ltd]:Company name
   Organizational Unit Name (eg, section) []:Department or any unit
   Common Name (eg, YOUR name) []:*.yourdomain.com
   Email Address []:your_email_address@somedomain.com

   Please enter the following 'extra' attributes
   to be sent with your certificate request
   A challenge password []:
   An optional company name []:

**Sign the Certificate Request:.**

Now the .csr file will be signed by a Certificate Authority. In this tutorial, we will be self-signging our certificate. This practice however is generally not recommended, and you will receive notifications that your certificate is not trusted. There are commercial offers from companies to sign your certificate from trusted sources. Please see the `Certificate From Other Providers <#OtherSources>`__ section for more information.

.. code:: bash

   openssl x509 -req -days 365 -in domain.com.csr -signkey domain.com.key -out domain.com.crt

This command signs the certificate for 365 days and generates the ``domain.com.crt`` file. You can, of course use any number of days you like.

**Generate PEM file.**

You should now have the following files in the working directory: ..\\ domain.com.key domain.com.csr domain.com.crt

.. code:: sh

   cat yourdomain.com.cert.pem intermediate.cert.pem root.cert.pem > yourdomain.com.pem

If the certificate is issued by third-party authority you will have to attach the certificate chain, that being certificate of the authority who has generated your certificate. You normally need to obtain certificates for your chain from the authority who has generated your certificate.

The result file should looks similar to:

.. code:: sh

   -----BEGIN CERTIFICATE-----
   MIIG/TCCBeWgAwIBAgIDAOwZMA0GCSqGSIb3DQEBBQUAMIGMMQswCQYDVQQGEwJJ
   .
   .
   .
   pSLqw/PmSLSmUNIr8yQnhy4=
   -----END CERTIFICATE-----
   -----BEGIN RSA PRIVATE KEY-----
   WW91J3JlIGtpZGRpbmchISEKSSBkb24ndCBzaG93IHlvdSBvdXIgcHJpdmF0ZSBr
   .
   .
   .
   ZXkhISEhCkNyZWF0ZSB5b3VyIG93biA7KSA7KSA7KQo=
   -----END RSA PRIVATE KEY-----
   -----BEGIN CERTIFICATE-----
   MIIHyTCCBbGgAwIBAgIBATANBgkqhkiG9w0BAQUFADB9MQswCQYDVQQGEwJJTDEW
   .
   .
   .
   xV/stleh
   -----END CERTIFICATE-----

For Tigase server as well as many other servers (Apache 2.x), the order is following; your domain certificate, your private key, authority issuing your certificate, root certificate.

.. NOTE::

   Tigase requires full certificate chain in PEM file (described above)! Different applications may require pem file with certificates and private key in different order. So the same file may not be necessarily used by other services like Web server or e-mail server. Currently, Tigase can automatically sort certificates in PEM file while loading it.**


Installing/Loading Certificate To the Tigase Server
''''''''''''''''''''''''''''''''''''''''''''''''''''

Installing and loading certificates is very easy. The server can load all certificates directly from **pem** files. You just need to create a separate pem file for each of your virtual domains and put the file in a directory accessible by the server. Tigase server can automatically load all **pem** files found in given directory. By default, and to make things easy, we recommend the ``Tigase/certs`` directory.

It’s also possible to use: \* Admin ad-hoc command via XMPP client - you should navigate to Service Discovery of your server and in the list of commands for ``VHost Manager`` component select ``Add SSL Certificate`` and then follow instructions \* Admin WebUI - open ``http://<host>/admin``, navigate to ``Other`` category and in it select ``Add SSL Certificate`` and then follow instructions \* REST API - make a ``POST`` request to ``http://localhost:8080/rest/adhoc/vhost-man@domain.com`` with payload containing your certificate; to get the required form fields make ``GET`` request to the same endpoint



Certificate From Other Providers
'''''''''''''''''''''''''''''''''

There is number of certificate providers offering certificates either for free or for money. You can use any of them, however you have to be aware that sometimes certificates might not be recognized by all XMPP servers, especially if it’s one from a new provider. Here is an example list of providers:

-  LetsEncrypt - please see `??? <#LetsEncryptCertificate>`__ for details

-  `CAcert <https://www.cacert.org/>`__ - free certificates with Web GUI. (WARNING: it’s not widely accepted)

-  `Verisign <https://www.verisign.com/>`__ - very expensive certificates comparing to above provides but the provider is recognized by everybody. If you have a certificate from Verisign you can be sure it is identified as a valid certificate.

-  `Comodo Certificate Authority <http://www.comodo.com/business-security/digital-certificates/ssl-certificates.php>`__ offers different kind of commercial certificates

To obtain certificate from a third party authority you have to go to its website and request the certificate using certificate request generated above. I cannot provide any instructions for this as each of the providers listed have different requirements and interfaces.

We **highly** recommend using LetsEncrypt keys to self-sign and secure your domain. Instructions are in the `next section <#LetsEncryptCertificate>`__.


Using one certificate for multiple domains
''''''''''''''''''''''''''''''''''''''''''

.. Note::

   Tigase tries to be *smart* and automatically detects wildcard domain and alternative domains so it’s not needed to duplicate same certificate in multiple files to match domains - same file will be loaded and make available for all domains (CNames) available in the certificate.

Installing LetsEncrypt Certificates in Your Linux System
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

LetsEncrypt is a trusted CA that provides free security certificates. Unlike previously self-signed certificates, we can use LetsEncrypt Certificates to certify your domains from a trusted source.

Please refer to official `certbot User Guide <https://certbot.eff.org/docs/using.html>`__ for details how to install and operate the tool, choosing desired method of domain authentication (DNS or webserver). After successful execution the certificate with all related files will be stored under ``/etc/letsencrypt/live/$domain``

.. code:: bash

   $ sudo ls  /etc/letsencrypt/live/$domain
   cert.pem  chain.pem  fullchain.pem  privkey.pem  README

In that directory, you will find four files:

-  ``privkey.pem`` - private key for the certificate

-  ``cert.pem`` - contains the server certificate by itself

-  ``chain.pem`` - contains the additional intermediate certificate or certificates

-  ``fullchain.pem`` - all certificates, including server certificate (aka leaf certificate or end-entity certificate). The server certificate is the first one in this file, followed by any intermediates.

For Tigase XMPP Server, we are only concerned with ``privkey.pem`` and ``fullchain.pem`` (or ``chain.pem`` - please consider actual issuers and certification chain!).

At this point we will need to obtain the root and intermediate certificates, this can be done by downloading these certificates from the `LetsEncrypt Chain of Trust website <https://letsencrypt.org/certificates/>`__.

.. Note::

   Please pay utmost attention to the actual certificate issuers and make sure that the certification chain is maintained!

On the time of the writing, LetsEncrypt was providing domain certificates issued by ``R3`` CertificateAuthorigy (CA). In order to provide complete chain to the root CA you should get Let’s Encrypt R3 (``RSA 2048, O = Let’s Encrypt, CN = R3``) certificate. Depending on desired certification chain you have two options: 1) (default and recommended) using own LetsEncrypt CA: a) ``R3`` certificate signed by ISRG Root X1: https://letsencrypt.org/certs/lets-encrypt-r3.pem b) ``ISRG Root X1`` root certificate: https://letsencrypt.org/certs/isrgrootx1.pem 2) (legacy, option more compatible with old systems): cross-signed certificate by IdenTrust: a) ``R3`` certificate cross-signed by IdenTrust: https://letsencrypt.org/certs/lets-encrypt-r3-cross-signed.pem b) ``TrustID X3 Root`` from IdenTrust: https://letsencrypt.org/certs/trustid-x3-root.pem.txt

Considering first (recommended) option, you may obtain them using wget:

.. code:: bash

   wget https://letsencrypt.org/certs/isrgrootx1.pem
   wget https://letsencrypt.org/certs/lets-encrypt-r3.pem

These are the root certificate, and the intermediate certificate signed by root certificate.

.. Note::

   IdenTrust cross-signed certificate will not function properly in the future!

Take the contents of your ``privkey.pem``, certificate, and combine them with the contents of ``isrgrootx1.pem`` and ``lets-encrypt-r3.pem`` into a single pem certificate.

Depending on your configuration you either need to name the file after your domain such as ``mydomain.com.pem`` and place it under ``certs/`` subdirectory of Tigase XMPP Server installation or update it using admin ad-hoc (see `??? <#certificateStorage>`__)

If you moved all certs to a single directory, you may combine them using the following command under \*nix operating systems:.

.. code:: bash

   cat ./cert.pem ./privkey.pem ./lets-encrypt-r3.pem ./isrgrootx1.pem > mydomain.com.pem


.. Note::

   If you are using ``isrgrootx1`` root make sure you use ``cert.pem`` file instead of ``fullchain.pem``, which uses different intermediate certificate ( `Let’s Encrypt Authority X3 (IdenTrust cross-signed) <https://letsencrypt.org/certs/lets-encrypt-x3-cross-signed.pem.txt>`__ ) and you will have to use `DST Root CA X3 <https://letsencrypt.org/certs/trustid-x3-root.pem.txt>`__ certificate!

Your certificate should look something like this:

.. code:: certificate

   -----BEGIN PRIVATE KEY-----
   MIIEvgIBADANBgkqhkiG9w0BAQEFAASCBKgwggSkAgEAAoIBAQDAUAqqKu7Z4odo
   ...
   og89F9AbWr1mNmyRoScyqMXo
   -----END PRIVATE KEY-----
   -----BEGIN CERTIFICATE-----
   cmNoIEdyb3VwMRUwEwYDVQQDEwxJU1JHIFJvb3QgWDEwHhcNMTUwNjA0MTEwNDM4
   ...
   TzELMAkGA1UEBhMCVVMxKTAnBgNVBAoTIEludGVybmV0IFNlY3VyaXR5IFJlc2Vh
   -----END CERTIFICATE-----
   -----BEGIN CERTIFICATE-----
   FhpodHRwOi8vY3BzLmxldHNlbmNyeXB0Lm9yZzCBqwYIKwYBBQUHAgIwgZ4MgZtU
   ...
   bmcgUGFydGllcyBhbmQgb25seSBpbiBhY2NvcmRhbmNlIHdpdGggdGhlIENlcnRp
   -----END CERTIFICATE-----


.. Warning::

    LetsEncrypt certificates expire 90 days from issue and need to be renewed in order for them to remain valid!

You can check your certificate with utility class:

::

   java -cp <path_to_tigase-server_installation>/jars/tigase-utils.jar tigase.cert.CertificateUtil -lc mydomain.com.pem -simple


Let’s encrypt and DNS verification
'''''''''''''''''''''''''''''''''''

The only way to obtain wildcard (``*.domain.com``) certificate is via DNS verification. Certbot support a number of DNS operators - you can check if your DNS provider is listed by executing ``$ certbot plugins``

AWS Route53

If you want to use it with Amazon Cloud you should install plugin for AWS:

::

   pip install certbot-dns-route53


.. Note::

   If you are using certbot under macOS and you installed it via brew then you should use: ``$( brew --prefix certbot )/libexec/bin/pip install certbot-dns-route53``

You should store your credentials in ``~/.aws/credentials`` (you may want to create dedicated policy for updating DNS as described in `plugin’s documentation <https://certbot-dns-route53.readthedocs.io/en/stable/>`__:

.. code:: bash

   [default]
   aws_access_key_id = <key_id>
   aws_secret_access_key = <key>

And afterward you should execute ``certbot`` with ``--dns-route53`` parameter

Certbot update hook and Tigase API
'''''''''''''''''''''''''''''''''''

For greater automation it’s possible to automate updating certificate obtained with ``certbot`` in Tigase XMPP Server. You should use following deploy hook - either add it to ``/etc/letsencrypt/renewal-hooks/deploy/`` or use it directly in ``certboot`` commandline with ``--deploy-hook`` parameter (in the latter case, it will be added to particular domain configuration so it’s not necessary to specify UPDATE_DOMAINS).

.. Note::

   Please adjust account credentials used for deployment (``USER``, ``PASS``, ``DOMAIN``) as well as paths to Let’s Encrypt certificates (*ISRG Root X1* named ``isrgrootx1.pem`` and *Let’s Encrypt Authority X3* named ``letsencryptauthorityx3.pem``)

.. code:: bash

   #!/bin/bash

   set -e

   ## Configuration START

   USER="admin_username"
   PASS="admin_password"
   DOMAIN="my_domain.tld"
   HOST=${DOMAIN}
   #UPDATE_DOMAINS=(${DOMAIN})
   # PORT=":8080"
   # APIKEY="?api-key=mySecretKey"
   LE_CERTS_PATH="/path/to/letsencrypt/CA/certificates/"

   ## Configuration END

   fail_count=0

   for domain in ${RENEWED_DOMAINS[@]}; do
       if [[ $domain == "*."* ]]; then
           CERT_DOMAIN=${domain#*\*.}
       else
           CERT_DOMAIN=${domain}
       fi

       if [[ ! -z "${UPDATE_DOMAINS}" ]] ; then
           match=0
           for dn in "${UPDATE_DOMAINS[@]}"; do
               if [[ $dn = "$CERT_DOMAIN" ]]; then
                   match=1
                   break
               fi
           done
           if [[ $match = 0 ]]; then
               echo "Skipping updating ${domain} because it's not in the list of supported domains: ${UPDATE_DOMAINS[@]}"
               continue
           fi
       fi

       CERT=`cat "$RENEWED_LINEAGE/cert.pem" "$RENEWED_LINEAGE/privkey.pem" ${LE_CERTS_PATH}/isrgrootx1.pem ${LE_CERTS_PATH}/letsencryptauthorityx3.pem`

       REQUEST="
       <command>
         <node>ssl-certificate-add</node>
         <fields>
           <item>
             <var>Certificate in PEM format</var>
             <value>${CERT}</value>
           </item>
           <item>
             <var>command-marker</var>
             <value>command-marker</value>
           </item>
           <item>
             <var>VHost</var>
             <value>${CERT_DOMAIN}</value>
           </item>
           <item>
             <var>Save to disk</var>
             <value>true</value>
           </item>
         </fields>
       </command>"

       response=`curl -s -L -H "Content-Type: text/xml" -X POST  http://${USER}%40${DOMAIN}:${PASS}@${HOST}${PORT}/rest/adhoc/vhost-man@${DOMAIN}${APIKEY} -d "${REQUEST}"`

       if [[ ! ${response} = *"loaded successfully"* ]] ; then
           echo -e "Server returned error while updating   ${domain}   certificate:\n ${response}"
           fail_count=$((${fail_count}+1))
       else
           echo "Correctly updated ${domain} certificate"
       fi
   done

   exit ${fail_count}

.. Note::

   If you are not using wildcard certificate when you have to provide certificate for main domain as well as certificates for subdomains that mach all components that you want to expose (muc, pubsub, push, etc…)

Storing and managing certificates
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Filesystem
''''''''''

By default Tigase loads and stores certificates in ``certs/`` subdirectory. Each *domain* certificate should be stored in a file which filename consists of domain name and ``.pem`` extension, i.e. ``<domain>.pem``. For example for domain tigase.net it would be ``certs/tigase.net.pem``.

.. Note::

   Tigase tries to be *smart* and automatically detects wildcard domain and alternative domains so it’s not needed to duplicate same certificate in multiple files to match domains.


Database repository
'''''''''''''''''''

Alternatively it’s possible to use database as a storage for the certificates. Upon enabling it certificates won’t be read nor stored to the filesystem. You can enable it by adding ``repository () {}`` bean to ``'certificate-container' () {}`` in your TDSL configuration file:

::

   'certificate-container' () {
       repository () {}
   }

If you are using database repository then you manage/update certificates using either ad-hoc command ``Add SSL certificate`` from *VHost Manager* or via HTTP REST API.

2.7.5. Custom Authentication Connectors
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

This article presents configuration options available to the administrator and describe how to set Tigase server up to use user accounts data from a different database.

The first thing to know is that Tigase server always opens 2 separate connections to the database. One connection is used for user login data and the other is for all other user data like the user roster, vCard, private data storage, privacy lists and so on…​

In this article we still assume that Tigase server keeps user data in it’s own database and only login data is retrieved from the external database.

At the moment Tigase offers following authentication connectors:

-  ``mysql``, ``pgsql``, ``derby`` - standard authentication connector used to load user login data from the main user database used by the Tigase server. In fact the same physical implementation is used for all JDBC databases.

-  ``drupal`` - is the authentication connector used to integrate the Tigase server with `Drupal CMS <http://drupal.org/>`__.

-  ``tigase-custom`` - is the authentication connector which can be used with any database. Unlike the 'tigase-auth' connector it allows you to define SQL queries in the configuration file. The advantage of this implementation is that you don’t have to touch your database. You can use either simple plain SQL queries or stored procedures. The configuration is more difficult as you have to enter carefully all SQL queries in the config file and changing the query usually involves restarting the server. For more details about this implementation and all configuration parameters please refer to `Tigase Custom Auth documentation <#custonAuthConnector>`__.

-  ``tigase-auth`` (**DEPRECATED**) - is the authentication connector which can be used with any database. It executes stored procedures to perform all actions. Therefore it is a very convenient way to integrate the server with an external database if you don’t want to expose the database structure. You just have to provide a set of stored procedures in the database. While implementing all stored procedures expected by the server might be a bit of work it allows you to hide the database structure and change the SP implementation at any time. You can add more actions on user login/logout without restarting or touching the server. And the configuration on the server side is very simple. For detailed description of this implementation please refer to `Tigase Auth documentation <#tigaseAuthConnector>`__.

As always the simplest way to configure the server is through the ``config.tdsl`` file. In the article describing this file you can find long list with all available options and all details how to handle it. For the authentication connector setup however we only need 2 options:

.. code:: dsl

   dataSource {
       'default-auth' () {
           uri = 'database connection url'
       }
   }
   authRepository {
       default () {
           cls = 'connector'
           'data-source' = 'default-auth'
       }
   }

For example if you store authentication data in a ``drupal`` database on ``localhost`` your settings would be:

.. code:: dsl

   dataSource {
       'default-auth' () {
           uri = 'jdbc:mysql://localhost/drupal?user=user&password=passwd'
       }
   }
   authRepository {
       default () {
           'data-source' = 'default-auth'
       }
   }

You have to use a class name if you want to attach your own authentication connector.

Default is:

.. code:: dsl

   authRepository {
       default {
           cls = 'tigase.db.jdbc.TigaseAuth'
       }
   }

In the same exact way you can setup connector for any different database type.

For example, drupal configuration is below

.. code:: dsl

   authRepository {
       default {
           cls = 'tigase.db.jdbc.DrupalWPAuth'
       }
   }

Or tigase-custom authentication connector.

.. code:: dsl

   authRepository {
       default {
           cls = 'tigase.db.jdbc.TigaseCustomAuth'
       }
   }

The different ``cls`` or classes are:

-  Drupal - ``tigase.db.jdbc.DrupalWPAuth``

-  MySQL, Derby, PostgreSQL, MS SQL Server - ``tigase.db.jdbc.JDBCRepository``

You can normally skip configuring connectors for the default Tigase database format: ``mysql``, ``pgsql`` and ``derby``, ``sqlserver`` as they are applied automatically if the parameter is missing.

One more important thing to know is that you will have to modify ``authRepository`` if you use a custom authentication connector. This is because if you retrieve user login data from the external database this external database is usually managed by an external system. User accounts are added without notifying Tigase server. Then, when the user logs in and tries to retrieve the user roster, the server can not find such a user in the roster database.

.. Important::

   To keep user accounts in sync between the authentication database and the main user database you have to add following option to the end of the database connection URL: ``autoCreateUser=true``.

For example:

.. code:: dsl

   dataSource {
       default () {
           uri = 'jdbc:mysql://localhost/tigasedb?user=nobody&password=pass&autoCreateUser=true'
       }
   }

If you are interested in even further customizing your authentication connector by writing your own queries or stored procedures, please have a look at the following guides:

-  `Tigase Auth guide <#tigaseAuthConnector>`__

-  `Tigase Custom Auth guide <#custonAuthConnector>`__

Tigase Auth Connector (DEPRECATED)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. Warning::
    Tigase Auth connector is **DEPRECATED** as of version 8.0.0 and will be removed in future releases

The Tigase Custom Auth connector with shortcut name: **tigase-custom** is implemented in the class: `tigase.db.jdbc.TigaseCustomAuth <https://github.com/tigase/tigase-server/tree/master/src/main/java/tigase/db/jdbc/TigaseCustomAuth.java>`__. It allows you to connect to any external database to perform user authentication and use a custom queries for all actions.

You can find more details how to setup a custom connector in the Custom Authentication Connectors guide.

The basic configuration is very simple:

.. code:: bash

   authRepository {
       default () {
           cls = 'tigase.db.jdbc.TigaseCustomAuth'
           'data-source' = 'default-auth'
       }
   }

That’s it.

The connector loads correctly and starts working using predefined, default list of queries. In most cases you also might want to define your own queries in the configuration file. The shortest possible description is the following example of the content from the ``config.tdsl`` file:

This query is used to check connection to the database, whether it is still alive or not

.. code:: dsl

   authRepository {
       default () {
           'conn-valid-query' = 'select 1'
       }
   }

This is database initialization query, normally we do not use it, especially in clustered environment

.. code:: dsl

   authRepository {
       default () {
           'init-db-query' = 'update tig_users set online_status = 0'
       }
   }

.. Note::

   ``online_status`` column does not exist and would need to be added for that query to work.

Below query performs user authentication on the database level. The Tigase server does not need to know authentication algorithm or password encoding type, it simply passes user id (BareJID) and password in form which was received from the client, to the stored procedure. If the authentication was successful the procedure returns user bare JID or null otherwise. Tigase checks whether the JID returned from the query matches JID passed as a parameter. If they match, the authentication is successful.

.. code:: dsl

   authRepository {
       default () {
           'user-login-query' = '{ call TigUserLoginPlainPw(?, ?) }'
       }
   }


.. Note::

   ``TigUserLoginPlainPw`` is no longer part of a Tigase XMPP Server database schema and would need to be created.

Below query returns number of user accounts in the database, this is mainly used for the server metrics and monitoring components.

.. code:: dsl

   authRepository {
       default () {
         'users-count-query' = '{ call TigAllUsersCount() }'
       }
   }

The Below query is used to add a new user account to the database.

.. code:: dsl

   authRepository {
       default () {
           'add-user-query' = '{call TigAddUserPlainPw(?, ?) }'
       }
   }

Below query is used to remove existing account with all user’s data from the database.

.. code:: dsl

   authRepository {
       default () {
           'del-user-query' = '{ call TigRemoveUser(?) }'
       }
   }

This query is used for the user authentication if ``user-login-query`` is not defined, that is if there is no database level user authentication algorithm available. In such a case the Tigase server loads user’s password from the database and compares it with data received from the client.

.. code:: dsl

   authRepository {
       default () {
           'get-password-query' = 'select user_pw from tig_users where user_id = ?'
       }
   }

Below query is used for user password update in case user decides to change his password.

.. code:: dsl

   authRepository {
       default () {
           'update-password-query' = 'update tig_users set user_pw = ? where user_id = ?'
       }
   }

This query is called on user logout event. Usually we use a stored procedure which records user logout time and marks user as offline in the database.

.. code:: dsl

   authRepository {
       default () {
           'update-logout-query' = 'update tig_users, set online_status = online_status - 1 where user_id = ?'
       }
   }


.. Note::

   ``online_status`` column does not exist and would need to be added for that query to work.

This configuration specifies what non-sasl authentication mechanisms to expose to the client

.. code:: dsl

   authRepository {
       default () {
           'non-sasl-mechs' = [ 'password', 'digest' ]
       }
   }

This setting to specify what sasl authentication mechanisms expose to the client

.. code:: dsl

   authRepository {
       default () {
           'sasl-mechs' = 'PLAIN,DIGEST-MD5'
       }
   }

Queries are defined in the configuration file and they can be either plain SQL queries or stored procedures. If the query starts with characters: ``{ call`` then the server assumes this is a stored procedure call, otherwise it is executed as a plain SQL query. Each configuration value is stripped from white characters on both ends before processing.

Please don’t use semicolon ``;`` at the end of the query as many JDBC drivers get confused and the query may not work.

Some queries can take arguments. Arguments are marked by question marks ``?`` in the query. Refer to the configuration parameters description for more details about what parameters are expected in each query.

This example shows how to use a stored procedure to add a user as a query with 2 required parameters (username, and password).

.. code:: dsl

   authRepository {
       default () {
           'add-user-query' = '{call TigAddUserPlainPw(?, ?) }'
       }
   }

The same query with plain SQL parameters instead:

.. code:: dsl

   'add-user-query' = 'insert into users (user_id, password) values (?, ?)'

The order of the query arguments is important and must be exactly as described in specification for each parameter.

+---------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------------------------------+-------------------------------------------------------------------------------+
| Query Name                | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               | Arguments                                        | Example Query                                                                 |
+===========================+===========================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================+==================================================+===============================================================================+
| ``conn-valid-query``      | Query executed periodically to ensure active connection with the database.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                | Takes no arguments.                              | ``select 1``                                                                  |
+---------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------------------------------+-------------------------------------------------------------------------------+
| ``init-db-query``         | Database initialization query which is run after the server is started.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   | Takes no arguments.                              | ``update tig_users set online_status = 0``                                    |
+---------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------------------------------+-------------------------------------------------------------------------------+
| ``add-user-query``        | Query adding a new user to the database.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  | Takes 2 arguments: ``(user_id (JID), password)`` | ``insert into tig_users (user_id, user_pw) values (?, ?)``                    |
+---------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------------------------------+-------------------------------------------------------------------------------+
| ``del-user-query``        | Removes a user from the database.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         | Takes 1 argument: ``(user_id (JID))``            | ``delete from tig_users where user_id = ?``                                   |
+---------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------------------------------+-------------------------------------------------------------------------------+
| ``get-password-query``    | Retrieves user password from the database for given user_id (JID).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        | Takes 1 argument: ``(user_id (JID))``            | ``select user_pw from tig_users where user_id = ?``                           |
+---------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------------------------------+-------------------------------------------------------------------------------+
| ``update-password-query`` | Updates (changes) password for a given user_id (JID).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     | Takes 2 arguments: ``(password, user_id (JID))`` | ``update tig_users set user_pw = ? where user_id = ?``                        |
+---------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------------------------------+-------------------------------------------------------------------------------+
| ``user-login-query``      | Performs user login. Normally used when there is a special SP used for this purpose. This is an alternative way to a method requiring retrieving user password. Therefore at least one of those queries must be defined: ``user-login-query`` or ``get-password-query``. If both queries are defined then ``user-login-query`` is used. Normally this method should be only used with plain text password authentication or sasl-plain. Tigase expects a result set with user_id to be returned from the query if login is successful and empty results set if the login is unsuccessful. | Takes 2 arguments: ``(user_id (JID), password)`` | ``select user_id from tig_users where (user_id = ?) AND (user_pw = ?)``       |
+---------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------------------------------+-------------------------------------------------------------------------------+
| ``user-logout-query``     | This query is called when user logs out or disconnects. It can record that event in the database.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         | Takes 1 argument: ``(user_id (JID))``            | ``update tig_users, set online_status = online_status - 1 where user_id = ?`` |
+---------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------------------------------+-------------------------------------------------------------------------------+
| ``non-sasl-mechs``        | Comma separated list of NON-SASL authentication mechanisms. Possible mechanisms are: ``password`` and ``digest``. The digest mechanism can work only with ``get-password-query`` active and only when password are stored in plain text format in the database.                                                                                                                                                                                                                                                                                                                           |                                                  |                                                                               |
+---------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------------------------------+-------------------------------------------------------------------------------+
| ``sasl-mechs``            | Comma separated list of SASL authentication mechanisms. Possible mechanisms are all mechanisms supported by Java implementation. The most common are: ``PLAIN``, ``DIGEST-MD5``, ``CRAM-MD5``. "Non-PLAIN" mechanisms will work only with the ``get-password-query`` active and only when passwords are stored in plain text format in the database.                                                                                                                                                                                                                                      |                                                  |                                                                               |
+---------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------------------------------+-------------------------------------------------------------------------------+

Drupal Authentication
~~~~~~~~~~~~~~~~~~~~~~

Currently, we can only check authentication against a **Drupal** database at the moment. Full **Drupal** authentication is not implemented as of yet.

As **Drupal** keeps encrypted passwords in database the only possible authorization protocols are those based on PLAIN passwords.

To protect your passwords **Tigase** server must be used with SSL or TLS encryption.

Implementation of a **Drupal** database based authorization is located in ``tigase.db.jdbc.DrupalAuth`` class. Although this class is capable of adding new users to the repository I recommend to switch in-band registration off due to the caching problems in **Drupal.** Changes in database are not synchronized with **Drupal** yet. Functionality for adding new users is implemented only to ease user accounts migration from different repository types from earlier **Tigase** server installations.

The purpose of that implementation was to allow all accounts administration tasks from **Drupal** like: account creation, all accounts settings, like e-mail, full name, password changes and so on.

**Tigase** server uses following fields from **Drupal** database: name (user account name), pass (user account password), status (status of the account). Server picks up all changes instantly. If user status is not 1 then server won’t allow user to login trough XMPP even if user provides valid password.

There is no *Roster* management in **Drupal** yet. So Roster management have to be done from the XMPP client.

LDAP Authentication Connector
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Tigase XMPP Server offers support for authenticating users against an LDAP server in **Bind** **Authentication** mode.

Configuration for the LDAP support is really simple you just have to add a few lines to your ``config.tdsl`` file.

.. code:: tdsl

   authRepository {
       default () {
           cls = 'tigase.db.ldap.LdapAuthProvider'
           uri = 'ldap://ldap.tigase.com:389'
           'user-dn-pattern' = 'cn=USER_ID,ou=people,dc=tigase,dc=org'
       }
   }

Please note the ``USER_ID`` element, this is a special element of the configuration which is used to authenticate particular user. Tigase LDAP connector replaces it with appropriate data during authentication. You can control what Tigase should put into this part. In your configuration you must replace this string with one of the following:

1. ``%1$s`` - use user name only for authentication (JabberID’s localpart)

2. ``%2$s`` - use domain name only for authentication (JabberID’s domain part)

3. ``%3$s`` - use the whole Jabber ID (JID) for authentication

.. Important::

   Please make sure that you included ``autoCreateUser=true`` in your main data source (UserRepository and **not** above AuthRepository) as outlined in `??? <#autoCreateUser>`__ - otherwise you may run into problems with data access.

Configuration of SASL EXTERNAL
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

In order to enable SASL External set "Client Certificate CA" (``client-trust-extension-ca-cert-path``) to the path containing Certification Authority (CA) certificate in the VHost (domain) configuration, for example ``/path/to/cacert.pem``

File ``cacert.pem`` contains Certificate Authority certificate which is used to sign clients certificate.

Client certificate must include user’s Jabber ID as ``XmppAddr`` in ``subjectAltName``:

   As specified in RFC 3920 and updated in RFC 6120, during the stream negotiation process an XMPP client can present a certificate (a “client certificate”). If a JabberID is included in a client certificate, it is encapsulated as an id-on-xmppAddr Object Identifier (“xmppAddr”), i.e., a subjectAltName entry of type otherName with an ASN.1 Object Identifier of “id-on-xmppAddr” as specified in Section 13.7.1.4 of RFC 6120, `XEP-0178 <http://xmpp.org/extensions/xep-0178.html#c2s>`__.

It is possible to make client certificate **required** using same VHost configuration and enabling option ``Client Certificate Required`` (``client-trust-extension-cert-required``).

If this option will be enabled, then client **must provide** certificate. This certificate will be verified against ``clientCertCA``. If client does not provide certificate or certificate will be invalid, **TLS handshake will be interrupted and client will be disconnected**.

Using this options does not force client to use SASL EXTERNAL. Client still may authenticate with other SASL mechanisms.

2.7.6. SASL Mechanisms
^^^^^^^^^^^^^^^^^^^^^^^

XMPP protocol supports many authentication methods, but most of them are used as `SASL <https://tools.ietf.org/html/rfc4422>`__ mechanisms. Tigase XMPP Server provides many SASL-based authentication mechanisms such as:

-  PLAIN *(enabled)*

-  ANONYMOUS

-  EXTERNAL

-  SCRAM-SHA-1 *(enabled)*

-  SCRAM-SHA-256 *(enabled)*

-  SCRAM-SHA-512

Most of them are enabled by default on default Tigase XMPP Server installation.

Enabling and disabling SASL mechanisms (credentials encoder/decoder)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

If you want to enable or disable one of password-based authentication mechanism such as ``SCRAM-SHA-1``, ``SCRAM-SHA-256`` or ``SCRAM-SHA-512`` you can do that by enabling or disabling encoders and decoders used on your installation. By enabling encoders/decoders you are deciding in what form the password is stored in the database. Those changes may (and in most cases will) impact which SASL mechanisms may be allowed to use on your installation.

.. Note::

   In most cases you should enable or disable both (credentials encoder and decoder) of the same type at the same time. The only exception of this rule is when you are changing those on already working installation. In this case you should only enable encoder of the type which you want to enable and request users to change their passwords. Then, after users will change their passwords, you should reconfigure server to enable decoder of the particular type. *(in other case user may loose a way to log in to your installation as system will reject their credentials as it may not have matching credentials for particular SASL mechanism)*.

**Enabling SCRAM-SHA-512 encoder**
'''''''''''''''''''''''''''''''''''
.. code:: tdsl

   authRepository () {
       default () {
           credentialEncoders () {
               'SCRAM-SHA-512' () {}
           }
       }
   }

**Disabling SCRAM-SHA-1 decoder**
'''''''''''''''''''''''''''''''''''
.. code:: tdsl

   authRepository () {
       default () {
           credentialDecoders () {
               'SCRAM-SHA-1' (active: false) {}
           }
       }
   }


.. Warning::

    It is strongly recommended not to disable encoders if you have enabled decoder of the same type as it may lead to the authentication issues, if client tries to use a mechanism which that is not available.

2.7.7. Application passwords
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

In recent versions of Tigase XMPP Server it is possible to create and use multiple username and password pairs to authorize connection to the single XMPP account.

With that in place it is now possible to have multiple password for a multiple clients accessing the same account what can be used to increase security of the account as even if one password compromised you can still log in and block lost or compromised device.

Adding application password
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

To add new username-password pair you need to execute ``Add user credentials`` ad-hoc command (command node ``auth-credentials-add`` at ``sess-man``) while logged in the XMPP account for which you want to add a new application password.

During execution for a command you will be provided with a form to fill in with following fields:

-  The Jabber ID for the account (``jid``) - bare JID of your account

-  Credential ID (``credentialId``) - username for the new application password

-  Password (``password``) - a new password

After submitting this form a new credential will be added.

Login in with application password
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

To log in with new password the XMPP client can use any SASL mechanism but it needs to provide (in SASL message):

-  ``authzid`` - account JID

-  ``authcid`` - username for application password

-  ``passwd`` - application password

With proper values, you application will be able to log in using application password.

Removing application password
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

If your device is compromised or lost and you want to remove application password, you need to use a different device and log in on your XMPP account. Then you need to execute ``Delete user credentials`` ad-hoc command (command node ``auth-credentials-delete`` at ``sess-man``).

During execution for a command you will be provided with a form to fill in with following fields:

-  The Jabber ID for the account (``jid``) - bare JID of your account

-  Credential ID (``credentialId``) - username for the application password which you want to remove

After submitting this form a credential will be removed.

2.7.8. Packet Filtering
^^^^^^^^^^^^^^^^^^^^^^^^

Tigase offers different ways to filter XMPP packets flying through the server. The most common use for packet filtering is to restrict users from sending or receiving packets based on the sender or received address.

There are also different possible scenarios: time based filtering, content filtering, volume filtering and so on.

All pages in this section describe different filtering strategies.

Domain Based Packet Filtering
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Domain based packet filtering is a simple filter allowing to restrict user communication based on the source/destination domain name. This is especially useful if we want to limit user communication within a single - own domain only or a list of domains.

A company might not wish to allow employers to chat during work hours with anybody in the world. A company may also have a few different domains used by different branches or departments. An administrator may restrict communication to a list of domains.

Introduction
'''''''''''''

The restriction is on a per-user basis. So the administrator can set a different filtering rules for each user. There is also a per-domain configuration and global-installation setting (applied from most general to most specific, i.e. from installation to user).

Regular users can not change the settings. So this is not like a privacy list where the user control the filter. Domain filter can not be changed or controlled by the user. The system administrator can change the settings based on the company policy.

There are predefined rules for packet filtering:

1. ``ALL`` - user can send and receive packets from anybody.

2. ``LOCAL`` - user can send and receive packets within the server installation only and all it’s virtual domains.

3. ``OWN`` - user can send and receive packets within his own domains only

4. ``BLOCK`` - user can’t communicate with anyone. This could be used as a means to temporarily disable account or domain.

5. ``LIST`` - user can send and receive packets within listed domains only (i.e. *whitelist*).

6. ``BLACKLIST`` - user can communicate with everybody (like ``ALL``), except contacts on listed domains.

7. ``CUSTOM`` - user can communicate only within custom created rules set.

Whitelist (``LIST``) and blacklist (``BLACKLIST``) settings are mutually exclusive, i.e. at any given point of time only one of them can be used.

Those rules applicable to particular users are stored in the user repository and are loaded for each user session. If there are no rules stored for a particular user server tries to apply rules for a VHost of particular user, and if there is no VHost filtering policy server uses global server configuration. If there is no filtering policy altogether server applies defaults based on following criteria:

1. If this is **Anonymous** user then ``LOCAL`` rule is applied

2. For all **other** users ``ALL`` rule is applied.

Configuration
''''''''''''''

Filtering is performed by the domain filter plugin which must be loaded at startup time. It is loaded by default if the plugins list is not set in the configuration file. However if you have a list of loaded plugins in the configuration file make sure ``domain-filter`` is on the list.

There is no other configuration required for the plugin to work.

Administration, Rules Management
''''''''''''''''''''''''''''''''''

Although controlling domain filtering rules is possible for each user separately, it is not practical for large installations. In most cases users are stored in the database and a third-party system keeps all the user information.

To change the rule for a single user you can use loadable administration scripts feature and load `UserDomainFilter.groovy <https://github.com/tigase/tigase-server/tree/master/src/main/groovy/tigase/admin/UserDomainFilter.groovy>`__ script. It enables modifying rules for a given user JID.

Implementation
'''''''''''''''

If you have a third party system which keeps and manages all user information than you probably have your own UserRepository implementation which allows the Tigase server to access user data. Filtering rules are loaded from user repository using following command:

.. code:: java

   repo.getData(user_id, null, DomainFilter.ALLOWED_DOMAINS_KEY, null);
   repo.getData(user_id, null, DomainFilter.ALLOWED_DOMAINS_LIST_KEY, null);

Where ``user_id`` is user Jabber ID without resource part, ``DomainFilter.ALLOWED_DOMAINS_KEY`` is a property key: ``allowed-domains``. The user repository MUST return one of following only:

1. ``ALL`` - if the user is allowed to communicate with anybody

2. ``LOCAL`` - if the user is allowed to communicate with users on the same server installation.

3. ``OWN`` - if the user is allowed to communicate with users within his own domain only.

4. ``LIST`` - list of domains within which the user is allowed to communicate with other users. No wild-cards are supported. User’s own domain should be included too.

5. ``BLACKLIST`` - list of domains within which the user is NOT allowed to communicate with other users. No wild-cards are supported. User’s own domain should NOT be included.

6. ``CUSTOM`` - list of rules defining custom communication permissions (server processes stanza according to first matched rule, similar to XEP-0016) in the following format:

::

   ruleSet = rule1;rule2;ruleX;

   rule = order_number|policy|UID_type[|UID]

   order_number = any integer;
   policy = (allow|deny);
   UID_type = [jid|domain|all];
   UID = user JID or domain, for example pubsub@test.com; if UID_type is ALL then this is ignored.

For example:

::

   1|allow|self;
   2|allow|jid|admin@test2.com;
   3|allow|jid|pubsub@test.com;
   4|deny|all;

1. ``null`` - a java null if there are no settings for the user.

In case of ``LIST`` and ``BLACKLIST`` filtering options, it’s essential to provide list of domains for the whitelisting/blacklisting. ``DomainFilter.ALLOWED_DOMAINS_LIST_KEY`` is a property key: "allowed-domains-list". The user repository MUST return semicolon separated list of domains: ``domain1.com;domain2.com,domain3.org``

The filtering is performed by the ```tigase.xmpp.impl.DomainFilter`` <https://github.com/tigase/tigase-server/tree/master/src/main/java/tigase/xmpp/impl/DomainFilter.java>`__ plugin. Please refer to source code for more implementation details.

2.7.9. Access Control Lists in Tigase
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Tigase offers support for **Access Control List (ACL)** to allow for fine grained access to administration commands on the server.

By default, all administration commands are only accessible (visible through service discovery and can be executed) by the service administrators. Service administrators are existing accounts with JIDs (**BareJIDs**) listed in the ``config.tdsl`` file under ``admins = []`` (please see `??? <#admins>`__ for details).

Additionally, other XMPP users and entities can be assigned permissions to execute a command or commands using Tigase’s ACL capabilities.

The following is a list of possible ACL modifiers for administrator command accessibility:

-  ``ALL`` - Everybody can execute the command, even users from different federated servers.

-  ``ADMIN`` - Local server administrators can execute the command, this is a default setting if no ACL is set for a command.

-  ``LOCAL`` - All users with accounts on the local server can execute the command. Users from other, federated servers will not be able to execute the command.

-  ``NONE`` - No one will be allowed to execute this command

-  ``DOMAIN_OWNER`` - Only user which is owner of the domain which items are being manipulated is allowed to execute the comment. If script is not checking permissions for the manipulated item, this value will behave in the same way as ``LOCAL``.

-  ``DOMAIN_ADMIN`` - Only user which is one of the domain administrators will be able to execute the command manipulating items related to the domain. If script is not checking permissions for the manipulated item, this value will behave in the same way as ``LOCAL``.

-  ``example.com`` - Only users with accounts on the selected domain will be able to execute the command. It may be useful to setup a domain specifically for admin accounts, and automatically all users within that domain would be able to run the command.

-  ``user@example.com`` - Comma separated list of JIDs of users who can execute the command.

In any case, regardless of ACL settings, any command can be executed and accessed by the designated service wide administrators, that is accounts listed as admins in the ``config.tdsl`` file.

Multiple ACL modifiers can be combined and applied for any command. This may not always makes sense. For example ALL supersedes all other settings, so it does not make sense to combine it with any other modifier. However, most others can be combined with JID to broaden access to specific accounts.

On Tigase server the Access Control List is checked for the first matching modifier. Therefore if you combine ALL with any other modifier, anybody from a local or remote service will always be able to execute the command, no matter what other modifiers are added.

Please note, the ACL lists work on the command framework level. Access is verified before the command is actually executed. There might be additional access restrictions within a command itself. In many cases, even if all local users are permitted to execute a command (LOCAL modifier), some commands allow only to be executed by a domain owner or a domain administrator (and of course by the service-wide administrators as well). All the commands related to a user management such as adding a new user, removing a user, password changes, etc… belong to this category. When conducting domain (vhost) management, creation/registration of a new domain can be done by any local user (if LOCAL ACL modifier is set) but then all subsequent domain management tasks such as removing the vhost, updating its configuration, setting SSL certificate can be done by the domain owner or administrator only.

The ACL list is set for a specific Tigase component and a specific command. Therefore the configuration property must specify all the details. So the general format for configuring ACL for a command is this:

.. code:: dsl

   comp-id () {
       commands {
           'command-id' = [ 'ACL_modifier', 'ACL_modifier', 'ACL_modifier' ]
       }
   }

The breakdown is as such:

-  ``comp-id`` is the Tigase server component ID such as: sess-man, vhost-man, c2s, etc..

-  ``commands`` is a static text which indicates that the property is for component’s command settings.

-  ``command-id`` is a command ID for which we set the ACL such as query-dns, http://jabber.org/protocol/admin#add-user, user-roster-management, etc…

Here are a few examples:

*Allowing local users to create and manage their own domains*

.. code:: dsl

   'vhost-man' () {
       commands {
           'comp-repo-item-add' = 'LOCAL'
           'comp-repo-item-remove' = 'LOCAL'
           'comp-repo-item-update' = 'LOCAL'
           'ssl-certificate-add' = 'LOCAL'
       }
   }

In fact all the commands except item-add can be executed by the domain owner or administrator.

*Allowing local users to execute user management commands:*

.. code:: dsl

   'sess-man' () {
       'commands' {
           'http://jabber.org/protocol/admin#add-user' = 'LOCAL'
           'http://jabber.org/protocol/admin#change-user-password' = 'LOCAL'
           'http://jabber.org/protocol/admin#delete-user' = 'LOCAL'
           'http://jabber.org/protocol/admin#get-online-users-list' = 'LOCAL'
           'http://jabber.org/protocol/admin#get-registered-user-list' = 'LOCAL'
           'http://jabber.org/protocol/admin#user-stats' = 'LOCAL'
           'http://jabber.org/protocol/admin#get-online-users-list' = 'LOCAL'
       }
   }

As in the previous example, the commands will by executed only by local users who are the specific domain administrators.

*Allowing users from a specific domain to execute query-dns command and some other users for given JIDs from other domains:*

.. code:: dsl

   'vhost-man' () {
       'commands' {
           'query-dns' = [ 'tigase.com', 'admin@tigase.org', 'frank@example.com' ]
       }
   }

To be able to set a correct ACL property you need to know component names and command IDs. Component IDs can be found in the service discovery information on running server or in the server logs during startup. A command ID can be found in the command script source code. Each script contains a list of metadata at the very beginning of it’s code. One of them is ``AS:CommandId`` which is what you have to use for the ACL setting.

2.7.10. TLS/SSL encryption features configuration
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^


Tigase allows adjusting the most important parameters used when establishing TLS connections - set of protocols and ciphers that will be used during negotiation of the connection. The single most important is ``hardened-mode`` - it’s the most general configuration and offers three-step adjustment of the settings - please see `??? <#hardenedMode>`__ for details. ``hardened-mode`` can be configured both via TDSL configuration file (either on ``root`` level or for ``sslContextContainer`` for particular connection managers) or on VHost level.

If you want to disable certain protocols or ciphers you can use two options: ``tls-disabled-protocols`` and ``tls-disabled-ciphers`` respectively. They allow, as name suggests, disabling certain items from default sets. They both takes an array of strings, which ten be removed from the lists.

Let’s say you’d like to remove support for ``SSL``, ``SSLv2`` and ``SSLv3`` protocols. You should simply use following configuraiton: ``'tls-disabled-protocols' = ['SSL', 'SSLv2', 'SSLv3']``. Complete list of protocols depends on particular Java version that you use - please refer to the documentation for details. For example for the default Java11 list you can check `SSLContext Algorithms <https://docs.oracle.com/en/java/javase/11/docs/specs/security/standard-names.html#sslcontext-algorithms>`__

``tls-disabled-ciphers`` follows same format and uses names defined in `JSSE Cipher Suite Names <https://docs.oracle.com/en/java/javase/11/docs/specs/security/standard-names.html#jsse-cipher-suite-names>`__. It’s also possible to use regular expressions to quickly eliminate groups of ciphers.

If you want to enable only specific protocols or ciphers irrespective of ``hardened-mode`` or above disabling options you can use ``tls-enabled-protocols`` and ``tls-enabled-ciphers`` - those two options take arrays as well and they will configure Tigase to use only those protocols or ciphers that are provided (without support for regular expressions). Therefore if you configure Tigase with ``'tls-enabled-protocols' = [ 'TLSv1.2' ]`` then **only** ``TLSv1.2`` will be supported by Tigase.

The last option that you may be interested in adjusting is ``ephemeral-key-size`` - it follows Java’s configuration capabilities outlined in `Customizing Size of Ephemeral Diffie-Hellman Keys <https://docs.oracle.com/en/java/javase/11/security/java-secure-socket-extension-jsse-reference-guide.html#GUID-D9B216E8-3EFC-4882-B76E-17A87D8F2F9D>`__. Tigase defaults Diffie-Hellman keys of 4096 bits.

.. Important::

   We try to provide the best default set of options therefore **it’s recommendable to use defaults provided by Tigase**. If you want to make your extremely secure (considering possible connectivity issues with installations that may be less secure) then you should only adjust ``hardened-mode`` setting (and switch it to ``strict``).

Testing hosts TLS capabilities
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

If you run into issues with TLS connectivity it’s helpful to compare if both installations support same set of protocols and ciphers. One of the most versatile and helpful tools is `Mozilla’s CipherScan <https://github.com/mozilla/cipherscan>`__. For example for our installation ``tigase.im`` result would look like this:

::

   $ ./cipherscan --curves -starttls xmpp -servername tigase.im tigase.me:5222
   .......................................................................
   Target: tigase.me:5222

   prio  ciphersuite                  protocols              pfs                 curves
   1     ECDHE-RSA-AES256-GCM-SHA384  TLSv1.2                ECDH,B-571,570bits  sect283k1,sect283r1,sect409k1,sect409r1,sect571k1,sect571r1,secp256k1,prime256v1,secp384r1,secp521r1
   2     ECDHE-RSA-AES256-SHA384      TLSv1.2                ECDH,B-571,570bits  sect283k1,sect283r1,sect409k1,sect409r1,sect571k1,sect571r1,secp256k1,prime256v1,secp384r1,secp521r1
   3     ECDHE-RSA-AES256-SHA         TLSv1,TLSv1.1,TLSv1.2  ECDH,B-571,570bits  sect283k1,sect283r1,sect409k1,sect409r1,sect571k1,sect571r1,secp256k1,prime256v1,secp384r1,secp521r1
   4     DHE-RSA-AES256-GCM-SHA384    TLSv1.2                DH,4096bits         None
   5     DHE-RSA-AES256-SHA256        TLSv1.2                DH,4096bits         None
   6     DHE-RSA-AES256-SHA           TLSv1,TLSv1.1,TLSv1.2  DH,4096bits         None
   7     ECDHE-RSA-AES128-GCM-SHA256  TLSv1.2                ECDH,B-571,570bits  sect283k1,sect283r1,sect409k1,sect409r1,sect571k1,sect571r1,secp256k1,prime256v1
   8     ECDHE-RSA-AES128-SHA256      TLSv1.2                ECDH,B-571,570bits  sect283k1,sect283r1,sect409k1,sect409r1,sect571k1,sect571r1,secp256k1,prime256v1,secp384r1,secp521r1
   9     ECDHE-RSA-AES128-SHA         TLSv1,TLSv1.1,TLSv1.2  ECDH,B-571,570bits  sect283k1,sect283r1,sect409k1,sect409r1,sect571k1,sect571r1,secp256k1,prime256v1,secp384r1,secp521r1
   10    DHE-RSA-AES128-GCM-SHA256    TLSv1.2                DH,4096bits         None
   11    DHE-RSA-AES128-SHA256        TLSv1.2                DH,4096bits         None
   12    DHE-RSA-AES128-SHA           TLSv1,TLSv1.1,TLSv1.2  DH,4096bits         None

   Certificate: trusted, 2048 bits, sha256WithRSAEncryption signature
   TLS ticket lifetime hint: None
   NPN protocols: None
   OCSP stapling: not supported
   Cipher ordering: client
   Curves ordering: client - fallback: no
   Server supports secure renegotiation
   Server supported compression methods: NONE
   TLS Tolerance: yes

TLS 1.3 compatibility
~~~~~~~~~~~~~~~~~~~~~~

Due to compatibility issues, TLS 1.3 is currently (version 8.1.x) disabled by default. It can be enabled by setting property ``tls-disable-tls13`` of ``sslContextContainer`` bean to ``false``:

::

   sslContextContainer () {
       'tls-disable-tls13' = false
   }

2.8. Database Management
------------------------

Tigase is coded to perform with multiple database types and numbers. Owing to it’s versatile nature, there are some tools and procedures that may be of use to certain administrators.

2.8.1. Recommended database versions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

As of v8.0.0 here are the minimum and recommended versions of databases for use with Tigase:

+------------+---------------------+-----------------+------------------------------------------------------------------------------------------------------------------------------------+
| Database   | Recommended Version | Minimum Version | Additional Information                                                                                                             |
+============+=====================+=================+====================================================================================================================================+
| DerbyDB    | 10.12.1.1           | 10.12.1.1       | Included with Tigase XMPP Server                                                                                                   |
+------------+---------------------+-----------------+------------------------------------------------------------------------------------------------------------------------------------+
| MySQL      | 5.7                 | 5.6.4           | Required to properly support timestamp storage with millisecond precision                                                          |
+------------+---------------------+-----------------+------------------------------------------------------------------------------------------------------------------------------------+
| SQLServer  | 2014                | 2012            | 2012 needed so we can count use fetch-offset pagination feature.                                                                   |
+------------+---------------------+-----------------+------------------------------------------------------------------------------------------------------------------------------------+
| PostgreSQL | 13.0                | 9.4             | New UA schema requires at least 9.4; if using version older than 13 manual installation of ``uuid-ossp`` extension is required (1) |
+------------+---------------------+-----------------+------------------------------------------------------------------------------------------------------------------------------------+
| MongoDB    | 3.2                 | 3.0             |                                                                                                                                    |
+------------+---------------------+-----------------+------------------------------------------------------------------------------------------------------------------------------------+
| MariaDB    | ?                   | 10.0.12         | Basic features works with 10.0.12-MariaDB Homebrew, but is not fully tested.                                                       |
+------------+---------------------+-----------------+------------------------------------------------------------------------------------------------------------------------------------+

.. Note::

   (1) For PostgreSQL version older than 13.0 manual installation of ``uuid-ossp`` by the superuser to the *created database* is required:

   .. code:: postgresql

      CREATE EXTENSION IF NOT EXISTS "uuid-ossp";

Although Tigase may support other versions of databases, these are the ones we are most familiar with in offering support and advice. Use of databases outside these guidelines may result in unforeseen errors.

2.8.2. Database Watchdog
^^^^^^^^^^^^^^^^^^^^^^^^^

It is possible to have Tigase test availability and existence of database periodically only when db connections are idle. By default this ping is sent once every 60 minutes to each connected repository. However this can be overridden as a part of the dataSource property:

.. code:: properties

   dataSource {
       default () {
           uri = '....'
       }
       'test' () {
           uri =  '...'
           'watchdog-frequency' = 'PT30M'
       }
   }

This setting changes frequency to 30 minutes.

.. code:: properties

   dataSource {
       default () {
           uri = '...'
       }
       'watchdog-frequency' = 'PT15M'
   }

This one changes to 15 minutes.

.. Note::

   see `??? <#periodDurationValues>`__ for format details


2.8.3. Using modified database schema
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

If you are using Tigase XMPP Server with modified schema (changed procedures or tables) and you do not want Tigase XMPP Server to maintain it and automatically upgrade, you can disable ``schema-management`` for any data source. If ``schema-management`` is disable for particular data source then Tigase XMPP Server will not update or modify database schema in any way. Moreover it will not check if schema version is correct or not.

**Disabling ``schema-management`` for ``default`` data source**

.. code:: tdsl

   dataSource {
       default () {
           uri = '...'
           'schema-management' = false
       }
   }

.. Warning::

    If ``schema-management`` is disabled, then it is administrator responsibility to maintain database schema and update it if needed (ie. if Tigase XMPP Server schema was changed).

2.8.4. Schema files maintenance
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

This document describes schema files layout and assumptions about it. In addition it describes how and when it should be updated.

Assumptions
~~~~~~~~~~~

Following assumptions are in place:

-  All schema files are *loadable* multiple times - this is by far most important assumptions and it’s allow to get away without explicit and detailed checking of loaded version (it’s already handled on the schema level as of version 8.0.0)

-  Required schema version is calculated from the component version (which is set in the project configuration file - usually ``pom.xml``, but it’s possible to override it in code via annotations - please see Developer Guild in Server documentation for details)

-  we will maintain *"3 versions schema files"*, i.e. in the distribution package we will provide schema versions for the ``current_version`` and two major versions behind (and all maintenance version schema files) - this will allow *quick upgrade* even from rather older versions

-  ``SNAPSHOT`` versions will print a log entry indicating that there may have been changes in schema and it’s recommended to run the upgrade (we are aiming at frequent releases thus mandatory schema version check will be done only with final version)

Checks
~~~~~~

We will check:

-  if it’s possible to upgrade the schema (based on the current schema version in the database and available SQL files and their respective versions - if );

-  if it’s required to upgrade the schema during server startup (until 7.1.x [inclusive] it was done only for tigase-server, will be done by all components)

-  if it’s required to upgrade the schema during run of ``upgrade-schema``) (if schema is already in the latest required version, executing all SQL files is not required hence speeding up upgrade)

   -  During startup of ``SNAPSHOT`` version, even if the schema version match, a prompt to re-run ``upgrade-schema`` will be printed in the ``logs/tigase-console.log``

Schema files layout
~~~~~~~~~~~~~~~~~~~~

Filename layout
'''''''''''''''

Basic schema filename layout consists of 3 basic parts:

-  name of relational database management system (RDBMS) for which it’s intended (e.g. ``derby``, ``mysql``, ``postgresql``, ``sqlserver``);

-  name of the Tigase component for which it’s intended;

-  version of the schema file.

For each component and version it’s possible (but not mandatory) to split all database related functionality into multiple files but it’s essential that they would be linked/included in the base file for particular database/component/version file. This allows separating Stored Procedures (``-sp``), base schema (``-schema``) and setting properties (``-props``). In principle the filename pattern looks as follows

::

   <RDBMS_name>-<tigase_component>-schema-<version>[-<sub_schema>].sql

For example schema file for version 7.0.0 of Tigase Server for Derby looks as follow:

::

   derby-server-schema-7.0.0-schema.sql


Files structure
''''''''''''''''

As mentioned before, we should support all versions matching ``old-stable``, ``stable`` and ``master``, which translates to two main versions behind *current-version*, that is version: *current-version - 2*). This results in having 3 versions of the schema in the repository at any given time (two of them being \``upgrades'' to the oldest, base schema):

-  ``current-version`` *minus* 2: base schema

-  ``current-version`` *minus* 1: all changes from ``current-version`` *minus* 2 to ``current-version`` *minus* 1

-  ``current-version``: all changes from ``current-version`` *minus* 1 to ``current-version``

.. Note::

   ``current-version`` *MUST* always match version of the component (defined in pom.xml).

 .. Note::

   It’s possible to have multiple files within version (related to smaller, maintenance upgrade) as the SchemaLoader would collect all files which version falls within range and .

For example with the release of version 8.0.0 this will translate to following versions:

-  ``7.0.0``: base schema

-  ``7.1.0``: all changes from ``7.0.0`` to ``7.1.0``

-  ``8.0.0``: all changes from ``7.1.0`` to ``8.0.0``

.. Note::

   All schema files must be stored under ``src/main/database/``


Handling of changes in the schema
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

There are two main workflows defined


During release of the version
''''''''''''''''''''''''''''''

As we keep at the most only 3 versions of the schema, after release of the version we need to adjust (flatten) the files to maintain structure defined in *Files structure* (it may happen, that there wouldn’t be any changes in the schema for particular version which will result in relatively empty ``current-version`` schema file – only setting current version for component with ``setVersion('component','<current-version></current-version>');`` ).

For example we are about to release version ``8.0.0``. This results in the following versions of the schema (in the example for the server) in the repository:

-  ``<database>-server-schema-7.0.0.sql``: base schema

-  ``<database>-server-schema-7.1.0.sql``: including changes for ``7.1.0``

-  ``<database>-server-schema-8.0.0.sql``: including changes for ``8.0.0``

.. Note::

   It’s possible that there will be maintenance versions in the list as well, e.g.: ``<database>-server-schema-7.1.1.sql`` and ``<database>-server-schema-7.1.2.sql``

After the release we specify the version of the next release in pom.xml (for example ``8.1.0`` and the same version will be the ``current-version`` making the oldest available version ``7.1.0``. Because of that we *MUST* incorporate all the changes in ``7.1.0`` onto ``7.0.0`` creating new base file with version ``7.1.0``, i.e.:

-  ``<database>-server-schema-7.1.0.sql``: base schema

-  ``<database>-server-schema-8.0.0.sql``: including changes for ``8.0.0``

-  ``<database>-server-schema-8.1.0.sql``: including changes for ``8.1.0``

Maintenance releases
'''''''''''''''''''''

Following cases will be discussed with solid-version examples. Comments will be provided in-line Following assumptions are made:

-  Version succession: ``5.1.0``, ``5.2.0``, ``7.0.0``, ``7.1.0``, ``8.0.0``

-  Versions mapping: ``master`` (``8.0.0``), ``stable`` (``7.1.0``), ``old-stable`` (``7.0.0``):

   -  schema files in ``old-stable`` branch

      -  5.1.0 (base)

      -  5.2.0 (upgrade)

      -  7.0.0 (upgrade)

   -  schema files in ``stable`` branch

      -  5.2.0 (base)

      -  7.0.0 (upgrade)

      -  7.1.0 (upgrade)

   -  schema files in ``master`` branch

      -  7.0.0 (base)

      -  7.1.0 (upgrade)

      -  8.0.0 (upgrade)


Making a change in ``old-stable`` (and ``stable``)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

If we made a schema change in ``old-stable`` version (and it’s branch) we must:

-  create a new file with upgraded version number;

-  propagate the change to the ``stable`` and ``master`` branch.

Repository changes:

-  schema files in ``old-stable`` branch

   -  5.1.0 (base)

   -  5.2.0 (upgrade)

   -  7.0.0 (upgrade)

   -  7.0.1 (upgrade) **←** making a *change* here results in the schema version being bumped to 7.0.1

-  schema files in ``stable`` branch

   -  5.2.0 (base)

   -  7.0.0 (upgrade)

   -  7.0.1 (upgrade) **←** we must port the *change* here

   -  7.1.0 (upgrade)

-  schema files in ``master`` branch

   -  7.0.0 (base)

   -  7.0.1 (upgrade) **←** we must port the *change* here

   -  7.1.0 (upgrade)

   -  8.0.0 (upgrade)


Making a change in ``master``
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

If we made a schema change in ``master`` version we don’t propagate the change to the ``stable`` and ``old-stable`` branch.

-  schema files in ``old-stable`` branch

   -  5.1.0 (base)

   -  5.2.0 (upgrade)

   -  7.0.0 (upgrade)

-  schema files in ``stable`` branch

   -  5.2.0 (base)

   -  7.0.0 (upgrade)

   -  7.1.0 (upgrade)

-  schema files in ``master`` branch

   -  7.0.0 (base)

   -  7.1.0 (upgrade)

   -  8.0.0 (upgrade) **←** we make the *change* here, as this is the development version schema version remains the same.


Implementation details
~~~~~~~~~~~~~~~~~~~~~~~

In-file control
''''''''''''''''

There are two main control instructions (intended for ``SchemaLoader``):

-  denoting Queries with ``-- QUERY START:`` and ``-- QUERY END:`` - each must be placed in own, separate file with the query being enclosed by the two of them, for example:

   .. code:: sql

      -- QUERY START:
      call TigPutDBProperty('schema-version', '5.1');
      -- QUERY END:

-  sourcing other file with ``-- LOAD FILE: <path to .sql file>`` - path must be on the same line, following control instruction, for example:

   .. code:: sql

      -- LOAD FILE: database/mysql-server-schema-7.0.0-schema.sql


Storing version in the database
''''''''''''''''''''''''''''''''

Each repository will have a table ``tig_schema_versions`` with the information about all installed components and it’s versions in that particular repository. There will be an associated stored procedure to obtain and set version:

-  table:

   .. code:: sql

      tig_schema_versions (
        component varchar(100) NOT NULL,
        version varchar(100) NOT NULL,
        last_update timestamp NOT NULL,
        primary key (component)
      );

-  stored procedures ``get/setVersion(‘component’,'version');``

It will be stored and maintained in the file named ``<RDBMS_name>-common-schema-<version>.sql``

2.8.5. Database Preparation
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Tigase uses generally the same database schema and the same set of stored procedures and functions on every database. However, the schema creation scripts and code for stored procedures is different for each database. Therefore the manual process to prepare database is different for each database system.

Starting with v8.0.0, most of the database tasks have been automated and can be called using simple text, or using interactive question and answer style. We **DO NOT RECOMMEND** going through manual operation, however we have kept manual activation of different databases to the Appendix. If you are interested in how we manage and update our database schemas, you may visit the `??? <#SchemaMaintenance>`__ section of our Redmine installation for more detailed information.

-  `The DBSchemaLoader Utility <#dbSchemaLoader>`__

-  `Hashed User Passwords in Database <#hashedPasswords>`__

-  `Support for MongoDB <#mongoDBSupport>`__

Appendix entries

-  `Manual installtion for MySQL <#prepareMysql>`__

-  `Manual installtion for Derby <#prepareDerby>`__

-  `Manual installtion for SQLServer <#prepareMssql>`__

-  `Manual installtion for PostGRESQL <#preparePostgresql>`__

Schema Utility
~~~~~~~~~~~~~~

With the release of v8.0.0 calling the Tigase dbSchemaLoader utility now can be done using tasks instead of calling the specific method. Support for Derby, MySQL, PostgreSQL, MSSQL, and MongoDB is available.

In order to use this utility with any of the databases, you will need to first have the database environment up and running, and have established user credentials. You may use root or an account with administrator write privileges.

Operation & Variables
'''''''''''''''''''''

Operation

Operating the schema utility is quite easy! To use it run this command from the installation directory:

.. code:: command

   ./scripts/tigase.sh [task] [params_file.conf] [options]

Operations are now converted to tasks, of which there are now three: ``install-schema``, ``upgrade-schema``, and ``destroy-schema``.

-  ``upgrade-schema``: Upgrade the schema of the database specified in your ``config.tdsl`` configuration file. (options are ignored for this option)

-  ``install-schema``: Install a schema to database.

-  ``destroy-schema``: Destroy database and schemas. **DANGEROUS**

Options

Use the following options to customize. Options in bold are required, *{potential options are in brackets}*:

-  ``--help`` Prints the help for the task.

-  ``-I`` or ``--interactive`` - enables interactive mode which will prompt for parameters not defined.

-  ``-T`` or ``--dbType`` - database type {derby, mongodb, mysql, postgresql, sqlserver}.

-  ``-C`` or ``--components`` - Allows the specification of components for use when installing a schema.

Usage
'''''

upgrade-schema

This task will locate any schema versions above your current one, and will install them to the database configured in the ``config.tdsl`` file.

.. Note::

   To use this utility, you must have Tigase XMPP server fully setup with a configured configuration file.

.. code:: command

   ./scripts/tigase.sh upgrade-schema etc/tigase.conf

Windows users will need to run the command using the following command:

.. code:: windows

   java -cp "jars/*" tigase.db.util.SchemaManager "upgrade-schema" --config-file=etc/config.tdsl

install-schema

This task will install a schema using the parameters provided.

**If you are setting up a server manually, we HIGHLY recommend using this method**

.. code:: command

   ./scripts/tigase.sh install-schema [Options]

This command will install tigase using a Derby database on one named ``tigasedb`` hosted on ``localhost``. The username and password editing the database is ``tigase_pass`` and ``root``. Note that ``-J`` explicitly adds the administrator, this is highly recommended with the ``-N`` passing the password.

If you are using a windows system, you need to call the program directly:

.. code:: windows

   java -cp "jars/*" tigase.db.util.SchemaManager "install-schema" [options]


Options

Options for schema installation are as follows, required options are in bold

-  ``--help``, Outputs the help.

-  ``-I``, ``--interactive`` - enables interactive mode, which will result in prompting for any missing parameters.

-  ``-C``, ``--components=`` - list of enabled components identifiers (+/-), possible values: [``amp``, ``bosh``, ``c2s``, ``eventbus``, ``ext-disco``, ``http``, ``mdns``, ``message-archive``, ``monitor``, ``muc``, ``pubsub``, ``push``, ``s2s``, ``socks5``, ``test``, ``unified-archive``, ``upload``, ``ws2s``] (default: amp,bosh,c2s,eventbus,http,message-archive,monitor,muc,pubsub,s2s,ws2s). **This is required for certain components like socks5.**

-  ``-T``, ``--dbType=`` - database server type, possible values are: [``derby``, ``mongodb``, ``mysql``, ``postgresql``, ``sqlserver``] (*required*)

-  ``-D``, ``--dbName=`` - name of the database that will be created (by default it is ``tigasedb``). (*required*)

-  ``-H``, ``--dbHostname=`` - address of the database instance (by default it is ``localhost``). (*required*)

-  ``-U``, ``--dbUser=`` - name of the user that will be created specifically to access Tigase XMPP Server database (default is ``tigase_user``). (*required*)

-  ``-P``, ``--dbPass=`` - password of the user that will be created specifically to access Tigase XMPP Server database (default is ``tigase_pass``). (*required*)

-  ``-R``, ``--rootUser=`` - database root account username used to create user and database (default is ``root``). (*required*)

-  ``-A``, ``--rootPass=`` - database root account password used to create user and database (default is ``root``). (*required*)

-  ``-S``, ``--useSSL`` - enable SSL support for database connection (if the database supports it) (default is false).

-  ``-F``, ``--file=`` - comma separated list of SQL files that will be processed.

-  ``-Q``, ``--query=`` - custom queries to be executed, see `Query function <#queryschema>`__ for details.

-  ``-L``, ``--logLevel=`` - logger level used during loading process (default is ``CONFIG``).

-  ``-J``, ``--adminJID=`` - comma separated list of administrator JID(s).

-  ``-N``, ``--adminJIDpass=`` - password that will be used for the entered JID(s) - one password for all configured JIDs.

-  ``--getURI=`` - generate database URI (default is ``false``).

-  ``--ignoreMissingFiles=`` - force ignoring missing files errors (default is ``false``).

Query function

Should you decide to customize your own functions, or have specific information you want to put into the database, you can use the -query function to perform a single query step.

.. code:: cmd

   ./scripts/tigase.sh install-schema -T mysql -D tigasedb -R root -A root -Q "CREATE TABLE tigasedb.EXTRA_TABLE (id INT(6) UNSIGNED AUTO_INCREMENT PRIMARY KEY, name VARCHAR(10) NOT NULL)"

Of course this would break the schema for tigasedb by adding an unexpected table, you will receive the following message:

::

   tigase.db.util.DBSchemaLoader       printInfo          WARNING       Database schema is invalid

But this is a demonstration how you may run a query through the database without the need to use another tool. Note that you will need to select the specific database for each query.

destroy-schema


This will destroy the database specified in the configuration file.

.. Warning::

    **THIS ACTION IS NOT REVERSIBLE**

.. code:: cmd

   ./scripts/tigase.sh destroy-schema etc/config.tdsl

Only use this if you wish to destroy a database and not have the information recoverable.

Windows users will need to call the method directly:

.. code:: cmd

   java -cp "jars/*" tigase.db.util.SchemaManager "destroy-schema" etc/config.tdsl


A note about MySQL

If you are using these commands, you may result in the following error:

.. code:: bash

   tigase.util.DBSchemaLoader       validateDBConnection    WARNING    Table 'performance_schema.session_variables' does not exist

If this occurs, you will need to upgrade your version of MySQL using the following command:

.. code:: bash

   mysql_upgrade -u root -p --force

After entering the password and upgrading MySQL the schema error should no longer show when working with Tigase databases.

Prepare the MySQL Database for the Tigase Server
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

This guide describes how to prepare MySQL database for connecting Tigase server.

The MySQL database can be prepared in many ways. Most Linux distributions contain tools which allow you to go through all steps from the shell command line. To make sure it works on all platforms in the same way, we will first show how to do it under MySQL command line client.

Configuring from MySQL command line tool
'''''''''''''''''''''''''''''''''''''''''

Run the MySQL command line client in either Linux or MS Windows environment and enter following instructions from the Tigase installation directory:

.. code:: sql

   mysql -u root -p

Once logged in, create the database for the Tigase server:

.. code:: sql

   mysql> create database tigasedb;

Add the ``tigase_user`` user and grant him access to the ``tigasedb`` database. Depending on how you plan to connect to the database (locally or over the network) use one of following commands or all if you are not sure:

-  Grant access to tigase_user connecting from any network address.

   .. code:: sql

      mysql> GRANT ALL ON tigasedb.* TO tigase_user@'%'
                  IDENTIFIED BY 'tigase_passwd';

-  Grant access to tigase_user connecting from localhost.

   .. code:: sql

      mysql> GRANT ALL ON tigasedb.* TO tigase_user@'localhost'
                  IDENTIFIED BY 'tigase_passwd';

-  Grant access to tigase_user connecting from local machine only.

   .. code:: sql

      mysql> GRANT ALL ON tigasedb.* TO tigase_user
                  IDENTIFIED BY 'tigase_passwd';

And now you can update user permission changes in the database:

.. code:: sql

   mysql> FLUSH PRIVILEGES;

.. Important::

   It’s essential to enable `log_bin_trust_function_creators <https://dev.mysql.com/doc/refman/8.0/en/replication-options-binary-log.html#sysvar_log_bin_trust_function_creators>`__ option in MySQL server, for example by running:

   .. code:: sql

      mysql> SET GLOBAL log_bin_trust_function_creators = 1;

Installing Schemas

Starting with v8.0.0 the Schemas are no longer linked, and will need to manually be installed in the following order.

Switch to the database you have created:

.. code:: sql

   mysql> use tigasedb;

..  Note::

   We are assuming you run the mysql client in Linux from the Tigase installation directory, so all file links will be relative.

Next install the schema files:

.. code:: sql

   mysql> source database/mysql-common-0.0.1.sql;

You will need to repeat this process for the following files:

.. code:: list

   mysql-common-0.0.1.sql
   mysql-common-0.0.2.sql
   mysql-server-7.0.0.sql
   mysql-server-7.1.0.sql
   mysql-server-8.0.0.sql
   mysql-muc-3.0.0.sql
   mysql-pubsub-3.1.0.sql
   mysql-pubsub-3.2.0.sql
   mysql-pubsub-4.0.0.sql
   mysql-http-api-2.0.0.sql

Other components may require installation such as:

.. code:: list

   mysql-socks5-2.0.0.sql
   mysql-push-1.0.0.sql
   mysql-message-archiving-2.0.0.sql
   mysql-unified-archive-2.0.0.sql


Windows instructions:

On Windows you have probably to enter the full path, assuming Tigase is installed in C:\Program Files\Tigase:

.. code:: sql

   mysql> source c:/Program Files/Tigase/database/mysql-common-0.0.1.sql;
   mysql> source c:/Program Files/Tigase/database/mysql-common-0.0.2.sql;
   mysql> source c:/Program Files/Tigase/database/mysql-server-7.0.0.sql;
   and so on...


Configuring From the Linux Shell Command Line
''''''''''''''''''''''''''''''''''''''''''''''

Follow steps below to prepare the MySQL database:

Create the database space for the Tigase server:

.. code:: sql

   mysqladmin -p create tigasedb

Add the ``tigase_user`` user and grant access to the tigasedb database. Depending on how you plan to connect to the database (locally or over the network) use one of following commands or all if you are not sure:

Selective access configuration

Grant access to tigase_user connecting from any network address.

.. code:: sql

   echo "GRANT ALL ON tigasedb.* TO tigase_user@'%' \
               IDENTIFIED BY 'tigase_passwd'; \
               FLUSH PRIVILEGES;" | mysql -u root -pdbpass mysql


Grant access to tigase_user connecting from localhost.

.. code:: sql

   echo "GRANT ALL ON tigasedb.* TO tigase_user@'localhost' \
               IDENTIFIED BY 'tigase_passwd'; \
               FLUSH PRIVILEGES;" | mysql -u root -pdbpass mysql


Grant access to tigase_user connecting from local machine only.

.. code:: sql

   echo "GRANT ALL ON tigasedb.* TO tigase_user \
               IDENTIFIED BY 'tigase_passwd'; \
               FLUSH PRIVILEGES;" | mysql -u root -pdbpass mysql


Schema Installation

Load the proper mysql schemas into the database.

.. code:: sql

   mysql -u dbuser -p tigasedb < mysql-common-0.0.1.sql
   mysql -u dbuser -p tigasedb < mysql-common-0.0.2.sql
   etc..

You will need to repeat this process for the following files:

.. code:: list

   mysql-common-0.0.1.sql
   mysql-common-0.0.2.sql
   mysql-server-7.0.0.sql
   mysql-server-7.1.0.sql
   mysql-server-8.0.0.sql
   mysql-muc-3.0.0.sql
   mysql-pubsub-3.1.0.sql
   mysql-pubsub-3.2.0.sql
   mysql-pubsub-4.0.0.sql
   mysql-http-api-2.0.0.sql

Other components may require installation such as:

.. code:: list

   mysql-socks5-2.0.0.sql
   mysql-push-1.0.0.sql
   mysql-message-archiving-2.0.0.sql
   mysql-unified-archive-2.0.0.sql


Configuring MySQL for UTF-8 Support
'''''''''''''''''''''''''''''''''''

In my.conf put following lines:

.. code:: bash

   [mysql]
   default-character-SET=utf8

   [client]
   default-character-SET=utf8

   [mysqld]
   init_connect='SET collation_connection = utf8_general_ci; SET NAMES utf8;'
   character-set-server=utf8
   default-character-SET=utf8
   collation-server=utf8_general_ci
   skip-character-set-client-handshake

Then connect to the database from the command line shell check settings:

.. code:: sql

   SHOW VARIABLES LIKE 'character_set_database';
   SHOW VARIABLES LIKE 'character_set_client';

If any of these shows something else then 'utf8' then you need to fix it using the command:

.. code:: sql

   ALTER DATABASE tigasedb DEFAULT CHARACTER SET utf8;

You can now also test your database installation if it accepts UTF-8 data. The easiest way to ensure this is to just to create an account with UTF-8 characters:

.. code:: sql

   call TigAddUserPlainPw('żółw@some.domain.com', 'żółw');

And then check that the account has been created:

.. code:: sql

   SELECT * FROM tig_users WHERE user_id = 'żółw@some.domain.com';

If the last command gives you no results it means there is still something wrong with your settings. You might also want to check your shell settings to make sure your command line shell supports UTF-8 characters and passes them correctly to MySQL:

.. code:: sh

   export LANG=en_US.UTF-8
   export LOCALE=UTF-8
   export LESSCHARSET='utf-8'

It seems that MySQL 5.0.x also needs extra parameters in the connection string: '&useUnicode=true&characterEncoding=UTF-8' while MySQL 5.1.x seems to not need it but it doesn’t hurt to have it for both versions. You have to edit ``etc/config.tdsl`` file and append this to the database connection string.

For MySQL 5.1.x, however, you need to also update code for all database stored procedures and functions used by the Tigase. They are updated for Tigase version 4.4.x and up, however if you use an older version of the Tigase server, you can reload stored procedures using the file from SVN.

Other MySQL Settings Worth Considering
''''''''''''''''''''''''''''''''''''''

There are a number of other useful options, especially for performance improvements. Please note, you will have to review them as some of them may impact data reliability and are useful for performance or load tests installations only.

.. code:: bash

   # InnoDB seems to be a better choice
   # so lets make it a default DB engine
   default-storage-engine = innodb

Some the general MySQL settings which mainly affect performance:

.. code:: bash

   key_buffer = 64M
   max_allowed_packet = 32M
   sort_buffer_size = 64M
   net_buffer_length = 64K
   read_buffer_size = 16M
   read_rnd_buffer_size = 16M
   thread_stack = 192K
   thread_cache_size = 8
   query_cache_limit = 10M
   query_cache_size = 64M

InnoDB specific settings:

.. code:: bash

   # Keep data in a separate file for each table
   innodb_file_per_table = 1
   # Allocate memory for data buffers
   innodb_buffer_pool_size = 1000M
   innodb_additional_mem_pool_size = 100M
   # A location of the MySQL database
   innodb_data_home_dir = /home/databases/mysql/
   innodb_log_group_home_dir = /home/databases/mysql/
   # The main thing here is the 'autoextend' property
   # without it your data file may reach maximum size and
   # no more records can be added to the table.
   innodb_data_file_path = ibdata1:10M:autoextend
   innodb_log_file_size = 10M
   innodb_log_buffer_size = 32M
   # Some other performance affecting settings
   innodb_flush_log_at_trx_commit = 2
   innodb_lock_wait_timeout = 50
   innodb_thread_concurrency = 16

These settings may not be fully optimized for your system, and have been only tested on our systems. If you have found better settings for your systems, feel free to `let us know <http://tigase.net/contact>`__.


Support for emoji and other icons

Tigase Database Schema can support emojis and other icons, however by using UTF-8 in ``mysqld`` settings will not allow this. To employ settings to support emojis and other icons, we recommend you use the following in your MySQL configuration file:

.. code:: properties

   [mysqld]
   character-set-server = utf8mb4
   collation-server = utf8mb4_bin
   character-set-client-handshake = FALSE

Doing this, Tigase XMPP Server Database will still use ``utf8`` character set, with ``utf8_general_ci`` as collation, and only fields which require support for emojis will be converted to ``utf8mb4``.

.. Note::

   If for some reason, with above settings applied to your MySQL instance, you still receive :literal:`java.sql.SQLException: Incorrect string value: ` you should add to your database URI passed in Tigase XMPP Server following configuration `&useUnicode=true&characterEncoding=UTF-8`. If even this fails too, then you may try adding ``&connectionCollation=utf8mb4_bin`` as a last resort. This changes situation from previous versions that shipped older MySQL JDBC connector.

.. Note::

   Tigase XMPP Server databases should be created with ``utf8_general_ci`` collation as it will work properly and is fastest from ``utf8mb4_general_ci`` collations supported by MySQL

Prepare the Derby Database for the Tigase Server
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

This guide describes how to prepare Derby database for connecting the Tigase server.

Basic Setup
''''''''''''
Preparation of Derby database is quite simple, but the following assumptions are made

-  ``DerbyDB`` - Derby database name

-  ``database/`` directory contains all necessary schema files

-  ``jars/`` and ``libs/`` directories contains Tigase and Derby binaries

General Approach

From the main Tigase directory execute following commands (Linux and Windows accordingly)

.. Note::

   You must use these sql files on order FIRST!

**Linux**

.. code:: sh

   java -Dij.protocol=jdbc:derby: -Dij.database="DerbyDB;create=true" -cp libs/derby.jar:libs/derbytools.jar:jars/tigase-server.jar org.apache.derby.tools.ij database/derby-common-0.0.1.sql

**Windows**

.. code:: sh

   java -Dij.protocol=jdbc:derby: -Dij.database="DerbyDB;create=true" -cp libs\derby.jar;libs\derbytools.jar;jars\tigase-server.jar org.apache.derby.tools.ij "database\derby-common-0.0.1.sql"

This will create Derby database named DerbyDB in the main Tigase directory and load common version for common v0.1.

You will need to repeat this process again in for following order:

.. code:: list

   derby-common-0.0.1.sql
   derby-common-0.0.2.sql
   derby-server-7.0.0.sql
   derby-server-7.1.0.sql
   derby-server-8.0.0.sql
   derby-muc-3.0.0.sql
   derby-pubsub-3.1.0.sql
   derby-pubsub-3.2.0.sql
   derby-pubsub-4.0.0.sql
   derby-http-api-2.0.0.sql

Other components may require installation such as:

.. code:: list

   derby-socks5-2.0.0.sql
   derby-push-1.0.0.sql
   derby-unified-archive-2.0.0.sql

Connecting Tigase to database
''''''''''''''''''''''''''''''

Once the database is setup, configure the ``config.tdsl`` file in Tigase and add the following configuration:

.. code:: properties

   dataSource {
       default () {
           uri = 'jdbc:derby:{location of derby database};'
       }
   }

Prepare the MS SQL Server Database for the Tigase Server
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

This guide describes how to prepare the MS SQL Server database for connecting the Tigase server to it.

It’s expected that a working installation of Microsoft SQL Server is present. The following guide will describe the necessary configurations required for using MS SQL Server with Tigase XMPP Server.

Preparing MS SQL Server Instance
'''''''''''''''''''''''''''''''''

After installation of MS SQL Server an instance needs to be configure to handle incoming JDBC connections. For that purpose it’s required to open *SQL Server Configuration Manager*. In the left-hand side panel navigate to *SQL Server Configuration Manager*, then *SQL Server Network Configuration → Protocols for ${INSTANCE_NAME}*. After selecting instance in the right-hand side panel select TCP/IP and open *Properties*, in the Protocol tab in General section select Yes for Enabled property. In the IP Addresses tab select Yes for Active and Enabled properties of all IP Addresses that you want MS SQL Server to handle. Subsequently set the TCP Port property (if missing) to the default value - 1433. A restart of the instance may be required afterwards.

Configuration using MS SQL Server Management Studio
''''''''''''''''''''''''''''''''''''''''''''''''''''

In order to prepare the database you can use either a wizard or execute queries directly in the Query Editor. Firstly you need to establish a connection to the MS SQL Server instance. From Object Explorer select Connect and in the Connect to Server dialog enter administrator credentials.

Using Wizards

-  Create Login

   In the left-hand side panel select Security → Logins and from context menu choose New Login, in the Wizard window enter desired Login name, select SQL Server authentication and enter desired password subsequently confirming action with OK

-  Create Database

   From the Object Explorer select Databases node and from context menu select New Database; in the Wizard window enter desired Database name and enter previously created Login name into Owner field; subsequently confirming action with OK.


Using Queries

From the Object Explorer root node’s context menu select New Query. In the Query windows execute following statements adjusting details to your liking:

.. code:: sql

   USE [master]
   GO

   CREATE DATABASE [tigasedb];
   GO

   CREATE LOGIN [tigase] WITH PASSWORD=N'tigase12', DEFAULT_DATABASE=[tigasedb]
   GO

   ALTER AUTHORIZATION ON DATABASE::tigasedb TO tigase;
   GO



Import Schema
''''''''''''''

From the File menu Select Open → File (or use Ctrl+O) and then open following files:

.. code:: list

   sqlserver-common-0.0.1.sql
   sqlserver-common-0.0.2.sql
   sqlserver-server-7.0.0.sql
   sqlserver-server-7.1.0.sql
   sqlserver-server-8.0.0.sql
   sqlserver-muc-3.0.0.sql
   sqlserver-pubsub-3.1.0.sql
   sqlserver-pubsub-3.2.0.sql
   sqlserver-pubsub-4.0.0.sql
   sqlserver-http-api-2.0.0.sql

.. Note::

   These files must be done sequentially! They are not linked, and so may need to be done one at a time.

Other components may require installation such as:

.. code:: list

   sqlserver-socks5-2.0.0.sql
   sqlserver-push-1.0.0.sql
   sqlserver-message-archiving-2.0.0.sql
   sqlserver-unified-archive-2.0.0.sql

Subsequently select created database from the list of Available Databases (Ctrl+U) available on the toolbar and execute each of the opened files in the order listed above.

Configuring from command line tool
'''''''''''''''''''''''''''''''''''

Creation of the database and import of schema can be done from command line as well. In order to do that, execute following commands from the directory where Tigase XMPP Server is installed otherwise paths to the schema need to be adjusted accordingly:

.. code:: bash

   sqlcmd -S %servername% -U %root_user% -P %root_pass% -Q "CREATE DATABASE [%database%]"
   sqlcmd -S %servername% -U %root_user% -P %root_pass% -Q "CREATE LOGIN [%user%] WITH PASSWORD=N'%password%', DEFAULT_DATABASE=[%database%]"
   sqlcmd -S %servername% -U %root_user% -P %root_pass% -d %database% -Q "ALTER AUTHORIZATION ON DATABASE::%database% TO %user%;"
   sqlcmd -S %servername% -U %root_user% -P %root_pass% -d %database% -i database\sqlserver-schema-7-1-schema.sql
   sqlcmd -S %servername% -U %root_user% -P %root_pass% -d %database% -i database\sqlserver-schema-7-1-sp.sql
   sqlcmd -S %servername% -U %root_user% -P %root_pass% -d %database% -i database\sqlserver-schema-7-1-props.sql
   sqlcmd -S %servername% -U %root_user% -P %root_pass% -d %database% -i database\sqlserver-pubsub-schema-3.2.0.sql

Above can be automatized with provided script %tigase-server%\scripts\db-create-sqlserver.cmd (note: it needs to be executed from main Tigase XMPP Server directory due to maintain correct paths):

.. code:: sh

   $ scripts\db-create-sqlserver.cmd %database_servername% %database_name% %tigase_username% %tigase_password% %root_username% %root_password%

If no parameters are provided then the following defaults are used:

.. code:: bash

   %database_servername%=localhost
   %database_name%=tigasedb
   %tigase_username%=tigase
   %tigase_password%=tigase12
   %root_username%=root
   %root_password%=root

Tigase configuration - config.tdsl
'''''''''''''''''''''''''''''''''''

Configuration of the MS SQL Server follows general database convention.

.. code:: bash

   dataSource {
       default () {
           uri = 'jdbc:[jtds:]sqlserver://db_hostname:port[;property=val]'
       }
   }

where any number of additional parameters can (and should) consist of:

-  ``databaseName`` - name of the database

-  ``user`` - username configured to access database

-  ``password`` - password for the above username

-  ``schema`` - name of the database schema

-  ``lastUpdateCount`` - 'false' value causes all update counts to be returned, including those returned by server triggers

Example:

.. code:: dsl

   dataSource {
       default () {
           uri = 'jdbc:sqlserver://hostname:1433;databaseName=tigasedb;user=tigase;password=tigase12;schema=dbo;lastUpdateCount=false'
       }
   }


JDBC: jTDS vs MS JDBC driver
'''''''''''''''''''''''''''''

Tigase XMPP Server supports two JDBC drivers intended to be used with Microsoft SQL Server - one created and provided by Microsoft itself and the alternative implementation - jTDS. Tigase is shipped with the latter in the distribution packages. Starting with the version 7.1.0 we recommend using jDTS driver that is shipped with Tigase as JDBC driver created by Microsoft can cause problems with some components in cluster installations. MS driver can be downloaded form the website: `JDBC Drivers 4.0, 4.1 for SQL Server <http://www.microsoft.com/en-us/download/details.aspx?displaylang=en&id=11774>`__ then unpack the archive. Copy sqljdbc_4.0/enu/sqljdbc4.jar file to ${tigase-server}/jars directory.

Depending on the driver used ``uri`` needs to be configured accordingly.

-  Microsoft driver:

   .. code:: dsl

      dataSource {
          default () {
              uri = 'jdbc:sqlserver://...'
          }
      }

-  jDTS driver

   .. code:: bash

      dataSource {
          default () {
              uri = 'jdbc:jdts://...'
          }
      }

Prepare the PostgreSQL Database for the Tigase Server
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

This guide describes how to prepare PostgreSQL database for connecting to Tigase server.

The PostgreSQL database can be prepared in many ways. Below are presented two possible ways. The following assumptions apply to both methods:

-  ``admin_db_user`` - database user with admin rights

-  ``tigase_user`` - database user for Tigase

-  ``tigasedb`` - database for Tigase

Configuring from PostgreSQL Command Line Tool
''''''''''''''''''''''''''''''''''''''''''''''

Run the PostgreSQL command line client and enter following instructions:

Add the ``tigase_user``:

.. code:: sql

   psql=# create role tigase_user with login password 'tigase123';

Next, Create the database for the Tigase server with ``tigase_user`` as owner of database:

.. code:: sql

   psql=# create database tigasedb owner tigase_user;

Schema Installation

Load database schema to initialize the Tigase server from the file that corresponds to the version of Tigase you want to use. First you need to switch to ``tigasedb``.

.. code:: sql

   psql=# \connect tigasedb

Begin by applying the basic Schema

.. code:: sql

   psql=# \i database/postgresql-common-0.0.1.sql

Continue by adding the schema files listed below:

.. code:: list

   postgresql-common-0.0.1.sql
   postgresql-common-0.0.2.sql
   postgresql-server-7.0.0.sql
   postgresql-server-7.1.0.sql
   postgresql-server-8.0.0.sql
   postgresql-muc-3.0.0.sql
   postgresql-pubsub-3.1.0.sql
   postgresql-pubsub-3.2.0.sql
   postgresql-pubsub-4.0.0.sql
   postgresql-http-api-2.0.0.sql

Other components may require installation such as:

.. code:: list

   postgresql-socks5-2.0.0.sql
   postgresql-push-1.0.0.sql
   postgresql-message-archiving-2.0.0.sql
   postgresql-unified-archive-2.0.0.sql

Configuring From the Linux Shell Command Line
''''''''''''''''''''''''''''''''''''''''''''''

Follow steps below to prepare the PostgreSQL database:

First, add the ``tigase_user``:

.. code:: sql

   createuser -U admin_db_user -W -D -R -S -P tigase_user

You will be asked for credentials for admin_db_user and password for new database user.

Create the database for the Tigase server with tigase_user as owner of database:

.. code:: sql

   createdb -U admin_db_user -W -O tigase_user tigasedb

Database Schema Installation

Load database schema to initialize the Tigase server

.. code:: sql

   psql -q -U tigase_user -W tigasedb -f database/postgresql-common-0.0.1.sql
   psql -q -U tigase_user -W tigasedb -f database/postgresql-common-0.0.2.sql
   etc..

Continue by adding the schema files listed below:

.. code:: list

   postgresql-common-0.0.1.sql
   postgresql-common-0.0.2.sql
   postgresql-server-7.0.0.sql
   postgresql-server-7.1.0.sql
   postgresql-server-8.0.0.sql
   postgresql-muc-3.0.0.sql
   postgresql-pubsub-3.1.0.sql
   postgresql-pubsub-3.2.0.sql
   postgresql-pubsub-4.0.0.sql
   postgresql-http-api-2.0.0.sql

Other components may require installation such as:

.. code:: list

   postgresql-socks5-2.0.0.sql
   postgresql-push-1.0.0.sql
   postgresql-message-archiving-2.0.0.sql
   postgresql-unified-archive-2.0.0.sql

.. Note::

   The above commands should be executed from the main Tigase directory. The initialization schema file should be also available locally in database/ directory of your Tigase installation.

Preparing Tigase for MongoDB
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Tigase now supports MongoDB for auth, settings, and storage repositories. If you wish to use MongoDB for Tigase, please use this guide to help you.

Dependencies
''''''''''''

To run Tigase MongoDB support library requires drivers for MongoDB for Java which can be downloaded from `here <https://github.com/mongodb/mongo-java-driver/releases>`__. This driver needs to be placed in ``jars/`` directory located in Tigase XMPP Server installation directory. If you are using a dist-max distribution, it is already included.

Configuration
''''''''''''''

Note that fresh installations of MongoDB do not come with users or databases installed. Once you have setup MongoDB you will need to create a user to be used with Tigase. To do this, bring up the mongo console by running mongo.exe in a cmd window for windows, or run mongo in linux. Once connected, enter then following:

.. code:: bash

   use admin
   db.createUser( { user: "tigase",
                    pwd: "password",
                    customData: { employeeId: 12345 },
                    roles: [ "root" ]
                   }
                 )

Be sure to give this user a ``root`` role in order to properly write to the database. Once you receive a ``user successfully created`` message, you are ready to install tigase on MongoDB.

Configuration of user repository for Tigase XMPP Server

To configure Tigase XMPP Server to use MongoDB you need to set ``dataSource`` in etc/config.tdsl file to proper MongoDB URI pointing to which MongoDB database should be used (it will be created by MongoDB if it does not exist). ``userRepository`` property should not be set to let Tigase XMPP Server auto-detect proper implementation of ``UserRepository``. Tigase XMPP Server will create proper collections in MongoDB if they do not exist so no schema files are necessary.

Example configuration of XMPP Server pointing to MongoDB database ``tigase_test`` in a local instance:

.. code:: dsl

   dataSource {
       default () {
           uri = 'mongodb://user:pass@localhost/tigase_test'
       }
   }
   userRepository {
       default () {}
   }
   authRepository {
       default () {}
   }

If Tigase Server is not able to detect a proper storage layer implementation, it can be forced to use one provided by Tigase using the following lines in ``etc/config.tdsl`` file:

.. code:: dsl

   userRepository {
       default () {
           cls = 'tigase.mongodb.MongoRepository'
       }
   }
   authRepository {
       default () {
           cls = 'tigase.mongodb.MongoRepository'
       }
   }

Every component should be able to use proper implementation to support MongoDB using this URI. Also MongoDB URI can be passed as any URI in configuration of any component.

Configuration for MUC

By default, MUC component will use MongoDB to store data if Tigase is configured to use it as a default store. However, if you would like to use a different MongoDB database to store MUC message archive, you can do this by adding the following lines to ``etc/config.tdsl`` file:

.. code:: dsl

   muc {
       'history-db-uri' = 'mongodb://user:pass@localhost/tigase_test'
   }

If MUC components fails to detect and use a proper storage layer for MongoDB, you can force it to use one provided by Tigase by using the following line in the ``config.tdsl`` file:

.. code:: dsl

   muc {
       'history-db' = 'tigase.mongodb.muc.MongoHistoryProvider'
   }


Configuration for PubSub

By default, PubSub component will use MongoDB to store data if Tigase is configured to use it as a default store. However, if you would like to use a different MongoDB database to store PubSub component data, you can do this by adding the following lines to ``etc/config.tdsl`` file:

.. code:: dsl

   pubsub {
       'pubsub-repo-url' = 'mongodb://user:pass@localhost/tigase_test'
   }

If the PubSub components fails to detect and use a proper storage layer for MongoDB, you can force it to use one provided by Tigase by using the following line in the ``config.tdsl`` file:

.. code:: dsl

   pubsub {
       'pubsub-repo-class' = 'tigase.mongodb.pubsub.PubSubDAOMongo'
   }


Configuration for Message Archiving

By default, the Message Archiving component will use MongoDB to store data if Tigase is configured to use it as a default store. However, if you would like to use a different MongoDB database to store message archives, you can do this by adding the following lines to ``etc/config.tdsl`` file:

.. code:: dsl

   'message-archive' {
       'archive-repo-uri' = 'mongodb://user:pass@localhost/tigase_test'
   }

If Message Archiving component fails to detect and use a proper storage layer for MongoDB, you can force it to use one provided by Tigase by using the following line in the ``config.tdsl`` file:

.. code:: dsl

   'message-archive' {
       'archive-repo-class' = 'tigase.mongodb.archive.MongoMessageArchiveRepository'
   }


Schema Description
'''''''''''''''''''

This description contains only basic description of schema and only basic part of it. More collections may be created if additional components of Tigase XMPP Server are loaded and configured to use MongoDB.

Tigase XMPP Server Schema
-------------------------

Basic schema for UserRespository and AuthRepository consists of two collections: . tig_users - contains list of users . tig_nodes - contains data related to users in tree-like way

``tig_users`` collection contains the following fields:

.. table:: Table 9. tig_users

   +----------+--------------------------------------------------------------------+
   | Name     | Description                                                        |
   +==========+====================================================================+
   | \_id     | id of user which is SHA256 hash of users jid (raw byte array).     |
   +----------+--------------------------------------------------------------------+
   | user_id  | contains full user jid.                                            |
   +----------+--------------------------------------------------------------------+
   | domain   | domain to which user belongs for easier lookup of users by domain. |
   +----------+--------------------------------------------------------------------+
   | password | password of user (will be removed after upgrade to 8.0.0).         |
   +----------+--------------------------------------------------------------------+

``tig_nodes`` collection contains the following fields

.. table:: Table 10. tig_nodes

   +-------+--------------------------------------------------------------------------+
   | Name  | Description                                                              |
   +=======+==========================================================================+
   | \_id  | id of row auto-generated by MongoDB.                                     |
   +-------+--------------------------------------------------------------------------+
   | uid   | id of user which is SHA256 hash of users jid (raw byte array).           |
   +-------+--------------------------------------------------------------------------+
   | node  | full path of node in tree-like structure separated by / (may not exist). |
   +-------+--------------------------------------------------------------------------+
   | key   | key for which value for node is set.                                     |
   +-------+--------------------------------------------------------------------------+
   | value | value which is set for node key.                                         |
   +-------+--------------------------------------------------------------------------+

Tigase XMPP Server also uses additional collections for storage of Offline Messages

.. table:: Table 11. msg_history collection

   +-----------+-----------------------------------------------------------------------------+
   | Name      | Description                                                                 |
   +===========+=============================================================================+
   | from      | full user jid of message sender.                                            |
   +-----------+-----------------------------------------------------------------------------+
   | from_hash | SHA256 hash of message sender jid as raw byte array.                        |
   +-----------+-----------------------------------------------------------------------------+
   | to        | full users jid of message recipient.                                        |
   +-----------+-----------------------------------------------------------------------------+
   | to_hash   | SHA256 hash of message recipient full jid as raw byte array.                |
   +-----------+-----------------------------------------------------------------------------+
   | ts        | timestamp of message as date.                                               |
   +-----------+-----------------------------------------------------------------------------+
   | message   | serialized XML stanza containing message.                                   |
   +-----------+-----------------------------------------------------------------------------+
   | expire-at | timestamp of expiration of message (if message contains AMP expire-at set). |
   +-----------+-----------------------------------------------------------------------------+

Due to changes in authentication and credentials storage in AuthRepository, we moved ``password`` field from ``tig_users`` collection to a newly created collection called ``tig_user_credentials``.

This new collection has following fields:

+----------------+----------------------------------------------------------------------------------+
| Name           | Description                                                                      |
+================+==================================================================================+
| \_id           | id of document automatically generated by MongoDB                                |
+----------------+----------------------------------------------------------------------------------+
| uid            | SHA256 hash of a user for which credentails are stored                           |
+----------------+----------------------------------------------------------------------------------+
| username       | username provided during authentication (or ``default``)                         |
+----------------+----------------------------------------------------------------------------------+
| account_status | name of an account state (copy of value stored in user document from`tig_users`) |
+----------------+----------------------------------------------------------------------------------+

Additionally for each mechanism we store separate field in this object, so for:

-  ``PLAIN`` we have ``PLAIN`` field with value for this mechanism

-  ``SCRAM-SHA-1`` we have ``SCRAM-SHA-1`` field with value for this mechanism

-  etc…​

Upgrade is not done in one step, and rather will be done once a particular user will log in. During authentication if there is no data in ``tig_user_credentials``, Tigase XMPP Server will check if ``password`` field in ``tig_user`` exists. If it does, and it is filled credentials will be migrated to the new collection.

2.8.6. Hashed User Passwords in Database
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. Warning::

   This feature is still available, but passwords are stored encrypted by default since v8.0.0. We do not recommend using these settings.

By default, user passwords are stored in plain-text in the Tigase’s database. However, there is an easy way to have them encoded in either one of already supported ways or to even add a new encoding algorithm on your own.

Storing passwords in hashed format in the database makes it possible to avoid using a plain-text password authentication mechanism. You cannot have hashed passwords in the database and non-plain-text password authentication. On the other hand, the connection between the server and the client is almost always secured by SSL/TLS so the plain-text password authentication method is perhaps less of a problem than storing plain-text passwords in the database.

Nevertheless, it is simple enough to adjust this in Tigase’s database.

Shortcut
~~~~~~~~

Connect to your database from a command line and execute following statement for MySQL database:

.. code:: sql

   call TigPutDBProperty('password-encoding', 'encoding-mode');

Where encoding mode is one of the following:

-  ``MD5-PASSWORD`` the database stores MD5 hash code from the user’s password.

-  ``MD5-USERID-PASSWORD`` the database stores MD5 hash code from concatenated user’s bare JID and password.

-  ``MD5-USERNAME-PASSWORD`` the database stores MD5 hash code from concatenated user’s name (localpart) and password.

For example:

.. code:: sql

   call TigPutDBProperty('password-encoding', 'MD5-PASSWORD');

Full Route
~~~~~~~~~~~

The way passwords are stored in the DB is controlled by Tigase database schema property. Properties in the database schema can be set by a stored procedure called: ``TigPutDBProperty(key, value)``. Properties from the DB schema can be retrieved using another stored function called: ``TigGetDBProperty(key)``.

The simplest way to call them is via command-line interface to the database.

For the purpose of this guide let’s say we have a MySQL database and a test account: ``test@example.com`` with password ``test77``.

By default, most of DB actions for Tigase, are performed using stored procedures including user authentication. So, the first thing to do is to make sure the stored procedures are working correctly.

Create a Test User Account
'''''''''''''''''''''''''''

To add a new user account we use a stored procedure: ``TigAddUserPlainPw(bareJid, password)``. As you can see there is this strange appendix to the procedure name: ``PlainPw``. This procedure accepts plain passwords regardless how it is stored in the database. So it is safe and easy to use either for plain-text passwords or hashed in the DB. There are also versions of procedures without this appendix but they are sensitive on the data format and always have to pass password in the exact format it is stored in the database.

So, let’s add a new user account:

.. code:: sql

   call TigAddUserPlainPw('test@example.com', 'test77');

If the result was 'Query OK', then it means the user account has been successfully created.

Test User Authentication
'''''''''''''''''''''''''

We can now test user authentication:

.. code:: sql

   call TigUserLoginPlainPw('test@example.com', 'test77');

If authentication was successful the result looks like this:

.. code:: sql

   +--------------------+
   | user_id            |
   +--------------------+
   | 'test@example.com' |
   +--------------------+
   1 row in set (0.01 sec)

   Query OK, 0 rows affected (0.01 sec)

If authentication was unsuccessful, the result looks like this:

.. code:: sql

   +---------+
   | user_id |
   +---------+
   |    NULL |
   +---------+
   1 row in set (0.01 sec)

   Query OK, 0 rows affected (0.01 sec)

Password Encoding Check
''''''''''''''''''''''''

``TigGetDBProperty`` is a function, not a procedure in MySQL database so we have to use select to call it:

.. code:: sql

   select TigGetDBProperty('password-encoding');

Most likely output is this:

.. code:: sql

   +---------------------------------------+
   | TigGetDBProperty('password-encoding') |
   +---------------------------------------+
   | NULL                                  |
   +---------------------------------------+
   1 row in set, 1 warning (0.00 sec)

Which means a default password encoding is used, in plain-text and thus no encoding. And we can actually check this in the database directly:

.. code:: sql

   select uid, user_id, user_pw from tig_users where user_id = 'test@example.com';

And expected result with plain-text password format would be:

.. code:: sql

   +-----+--------------------+---------+
   | uid | user_id            | user_pw |
   +-----+--------------------+---------+
   |  41 | 'test@example.com' | test77  |
   +-----+--------------------+---------+
   1 row in set (0.00 sec)

Password Encoding Change
'''''''''''''''''''''''''

Now let’s set password encoding to MD5 hash:

.. code:: sql

   call TigPutDBProperty('password-encoding', 'MD5-PASSWORD');

'Query OK', means the password encoding has been successfully changed. Of course we changed the property only. All the existing passwords in the database are still in plain-text format. Therefore we expect that attempt to authenticate the user would fail:

.. code:: sql

   call TigUserLoginPlainPw('test@example.com', 'test777');
   +---------+
   | user_id |
   +---------+
   |    NULL |
   +---------+
   1 row in set (0.00 sec)

   Query OK, 0 rows affected (0.00 sec)

We can fix this by updating the user’s password in the database:

.. code:: sql

   call TigUpdatePasswordPlainPw('test@example.com', 'test777');
   Query OK, 1 row affected (0.01 sec)

   mysql> call TigUserLoginPlainPw('test@example.com', 'test777');
   +--------------------+
   | user_id            |
   +--------------------+
   | 'test@example.com' |
   +--------------------+
   1 row in set (0.00 sec)

   Query OK, 0 rows affected (0.00 sec)

2.8.7. Tigase Server and Multiple Databases
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Splitting user authentication data from all other XMPP information such as roster, vcards, etc…​ was almost always possible in Tigase XMPP Server. Possible and quite simple thing to configure. Also it has been always possible and easy to assign a different database for each Tigase component (MUC, PubSub, AMP), for recording the server statistics. Almost every data type or component can store information in a different location, simple and easy to setup through the configuration file.

However it is much less known that it is also possible to have a different database for each virtual domain. This applies to both the user repository and authentication repository. This allows for very interesting configuration such as user database sharing where each shard keeps users for a specific domain, or physically split data based on virtual domain if each domain refers to a different customer or group of people.

How can we do that then?

This is very easy to do through the Tigase’s configuration file.

.. code:: dsl

   dataSource {
       default () {
           uri = 'jdbc:mysql://db2.tigase/dbname?user&password'
       }
       'default-auth' () {
           uri = 'jdbc:mysql://db1.tigase/dbname?user&password'
       }
   }
   userRepository {
       default () {}
   }
   authRepository {
       default () {
           cls = 'tigase.db.jdbc.TigaseCustomAuth'
           'data-source' = 'default-auth'
       }
   }

This configuration defines just a default databases for both user repository and authentication repository. Default means it is used when there is no repository specified for a particular virtual domain. However, you can have a separate, both user and authentication repository for each virtual domain.

Here is, how it works:

First, let’s define our default database for all VHosts

.. code:: dsl

   dataSource {
       default () {
           uri = 'jdbc:mysql://db2.tigase/dbname?user&password'
       }
       'default-auth' () {
           uri = 'jdbc:mysql://db1.tigase/dbname?user&password'
       }
   }
   userRepository {
       default () {}
   }
   authRepository {
       default () {
           cls = 'tigase.db.jdbc.TigaseCustomAuth'
           'data-source' = 'default-auth'
       }
   }

Now, we have VHost: domain1.com User authentication data for this VHost is stored in Drupal database

.. code:: dsl

   dataSource {
     'domain1.com-auth' () {
       uri = jdbc:mysql://db7.tigase/dbname?user&password'
     }
   }
   authRepository {
     domain1.com () {
       cls = 'tigase/db/jdbc.TigaseCustomAuth'
       'data-source' = 'domain1.com-auth'
     }
   }

All other user data is stored in Tigase’s standard database in MySQL

.. code:: dsl

   dataSource {
     'domain1.com' () {
       uri = jdbc:mysql://db4.tigase/dbname?user&password'
     }
   }
   userRepository {
     domain1.com () {}
   }

Next VHost: domain2.com User authentication is in LDAP server but all other user data is stored in Tigase’s standard database

.. code:: dsl

   authRepository {
       domain2.com () {
           cls = 'tigase.db.ldap.LdapAuthProvider'
           uri = 'ldap://ldap.domain2.com:389'
           'data-source' = 'default'
       }
   }

Now is something new, we have a custom authentication repository and separate user settings for a single domain. Please note how we define the VHost for which we set custom parameters

.. code:: dsl

   authRepository {
       domain2.com {
           'user-dn-pattern' = 'cn=,ou=,dc=,dc='
       }
   }

All other user data is stored in the same as default repository

.. code:: dsl

   userRepository {
       domain2.com () {}
   }
   dataSource {
       domain2.com () {
           uri = 'jdbc:mysql://db2.tigase/dbname?user&password'
       }
   }

When combined, the DSL output should look like this:

.. code:: dsl

   dataSource {
       domain2.com () {
           uri = 'jdbc:mysql://db2.tigase/dbname?user&password'
       }
   }
   userRepository {
       domain2.com () {}
   }
   authRepository {
       domain2.com () {
           cls = 'tigase.db.ldap.LdapAuthProvider'
           uri = 'ldap://ldap.domain2.com:389'
           'user-dn-pattern' = 'cn=,ou=,dc=,dc='
       }
   }

Next VHost: domain3.com Again user authentication is in LDAP server but pointing to a different LDAP server with different access credentials and parameters. User information is stored in a postgreSQL database.

.. code:: dsl

   dataSource {
       domain3.com () {
           uri = 'jdbc:pgsql://db.domain3.com/dbname?user&password'
       }
   }
   userRepository {
       domain3.com () {}
   }
   authRepository {
       domain3.com () {
           cls = 'tigase.db.ldap.LdapAuthProvider'
           uri = 'ldap://ldap.domain3.com:389'
           'user-dn-pattern' = 'cn=,ou=,dc=,dc='
       }
   }

For VHost: domain4.com all the data, both authentication and user XMPP data are stored on a separate MySQL server with custom stored procedures for both user login and user logout processing.

.. code:: dsl

   dataSource {
       domain4.com () {
           uri = 'jdbc:mysql://db14.domain4.com/dbname?user&password'
       }
   }
   userRepository {
       domain4.com () {}
   }
   authRepository {
       domain4.com () {
           cls = 'tigase.db.jdbc.TigaseCustomAuth'
           'user-login-query' = '{ call UserLogin(?, ?) }'
           'user-logout-query' = '{ call UserLogout(?) }'
           'sasl-mechs' = [ 'PLAIN', 'DIGEST-MD5' ]
       }
   }

As you can see, it requires some writing but flexibility is very extensive and you can setup as many separate databases as you need or want. If one database (recognized by the database connection string) is shared among different VHosts, Tigase still uses a single connection pool, so it won’t create an excessive number of connections to the database.

2.8.8. Importing User Data
^^^^^^^^^^^^^^^^^^^^^^^^^^^

You can easily copy data between Tigase compatible repositories that is repositories for which there is a database connector. However, it is not that easy to import data from an external source. Therefore a simple data import functionality has been added to repository utilities package.

You can access repository utilities through command ``./bin/repo.sh`` or ``./scripts/repo.sh`` depending on whether you use a binary package or source distribution.

``-h`` parameter gives you a list of all possible parameters:

.. code:: sh

   ./scripts/repo.sh -h

   Parameters:
    -h          this help message
    -sc class   source repository class name
    -su uri     source repository init string
    -dc class   destination repository class name
    -du uri     destination repository init string
    -dt string  data content to set/remove in repository
    -u user     user ID, if given all operations are only for that ID
                if you want to add user to AuthRepository parameter must
                in form: "user:password"
    -st         perform simple test on repository
    -at         simple test for adding and removing user
    -cp         copy content from source to destination repository
    -pr         print content of the repository
    -n          data content string is a node string
    -kv         data content string is node/key=value string
    -add        add data content to repository
    -del        delete data content from repository
    ------------
    -roster     check the user roster
    -aeg [true|false]  Allow empty group list for the contact
    -import file  import user data from the file of following format:
            user_jid, password, roser_jid, roster_nick, subscription, group



   Note! If you put UserAuthRepository implementation as a class name
         some operation are not allowed and will be silently skipped.
         Have a look at UserAuthRepository to see what operations are
         possible or what operation does make sense.
         Alternatively look for admin tools guide on web site.

The most critical parameters are the source repository class name and the initialization string. Therefore there are a few example preset parameters which you can use and adjust for your system. If you look inside the ``repo.sh`` script you can find at the end of the script following lines:

.. code:: sh

   XML_REP="-sc tigase.db.xml.XMLRepository -su ../testsuite/user-repository.xml_200k_backup"
   MYSQL_REP="-sc tigase.db.jdbc.JDBCRepository -su jdbc:mysql://localhost/tigase?user=root&password=mypass"
   PGSQL_REP="-sc tigase.db.jdbc.JDBCRepository -su jdbc:postgresql://localhost/tigase?user=tigase"

   java $D -cp $CP tigase.util.RepositoryUtils $MYSQL_REP $*

You can see that the source repository has been set to MySQL database with ``tigase`` as the database name, ``root`` the database user and ``mypass`` the user password.

You can adjust these settings for your system.

Now to import data to your repository simply execute the command:

.. code:: sh

   ./bin/repo.sh -import import-file.txt

*Note, the import function is available from* **b895**

The format of the import file is very simple. This is a flat file with comma separated values:

.. code:: bash

   jid,password,roster_jid,roster_nick,subscriptio,group

To create such a file from MySQL database you will have to execute a command like this one:

.. code:: sql

   SELECT a, b, c, d INTO OUTFILE 'import-file.txt'
   FIELDS TERMINATED BY ','
   LINES TERMINATED BY '\n'
   FROM test_table;

2.8.9. Importing Existing Data
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Information about importing user data from other databases.

Connecting the Tigase Server to MySQL Database
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Please before continuing reading of this manual have a look at the `initial MySQL database setup <#prepareMysql>`__. It will help you with database preparation for connecting with Tigase server.

This guide describes MySQL database connection parameters.

This guide is actually very short as there are example configuration files which can be used and customized for your environment.

.. code:: dsl

   dataSource {
       default () {
           uri = 'jdbc:mysql://localhost/tigasedb?user=tigase_user&password=mypass'
       }
   }
   userRepository {
       default () {}
   }
   authRepository {
       default () {}
   }

This is the basic setup for setting up an SQL repository for Tigase. dataSource contains the uri for ``default`` which is the mysql database. MySQL connector requires connection string in the following format: ``jdbc:mysql://[hostname]/[database name]?user=[user name]&password=[user password]``

Edit the ``config.tdsl`` file for your environment.

Start the server using following command:

.. code:: sh

   ./scripts/tigase.sh start etc/tigase.conf

Integrating Tigase Server with Drupal
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

First of all, Tigase can authenticate users against a Drupal database which means you have the same user account for both Drupal website and the XMPP server. Moreover in such a configuration all account management is done via Drupal web interface like account creation, password change update user details and so on. Administrator can temporarily disable user account and this is followed by Tigase server too.

Connecting to Drupal Database
''''''''''''''''''''''''''''''

The best way to setup Tigase with Drupal database is via the ``config.tdsl`` file where you can put initial setting for Tigase configuration.

If you look in ``etc/`` directory of your Tigase installation you should find a the file there.

All you need to connect to Drupal database is set the following:

.. code:: dsl

   dataSource {
       'default-auth' () {
           uri = 'jdbc:mysql://localhost/drupal?user=drupalusr&password=drupalpass'
       }
   }
   authRepository {
       default () {
           cls = 'tigase.db.jdbc.DrupalWPAuth'
           'data-source' = 'default-auth'
       }
   }

Typically, you will need to have drupal for authentication, and another for user repository. In this case, we will use SQL for user DB.

.. code:: dsl

   dataSource {
       default () {
           uri = 'jdbc:mysql://localhost/tigasedb?user=tigase_user&password=mypass'
       }
       'default-auth' () {
           uri = 'jdbc:mysql://localhost/drupal?user=drupalusr&password=drupalpass'
       }
   }
   userRepository {
       default () {}
   }
   authRepository {
       default () {
           cls = 'tigase.db.jdbc.DrupalWPAuth'
           'data-source' = 'default-auth'
       }
   }

In theory you can load Tigase database schema to Drupal database and then both ``db-uris`` would have the same database connection string. More details about setting up and connecting to MySQL database can be found in the `MySQL guide <#prepareMysql>`__.

Now run the Tigase server.

.. code:: sh

   ./scripts/tigase.sh start etc/tigase.conf

Now you can register an account on your Drupal website and connect with an XMPP client using the account details.

.. Note::

   You have to enable plain password authentication in your XMPP client to connect to Tigase server with Drupal database.

PostgreSQL Database Use
~~~~~~~~~~~~~~~~~~~~~~~

This guide describes how to configure Tigase server to use `PostgreSQL <http://www.postgresql.org/>`__ database as a user repository.

If you used an XML based user repository before you can copy all user data to PostgreSQL database using repository management tool. All steps are described below.

PostgreSQL Database Preparation
''''''''''''''''''''''''''''''''

Create new database user account which will be used to connect to your database:

.. code:: sh

   # createuser
   Enter name of user to add: tigase
   Shall the new user be allowed to create databases? (y/n) y
   Shall the new user be allowed to create more new users? (y/n) y

Now using new database user account create database for your service:

.. code:: sh

   # createdb -U tigase tigasedb
   CREATE DATABASE

Now you can load the database schema:

.. code:: sh

   # psql -U tigase -d tigasedb -f postgresql-schema.sql

Now the database is ready for Tigase server to use.

Server Configuration
'''''''''''''''''''''

Server configuration is almost identical to MySQL database setup. The only difference is the connection string which usually looks like:

.. code:: dsl

   dataSource {
       default () {
           uri = 'postgresql://localhost/tigasdb?user=tigase'
       }
   }

2.8.10. Schema Updates
^^^^^^^^^^^^^^^^^^^^^^

This is a repository for Schema updates in case you have to upgrade from older installations.

-  `Tigase Server Schema v7.1 Updates <#tigaseServer71>`__ Applies to v7.1.0 and v8.0.0

Changes to Schema in v8.0.0
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

For version 8.0.0 of Tigase XMPP Server, we decided to improve authentication and security that was provided. In order to do this, implementation of repository and database schemas needed to be changed to achieve this goal. This document, as well one in the HTTP API, will describe the changes to the schemas in this new version.

Reasons
''''''''

Before version 8.0.0, user passwords were stored in plaintext in ``user_pw`` database field within ``tig_users`` table, but in plaintext. It was possible to enable storage of the MD5 hash of the password instead, however this limited authentication mechanism SASL PLAIN only. However an MD5 hash of a password is not really a secure method as it is possible to revert this mechanism using rainbow tables.

Therefore, we decided to change this and store only encrypted versions of a password in ``PBKDF2`` form which can be easily used for ``SCRAM-SHA-1`` authentication mechanism or ``SCRAM-SHA-256``. SASL PLAIN mechanism can also used these encrypted passwords. The storage of encrypted passwords is now enabled **by default** in v8.0.0 of Tigase.

Summary of changes
'''''''''''''''''''

Added support for storage of encrypted password

Passwords are no longer stored in plaintext on any database.

Using same salt for any subsequent authentications

This allows clients to reuse calculated credentials and keep them instead of storing plaintext passwords.

Disabled usage of stored procedure for authentication

In previous versions, Tigase used stored procedures ``TigUserLoginPlainPw`` and ``TigUserLogin`` for SASL PLAIN authentication. From version 8.0.0, those procedures are no longer used, but they are updated to use passwords stored in ``tig_user_credentials`` table.

It is still possible to use this procedures for authentication, but to do that you need add:

.. code:: tdsl

   'user-login-query' = '{ call TigUserLoginPlainPw(?, ?) }'

to configuration block of **every** authentication repository.

To enable this for default repository, the ``authRepository`` configuration block will look like this:

.. code:: tdsl

   authRepository () {
       default () {
           'user-login-query' = '{ call TigUserLoginPlainPw(?, ?) }'
       }
   }


Deprecated API

Some methods of ``AuthRepository`` API were deprecated and should not be used. Most of them were used for authentication using stored procedures, retrieval of password in plaintext or for password change.

For most of these methods, new versions based on ``tig_user_credentials`` table and user credentials storage are provided where possible.

Deprecated storage procedures

Stored procedures for authentication and password manipulation were updated to a new form, so that will be possible to use them by older versions of Tigase XMPP Server during rolling updates of a cluster. However, these procedures will not be used any more and will be depreciated and removed in future versions of Tigase XMPP Server.

Usage of MD5 hashes of passwords

If you have changed ``password-encoding`` database property in previous versions of Tigase XMPP Server, then you will need to modify your configuration to keep it working. If you wish only to allow access using old passwords and to store changed passwords in the new form, then you need to enable credentials decoder for the correct authentication repository. In this example we will provided changes required for ``MD5-PASSWORD`` value of ``password-encoding`` database property. If you have used a different one, then just replace ``MD5-PASSWORD`` with ``MD5-USERNAME-PASSWORD`` or ``MD5-USERID-PASSWORD``.

**Usage of MD5 decoder.**

.. code:: tdsl

   authRepository () {
       default () {
           credentialDecoders () {
               'MD5-PASSWORD' () {}
           }
       }
   }

If you wish to store passwords in MD5 form then use following entries in your configuration file:

**Usage of MD5 encoder.**

.. code:: tdsl

   authRepository () {
       default () {
           credentialEncoders () {
               'MD5-PASSWORD' () {}
           }
       }
   }


Enabling and disabling credentials encoders/decoders

You may enable which encoders and decoders used on your installation. By enabling encoders/decoders you are deciding in what form the password is stored in the database. Those changes may impact which SASL mechanisms may be allowed to use on your installation.

**Enabling PLAIN decoder.**

.. code:: tdsl

   authRepository () {
       default () {
           credentialDecoders () {
               'PLAIN' () {}
           }
       }
   }

**Disabling SCRAM-SHA-1 encoder.**

.. code:: tdsl

   authRepository () {
       default () {
           credentialEncoders () {
               'SCRAM-SHA-1' (active: false) {}
               'SCRAM-SHA-256' (active: false) {}
           }
       }
   }

.. Warning::

    It is strongly recommended not to disable encoders if you have enabled decoder of the same type as it may lead to the authentication issues, if client tries to use a mechanism which that is not available.

Schema changes

This change resulted in a creation of the new table ``tig_user_credentials`` with following fields:

**uid**
   id of a user row in ``tig_users``.

**username**
   username used for authentication (if ``authzid`` is not provided or ``authzid`` localpart is equal to ``authcid`` then row with ``default`` value will be used).

**mechanism**
   name of mechanism for which this credentials will be used, ie. ``SCRAM-SHA-1`` or ``PLAIN``.

**value**
   serialized value required for mechanism to confirm that credentials match.

.. Warning::

    During execution of ``upgrade-schema`` task, passwords will be removed from ``tig_users`` table from ``user_pw`` field and moved to ``tig_user_credentials`` table.

Added password reset mechanism

As a part of Tigase HTTP API component and Tigase Extras, we developed a mechanism which allows user to reset their password. To use this mechanism HTTP API component and its REST module **must** to be enabled on Tigase XMPP Server installation.

.. Note::

   Additionally this mechanism need to be enabled in the configuration file. For more information about configuration of this mechanism please check Tigase HTTP API component documentation.

Assuming that HTTP API component is configured to run on port 8080 *(default)*, then after accessing address http://localhost:8080/rest/user/resetPassword in the web browser it will present a web form. By filling and submitting this form, the user will initiate a password reset process. During this process, Tigase XMPP Server will send an email to the user’s email address (provided during registration) with a link to the password change form.


Upgrading from v7.1.x
~~~~~~~~~~~~~~~~~~~~~~

When upgrading from previous versions of Tigase, it is recommended that you first backup the database. Refer to the documentation of your database software to find out how to export a copy. Once the backup is made, it will be time to run the schema upgrade. Be sure that your schema is up to date, and should be v7.1.0 Schema.

To upgrade, use the new ``upgrade-schema`` task of SchemaManager:

-  In linux

   .. code:: bash

      ./scripts/tigase.sh install-schema etc/tigase.conf

-  In Windows

   .. code:: bash

      java -cp "jars/*" tigase.db.util.SchemaManager "install-schema"

You will need to configure the following switches:

-  | ``-T`` Specifies Database Type
   | Possible values are: ``mysql``, ``derby``, ``sqlserver``, ``postgresql``, ``mongodb``

-  | ``-D`` Specifies Databse Name
   | The explicit name of the database you wish to upgrade.

-  | ``-H`` Specifies Host address
   | By default, this is localhost, but may be set to IP address or FQDNS address.

-  | ``-U`` Specifies Username
   | This is the username that is authorized to make changes to the database defined in -D.

-  | ``-P`` Specifies Password
   | The password for username specified in -U.

-  ``-R`` Password for Administrator or Root DB account.

-  ``-A`` Password for Administrator or Root DB account.

-  ``-J`` Jid of user authorized as admin user from Tigase.

-  ``-N`` Password for user specified in -J.

-  | ``-F`` Points to the file that will perform the upgrade.
   | Will follow this form database/{dbname}-server-schema-8.0.0.sql

Tigase Server Schema v7.2 Updates
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**FOR ALL USERS UPGRADING TO v8.0.0 FROM A v7.0.2 INSTALLATION**
''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''

| The schema has changed for the main database, and the pubsub repository. In order to upgrade to the new schemas, you will need to do the following:

1. Upgrade the Main database schema to v7.1 using the ``database/${DB_TYPE}-schema-upgrade-to-7-1.sql`` file

2. Upgrade the Pubsub Schema to v3.1.0 using the ``database/${DB_TYPE}-pubsub-schema-3.1.0.sql`` file

3. Upgrade the Pubsub Schema to v3.2.0 using the ``database/${DB_TYPE}-pubsub-schema-3.2.0.sql`` file

4. Upgrade the Pubsub Schema to v3.3.0 using the ``database/${DB_TYPE}-pubsub-schema-3.3.0.sql`` file

All three commands may be done at the same time in that order, it is suggested you make a backup of your current database to prevent data loss.


Tigase Schema Change for v7.1
''''''''''''''''''''''''''''''

Tigase has made changes to its database to include primary keys in the tig_pairs table to improve performance of the Tigase server. This is an auto-incremented column for Primary Key items appended to the previous schema.

.. Warning::

    You MUST update your database to be compliant with the new schema. If you do not, Tigase will not function properly.**

.. Note::

   *This change will affect all users of Tigase using v7.1.0 and newer.*

If you are installing a new version of v8.0.0 on a new database, the schema should automatically be installed.

First, shut down any running instances of Tigase to prevent conflicts with database editing. Then from command line use the DBSchemaLoader class to run the -schema-upgrade-to-7.1.sql file to the database. The command is as follows:

In a linux environment

.. code:: bash

   java -cp "jars/*" tigase.db.util.DBSchemaLoader -dbHostname ${HOSTNAME} -dbType ${DB_TYPE} -rootUser ${ROOT_USER} -dbPass ${DB_USER_PASS} -dbName ${DB_NAME} -schemaVersion ${DB_VERSION} -rootPass ${ROOT_USER_PASS} -dbUser ${DB_USER}  -adminJID "${ADMIN_JID}" -adminJIDpass ${ADMIN_JID_PASS}  -logLevel ALL -file database/${DB_TYPE}-schema-upgrade-to-7-1.sql

In a windows environment

.. code:: bash

   java -cp jars/* tigase.db.util.DBSchemaLoader -dbHostname ${HOSTNAME} -dbType ${DB_TYPE} -rootUser ${ROOT_USER} -dbPass ${DB_USER_PASS} -dbName ${DB_NAME} -schemaVersion ${DB_VERSION} -rootPass ${ROOT_USER_PASS} -dbUser ${DB_USER}  -adminJID "${ADMIN_JID}" -adminJIDpass ${ADMIN_JID_PASS}  -logLevel ALL -file database/${DB_TYPE}-schema-upgrade-to-7-1.sql

All variables will be required, they are as follows:

-  ``${HOSTNAME}`` - Hostname of the database you wish to upgrade.

-  ``${DB_TYPE}`` - Type of database [derby, mysql, postgresql, sqlserver].

-  ``${ROOT_USER}`` - Username of root user.

-  ``${ROOT_USER_PASS}`` - Password of specified root user.

-  ``${DB_USER}`` - Login of user that can edit database.

-  ``${DB_USER_PASS}`` - Password of the specified user.

-  ``${DB_NAME}`` - Name of the database to be edited.

-  ``${DB_VERSION}`` - In this case, we want this to be 7.1.

-  ``${ADMIN_JID}`` - Bare JID of a database user with admin privileges. Must be contained within quotation marks.

-  ``${ADMIN_JID_PASS}`` - Password of associated admin JID.

Please note that the SQL file for the update will have an associated database with the filename. i.e. postgresql-update-to-7.1.sql for postgresql database.

A finalized command will look something like this:

.. code:: bash

   java -cp "jars/*" tigase.db.util.DBSchemaLoader -dbHostname localhost -dbType mysql -rootUser root -rootPass root -dbUser admin -dbPass admin -schemaVersion 7.1 -dbName Tigasedb -adminJID "admin@local.com" -adminJIDPass adminpass -logLevel ALL -file database/mysql-schema-upgrade-to-7.1.sql

Once this has successfully executed, you may restart you server. Watch logs for any db errors that may indicate an incomplete schema upgrade.

Changes to Pubsub Schema
'''''''''''''''''''''''''

Tigase has had a change to the PubSub Schema, to upgrade to PubSub Schema v7.1 without having to reform your databases, use this guide to update your databases to be compatible with the new version of Tigase.

.. Note::

   Current PubSub Schema is v3.3.0, you will need to repeat these instructions for v3.1.0, v3.2.0 and then v3.3.0 before you run Tigase V7.1.0.

The PubSub Schema has been streamlined for better resource use, this change affects all users of Tigase. To prepare your database for the new schema, first be sure to create a backup! Then apply the appropriate PubSub schema to your MySQL and it will add the new storage procedure.

All these files should be in your /database folder within Tigase, however if you are missing the appropriate files, use the links below and place them into that folder.

The MySQL schema can be found `Here <https://github.com/tigase/tigase-pubsub/blob/master/src/main/database/mysql-pubsub-4.1.0.sql>`__.

The Derby schema can be found `Here <https://github.com/tigase/tigase-pubsub/blob/master/src/main/database/derby-pubsub-4.1.0.sql>`__.

The PostGRESQL schema can be found `Here <https://github.com/tigase/tigase-pubsub/blob/master/src/main/database/postgresql-pubsub-4.1.0.sql>`__.

The same files are also included in all distributions of v8.0.0 in [tigaseroot]/database/ . All changes to database schema are meant to be backward compatible.

You can use a utility in Tigase to update the schema using the following command from the Tigase root:

-  Linux

   .. code:: bash

      java -cp "jars/*" tigase.db.util.DBSchemaLoader

-  Windows:

   ::

      java -cp jars/* tigase.db.util.DBSchemaLoader

.. Note::

   **Some variation may be necessary depending on how your java build uses ``-cp`` option**

Use the following options to customize. Options in bold are required.:

-  ``-dbType`` database_type {derby, mysql, postgresql, sqlserver} (*required*)

-  ``-schemaVersion`` schema version {4, 5, 5-1}

-  ``-dbName`` database name (*required*)

-  ``-dbHostname`` database hostname (default is localhost)

-  ``-dbUser`` tigase username

-  ``-dbPass`` tigase user password

-  ``-rootUser`` database root username (*required*)

-  ``-rootPass`` database root password (*required*)

-  ``-file path`` to sql schema file (*required*)

-  ``-query`` sql query to execute

-  ``-logLevel`` java logger Level

-  ``-adminJID`` comma separated list of admin JIDs

-  ``-adminJIDpass`` password (one for all entered JIDs

.. Note::

   Arguments take following precedent: query, file, whole schema

As a result your final command should look something like this:

::

   java -cp "jars/*" tigase.db.util.DBSchemaLoader -dbType mysql -dbName tigasedb -dbUser root -dbPass password -file database/mysql-pubsub-schema-3.1.0.sql

2.9. Components
----------------
The only step is to tell the server what components to load, how to name them and optionally give some extra parameters. To do so open the ``config.tdsl`` file you use in your installation.

Let’s say you want to just add PubSub for now. All you need to do is add the following to the properties file:

.. code:: dsl

   pubsub (class: tigase.pubsub.PubSubComponent) {}

Normally, this is not necessary since pubsub is loaded by default, however this is just an example of loading a class with the DSL format.

.. code:: dsl

   'pubsub-priv' (class: tigase.pubsub.PubSubComponent) {}

As you can see, we can customize the name of a component in the deceleration, here we are using pubsub-priv.

Although this may be rare, it allows for wide compatibility and platform stability.

Normally, however we want to load few different components like PubSub, MUC, MSN Transport and so on…​. Therefore instead of the above second PubSub we can load the MUC component:

.. code:: dsl

   muc (class: tigase.muc.MUCComponent) {}
   pubsub (class: tigase.pubsub.PubSubComponent) {}

Changes to the ``config.tdsl`` file will take effect upon server restart.

2.9.1. Advanced Message Processing - AMP XEP-0079
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Tigase server offers support for `XEP-0079: Advanced Message Processing <http://xmpp.org/extensions/xep-0079.html>`__ (often abbreviated to AMP).

It is enabled by default but there are several configuration options that you may tweak.

Configuration of AMP is not very complex, but as it is implemented as a component in the Tigase server it does needs a few settings to get it right.

Here is a first, brief overview of the AMP configuration and later detailed explanation of each parameter.

.. code:: dsl

   'sess-man' {
       amp () {
           'amp-jid' = 'amp@your-domain.tld'
       }
       message (active: false) {}
       msgoffline (active: false) {}
   }
   'amp-security-level' = 'STRICT'

First of all: plugins
~~~~~~~~~~~~~~~~~~~~~~~

Even though the whole functionality is implemented inside the component you need a way to forward messages with ``AMP`` payload to that component. This is what the ``amp`` plugin does. The ``amp`` plugin intercepts all ``<message/>`` packets even without AMP payload, redirecting some of the to the ``AMP`` component and others processing in a standard way. Therefore you no longer need ``message`` plugin or ``msgoffline`` plugin. Those are all functions are offered by the ``amp`` plugin now. Hence you have to switch ``message`` and ``msgoffline`` plugins off (the ``amp`` plugin is loaded by default):

.. code:: dsl

   'sess-man' {
       amp () {}
       message (active: false) {}
       msgoffline (active: false) {}
   }

The ``amp`` plugin needs to know where to forward all the ``AMP`` packets. By default plugin uses hostname of the given machine as this is true to the most installations. However, this is configured by the last line of the example configuration, which forwards all packets to the address ``amp@your-domain.tld``:

.. code:: dsl

   'sess-man' {
       amp () {
           'amp-jid' = 'amp@your-domain.tld'
       }
   }

Secondly: component
~~~~~~~~~~~~~~~~~~~~

By default Tigase loads the component with the standard name ``amp``

Optional parameters
~~~~~~~~~~~~~~~~~~~~

There is also one parameter shared between the component and the plugin. Connection to the database where offline messages are stored. The AMP component has a dedicated schema for storing offline messages designed for a high traffic and high load installations. It does not use ``UserRepository`` for storing messages.

By default the same physical database as for ``UserRepository`` is used but you can change it and store messages in a completely separate location to reduce performance degradation of rest of the system. You can set a database connection string using following property:

.. code:: dsl

   dataSource {
       'default-amp' () {
           uri = 'jdbc:mysql://localhost/tigasedb?user=db_usr&password=db_pwd'
       }
   }

The `XEP-0079 <http://xmpp.org/extensions/xep-0079.html>`__ specification has a `Section 9. - Security Considerations <http://xmpp.org/extensions/xep-0079.html#security>`__. As it describes, in some cases the AMP protocol can be used to reveal user’s presence information by other users who are not authorized for presence updates. There are a few possible ways to prevent this.

Tigase’s implementation offers 3 modes to handle ``AMP`` requests to prevent revealing user’s status to non-authorized users:

.. code:: dsl

   'amp-security-level' = 'STRICT'

In this mode the server performs strict checking. The ``AMP`` specification is fully handled. This however involves roster loading for each offline user, hence it may impact the service performance. It may not be feasible or possible to run in this mode for services under a high load with lots of AMP messages.

In the XEP this mode is described in the following way:

*Accept the relevant condition only if the sender is authorized to receive the receiver’s presence, as a result of which the server MUST reply with a <not-acceptable/> error condition if the sender is not so authorized; this is the RECOMMENDED behavior. This is also the default in Tigase.*

.. code:: dsl

   'amp-security-level' = 'PERFORMANCE'

Dummy checking is performed efficiently by just returning an error response every time there is a chance that the default action may reveal user status without looking into the user’s roster. This does not affect performance but it does impact the ``AMP`` compliance.

In the XEP this mode is described in the following way:

*Accept the relevant condition only if the action is "drop", as a result of which the server MUST reply with a <not-acceptable/> error condition if the action is "alert", "error", or "notify"; this is slightly less restrictive but still unnecessarily restricts the functionality of the system, so is NOT RECOMMENDED.*

It does not do any checking. It acts like all users are authorized to receive notifications, even if it may reveal user status to unauthorized users. It does not impact the server performance and it offers full AMP compliance.

.. code:: dsl

   'amp-security-level' = 'NONE'

2.9.2. Server Monitoring
^^^^^^^^^^^^^^^^^^^^^^^^

All the documentation and resources related to the Tigase server monitoring.

-  `Setting up Remote Monitoring in the Server <#setupRemoteMonitoring>`__

-  `Statistics Logger Configuration <#statLoggerConfig>`__

-  `Retrieving Statistics from the Server <#retrievingStatisticsFromTheServer>`__

-  `Monitor Component <#monitorComponent>`__

Setting Up Remote Monitoring in the Server
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Tigase server can be remotely monitored over following protocols: ``JMX/RMI``, ``SNMP`` and ``HTTP``. Even though ``JMX`` offers the biggest control and visibility to the server states, all of the monitoring services give the same basic set of the server statistics:

-  Number of network connections for s2s, c2s and Bosh

-  Last second, last minute and last hour load for all main components: SM, MR, c2s, s2s, Bosh, MUC and PubSub

-  System statistics - memory usage (heap and non heap) and the server uptime in milliseconds and human readable text.

-  Users statistics - number of registered users and number of online user session.

JMX/RMI and SNMP servers offer basic security and can restrict access while the HTTP server doesn’t offer any access restriction mechanisms. Therefore HTTP monitoring is recommended to operate behind a firewall.

The monitoring itself causes very low overhead in terms of the resources and CPU consumption on top of the normal Tigase processing requirements so it can be left on without worrying about performance degradation.

NOTE This works with the Tigase server from version **4.2.0** or build **1418**.

What You Need
'''''''''''''

Statistics binaries are built-in ``-dist-max`` and no extra files are needed. If you have downloaded ``-dist`` file, you will need tigase-extras[https://github.com/tigase/tigase-extras] built and included in the ``jars/`` directory.

Activation
''''''''''

You can either run the Tigase installer and use the configuration wizard to activate the monitoring or edit etc/config.tdsl file and add following lines:

.. code:: dsl

   monitoring() {
     jmx() {
       port = 9050
     }
     http() {
       port = 9080
     }
     snmp() {
       port = 9060
     }
   }

As you see there is a separate block for each monitoring server you want to activate. Each server is responsible for activation of a different protocol and takes a single parameter - port number. There are following protocols supported right now:

-  ``jmx`` - activating monitoring via JMX/RMI

-  ``http`` - activating monitoring over HTTP protocol

-  ``snmp`` - activating monitoring over SNMP protocol

You can have all protocols active at the same time or any combination of them or none.

Security
''''''''

Both JMX and SNMP offer security protection to limit access to monitoring data. The security configuration is a bit different for both.

JMX
'''

After the server installation or in the SVN repository you can find 2 files in the ``etc/`` directory: ``jmx.access`` and ``jmx.password``.

-  ``jmx.access`` is a user permission file. You can use it to specify whether the user can access the monitoring data for reading only ``readonly`` or with read-write ``readwrite`` access. There are example entries in the file already and the content may simply look like:

   .. code:: bash

      monitor readonly
      admin readwrite

-  ``jmx.password`` is a user password file. You can set user passwords here and the format again is very simple and the same as for jmx.access. There are example entries already provided for you convenience. Content of the file may look like the example below:

   .. code:: bash

      admin admin_pass
      monitor monitor_pass

Using above to files you can control who and how can access the JMX monitoring services.

SNMP

Access to SNMP monitoring is controlled using ACL (access control lists) which can be configured in the file ``snmp.acl`` located in ``etc/`` directory. It contains lots of detailed instructions how to setup ACL and restrict access per user, host and what kind access is allowed. The simplest possible configuration may look like this:

.. code:: bash

   acl = {
     {
       communities = public, private
       access = read-only
       managers = public.host.com, private.host.com
     }
     {
       communities = admin
       access = read-write
       managers = localhost, admin.host.com
     }
   }

You might also need Tigase MIB definition: `TIGASE-MANAGEMENT-MIB.mib <https://github.com/tigase/tigase-server/blob/master/src/main/resources/mib/JVM-MANAGEMENT-MIB.mib>`__ for the server specific statistics. The MIB contains definition for all the server statistics exposed via SNMP.

HTTP

Access the server at example.com:9080 and you will be presented with an Agent View.

Retrieving statistics from the server
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

By default we can retrieve server statistics using XMPP, no additional setup is necessary.

Retrieving statistics using XMPP
'''''''''''''''''''''''''''''''''

Accessing statistics over XMPP protocol requires any XMPP client capable of executing `XEP-0050: Ad-Hoc Commands <http://xmpp.org/extensions/xep-0050.html>`__. It’s essential to remember, that only administrator (a user whose JID is configured as administrative) can access the statistics.

Psi XMPP Client
''''''''''''''''

For the purpose of this guide `Psi <http://psi-im.org/>`__ client will be used. After successfully configuring and connecting to account with administrative privileges we need to access *Service Discovery*, either from application menu or from context menu of the particular account account:

|roster-discovery|

In the *Service Discovery* window we need to find *Server Statistics* component:

|discovery-stats|

We can either access statistics for all components or select particular component after expanding the tree. To execute ad-hoc command simply double click on the particular node which will open window with statistics:

|server-stats|

In this window, in addition to see the statistics, we can adjust *Stats level* by selecting desired level from the list and confirm by clicking *Finish*.

Retrieving statistics using JMX
''''''''''''''''''''''''''''''''

In order to access statistics over JMX we need to enable support for it in Tigase - `Monitoring Activation <#monitoring_activation>`__. Afterwards we can use a number of tools to get to the statistics, for example the following:

JConsole
'''''''''

After opening JConsole we either select local process or provide details of the remote process, including IP, port and credentials from **etc/jmx.**\ \* files:

|jconsole|

Afterwards we navigate to the MBeans tab from where we can access the ``tigase.stats`` MBean. It offers similar options to XMPP - either accessing statistics for all components or only for particular component as well as adjusting level for which we want to obtain statistics:

|jconsole-1|


StatsDumper.groovy
'''''''''''''''''''

In order to collect statistics over period of time following groovy script can be used: `StatsDumper.groovy <files/StatsDumper.groovy>`__. It’s a Simple JMX client that connects to Tigase and periodically saves all statistics to files.

It takes following parameters:

.. code:: bash

   $ groovy StatsDumper.groovy [hostname] [username] [password] [dir] [port] [delay(ms)] [interval(ms)] [loadhistory(bool)]

-  ``hostname`` - address of the instance

-  ``username`` - JMX username

-  ``password`` - JMX username

-  ``dir`` - directory to which save the files with statistics

-  ``port`` - port on which to make the connection

-  ``delay``\ (ms) - initial delay in milliseconds after which statistics should be saved

-  ``interval``\ (ms) - interval between each retrieval/saving of statistics

-  ``loadhistory``\ (bool) - indicates whether or not load statistics history from server (if such is enabled in Tigase)

.. |roster-discovery| image:: images/admin/monitoring_xmpp_1.png
.. |discovery-stats| image:: images/admin/monitoring_xmpp_2.png
.. |server-stats| image:: images/admin/monitoring_xmpp_3.png
.. |jconsole| image:: images/admin/monitoring_jmx_jconsole_1.png
.. |jconsole-1| image:: images/admin/monitoring_jmx_jconsole_2.png

Monitor Component
~~~~~~~~~~~~~~~~~

Tigase includes an **Monitor Component** to help with monitoring has been implemented. This allows you to set thresholds for certain predefined tasks and you or other JIDs can be sent a message when those thresholds are passed. You can even configure a mailer extension to have an E-mail sent to system administrators to let them know an event has occurred! Lets begin with setup and requirements.

Monitor Component is based on eventbus which in turn is based on a limited `PubSub <http://www.xmpp.org/extensions/xep-0060.html>`__ specification. Events are delivered to subscribers as a normal PubSub notification.

Each component or client may subscribe for specific types of events. Only components on cluster nodes are allowed to publish events.

Setup
'''''

Monitor Component is enabled by default on v7.1.0 b4001 and later, so no setup needed!

How it Works
''''''''''''

Events in Eventbus are identified by two elements: name of event and its namespace:

.. code:: xml

   <EventName xmlns="tigase:demo">
     <sample_value>1</sample_value>
   </EventName>

Where event name is ``EventName`` and namespace is ``tigase:demo``.

Listeners may subscribe for a specific event or for all events with specific a namespace. Because in pubsub, only one node name exists, so we have to add a way to convert the event name and namespace to a node name:

::

   nodename = eventname + "|" + namespace

So for example, to subscribe to ``<EventName xmlns="tigase:demo">``, node must be: ``EventName|tigase:demo``. If you wish to subscribe to all events with a specific namespace, use an asterisk (``*``) instead of the event name: ``*|tigase:demo``.

   **Note**

   If client is subscribed to ``*|tigase:demo node``, then events will not be sent from node ``*|tigase:demo``, but from the **real** node (in this case: ``EventName|tigase:demo``).

Available Tasks
'''''''''''''''

Monitor Component has several pre-defined tasks that can be monitored and set to trigger. What follows is the list of tasks with the options attributed to each task.

-  | **disk-task** - Used to check disk usage.
   | Available Options

   1. ``enabled`` - Enable or disable task, Boolean value.

   2. ``period`` - Period of running check, Integer value.

   3. ``threshold`` - Percentage of used space on disk, Float value.

-  | **cpu-temp-task** - Used to check CPU temperature.
   | Available Options

   1. ``enabled`` - Enable or disable task, Boolean value.

   2. ``period`` - Period of running check, Integer value.

   3. ``cpuTempThreshold`` - Temperature threshold of CPU in °C.

-  | **load-checker-task** - Used to check system load.
   | Available Options

   1. ``enabled`` - Enable or disable task, Boolean value.

   2. ``period`` - Period of running check, Integer value.

   3. ``averageLoadThreshold`` - Average percent load threshold, Long value.

-  | **memory-checker-task** - Used to check memory usage.
   | Available Options

   1. ``enabled`` - Enable or disable task, Boolean value.

   2. ``period`` - Period of running check, Integer value.

   3. ``maxHeapMemUsagePercentThreshold`` - Alarm when percent of used Heap memory is larger than, Integer value.

   4. ``maxNonHeapMemUsagePercentThreshold`` - Alarm when percent of used Non Heap memory is larger than, Integer value.

-  | **logger-task** - Used to transmit log entries depending on level entered.

   1. ``enabled`` - Enable or disable task, Boolean value.

   2. ``levelThreshold`` - Minimal log level that will be the threshold. Possible values are SEVERE, WARNING, INFO, CONFIG, FINE, FINER, FINEST, and ALL.

-  | **connections-task** - Used to check users disconnections.
   | **NOTE: The event will be generated only if both thresholds (amount and percentage) will be fulfilled.**

   1. ``enabled`` - Enable or disable task, Boolean value.

   2. ``period`` - Period of running check in ms, Integer value.

   3. ``thresholdMinimal`` - Minimal amount of disconnected users required to generate alarm.

   4. ``threshold`` - Minimal percent of disconnected users required to generate alarm.


Configuration
''''''''''''''

Configuration of the monitor can be done one of two ways; either by lines in ``config.tdsl`` file, or by sending XMPP stanzas to the server. You may also send XMPP stanzas VIA HTTP REST. XMPP stanza configurations will override ones in config.tdsl, but they will only last until the server restarts.

config.tdsl

Tasks can be configured in the ``config.tdsl`` file. See `available tasks <#availableTasks>`__ for the tasks that can be setup.

To enable a specific monitor task, use the following line:

.. code:: dsl

   monitor {
       '$TASKNAME' {
           setting = value
       }
   }

Where monitor is the component name for ``MonitorComponent``, and ``$TASKNAME`` is one of the `available task names <#availableTasks>`__.

This format will be the same for other settings for tasks, and it’s best to group settings under one heading. For example:

.. code:: dsl

   monitor {
       'connections-task' {
           enabled = true
           period = 1000
       }
   }

sets the check period to 1000 milliseconds and enables ``connections-task``.

.. Note::

   Once triggers have been activated, they will become dormant. Think of these as one-shot settings.


Subscription Limitations

To define list of JIDs allowed to subscribe for events:

.. code:: dsl

   eventbus {
       affiliations {
           allowedSubscribers = 'francisco@denmark.lit,bernardo@denmark.lit'
       }
   }

If this is not specified, all users can subscribe.

Configuration via XMPP

We can also configure the eventbus monitor component using XMPP stanzas. This allows us to set and change configurations during server runtime. This is done using a series of ``iq`` stanzas send to the monitor component.

We can query each component for its current settings using the following stanza.

.. code:: xml

   <iq type="set" to="monitor@$DOMAIN/disk-task" id="aad0a">
       <command xmlns="http://jabber.org/protocol/commands" node="x-config"/>
   </iq>

The server will return the component current settings which will make things easier if you wish to edit them. In this case, the server has returned the following to us

.. code:: xml

   <iq from="monitor@$DOMAIN/disk-task" type="result" id="aad0a" to="alice@coffeebean.local/Psi+">
       <command xmlns="http://jabber.org/protocol/commands" status="executing" node="x-config"
                sessionid="0dad3436-a029-4082-b0e0-04d838c6c0da">
           <x xmlns="jabber:x:data" type="">
               <title>Task Configuration</title>
               <instructions/>
               <field type="boolean" label="Enabled" var="x-task#enabled">
                   <value>0</value>
               </field>
               <field type="text-single" label="Period [ms]" var="x-task#period">
                   <value>60000</value>
               </field>
               <field type="text-single" label="Disk usage ratio threshold" var="threshold">
                   <value>0.8</value>
               </field>
           </x>
       </command>
   </iq>

This tells us that the disk-task setting is not active, has a period of 60000ms, and will trigger when disk usage is over 80%.

To send new settings to the monitor component, we can send a similar stanza back to the monitor component.

.. code:: xml

   <iq type="set" to="monitor@$DOMAIN/disk-task" id="aad1a">
       <command xmlns="http://jabber.org/protocol/commands" node="x-config"
                sessionid="0dad3436-a029-4082-b0e0-04d838c6c0da">
           <x xmlns="jabber:x:data" type="submit">
               <field type="boolean" var="x-task#enabled">
                   <value>0</value>
               </field>
               <field type="text-single" var="x-task#period">
                   <value>60000</value>
               </field>
               <field type="text-single" var="threshold">
                   <value>0.8</value>
               </field>
           </x>
       </command>
   </iq>

To which a successful update will give you an XMPP success stanza to let you know everything is set correctly.

Alternatively, you can update specific settings by editing a single field without adding anything else. For example, if we just wanted to turn the disk-task on we could send the following stanza:

.. code:: xml

   <iq type="set" to="monitor@$HOSTNAME/disk-task" id="ab53a">
       <command xmlns="http://jabber.org/protocol/commands" node="x-config">
           <x xmlns="jabber:x:data" type="submit">
               <field type="boolean" var="x-task#enabled">
                   <value>1</value>
               </field>
           </x>
       </command>
   </iq>

To set any other values, do not forget that certain parts may need to be changed, specifically the ``<field type="boolean" var=x-task#enabled">`` fields:

-  | Your field type will be defined by the type of variable specified in the `Available Tasks <#availableTasks>`__ section.

-  ``var=x task#`` will be followed by the property value taken directly from the `Available Tasks <#availableTasks>`__ section.

Getting the Message
''''''''''''''''''''

Without a place to send messages to, monitor will just trigger and shut down. There are two different methods that monitor can deliver alarm messages and relevant data; XMPP messages and using the mailer extension.

XMPP notification

| In order to retrieve notifications, a subscription to the ``eventbus@<VHost>`` user must be made. Keep in mind that subscriptions are not persistent across server restarts, or triggers.
| The monitor schema is very similar to most XMPP subscription requests but with a few tweaks to differentiate it if you wanted to subscribe to a certain task or all of them. Each task is considered a node, and each node has the following pattern: ``eventName|eventXMLNS``. Since each monitoring task has the ``tigase:monitor:event`` event XMLNS, we just need to pick the event name from the list of tasks. So like the above example, our event node for the disk task will be ``disk-task|tigase:monitor:event``. Applied to an XMPP stanza, it will look something like this:

.. code:: xml

   <iq type='set'
       to='eventbus@<VHost>'
       id='sub1'>
     <pubsub xmlns='http://jabber.org/protocol/pubsub'>
       <subscribe node='disk-taskEvent|tigase:monitor:event' jid='$USER_JID'/>
     </pubsub>
   </iq>

Don’t forget to replace ``$USER_JID`` with the bare JID of the user you want to receive those messages. You can even have them sent to a MUC or any component with a JID.

Available events are as follows:

-  DiskUsageMonitorEvent for ``disk-task``

-  LoggerMonitorEvent for ``logger-task``

-  HeapMemoryMonitorEvent for ``memory-checker-task``

-  LoadAverageMonitorEvent for ``load-checker-task``

-  CPUTempMonitorEvent for ``cpu-temp-task``

-  UsersDisconnected for ``connections-task``

Alternatively, you can also subscribe to all events within the eventbus by using a wildcard \* in place of the event XMLNS like this example:

.. code:: xml

   <iq type='set'
       to='eventbus@<VHost>'
       id='sub1'>
     <pubsub xmlns='http://jabber.org/protocol/pubsub'>
       <subscribe node='*|tigase:monitor:event' jid='$USER_JID'/>
     </pubsub>
   </iq>

Sample notification from Monitor

.. code:: xml

   <message from='eventbus.shakespeare.lit' to='francisco@denmark.lit' id='foo'>
     <event xmlns='http://jabber.org/protocol/pubsub#event'>
       <items node='EventName|tigase:demo'>
         <item>
           <EventName xmlns="tigase:demo" eventSource="samplecomponent.shakespeare.lit'" eventTimestamp="1444216850">
             <sample_value>1</sample_value>
           </EventName>
         </item>
       </items>
     </event>
   </message>

Mailer Extension
'''''''''''''''''

*Tigase Server Monitor Mailer Extension* (TSMME) can send messages from the monitor component to a specified E-mail address so system administrators who are not logged into the XMPP server.

For v7.1.0 versions and later, TSMME is already included in your distribution package and no extra installation is needed.

Configuration

Tigase Mailer Extension may be configured via the ``config.tdsl`` file in the following manner:

.. code:: dsl

   monitor {
       'mailer-from-address' = 'sender@<VHost>'
       'mailer-smtp-host' = 'mail.tigase.org'
       'mailer-smtp-password' = '********'
       'mailer-smtp-port' = '587'
       'mailer-smtp-username' = 'sender'
       'mailer-to-addresses' = 'receiver@<VHost>,admin@<VHost>'
   }

Here is an explanation of those variables.

-  ``mailer-smtp-host`` - SMTP Server hostname.

-  ``mailer-smtp-port`` - SMTP Server port.

-  ``mailer-smtp-usernam`` - name of sender account.

-  ``mailer-smtp-password`` - password of sender account.

-  ``mailer-from-address`` - sender email address. It will be set in field from in email.

-  ``mailer-to-addresses`` - comma separated notification receivers email addresses.

It is recommended to create a specific e-mail address in your mail server for this purpose only, as the account settings are stored in plaintext without encryption.

Configuration of statistics loggers
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

It is possible to enable and configure automatic storage of statistics information. To do that you need to configure any of following statistics loggers as a ``StatisticsCollector`` component sub-beans:

``tigase.stats.CounterDataArchivizer``
   every execution put current basic server metrics (CPU usage, memory usage, number of user connections, uptime) into database (overwrites previous entry).

``tigase.stats.CounterDataLogger``
   every execution insert new row with new set of number of server statistics (CPU usage, memory usage, number of user connections per connector, number of processed packets of different types, uptime, etc) into the database.

``tigase.stats.CounterDataFileLogger``
   every execution store all server statistics into separate file.

As an example to configure ``tigase.stats.CounterDataFileLogger`` to archive statistics data with level ``FINE`` every 60 seconds to file prefixed with ``stat`` and located in ``logs/server_statistics`` following entry is needed:

.. code:: dsl

   stats() {
       'stats-file-logger' (class: tigase.stats.CounterDataFileLogger) {
           'stats-directory' = 'logs/server_statistics'
           'stats-filename' = 'stat'
           'stats-unixtime' = false
           'stats-datetime' = true
           'stats-datetime-format' = 'HH:mm:ss'
           'stats-level' = 'FINEST'
       }
   }

2.9.3. Server to Server Protocol Settings
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Tigase server-to-server communication component facilitates communication with other XMPP servers (federation) and allows you to tweak it’s configuration to get a better performance in your installation.

S2S (or server to server) protocol is enabled by default with optimal settings chosen. There are however, a set of configuration parameters you can adjust the server behavior to achieve optimal performance on your installation.

This documents describes following elements of the Tigase server configuration:

1. Number of concurrent connections to external servers

2. The connection throughput parameters

3. Maximum waiting time for packets addressed to external servers and the connection inactivity time

4. Custom plugins selecting connection to the remote server

Number of Concurrent Connections
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Normally only one connection to the remote server is required to send XMPP stanza to that server. In some cases however, under a high load, you can get much better throughput and performance if you open multiple connections to the remote server.

This is especially true when the remote server works in a cluster mode. Ideally you want to open a connection to each of the cluster nodes on the remote server. This way you can spread the traffic evenly among cluster nodes and improve the performance for s2s connections.

Tigase server offers 2 different parameters to tweak the number of concurrent, s2s connections:

-  ``max-out-total-conns`` - this property specifies the maximum outgoing connections the Tigase server opens to any remote XMPP server. This is a **per domain** limit, which means that this limit applies to each of the remote domains Tigase connects to. If it is set to ``4`` then Tigase opens a maximum of 4 connections to ``jabber.org`` plus maximum 4 connections to ``muc.jabber.org`` even if this is the same physical server behind the same IP address.

   To adjust the limit you have to add following to the ``config.tdsl`` file:

   .. code:: dsl

      s2s {
          'max-out-total-conns' = 2
      }

-  ``max-out-per-ip-conns`` - this property specifies the maximum outgoing connections Tigase server opens to any remote XMPP server to its single IP address. This too, is **per domain** limit, which means that this limit applies to each of the remote domains Tigase connects to. If it is set to ``1``, and the above limit is set to ``4``, and the remote server is visible behind 1 IP address, then Tigase opens a maximum of 1 connection to ``jabber.org`` plus a maximum of 1 connection to ``muc.jabber.org`` and other subdomains.

   To adjust the limit you have to add following line to the ``config.tdsl`` file:

   .. code:: dsl

      s2s {
          'max-out-per-ip-conns' = 2
      }


Connection Throughput
~~~~~~~~~~~~~~~~~~~~~

Of course everybody wants his server to run with maximum throughput. This comes with a cost on resources, usually increased memory usage. This is especially important if you have large number of s2s connections on your installations. High throughput means lots of memory for network buffers for every single s2s connection. You may soon run out of all available memory.

There is one configuration property which allows you to adjust the network buffers for s2s connections to lower your memory usage or increase data throughput for s2s communication.

More details about are available in the `net-buff-high-throughput <#netBuffHighThroughput>`__ or `net-buff-Standard <#netBuffStandard>`__ property descriptions.

Maximum Packet Waiting Time and Connection Inactivity Time
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

There are 2 timeouts you can set for the component controlling s2s communication.

-  ``max-packet-waiting-time`` - this sets the maximum time for the packets waiting for sending to some remote server. Sometimes, due to networking problems or DNS problems it might be impossible to send message to remote server right away. Establishing a new connection may take time or there might be communication problems between servers or perhaps the remote server is restarted. Tigase will try a few times to connect to the remote server before giving up. This parameter specifies how long the packet is waiting for sending before it is returned to the sender with an error. The timeout is specified in seconds:

   .. code:: dsl

      s2s {
          'max-packet-waiting-time' = 420L
      }

-  ``max-inactivity-time`` - this parameters specifies the maximum s2s connection inactivity time before it is closed. If a connection is not in use for a long time, it doesn’t make sense to keep it open and tie resources up. Tigase closes s2s connection after specified period of time and reconnects when it is necessary. The timeout is specified in seconds:

   .. code:: dsl

      s2s {
          'max-inactivity-time' = 900L
      }

Custom Plugin: Selecting s2s Connection
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Sometimes for very large installations you may want to set larger number of s2s connections to remote servers, especially if they work in cluster of several nodes. In such a case you can also have a control over XMPP packets distribution among s2s connections to a single remote server.

This piece of code is pluggable and you can write your own connection selector. It is enough to implement ``S2SConnectionSelector`` interface and set your class name in the configuration using following parameter in ``config.tdsl`` file:

.. code:: dsl

   s2s {
       's2s-conn-selector' = 'YourSelectorImplementation'
   }

The default selector picks connections randomly.

skip-tls-hostnames
~~~~~~~~~~~~~~~~~~~

The ``s2s-skip-tls-hostnames`` property disables TLS handshaking for s2s connections to selected remote domains. Unfortunately some servers (certain versions of Openfire - [`1 <http://community.igniterealtime.org/thread/36206>`__] or [`2 <http://community.igniterealtime.org/thread/30578>`__]) have problems with TLS handshaking over s2s which prevents establishing a usable connection. This completely blocks any communication to these servers. As a workaround you can disable TLS for these domains to get communication back. Enabling this can be done on any vhost, but must be configured under the s2s component.

.. code:: dsl

   s2s {
       'skip-tls-hostnames' = [ 'domain1', 'domain2' ]
   }

ejabberd-bug-workaround
~~~~~~~~~~~~~~~~~~~~~~~~

This property activates a workaround for a bug in EJabberd in it’s s2s implementation. EJabberd does not send dialback in stream features after TLS handshaking even if the dialback is expected/needed. This results in unusable connection as EJabberd does not accept any packets on this connection either. The workaround is enabled by default right now until the EJabberd version without the bug is popular enough. A disadvantage of the workaround is that dialback is always performed even if the SSL certificate is fully trusted and in theory this dialback could be avoided. By default, this is not enabled.

.. code:: dsl

   s2s {
       dialback () {
           'ejabbered-bug-workaround' = true
           }
   }

This replaces the old ``--s2s-ejabberd-bug-workaround-active`` property.

2.9.4. Tigase Load Balancing
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Tigase includes load balancing functionality allowing users to be redirected to the most suitable cluster node. Functionality relies on a see-other-host XMPP stream error message. The basic principle behind the mechanism is that user will get redirect if the host returned by the implementation differ from the host to which user currently tries to connect. It is required that the user JID to be known for the redirection to work correctly.

Available Implementations
~~~~~~~~~~~~~~~~~~~~~~~~~~~

Tigase implementation is, as usual, extensible and allows for different, pluggable redirection strategies that implement the ``SeeOtherHostIfc`` interface.

Currently there are three strategies available:

-  ``SeeOtherHost`` - most basic implementation returning either single host configured in ``config.tdsl`` file or name of the current host;

-  ``SeeOtherHostHashed`` (default) - default implementation for cluster environment of SeeOtherHostIfc returning redirect host based on the hash value of the user’s JID; list of the available nodes from which a selection would be made is by default composed and reflects all connected nodes, alternatively hosts list can be configured in the config.tdsl;

-  ``SeeOtherHostDB`` - extended implementation of SeeOtherHost using redirect information from database in the form of pairs ``user_id`` and ``node_id`` to which given user should be redirected.

-  ``SeeOtherHostDualIP`` - matches internal Tigase cluster nodes against the lookup table to provide relevant redirection hostname/IP (by default internal Tigase tig_cluster_nodes table will be used)

Configuration Options
~~~~~~~~~~~~~~~~~~~~~~

The most basic configuration is related to the choice of actual redirection implementation by declaring class for each connector:

.. code:: dsl

   bosh {
       seeOtherHost (class: <value>) {}
   }
   c2s {
       seeOtherHost (class: <value>) {}
   }
   ws2s {
       seeOtherHost (class: <value>) {}
   }

Possible values are:

-  ``tigase.server.xmppclient.SeeOtherHost``

-  ``tigase.server.xmppclient.SeeOtherHostHashed``

-  ``tigase.server.xmppclient.SeeOtherHostDB``

-  ``tigase.server.xmppclient.SeeOtherHostDualIP``

-  ``none`` - disables redirection

All options are configured on a per-connection-manager basis, thus all options need to be prefixed with the corresponding connection manager ID, i.e. c2s, bosh or ws; we will use c2s in the examples:

.. code:: dsl

   c2s {
       'cm-see-other-host' {
           'default-host' = 'host1;host2;host3'
           'phases' = [ 'OPEN', 'LOGIN' ]
       }
   }

-  ``'default-host' = 'host1;host2;host3'`` - a semicolon separated list of hosts to be used for redirection.

-  ``'phases' = []`` - an array of phases in which redirection should be active, currently possible values are:

   -  ``OPEN`` which enables redirection during opening of the XMPP stream;

   -  ``LOGIN`` which enables redirection upon authenticating user session;

By default redirection is currently enabled only in the ``OPEN`` phase.

SeeOtherHostDB
''''''''''''''

For ``SeeOtherHostDB`` implementation there are additional options:

.. code:: dsl

   c2s {
       'cm-see-other-host' {
           'db-url' = 'jdbc:mysqk://localhost/username?,password?'
           'get-all-query-timeout' = '10'
       }
   }

-  ``db-url`` - a JDBC connection URI which should be used to query redirect information; if not configured the default ``dataSource`` will be used;

-  ``get-host-query`` - a SQL query which should return redirection hostname;

-  ``get-all-data-query`` - a SQL helper query which should return all redirection data from database;

-  ``get-all-query-timeout`` - allows to set timeout for executed queries.


SeeOtherHostDualIP
'''''''''''''''''''

This mechanisms matches internal Tigase cluster nodes against the lookup table to provide matching and relevant redirection hostname/IP. By default internal Tigase ``tig_cluster_nodes`` table is used (and appropriate repository implementation will be used).

To enable this redirection mechanism following configuration / class should be used. Note that for global use, all connection managers must have the same class defined. You can define each connection manager individually.

.. code:: dsl

   bosh {
       seeOtherHost (class: tigase.server.xmppclient.SeeOtherHostDualIP) {}
   }
   c2s {
       seeOtherHost (class: tigase.server.xmppclient.SeeOtherHostDualIP) {}
   }
   ws2s {
       seeOtherHost (class: tigase.server.xmppclient.SeeOtherHostDualIP) {}
   }

It offers following configuration options:

-  ``data-source`` - configuration of the source of redirection information - by default internal Tigase ``tig_cluster_nodes`` table will be used (and appropriate repository implementation will be used); alternatively it’s possible to use ``eventbus`` source;

-  ``db-url`` - a JDBC connection URI which should be used to query redirect information; if not configured ``user-db-uri`` will be used;

-  ``get-all-data-query`` - a SQL helper query which should return all redirection data from database;

-  ``get-all-query-timeout`` - allows to set timeout for executed queries;

-  ``fallback-redirection-host`` - if there is no redirection information present (i.e. secondary hostname is not configured for the particular node) redirection won’t be generated; with this it’s possible to configure fallback redirection address.

All options are configured or on per-component basis:

.. code:: dsl

   <connector> {
       'cm-see-other-host' {
           'data-source' = '<class implementing tigase.server.xmppclient.SeeOtherHostDualIP.DualIPRepository>'
           'db-url' = 'jdbc:<database>://<uri>'
           'fallback-redirection-host' = '<hostname>'
           'get-all-data-query' = 'select * from tig_cluster_nodes'
           'get-all-query-timeout' = 10
       }
   }

EventBus as a source of information

It’s possible to utilize EventBus and internal Tigase events as a source of redirection data. In order to do that ``eventbus-repository-notifications`` needs to be enabled in ClusterConnectionManager:

.. code:: dsl

   'cl-comp' {
       'eventbus-repository-notifications' = true
   }


Auxiliary setup options
~~~~~~~~~~~~~~~~~~~~~~~~

Enforcing redirection
''''''''''''''''''''''

It’s possible to enforce redirection of connections on the particular port of connection manager with ``force-redirect-to`` set to Integer with the following general setting option:

.. code:: dsl

   <connection_manager> {
       connections {
           <listening_port> {
               'force-redirect-to' = <destination_port>
           }
       }
   }

for example, enable additional port ``5322`` for ``c2s`` connection manager and enforce all connections to be redirected to port ``5222`` (it will utilize hostname retrieved from ``SeeOtherHost`` implementation and will be only used when such value is returned):

.. code:: dsl

   c2s {
       connections {
           ports = [ 5222, 5322 ]
           5322 {
               'force-redirect-to' = 5222
               socket = 'plain'
               type = 'accept'
           }
       }
   }


Configuring hostnames
''''''''''''''''''''''

To fully utilize ``SeeOtherHostDualIP`` setup in automated fashion it’s now possible to provide both primary (*internal*) and secondary (*external*) hostname/IP (they need to be correct, ``InetAddress.getByName( property );`` will be used to verify correctness). It can be done via JVM properties ``tigase-primary-address`` and ``tigase-secondary-address``. You can also utilize different implementation of DNS resolver by providing class implementing ``tigase.util.DNSResolverIfc`` interface as value to ``resolver-class`` property. Those properties can be set via ``etc/tigase.conf`` (uncommenting following lines, or manually exposing in environment):

.. code:: bash

   DNS_RESOLVER=" -Dresolver-class=tigase.util.DNSResolverDefault "

   INTERNAL_IP=" -Dtigase-primary-address=hostname.local "
   EXTERNAL_IP=" -Dtigase-secondary-address=hostname "

or in the ``etc/config.tdsl`` (they will be converted to JVM properties):

.. code:: dsl

   'dns-resolver' {
       'tigase-resolver-class' = 'tigase.util.DNSResolverDefault'
       'tigase-primary-address' = 'hostname.local'
       'tigase-secondary-address' = 'hostname'
   }

2.9.5. External Component Configuration
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Tigase can connect to external components, this guide will show you how this can be accomplished.

Configuration follows the same standards as all other components. It is also much more powerful as a single Tigase instance can control many TCP/IP ports and many external components on each port and even allows for multiple connections for the same component. It supports both XEP-0114 and XEP-0225 with protocol auto-detection mechanisms. Protocols are pluggable so more protocols can be supported or custom extensions to existing protocols can be added.

The implementation also supports a scripting API and new domains with passwords can be added at run-time using ad-hoc commands. New scripts can be loaded to even further control all connected external components.

Pages in this guide describe in details all the administration aspects of setting up and managing external components.

-  `External Component Configuration <#tigaseExternalComponent>`__

-  `Tigase as an External Component <#tigaseasExternal>`__

-  `Load Balancing External Components in Cluster Mode <#loadBalancingExternalComponent>`__

External Component Configuration
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

As for all Tigase components you can load and configure external components via the ``config.tdsl`` file described in details in the `DSL configuration <#dslConfig>`__ section. This document describes how to enable the component and set the initial configuration to accept or initiate connections for an external component.

First thing to do is to specify the component class and the component name which must be unique within the Tigase installation. The most commonly name used is ``ext`` and the class is ``tigase.server.ext.ComponentProtocol`` (class doesn’t have to be specified when using default name).

The following line in the ``config.tdsl`` will load the component during the server startup time:

.. code:: dsl

   ext (class: tigase.server.ext.ComponentProtocol) {}

While this would load the component, without any additional configurations provided, the component would be practically useless. It is necessary to configure the virtual host domains of the external component during run-time via ad-hoc commands to make use of this component.

You may additionally configure the ```bind-ext-hostnames`` <#bindExtHostnames>`__ property.

To configure external component connections using Admin UI you need to open Admin UI web page (if you are logged in the same computer on which Tigase XMPP Server is running by default it should be available at http://localhost:8080/admin/). Then you should click on ``Configuration`` on the left side of the Admin UI web page and then select ``Add new item`` on ``ext`` component or by execution corresponding ad-hoc command on ``ext`` component using ad-hoc capable XMPP client, ie. `Psi <http://psi-im.org>`__.

|adminui ext add item button|

You will be presented with a form which you should fill to configure external component connection details:

|adminui ext add item form|

-  *Domain name* - external component domain name (``muc.devel.tigase.org``)

-  *Domain password* - password for authentication of the external component connection (``muc-pass``)

-  *Connection type* - ``accept`` to make component wait for connection or ``connect`` force component to connect to the server (``connect``)

-  *Port number* - port on which component should wait for connection or on which it try to connect (``5270``)

-  *Remote host* - host to connect to (``devel.tigase.org``) *(may be left blank if component will only accept connections)*

-  *Protocol* - id of protocol used for establishing connection

   -  if connection type is ``connect``:

      -  ``XEP-0114: Jabber Component Protocol (accept)`` - for `XEP-0114: Jabber Component Protocol <https://xmpp.org/extensions/xep-0114.html>`__

      -  ``XEP-0225: Component Connections`` - for `XEP-0225: Component Connections <https://xmpp.org/extensions/xep-0225.html>`__

   -  if connection type is ``accept``:

      -  ``Autodetect`` - for automatic detection of protocol used by incoming connection *(recommended)*

      -  ``XEP-0114: Jabber Component Protocol (accept)`` - for `XEP-0114: Jabber Component Protocol <https://xmpp.org/extensions/xep-0114.html>`__

      -  ``XEP-0225: Component Connections`` - for `XEP-0225: Component Connections <https://xmpp.org/extensions/xep-0225.html>`__

Additional options may be left with defaults.

Later on if you would like to modify this values, you can do that using Admin UI by clicking on ``Configuration`` and ``Remove an item`` or ``Update item configuration`` at ``ext`` component or by execution corresponding ad-hoc commands on ``ext`` component using ad-hoc capable XMPP client, ie. `Psi <http://psi-im.org>`__.

.. |adminui ext add item button| image:: images/admin/adminui_ext_add_item_button.png
.. |adminui ext add item form| image:: images/admin/adminui_ext_add_item_form.png

Tigase as an External Component
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

There are cases when you want to deploy one or more Tigase components separately from the main server, or perhaps you want to run some Tigase components connecting to a different XMPP server, or perhaps you work on a component and you do not want to restart the main server every time you make a change.

There is a way to run the Tigase server in *external component mode*. In fact you can run any of Tigase’s components as an external component and connect them to the main XMPP server either via `XEP-0114 <http://xmpp.org/extensions/xep-0114.html>`__ or `XEP-0225 <http://xmpp.org/extensions/xep-0225.html>`__ connection.

Let’s look at the examples…​

Usage with shared database (since version 8.0.0)
'''''''''''''''''''''''''''''''''''''''''''''''''

When you are using Tigase server 8.0.0 or newer in the "external component mode" while using shared default "user repository" and you have main server also running Tigase XMPP Server 8.0.0 or newer, then you can benefit from the remote management of the component connections from the main server. To use that, you need to enable external component and external component manager on the main server by adding following line to the config file:

.. code:: dsl

   'ext' () {}
   'ext-man' () {}

With that in place you can use Admin UI or ad-hoc commands available at ``ext-man`` component of the main server to configure connection details of the servers running in the ``component`` mode.

In Admin UI you click on ``Configuration`` section and select ``Add new item`` at the ``ext-man`` component, which will present you with a following form to fill in external component connectivity details:

|adminui extman add item form|


A Simple Case - MUC as an External Component

A few assumptions:

1. We want to run a MUC component for a domain: ``muc.devel.tigase.org`` and password ``muc-pass``

2. The main server works at an address: devel.tigase.org and for the same virtual domain

3. We want to connect to the server using `XEP-0114 <http://xmpp.org/extensions/xep-0114.html>`__ protocol and port ``5270``.

There is a special configuration type for this case which simplifies setting needed to run Tigase as an external component:

.. code:: dsl

   'config-type' = 'component'

Knowing that we can now create simple configuration file for Tigase XMPP Server:

.. code:: dsl

   admins = [ 'admin@devel.tigase.org' ]
   'config-type' = 'component'
   debug = [ 'server' ]
   'default-virtual-host' = [ 'devel.tigase.org' ]
   dataSource {
       default () {
           uri = 'master_server_default_database_url'
       }
   }
   userRepository {
       default () {}
   }
   authRepository {
       default () {}
   }
   muc (class: tigase.muc.MUCComponent) {}
   ext () {
   }

where ``master_server_default_database_url`` is the same URL as the one used on the main server for default data source.

With that in place we can use ad-hoc commands or Admin UI on the main server to configure Tigase XMPP Server to accept external component connections and to connect from the external component to the master server.

**Adding external component connection settings to the manager (ext-man) using Admin UI.**

|adminui extman add item form external muc|

You need to pass:

-  Domain name - external component domain name (``muc.devel.tigase.org``)

-  Domain password - password for authentication of the external component connection (``muc-pass``)

-  Connection type - ``accept`` to make component wait for connection or ``connect`` force component to connect to the server (``connect``)

-  Port number - port on which component should wait for connection or on which it try to connect (``5270``)

-  Remote host - host to connect to (``devel.tigase.org``)

-  Protocol - id of protocol used for establishing connection

   -  ``XEP-0114: Jabber Component Protocol (accept)`` - establish connection using `XEP-0114: Jabber Component Protocol <https://xmpp.org/extensions/xep-0114.html>`__

   -  ``XEP-0225: Component Connections`` - establish connection using `XEP-0225: Component Connections <https://xmpp.org/extensions/xep-0225.html>`__

Additional options may be left with defaults.

More Components

Suppose you want to run more than one component as an external components within one Tigase instance. Let’s add another - PubSub component to the configuration above and see how to set it up.

The most straightforward way is just to add another component to the server running in the component mode for the component domain

.. code:: dsl

   admins = [ 'admin@devel.tigase.org' ]
   'config-type' = 'component'
   debug = [ 'server' ]
   'default-virtual-host' = [ 'devel.tigase.org' ]
   dataSource {
       default () {
           uri = 'jdbc:derby:/tigasedb'
       }
   }
   userRepository {
       default () {}
   }
   authRepository {
       default () {}
   }
   muc (class: tigase.muc.MUCComponent) {}
   pubsub (class: tigase.pubsub.PubSubComponent) {}
   ext () {}

and then to add new connection domain to the main server external component settings and to the external component manager settings. You basically do the same thing as you did while adding only MUC component as the external component.

Please note however that we are opening two connections to the same server. This can waste resources and over-complicate the system. For example, what if we want to run even more components? Opening a separate connection for each component is a tad overkill.

In fact there is a way to reuse the same connection for all component domains running as an external component. The property ``bind-ext-hostnames`` contains a comma separated list of all hostnames (external domains) which should reuse the existing connection.

There is one catch however. Since you are reusing connections (hostname binding is defined in `XEP-0225 <http://xmpp.org/extensions/xep-0225.html>`__ only), you must use this protocol for the functionality.

Here is an example configuration with a single connection over the `XEP-0225 <http://xmpp.org/extensions/xep-0225.html>`__ protocol used by both external domains:

.. code:: dsl

   admins = [ 'admin@devel.tigase.org' ]
   'bind-ext-hostnames' = [ 'pubsub.devel.tigase.org' ]
   'config-type' = 'component'
   debug = [ 'server' ]
   'default-virtual-host' = [ 'devel.tigase.org' ]
   dataSource {
       default () {
           uri = 'jdbc:derby:/tigasedb'
       }
   }
   ext () {
   }
   userRepository {
       default () {}
   }
   authRepository {
       default () {}
   }
   muc (class: tigase.muc.MUCComponent) {}
   pubsub (class: tigase.pubsub.PubSubComponent) {}

With this configuration you do not need to configure entries in ``ext-man`` for PubSub component, only for MUC component but you need to user ``client`` as the value for protocol field.

Usage with a separate database
''''''''''''''''''''''''''''''

A Simple Case - MUC as an External Component

A few assumptions:

1. We want to run a MUC component for a domain: ``muc.devel.tigase.org`` and password ``muc-pass``

2. The main server works at an address: devel.tigase.org and for the same virtual domain

3. We want to connect to the server using `XEP-0114 <http://xmpp.org/extensions/xep-0114.html>`__ protocol and port ``5270``.

There is a special configuration type for this case which simplifies setting needed to run Tigase as an external component:

.. code:: dsl

   'config-type' = 'component'

This generates a configuration for Tigase with only one component loaded by default - the component used for external component connection. If you use this configuration type, your ``config.tdsl`` file may look like this:

.. code:: dsl

   admins = [ 'admin@devel.tigase.org' ]
   'config-type' = 'component'
   debug = [ 'server' ]
   'default-virtual-host' = [ 'devel.tigase.org' ]
   dataSource {
       default () {
           uri = 'jdbc:derby:/tigasedb'
       }
   }
   userRepository {
       default () {}
   }
   authRepository {
       default () {}
   }
   muc (class: tigase.muc.MUCComponent) {}
   ext () {
   }

To make this new instance connect to the Tigase XMPP Server, you need to create one more file with external connection configuration at ``etc/externalComponentItems`` which will be loaded to the local database and then removed.

.. code:: text

   muc.devel.tigase.org:muc-pass:connect:5270:devel.tigase.org:accept

.. Warning::

    While loading configuration from ``etc/externalComponentItems`` file is supported, we recommend usage of shared database if possible. In future this method may be deprecated.


More Components

Suppose you want to run more than one component as an external components within one Tigase instance. Let’s add another - PubSub component to the configuration above and see how to set it up.

The most straightforward way is just to add another external component connection to the main server for the component domain using Admin UI or ad-hoc command on the main server.

Then we can use following configuration on the server running in the ``component`` mode:

.. code:: dsl

   admins = [ 'admin@devel.tigase.org' ]
   'config-type' = 'component'
   debug = [ 'server' ]
   'default-virtual-host' = [ 'devel.tigase.org' ]
   dataSource {
       default () {
           uri = 'jdbc:derby:/tigasedb'
       }
   }
   userRepository {
       default () {}
   }
   authRepository {
       default () {}
   }
   muc (class: tigase.muc.MUCComponent) {}
   pubsub (class: tigase.pubsub.PubSubComponent) {}
   ext () {
   }

and we need to create a file with configuration for external component connection which will be loaded to the internal database:

.. code:: text

   muc.devel.tigase.org:muc-pass:connect:5270:devel.tigase.org:accept
   pubsub.devel.tigase.org:pubsub-pass:connect:5270:devel.tigase.org:accept

Please note however that we are opening two connections to the same server. This can waste resources and over-complicate the system. For example, what if we want to run even more components? Opening a separate connection for each component is a tad overkill.

In fact there is a way to reuse the same connection for all component domains running as an external component. The property ``bind-ext-hostnames`` contains a comma separated list of all hostnames (external domains) which should reuse the existing connection.

There is one catch however. Since you are reusing connections (hostname binding is defined in `XEP-0225 <http://xmpp.org/extensions/xep-0225.html>`__ only), you must use this protocol for the functionality.

Here is an example configuration with a single connection over the `XEP-0225 <http://xmpp.org/extensions/xep-0225.html>`__ protocol used by both external domains:

.. code:: dsl

   admins = [ 'admin@devel.tigase.org' ]
   'bind-ext-hostnames' = [ 'pubsub.devel.tigase.org' ]
   'config-type' = 'component'
   debug = [ 'server' ]
   'default-virtual-host' = [ 'devel.tigase.org' ]
   dataSource {
       default () {
           uri = 'jdbc:derby:/tigasedb'
       }
   }
   ext () {
   }
   userRepository {
       default () {}
   }
   authRepository {
       default () {}
   }
   muc (class: tigase.muc.MUCComponent) {}
   pubsub (class: tigase.pubsub.PubSubComponent) {}

and example of the external connections configuration file:

.. code:: text

   muc.devel.tigase.org:muc-pass:connect:5270:devel.tigase.org:client

.. |adminui extman add item form| image:: images/admin/adminui_extman_add_item_form.png
.. |adminui extman add item form external muc| image:: images/admin/adminui_extman_add_item_form_external_muc.png

2.9.6. Load Balancing External Components in Cluster Mode
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~



































