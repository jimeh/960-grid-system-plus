# 960 Grid System Plus

This is a kind of clone/enhancement of the excellent [960 Grid System][960.gs] by [Nathan Smith][ns] to fit my personal likes and dislikes.


## Differences from original 960 Grid System

### .grid-* Classes

The `.grid-*` classes are meant to supplement the default `.grid_*` classes. The `.grid-*` classes work the exact same way, except that they are margin-less, so you can easily place multiple `.grid_*` elements within a `.grid-*` element, and gives you more flexibility with custom paddings/margins for text content.

It might be an issue of taste, but personally I don't like using the `alpha` and `omega` classes on the first and last child element. I'd rater use a different parent class, and use the `.grid_*` classes like normal within the parent grid class.

### 24 Column Grid by Default

The latest release of 960.gs includes a 24 column grid, but it can not be used with the default 960.css file which contains the 12 and 16 column grids. 960.gs+ includes all grid sizes within the one 960.css file.


## Grid Usage

Usage is identical to [960.gs][960.gs] aside from the `.grid-*` classes. To quickly explain, you can create two `.grid-8` elements with a `.container_16` element to create two columns. Within each `.grid-8` column, you can create `.grid_*` elements like normal, except you only have 8 columns of width to play with.


## Design Templates

Please refer to [960.gs][960.gs] for design templates for Photoshop, Illustrator, and many other applications.


## Generator Usage

I used the same generator (with the `.grid-*` addition) that I used for my [760 Grid System][760.gs] project.

The generator is an easy to use shell script. Just edit `grids.yml` to your needs, and run:

    ./generate-grid.rb > my_grid.css


## Legal

* Released under MIT license, of course.
* Included Eric Meyer's comprehensive browser [reset stylesheet][em], which [960.gs][960.gs] also uses.
* I borrowed the `text.css` and demo files from [960.gs][960.gs], I hope nobody minds :)


[960.gs]: http://960.gs/
[760.gs]: http://github.com/jimeh/760-grid-system
[ns]: http://sonspring.com/
[em]: http://meyerweb.com/eric/tools/css/reset/
