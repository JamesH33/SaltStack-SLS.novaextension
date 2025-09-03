**SaltStack SLS** provides syntax highlighting for SaltStack sls files.

![Syntax Highlighting Example](https://github.com/JamesH33/SaltStack-SLS.novaextension/blob/main/example.png?raw=true)

## Syntax Highlighting
This language extension combines the basics of YAML and Jinja syntax and enables highlighting. This allows your themes to properly highlight any SaltStack files that use both.

This is a very barebones extension. It relies on the old regex syntax definitions instead of Tree-sitter, frankly because I have neither the time nor knowledge to set it up that way. This extension also currently does not do anything fancier than syntax highlighting and allowing the CMD+/ comment hotkey. 

The current syntax highlighting that works:
- key highlighting: `key: value`
- string highlighting with both single and double quotes
- Jinja expressions: `{{ jinja stuff }}`
- Jinja statements: `{% other jinja stuff %}`
- Booleans: `true/True`, `false/False`, `null/Null`
- Comments: `# Comment`
- Numbers

The current highlighting from YAML is known not to work; not sure if I will add these in the future
- Anchors: `&foo`
- Aliases: `*bar`
- Tags: `!tag`
- Scalars: `|` or `>`

## Attribution
SaltStack and the SaltStack logo (contained here as extension.png) are both copyrighted by the [SaltStack Team](https://saltproject.io), used under the Apache 2.0 license. You may obtain a copy of the license at http://www.apache.org/licenses/LICENSE-2.0