---
title: Seabird 0.3
date: 2024-04-03
summary: Today, we release Seabird version 0.3.
authors:
  - name: Jakob Gillich
    link: https://github.com/jgillich
    image: https://2.gravatar.com/avatar/43f469474de5a70ca41002a6d8abee0cb24fd75e7c9e236bdeb918f78ded6429?size=256
---

Today, we release Seabird version 0.3. This release features major changes to the layout of the app.

_Seabird is a native cross-platform Kubernetes IDE written in Go & GTK._

### Object Overlay

Object properties are now displayed in a sliding overlay the navigation is always visible at all sizes. This is a pattern used by Lens as well, and we think it is a better compromise to optimize space usage.

![Screenshot](/images/screenshots/0.3-overlay.png)

### Navigation

All resources are now displayed in the navigation sidebar, and favourites are added and removed with a right click.

### Editor

The resource editor now works with all resources and a new edit button in the object property view now opens the source in the editor.

### Object Pinning

Objects can now be pinned, which makes them available in the navigation. Besides quicker access to objects, it also enables you to keep terminal session running in the background, which would normally be terminated when navigating to another object.

![Screenshot](/images/screenshots/0.3-pin.png)

### Read-only mode

The cluster preferences now have a toggle to enable read-only mode, which will hide all mutating features. This can help prevent accidental modifications on production clusters.

To download the new version, go [here](https://github.com/getseabird/seabird/releases) or get the [Flatpak](https://flathub.org/apps/dev.skynomads.Seabird). For questions and feedback, [join the discussion](https://github.com/getseabird/seabird/discussions/77).
