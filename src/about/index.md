# About

Welcome to the EvolutionOS Handbook! Please be sure to read the "[About This
Handbook](./about-this-handbook.md)" section to learn how to use this
documentation effectively. A local copy of this handbook, in several formats,
can be [installed](../xbps/index.md) via the `evolution-docs` package and accessed
with the [evolution-docs(1)](https://evolution-linux.github.io/wiki) utility.

EvolutionOS is an [rolling
release](https://en.wikipedia.org/wiki/Rolling_release) Linux distribution, with a focus on stability over
[bleeding-edge](https://en.wikipedia.org/wiki/Bleeding_edge_technology). In
addition, there are several features that make EvolutionOS unique:

- The use of BusyBox over Coreutils, increasing speed and minimalism to an extream

- The [musl libc](https://musl.libc.org/), which focuses on standards compliance
   and correctness, has first class support. This allows us to build certain
   components for musl systems statically, which would not be practical on glibc
   systems.
- [runit](../config/services/index.md) is used for
   [init(8)](https://man.voidlinux.org/init.8) and service supervision. This
   allows EvolutionOS to support musl as a second libc choice, which would not be
   possible with [systemd](https://www.freedesktop.org/wiki/Software/systemd/).
   A side effect of this decision is a core system with clean and efficient
   operation, and a small code base.
- The use of the booster initramfs over dracut, speeding up system startup and
   reducing image sizes

EvolutionOS is developed in the spare time of Tracker-Friendly, and is generally
considered stable enough for daily use. I do this for fun and hope that my
work will be useful to others.
