# Livestatus Multitool Daemon - LMD

LMD fetches Livestatus data from one or multiple sources and provides:

* A combined Livestatus API for those sources.
* A cache which makes Livestatus queries a lot faster than requesting them directly from the remote sources.
* A enhanced Livestatus API with more useful output formats and sorting. See list below.
* Aggregated Livestatus results for multiple backends.
* A Prometheus exporter for Livestatus based metrics for Nagios, Icinga, Shinken and Naemon.

So basically this is a `Livestatus In / Livestatus Out` daemon. Its main purpose is to provide the backend handling of the Thruk Monitoring Gui in a native compiled fast daemon, but it should work for everything which requires Livestatus.

[LMD on Github](https://github.com/sni/lmd)

