POE Stack Light Documentation
=======================

The [POE stack light][blog-post] is a network controlled status indication light that is powered over the network using POE.


![POE stack light photo](stacklight-photo.jpg)

This repository contains the user and build guides, the [PCB designs][hardware-repo] and [firmware][firmware-repo] can be found in their respective git repositories.

Documentation Summary
---------------------

The documentation is broken into two documents.
The construction guide covers the steps required to build and program the stack light.
The users guide provides a reference to the function of the device along with documentation on its control APIs and DMX channels.

Both of the documents are compiled into PDFs using pandoc, the commands to compile the documents are listed below.

```
pandoc --output=output/construction-guide.pdf -H head.tex -f gfm --shift-heading-level-by -1 construction-guide.md
pandoc --output=output/user-guide.pdf -H head.tex -f gfm --shift-heading-level-by -1 user-guide.md
```


[blog-post]: https://www.scorpia.co.uk/2021/05/23/building-a-poe-enabled-lighting-fixture/
[hardware-repo]: https://github.com/Tyler-Ward/stacklight-hardware
[firmware-repo]: https://github.com/Tyler-Ward/stacklight-firmware
