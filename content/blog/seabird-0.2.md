---
title: Seabird 0.2
date: 2024-03-01
summary: Today, we release Seabird version 0.2.
authors:
  - name: Jakob Gillich
    link: https://github.com/jgillich
    image: https://2.gravatar.com/avatar/43f469474de5a70ca41002a6d8abee0cb24fd75e7c9e236bdeb918f78ded6429?size=256
---

Today, we release Seabird version 0.2. Much has changed since 0.1, so here's a quick overview of the most notable changes.

_Seabird is a native cross-platform Kubernetes GUI written in Go._

### Responsive Layout

The sidebar is now hidden by default to leave more room for the content. This means the app will work much better in windowed mode and on low resolution displays. The sidebar will reappear as you resize the window.

![Screenshot](/images/screenshots/0.2-main.png)

### Resource Editor

The app now comes with a resource editor that puts the API reference right at your fingertips. Note that this only supports the core API at the moment.

![Screenshot](/images/screenshots/0.2-editor.png)

### Column Sorting

Most list columns are now sortable.

### Common Kubeconfig Paths

Common Kubeconfig paths like `~/.kube/config` and `$KUBECONFIG` are now imported automatically at startup.

### Platform Styles

We now emulate native styles of Mac and Windows via color palettes and window controls.

![Screenshot](/images/screenshots/0.2-mac.png)

### Purchase Banner

The start window now comes with a small banner requesting purchase of a license. This is optional and does not unlock additional features, however it gives you access to direct email support. Bug reports and feature requests from subscribed users will be treated with a higher priority.

Everyone loves open source, but funding its development is still a big challenge. A share of the revenue will be reinvested into related open source projects.

![XKCD Comic](https://imgs.xkcd.com/comics/dependency.png)

To download the new version, go [here](https://github.com/getseabird/seabird/releases) or get the [Flatpak](https://flathub.org/apps/dev.skynomads.Seabird).

For questions and comments, [join the discussion](https://github.com/getseabird/seabird/discussions/58).
