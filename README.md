# Aristo Compass Plugin

A [Compass](http://compass-style.org/) plugin that provides a CSS3 port of the [Aristo](http://github.com/280north/aristo) UI elements.

## Install

You'll need to be familiar with the [Compass](http://compass-style.org/) CSS authoring framework and have it installed.  Then install the plugin as a gem:

    sudo gem install hpoydar-compass-aristo-plugin
    
To add the plugin to an existing Compass project:

    cd <compass_project_name>
    compass -f aristo -p project .

And add the following line to the top of the `config.rb` file created by Compass:

    require 'aristo'

## Usage

Within your application's Sass files, import the Aristo mixins:

    @import aristo

Then modify the generated `aristo.sass` file to suit your needs. See [http://hpoydar.com/aristo](http://hpoydar.com/aristo) for examples and syntax.

## TODO

* Skin the combobox
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

Thanks to Alex MacCaw, who took the first crack at CSS-ifing Aristo: [http://github.com/maccman/aristo](http://github.com/maccman/aristo)