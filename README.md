# LinVst*

-----

LinVst* may help with some Linux vst incompatability problems that occur in some Linux DAWS, such as gtk errors that occur in some Linux vst plugins (lsp vst plugins/amsynth vst plugin etc).

LinVst* loads a Linux vst and manages it within a Linux DAW.

-------

How to use,

linvst*.so gets renamed to pluginname*.so

For example,

For a linux vst plugin named Delay.so, linvst*.so would get renamed to Delay*.so

The plugin name with an asterisk contained in it's name would then be used inside of a Linux DAW instead of the original plugin name.

For instance, Delay*.so would then be used inside of a Linux DAW (not the original Delay.so)

Delay.so and Delay*.so need to be kept in the same location after the renaming as they are then a matched pair.

To install,

Copy lin-vst-server to /usr/bin

convert(rename) linvst*.so to the plugin name.

linvst*convert can do the name conversion automatically for multiple plugins in a folder.

64 bit Linux vst's only.

-----------

The window embedded version works in Linux Reaper and Linux Bitwig.

The standalone window version works in Tracktion.

LinVst-lx2.zip and LinVst-lx2embed.zip contain binaries.

The pluginterfaces folder from the Steinberg vst sdk is needed for compiling.

The x11-dev package is also needed for compiling.

sudo make clean

make

sudo make install

-----------

The lsp vst plugins need the lsp-plugins-vst-core.so file copied to /usr/lib/vst for plugin scanning to be successful.
