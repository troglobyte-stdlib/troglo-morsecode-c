# Troglobyte Morse Code

## overview

* * *

Morse code is a method used in telecommunication to encode text characters as
standardized sequences of two different signal durations, called dots and dashes,
or dits and dahs. Morse code is named after Samuel Morse, one of the inventors of
the telegraph.

This library will help with encoding and decoding the morse code.

## tooling

* * *

The targeted audience we are building for is *Windows 10*, *MacOSX*, *ChromeOS*
and *Linux* users. This project uses [Meson](https://mesonbuild.com/) `0.62.0`
and newer, uses `c18` standards for initial implementation of the package. The
objective by far is usability, security, transparency, and lightweight, packages
for any if not most of your application development needs.

## Setup, Compile and Install

* * *

Using this package should be fairly simple just add the git wrap file
in your subprojects directory and include the dependency in your project.

```console
[wrap-git]
directory = troglo-morsecode-c
url = https://github.com/troglobyte-stdlib/troglo-morsecode-c.git
revision = main

[provide]
module = trog_dep
```


The next step should be to add the package to your Meson project:

```meson
trog_dep = dependency('troglo-morsecode-c')

executable('prog', 'main.c',
    dependencies : [trog_dep])

```

And finally we setup, and compile the project just like normal.

## usage

* * *

Here is a simple sample application that should get you up and
running with using this library as soon as possible but to learn
more please view the API documentation thanks.

**Usage in C**:

```c
//
// Troglobyte stdlib:
// author: Michael Gene Brockus
// gmail: <michaelbrockus@gmail.com>
//
#include <stdio.h>
#include <troglobyte/morsecode.h>


//
// main is where all good examples start
//
int main()
{
    printf("%s\n", trog::greet());
    return 0;
} // end of func

```

## contact

If you want to contact me and have a few questions
regarding the solutions in the programming you can write
me a letter, my Gmail is <michaelbrockus@gmail.com>.

You may find that I have some social media platforms
in which you can follow me. [LinkedIn](https://www.linkedin.com/in/michael-brockus), [Facebook](https://facebook.com/michael.brockus.555), and [Instagram](https://instagram.com/troglobyte_coder/)
