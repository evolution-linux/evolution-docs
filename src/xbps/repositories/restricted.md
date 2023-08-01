# Restricted Packages

EvolutionOS offers some packages that are officially maintained, but not distributed.
These packages are marked as restricted and must be built from their
[evolution-packages](https://github.com/evolution-linux/evolution-packages) template locally.

Packages can be restricted from distribution by either the upstream author or
EvolutionOS. EvolutionOS reserves the right to restrict distribution of any package for
effectively any reason, massive size being the most common. Another common
reason is restrictive licensing that does not allow third-party redistribution
of source or binary packages.

## Building manually

You can use `xbps-src` in the
[evolution-packages](https://github.com/evolution-linux/evolution-packages) repository to build
the restricted packages from templates. For instructions on building packages
from templates, refer to the
[evolution-packages](https://github.com/evolution-linux/evolution-packages) documentation, and
the ["Quick start"
section](https://github.com/evolution-linux/evolution-packages#quick-start) in particular
.

Remember that the building of restricted packages must be enabled explicitly by
setting `XBPS_ALLOW_RESTRICTED=yes` in your `xbps-src` configuration (in the
`etc/conf` file in the repository.)

## Automated building

There is also a tool,
[xbps-mini-builder](https://github.com/the-maldridge/xbps-mini-builder) which
automates the process of building a list of packages. The script can be called
periodically and will only rebuild packages if their templates have changed.
