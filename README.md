#Late Afternoon

## Design rationale
This is an icon theme for linux systems using freedesktop's icon naming scheme, 
as well as GNOME/KDE specific names.

The icons are all scalable vector graphics (SVG). Application icons have a 
standard size of 48px, symbolic icons 16px and panel icons 24px. This means 
they are designed to be pixel perfect at that size.

The color palette used is the Echo icon palette coming with inkscape. Different 
colors are only used for icons which have a unique color identity.

Application icons are designed to be nearly square (very small corner radius) 
and relatively flat with a central shape identifying the application. The 
central shape has a "long shadow" as an eye catcher which points diagonally to 
the south-east corner.

## Imported icons from other themes
All status, symbolic, mimetype and actions icons are taken from the Numix 
theme, see [Numix Project](numixproject.org).

Some shapes of application icons are inspired by the [FlatWoken 
theme](https://github.com/alecive/FlatWoken).

## TODO
* Icons that should be made (by priority, important first)
  - Brightness & Lock (system-lock-screen)
  - Big trash icon
  - ...

* Reconstruct color palette from numix icons?


## Technicalities
If you clone the repo, you will see that the theme contains no soft links as 
other themes do. To make life easier for me, I wrote a shell script called 
`distribute.sh` and there are `make_links` files in the subfolders which do the 
actual linking. So if you cloned it and want to use the theme, go into the top 
folder and type

> ./distribute -s -i

This will copy the SVGs in the subfolders defined in index.theme,  scour them 
([Scour](http://www.codedread.com/scour/) has to be installed) and create a 
bunch of symbolic links. There are also other options, see `./distribute -h`.

## Contact and Download

You can find a packaged version of the theme at 
[Deviantart](http://manicfold.deviantart.com/art/LateAfternoon-444389530).  
There you can also reach me throught the comments.
