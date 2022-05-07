# MicroWebStacks
Main repo to host design and discussions

https://github.com/orgs/MicroWebStacks/discussions/2

https://github.com/orgs/MicroWebStacks/discussions/3

https://github.com/orgs/MicroWebStacks/discussions/4

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

## alternative
* Reactive fine-grained change propagation
## using html litteral strings
Easy and practicle for systematic full render scenario e.g. SVG voronoi generator
* `html` litteral string : https://github.com/WebSVG/voronoi/blob/608c5757c446a29c8925baccf4b36e016aa7bd51/src/web-js-utils.js#L29
* example svg with variables : https://github.com/WebSVG/voronoi/blob/608c5757c446a29c8925baccf4b36e016aa7bd51/src/svg_utils.js#L12

# Q&A
* how does solid compare to svelte
  * https://ryansolid.medium.com/javascript-ui-compilers-comparing-svelte-and-solid-cbcba2120cea
* How does solid update the DOM based on states changes ?
  * Solid Signals are getters and setters, not like react render all and let vdomdo the diff https://dev.to/alexmercedcoder/solidjs-react-meets-svelte-4fmm
* How does solid updates components visibility, with css or by inject-remove ?
* Is it possible to create an html css component out of Solid ?
* What is a good framework to use Solid with ?
* will nextjs support Solid ?

# TODOs
* test ASTRO with Solid

# Help wanted
* Find a Nextjs equivalent that works with Solid.js (Express, Nest, ASTRO)
* Find a library that creates web components that can run without javascript (native DOM components)
