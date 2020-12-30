# 🐓 Chicken stream input

## About

* * *

`Chicken Stream Output` package is a lightweight package for handling
output streams. Gain the ability to manage this safely.

## Tooling information

* * *

Targeted audience we are building for is Windows 10, MacOSX and Linux users. This
project uses [Meson](https://mesonbuild.com/) `0.56.0` and newer.

## Setup, Compile and Install

* * *

Using this package should be fairly simple just add the git wrap file in your subprojects
directory and include the dependency in your project.

```console
[wrap-git]
directory = chicken-stream-in
url = https://github.com/chicken-libraries/chicken-stream-in.git
revision = main
```


The next step should be to add the package to your Meson project:

```meson
chicken_stream_in = subproject('chicken-stream-in')

executable('prog', files('main.c'),
    dependencies : [chicken_stream_in.get_variable('chicken_stream_in_dep')])

```

And finally we setup, and compile the project just like normal.

## Usage of this package

* * *

Here is a simple sample application that should get you up and running with using this
library as soon as possible but to learn more please view the API documentation thanks.

```c
#include <stdio.h>
#include <stdlib.h>
#include <chicken/package.h>

//
// main is where all good examples start
//
int main(void)
{
    puts(greet());
    return EXIT_SUCCESS;
} // end of function main

```

## Contact the developer

* * *

You can contact me with either of these methods.

-   linkedin: [michael-brockus](https://www.linkedin.com/in/michael-brockus-1009a1174/)
-   reddit: [MichaelBrockus](https://www.reddit.com/user/MichaelBrockus)
-   gmail: [michaelbrockus@gmail.com](mailto:michaelbrockus@gmail.com).
