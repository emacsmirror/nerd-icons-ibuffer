# nerd-icons-ibuffer

[![Build Status](https://github.com/seagle0128/nerd-icons-ibuffer/workflows/CI/badge.svg?branch=master)](https://github.com/seagle0128/nerd-icons-ibuffer/actions)
[![Release Tag](https://img.shields.io/github/tag/seagle0128/nerd-icons-ibuffer.svg?label=Release)](https://github.com/seagle0128/nerd-icons-buffer/releases)
[![License](http://img.shields.io/:License-GPL3-blue.svg)](License)
[![MELPA](https://melpa.org/packages/nerd-icons-ibuffer-badge.svg)](https://melpa.org/#/nerd-icons-ibuffer)
[![MELPA Stable](https://stable.melpa.org/packages/nerd-icons-ibuffer-badge.svg)](https://stable.melpa.org/#/nerd-icons-ibuffer)

<!-- markdown-toc start - Don't edit this section. Run M-x markdown-toc-refresh-toc -->

## Table of Contents

- [Install](#install)
  - [Manual](#manual)
  - [Use-package](#use-package)
- [Customize](#customize)
- [Screenshots](#screenshots)
- [Donate](#donate)

<!-- markdown-toc end -->

Display nerd icons in ibuffer.

This package is extracted from [Centaur
Emacs](https://github.com/seagle0128/.emacs.d) and leverages
[nerd-icons](https://github.com/rainstormstudio/nerd-icons.el).

## Install

### Manual

From melpa, `M-x package-install RET nerd-icons-ibuffer RET`.

```emacs-lisp
(add-hook 'ibuffer-mode-hook #'nerd-icons-ibuffer-mode)
```

### Use-package

```emacs-lisp
(use-package nerd-icons-ibuffer
  :ensure t
  :hook (ibuffer-mode . nerd-icons-ibuffer-mode))
```

To display icons correctly, you should run `M-x nerd-icons-install-fonts` to
install the necessary fonts.

Enjoy! :smile:

## Customize

```emacs-lisp
;; Whether display the icons.
(setq nerd-icons-ibuffer-icon t)

;; Whether display the colorful icons.
;; It respects `nerd-icons-color-icons'.
(setq nerd-icons-ibuffer-color-icon t)

;; The default icon size in ibuffer.
(setq nerd-icons-ibuffer-icon-size 1.0)

;; Use human readable file size in ibuffer.
(setq  nerd-icons-ibuffer-human-readable-size t)

;; A list of ways to display buffer lines with `nerd-icons'.
;; See `ibuffer-formats' for details.
nerd-icons-ibuffer-formats

;; Slow Rendering
;; If you experience a slow down in performance when rendering multiple icons simultaneously,
;; you can try setting the following variable
(setq inhibit-compacting-font-caches t)
```

## Screenshots

![nerd-icons-ibuffer](https://user-images.githubusercontent.com/140797/97093181-65867b00-167c-11eb-816c-0a96d69dcb94.png "icons with ibuffer")

## Donate

If you think the it's helpful for you, please consider paying a cup of coffee
for me. Thank you! :smile:

<img
src="https://user-images.githubusercontent.com/140797/65818854-44204900-e248-11e9-9cc5-3e6339587cd8.png"
alt="Alipay" width="120"/>
&nbsp;&nbsp;&nbsp;&nbsp;
<img
src="https://user-images.githubusercontent.com/140797/65818844-366ac380-e248-11e9-931c-4bd872d0566b.png"
alt="Wechat Pay" width="120"/>

<a href="https://paypal.me/seagle0128" target="_blank">
<img
src="https://www.paypalobjects.com/digitalassets/c/website/marketing/apac/C2/logos-buttons/optimize/44_Grey_PayPal_Pill_Button.png"
alt="PayPal" width="120" />
</a>
&nbsp;&nbsp;&nbsp;&nbsp;
<a href="https://www.buymeacoffee.com/s9giES1" target="_blank">
<img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee"
width="160"/>
</a>
