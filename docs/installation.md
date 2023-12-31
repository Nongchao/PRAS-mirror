# Installation

PRAS is written in the [Julia](https://julialang.org/) numerical programming
language. If you haven't already, your first step should be to install Julia.
Instructions are available at
[julialang.org/downloads](https://julialang.org/downloads/).

Once you have Julia installed, PRAS can be installed in two easy steps!

First, add NREL's Julia package registry to your Julia installation.
From the main Julia prompt, type `]` to enter the package management REPL.
The prompt should change from `julia>` to something like `(v1.3) pkg>`
(your version number may be slightly different).
Type (or paste) the following (minus the `pkg>` prompt) - note that the first
line is only necessary if your Julia installation is brand new and you've
never installed a package before:

```
pkg> registry add https://github.com/JuliaRegistries/General.git
pkg> registry add https://github.com/NREL/JuliaRegistry.git
```

Adding the NREL registry will allow you to easily add NREL-developed
packages (like PRAS) that aren't yet available in the main Julia registry.

Now you can install the PRAS package. In the package REPL (`(v1.1) pkg>`),
simply type or paste:

```
pkg> add PRAS
```

This will automatically install the PRAS Julia module and all of its
related dependencies. At this point you can hit Backspace to switch back to the
main `julia>` prompt.

# Usage

With PRAS installed, you can load it into Julia as follows:

`using PRAS`

This will make the core PRAS functions (most importantly, the `SystemModel`
and `assess` functions) available for use in your Julia script or
interactive REPL session.

The [Getting Started](./getting-started) page provides more information
on using PRAS.
