# game_palette_unifier
Enumerate all pixel colors used in game all game images, and then 
collapse all like colors into a single, small, coherent palette across 
all graphics.

## intro
It might seem counter-intuitive, but most computer games benefit 
significantly from having as few colors in the artwork as needed. A 
balance is needed, too few colors and it will be difficult to express 
all needed visual effects. However, have too many colors and your 
graphics will feel like they do not fit together.

Opensource and independent games suffer the most, as resources are 
tight, many games use open game assets created by several different 
artists. The different artists might have different art styles and this 
might manifest into the final product as graphics which feel out of 
place.

Simply ensuring that all game graphics utilize the same restricted 
palette can go a long way to mitigate this issue, making the final 
product feel the way it should.
Utilizing a smaller palette can also help you reduce the size of your 
image files, making your game easier to deploy.

## usage
All you need to do is point gpu to your game images directory and 
specify how large you want your palette to be. gpu should be smart 
enough to select colors that you need and map other colors to the best 
color in your palette.

If the resultant images are not suitable, you can consider adjusting 
your palette size, or by entering manual mapping mode.
In manual mapping mode, gpu will still auto-map a palette for you, but 
before creating a new set of artwork, gpu will allow you to adjust the 
choices it has made.

Note: This application works only on BMPs. If you intend to use another 
image format in your game, you can use ImageMagick's convert to change 
between image formats for the purpose of using this application, and 
then back to your preferred game format (assuming you are using a 
format supported by ImageMagick).
