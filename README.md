# cairo
A patched version of the cairo graphics library (https://cairographics.org/) with a couple of fixes not yet in mainline:
- cairo-win32-private.h.patch: temp fix for https://bugs.freedesktop.org/show_bug.cgi?id=94836
- build-cairo-gl-win.patch and cairo-wgl-context.c.patch: build cairo with gl support on Windows (experimental)
- cairo-win32-device-leak.patch: fixing a memory leak with cairo_device on Windows (https://bugs.freedesktop.org/show_bug.cgi?id=67171).
- cairo-scaled-font.c.patch: fixing lifecycle issue with system fonts because of cairo's internal mru cache (see this discussion https://lists.cairographics.org/archives/cairo/2016-April/027349.html)
