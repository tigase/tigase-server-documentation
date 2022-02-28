
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

This Article Describes How to use tigase.im Service for Instant Communications
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

You have to install and run a Jabber client application to use the service.

There are multiple domains available: tigase.im, sure.im, xmpp.cloud (and you can host your own domain as well)

Short instructions:
~~~~~~~~~~~~~~~~~~~

Usually you just need to enter the user name of the form: user@tigase.im. Your XMPP client should take care of all other things as our service doesn’t need any special settings. If you don’t have an account on tigase.im server yet just tick the option to register new account. That’s it!

**Long Instructions:**

Good news is that there are many programs to choose from which allow you to communicate through our server. So you can pick up your favorite application or use an existing one that is compatible and start using our service.

All clients presented below support multiple accounts on Jabber servers. What this means is that you can have a few Jabber accounts on different Jabber servers and you can still use just one program to connect to all of them at the same time.

The "full list of all known XMPP<https://xmpp.org/software/clients/>"_ clients is very long. You can obviously try them all but below is a selection which is recommended by the Tigase team. The selected programs might not be the best choice for you, but these programs have been tested and we can offer help with using them. Here is a list of recommended instant messaging clients:

- Beagle.im - macOS desktop client developed by Tigase team supporting all the latest and greatest features

- Tigase Messenger for iOS - lightweight, powerful XMPP client developed by Tigase, Inc. It provides an easy way to start using the XMPP Protocol (formerly known as Jabber) if you’ve never used it before. Veterans of the protocol will find many features here they are familiar with along with enhancements to reduce data use and extend battery life.

- Tigase Messenger for Android - mobile chat client to use with XMPP services and servers. The totally revamped v3.0 now has new features, a better design, and Google integration.
  Application supports any XMPP server, from free services like sure.im or Tigase.im, to a server you may host on your own.

- tigase.im[Tigase.im] - web-based client allowing to easily chat with friends independently of platform.

- Psi Pure Jabber client. Although it supports only Jabber network it is a very user friendly and comfortable program. It works on most popular operating systems like Linux, MS
  Windows, and Apple MacOS X.

- Gajim This is another Jabber only client. Very user friendly and works on most of Linux distributions, FreeBSD, and MS Windows.

- Pidgin (previously Gaim) This is not just a Jabber client. This type of application is called multicommunicator as apart from Jabber it supports many other instant messaging
  networks/protocols such as: AIM/ICQ, MSN, Yahoo, Gadu-Gadu, IRC, and a few others. So it is especially convenient if you have friends using other messaging networks. Pidgin works on most Linux distributions, and on MS Windows.

- Kopete This is a KDE component and although it only works on Linux based system it also supports many of the most popular instant messaging protocols apart from Jabber like: AIM,
  Gadu-Gadu, ICQ, IRC, MSN, Yahoo.

Install the Jabber client of your choice and set up for a Tigase account:

2.1.3. Configuration instructions for Psi
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Psi - Initial configuration
~~~~~~~~~~~~~~~~~~~~~~~~~~~
The first time you run Psi you see a screen like this:

.. image:: image/psi-first-run.png

To connect to tigase.org server we need to configure the program. Below are step-by-step instructions for novice users on how to setup Psi.

1. Psi can connect to many Jabber servers at the same time so we have to identify each connection somehow. The first thing to do is assign a name to the connection we just created.
   As we are going to define connection to tigase.org server let’s just name it: **Tigase**.
   .. image:: image/psi-add-account.png

   **Note!** At the moment you can register an account through the Web site only. This is a single account for both services: The Drupal website and Jabber/XMPP service on the tigase.org domain. If you want to have a Jabber account on the tigase.org server go to the registration page, un-tick "Register new account", and go to the point no 5. You can use guide points 2-4 to register a Jabber account on any other Jabber server.

2. When you press the Add button you will see next window where you can enter your Jabber account details:
   .. image:: image/psi-register-account-empty.png

3. Invent your user name for the account on Tigase server. Let’s assume your user name is: **frank**. Jabber ID’s however consist of 2 parts - your user name and server address.
    Exactly the same as an e-mail address. As you are registering an account on tigase.org server, you will have to enter in this field: **frank@tigase.org**. Next enter the password of your choice and click the Register button.
     .. image:: image/psi-register-account-nossl.png

4. On successful registration you will receive a confirmation message and you should see a window like this:
   .. image:: image/psi-register-account-success.png
    
    It may happen that somebody earlier registered an account with the same name you’ve selected for yourself. If so, you will receive error message. You will then have to select another user name and try to register again.

5. After clicking the **OK** button you will see a window with your connection and account setup. You can stick with default values for now.
   .. image:: image/psi-after-registration.png
   Just click the **Save** button and this window closes.

6. Now you have your account configured and ready to use but you are still off-line. You can find out whether you are on-line or off-line by looking at the bottom of main Psi
   window. There you can see **Offline** text.

  Click on this **Offline** text and you will see a list of possible options. Just select **Online**.
  .. image:: image/psi-first-run.png
  Now you are connected!

Well, you are now connected but how to talk to other people? How to add friends to the contact list? You can send a message to your friends straight away using the **Psi menu** option *8New blank message**. It is much more convenient however, if you could see which of your friends is online and available for chatting and if you could start talking to your friend just by clicking on his name.

Short Instructions How to Add Your First Contact
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

1. Click on Psi menu - the button next to the Online text. You will see something like this:
  .. image:: image/psi-menu.png
  From all menu options select the top one - Add a contact:
  .. image:: image/psi-menu-add-contact.png

2. The next window will display where you can enter your contact details:
  .. image:: image/psi-add-user-empty.png
  You have to know the Jabber ID of the person you want to add to your contact list. Let’s assume, for example, you want to add Tigase server administrator’s Jabber ID to your contact list. So, after you enter these details the window will look like this:
  .. image:: image/psi-add-user-filled.png
  Click the **Add** button.

3. Now you will see a confirmation window that a new person has been added to your contact list:
  .. image:: image/psi-kobit-added.png
  But there is more behind the scenes. Adding a contact to your **Roster** (contact list) usually means you can see whether the person is online and available to talk or not. The person however, may not wish you to see his presence. So, to make sure the other person accepts you as a friend Psi sent a request to the address you just entered with the question of whether he agrees to show his presence to you.

  You won’t be able to see the users availability until he sends confirmation.

4. Once the other user sends confirmation back, you will usually receive 2 system events:
  .. image:: image/psi-kobit-auth-received.png

5. Click on the contact to see a window with these messages:
  .. image:: image/psi-authorized-window.png

6. One message just says you have been authorized by the other user:
  .. image:: image/psi-authorized-window-2.png
  So you simply click **Next** to see the second message.

7. The second message is a bit more interesting. It contains the question of whether you also authorize the other user to see your presence. If you want to accept this request just
   click **Add/Auth**.
   .. image:: image/psi-authorized-window-3.png

8. Finally main Psi window with your new contact:
  .. image:: image/psi-kobit-added-authorized.png

Well done!

You are ready to start Jabbering. Good luck.

Where to go next? For detailed Psi documentation refer to the program Wiki page: http://psi-im.org/wiki/Main_Page

Welcome to the Tigase Administration Guide.

2.2. About Tigase XMPP Server
-----------------------------

**Tigase XMPP Server** is an **Open Source and Free (AGPLv3)** Java based server. The goals behind its design and implementation of the server are:

  1.Make the server robust and reliable.

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

2.2.2. Securit
^^^^^^^^^^^^^^

There are a few elements of the security related to XMPP servers: secure data transmissions which is met by the implementation of **SSL or **TLS** protocol, secure user authorization which is met by the implementation of **DIGEST** or **SASL** user authorization and secure deployment which is met by component architecture.

**Secure deployment** Tigase software installation does not impact network security. Companies usually have their networks divided into 2 parts: **DMZ** which is partially open to the outside world and the **Private network** which is closed to the outside world.

If the XMPP server is to provide an effective way of communication between company employees regardless if they are in a secure company office or outside (perhaps at a customer site), it needs to accept both internal and external connections. So the natural location for the server deployment is the **DMZ**. However, this solution has some considerations: each company has normally established network users base and integrated authorization mechanisms. However, that information should be stored outside the DMZ to protect internal security, so how to maintain ease of installation and system security?

**Tigase server** offers a solution for such a case. With it’s component structure, Tigase can be easily deployed on any number machines and from the user’s point of view it is seen as a one logical XMPP server. In this case we can install a Session Manager module in the **private** network, and a Client Connection Manager with Server Connection Manager in the **DMZ**.

Session Manager connects to **DMZ** and receives all packets from external users. Thus is can securely realize users authorization based on company authorization mechanisms.

2.2.3. Flexibility
^^^^^^^^^^^^^^^^^^
There are many different XMPP server implementations. The most prevalent are:

- Used as a business communication platform in small and medium companies where the server is not under a heavy load. For such deployments security is a key feature.

- For huge community websites or internet portal servers is, on the other hand, usually under very heavy load and has to support thousands or millions of simultaneous connections. For such a deployment we need a different level of security as most of the service is open to the public.

- For very small community deployments or for small home networks the key factor is ease to deploy and maintain.

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

Based on XEP-0387: 'XMPP Compliance Suites 2018<https://xmpp.org/extensions/xep-0387.html>"_

Core Compliance Suite
~~~~~~~~~~~~~~~~~~~~~

.. list-table:: Table 1. Core Compliance Suite
  :align: left

* - Support
  - Specification
  - Name
  - Comment
* - ✓
  - 'RFC6120<https://datatracker.ietf.org/doc/html/rfc6120>'_
  - Extensible Messaging and Presence Protocol (XMPP): Core
  - 
* - ✓
  - 'RFC7622<https://datatracker.ietf.org/doc/html/rfc7622>'_
  - Extensible Messaging and Presence Protocol (XMPP): Address Format
  - We support previous version of the specification: RFC6122
  * - ✓
  - 'RFC7590<https://datatracker.ietf.org/doc/html/rfc7590>'_
  - Use of Transport Layer Security (TLS) in the Extensible Messaging and Presence Protocol (XMPP)
  - 
* - ✓
  - 'XEP-0368<https://xmpp.org/extensions/xep-0368.html>'_
  - SRV records for XMPP over TLS
  - Requires adding DNS entries pointing to port 5223
* - ✓
  - 'XEP-0030<https://xmpp.org/extensions/xep-0030.html>'_
  - Service Discovery
  - 
* - ✓
  - 'XEP-0115<https://xmpp.org/extensions/xep-0115.html>'_
  - Entity Capabilities
  - 
* - ✓
  - 'XEP-0114<https://xmpp.org/extensions/xep-0114.html>'_
  - Jabber Component Protocol
* - ✓
  - 'XEP-0163<https://xmpp.org/extensions/xep-0163.html>'_
  - Personal Eventing Protocol
  - 

Web Compliance Suite
~~~~~~~~~~~~~~~~~~~~~
.. list-table:: Table 2. Web Compliance Suite
  :align: left

* - Support
  - Specification
  - Name
  - Comment
* - ✓
  - 'RFC7395<https://datatracker.ietf.org/doc/html/rfc7395>'_
  - An Extensible Messaging and Presence Protocol (XMPP) Subprotocol for WebSocket
  - 
* - ✓
  - 'XEP-0206<https://xmpp.org/extensions/xep-0206.html>'_
  - XMPP Over BOSH
    - 
* - ✓
  - 'XEP-0124<https://xmpp.org/extensions/xep-0124.html>'_
  - Bidirectional-streams Over Synchronous HTTP (BOSH)
  - 

IM Compliance Suite
~~~~~~~~~~~~~~~~~~~~~
.. list-table:: Table 3. Web Compliance Suite
  :align: left

* - Support
  - Specification
  - Name
  - Comment
* - ✓
  - RFC6120
  - Extensible Messaging and Presence Protocol (XMPP): Instant Messaging and Presence
    - 
* - ✓
  - XEP-0084
  - User Avatar
  - 
* - ✓
  - XEP-0153
  - vCard-Based Avatars
  - 
* - ✓
  - XEP-0054
  - vcard-temp
  - 
* - ✓
  - XEP-0280
  - Message Carbons
  - 
* - ✓
  - XEP-0191
  - Blocking Command
  - 
* - ✓
  - XEP-0045
  - Multi-User Chat
  - 
* - ✓
  - XEP-0249
  - Direct MUC Invitations
  - 
* - ✓
  - XEP-0048
  - Bookmarks
  - 
* - ✓
  - XEP-0223
  - Persistent Storage of Private Data via PubSub
  - 
* - ✓
  - XEP-0049
  - Private XML Storage
  - 
* - ✓
  - XEP-0198
  - Stream Management
  - Both Session Resumption and Stanza Acknowledgements
* - ✓
  - XEP-0313
  - Message Archive Management
  - 
Mobile Compliance Suite
~~~~~~~~~~~~~~~~~~~~~~~~
.. list-table:: Table 4. Web Compliance Suite
  :align: left

* - Support
  - Specification
  - Name
  - Comment

* - ✓
  - RFC7395
  - An Extensible Messaging and Presence Protocol (XMPP) Subprotocol for WebSocket
  - 
* - ✓
  - XEP-0198
  - Stream Management
  - Both Session Resumption and Stanza Acknowledgements
* - ✓
  - XEP-0352
  - Client State Indication
  - 
* - ✓
  - XEP-0357
  - Push Notifications
  - 
Non-Compliance Suite Extensions
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
.. list-table:: Table 5. Core Compliance Suite
  :align: left

* - Support
  - Specification
  - Name
  - Comment
  - ✓
  - XEP-0004
  - Data Forms
  - 
  - ✓
  - XEP-0008
  - IQ-Based Avatars
  - 
  - ✓
  - XEP-0012
  - Last Activity
  - 
  - ✓
  - XEP-0013
  - Flexible Offline Message Retrieval
✓
XEP-0016
Privacy Lists
✓
XEP-0020
Feature Negotiation
✓
XEP-0022
Message Events
✓
XEP-0047
In-Band Bytestreams
✓
XEP-0050
Ad-Hoc Commands
✓
XEP-0059
Result Set Management
✓
XEP-0060
Publish-Subscribe
✓
XEP-0065
SOCKS5 Bytestreams
✓
XEP-0066
Out of Band Data
✓
XEP-0068
Field Standardization for Data Forms
✓
XEP-0071
XHTML-IM
✓
XEP-0072
SOAP Over XMPP
✓
XEP-0077
In-Band Registration
✓
XEP-0078
Non-SASL Authentication
✓
XEP-0079
Advanced Message Processing
✓
XEP-0080
User Location
✓
XEP-0082
XMPP Date and Time Profiles
✓
XEP-0083
Nested Roster Groups
✓
XEP-0085
Chat State Notifications
✓
XEP-0086
Error Condition Mappings
✓
XEP-0091
Legacy Delayed Delivery
✓
XEP-0092
Software Version
✓
XEP-0096
File Transfer
✓
XEP-0100
Gateway Interaction
✓
XEP-0106
JID Escaping
✓
XEP-0107
User Mood
Server support via Personal Eventing Protocol (XEP-0163)
✓
XEP-0108
User Activity
Server support via Personal Eventing Protocol (XEP-0163)
✓
XEP-0118
User Tune
Server support via Personal Eventing Protocol (XEP-0163)
✓
XEP-0127
Common Alerting Protocol (CAP) Over XMPP
✓
XEP-0128
Service Discovery Extensions
✓
XEP-0131
Stanza Headers and Internet Metadata (SHIM)
✓
XEP-0133
Service Administration
✓
XEP-0136
Message Archiving
✓
XEP-0141
Data Forms Layout
✓[1]
XEP-0142
Workgroup Queues
✓
XEP-0144
Roster Item Exchange
✓
XEP-0145
Annotations
✓
XEP-0146
Remote Controlling Clients
✓
XEP-0152
Reachability Addresses
✓
XEP-0155
Stanza Session Negotiation
✓
XEP-0156
Discovering Alternative XMPP Connection Methods
Uses DNS records, so will work with Tigase XMPP Server
✓
XEP-0157
Contact Addresses for XMPP Services
✓
XEP-0160
Best Practices for Handling Offline Messages
✓
XEP-0166
Jingle
✓
XEP-0167
Jingle RTP Sessions
✓
XEP-0170
Recommended Order of Stream Feature Negotiation
✓
XEP-0171
Language Translation
✓
XEP-0172
User Nickname
✓
XEP-0174
Serverless Messaging
✓
XEP-0175
Best Practices for Use of SASL ANONYMOUS
✓
XEP-0176
Jingle ICE-UDP Transport Method
✓
XEP-0177
Jingle Raw UDP Transport Method
✓
XEP-0178
Best Practices for Use of SASL EXTERNAL with Certificates
✓
XEP-0179
Jingle IAX Transport Method
✓
XEP-0180
Jingle Video via RTP
✓
XEP-0181
Jingle DTMF
✓
XEP-0184
Message Receipts
✓
XEP-0185
Dialback Key Generation and Validation
✓
XEP-0190
Best Practice for Closing Idle Streams
✓
XEP-0199
XMPP Ping
✓
XEP-0201
Best Practices for Message Threads
✓
XEP-0202
Entity Time
✓
XEP-0203
Delayed Delivery
✓
XEP-0205
Best Practices to Discourage Denial of Service Attacks
✓
XEP-0209
Metacontacts
✓
XEP-0220
Server Dialback
✓
XEP-0224
Attention
✓
XEP-0225
Component Connections
✓
XEP-0226
Message Stanza Profiles
✓
XEP-0231
Bits of Binary
✓
XEP-0234
Jingle File Transfer
✓
XEP-0245
The /me Command
✓
XEP-0246
End-to-End XML Streams
✓
XEP-0247
Jingle XML Streams
✓
XEP-0250
C2C Authentication Using TLS
✓
XEP-0251
Jingle Session Transfer
✓
XEP-0260
Jingle SOCKS5 Bytestreams Transport Method
✓
XEP-0261
Jingle In-Band Bytestreams Transport
✓
XEP-0262
Use of ZRTP in Jingle RTP Sessions
✓
XEP-0277
Microblogging over XMPP
✓
XEP-0292
vCard4 Over XMPP
✓
XEP-0301
In-Band Real Time Text
✓
XEP-0305
XMPP Quickstart
✓
XEP-0323
Internet of Things - Sensor Data
✓
XEP-0324
Internet of Things - Provisioning
✓
XEP-0325
Internet of Things - Control
✓
XEP-0326
Internet of Things - Concentrators
✓
XEP-0333
Chat Markers
✓
XEP-0363
HTTP File Upload
✓
XEP-0387
XMPP Compliance Suites 2018
Full, ordered list of supported RFCs and XEPs:
Support
Specification
Name
Comment
✓
RFC6120
Extensible Messaging and Presence Protocol (XMPP): Core
✓
RFC6120
Extensible Messaging and Presence Protocol (XMPP): Instant Messaging and Presence
⍻
RFC7622
Extensible Messaging and Presence Protocol (XMPP): Address Format
We support previous version of the specification: RFC6122
✓
RFC7395
An Extensible Messaging and Presence Protocol (XMPP) Subprotocol for WebSocket
✓
RFC7395
An Extensible Messaging and Presence Protocol (XMPP) Subprotocol for WebSocket
✓
RFC7590
Use of Transport Layer Security (TLS) in the Extensible Messaging and Presence Protocol (XMPP)
✓
XEP-0004
Data Forms
✓
XEP-0008
IQ-Based Avatars
✓
XEP-0012
Last Activity
✓
XEP-0013
Flexible Offline Message Retrieval
✓
XEP-0016
Privacy Lists
✓
XEP-0020
Feature Negotiation
✓
XEP-0022
Message Events
✓
XEP-0030
Service Discovery
✓
XEP-0045
Multi-User Chat
✓
XEP-0047
In-Band Bytestreams
✓
XEP-0048
Bookmarks
✓
XEP-0049
Private XML Storage
✓
XEP-0050
Ad-Hoc Commands
✓
XEP-0054
vcard-temp
✓
XEP-0059
Result Set Management
✓
XEP-0060
Publish-Subscribe
✓
XEP-0065
SOCKS5 Bytestreams
✓
XEP-0066
Out of Band Data
✓
XEP-0068
Field Standardization for Data Forms
✓
XEP-0071
XHTML-IM
✓
XEP-0072
SOAP Over XMPP
✓
XEP-0077
In-Band Registration
✓
XEP-0078
Non-SASL Authentication
✓
XEP-0079
Advanced Message Processing
✓
XEP-0080
User Location
✓
XEP-0082
XMPP Date and Time Profiles
✓
XEP-0083
Nested Roster Groups
✓
XEP-0084
User Avatar
✓
XEP-0085
Chat State Notifications
✓
XEP-0086
Error Condition Mappings
✓
XEP-0091
Legacy Delayed Delivery
✓
XEP-0092
Software Version
✓
XEP-0096
File Transfer
✓
XEP-0100
Gateway Interaction
✓
XEP-0106
JID Escaping
✓
XEP-0107
User Mood
Server support via Personal Eventing Protocol (XEP-0163)
✓
XEP-0108
User Activity
Server support via Personal Eventing Protocol (XEP-0163)
✓
XEP-0114
Jabber Component Protocol
✓
XEP-0115
Entity Capabilities
✓
XEP-0118
User Tune
Server support via Personal Eventing Protocol (XEP-0163)
✓
XEP-0124
Bidirectional-streams Over Synchronous HTTP (BOSH)
✓
XEP-0128
Service Discovery Extensions
✓
XEP-0127
Common Alerting Protocol (CAP) Over XMPP
✓
XEP-0131
Stanza Headers and Internet Metadata (SHIM)
✓
XEP-0133
Service Administration
✓
XEP-0136
Message Archiving
✓
XEP-0141
Data Forms Layout
✓
XEP-0142
Workgroup Queues
✓
XEP-0144
Roster Item Exchange
✓
XEP-0145
Annotations
✓
XEP-0146
Remote Controlling Clients
✓
XEP-0152
Reachability Addresses
✓
XEP-0153
vCard-Based Avatars
✓
XEP-0155
Stanza Session Negotiation
✓
XEP-0156
Discovering Alternative XMPP Connection Methods
Uses DNS records, so will work with Tigase XMPP Server
✓
XEP-0157
Contact Addresses for XMPP Services
✓
XEP-0160
Best Practices for Handling Offline Messages
✓
XEP-0163
Personal Eventing Protocol
✓
XEP-0166
Jingle
✓
XEP-0167
Jingle RTP Sessions
✓
XEP-0170
Recommended Order of Stream Feature Negotiation
✓
XEP-0171
Language Translation
✓
XEP-0172
User Nickname
✓
XEP-0174
Serverless Messaging
✓
XEP-0175
Best Practices for Use of SASL ANONYMOUS
✓
XEP-0176
Jingle ICE-UDP Transport Method
✓
XEP-0177
Jingle Raw UDP Transport Method
✓
XEP-0178
Best Practices for Use of SASL EXTERNAL with Certificates
✓
XEP-0179
Jingle IAX Transport Method
✓
XEP-0180
Jingle Video via RTP
✓
XEP-0181
Jingle DTMF
✓
XEP-0184
Message Receipts
✓
XEP-0185
Dialback Key Generation and Validation
✓
XEP-0190
Best Practice for Closing Idle Streams
✓
XEP-0191
Blocking Command
✓
XEP-0198
Stream Management
Both Session Resumption and Stanza Acknowledgements
✓
XEP-0199
XMPP Ping
✓
XEP-0201
Best Practices for Message Threads
✓
XEP-0202
Entity Time
✓
XEP-0203
Delayed Delivery
✓
XEP-0205
Best Practices to Discourage Denial of Service Attacks
✓
XEP-0206
XMPP Over BOSH
✓
XEP-0209
Metacontacts
✓
XEP-0220
Server Dialback
✓
XEP-0223
Persistent Storage of Private Data via PubSub
✓
XEP-0224
Attention
✓
XEP-0225
Component Connections
✓
XEP-0226
Message Stanza Profiles
✓
XEP-0231
Bits of Binary
✓
XEP-0234
Jingle File Transfer
✓
XEP-0245
The /me Command
✓
XEP-0246
End-to-End XML Streams
✓
XEP-0247
Jingle XML Streams
✓
XEP-0249
Direct MUC Invitations
✓
XEP-0250
C2C Authentication Using TLS
✓
XEP-0251
Jingle Session Transfer
✓
XEP-0260
Jingle SOCKS5 Bytestreams Transport Method
✓
XEP-0261
Jingle In-Band Bytestreams Transport
✓
XEP-0262
Use of ZRTP in Jingle RTP Sessions
✓
XEP-0277
Microblogging over XMPP
✓
XEP-0280
Message Carbons
✓
XEP-0292
vCard4 Over XMPP
✓
XEP-0301
In-Band Real Time Text
✓
XEP-0305
XMPP Quickstart
✓
XEP-0313
Message Archive Management
✓
XEP-0323
Internet of Things - Sensor Data
✓
XEP-0324
Internet of Things - Provisioning
✓
XEP-0325
Internet of Things - Control
✓
XEP-0326
Internet of Things - Concentrators
✓
XEP-0333
Chat Markers
✓
XEP-0352
Client State Indication
✓[1]
XEP-0357
Push Notifications
✓
XEP-0363
HTTP File Upload
✓
XEP-0368
SRV records for XMPP over TLS
Requires adding DNS entries pointing to port 5223
✓
XEP-0387
XMPP Compliance Suites 2018
