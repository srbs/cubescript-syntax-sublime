Sublime Text Cubescript Syntax Definition
=========================================

Syntax highlighting for [Sauerbraten](sauerbraten)'s scripting langauge, Cubescript, in Sublime Text [2](sublime2) & [3](sublime3).


### Installation

With [Package Control](package_control):

1. Run `Package Control: Install Package` command, find and install `Cubescript Syntax Highlighting` plugin.
2. Restart Sublime Text editor (if required)

Using Package Control ensures package will stay up to date automatically.

Manually:

1. Clone or [download](https://github.com/srbs/cubescript-syntax-sublime/master.zip) git repo into your Packages folder (in Sublime Text, find `Browse Packages...` menu item to open this folder)
2. Restart Sublime Text editor (if required)

    Example commands:

        cd ~/Library/Application\ Support/Sublime\ Text\ 2/Packages
        git clone https://github.com/srbs/cubescript-syntax-sublime.git Cubescript


### Usage

Menu:

1. Open up the Syntax Menu (`View` -> `Syntax`)
2. Click `Cubescipt`

Command:

1. Run `Set Syntax: Cubescript` command

All *.cfg files:

1. Open any *.cfg file
2. Open up the Syntax Menu (`View` -> `Syntax`)
3. Select `Open all with current extension as...`
4. Click `Cubescript`


### Contributing

Development for this project is primarily done in [cubescript-syntax-tmbundle](textmate-repo) project. My [converter](converter-repo) is used to convert between the two structures using this `build.xml` in the parent folder of all three projects:

```xml
<project basedir=".">
    <include file="textmate-to-sublime-converter/tm2subl.xml" />
    <tm2subl destdir="cubescript-syntax-sublime" srcdir="cubescript-syntax-tmbundle" />
</project>
```

Please see the respective [Contributing](textmate-repo-contributing) section for contributing information.

This project uses the Zlib license. See the License section for details.


### License (Zlib)

    Copyright (c) 2012-2012 David "srbs" Forrest
    
    This software is provided 'as-is', without any express or implied
    warranty. In no event will the authors be held liable for any damages
    arising from the use of this software.
    
    Permission is granted to anyone to use this software for any purpose,
    including commercial applications, and to alter it and redistribute it
    freely, subject to the following restrictions:
    
        1.  The origin of this software must not be misrepresented; you must not
            claim that you wrote the original software. If you use this software
            in a product, an acknowledgment in the product documentation would be
            appreciated but is not required.
    
        2.  Altered source versions must be plainly marked as such, and must not be
            misrepresented as being the original software.
    
        3.  This notice may not be removed or altered from any source
            distribution.

[sauerbraten]: http://sauerbraten.org/ "Sauerbraten"

[sublime2]: http://www.sublimetext.com/2 "Sublime Text 2"
[sublime3]: http://www.sublimetext.com/3 "Sublime Text 3"

[package_control]: http://wbond.net/sublime_packages/package_control "Package Control"

[textmate-repo]: https://github.com/srbs/cubescript-syntax-tmbundle
[converter-repo]: https://github.com/srbs/textmate-to-sublime-converter

[textmate-repo-contributing]: https://github.com/srbs/cubescript-syntax-tmbundle#contributing "Contributing"
