<!-- This file is mostly readable as plain text, but it will look better
  -- in a Markdown reader (try Frogmouth).
  -- 
  -- Alternately, go to https://hpjansson.org/chafa/ in a web browser. -->

<p align="center"><a href="https://hpjansson.org/chafa/"><img src="https://raw.githubusercontent.com/hpjansson/chafa/master/docs/chafa-logo.gif" /></a></p>


## About

Chafa is a command-line utility that converts image data, including
animated GIFs, into graphics formats or ANSI/Unicode character art suitable
for display in a terminal. 


## Installing
 If you want to
build the latest and greatest yourself, read on.

You will need GCC, make, Autoconf, Automake, Libtool and the GLib
development package installed to compile Chafa from its git repository. If
you want to build the command-line tool `chafa` and not just the library,
you will additionally need development packages for:

* FreeType2. Often packaged as `libfreetype6-dev` or `freetype2-devel`.
* libjpeg (optional). Look for `libjpeg-dev`, `libjpeg62-devel` or `libjpeg8-devel`.
* librsvg (optional). Look for `librsvg2-dev` or `librsvg-devel`.
* libtiff (optional). Look for `libtiff5-dev` or `libtiff-devel`.
* libwebp (optional). Look for `libwebp-dev` or `libwebp-devel`.

If you want to build documentation, you will also need gtk-doc.

Start by cloning the repository:

```sh
$ git clone https://github.com/hpjansson/chafa.git
```

Then cd to the toplevel directory and issue the following shell commands:

```sh
$ ./autogen.sh
$ make
$ sudo make install
```

That should do it!

## Python bindings

[Erica Ferrua Edwardsdóttir](https://mage.black/) maintains
[excellent Python bindings](https://chafapy.mage.black/) for Chafa. If
Python's your thing, check them out. They are easy to use and come with a
[detailed tutorial](https://chafapy.mage.black/usage/tutorial.html).

## JavaScript bindings

[Héctor Molinero Fernández](https://hector.molinero.dev/) maintains
[wonderful JavaScript bindings](https://github.com/hectorm/chafa-wasm)
built around his WebAssembly port. These are available from NPM and can
be used in Node.js, web browsers, and more.
