sublime text 2/3 Configuration and usefull plugins for WEB FRONT DEVELOPPER
===========================

----------

Copy/paste ST2 packages into %APPDATA%\Sublime Text 2

Copy/paste ST3 packages into %APPDATA%\Sublime Text 3

Full tutorial (FR) : [http://www.js-attitude.fr/2013/03/12/sublime-text-dev-web-config-trucs-astuces/](http://www.js-attitude.fr/2013/03/12/sublime-text-dev-web-config-trucs-astuces/)


First step, install control package manager : 

## Control package manager : ##

	
    View > show console (ctrl+`)

Copy/past the package control install command :

Sublime text 2 :

	import urllib2,os,hashlib; h = '7183a2d3e96f11eeadd761d777e62404' + 'e330c659d4bb41d3bdf022e94cab3cd0'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); os.makedirs( ipp ) if not os.path.exists(ipp) else None; urllib2.install_opener( urllib2.build_opener( urllib2.ProxyHandler()) ); by = urllib2.urlopen( 'http://sublime.wbond.net/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); open( os.path.join( ipp, pf), 'wb' ).write(by) if dh == h else None; print('Error validating download (got %s instead of %s), please try manual install' % (dh, h) if dh != h else 'Please restart Sublime Text to finish installation')

Sublime text 3 :

	import urllib.request,os,hashlib; h = '7183a2d3e96f11eeadd761d777e62404' + 'e330c659d4bb41d3bdf022e94cab3cd0'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://sublime.wbond.net/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by)


Reboot sublime text.

To install package :

	Preferences > package contrle > Package control : install package

Or 
	ctrl+shift+p then type : pci

## Usefull plugins :  ##


### EditorConfig ###

**Package name :** EditorConfig

**Documentation :** [https://sublime.wbond.net/packages/EditorConfig](https://sublime.wbond.net/packages/EditorConfig)

**Description :**
EditorConfig helps developers define and maintain consistent coding styles between different editors and IDEs. The EditorConfig project consists of a file format for defining coding styles and a collection of text editor plugins that enable editors to read the file format and adhere to defined styles. EditorConfig files are easily readable and they work nicely with version control systems.



### Emmet ###

**Package name :** Emmet

**Documentation :** [https://sublime.wbond.net/packages/Emmet](https://sublime.wbond.net/packages/Emmet)

**Description :** 
Emmet is a plugin for many popular text editors which greatly improves HTML & CSS 



### AdvancedNewFile ###

**Package name :** AdvancedNewFile

**Documentation :** [https://sublime.wbond.net/packages/AdvancedNewFile](https://sublime.wbond.net/packages/AdvancedNewFile)

**Description :** 
Advanced file creation for Sublime Text 2 and Sublime Text 3.This plugin allows for faster file creation within a project. Please see the [Features](https://github.com/skuroda/Sublime-AdvancedNewFile#features) section for more detailed information about advanced features.



### Alignment ###

**Package name :** Alignment

**Documentation :** [https://sublime.wbond.net/packages/Alignment](https://sublime.wbond.net/packages/Alignment)

**Description :** 
Dead-simple alignment of multi-line selections and multiple selections for Sublime Text 2.



### Handlebars ###

**Package name :** Handlebars

**Documentation :** [https://sublime.wbond.net/packages/Handlebars](https://sublime.wbond.net/packages/Handlebars)

**Description :** 
It's a great JavaScript templating engine, based on [Mustache](http://mustache.github.io/ "Mustache"), but adding the ability to precompile templates and to create custom helpers.

Official website: [handlebarsjs.com](handlebarsjs.com)



### CoffeeScript ###

**Package name :** CoffeeScript

**Documentation :** [https://sublime.wbond.net/packages/CoffeeScript](https://sublime.wbond.net/packages/CoffeeScript)

[https://sublime.wbond.net/packages/Better%20CoffeeScript](https://sublime.wbond.net/packages/Better%20CoffeeScript)

**Description :** 
Syntax highlighting and checking, commands, shortcuts, snippets, compilation and more.



### JsFormat ###

**Package name :** JsFormat

**Documentation :** [https://sublime.wbond.net/packages/JsFormat](https://sublime.wbond.net/packages/JsFormat)

**Description :** 
JsFormat is a javascript formatting plugin for Sublime Text 2. It uses the command-line/python-module javascript formatter from [http://jsbeautifier.org/](http://jsbeautifier.org/) to format whole js or json files, or the selected portion(s).



### SASS ###

**Package name :** SASS

**Documentation :** [https://sublime.wbond.net/packages/Sass](https://sublime.wbond.net/packages/Sass)

**Description :** 
This add-on adds syntax highlighting and tab/code completion for Sass and SCSS files. It features Zen Coding shortcuts for many CSS properties, making you look like some kind of stylesheet wizard to everyone around you. You've got to like that.



### SublimeLinter ###

**Package name :** SublimeLinter

**Documentation :** [https://sublime.wbond.net/packages/SublimeLinter](https://sublime.wbond.net/packages/SublimeLinter)

**Description :** 
SublimeLinter is a plugin that supports "lint" programs (known as "linters"). SublimeLinter highlights
  lines of code the linter deems to contain (potential) errors. It also
  supports highlighting special annotations (for example: TODO) so that they
  can be quickly located.




### Unicode Character Highlighter ###

**Package name :** Unicode Character Highlighter

**Documentation :** [https://sublime.wbond.net/packages/Unicode%20Character%20Highlighter](https://sublime.wbond.net/packages/Unicode%20Character%20Highlighter)

**Description :** 
This plug-in highlights characters such as non breakable space, characters that often break compilers and scripts and is almost impossible to spot in the editor.




### TortoiseSVN ###

**Package name :** TortoiseSVN

**Documentation :** [https://sublime.wbond.net/packages/TortoiseSVN](https://sublime.wbond.net/packages/TortoiseSVN)

**Description :** 
TortoiseSVN, TortoiseGit and TortoiseHg integration with Sublime Text 2 via menus and keyboard shortcuts.






### Local History ###

**Package name :** Local History

**Documentation :** [https://sublime.wbond.net/packages/Local%20History](https://sublime.wbond.net/packages/Local%20History)

**Description :** 
A Sublime Text 2/3 plugin for maintaining local history of files





### LoremIpsum ###

**Package name :** LoremIpsum

**Documentation :** [https://sublime.wbond.net/packages/LoremIpsum](https://sublime.wbond.net/packages/LoremIpsum)

**Description :** 
An extension for Sublime Text 2 and 3!

(Support for Sublime Text 3 is new, and barely tested - any feedback appreciated - see ST3 section below)

It allow you to Insert Lorem Ipsum in the editor via menu items or keyboard shortcut.




### Placehold.it Image Tag Generator ###

**Package name :** Placehold.it Image Tag Generator

**Documentation :** [https://sublime.wbond.net/packages/Placehold.it%20Image%20Tag%20Generator](https://sublime.wbond.net/packages/Placehold.it%20Image%20Tag%20Generator)

**Description :** 
Placehold.it plugin for Sublime Text 2




### Side​Bar​Enhancements ###

**Package name :** Side​Bar​Enhancements

**Documentation :** [https://sublime.wbond.net/packages/SideBarEnhancements](https://sublime.wbond.net/packages/SideBarEnhancements)

**Description :** 
Sublime Text 3+ Package. Install via an updated version of Package Control 2+. Just *DON'T install manually.

Provides enhancements to the operations on Sidebar of Files and Folders for Sublime Text. See: http://www.sublimetext.com/

Notably provides delete as "move to trash", open with.. and a clipboard. Close, move, open and restore buffers affected by a rename/move command.

Provides the basics: new file/folder, edit, open/run, reveal, find in selected/parent/project, cut, copy, paste, paste in parent, rename, move, delete, refresh....

The not so basic: copy paths as URIs, URLs, content as UTF8, content as data:uri base64 ( nice for embedding into CSS! ), copy as tags img/a/script/style, duplicate

Preference to control if a buffer should be closed when affected by a deletion operation.

Allows to display "file modified date" and "file size" on statusbar.





### Inc-Dec-Value ###

**Package name :** Inc-Dec-Value

**Documentation :** [https://sublime.wbond.net/packages/Inc-Dec-Value](https://sublime.wbond.net/packages/Inc-Dec-Value)

**Description :** 
increase / decrease of numbers (integer and fractional), dates, hex color values, opposite relations or cycled enumerations on the configured value and a bonus - string actions (upper, lower, capitalize)
