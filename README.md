# Aristo Compass Plugin

A [Compass](http://compass-style.org/) plugin that provides a CSS3 port of the [Aristo](http://github.com/280north/aristo) UI elements.

## Install

    sudo gem install hpoydar-compass-aristo-plugin
    
To add the plugin to an existing Compass project:

    cd <compass_project_name>
    compass -f aristo -p project .

And add the following line to the top of the `config.rb` file created by Compass:

    require 'aristo'

## Usage

Within your application's Sass files, import the Aristo mixins:

    @import aristo

Then modify the generated `aristo.sass` file to suit your needs. (The file itself has some useful comments.)

## TODO

* Add segmented controls
* Add windows
* Documentation
* Attempt to have it look as good on FF3.5 as it does in Webkit/Chrome
* Take a look in IE and document what works

## About Aristo

Aristo is an open source UI distributed as part of the Cappuccino Open Source Framework [http://cappuccino.org)](http://cappuccino.org)
and specifically designed for the cross platform challenges applications face today. It is a collaborative 
effort by 280 North, Inc. and Sofa and released under the Creative Commons Attribution Share-Alike License.
You can view this license here: [http://creativecommons.org/licenses/by-sa/3.0/us/](http://creativecommons.org/licenses/by-sa/3.0/us/)

You can find out more about Aristo by visiting [http://cappuccino.org/aristo](http://cappuccino.org/aristo)
