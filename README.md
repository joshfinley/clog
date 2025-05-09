# clog

`clog` is a developmental selective logging utility, primarily designed for penetration testing note taking.

Full console logging has two notable downsides for work like penetration testing:

1. Data overload: Some work (like penetration testing) involves large amounts of trial and error in the console. Having to dig through thousands of lines of console output to find snippets for notes is slow and error prone. Conversely, manually copying console output into notes mid-workflow can slow work down and be disruptive to the user's _"flow state"_. `clog` attempts to provide a middle ground by offering fast, repeatable recording of output of interest.
2. Logging of sensitive data is inevitable in many workflows - allowing for rule-based control of included log text allows (an albeit imperfect) way of automatically redacting sensitive information when performing note taking.

## setup

First, make sure `rustc` and `cargo` are installed.

If contributing, it's recommended to set up local `git` hooks:

```
cargo run -p xtask -- install-hooks
```
