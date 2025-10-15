# cairo
A patched version of the cairo graphics library (https://cairographics.org/) with a couple of fixes not yet in mainline:
- cairo-1.18-quartz-modifications.patch extra modifications for cairo 1.18 to avoid bitmap duplication when possible + color space management and memory leak fixes. changes proposed on the cairo mailing list.
- cairo-quartz-surface 10.14 retina scaling.patch: fixes pattern scaling issues on Retina displays with Mac OS SDK 10.14 and newer.
- cairo-win32-device-leak.patch: fixing a memory leak with cairo_device on Windows (https://bugs.freedesktop.org/show_bug.cgi?id=67171).
- cairo-scaled-font.c.patch: fixing lifecycle issue with system fonts because of cairo's internal mru cache (see this discussion https://lists.cairographics.org/archives/cairo/2016-April/027349.html)
