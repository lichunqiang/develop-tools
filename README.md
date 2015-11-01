## Install package control

```
import urllib.request,os,hashlib; h = '2915d1851351e5ee549c20394736b442' + '8bc59f460fa1548d1514676163dafc88'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by)
```

## Config the sublime

### Theme

Perferences > color scheme > Black borad

### Font and other sitting

Click: Perferences > Setting-User

```
{
	"color_scheme": "Packages/Color Scheme - Default/Blackboard.tmTheme", //determined by theme selected
	"font_face": "Courier New",
	"font_size": 10,
	"ignored_packages":
	[
		"jQuery",
		"Markdown",
		"PhpDoc",
		"SublimeLinter",
		"SublimeLinter-contrib-standard",
		"SublimeLinter-jscs",
		"SublimeLinter-php",
		"Vintage"
	],
	"trim_trailing_white_space_on_save": true,
	"word_wrap": true
}

```

## Useful packages

### phpfmt

Open packages control, search for `phpfmt`;

__config:__

Key binding:

```
[
	{ "keys": ["ctrl+2"], "command": "analyse_this" },
	{ "keys": ["ctrl+1"], "command": "fmt_now" }
]
```

Settings - User:

```
{
	"disable_auto_align": true,
	"format_on_save": false,
	"passes":
	[
		"ReindentSwitchBlocks",
		"ReindentAndAlignObjOps"
	],
	"php55warning": false,
	"php_bin": "D:\\wamp\\bin\\php\\php5.6.11\\php.exe",
	"psr2": true,
	"version": 4
}
```

### Emmet

### bootstrap 3 snippets

### SideBarEnhancements

### DocBlockr

### EditorConfig

### GotoDocumentation
