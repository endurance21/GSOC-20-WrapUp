

<p align="center">
  <img src="/assets/images/headingFinal2.png"  width="300" style="margin-left:50%;transform:translateX(-50%);"/>
</p

<p>

  # Project Overview
  This projects aimed at ::
  * REVAMPING the current modules system from ``require.js`` to ``ESModules``
  
  * Writing   Audio Nodes in `ES6 classes` way rather than older `function Constructor` way ! 
  
  * REVAMPING Testing Architecture of the codebase 
  
</p>

## The New Module system 
Javascript has  a great history of module sytems , from ``IIFE`` to ``ESM 2015`` we have come a long  way to finally own a native module support ! [here is a great tutorial for the same ](https://www.youtube.com/watch?v=qJWALEoGge4&t=3s) .
Earlier p5.js-sound library was dependent on  `require.js` for making the codebase modular , which was very cumbersome to maintain and scale , However , now we have been shifted to ESM .

Perks of having native ESM -->

 * More cleaner way to write modules ( export/import keywords instead of require()).
 * Named exports has always been great feature of ESM .
 * Modules can be loaded from a URL, which is not there in Commonjs .

[More on ESM Modules](https://nodejs.org/api/esm.html#esm_ecmascript_modules)



This is not it !,
Many browsers does not support many ES6 features such as `export/import` , ``classes``  , ``arrow functions `` .. etc , and here we needed the backward compatiblity , and BABEL (JS TRANSPILER ) is 
here to save the day  , which with help of WEBPACK ( module bundler ) ships the final code in older verion of ES ! YES you heard it right , we write code in NODE.JS env with modern JS syntax but at the end of the day we ship the code in older ES versions to ensure compatiblity in all browsers ! 



[More On BABEL ](https://babeljs.io/docs/en/babel-preset-env)

[More On WEBPACK ](https://webpack.js.org/concepts/ )


[THIS PR SUCCESSFULLY REVAMPED THE CODEBASE TO THE NEW MODULE SYSTEM ](https://github.com/processing/p5.js-sound/pull/489)



## Class Based Audio Nodes 

The introduction of es6 classes into the JS world , was a great relief for developers out there , though its a syntactic sugar for Constructor Functions yet it abstracts out the protypal approach under the hood ,leaving a cleaner interface to the developers .

[More on ES6 CLASSES ](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes)

when it comes to AUDIO GRAPHS , where one node is connected to so many other nodes and inherit property from its parent nodes , a more robust and cleaner  implementation of Nodes was required and ES6 classes rocked the way  .

Following PR REVAMPED the AUDIO NODES  to ES6 Classes 

[#502](https://github.com/processing/p5.js-sound/pull/502)
[#503](https://github.com/processing/p5.js-sound/pull/503)
[#508](https://github.com/processing/p5.js-sound/pull/508)
[#509](https://github.com/processing/p5.js-sound/pull/509)
[#514](https://github.com/processing/p5.js-sound/pull/514)
[#515](https://github.com/processing/p5.js-sound/pull/515)
[#516](https://github.com/processing/p5.js-sound/pull/516)
[#517](https://github.com/processing/p5.js-sound/pull/517)
[#518](https://github.com/processing/p5.js-sound/pull/518)
[#519](https://github.com/processing/p5.js-sound/pull/519)
[#520](https://github.com/processing/p5.js-sound/pull/520)
[#521](https://github.com/processing/p5.js-sound/pull/521)
[#522](https://github.com/processing/p5.js-sound/pull/522)
[#523](https://github.com/processing/p5.js-sound/pull/523)
[#524](https://github.com/processing/p5.js-sound/pull/524)
[#525](https://github.com/processing/p5.js-sound/pull/525)
[#526](https://github.com/processing/p5.js-sound/pull/526)
[#527](https://github.com/processing/p5.js-sound/pull/527)
[#528](https://github.com/processing/p5.js-sound/pull/528)
[#530](https://github.com/processing/p5.js-sound/pull/530)
[#531](https://github.com/processing/p5.js-sound/pull/531)
[#532](https://github.com/processing/p5.js-sound/pull/532)
[#533](https://github.com/processing/p5.js-sound/pull/533)
[#534](https://github.com/processing/p5.js-sound/pull/534)
[#535](https://github.com/processing/p5.js-sound/pull/535)
[#536](https://github.com/processing/p5.js-sound/pull/536)
[#537](https://github.com/processing/p5.js-sound/pull/537)
[#538](https://github.com/processing/p5.js-sound/pull/538)
[#539](https://github.com/processing/p5.js-sound/pull/539)

