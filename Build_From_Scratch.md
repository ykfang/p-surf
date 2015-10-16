### Building from scratch ###
If you are new to [mercurial](http://www.selenic.com/mercurial/) please consider following [Mercurial QuickStart](http://www.selenic.com/mercurial/wiki/index.cgi/QuickStart) or the [Bryan O'Sullivan](http://hgbook.red-bean.com/read/)'s  lovely guide.
```
hg clone https://p-surf.googlecode.com/hg/p-surf
cd p-surf
cp user_pref.xml.template user_pref.xml
```

Edit in _user\_pref.xml_ procesing-core to respect your system installation.

```
#!xml
<property name="processing-core" 
    value="C:\Programmi\processing-0135-expert\lib\core.jar"/>
```

After that

```
ant dowload_deps
ant deploy
```

You will find a _p-surf.zip_ file in the _release_ subfolder of the source tree.
Copy that zip file into your sketchbooks folder as described in [Getting Started](Getting_Started.md) and you're done.