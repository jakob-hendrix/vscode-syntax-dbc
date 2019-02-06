# OGB-code-dbc-language-syntax README

This is the README for your extension "OGB-code-dbc-language-syntax". After writing up a brief description, we recommend including the following sections.

## Features

This provided syntax highighting for all `DBC` code in Visual Studio Code.

## Install your extension

* To start using your extension with Visual Studio Code copy it into the `<user home>/.vscode/extensions` folder and restart Code.

## Requirements

* Have Visual Studio Code installed

## Extension Settings

None yet...

## Known Issues

None yet...

## How To Contribute

### Grammar Creation Guide

Look at the following links for guides to editing custom grammars. For any changes you make, be sure to follow the standard Git workflow.

#### Tools that helped me

* https://rubular.com/ - a Ruby-style regex tester. It was recommended one of the links below
  * See the regex guide: http://ruby-doc.org/core-1.9.3/Regexp.html#class-Regexp-label-Options

#### Links that helped me

* https://benparizek.com/notebook/notes-on-how-to-create-a-language-grammar-and-custom-theme-for-a-textmate-bundle

* http://www.apeth.com/nonblog/stories/textmatebundle.html
* https://gcthesoftwareengineer.com/2017/01/how-to-create-custom-syntax-highlighting-in-a-visual-studio-code-extension/
* https://stackoverflow.com/questions/33403324/how-to-create-a-simple-custom-language-colorization-to-vs-code
* https://macromates.com/manual/en/language_grammars

#### Scopes we should handle, if possible:

comment
constant
constant.character.escape
constant.language
constant.numeric
declaration.section entity.name.section
declaration.tag
deco.folding
entity.name.function
entity.name.tag
entity.name.type
entity.other.attribute-name
entity.other.inherited-class
invalid
invalid.deprecated.trailing-whitespace
keyword
keyword.control.import
keyword.operator.js
markup.heading
markup.list
markup.quote
meta.embedded
meta.preprocessor
meta.section entity.name.section
meta.tag
storage
storage.type.method
string
string source
string.unquoted
support.class
support.constant
support.function
support.type
support.variable
text source
variable
variable.language
variable.other
variable.parameter

#### Standard scopes

> \* - present on list of commonly styled scopes
> \*\* - styled by settings

comment*
    line
        double-slash
        double-dash
        number-sign
        percentage
        [character]
    block
        documentation
constant*
    numeric*
    character
        escape*
    language*
    other
entity
    name
        function*
        type*
        tag()
        section*
    other
        inherited-class*
        attribute-name*
invalid*
    illegal
    deprecated
keyword*
    control [control.import*]
    operator [operator.js*]
    other
markup
    underline**
        link
    bold**
    heading*
    italic**
    list*
        numbered
        unnumbered
    quote* (and **)
    raw
    other
meta
storage*
    type [type.method*]
    modifier
string* (and string source*)
    quoted
        single
        double
        triple
        other
    unquoted*
    interpolated
    regexp
    other
support
    function*
    class*
    type*
    constant*
    variable*
    other [other.variable*]
variable
    parameter*
    language*
    other*

## Release Notes

### 0.0.1

Mostly just the Yeoman scaffolding for a Code extention.

-----------------------------------------------------------------------------------------------------------
