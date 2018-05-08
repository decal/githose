### Changes in githose 20180508
  * Gists with identical filenames are no longer clobbered by `wget -nc`
  * `$GITHOSE_NUM_JOBS` is being set in `inc/inits` to optimize speedup
  * `contrib/get-repo-desc` gets the description of a particular user/repo pair

### Changes in githose 20171206
  * Renamed `githose-usage` symbolic link to `githose-help`
  * Added ability to loop over multiple usernames passed on the command line 
  * Various modularization improvements to `githose clone` 
  * Moved `README.md` to doc and created a symbolic link to it in the root directory
  * Slightly modified the color scheme of the command usage output line
  * Made a `$GITHUB_API_TOKEN` assignment in `etc/githose.conf` for non-anonymous requests
  * Fixed a bug in creation of a non-existent `$GITAA_PATH_CLONE`
  * Created a new include source file for user-defined functions at `inc/funcs`

### Changes in githose 20170625
  * Wrote code for pulling per-user and all local users' repositories, ex.
    - `githose pull decal`
    - `githose pull --all` *or* `githose pull -a`
  * Refined URI style input feature to parse username, ex.
    - `githose clone https://github.com/user`
  * Implemented `githose-usage` (now `githose-help`) to show generic usage for all commands
  * Edited usages text to be more informative
  * Created `etc/githose.issue` and related symlinks for current version banner

### Changes in githose 20170216
  * Created `gristhose` command
    - combines functionality of `githose` and `gisthose`
  * Added ANSI color cosmetics to command-line help/usage and general output
  * Updated `README.md` and the other `markdown` files in the `doc` directory

### Changes in githose 20170113
  * Created `gisthose` command 
    - same idea as `githose` but for gist text instead of git repositories
  * Implemented global configuration file: `etc/githost.conf`

### Changes in githose 20161014
  * First public release 
  * Early implementation of primary sub-command pair: `clone` and `pull`
