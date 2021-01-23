This is a modified subset of the Blackbox framework 1.7.2 used to test my [Oberon+](https://github.com/rochus-keller/Oberon/blob/master/documentation/The_Programming_Language_Oberon%2B.adoc) parser and validator.

I originally downloaded the framework from https://blackboxframework.org/stable/blackbox-1.7.2.zip on 2020-11-08 and run *odcread* (see [this post](https://community.blackboxframework.org/viewtopic.php?f=32&t=272&p=1760&hilit=odcread#p1760)) on each Mod/*.odc file to create the corresponding source code text file.

Then I removed the Com, Ctl, Dev, Obx, Ole, Sql and parts of the Win subsystems and converted the source code to Oberon+ using my [OberonViewer 0.8.4](https://github.com/rochus-keller/Oberon#code-browser-features). About ten of the hundred resulting obx files required some manual fixes and additions.

The original Blackbox framework source files are licensed under a BSD 2-clause license (see file License.txt).

Here is a screenshot of the current state of the Oberon+ IDE with the Blackbox framework loaded:

![Oberon+ IDE Screenshot](http://software.rochus-keller.info/screenshot_obx_ide_0.1.png)

The ~96 kLOC (physical code lines, no whitespace or comment only lines) require less than two seconds to parse and validate on my HP EliteBook 2530p. See https://github.com/rochus-keller/Oberon for more information.
