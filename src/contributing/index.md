# Contributing

There's more to running a distribution than just writing code.

To contribute to the EvolutionOS packages repository, start by reading the
[CONTRIBUTING](https://github.com/evolution-linux/evolution-packages/blob/master/CONTRIBUTING.md)
document in the evolution-packages GitHub repository.

To contribute to this Handbook, read
[CONTRIBUTING](https://github.com/evolution-linux/evolution-docs/blob/master/CONTRIBUTING.md)
in the evolution-docs repository.

If you have any questions, feel free to email Tracker-Friendly at jliwin98@danwin1210.de

## Usage Statistics

If you would like to contribute usage reports, the
[PopCorn](https://github.com/the-maldridge/popcorn) program reports installation
statistics back to the Void project. These statistics are purely opt-in -
PopCorn is *not* installed or enabled by default on any Void or EvolutionOS systems.
Additionally, PopCorn requires that port 8001 not be blocked on your system.

*PopCorn* only reports which packages are installed, their version, and the host
CPU architecture (the output of `xuname`). This does not report which services
are enabled, or any other personal information. Individual systems are tracked
persistently by a random (client-generated) UUID, to ensure that each system is
only counted once in each 24-hour sampling period.

The data collected by *PopCorn* is available to view at
<http://popcorn.voidlinux.org>

### Setting up PopCorn

First, install the `PopCorn` package. Then, enable the `popcorn` service, which
will attempt to report statistics once per day.
