# MicroWebStacks
Main repo to host design and discussions

# Wishes for the future of Web
* No V-DOM lockin
* No transpilers or less transpilers and used in isolation
* Native DOM components with optional js
* no `.custom` format
* optioanl components states and liefcycle management
* No TS TSX or optional at least
* generate html,css, js from JSX
* Concatenate components easily e.g. JSX (easier than .custom template that supports no infile partials)
* native js events
* no framework black magic events or bindings (but how to bind data then? optionally e.g. getelwithid)
* spend cpu once on build time rather than milliin times on every client
## Statements
* JSX is an approach that can scale complexity hierarchically by concatenating html, css and js from a single abstraction call
* abstracting DOM manipulations from the developper can result in poor performance (https://svelte.dev/blog/virtual-dom-is-pure-overhead)


## most promising
### Solidjs
https://www.solidjs.com/
* not a framework, just a library
* has signals (states)
* compiling like svelte, or not ?
  * https://dev.to/alexmercedcoder/solidjs-react-meets-svelte-4fmm
### Astro build
https://astro.build/
* still not stable, does not handle React components properly

# Frameworks dom and jsx
![frameworks](./frameworks%20and%20dom.svg)
# Using JSX without React
https://dev.to/kartiknair/using-jsx-without-react-28eb
https://adostes.medium.com/you-dont-need-react-to-use-jsx-b78dd2a95c27

# No V-Dom
https://github.com/achou11/no-virtual-dom

* V-DOM can be a good rescue for messed up applications that have no proper DOM manipulation logic
* V-DOM is a practical SPA approach for those who do not care about bloating performance, or if application is not too complex
* V-DOM i not good for scaling the web with Micro services approaches (Micro-Front Ends)
## alternative
* Reactive fine-grained change propagation
## using html litteral strings
Easy and practicle for systematic full render scenario e.g. SVG voronoi generator
* `html` litteral string : https://github.com/WebSVG/voronoi/blob/608c5757c446a29c8925baccf4b36e016aa7bd51/src/web-js-utils.js#L29
* example svg with variables : https://github.com/WebSVG/voronoi/blob/608c5757c446a29c8925baccf4b36e016aa7bd51/src/svg_utils.js#L12

# Q&A
* What is the dom update efficiency
  * some tricks like templates and batching help https://gist.github.com/faressoft/36cdd64faae21ed22948b458e6bf04d5#file-dom_performance_reflow_repaint-md
* why don't browsers implement v-dom natively and use it to improve efficiency ?
  * they're actually doing it https://stackoverflow.com/questions/42622666/why-cant-browsers-use-a-virtual-dom-internally-as-an-optimisation
* how does solid compare to svelte
  * https://ryansolid.medium.com/javascript-ui-compilers-comparing-svelte-and-solid-cbcba2120cea
* How does solid update the DOM based on states changes ?
  * Solid Signals are getters and setters, not like react render all and let vdomdo the diff https://dev.to/alexmercedcoder/solidjs-react-meets-svelte-4fmm
* How does solid updates components visibility, with css or by inject-remove ?
* Is it possible to create an html css component out of Solid ?
  * react server side components https://reactjs.org/blog/2020/12/21/data-fetching-with-react-server-components.html
  * react in a web component https://reactjs.org/docs/web-components.html#using-react-in-your-web-components
* What is a good framework to use Solid with ?
* will nextjs support Solid ?
* Is Puppeteer a proper way to generate native web components from jsx ?
  * svelte can create spa out of the box
# TODOs
* test ASTRO with Solid
* resolve Nextjs dependencies e.g. next.router
* understand Nextjs added value e.g. routing, serving pages, SSG,... what else ?
* Find a Nextjs replacement that works with Solid.js (Express, Nest, ASTRO)
* Find a library that creates web components that can run without javascript (native DOM components)
