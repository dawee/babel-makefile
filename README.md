# Babel Makefile

Base Makefile for Babel-based projects

## Usage

* Add **babel.mk** in your project
* Create a **Makefile** with your settings (see the example)
* Include _babel.mk_ (as in the example)

## Example Makefile

**Makefile** content :

```make
babel := babel
browserify := browserify
presets := es2015
sourcesdir := lib test
builddir := es5
standalone := static/standalone.js
main := lib/main.js

include babel.mk
```

Build the standalone :

```sh
make
```

Clean build :

```sh
make clean
```

Re-build (clean + all) :

```sh
make re
```

Build one file only:

```sh
make es5/lib/main.js
```

