
# EJS

* EJS is a simple templating language that lets you generate HTML markup with plain JavaScript. No religiousness about how to organize things. No reinvention of iteration and control-flow. It's just plain JavaScript.

------------------------------------------------

 ## Advanteges :
* Use plain JavaScript.
* Fast development time.
* Simple syntax.
* Speedy execution.
* Easy debugging.
* Active development.

--------------------------------

## Features
* Fast compilation and rendering.
* Simple template tags: <% %>.
* Custom delimiters (e.g., use [? ?] instead of <% %>).
* Sub-template includes.
* Ships with CLI.
* Both server JS and browser support.
* Static caching of intermediate JavaScript.
* Static caching of templates.
* Complies with the Express view system.

------------------------------------

## Tags
* `<%` 'Scriptlet' tag, for control-flow, no output.
* `<%_` ‘Whitespace Slurping’ Scriptlet tag, strips all whitespace before it.
* `<%=` Outputs the value into the template (HTML escaped).
* `<%-` Outputs the unescaped value into the template.
* `<%#` Comment tag, no execution, no output.
* `<%%` Outputs a literal `'<%'`.
* `%>` Plain ending tag.
* `-%>` Trim-mode ('newline slurp') tag, trims following newline.
* `_%>` ‘Whitespace Slurping’ ending tag, removes all whitespace after it.
