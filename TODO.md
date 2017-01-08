**Things To Do**
============

* Program in proper support for gists!

* Write a `parallel` command for fetching the text of gists 

* Fix `inc/inits` to declare the `GITHOSE_CPU_CORES` environment variable properly..

* Command-line arguments..
  1. Pass global `getopt` flags to `bin/githose`
  2. Pass local `getopt` flags to `lib/githose/*` and `lib/gisthose/*`

* Implement `githose set` sub-command for modifying `githose.conf` file

* Introduce `githose set color` sub-sub-command (toggles color flag on/off)
 
* Implement `githose conf_(ig)?_` for managing config variables in `etc/githose.conf`

* Continue testing puller scripts

* Design new sub-command `githose list` to use the GitHub API in order to view a user's:
  - repositories
  - gists
  - logs, i.e. `git log`
  - followers 
  - following

* Make a Gist spider known as `spidigister`

* Create `lib/wgetter` so all `wget` invocations share function code


### Long-Term Goals..

* Make `githose` and `gisthose` work on sites outside of the `github.com` domain

* Write `lib/getopt` as a central command-line argument parsing function named `githose_getopt`

* Implement a _one-or-more_ `getopt` flag for verbosity: `-v` 
 - should also be used like: `-vv`

* Invent more custom URL scheme handlers such as `repos://user?repo1&repo2` 
