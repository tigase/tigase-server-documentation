
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

   **Note**

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

   **Important**

   You should always run the latest point/bugfix release of the recommended JDK.

   **Note**

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

..

   **Tip**

   Do not run as root user!


Start the Server
~~~~~~~~~~~~~~~~~

   **Note**

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

   **Note**

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

..

   **Note**

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

   **Note**

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
''''''''''''''''''''''

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

2.5.6. Tigase Server Network Instructions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

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

..

   **Note**

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

   **Note**

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

   =============================================================================
     Configuration file etc/init.properties was converted to DSL format.
     Previous version of a configuration file was saved at etc/init.properties.old
   =============================================================================


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

..

   **Warning**

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
In previous Tigase XMPP Server releases configuration was stored in properties based configuration file.
From Tigase XMPP Server 8.0.0 release it will be required to use new DSL based configuration file format. This file format was inspired by Groovy language syntax and new core feature of Tigase XMPP Server - Tigase Kernel Framework.

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

To illustrate it better let's start with a simple example. In properties file in order to configure PubSub component named '`pubsub`' you would use following properties:

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


in which we define bean with name `pubsub` and set it's class inside `()` block to `tigase.pubsub.PubSubComponent`.
We also use block between `{}` chars to define properties which are related to bean.
Which means this properties will be passed only to this instance of Tigase PubSub Component, same as it was before where we needed to add prefix.
Entries after `\#` are comments, to pass `#` you need to wrap whole part containing it in `''`, ie. `'test#242'`

WARNING: If a string value assigned to a property contains any char from a following list `=:,[]#+-*/` it needs to be wrapped in a `''`.

Why DSL?
~~~~~~~~

DSL configuration format provides a number of advantages over the old system of configuration.
. All configurations for components are related in a single block, so they are not spread out over several different lines.
. No need for long property names, no longer have to invoke a long string of settings for multiple values.
. Support is provided for environment variables.
. No longer need to escape certain characters, making settings far more readable at a glance.
. Values may be set using basic calculations, such as `100 * 200 * 2` rather than `40000`.
. Parameter type values are no longer necessary, no more [i], [S], [B] etc..
. Comma separated values can now be simplified lists with separate entries being able to be in multiple lines.

Although the format may seem more complex, looking like a section of java code, the formatting is consistent and can be far more readable.
After some experience with DSL format, you'll find it's far more intuitive and user friendly than it may appear. Of course if there's any real confusion, Tigase can automatically convert old style properties files to the DSL format using the following command:
[source,bash]

.. code-block:: bash

   ./scripts/tigase.sh upgrade-config etc/tigase.conf

Setting property
'''''''''''''''''

To set property you just write property name followed by `=` and value to set. This is always done in context of bean which configuration property you want to set.

::

   test=true

It is also possible to set property in main context by placing property outside of any context.
This sets property which value is available to access by any bean.

Setting global property
''''''''''''''''''''''''
Like in properties file it is still possible to use property names starting with `--` without any context or any other properties at global scope.
Format is the same as in case of setting property but they are defined without scope (in global scope).
This properties are global and accessible by any bean but also set as system property in JVM.

Defining bean
''''''''''''''

You can configure bean by using following format:


.. code:: bash

   beanName (class: className, active: activeValue, exportable: exportableValue) {
       # scope of bean properties
   }

where `beanName` is name under which you want to configure bean.
`beanName` must be wrapped in `''`, if `beanName` contains characters like `=:,[]#+-*/` and is recommended, if `beanName` is numeric only.

Inside block between `(` and `)` you can define:

* `class` which will be used as a bean, in example above we set class as `className`. *_(default: if you try to configure bean under name which has default class assigned with it in Tigase framework then this assigned class will be used. In other case you need to pass name of class to use as a bean)_*
* `active` (boolean) whether you want the bean to be active or not (beans with `active` set to `false` are not loaded). *_(default: true)_*
* `exportable` (boolean) defines if this bean should be exported and available for use for beans in inner scopes. This is advanced option in most cases it is recommended to omit this field in configuration. *_(default: false)_*

Spaces between `beanName` and block between `()` is optional as well as space between block `()` and block `{}`.
It is recommended that properties of bean would be placed in separate lines with indentation and first property will be placed in new line.

.. important::

   Usage of `()` block is very important. When this block is used in configuration it automatically sets `active` property of bean definition for bean for which it is used to to `true`. This is done due to fact that default value of `active` is `true`.

   If you omit it in configuration, you will set bean configuration but it may remain `inactive`. In this state bean will not be loaded and as a result will not be used by Tigase XMPP Server.


Configuring bean
'''''''''''''''''
If you know that bean is defined and you do not want to change it's activity or class then you can just pass properties to configure bean in following way:

::

   beanName {
       # scope of bean properties
       test = true
   }


where `beanName` is name of bean to configure and `test` is name of property to set to `true` in this bean.

Format of values
'''''''''''''''''

In properties based configuration file every property was defined as a string and only by defining expected format it was properly converted to expected value. In DSL it is possible to set values in two ways:

as an object
   Using this format you set list as a list and integer is set as an integer.

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

::

   user {
     name = env('USER')
     home = prop('user.home')
     paths = [ prop('user.home'), prop('user.dir') ]
   }

..

      **Warning**

   For properties which accepts lists it is not allowed to set value using variable/property with comma separated values like ``value1,value2`` wrapped in ``[]``, ie. ``property = [ env('some-variable') ]``. It needs to be set in following way ``property = env('some-variable')``
 
Computed values
''''''''''''''''

With DSL configuration format we introduce support for computable values for properties. It is now possible to set value which is result of a computation, ie. concatenation of a strings or very simple mathematical expression. We currently support only following mathematical operations:

-  add

-  subtract

-  multiply

-  divide

**Example of setting environment variable related path and computed timeout.**

::

   bean {
     # setting path to `some-subdirectory` of user home directory
     path = prop('user.home') + '/some-subdirectory/'

     # setting timeout to 5 minutes (setting value in milliseconds)
     timeout = 5L * 60 * 1000
     # previously it would need to be configured in following way:
     # timeout = 300000L
   }

..

   **Warning**

   For properties which accepts lists it is not allowed to set value using computed values with comma separated values like ``value1,value2`` wrapped in ``[]``, ie. ``property = [ env('some-variable') + ',other-value' ]``. It needs to be set in following way ``property = env('some-variable') + ',other-value'``.

.. _periodDurationValues:

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

   **Note**

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

**Note! Tigase requires full certificate chain in PEM file (described above)! Different applications may require pem file with certificates and private key in different order. So the same file may not be necessarily used by other services like Web server or e-mail server. Currently, Tigase can automatically sort certificates in PEM file while loading it.**


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

   **Note**

   Tigase tries to be *smart* and automatically detects wildcard domain and alternative domains so it’s not needed to duplicate same certificate in multiple files to match domains - same file will be loaded and make available for all domains (CNames) available in the certificate.



