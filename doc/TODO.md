**Things To Do**
============

* Clone someone's stars

* Fix `githose clone yarn`

* Replace exit codes with `EX_` constants from `inc/sysexits`

* Why isn't `gristhose clone postmodern` getting {https://github.com/postmodern/robots} repo?

* Add support for [BitBucket](http://www.bitbucket.org "bitbucket.org")

* Translate github.com URL's into this format:
  - `https://raw.githubusercontent.com/jasonish/snort/master/doc/README.http_inspect`

* Gristhose flag that writes both repos and gists to same parent directory 
  - i.e. `user/{repos,gists}/` __or__...
  - `user/{repos/,gists.* }`

* Commands to easily view repos or gists (or both) of a given GitHub user

* Support independent GitLab, git-web, etc. sites

* Make asciinema's out of use-cases..

* Make it work on non-GitHub repositories
  - i.e. [](https://git.zx2c4.com "") __and__...
  - [](https://bitbucket.org "")

* Write `gristhose pull` 

* Don't maintain repos under `~/github` that are `chmod 0`

* Write the User's Guide in `GUIDE.md` 

* Mention other GitHub-based [OSINT](https://wikipedia.org/wiki/Open-source_intelligence "Open-source Intelligence") tools in user guide..

* Parse updated_at JSON member from GitHub API to check for modified gists
  - will be code for `lib/gisthose/pull`

* Support downloads based on searches using topic operator like:
  - [GitHub search for 'topic:security'](https://github.com/search?q=topic%3Asecurity&type=Repositories "GitHub search for 'topic:security'")

* Make `exit $BASH_LINENO` into `function codeError` or something..

* Fix usage condition by replacing with function in `lib/githose/pull`

* Test FreeBSD for FAQ question #3

* Write `man` page using `nroff`: `githose(1)`

* Write a `parallel` command for fetching the text of gists 

* _X_ Fix `inc/inits` to declare the `GITHOSE_CPU_CORES` environment variable properly.. 

* Command-line arguments..
  1. Pass global `getopt` flags to `bin/githose`
  2. Pass local `getopt` flags to `lib/githose/*` and `lib/gisthose/*`

* Implement `githose set` sub-command for modifying `githose.conf` file

* Introduce `githose set color` sub-sub-command (toggles color flag on/off)
 
* Implement `githose conf_(ig)?_` for managing config variables in `etc/githose.conf`

* Make `pull` work with gists?

* Design new sub-command `githose list` to use the GitHub API in order to view a user's:
  - repositories
  - gists
  - logs, i.e. `git log`
  - followers 
  - following

* Create `lib/wgetter` so all `wget` invocations share function code
  - Try using `lynx` or `curl` if `wget` isn't available..

* Performance-based profile tracing on all scripts to meet acceptable benchmarks


### Long-Term Goals..

* Make `githose` and `gisthose` work on sites outside of the `github.com` domain

* Write `lib/getopt` as a central command-line argument parsing function named `githose_getopt`

* Implement a _one-or-more_ `getopt` flag for verbosity: `-v` 
 - should also be used like: `-vv`

* Make a Gist spider known as `spidigister` that checks a given user's followers gists as well
