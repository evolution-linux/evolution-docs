# Logging

## Syslog

The default installation comes with no syslog daemon. However, there are syslog
implementations available in the EvolutionOS repositories.

### Socklog

[socklog(8)](https://man.voidlinux.org/socklog.8) is a syslog implementation
from the author of [runit(8)](https://man.voidlinux.org/runit.8). Use socklog if
you're not sure which syslog implementation to use. To enable it, install the
`socklog-void` package and enable the `socklog-unix` and `nanoklogd` services.
Ensure no other syslog daemon is running.

The logs are saved in sub-directories of `/var/log/socklog/`, and `svlogtail`
can be used to access them conveniently.

The ability to read logs is limited to `root` and users who are part of the
`socklog` group.

### Other syslog daemons

The EvolutionOS repositories also include packages for `rsyslog` and `metalog`.
