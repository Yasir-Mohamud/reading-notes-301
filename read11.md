# EJS 
_______

- It stands for Embedded JavaScript templating.
- Some of the features it has is fast compilation , supports both the browser and server js, Compiles with the Express view system etc.
- The tags can be either ``` <% %> ``` or ``` <? ?>``` .
- It has to be installed using the ``` npm install ejs ```
- use case look like this =
``` js
let ejs = require('ejs'),
    people = ['geddy', 'neil', 'alex'],
    html = ejs.render('<%= people.join(", "); %>', {people: people});
```
- and the browser support looks like = 
``` html 

<script src="ejs.js"></script>
<script>
  let people = ['geddy', 'neil', 'alex'],
      html = ejs.render('<%= people.join(", "); %>', {people: people});
</script>

```
- some of the tag use cases are as follows :-
 - <% 'Scriptlet' tag, for control-flow, no output
- <%_ ‘Whitespace Slurping’ Scriptlet tag, strips all whitespace before it
- <%= Outputs the value into the template (HTML escaped)
- <%- Outputs the unescaped value into the template
- <%# Comment tag, no execution, no output
- <%% Outputs a literal '<%'
- -%> Trim-mode ('newline slurp') tag, trims following newline
- _%> ‘Whitespace Slurping’ ending tag, removes all whitespace after it
