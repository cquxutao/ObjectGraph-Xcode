## ObjectGraph

![](https://travis-ci.org/vampirewalk/ObjectGraph-Xcode.svg?branch=master)
[![Twitter: @vampirewalk666](https://img.shields.io/badge/contact-%40vampirewalk-blue.svg)](https://twitter.com/vampirewalk666)

ObjectGraph can show oriented graph of dependencies between classes in your project.
This plugin is based on [objc_dep](https://github.com/nst/objc_dep) and [Graphviz](http://www.graphviz.org/).

![Screenshot](https://raw.githubusercontent.com/vampirewalk/ObjectGraph-Xcode/master/ScreenShot.png)

![Example](https://raw.githubusercontent.com/vampirewalk/ObjectGraph-Xcode/master/ObjectGraph.png)

- Black arrows: imports
- <font color="red">Red arrows</font>: .pch imports
- <font color="blue">Blue arrows</font>: two ways imports

## Usage
The default path of source code parsing is project root path, you can set new path by clicking "Set Source Path Path...".
For example, if you just want to parse your product class, not test class or external library class in Pods directory, you can set path to directory which contains your product class and execute "Draw Object Graph" again.

## Install 
First step, install Graphviz via Homebrew
```
brew install graphviz
```
or MacPorts
```
sudo port install graphviz
```
Second, install ObjectGraph-Xcode via [Alcatraz](http://alcatraz.io/)
or
Clone and build the project, then restart Xcode.

## Uninstall
Uninstall it via [Alcatraz](http://alcatraz.io/)
or
```
Run rm -r ~/Library/Application\ Support/Developer/Shared/Xcode/Plug-ins/ObjectGraph.xcplugin/
```

## Thanks
Thanks to kattrali, I get inspiration and import some code from [cocoapods-xcode-plugin](https://github.com/kattrali/cocoapods-xcode-plugin).

