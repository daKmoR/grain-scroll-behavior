[![Polymer Version](https://img.shields.io/badge/polymer-v2-blue.svg)](https://www.polymer-project.org)

# \<grain-scroll-behavior\>

Using this behavior you do get a onScroll function with the current scroll position.

## Installation

```sh
$ bower install --save daKmoR/grain-scroll-behavior
```

## Getting Started

Import the package.

```html
<link rel="import" href="/bower_components/grain-scroll-behavior/grain-scroll-behavior.html">
```

Create your element using this behavior utilizing onScroll.

```js
class GrainResponsiveBehaviorExample extends GrainScrollBehavior(Polymer.Element) {
  ready() {
    super.ready();
    this.scrollLoop(); // init/start the behavior
  }

  onScroll(scrollTop) {
    // your code for example something like this
    if (scrollTop > this.vhToPx('10vh')) {
      // ...
    }
  }
}
```

*For more information, see the API documentation.*

## Working on the Element

First, make sure you have the [Polymer CLI](https://www.npmjs.com/package/polymer-cli) installed.
* View the Element via `polymer serve`
* Run tests via `polymer test`