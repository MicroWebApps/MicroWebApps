# MicroWebStacks
Main repo to host design and discussions

# Wishes for the future of Web
* No V-DOM lockin
* No transpilers or isolated components transpilation
* Native DOM components with optional js
* no `.custom` format
* optioanl components states and liefcycle management
* No TS TSX or optional at least
* generate html,css, js from JSX
* Concatenate components easily e.g. JSX
* native js events
* no framework black magic events or bindings
## Statements
* JSX is an approach that can scale complexity hierarchically by concatenating html, css and js from a single abstraction call
* abstracting DOM manipulations from the developper can result in poor performance (https://svelte.dev/blog/virtual-dom-is-pure-overhead)


## most promising
### Solidjs
https://www.solidjs.com/
* not a framework, just a library
* has signals (states)
### Astro build
https://astro.build/
* still not stable, does not handle React components properly

 [] test ASTRO with Solid

![frameworks](./frameworks%20and%20dom.svg)
# Using JSX without React
https://dev.to/kartiknair/using-jsx-without-react-28eb
https://adostes.medium.com/you-dont-need-react-to-use-jsx-b78dd2a95c27

# No V-Dom
https://github.com/achou11/no-virtual-dom

* V-DOM can be a good rescue for messed up applications that have no proper DOM manipulation logic
* V-DOM is a practical SPA approach for those who do not care about bloating performance, or if application is not too complex
* V-DOM i not good for scaling the web with Micro services approaches (Micro-Front Ends)


## using html litteral strings
Easy and practicle for systematic full render scenario e.g. SVG voronoi generator
* `html` litteral string : https://github.com/WebSVG/voronoi/blob/608c5757c446a29c8925baccf4b36e016aa7bd51/src/web-js-utils.js#L29
* example svg with variables : https://github.com/WebSVG/voronoi/blob/608c5757c446a29c8925baccf4b36e016aa7bd51/src/svg_utils.js#L12

# Questions
* How does solid update the DOM based on states changes ?
* How does solid updates components visibility, with css or by inject-remove ?
* Is it possible to create an html css component out of Solid ?
