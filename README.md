# Language Meson

Syntax highlighting for the [Meson](http://mesonbuild.com/) language.

## Note for other editors

Editors such as Sublime Text, TextMate, and Visual Studio Code can use the same
syntax highlighting but the grammar file must be converted to the TextMate format.

Note that you would first have to convert the grammar file in either JSON format, PLIST format, or YAML format.

The easiest method to do so is via the Sublime Text [PackageDev](https://packagecontrol.io/packages/PackageDev)
package. Somebody could decouple the conversion [library](https://github.com/SublimeText/PackageDev/tree/master/plugins/lib/fileconv)
it uses to ease future conversion also. Example output is [here](https://gist.github.com/TingPing/02aea7422dacaded3a35a6ba12fc3757).
