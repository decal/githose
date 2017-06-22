**githose v0.8.94a**
================

_`githose` concurrently archives GitHub users' code repositories and gist text!_

This is similar to `github_cloner` by `anantshri` on GitHub which is written in
Python.  However, that project does not support gists or implement any form of 
concurrent programming.  `githose` utilizes GNU `parallel` for a significant 
speedup in multi-tasking, especially when a user's account hosts many hundreds 
of repositories (and some which are rather large.) 

### Features

The table below is a feature comparison between `githose` and `github_cloner`:

***

| Software Tool | Colors | Threads | Gists | One-to-many | GUI |
|:-------------:|:------:|:-------:|:-----:|:-----------:|:---:|
| web interface |  yes   |   no    |  yes  |     no      | yes |
| git(1) CLI    |  yes   |   no    |   no  |     no      |  no |
| github_cloner |   no   |   no    |   no  |    yes      |  no |
| githose       |  yes   |  yes    |  yes  |    yes      |  no |
|---------------|--------|---------|-------|-------------|-----|

***

### Documentation

* Refer to the `doc` directory which has the files/directories outlined below:

  1. `AUTHORS.md`
  2. `NEWS.md`
  3. `FAQ.md`
  4. `INSTALL.md`
  5. `LICENSE.md`
  6. `GUIDE.md`
  7. `TODO.md`
  8. `use-cases` 
    1. gisthose-clone-decal.scr
    2. githose-clone-decal.scr
    3. gristhose-clone-klacke.scr

### Feature List

* Multi-Threaded Anonymous Access to [GitHub API v3](https://developer.github.com/v3/) 
  - Git commands parallelized via GNU `parallel` if found in `PATH` by `which`
  - Application-level anonymity due to lack of uniquely identifying API key
  - Responsibility for transport layer anonymity falls squarely on the user 
  - Low-level network function wrapper like `torify` needed to conceal source IP

* Clone/pull all of a user's repositories and gists in one fell swoop
  - `githose` handles code repositories
  - `gisthose` handles gist entries
  - `gristhose` handles both code repositories and gist entries

* Support for [ANSI escape code colors](https://en.wikipedia.org/wiki/ANSI_escape_code#Colors)

### DevOps Info

Coded by*:*    _Derek Callaway_ [<decal {AT} sdf {D0T} org>](mailto:decal@sdf.org)
               `@decalresponds` on [Twitter](https://github.com/decalresponds)

Tested on*:*   `Linux Version 4.8.0-kali2-amd64, Compiled #1 SMP Debian 4.8.15-1kali1 (2016-12-23)`
               `Eight 3.37GHz Intel i7 Processors, 128TB RAM, 39913 Bogomips Total`

Released at*:* `Thu Feb 16 02:01:31 EST 2017`

