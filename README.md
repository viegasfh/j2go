# J2Go - A Java to Go Translator

`Java` was once my main programming language for writing all sorts of software. From applications software to systems software. But, from 2019, I switched permanently to `Go`, a language that compiles natively as opposed to a virtual machine, and doesn't have some of the shortcomings we find in the `JVM` (Java Virtual Machine).

With the switch to `Go`, I decided to convert some of the programs I work with on a regular basis to `Go`. However, rewriting the apps by hand is a great endeavour, and it would take months if not years to accomplish. As such, I decided to go the transpiler route, which, I am aware does not translate to a working `Go` program, it does speed up considerably. Meaning, that I would focus on making the code work by adding the missing elements, and then refactor it so that I could have a proper code in the `Go` way.

The idea sounded great and I tried to find a good transpiler on the Internet, but the one I found couldn't meet my needs. It was stuck at `Java 1.1`, and it failed at new `Java` syntax. So, I decided to craft my own. Initially, I was going to use [Sablecc](https://www.sablecc.org), but given that I found that [ANTLR](https://www.antlr.org) had working `Java` grammar that supports modern versions, I opted for that instead.

This project is the result of that decision. The aim is not to write a transpiler that converts from `Java` to working `Go` code, but to speed up the translation process. It will eventually evolve into an app that allows the user to control some of the code generation process. For instance, one could create a mapping of `Java` import libraries to `Go` import libraries, as well as classes to structs, and identifiers, which would shorten the fixing process. But, for the time being, my aim is to create something that will allow me to have `Go` code that I can fix and make it work.

If you find this tool useful, and if you have any suggestions or bug reports, please do it [here](https://github.com/viegasfh/j2go/issues), and I'll look at them whenever I can.
