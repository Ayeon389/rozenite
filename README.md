# Broadly speaking what is Rozenite?
Rozenite is an embeddable lightweight efficient, statically typed, procedural programming language.

# Okay so, what's inside this repository?
This repository contains a bootstrap compiler written in javascript.

As this is the bootstrap compiler implementation, there is zero intention to keep maintained once it is capable of being used to compile a minimal functioning implementation of a compiler written in Rozenite itself.

# Important details relating to this implentation.
* This implementation doesn't provide proper support for import
* Import can only import a list of hardcoded libraries provided by the compiler
* The bootstrap compiler doesn't produce Rozenite bytecode for [the runtime](https://github.com/Ayeon389/rozenite-runtime), it directly executes it's own AST using it's own inline as-needed implementation of runtime stdlib. The pro for doing this, is that the bytecode emitting code only needs to be written once. The innate con, this is probably very slow. If it is too slow, i'd rather attempt transpiling to javascript before writing code to emit bytecode.

# List of Rozenite repositories.
* [The Runtime](https://github.com/Ayeon389/rozenite-runtime)
* [The Bootstrap Compiler](https://github.com/Ayeon389/rozenite-compiler)
* [The Specification's For Rozenite](https://github.com/Ayeon389/rozenite-spec)
