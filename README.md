# Broadly speaking what is Rozenite?
Rozenite is an embeddable lightweight efficient, statically typed, procedural programming language.

# Okay so, what's inside this repository?
This repository contains a bootstrap compiler written in typescript.

As this is the bootstrap compiler implementation, there is zero intention to keep maintained once it is capable of being used to compile a minimal functioning implementation of a compiler written in Rozenite itself.

# Important details relating to this implentation.
* This implementation doesn't provide proper support for import
* Import can only import a list of hardcoded libraries provided by the compiler
* The bootstrap compiler doesn't produce Rozenite bytecode for [the runtime](https://github.com/Ayeon389/rozenite-runtime), it produces typescript.  
