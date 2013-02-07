BOOTSTRAP FOR LUCI
=================

Bootstrap is a clean HTML5 theme for LuCI - the web configuration interface commonly found on OpenWrt installation. It is based on Bootstrap, Twitter's toolkit for kickstarting CSS for websites, apps, and more. 
It includes base CSS styles for typography, forms, buttons, tables, grids, navigation, alerts, and more.

![Bootstrap for LuCI](http://nut-bolt.nl/assets/LuCI-bootstrap.png)

It is currently not included in the default OpenWrt package repository so you will have to compile it yourself.

How it works
------------

Bootstrap defines default themes for most HTML elements. For an indication of which components are available, have a look at
+ http://twitter.github.com/bootstrap/components.html
Please note not all components are available or will look the same. Twitter Bootstrap is an evolving project and LuCI Bootstrap does not precisely track its development.

Every page gets assigned a body class based on the name of the node/module/app you are currently in. For the Overview page it will be as follows
`<body class="Overview">`

This allows node-specific style rules to be applied by prefixing the css selector for your style override by `.node-name`. Say you want to change the alignment of label items on the Overview page, you would do that as follows:
`.Overview label {
    text-align: left
}`


Bug tracker
-----------

Have a bug? Please create an issue here on GitHub!

https://github.com/nutbolt/luci-theme-bootstrap/issues


Authors
-------

**David Menting**

+ http://twitter.com/studiomenting
+ http://github.com/DavidMenting

License
---------------------

LuCI Theme Bootstrap: Copyright 2012 Nut & Bolt
Twitter Bootstrap: Copyright 2011 Twitter, Inc.

Licensed under the Apache License, Version 2.0: http://www.apache.org/licenses/LICENSE-2.0
