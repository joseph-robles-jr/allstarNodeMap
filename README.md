# allstarNodeMap Overview
A JavaScript module that renders a simple map of directly attached AllStarLink Nodes.

I run a small AllStarLink repeater and was tired of slow and overly complex interfaces for just checking who was connected in over allstar. I build this small module and webpage to display current DIRECT connections for any allstar node. It is still in an early stage, but I am making progress on it. You can find a live version at [ham.ki5tlz.net](https://ham.ki5tlz.net/apps/NodeMapApp/NodeMapApp.html)

This relies on the allstarlink.org API's.

# Setup
There are 2 ways to run this. You can either import the module directly from `jsModules/allstarNodeMap/` and build a site around it, or you can do the following:

At the top of the `NodeMapApp.js` file, you will see `const DEFAULT_NODE_NUMBER = 603450;`. This is the default AllStarLink node number that is loaded when the page is loaded. Change this to whatever you want to start at, like `const DEFAULT_NODE_NUMBER = 51018;` for the W6EK repeater. Then move these files into a webserver of your choosing. It should just work.

### Note:
Web browsers require this project to be served over HTTP because it loads JavaScript modules. It is a security feature. This project will not function if simply opening the `NodeMapApp.html' file from a file browser. A web server like Apache2 or Java's Tomcat is necessary. 



