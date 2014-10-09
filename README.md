# radial-progress

Forked from [brightpoint inc](http://www.brightpointinc.com/clients/brightpointinc.com/library/radialProgress/index.html)

`npm install radial-progress`

## notes
This was forked in a jiffy, I know it is not structured well, I plan to fix
it as soon as I get a free moment. Please do not create issues telling me
about the bad practices. I will be more than happy to recieve pull requests.

## usage
``` javascript
var radialProgress = require('./index');
var DEFAULT_DIAMETER = 150;

function makeRadialGraph (selector, value, diameter) {
  var containEl = document.querySelector(selector);
  var diameter = diameter ? diameter : DEFAULT_DIAMETER;

  var radialGraphComponent = radialProgress(containEl)
                             .diameter(diameter)
                             .value(value);

  return radialGraphComponent;
}

var radialGraph = makeRadialGraph('.radial-example', 75);
radialGraph.render();

```

You will also want to include(possibly override) the css
sound in style.css in the project root.

## LICENSE

originally licensed as MIT, still licensed as MIT
(license at top of index.js)
