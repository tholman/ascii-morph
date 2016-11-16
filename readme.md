## AsciiMorph
AsciiMorph is a small stand alone javascript library for rendering ascii art and creations into elements, allowing for them to be changed out with a morphing transition.

### Demo
Here's a gif of it in action. You can also play with the demo live here.

### Usage


var element = document.querySelectorAll('pre')[0];
AsciiMorph(element, {x: 51,y: 28});

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
],

var mona_lisa = [
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
