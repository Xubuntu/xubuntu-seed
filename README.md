# Xubuntu Seeds

**Seeds** contain the list of packages that are included in Xubuntu. We have three primary seeds, **core**, **desktop**, and **live**. Our supporting seeds include **blacklist**, **ship-live**, and **supported**. 

Changes to the Xubuntu seeds are reflected in the [xubuntu-meta](https://launchpad.net/ubuntu/+source/xubuntu-meta) source package. Each upload of **xubuntu-meta** results in new **xubuntu-core** and **xubuntu-desktop** metapackages. These metapackages pull the default applications and libraries included in Xubuntu Core and Xubuntu Desktop.

Learn more about Seed Management on the [Ubuntu Wiki](https://wiki.ubuntu.com/SeedManagement).

## Updating the Xubuntu Seeds

Our GitHub repository is a read-only mirror of the seeds as found on Launchpad. To make changes to the seeds, please [submit a new issue](https://bugs.launchpad.net/ubuntu/+source/xubuntu-meta/+filebug) for the xubuntu-meta source package with your changes.

## Primary Seeds

### Core

The core seed provides the components for a minimal Xubuntu installation. This is the seed for packages included in Xubuntu Core.

### Desktop

The desktop seed provides the components for a standard Xubuntu installation. It includes all packages from the core seed, and adds the remaining full desktop experience. This is the seed for packages included in Xubuntu Desktop.

The **desktop.minimal-remove** seed is used for the Minimal install option found in Ubiquity. Packages listed here are removed as one of the final steps of the installation process. This seed is designed to simulate a core seed installation.

### Live

The live seed provides the additional components used in a Xubuntu live environment. It includes all packages from the desktop seed, and adds a few more for installer support.

## Supporting Seeds

### Blacklist

This supporting seed includes packages which are pulled in incidentally (typically by build-dependencies) and could be trivially replaced with something that we ship. Packages listed in this seed are excluded from our metapackages.

### Ship Live

This supporting seed includes packages that are added to the live environment as an ordinary package archive. Packages listed in this seed include anything that somebody might need to install after installing the desktop in order to get online and fetch more packages.

### Supported

The supported seed includes packages that are supported by Xubuntu but not included in our base installation. This seed primarily consists of other Xfce packages.
