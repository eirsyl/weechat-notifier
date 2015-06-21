weechat-notifier
================

[![Join the chat at https://gitter.im/eirsyl/weechat-notifier](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/eirsyl/weechat-notifier?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

WeeChat notifications on OS X using Weechat relay protocol.


### Installation

Enable relay in WeeChat with the command: 

    /set relay.network.password "your password"
    /relay add weechat PORT

You need to export the variables SERVER, PASSWORD, PORT and NICKS (comma-separated).
Then install with: 

    npm install -g weechat-notifier
    
    # Or:
    
    git clone git@github.com:eirsyl/weechat-notifier.git
    npm install 
    node index.js

### launchd

If you want weechat-notifier to run on startup you can add it as a launchd-plist (~/Library/LaunchAgents). A template can be found [here](https://gist.github.com/ekmartin/05b794ac1a2eaa803ff0).
