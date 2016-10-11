#Interface

##News-Feed
![news feed interface](../img/interface/newsfeed.png "Newsfeed")  

The News Feed diplays the last events on your network, 
sorted by the time you received them. 
This gives you a summary of the activity of your friends. 
You can configure which events to show by pressing on [Options](../user-guide/settings/#notify).  

The various events shown are:  

 - Connection attempts (useful to make friends with new people and cotnrol who's trying to reach you)
 - Channel and Forum posts
 - New Channel and Forums you can subscribe to 
 - Private messages from your friends

![news feed example](../img/interface/newsfeed/feed.png "Newsfeed Example")  
This shows an entry in the newsfeed because a friend came online, 
and this friend sent a message. 


##Network
![network interface](../img/interface/network.png "Network")  
The Network tab shows your friend RetroShare nodes: the neighbor RetroShare nodes that are connected to you.  
You can group noed together to allow a finer level of information access, for instance to only allow some nodes to see some of your files. 

On the right, you will find 3 useful tabs:

 - [Broadcast](../user-guide/interface/#broadcast)  
   sends messages to all connected nodes at once
 - [Local network graph](../user-guide/interface/#network-graph)  
   shows the network around you, based on discovery information
 - [Keyring](../user-guide/interface/#keyring)  
   contains node keys you collected, mostly forwarded to you by your friend nodes

![Network](../img/interface/network/redqueen.png "Network RedQueen")  
The Red Queen is having a friend in here Network/Friendlist. 
It's the User Bunny and RedQueen is connected to both of his Locations. 
Bunny runs two different locations. One for each of his device. 
The location *shelter* is running on his laptop, and the location *hole* 
is on his personal Computer. 

###Change Avatar
![Avatar and Message](../img/interface/network/avatar_message.png "Avatar and Message")  
By clicking on the default Avatar Icon you can set your avatar picture 
to any picture you prefer. 

![empty Avatar](../img/interface/network/empty_avatar.png "Empty Avatar")  
Only your friends will be able to see it. You can also change it later on.  

![Change Avatar](../img/interface/network/change_avatar.png "Change Avatar")  

###Status Message
![Status Button](../img/interface/network/status_button.png "Status Button")  
Your status message will be shown in the Network/Friendlist of your friends 
beside your Avatar. 
![Status Edit](../img/interface/network/status_edit.png "Status Edit")  

###Friendlist

Friends are sorted by name or by state. 

![Friendlist](../img/interface/network/friendlist.png "Friendlist")  

The columns with the last contact and ip can be enabled with right click.  
![Tree View](../img/interface/network/tree_view.png "Tree View Option")  

###Broadcast
The Broadcast Chat sends a message to all online friends at once. 
![Broadcast](../img/interface/network/broadcast.png "Broadcast")  

###Network Graph
The network graph shows all friends and their interconnections. 
Bunny has friended with Alice and RedQueen. 
![Graph](../img/interface/network/network_graph.png "Network Graph")  

###Keyring
RetroShare collects keys from other nodes in the network, 
mostly forwarded by friends.  
![Keyring](../img/interface/network/keyring.png "Keyring")  

Columns of the Keyring 

 - Do you accept connections signed by this key  
 - Name of the Key  
 - This column indicates the trust level and wheter you signed their key  
 - Did that peer sign your key  
 - Certificate ID  
 - Last time this certificate has been used
 
 Colours
 
 - Yellow is your own Key  
 - Green are Friends  
 - Grey are Persons  

##People
![people interface](../img/interface/people.png "People")  

Identities are used to securely identify your data: sign messages in chat 
lobbies, forum and channel posts, receive feedback using RetroShare 
built-in email system, post comments after channel posts, 
chat using secured tunnels, etc. 

![person](../img/interface/people/people.png "People")  

###Identities  
Two kinds of Identities can be utilized. 

Click the ![add ID](../img/interface/people/add_id.png "Create New Identity") 
Icon to create a new Identity ![add ID menu](../img/interface/people/add_id_menu.png "Add ID Menu") 

####Pseudonymous Identities
Identities can optionally be signed by your RetroShare node's certificate. 
Signed identities are easier to trust but are easily linked to your node's IP address. 

![pseudo ID create](../img/interface/people/pseudo_id_create.png "Pseudo Identity Create")  

 - Identiy Name  
   Name of the Identity. It is not necessary to use the same name as  
   your Node User. But it's common.  
 - Identity ID  
   Each Identity has it's own crypto hash ID number.  
 - Type  
   Owned by you and linked to your RetroShare Node. Instead of Anonymous  
 - Owner Node ID  
   GPG-ID Number used by your [Node](../user-guide/settings/#public-information)
 - Owner Node Name  
   User Name of your Node User  
 - Last Used  
   Last time the Identity has been in use. This can be a forum post or 
   anything else. 
 - Your opinion  
   Your opininon on your owned ID is Neutral. This is used to rate other ID's for a 
   reputation system. 
 - Auto-Ban all identities from this node  
   Ban all ID's from a specific node. 
 - Neighbor nodes  
   Average opinion of neighbor nodes about this identity. 
   Negative is bad, positive is good. Zero is neutral.
 - Overall  
   Overall reputation score, accounting for yours and your friends'. 
   Negative is bad, positive is good. Zero is neutral. If the score is too 
   low, the identity is flagged as bad, and will be filtered out in forums, 
   chat lobbies, channels, etc. 

![pseudo bunny ID](../img/interface/people/bunny_id.png "Bunny Pseudonymous ID")  

####Anonymous Identities
Anonymous identities allow you to anonymously interact with other users. 
They cannot be spoofed, but noone can prove who really owns a given identity. 

![create freebunny ID](../img/interface/people/create_freebunny.png "Create FreeBunny Anonymous ID") 

 - Identity Name  
   Name of the Identity. Can be named anything. 
 - Identity ID  
   Each Identity has it's own crypto hash ID number.  
 - Type  
   Anonymous identity
 - Last Used  
   Last time the Identity has been in use. This can be a forum post or 
   anything else. 
 - Your opinion  
   Your opininon on your owned ID is Neutral. This is used to rate other ID's for a 
   reputation system. 
 - Neighbor nodes  
   Average opinion of neighbor nodes about this identity. 
   Negative is bad, positive is good. Zero is neutral.
 - Overall  
   Overall reputation score, accounting for yours and your friends'. 
   Negative is bad, positive is good. Zero is neutral. If the score is too 
   low, the identity is flagged as bad, and will be filtered out in forums, 
   chat lobbies, channels, etc.    
 
![freebunny ID](../img/interface/people/freebunny_id.png "FreeBunny ID") 

###Circles
![Circles](../img/interface/people/circles.png "Circles") 

Circles are groups of identities (anonymous or signed), that are shared at a distance over the network. They can be used to restrict the visibility to forums, channels, etc.  
A circle can be restricted to another circle, thereby limiting it's visibility to members of that circle or even self-restricted, meaning that it is only visible to invited members.  

####Create Circles

Click the ![add ID](../img/interface/people/add_id.png "Create New Identity") 
Icon to create a new Identity ![add ID menu](../img/interface/people/add_id_menu.png "Add ID Menu") 

 - ![public circle](../img/interface/people/public_circle.png "Public Circle") Public  
   Publicly distributed circles, are visible to your friends, which 
   will get to know the circle data (Creator, members, etc)
 - ![private Circle](../img/interface/people/private_circle.png "Private Circle")  Private  
   Private (a.k.a. self-restricted) circles are only visible to the 
   invited members of these circles. In practice the circle uses its own list 
   of invited members to limit its own distribution. 
 - ![limit Circle](../img/interface/people/limit_circle.png "Limited to Circle") Only visible to members of another Circle  
   Circles can be restricted to the members of another circle. 
   Only the members of that second circle will be allowed to see the new 
   circle and its contents (list of members, etc).
 - Invited Members  
   Members of this list will be automatically proposed to join the circle (by accepting membership). 
   They will not receive data that is restricted to this circle until they do so. 

The circle name, contact author and invited member list will be visible 
to all invited members. If the cricle is not private, it will also be visible to neighbor nodes 
of the nodes who host the invited members. 

![Umbrella Circles](../img/interface/people/create_umbrella.png "Creating Umbrella Corporation Circle") 

####Join Circles

![Umbrella Circle Empty](../img/interface/people/umbrella_circle_empty.png "Umbrella Circle Without Members") 

Accept your circle invitation by right clicking  
![Join Invitation](../img/interface/people/accept_circle.png "Accept Invitation")  

![Umbrella Circles](../img/interface/people/umbrella_circle.png "Umbrella Circle Joined")  


##File Sharing
![filesharing interface](../img/interface/filesharing.png "File Sharing")  

RetroShare birngs two ways fo transferring files: 

 - direct file transfers from your friends
 - distant anonymous tunneled transfers  
In addition, file transfer is multi-source and allows swarming (you can be source while downloading).  

<a href="../../img/interface/filesharing/up_and_down.png" target="_blank">![up and down](../img/interface/filesharing/up_and_down.png "Up and Downloading")</a>
In this Screenshot, the files are not yet finished and still start to upload to other friends. 

###Download
<a href="../../img/interface/filesharing/download.png" target="_blank">![downlaod](../img/interface/filesharing/download.png "Download")</a>  


Columns from the Download Tab ![downlaod tab](../img/interface/filesharing/download_tab.png "Download Tab")  

 - Name  
   Name of the file    
 - Size  
   Size of the downloaded  
 - Completed  
   already downloaded size  
 - Speed  
   actual speed of the download  
 - Progress / Availability  
   each Chunk (1 Chunk = 1MB part) is shows it status by colour
   ![progress bar](../img/interface/filesharing/progress_bar.png "Progress Bar")  
    - Blue - already finished
    - Red - active download
    - Yellow - calculating checksums
    - empty - not downloaded yet
    
 - Sources  
   active sources in brackets the total number of available files in the network   
 - Status  
    - Waiting
    - Downloading  
    - Paused  
      manually paused state, can be resumed also  
    - Checking  
      calculating checksums of all Chunks of the Download  
    - Completed  
      The Download has finished, and should be available in the Download Directorie
 - Speed / Queue position   
    - Faster  
    - Average  
    - Slower   
 - Remaining  
   remaining file size to download till it's finished
 - Download Time  
   estimated time to finish the download  
 - Hash  
   Hash number of the file [SHA1](https://en.wikipedia.org/wiki/SHA-1)
 - Last Time Seen  
   last time when the source of this file has been available  
 - Path  
   destination folder

###Multiple Sources  
Multi Sources are shown in the Sources Column and can be 
displayed in detail by clicking the dropdown button

 - ![active tunnel](../img/interface/filesharing/green_source.png "active Tunnel") active source transferring data  
 - ![yellow tunnel](../img/interface/filesharing/yellow_source.png "inactive Tunnel") no data currently transferring  


###Context Menu  
By right-clicking on the download, the Context menu provides actions to the user.

![context menu download](../img/interface/filesharing/context_menu.png "Download Context Menu") 

 - Priority  
   ![context menu priority](../img/interface/filesharing/context_menu_priority.png "Context Menu Priority")  
 - Chunk Strategy  
   ![context menu strategy](../img/interface/filesharing/context_menu_strategy.png "Context Menu Strategy")  
 - Rename file...  
 - Set destination directory  
   ![context menu destination](../img/interface/filesharing/specify_destination.png "Context Menu Destination")  
   Set the directory where the file should be put when it's completed
 - Pause  
   Pause the download and resume it later
 - Force Check  
   Trigger a check of the checksums manually
 - Cancel  
   Stop the download
 - Open Folder  
   Open the Folder where the file has been downloaded
 - Details...  
   show Details from the download.
   ![context menu details](../img/interface/filesharing/context_details.png "Context Menu Details")  
 - Clear Completed  
   removes finished downloads, and removes them from the Download Tab  
 - Copy RetroShare Link  
   copy the RetroShare Link to the Clipboard  
   
        retroshare://file?name=RetroShare-0.6.1-Windows-Portable-20161005-d020d8d8-Qt-5.7.0-dev.7z&size=20476577&hash=d5d91d4ec9438c6df2dcbd9236d4faebd2eef75d
   
   ![context menu details links](../img/interface/filesharing/context_details_links.png "Context Menu Details Links")  
   
 - Expand all  
   Open all downloads with multi source dropdown buttons
 - Collapse all  
   Collapes all downloads with open multisources 
 - Collection  
   ![context menu collection](../img/interface/filesharing/context_menu_collection.png "Context Menu Collection")  
    - download from **.rscollection** files 
   
You can share files using the "Directory Plus" icon from the left side bar. These files will be listed in the My Files tab. You can decide for each friend group wheter they can or not see these files in their Friends Files tab. 

The search tab reports files from your friends' file lists, and distant files that can be reached anonymously using the multi-hop tunneling system. 

##Chat Lobbies
![chat-lobbies interface](../img/interface/chat-lobbies.png "Chat Lobbies")  
Chat lobbies are distributed chat rooms, and work pretty much like 
[IRC](https://en.wikipedia.org/wiki/Internet_Relay_Chat) or 
[XMPP/Jabber](https://de.wikipedia.org/wiki/Extensible_Messaging_and_Presence_Protocol). 
They allow you to talk anonymously with tons of people without the need to make friends. 
Chatrooms are decentralized and serverless. This means they do not require 
a central server and are shared between direct friends. 
All participants receive all messages. 
Once the lobby is created you can invite other friends from the friends tab. 

###Types of Chat Rooms  
 - Public Chatrooms  
   You can join all chatrooms which are subscribed by your friends.  
   Your friends will be able to join all chatrooms which you have subscribed.  
 - Private Chatrooms  
   This chatrooms is only visible and shared to invited members. 
   Your friends can't see it, unless you invite them. 
   Once you have been invited to a private lobby, 
   you will be able o see it when your friends are using it.  
  
![empty chatrooms](../img/interface/chatrooms/empty_chat.png "Empty Chatrooms")  

###Chat Room Creation

Click the ![add ID](../img/interface/people/add_id.png "Create New Identity") 
Icon to create a new Chat room. 

 - Lobby name  
   The name of the Chatroom. It can't be changed afterwards.  
 - Lobby topic  
   A welcome message in the Lobby room. It can't be changed afterwards.  
 - Identiy to use  
   ![select identity](../img/interface/chatrooms/select_identity.png "Select Identity for Chat")  
   This needs to be one of your identies created in [People](../user-guide/interface/#people)  
 - Visibility  
   ![select visibility](../img/interface/chatrooms/select_visibility.png "Select Visibility of Chatroom")  
   For a list of Chatroom see [Types](../user-guide/interface/#types-of-chat-rooms)
 - Security  
   If you check this, only PGP-signed ids can be used to join and talk in this lobby. 
   This limitation prevents anonymous spamming as it becomes possible 
   for at least some people in the lobby to locate the spammer's node. 
 - Contacts  
   Initially send invitations to online friends of your Node. Only direct 
   friends can join with their Identities. 

![chatroom creation](../img/interface/chatrooms/create_chat.png "Chatroom Creation")  

The choosen contacts will be invited to the join the chatroom with an identity.  

 - Choose an identity for this lobby: 
![bunny choose id](../img/interface/chatrooms/invite_bunny_id.png "Bunny choose ID")  

![chatroom invitation](../img/interface/chatrooms/chat_invitation.png "Chatroom Invitation")  

The Friend Bunny has joined the newly created Chatroom and starts chatting. Now all Friends of 
The Public Chatroom propagates to all Friends of Bunny and they can join as well.  
![chatroom established](../img/interface/chatrooms/chat_established.png "Chatroom established")  

###Join Existing Chatrooms

Join existing chatrooms by double clicking or right-clicking.

![Join Chatroom](../img/interface/chatrooms/join_chat.png "Join Chatroom")

Right click offers following possibilities

 - Enter this lobby  
   Joins the Chatroom  
 - Add Auto Subscribe  
   Joins the Chatroom and adds auto subscribe. So this Chatroom will be 
   joined also after each restart again.  
 - Columns  
    - Count  
      Shows a count of members in this Chatroom  
    - Topic  
      Displays the Topic  
    - Subscribed  
      If you are already subscribed or not  
      
![enter chatrooms](../img/interface/chatrooms/enter_chat.png "Enter Chatrooms")  

###Chat Room Usage
Note: For the chat lobbies to work properly, your computer needs be on time. So check your systems clock!

####Chat Window

 - ![invite to chatroom](../img/interface/chatrooms/invite.png "Invite ") invite  
   invite friends to this chatroom
 - ![leave chatroom](../img/interface/chatrooms/leave.png "Invite ") leave  
   leave the chatroom
 - ![add smileys](../img/interface/chatrooms/smileys.png "Smileys") smileys  
   choose one of these smileys  
   ![choose one of these smileys](../img/interface/chatrooms/smileys_available.png "Available Smileys") 
 - ![attach picture](../img/interface/chatrooms/attach_img.png "Invite ") attach picture  
   attach a picture into your chat message  
 - ![attach file](../img/interface/chatrooms/attach_file.png "Invite ") attach file  
   attach files from your computer into your chat message
 - ![settings](../img/interface/chatrooms/settings.png "Invite ") settings  
    - Clear Chat History  
      emptys the chat window  
    - Delete Chat History  
      deletes stored 
    - Save Chat History  
      Save Chat History to a file
    - Browse Message History
      Browse the already saved Message History 
    - Set text font color
      Change your color and font
    - Switch Identity   
      Change your Identity  
      ![chat settings menu](../img/interface/chatrooms/chat_settings_menu.png "Invite ")  
 - ![search](../img/interface/chatrooms/search.png "Invite ") search  
   Search the Chatroom Messages for a keyword  
 - ![send](../img/interface/chatrooms/send.png "Send Chat Message") send  
   Send your typed message to the Chatroom
 
![chatroom usage](../img/interface/chatrooms/chat_usage.png "Chatroom usage")  
 
####Participant List
All Members of the Chatroom are shown in the list at the left. 

#####Chat Status Button  
The coloured circle shows the status of the participant  

 - ![Yellow - Your Own ID](../img/interface/chatrooms/bullet_yellow.png "Your own Identity") Yellow  
   This is your own identity
 - ![Active ID](../img/interface/chatrooms/bullet_green.png "Active ID")Green  
   Active, this Identity has been in use in the last 300 seconds
 - ![Grey - not active](../img/interface/chatrooms/bullet_grey.png "Not active Identity")Grey  
   This Identity is not active in this chatroom.  

![Participant List](../img/interface/chatrooms/member_list.png "Participant List")

#####Chat ID Tooltip
Hover with your mouse over the ID and some information will pop up in the tooltip. 
![Chat ID Tooltip](../img/interface/chatrooms/id_tooltip.png "Tooltip for Chat ID")

#####Chat ID Actions
When you right-click on the Chat ID, an additional context menu will popup and show some actions. 

 - Start private chat  
   Opens a distant chat to that person  
 - Send Message  
   Opens the message composer to send a mail to this Identity
 - Sort by Activity  
 - Sort by Name  
 - Mute participant  
   Mute the participant in this room
 - Ban this person (sets negative opinion)  
   Bans the whole Identity. Does not display Content (Forum posts, Channel messages, posted links, ... ) 
   neither does the content of this person get's forwarded to friends anymore. 
   
![Context Menu Chat ID](../img/interface/chatrooms/menu_chat_id.png "Right Click Menu Chat ID")


##Messages
![messages interface](../img/interface/messages.png "Messages")  
RetroShare has its own internal email system. You can send/receive emails to/from connected friend nodes.  

It is also possible to send messages to other people's Identities using the global routing system. These messages are always encrypted and signed, and are relayed by intermediate nodes until they reach their final destination. 

Distant messages stay into your Outbox untial an acknowledgment of receipt has been received. 

Generally, you mey use messages to recommended files to your friends by pasting file links, or recommend friend nodes to other friend nodes, in order to strenghten your networ, or send feedback to a channel's owner. 


##Channels
![channels interface](../img/interface/channels.png "Channels")  
Channels allow sou to paost data (e.g. movies, music) that will spread the network

You can see the channels your friends are subscribed to, and you automatically forward subscribed channels to your friends. 
This promotes good channels in the network. 

Only the channel's creator can post on that channel. Other peers in the network can only read from it, unless the channel is private. You can however share the posting rights or the reading rights with friend RetroShare nodes. 

Channels can be made anonymous, or attached to a RetroShare identity so that readers can contact you if needed. Enable "Allow Comments" if you want to let users comment on your posts. 

Channel posts get deleted after 4 months. 

##Forums
![forums interface](../img/interface/forums.png "Forums")  
RetroShare Forums look like internet forums, but they work in a decentralized way. 

<a href="../../img/interface/forums/empty_forum.png" target="_blank">![empty forums](../img/interface/forums/empty_forum.png "Empty Forums")</a>  

You see forums your friends are subscribed to, and you forward subscribed forums to your friends. 
This automatically promotes interresting forums in the network. 
Forum messages get deleted after 12 months. 

###Forum Settings

![create forums](../img/interface/forums/create_forum.png "Create Forums")  


 - Name  
   Name of the Forum
 - Owner  
   Owner of the Forum
 - Add Forum Admins  
   Key recipients can publish to restricted-type group and can view and 
   publish for private-type channels. 

####Forum Message Distribution

 - ![public Forum](../img/interface/forums/network-public.png "Public Forum") Public  
   Message will spread way beyond your friend nodes, as long as people 
   subscribe to the channel/forum/posted you're creating. 
 - ![Circle Restricted Forum](../img/interface/forums/circles.png "Circle Restricted Forum") Restricted to Circle  
   Message will spread among RetroShare nodes that host one of the 
   identities listed as member of the circle and who also subscribe the media. 
   Only these nodes will be able to see that this forum/channel/posted media exists. 
 - ![Network Forum](../img/interface/forums/network.png "Only Friends Forum") Only For Your Friends  
   Messages will only be distributed to the selected subset of your 
   friend nodes. They will not forward messages with each other, but 
   only use your own node as a central hub to distribute them. 
   
####Description  


  
####Spam Protection
![posts permissions](../img/interface/forums/posts_permission.png "Forums Post Permissions")  

 - Posts permissions  
   This combo box allows you to choose how posts are handled depending 
   on the node the poster belongs to. 
 - All allowed  
   all posts are treated equally
 - Defavor posts from unsigned IDs  
   anonymous IDs will require a reputation of 0.4 to be received/forwarded. 
 - Defavor posts from unsigned IDs and IDs from unknown nodes  
   anonymous IDs and IDs signed by unknown RetroShare nodes will require 
   a reputation of 0.4 to be received/forwarded. 


###Create Forums  

click the ![create forum button](../img/interface/forums/add.png "Create Forum Button") 
button, and fill in the name and select a Message Distribution Type. 

![create forums](../img/interface/forums/friendship.png "Create Forums") 
 
Your newly created Forum will be available at ![my forums](../img/interface/forums/folder_blue.png "My Forums") *My Forums*  
![my forums](../img/interface/forums/my_friendship_forum.png "My Forums")  

Empty new Forum without any Threads  
![Post New Thread](../img/interface/forums/create_thread.png "Post New Thread")  


###Post new Thread  


click on the ![Post New Thread](../img/interface/forums/mail_new.png "Post New Thread") 
icon to create a new post.  

![Edit New Thread](../img/interface/forums/start_new_thread.png "Edit New Thread")  

![Thread Created](../img/interface/forums/thread_created.png "Thread Created")  


###Reply a Post  

click on the ![reply post](../img/interface/forums/mail_reply.png "Reply Post") 
icon to create a new post.  

![Reply to Post](../img/interface/forums/reply_post.png "Reply to Post")  

![Reply](../img/interface/forums/reply.png "Reply")  


![Thread Answered](../img/interface/forums/thread_reply.png "Thread Answered")  


###Forum Details  

 - ![my forums](../img/interface/forums/folder_blue.png "My Forums") My Forums  
 - ![subscribed forums](../img/interface/forums/folder_red.png "Subscribed Forums") Subscribed Forums   
 - ![Popular Forums](../img/interface/forums/folder_green.png "Popular Forums") Popular Forums  
 - ![other Forums](../img/interface/forums/folder_yellow.png "Other Forums") Other Forums  
 
 
 - ![post thread](../img/interface/forums/mail_new.png "Post Thread") Post Thread  
 - Thread Title   
 - Forum View  
   - Last Post  
   - Threaded View  
   - Flat View  
   ![forum view](../img/interface/forums/forum_view.png "Forum View")
 - ![Post Reply](../img/interface/forums/mail_reply.png "Post Reply") Post Reply  
 - ![Previous Thread](../img/interface/forums/back.png "Previous Thread") Previous Thread  
 - ![Next Thread](../img/interface/forums/forward.png "Next Thread") Next Thread  
 - ![Download All](../img/interface/forums/down.png "Download All") Download All  
 - ![Next unread](../img/interface/forums/next_unread.png "Next unread") Next unread  
 - ![Change Forum Sort](../img/interface/forums/looknfeel.png "Forum Sort") Forum Sort  
 
    - Sort by Name  
    - Sort by Popularity  
    - Sort by Last Post  
    - Sort by Posts  
      ![forums Sort](../img/interface/forums/sort_forums.png "Forum Sort")



##Posted
![posted interface](../img/interface/posted.png "Posted")  

Plugin Posted

##FeedReader 
![feedreader interface](../img/interface/feedreader.png "FeedReader") 

The posted service allows to share internet links, that spread among RetroShare nodes like forums and channels. 

Links can be commented by subscribed users. A promotion system also gives the opportunity to enlight important links.  

There is no restriction on which links are shared. Be carefull when clicking on them. 

Posted links get deleted after 4 months. 

##Add
![Add interface](../img/interface/invite.png "Add")  



##Options

![settings interface](../img/interface/options.png "Options/Settings")  


The Options/Settings are explained more detailed [here](/user-guide/settings/). 

![ interface](../img/interface/settings.png "") 


##About
![about interface](../img/interface/info.png "About")  

###About
The about section shows the RetroShare version and Revision and Qt Version 
![about interface](../img/interface/about_retroshare.png "About RetroShare") 

####About RetroShare
Contains a small description and links to:  
 - [RetroShare WebSite](http://retroshare.github.io)  
 - [legacy WebSite](http://retroshare.sourceforge.net) on SourceForge has been renewed  
 - [legacy Wiki](http://retroshare.sourceforge.net) on SourceForge  
 - [RetroShare Organization on GitHub](https://github.com/RetroShare)  
 - [RetroShare Forum](http://retroshare.sourceforge.net)  
 - [DevBlog](https://github.com/RetroShare)  
 - [Twitter](https://twitter.com/retroshare)  
![about retroshare interface](../img/interface/about_retroshare_about.png "About")  

####Authors
Over the years lot of different People have helped to improve RetroShare. 

To be named in front:  
Lead Developer *csoler*  
Founder *drBob*  

and many many more

![authors retroshare interface](../img/interface/about_retroshare_authors.png "Authors") 

####Thanks to

nanos gigantum humeris insidentes - dwarfs standing on the shoulders of giants  

RetroShare couldn't exist without the building upon the work of other great projects. 

![thanks retroshare interface](../img/interface/about_retroshare_thanks.png "Thanks") 

####Translation

![translation retroshare interface](../img/interface/about_retroshare_translation.png "Translation") 

####License Agreement

![License Agreement interface](../img/interface/about_retroshare_license.png "License Agreement") 


##Quit
![quit interface](../img/interface/exit.png "Quit") 

To close RetroShare click on the quit button and choose yes at the popup. 

![really quit interface](../img/interface/really_quit.png "Really Quit") 

