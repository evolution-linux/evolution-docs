# Installation

This section includes general information about the process of installing EvolutionOS.
For specific guides, see the "[Advanced Installation](./guides/index.md)"
section.

## Base system requirements

EvolutionOS can be installed on very minimalist hardware, though we recommend the
following minimums for most installations:

| Architecture | CPU              | RAM  | Storage |
|--------------|------------------|------|---------|
| x86_64-glibc | x86_64           | 96MB | 700MB   |
| x86_64-musl  | x86_64           | 96MB | 600MB   |
| i686-glibc   | Pentium 4 (SSE2) | 96MB | 700MB   |

Note that xfce image installations require more resources.

EvolutionOS is not available for the i386, i486, or i586 architectures.

Before installing musl EvolutionOS, please read [the "musl" section](./musl.md) of this
Handbook, so that you are aware of software incompatibilities.

It is highly recommended to have a network connection available during install
to download updates, but this is not required. ISO images contain installation
data on-disk and can be installed without network connectivity.

## Downloading installation media

The most recent live images can be downloaded from
<https://evolution-linux.github.io/download>. Previous releases
can be found under <https://github.com/evolution-linux/evolution-linux.github.io/releases>, organized by
date.
