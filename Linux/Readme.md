This is a modified subset of the Blackbox framework 1.7.2 used to test my [Oberon+](https://github.com/rochus-keller/Oberon/blob/master/documentation/The_Programming_Language_Oberon%2B.adoc) parser and validator.

I originally downloaded the framework from https://blackbox.oberon.org/unstable/master/bbcb-1.7.2~b1.154.tar.gz on 2020-12-12 (which seems to correspond with https://github.com/bbcb/bbcp commit 9b3b60e on 14 Aug) and run *odcread* (see [this post](https://community.blackboxframework.org/viewtopic.php?f=32&t=272&p=1760&hilit=odcread#p1760)) on each Mod/*.odc file to create the corresponding source code text file.

Then I removed the Cons, Dev, Dev2, Obx, Sql, and parts of the Gtk2 and Lin subsystems and converted the source code to Oberon+ using my [OberonViewer 0.8.4](https://github.com/rochus-keller/Oberon#code-browser-features). Some of the resulting files needed manual fixes. 

Then I removed all procedures (and some of the types and consts) from the Gtk2* and Lin* files which are no longer used by the subset of the remaining subsysytems. The resulting code has ~73 kLOC (physical code lines, no whitespace or comment only lines).

The original Blackbox framework source files are licensed under a BSD 2-clause license (see file LICENSE.txt).

