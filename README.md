# Bootstrap

## Check out this repo
Clone this repository into your `~/.emacs.d/` directory.  For example

`cd ~/.emacs.d ; git clone ... okl`

This will clone this content into the `okl` directory.

## Update your `~/.emacs load-path`
Now add that directory to your loadpath. In your ~/.emacs file add

`(setq load-path (cons (expand-file-name "~/.emacs.d/okl") load-path))`

## Initialize the submodules
After you check out this repo, from the root level directory run `git submodule init` and `git submodule update`

## Initialize the emacs package manager

* `M-x package-refresh-contents`

### Download packages

If you add new packages to the repo, make sure to update the lists below.

#### Clojure

* `M-x package-install [RET] clojure-mode [RET]`
* `M-x package-install [RET] nrepl [RET]`