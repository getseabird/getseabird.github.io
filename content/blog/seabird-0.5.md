---
title: Seabird 0.5
date: 2024-07-18
summary: Today, we release Seabird version 0.5.
authors:
  - name: Jakob Gillich
    link: https://github.com/jgillich
    image: https://2.gravatar.com/avatar/43f469474de5a70ca41002a6d8abee0cb24fd75e7c9e236bdeb918f78ded6429?size=256
---

Today, we are launching Seabird version 0.5. Here are the latest updates.

#### Resource Navigation Status

The resource navigation has been enhanced to show the count of both healthy and unhealthy objects, allowing you to quickly identify any issues within your cluster. To minimize API load, it is only visible for favorited resources.

![Screenshot](/images/screenshots/0.5-main.png)

#### Object Dialog

The object page now uses the bottom sheet dialog widget, which slides in from the bottom. This is particularly beneficial for touch device users.

![Screenshot](/images/screenshots/0.5-dialog.png)

#### Port Forwarding

With just a click of a button, you can now easily forward container ports to localhost.

#### Additional Print Columns

Additional print columns on custom resource definitions are now supported.

#### New Properties

New properties and columns have been added for Job, CronJob, ReplicaSet, PersistentVolume and PersistentVolumeClaim.

#### More Resilient Watch

The watch logic has been rewritten to use informer. It should now be more resilient to connection drops.

### Download

To download the latest update, go to [releases](https://github.com/getseabird/seabird/releases) or get the [Flatpak](https://flathub.org/apps/dev.skynomads.Seabird). Any queries or feedback can be shared by [creating a discussion](https://github.com/getseabird/seabird/discussions).
