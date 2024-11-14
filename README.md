# My Hyperleaf Configuration

This repository is my configuration of the toolkit, to create a working overleaf instance with persistent latex packages and fixes.

At the moment, to get this running you have to do the following steps:

1. Start instance with "bin/init" and "bin/up"
2. Use "docker cp /usr/local/texlive <absolute_path>/data/texlive" to get the current texlive status
3. Log into the container using bin/shell
4. Run tlmgr install scheme-full
5. Now you should be ready to use overleaf like below


# Original README

# Overleaf Toolkit

This repository contains the Overleaf Toolkit, the standard tools for running a local
instance of [Overleaf](https://overleaf.com). This toolkit will help you to set up and administer both Overleaf Community Edition (free to use, and community supported), and Overleaf Server Pro (commercial, with professional support).

The [Developer wiki](https://github.com/overleaf/overleaf/wiki) contains further documentation on releases, features and other configuration elements.


## Getting Started

Clone this repository locally:

``` sh
git clone https://github.com/overleaf/toolkit.git ./overleaf-toolkit
```

Then follow the [Quick Start Guide](./doc/quick-start-guide.md).


## Documentation

See [Documentation Index](./doc/README.md)


## Contributing

See the [CONTRIBUTING](https://github.com/overleaf/overleaf/blob/main/CONTRIBUTING.md) file.


## Getting Help

Users of the free Community Edition should [open an issue on github](https://github.com/overleaf/toolkit/issues). 

Users of Server Pro should contact `support@overleaf.com` for assistance.

In both cases, it is a good idea to include the output of the `bin/doctor` script in your message.

