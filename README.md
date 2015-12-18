# Rand-Theme

Random Emacs theme at start-up!


This package randomly selects a theme at start-up, if you like to use different
themes then this is for you! \o/

## Features
 - Randomly pick a theme from a list you want.
 You can setup a list that you only want to choose from or
 create a list of themes you *never* want to use.

- You can iterate forwards and backwards through the themes you have, in case you don't
want it to be random.

## How to install

## How to use

Before using you **must** first setup **either** `rand-theme-unwanted` or `rand-theme-wanted`. These  are lists in which the package will use
to decide what themes to select.

Example:
```lisp
(require 'rand-theme)
;; Themes I never want to be selected
(setq rand-theme-unwanted '(leuven tango adwaita light-blue tsdh-light dichromacy whiteboard))
(rand-theme)
```
```lisp
(require 'rand-theme)
;; Themes I *only* want to be selected
(setq rand-theme-wanted '(abyss lush manoj-dark))
(rand-theme)
```

## Keybindings

By default, there are no keybindings to this. 

You can set them up yourself. My personal preference was setting `C-z` to run `rand-theme-iterate`.
