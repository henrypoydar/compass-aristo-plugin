# Aristo Compass Plugin

A [Compass](http://compass-style.org/) plugin that provides a CSS3 port of the [Aristo](http://github.com/280north/aristo) UI elements.

## Install

    sudo gem install chriseppstein-compass
    sudo gem install hpoydar-compass-aristo-plugin
    
    
    TODO
    

## Usage

To add the 

    compass -r aristo -f <framework name> <project name>
    
_TODO: syntax for doing this with existing projects?_

Within your application's Sass files, import the Aristo mixins. You can either import all of them or one at a time:

    @import aristo/all
    
Or

    @import aristo/buttons
    @import aristo/controls
    @import aristo/menus
    @import aristo/scrollbars
    @import aristo/text
    @import aristo/windows

_TODO: document specifics for each_

## TODO

* Sass
* Templates?
* Image locations?
* Rake tasks for building examples
* Documentation
* Gem-ify
* Attempt to have it look as good on FF3.5 as it does in Webkit/Chrome
* Take a look in IE and document what works

## About Aristo

Aristo is an open source UI distributed as part of the Cappuccino Open Source Framework [http://cappuccino.org)](http://cappuccino.org)
and specifically designed for the cross platform challenges applications face today. It is a collaborative 
effort by 280 North, Inc. and Sofa and released under the Creative Commons Attribution Share-Alike License.
You can view this license here: [http://creativecommons.org/licenses/by-sa/3.0/us/](http://creativecommons.org/licenses/by-sa/3.0/us/)

You can find out more about Aristo by visiting [http://cappuccino.org/aristo](http://cappuccino.org/aristo)
