Frequently Asked Questions
==========================

1. How is the name of this program ("`githose`") actually pronounced in spoken English?

  * `githose` was purposely named so that it can be pronounced in the following two ways:
    1. "git" "hose" 
    2. "git" "those"

  * both pronounciations are acceptable and very self-explanatory as well
  * whenever you want to 'get those' repositories from a user without manually typing `git clone` for each just use `githose`
  * metaphorically speaking, `githose` acts as a "hose" by spraying the repositories/gists with [GitHub API](https://api.github.com/)
  * `gisthose` is pronounced exactly as it reads: "jist" "hoes"
  * `gristhose` also has a straightforward pronunciation: "guh-wrist" "ho's"

2. What type of computing environment was `githose` initially developed in?

  * `githose` was developed in the [Kali](https://kali.org/) Linux distribution which is a fork of [Debian](https://debian.org/)
  * MSI GT72 2QE Dominator Pro laptop with an Intel Core i7 running at ~5K BogoMIPS
  * GNU bash, version 4.4.11(1)-release (x86_64-pc-linux-gnu)
  * GNU parallel 20161222
  * Currently maintained in WSL ([Windows Subsystem for Linux](https://msdn.microsoft.com/commandline/wsl/about "Bash on Ubuntu on Windows - About")) 

3. Which platforms should `githose` properly operate under?

  * Just about any Linux distribution with the Bourne Again Shell..

4. How do I report bugs?
  * Send an e-mail message to: **[decal (AT) sdf {D0T} org]** with Subject line:
    - `GITHOSE BUG REPORT` 
  * Alternatively (if you've written a patch), submit a pull request to the GitHub repository!

5. What if I want to troubleshoot a bug by myself?

  * The author primarily utilizes the following troubleshooting techniques with `githose`: 
    - Set the environment variable named `GITHOSE_DEBUG` to `1`, i.e. `GITHOSE_DEBUG=1 githose -h`
    - bashdb(1) - bash debugger script
    - Debugging echo statements
    - Execute sub-scripts sourced from the `lib` directory on an individual basis when narrowing down the issue

6. Can I contrib code to the `githose` project?

  * Absolutely! One of the following two additions may occur depending upon the extent of your contributions and 
    how well it functions with the existing code..
    1. I may commit your script to the contrib folder as a plug-in..
    2. If it defines a robust new feature, I might include your code as part of the master repository..

7. What if I can't install GNU `parallel`?

  * No problem--`githose`, `gisthose` and `gristhose` will all still run just fine.
  * Without access to GNU `parallel` the scripts execute sequentially which makes multiple downloads slower.

8. What if I can't install the GNU Bourne Again Shell, i.e. `bash`?

  * Sorry, but in this case you're just [SOL](http://www.urbandictionary.com/define.php?term=SOL "Urban Dictionary definition of SOL")!

9. How come I'm seeing escape characters instead of ANSI colors?!

  * This can be caused by one or more software/configuration issues..
    - Ensure that your `TERM` environment variable is set correctly
    - For example: `export TERM=xterm-256color`
    - Add setting to: `~/.bashrc` or `~/.bash_profile` or `/etc/bash.bashrc`

10. Why am I getting Perl-related errors from [GNU parallel](https://www.gnu.org/software/parallel/)

  * Check for bad permissions or uninstalled [CPAN](http://www.cpan.org) modules
  * Don't forget `parallel` isn't a required dependency, so try uninstalling it
