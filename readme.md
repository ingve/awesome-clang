# Awesome Clang [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

> Useful resources and samples for using [Clang](http://clang.llvm.org/)-related tools, or for [building stuff on top of Clang](http://clang.llvm.org/docs/Tooling.html).

*Inspired by the [awesome](https://github.com/sindresorhus/awesome) list thing.

## Tools

### clang-format

- [clang-format docs](https://clang.llvm.org/docs/ClangFormat.html) - A tool to format C/C++/Java/JavaScript/Objective-C/Protobuf code.
- [style options](https://clang.llvm.org/docs/ClangFormatStyleOptions.html) - clang-format style options.
- [configurator](https://zed0.co.uk/clang-format-configurator/) -  clang-format configurator.

### clang-tidy

- [clang-tidy](https://clang.llvm.org/extra/clang-tidy/) - clang-based C++ linter tool.
- [List of clang-tidy checks](https://clang.llvm.org/extra/clang-tidy/checks/list.html)
- [Writing a basic clang static analysis check](https://bbannier.github.io/blog/2015/05/02/Writing-a-basic-clang-static-analysis-check.html)

## pp-trace

- [pp-trace](https://clang.llvm.org/extra/pp-trace.html) - tool that traces preprocessor activity.

### Clang static analyzer

- [Clang Static Analyzer](https://clang-analyzer.llvm.org/index.html) - a source code analysis tool that finds bugs in C, C++, and Objective-C programs.
- [scan-build](https://clang-analyzer.llvm.org/scan-build.html) -Running the analyzer from the command line.
- [Static Analysis with clang](https://btorpey.github.io/blog/2015/04/27/static-analysis-with-clang/)
- [CodeChecker](https://github.com/Ericsson/codechecker) - defect database and viewer extension for Clang Static Analyzer.
- [clang-analyzer-guide](https://github.com/haoNoQ/clang-analyzer-guide) An easy guide to Clang Static Analyzer extension.

### AddressSanitizer

- [AddressSanitizer](https://clang.llvm.org/docs/AddressSanitizer.html) - a fast memory error detector.
- [Address Sanitizer](https://www.mikeash.com/pyblog/friday-qa-2015-07-03-address-sanitizer.html) - overview by Mike Ash.

### Other Clang-based tools

- [C++ Insights](https://github.com/andreasfertig/cppinsights) - a clang-based tool which does source to source transformation. Its goal is it to make things visible which normally, and intentionally, happen behind the scenes. [Live/online demo](https://cppinsights.io/) available.
- [Clang Power Tools](https://github.com/Caphyon/clang-power-tools) - Visual Studio extension with Clang/LLVM tools (`clang++`, `clang-tidy` and `clang-format`).

## Libraries

### LibClang

- [libclang:](https://clang.llvm.org/doxygen/group__CINDEX.html) -  C Interface to Clang.
- [Introduction to libclang](https://www.mikeash.com/pyblog/friday-qa-2014-01-24-introduction-to-libclang.html)
- [LLVM & Clang library usage samples](https://github.com/eliben/llvm-clang-samples)
- [lloccount](https://github.com/neolynx/lloccount) - C/C++ Logical Lines Of Code Counter.
- [libclangmm](https://github.com/cppit/libclangmm) - C++-wrapper for libclang (developed for [juCi++](https://github.com/cppit/jucipp))
- [Customizable Naming Convention Checker](https://github.com/mapbox/cncc/) - similar to clang-format, but for naming conventions only.
- [irony-mode](https://github.com/Sarcasm/irony-mode) - A C/C++ minor mode for Emacs powered by libclang.
- [c99-to-c89](https://github.com/libav/c99-to-c89/) - Tool to convert C99 code to MSVC-compatible C89.
- [ClangKit](https://github.com/macmade/ClangKit) - Objective-C frontend to LibClang.
- [Skipping library code in gdb with help from libClang](https://jefftrull.github.io/c++/gdb/python/libclang/llvm/2018/04/30/stepping-with-libclang.html) - using libClang’s Python bindings.

### LibTooling

- [LibTooling](https://clang.llvm.org/docs/LibTooling.html) - library to support writing standalone tools based on Clang
- [Tutorial for building tools using LibTooling and LibASTMatchers](https://clang.llvm.org/docs/LibASTMatchersTutorial.html)
- [Modern source-to-source transformation with Clang and libTooling](https://eli.thegreenplace.net/2014/05/01/modern-source-to-source-transformation-with-clang-and-libtooling)
- [AST matchers and Clang refactoring tools](https://eli.thegreenplace.net/2014/07/29/ast-matchers-and-clang-refactoring-tools)
- [Compilation databases for Clang-based tools](https://eli.thegreenplace.net/2014/05/21/compilation-databases-for-clang-based-tools)
- [LibTooling Example](https://kevinaboos.wordpress.com/2013/07/23/clang-tutorial-part-ii-libtooling-example/)
- [Lecture slides and code examples for the Clang libraries](https://github.com/mdadams/clang_libraries_companion)

### Important Clang concepts

- [Quick overview of how Clang works internally](http://cppdepend.com/blog/?p=321)
- [Getting Started with LLVM Core Libraries](https://www.packtpub.com/application-development/getting-started-llvm-core-libraries) - PacktPub books can be a bit hit and miss, but this one is excellent. (A [PDF with updates for Clang 3.5](https://www.packtpub.com/sites/default/files/downloads/6924OS_Appendix.pdf) is available for free download).
- [Introduction to the Clang AST](https://clang.llvm.org/docs/IntroductionToTheClangAST.html) - a gentle introduction to the mysteries of the Clang AST.
- [Matching the Clang AST](https://clang.llvm.org/docs/LibASTMatchers.html) - how to use Clang’s LibASTMatchers to match interesting nodes of the AST and execute code that uses the matched nodes.
- [AST Matcher Reference](https://clang.llvm.org/docs/LibASTMatchersReference.html) - AST matchers implemented by Clang.
- [How to build LLVM from source](https://quuxplusone.github.io/blog/2018/04/16/building-llvm-from-source/) - Step-by step, using the GitHub mirror.
- [Writing LLVM Pass in 2018 — Part I](https://medium.com/@mshockwave/writing-llvm-pass-in-2018-part-i-531c700e85eb) - New Pass & Pass Manager in a Peek.
- [The future of Clang-based tooling](https://blog.trailofbits.com/2023/07/28/the-future-of-clang-based-tooling/)

## Videos

- [Create your own Refactoring Tool in Clang](https://www.youtube.com/watch?v=8PndHo7jjHk) - Richard Thompson's presentation from C++Now 2014.
- [Refactoring C++ with Clang](https://www.youtube.com/watch?v=yuIOGfcOH0k) - Chandler Carruth's talk from C++Now 2012.
- [Automatic C++ source code generation with clang](https://www.youtube.com/watch?v=aPTyatTI42k) - Sergei Sadovnikov's ACCU 2017 talk.

## Tips

Contributions welcome :)

## License

<a rel="license" href="https://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="https://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.
