---
title: Seabird 0.1
date: 2024-02-09
summary: Today, we release Seabird version 0.1. This is the first minor release, and with it we officially enter beta. Here's what's changed since our initial release last month.
authors:
  - name: Jakob Gillich
    link: https://github.com/jgillich
    image: https://2.gravatar.com/avatar/43f469474de5a70ca41002a6d8abee0cb24fd75e7c9e236bdeb918f78ded6429?size=256
---

Today, we release Seabird version 0.1. This is the first minor release, and with it we officially enter beta. Here's what's changed since our initial release last month.

_Seabird is a native (GTK) Kubernetes desktop client written in Go. We aim to make working with Kubernetes as simple as possible._

### Native Packages

Seabird now ships in the preferred app distribution format on each platform: Flatpak on Linux, MSI installer on Windows and DMG disk image on MacOS. The Flatpak can be downloaded from [Flathub](https://flathub.org/apps/dev.skynomads.Seabird), all other downloads are available from the [releases](https://github.com/getseabird/seabird/releases) page on GitHub.

### Token & Exec Authentication Support

We originally only supported authentication via certificates. In our latest release, we now also support tokens and exec-based auth providers. You can now also select a different context when you load a kubeconfig.

### Integrated Terminal

Seabird now includes a terminal, which allows you to exec into containers for debugging purposes.

![Screenshot](/images/screenshots/0.1-terminal.png)

Note: This feature is not available on Windows yet.

### Editing & Deleting Objects

We designed Seabird as a read-only resource explorer since we believe gitops is the best way to manage changes in a Kubernetes cluster. But you still want to modify objects sometimes, be it in test or development envs, and you shouldn't have to revert to kubectl to do it.

In the Yaml view, you can now right click to enable editing. On save, you are presented with a diff of the changes. Deleting objects is now also possible in the properties view.

<img src="/images/screenshots/0.1-diff.png" width="500px">

### Metrics Server Integration

Seabird now queries [metrics-server](github.com/kubernetes-sigs/metrics-server) for pod metrics, and if either requests or limits are set, displays the current usage percentage.

![Screenshot](/images/screenshots/0.1-metrics.png)

### Live Updates

Seabird now watches for changes and automatically displays them.

### The Road Ahead

Over 100 changesets have been committed in the last few weeks, too many to mention in this post. All essential features are now implemented, but there is much more to do. We are confident to promote Seabird to beta status, but still advise caution when using it with production clusters.

We thank to all our contributors and testers! This is only the beginning of our journey, we have great plans such as an extension interface or integrated resource documentation browser. But to fully realize our vision, we need funding. That's why we'll be introducing a paid subscription soon that will provide benefits such as direct priority support. But not to worry, an unlimited free version will always be available, and all code is public under the MPLv2 license.
