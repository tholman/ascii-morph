## AsciiMorph
AsciiMorph is a small stand alone javascript library for rendering ascii art and creations into elements, allowing for them to be changed out with a morphing transition.

### Demo
Here's a gif of it in action. You can also play with the [demo live here](http://codepen.io/tholman/full/BQLQyo).

![Ascii Morph in action](https://s3.amazonaws.com/tholman.com/static-assets/ascii-morph-demo.gif)

### Usage

You'll need an `dom` element for the ascii's to be rendered within.

```html
<!-- Pre elements are perfect for this. -->
<pre class="ascii-element">
</pre>
```

Next up, you will want to initialize the library. The second parameter is the `width` and `height` properties you want in your rendering square. The ascii will be rendered centered within them, and fill the rest with white space. Naturally this looks best with monospace fonts.

```javascript
// Initialize AsciiMorph
var element = document.querySelector('pre');
AsciiMorph(element, {x: 50,y: 25});
```

Then you can get to the fun, rendering elements, and morphing between them.

```javascript

// First, define some ascii art.
var bird = [
 "                             /",
 "                            /",
 "                           /;",
 "                          //",
 "                         ;/",
 "                       ,//",
 "                   _,-' ;_,,",
 "                _,'-_  ;|,'",
 "            _,-'_,..--. |",
 "    ___   .'-'_)'  ) _)\\|      ___",
 "  ,'\"\"\"`'' _  )   ) _)  ''--'''_,-'",
 "-={-o-  /|    )  _)  ) ; '_,--''",
 "  \\ -' ,`.  ) .)  _)_,''|",
 "   `.\"(   `------''     /",
 "     `.\\             _,'",
 "       `-.____....-\\\\",
 "                 || \\\\",
 "                 // ||",
 "                //  ||",
 "            _-.//_ _||_,",
 "              ,'  ,-'/"
 ]

var mona = [
 "         ____",
 "        o8%8888,",
 "      o88%8888888.",
 "     8'-    -:8888b",
 "    8'         8888",
 "   d8.-=. ,==-.:888b",
 "   >8 `~` :`~' d8888",
 "   88         ,88888",
 "   88b. `-~  ':88888",
 "   888b ~==~ .:88888",
 "   88888o--:':::8888",
 "   `88888| :::' 8888b",
 "   8888^^'       8888b",
 "  d888           ,%888b.",
 " d88%            %%%8--'-.",
 "/88:.__ ,       _%-' ---  -",
 "    '''::===..-'   =  --.  `",
 ]
 
// Then, you can render (will render instantly)
AsciiMorph.render(bird);

// Then morph, to a new creation
AsciiMorph.morph(mona);

```

### License

Copyright (c) 2016 Tim Holman - http://tholman.com

[The MIT License](https://github.com/tholman/ascii-morph/blob/master/license.md)
