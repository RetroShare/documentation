#First Steps

This aims to be a Step by Step Guide for New Users. 

##Download  
Download RetroShare from [here](../user-guide/installation/).

##Install
Install RetroShare on your Computer

##Create new Profile
Start RetroShare to create your Node. 

![create new node](../img/first-steps/create_new_profile.png "Create New Node")  

Select following settings:  
 
 - ![create new profile](../img/first-steps/profile.png "Create New Profile") Create new Profile  
 - ![Advanced Settings](../img/first-steps/advanced.png "Advanced Settings") Advanced Settings  
 - Choose your PGP Size (2048, 3072 or 4096 bits)  
![choose PGP size](../img/first-steps/pgp_size.png "Select PGP Size")  

Enter the values:  

 - Name  
   Name of your Account ([GPG-ID](../user-guide/settings/#public-information)) 
   Visible to your friends, and friends of friends. 
 - Nickname  
   Name of your first Identity ([GXS-ID](../user-guide/interface/#pseudonymous-identities)) 
   Used when you write in chat lobbies, forums and channel comments. Can be setup later if you need one. 
 - Password  
   This password protects your private PGP key. 
   It's wise to choose a long password for your GPG-ID, as this also 
   encrypts your entire RetroShare directory.  
 - Node Name ([Location](../user-guide/settings/#public-information))
   Each user can have several Locations were RetroShare is running on 
   different devices with the same [GPG-ID](../user-guide/settings/#public-information). 

Move your mouse to create randomness for the Key creation. 

![Enter Profile Values](../img/first-steps/enter_profile_values.png "Enter Profile Values")  


Sign your Certificate by entering your Password.  
![Sign your Certificate](../img/first-steps/sign_cert.png "Sign your Certificate")  

##First Start  
When you start RetroShare the first time it's empty, because there is no 
content shared by friends. This will change soon with your first connected Friend. 

![First Start](../img/first-steps/first_start.png "First Start")  

##Initial Settings
Click on the ![Options](../img/first-steps/options.png "Options") Options 
Button to change your ![Network](../img/first-steps/network.png "Network") 
Network Settings  
![Initial Settings](../img/first-steps/initial_settings.png "Initial Settings")  


 - ![NAT Settings](../img/first-steps/nat_settings.png "NAT Settings")  
   Keep your Network Mode at *Public: DHT & Discovery*  
   This will enable DHT and Discovery to improve the connectivity. DHT is 
   also recommended to use, because it provides [Hole Punching](https://en.wikipedia.org/wiki/UDP_hole_punching) 
   and [NAT-PMP](https://en.wikipedia.org/wiki/NAT_Port_Mapping_Protocol) 
   technics to open a port in your firewall. 
 - ![Network Mode](../img/first-steps/network_mode.png "Network Mode")  
   If your Router is enabling [UPnP](https://en.wikipedia.org/wiki/Universal_Plug_and_Play), 
   keep UPnP. UPnP enables RetroShare to open itself a port on your Router. 
   Otherwise change it to *Manually Forwarded Port* and set a manual Port Forward to your 
   [NAT](../user-guide/settings/#nat) Firewall. For manual Port forward, 
   you can choose your RetroShare port also.  
 - Set your download and upload speeds to fit your Internet Connection. 
   Keeping this setting below of your total speed is recommended.  
   
For detailed Network Settings explanations click [here](../user-guide/settings/#network)

###Avatar

![empty Avatar](../img/first-steps/empty_avatar.png "Empty Avatar")  

You may want to change the Avatar of your Location and set a Status message.  

![Avatar](../img/first-steps/avatar.png "Avatar")  
<sub>Click on the avatar to change it.</sub>  

![Status](../img/first-steps/status.png "Status")  
<sub>Click on the message to change it.</sub>  

![avatar and status](../img/first-steps/avatar_status.png "Avatar and Status")  

###Identity
![People](../img/first-steps/people.png "People")  

RetroShare has already created a first [signed Identity](../user-guide/interface/#pseudonymous-identities) 
for your use in [Chatrooms](../user-guide/interface/#chat-lobbies) 
and [Forums](../user-guide/interface/#forums) and Distant Chats and Mails. 

You may want to create as many additional Identities as well if needed. 

![Identity](../img/first-steps/identity.png "signed Identity") 

To change the Avatar of your Identity right click it.  
![Edit Identity](../img/first-steps/edit_id.png "Edit Identity")  

![Edit Identity](../img/first-steps/edit_identity.png "Edit Identity")  

And change your avatar picture. 

![Edit Identity](../img/first-steps/id.png "Edit Identity")  


##First Friend
![Invite](../img/first-steps/invite.png "Invite")  

Click on the ![Invite](../img/first-steps/invite_40.png "Invite")   Invite Button. 

The fastest way is to exchange the certificates directly with your friends. 
You can also export them to a file and hand them out manually or send it by mail. 

It's important to accept each other vice versa. Your friend must add your 
certificate to his Network/Friendlist. And you need to add the certificate from 
your Friend to your Network/Friendlist.  
![Connect Wizard](../img/first-steps/connect_wizard.png "Connect Wizard")  

 - ![Copy to Clipborad](../img/first-steps/copyrslink.png "Copy to Clipboard") copy to clipboard  
 - ![Save to File](../img/first-steps/document_save.png "Save to File") save to file  
 - ![Send by Mail](../img/first-steps/mail_send.png "Send by Mail") send by mail  

![Show Certificate](../img/first-steps/show_cert.png "Show Certificate")  

Share your certificate with your friend and request the certificate from 
your Friend.  

Accept your Friend's certificate.  
![Accept Certificate](../img/first-steps/accept_cert.png "Accept Certificate")  


Have a look at the details and finish.  
![Make Friend](../img/first-steps/make_friend.png "Make Friend")  

Connection in Progress, your Node tries to connect to your Friend. 
![Connection in Progress](../img/first-steps/connection_progress.png "Connection in Progress")  

Your connect attempt has been successful, the connection is established. 
![Connection in Established](../img/first-steps/connection_established.png "Connection in Established")  


##First Chat
Your online Contacts(Friend Nodes) will be listed in the Network Tab. 
![Friendlist](../img/first-steps/friendlist.png "Friendlist")  

Double Clicking will start an instant Chat with your Friends. 
![Instant Chat](../img/first-steps/instant.png "Instant Chat")  

##First Chatroom
Subscribed [Chatrooms](../user-guide/interface/#chat-lobbies) 
from your online friends are shared to you, 
and you are free to subscribe and re-share them as well to your friends.  
![Chatroom](../img/first-steps/chatroom.png "Chatroom")  

In the same manner ![Forums](../img/first-steps/forums.png "Forums") [Forums](../user-guide/interface/#forums), 
![Channels](../img/first-steps/channels.png "Channels") [Channels](../user-guide/interface/#channels), 
![Posted](../img/first-steps/posted.png "Posted") [Posted](../user-guide/interface/#posted) and 
![File Sharing](../img/first-steps/filesharing.png "File Sharing") [File Sharing](../user-guide/interface/#file-sharing) 
will become more and more available per direct 
[Friend-2-Friend](../concept/Friend-2-Friend/#retroshare) 
connections as 
[**your network**](../concept/topology/#retroshare) grows.  
