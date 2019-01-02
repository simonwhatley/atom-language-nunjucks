# Nunjucks snippets for Atom

## Available snippets

|Name|Shortcut|Notes|
|-------------------------|-------------------------|-------------------------|
|asyncAll|asyncall|asyncAll is similar to asyncEach, except it renders all the items in parallel, preserving the order of the items. This is only helpful if you are using asynchronous filters, extensions, or loaders. Otherwise you should never use this. [Read the docs](https://mozilla.github.io/nunjucks/templating.html#asyncall)|
|asynchEach|asyncheach|asyncEach is an asynchronous version of for. You only need this if you are using a custom template loader that is asynchronous; otherwise you will never need it. Async filters and extensions also need this, but internally loops are automatically converted into asyncEach if any async filters and extensions are used within the loop. [Read the docs](https://mozilla.github.io/nunjucks/templating.html#asynceach)|
|block|block|A block defines a section on the template and identifies it with a name. This is used by template inheritance. Base templates can specify blocks and child templates can override them with new content. [Read the docs](https://mozilla.github.io/nunjucks/templating.html#block)|
|call|get|A call block enables you to call a macro with all the text inside the tag. This is helpful if you want to pass a lot of content into a macro. The content is available inside the macro as `caller()`. [Read the docs](https://mozilla.github.io/nunjucks/templating.html#call)|
|comment|comment|You can write comments using `{#` and `#}`. Comments are completely stripped out when rendering. [Read the docs](https://mozilla.github.io/nunjucks/templating.html#comments)|
|elif|elif|Alternative condition in an if block. [Read the docs](https://mozilla.github.io/nunjucks/templating.html#if)|
|else|else|Else condition in an if block. [Read the docs](https://mozilla.github.io/nunjucks/templating.html#if)|
|extends|extends|Extends is used to specify template inheritance. The specified template is used as a base template. [Read the docs](https://mozilla.github.io/nunjucks/templating.html#extends)|
|filter|filter|A filter block allows you to call a filter with the contents of the block. Instead passing a value with the | syntax, the render contents from the block will be passed. [Read the docs](https://mozilla.github.io/nunjucks/templating.html#filter)|
|for|for|For iterates over arrays and dictionaries. [Read the docs](https://mozilla.github.io/nunjucks/templating.html#for)|
|from|from|From imports specific values from a template into the current namespace. [Read the docs](https://mozilla.github.io/nunjucks/templating.html#import)|
|if elif|ifelif|If block with an alternative condition. [Read the docs](https://mozilla.github.io/nunjucks/templating.html#if)|
|if else|ifelse|If block with an else condition. [Read the docs](https://mozilla.github.io/nunjucks/templating.html#if)|
|if|if|If tests a condition and lets you selectively display content. It behaves exactly as the JavaScript if behaves. [Read the docs](https://mozilla.github.io/nunjucks/templating.html#if)|
|import|import|Import loads a different template and allows you to access its exported values. Macros and top-level assignments (done with set) are exported from templates, allowing you to access them in a different template. [Read the docs](https://mozilla.github.io/nunjucks/templating.html#import)|
|include|include|Include pulls in other templates in place.It\'s useful when you need to share smaller chunks across several templates that already inherit other templates. [Read the docs](https://mozilla.github.io/nunjucks/templating.html#include)|
|macro|macro|Macro allows you to define reusable chunks of content. It is similar to a function in a programming language. [Read the docs](https://mozilla.github.io/nunjucks/templating.html#macro)|
|pipe|pipe|A pipe filter allows you to call a filter within the context of a variable, e.g., `{{ variable | filter }}`. [Read the docs](https://mozilla.github.io/nunjucks/templating.html#filters)|
|raw|raw|If you want to output any of the special nunjucks tags like `{{`, you can use raw and anything inside of it will be output as plain text. [Read the docs](https://mozilla.github.io/nunjucks/templating.html#raw)|
|set|set|Create or modify a variable. [Read the docs](https://mozilla.github.io/nunjucks/templating.html#set)|
|super|super|Render the contents of the parent block inside a child block by calling super. [Read the docs](https://mozilla.github.io/nunjucks/templating.html#super)|
|variable|var|Output a variable from the template context. [Read the docs](https://mozilla.github.io/nunjucks/templating.html#variables)|
|verbatim|verbatim|Verbatim has identical behaviour as raw. It is added for compatibility with the Twig verbatim tag. [Read the docs](https://mozilla.github.io/nunjucks/templating.html#verbatim)|