Frequently Asked Questions
==========================

1. How is the name of this program ("`githose`") actually pronounced in spoken English?

  * `githose` was purposely named so that it can be pronounced in the following two ways:
    1. "git" "hose" 
    2. "git" "those"

  * both pronounciations are acceptable and very self-explanatory as well..
  * whenever you want to 'get those' repositories without having to manually type out `git clone` for each one just use `githose`..
  * metaphorically speaking, `githose` acts as a 'hose' by spraying the repositories or gists on a [GitHub](https://github.com/) user's account..
  * `gisthose` is pronounced exactly as it reads: "jist" "hoes"

2. What type of computing environment was `githose` developed in?

  * `githose` was developed in the [Kali](https://kali.org/) Linux distribution which is a fork of [Debian](https://debian.org/)
  * MSI GT72 2QE Dominator Pro laptop with an Intel Core i7 running at ~5K BogoMIPS
  * GNU bash, version 4.4.5(1)-release (x86_64-pc-linux-gnu)
  * GNU parallel 20161222

3. Which platforms should `githose` properly operate under?

  * Just about any Linux distribution with the Bourne Again Shell..

4. How do I report bugs?
  * Send an e-mail to: [decal (AT) sdf {D0T} org]

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

  * No problem--`githose` and `gisthose` will both still run just fine.
  * Without access to GNU `parallel` the scripts execute sequentially which makes multiple downloads slower.

8. What if I can't install the GNU Bourne Again Shell, i.e. `bash`?

  * Sorry, but in this case you're SOL!
