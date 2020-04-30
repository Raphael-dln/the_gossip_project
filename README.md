# README

Welcome to the Gossip Project ! Here you can share your gossips and learn more about THP community...

Here is what you should know about this fantastic project :

# Versions
* Ruby version 2.5.1
* Rails version 5.2.4

# Relation between tables
* User - City :            1 - n
* User - Gossip :          1 - n
* Gossip - Tag :           n - n
* Gossip - Gossip_Tag :    n - 1
* Tag - Gossip_Tag :       n - 1
* PrivateMessage - User :  n - 1  with classname : recipient and sender

# Run tests
* $ tp User.all
* $ tp Gossip.all
* $ tp Gossip.find(x) => x.gossip_tags

# Gem
* table_print: You can use "tp" to visualize the information as tables
* faker: To create a fake database