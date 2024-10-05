# Two weeks of Rust, small steps, big understanding

## How I learn

For now I'm using 3 ressources
* Pluralsight: I'm watching the [Rust path](https://app.pluralsight.com/paths/skill/rust-2021) videos. I'm still in the begginner bracket of content, but it's ok
* [Rustonomicon](https://doc.rust-lang.org/nomicon/), the official documentation and learning material
* [https://roadmap.sh/](https://roadmap.sh/), useful to target knowledge when learning a new topic. Particularry I'm using [The project idea list](https://roadmap.sh/projects)

Initially I wanted to rewrite [Xpansion problem generation module](https://github.com/AntaresSimulatorTeam/antares-xpansion/tree/develop/src/cpp/lpnamer) because I'm working on it for my job so I understand what it does and would be interest to see if -or how much more- it is better in Rust performance wise. But for now I'm doing roadmap projects

## Goal change

As I said above I wanted to rewrite a part of Xpansion is Rust. Problem Generation is an ETL that takes linear problems in input, add constraints, write updated problems. The main difficulty is having access to a linear problem library in Rust. Unfortunatly I didn't find anything I could use for my case. The main issue is being able to read and write mps files.
I did found some LP Libraries but they don't offer read/write.
I did found bindings for Coin or OR-tools, but not up to date.
If I wanted to continue with this goal I would have to continue looking for the one library, write one, or re-write a crate with Coin bindingd (and probably Xpress bindings too).

## What I learned so far

* Rust is const (immutable) by default. That's awesome
* Rust is "move by default", comparing to pass by Value by default in C++.
* Rust is multi-paradigme but contrary to C++, Java etc. it is a functionnal language with OOP capabilities rather than the other way.

## What I did so far

I did successfully create binding with bindgen to[a simple C API](https://gitlab.com/JasonMarechal25/testapi) [here](https://gitlab.com/JasonMarechal25/rusttestapicbinding/-/tree/master?ref_type=heads)

I started the [tasklist project](https://github.com/JasonMarechal25/tasklist) from [roadmap](https://roadmap.sh/projects/task-tracker)
