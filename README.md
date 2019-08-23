## makefont - Easily display TTF fonts in OpenGL 1.2

This is a small tool from the freetype-gl project: https://github.com/rougier/freetype-gl

This version was taking from an old version of the source tree from 2014, specifically commit `683bae3b423dee824a772a9b02e82ab1680ee387`.

The reason I used an old version is that it includes an example using OpenGL immediate mode (aka fixed function) and a very simple function, with no dependency on the actual freetype library, to display any TTF font converted to bitmap format using the `makefont` tool. Example code in `demo-makefont.c` and `arial-16.h`.

I wanted an immediate mode version to use on older game consoles such as the Dreamcast and original Xbox. There are newer, shader-based examples in the master branch of that repo.

I moved just this tool and example into it's own repository so that I could more easily modify it for my use-case.

---
Note: Currently only tested building on macOS, but Linux should also work. I removed the Windows stuff from Cmake to clean it up as I don't use Windows.