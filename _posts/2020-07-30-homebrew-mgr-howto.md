### Quickstart for installing homebrew on your macintosh in 2 minutes
(This is just a quick "cheat-sheet" to get you started... I'll try to find better guides for using brew or add them to a wiki!)
Do steps below as shown in the first minute of [this 2-minute video](https://www.youtube.com/watch?v=NhOkYXB2_QQ)
  * Do a google search for "homebrew mac" and top hit should take you to [homebrew at https://brew.sh/](https://brew.sh/)
  * Finder: Go: Utilities: Terminal
  * Copy and paste the long line from above website into Terminal (and hit return/enter key). At some point it asks you to type in the password for your mac in the Terminal... no dots appear as you type it: just blindly type it and hit enter key. The brew commands can output a lot of info that scrolls by and that is normal.

```command
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
```
### Example: Use `brew` to `search` for `pymol`, then install it (another 2 minutes).
Now that you have brew, you can use it to install 1000's of formula and casks (Applications), using just `brew search` and `brew install`.
For example, if you do `brew search pymol` and `brew install brewsci/bio/pymol` results should be similar to below.  Note: All `brew` formulas, like for pymol install in /usr/local and so brew should *not* break or touch any existing Pymol you have. It is very well behaved that way!  Plus the pymol that brew installs is 100% free and open-source, and so never requires any activation nor any license. 
```command
$     brew search pymol
==> Formulae
brewsci/bio/pymol ✔

$  brew  install  brewsci/bio/pymol
...
==> Installing brewsci/bio/pymol
==> Pouring pymol-2.3.0.mojave.bottle.tar.gz
🍺  /usr/local/Cellar/pymol/2.3.0: 1,439 files, 35.2MB
==> Upgrading 6 dependents: 
...  ### Here you will see progress as brew installs all the dependencies for you
### To run it, type pymol and hit enter key
$   pymol

```
Any time you want to check for a newer version of pymol do: `brew update pymol`
If you have the newest version already you'll see a harmless "warning"
``` command
$   brew update pymol
Warning: brewsci/bio/pymol 2.3.0 already installed
```
Optionally, do next 2 lines to put pymol.command on desktop that you click to run
```
$    which pymol > ~/Desktop/pymol.command
$    chmod a+x ~/Desktop/pymol.command
```
![screenshot of pymol running](https://raw.githubusercontent.com/porteusconf/porteusconf.github.io/master/images/pymol-open-source-version.png)
