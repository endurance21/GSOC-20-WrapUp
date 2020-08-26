

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

 * More cleaner way to write modules ( export/import keywords instead of require())
 * Named exports has always been great feature of ESM 
 * Modules can be loaded from a URL, which is not there in Commonjs  !

[for more on ESM Modules](https://nodejs.org/api/esm.html#esm_ecmascript_modules)

[This huge PR sucessfully revamped the codebase from ``require()`` to ``export/import``](https://github.com/processing/p5.js-sound/pull/489)


