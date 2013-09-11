# Bootstrap

## Check out this repo
Clone this repository into your `~/.emacs.d/` directory.  For example

`cd ~/.emacs.d ; git clone git@github.com:okl/danger-emacs.git`

This will clone this content into the `danger-emacs` directory.

## Initialize the submodules
After you check out this repo, from the root level directory run 
1. `git submodule init`
2. `git submodule update`

## Update your `~/.emacs load-path`
Now add that directory to your loadpath. In your ~/.emacs file add

```
(setq load-path (cons (expand-file-name "~/.emacs.d/danger-core") load-path))
(require 'danger-core)
```

Restart emacs.
When emacs starts up again, it will have errors like:

```
(file-error "Cannot open load file" "clojure-mode")
  require(clojure-mode)
```

That's ok, keep going.

## Initialize the emacs package manager


* `M-x package-refresh-contents
`

### Download packages

If you add new packages to the repo, make sure to update the lists below.

#### Clojure

* `M-x package-install [RET] clojure-mode [RET]`
* `M-x package-install [RET] nrepl [RET]`