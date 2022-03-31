# My Personal "Awesome" Go List

> "Oh really, Jessie, does it inspire awe?" (Jane, Breaking Bad)

I'm not a fan of most "awesome" lists. Most of them are full of crap and
many are more about promoting that crap than anything else. My list has
two purposes:

1. Promote my own crap and keep track of it
2. Easily find awe-inspiring Go 1.18+ code and content
3. Help people get started with Go programming

Disclosure: I actually sponsor some of these with my own cash. They are
really that good.

## My Own Stuff

* 🌳 **Go Bonzai™ Composite Commander**
  ([rwxrob/bonzai](https://github.com/rwxrob/bonzai))

  A truly unique commander with recursive tab completion (without
  exporting shell code), command aliases, multicall or monolith mode,
  rich embedded command documentation (markdown, formatted, pager-aware,
  color, interactive terminal detection), library of completers (files,
  dates, calculator), localized, modular configuration management, fast
  local YAML caching

* 🌳 **Personal Bonzai Command Tree Monolith**
  ([rwxrob/z](https://github.com/rwxrob/z))

  My meticulously manicured `z` command (which I use *constantly*) and
  easily copy to *any* system so I have all my favorite "scripts";
  replacement for my [dot](https://github.com/rwxrob/dot) scripts
  collection; goal is to be 100% script free by 2023 (that rhymed); will
  integrate with workspace-container to get my environment up anywhere
  in seconds, with or without Docker (even in a K8S pod); possible
  companion to a Go Bonzai root-kit monolith

* 🌳 **Local Config Management with YAML**
  ([rwxrob/config](https://github.com/rwxrob/config))

  Bonzai branch for universal YAML configuration management; default
  `Configurer` for all `bonzai.Cmds`; includes `yq` expressions and
  pathing

* **Universal Rune Scanner with scan.X Expressions**
  ([rwxrob/scan](https://github.com/rwxrob/scan))

  A unique, performant rune scanner optimized for infinite look-ahead
  and behind including multiple cursor support and optional node-tree
  parser designed for rapid grammar and domain-specific language
  development with intuitive methods and traceable scan.X expression
  language interpreter in pure Go for easy code generation from meta
  languages such as PEGN

* **Functional Programming with Go Generics**
  ([rwxrob/fn](https://github.com/rwxrob/fn))

  My own collection of map/filter/reduce/each-like things; great for
  rapid (replacing shell scripts) development; includes a terse `fn.A`
  functional array type, library of map functions (`mapf`), map
  transformations (`maps`), and UNIX filters (`filt`); (also see
  [samber/lo](https://github.com/samber/lo))

* **File and Directory Utilities**
  ([rwxrob/fs](https://github.com/rwxrob/fs))

  Supplements the standard filesystem functions with simplifications and
  extras that make rapid application development slightly less annoying
  in Go; be sure to use `lockedfile` from
  [rogpeppe/go-internal](https://github.com/rogpeppe/go-internal) for
  system-wide file locking

* **JSON Done Right with Remote Source Marshaling**
  ([rwxrob/json](https://github.com/rwxrob/json))

  Fixes the very broken defaults in `encoding/json`; includes
  unmarshaling JSON directly from web via HTTP requests into any type
  that can be passed to `json.Unmarshal` by leveraging yaml.v3 `inline`
  (learned from the Kind project)

* **VT100 ANSI Terminal Utilities**
  ([rwxrob/term](https://github.com/rwxrob/term))

  VT100 ANSI terminal escapes; no wasteful function calls just to change
  colors or terminal state; interactive terminal detection; window size
  queries; read visible and hidden user input 

* **Converter Utility Functions**
  ([rwxrob/to](https://github.com/rwxrob/to))

  Transformations I find myself doing so much that they warrant their
  own `to` package module; string -> lines, etc.

* **Hybrid Data Structures with Generics**
  ([rwxrob/structs](https://github.com/rwxrob/structs))

  List, set, stack, node, tree, etc. implemented with rapid applications
  development (replacing shell scripts) as design priority; used in most
  other applications listed here --- especially `qstack` and `tree`.

* 🌳 **Universal Unique Identifiers**
  ([rwxrob/uniq](https://github.com/rwxrob/uniq))

  The usual universal unique identifiers: `uuid`, `isosec`, `epoch`,
  `base32`, `hex`; includes high-level `pkg` library; essential for
  cobbling together flat-file data stores, etc.

* 🌳 **YAML to JSON Converter**
  ([rwxrob/y2j](https://github.com/rwxrob/y2j))

  YAML to JSON conversion without the unnecessary `encoding/json`
  escapes (see rwxrob/json above); includes `pkg` with high-level
  `Convert` function

* 🌳 **Popular YAML Query Utility without Cobra**
  ([rwxrob/yq](https://github.com/rwxrob/yq))

  This is a duplicate of the `yq` tool (with the same `yqlib`
  dependency); includes `pkg` with high-level `Evaluate` and
  `EvaluateToString` functions with reasonable defaults; can be called
  from other Bonzai commands 

## Other Awesome Stuff

* [gdamore/tcell](https://github.com/gdamore/tcell) - cell-based view
  for text terminals, favorite library for creating terminal apps

* [rivo/tview](https://github.com/rivo/tview) - it's like having CSS in
  your terminal (but not), makes short work of terminal applications
  that need regularly used widgets

* [samber/lo](https://github.com/samber/lo) - lodash in Go 1.18 that's 7
  times faster than equivalents using reflection

* [cavaliercoder/grab](https://github.com/cavaliercoder/grab) - highly
  concurrent downloads with status updates in Go

* [rogpeppe/go-internal](https://github.com/rogpeppe/go-internal) - home
  of `lockedfile` (proposed standard addition), the only one anyone
  should use for *truly* safe writes to a file on all operating systems
  (hint: you're probably doing it wrong, creating a "lock" file is never
  enough)); this is currently how `go` binary handles system-wide file
  read/write locking

## Learning Resources

There are a lot of bad Go learning resources out there. Most of them are
woefully out of date. Just be really careful. Nothing goes on this this
that isn't 100% relevant to modern Go 1.18+.

* **Go-Nuts USENET Newsgroup.**
  <https://groups.google.com/g/golang-nuts>

  This is where the creators and Go project leaders are regularly
  answering questions and discussing the direction of the language. This
  resource is far better than Reddit and even the official Go Discord
  channel (which you can find from <https://go.dev>). Keep in mind that
  anything ever written here is permanently saved, forever. I prefer
  this because all submissions are moderated and people actually take a
  moment to consider what they write before posting toxic crap (unlike
  Reddit and Discord, etc.)

* **Get Programming with Go**
  <https://www.manning.com/books/get-programming-with-go>

  This book seems like the best for absolute beginners since it assumes
  you know nothing about programming at all and uses the Go playground
  and nothing more and doesn't get into the weeds about modules and
  project management and stuff (which is also its greatest weakness
  since you have to learn that stuff as well before doing anything
  significant with it). I intend to use this book (and the author has
  volunteered to help) during the [2022 Beginner
  Boost](https://github.com/rwxrob/boost) on May 4th.

* **Go Code Review Comments**
  <https://github.com/golang/go/wiki/CodeReviewComments>

* **Beej's Guide to Network Programming**
  <https://beej.us/guide/bgnet/>

  The book is in C, but so much of Go programming overlaps with that
  domain --- especially with microservices --- that reading this book
  should be mandatory for Go developers (or any developer). It covers
  things like proper UNIX file system semaphores and other architectural
  design concerns that most people coming to coding from academia or
  otherwise just won't think about intuitively.
