# My Personal "Awesome" Go List

> 🎉 Just learning Go? Never coded before? Welcome to the party! Here's
> what I recommend most people do to learn it well. (Note that I do not
> list non-free resources, ever, but you can always support these
> financially if you choose):
>
> 0. Do the [Beginner Boost™][0] (every year)
> 1. [Tour of Go][1] (no setup, get coding, okay not to finish)
> 2. Start a personal [Bonzai™ command tree][2] to play around
> 3. [How to Write Go Code][3]
> 4. [Effective go][4] (to understand *why*)
> 5. Start reading [Go 101][5] concurrently (600 pages)
> 6. Code something with concurrency (`net/http`, contexts)
> 7. Read [Go Code Review Comments][7] for style guide
> 8. [The Go Programming Language Specification][5] to fill any gap
> 9. Read and learn from the [Go standard library][6] source code
>
> 💥 It is really important you get coding something you *want* to make,
> a project, as soon as possible. That will keep you motivated to learn.
> Obviously, you'll be writing a lot of your own code between reading
> books. But, by the time you read all of that, while coding at the same
> time, you'll be on your way to becoming a Go master for sure.
 
[0]: <https://github.com/rwxrob/boost>
[1]: <http://go.dev/tour>
[2]: <https://github.com/rwxrob/foo>
[3]: <https://golang.org/doc/code.html>
[4]: <https://golang.org/doc/effective_go.html>
[5]: <https://golang.org/ref/spec>
[6]: <https://pkg.go.dev/std>
[7]: <https://github.com/golang/go/wiki/CodeReviewComments>

And ...

> "Oh really, Jessie, does it inspire awe?" (Jane, Breaking Bad)

I'm not a fan of most "awesome" lists. Most of them are full of crap and
many are more about promoting that crap than anything else. My list has
two purposes:

1. Promote my own crap and keep track of it
2. Easily find awe-inspiring Go 1.18+ code and content
3. Help people get started with Go programming

Disclosure: I actually sponsor some of these with my own cash. They are
really that good.

## No-Cost, Non-Restrictive

Everything here is either Apache, BSD, or MIT licensed. I don't do GPLv3
and personally share Linus Torvalds opinion that it destroyed the FSF.

I also won't list anything here that has a paywall of any kind,
including books you have to purchase without a free version. Not
everyone in the world can find the money to pay American prices for
things. Holding knowledge behind a paywall that is based on the economy
of your particularly affluent country is unethical. I won't do it.
People can pay what they can for content I produce. That decision is up
to them, not the randomness of the conditions in which a person is born.

## My Own Stuff

* 🌳 **Go Bonzai™ Composite Commander**  
  https://github.com/rwxrob/bonzai

  A truly unique commander with recursive tab completion (without
  exporting shell code), command aliases, multicall or monolith mode,
  rich embedded command documentation (markdown, formatted, pager-aware,
  color, interactive terminal detection), library of completers (files,
  dates, calculator), localized, modular configuration management, fast
  local YAML caching

* 🌳 **Personal Bonzai Command Tree Monolith**  
  https://github.com/rwxrob/z

  My meticulously manicured monolith (`z`) command (which I use
  *constantly*) and easily copy to *any* system so I have all my
  favorite "scripts"; replacement for my
  [dot](https://github.com/rwxrob/dot) scripts collection; goal is to be
  100% script free by 2023 (that rhymed); will integrate with
  workspace-container to get my environment up anywhere in seconds, with
  or without Docker (even in a K8S pod); possible companion to a Go
  Bonzai root-kit monolith

* 🌳 **Help Docs with Templates, Like `man` Pages**  
  https://github.com/rwxrob/help

  Bundle your documentation with your Bonzai branch or tree with
  `help.Cmd`; supports BonzaiMark, CommonMark templates
  (`text/template`) with full set of common template functions; like
  Hugo for terminal apps

* 🌳 **Persist Variables to Portable Local Cache**  
  https://github.com/rwxrob/vars

  Better than environment variables; add scoped, persistent variables to
  any of your Bonzai branch or tree; .key=value properties value form
  for fastest-possible parsing (way faster than YAML/JSON; single file;
  standard user cache location; includes high-level `pkg` for use
  without `bonzai`

* 🌳 **Local Configuration Management with YAML/JSON**  
  https://github.com/rwxrob/conf

  Built on the highly popular and performant yaml.v3 and
  [yqlib](https://github.com/rwxrob/yq); add persistent, manageable
  configuration to any Bonzai branch or tree; single file; edit with
  preferred local editor; includes high-level `pkg` for use without
  `bonzai`

* **Buffered Rune Scanner**  
  https://github.com/rwxrob/scan

  A simple, highly performant buffered rune scanner; optimized for
  infinite lookahead/behind; designed with grammar creation in mind;
  optional trace logs to help debug complex scans

* **Functional Programming with Go Generics**  
  https://github.com/rwxrob/fn

  My own collection of map/filter/reduce/each-like things; great for
  rapid (replacing shell scripts) development; includes a terse `fn.A`
  functional array type, library of map functions (`mapf`), map
  transformations (`maps`), and UNIX filters (`filt`); (also see
  https://github.com/samber/lo

* **File and Directory Utilities**  
  https://github.com/rwxrob/fs

  Supplements the standard filesystem functions with simplifications and
  extras that make rapid application development slightly less annoying
  in Go; be sure to use `lockedfile` from
  https://github.com/rogpeppe/go-internal) for
  system-wide file locking

* **JSON Done Right with Remote Source Marshaling**  
  https://github.com/rwxrob/json

  Fixes the very broken defaults in `encoding/json`; includes `AsJSON`
  interface; unmarshaling JSON directly from web via HTTP requests into
  any type that can be passed to `json.Unmarshal` by leveraging yaml.v3
  `inline` (learned from the Kind project)

* **Marshal Anything as YAML**  
  https://github.com/rwxrob/yaml

  A personal commitment to first marshal everything in YAML since
  yaml.v3 is so superior to anything available for JSON --- especially
  `yaml:",inline"`. I prefer to YAML all the config things and Protobuf
  all the performant data serialization things. JSON is unavoidable when
  consuming web APIs, however.

* **VT100 ANSI Terminal Utilities**  
  https://github.com/rwxrob/term

  VT100 ANSI terminal escapes; no wasteful function calls just to change
  colors or terminal state; interactive terminal detection; window size
  queries; read visible and hidden user input

* **Converter Utility Functions**  
  https://github.com/rwxrob/to

  Transformations I find myself doing so much that they warrant their
  own `to` package module; string -> lines, etc.

* **Hybrid Data Structures with Generics**  
  https://github.com/rwxrob/structs

  I use this everywhere. Having proper data structures is main reason I
  maintain a [Bonzai command tree](https://github.com/rwxrob/z) instead
  of a bunch of shell scripts. `qstack` is usually better than Go slices
  for most applications; `tree` is perfect for making ASTs and domain
  specific language parsing combined with
  https://github.com/rwxrob/scan)

* 🌳 **Universal Unique Identifiers**  
  https://github.com/rwxrob/uniq

  The usual universal unique identifiers: `uuid`, `isosec`, `epoch`,
  `base32`, `hex`; includes high-level `pkg` library; essential for
  cobbling together flat-file data stores, etc.

* 🌳 **YAML to JSON Converter**  
  https://github.com/rwxrob/y2j

  YAML to JSON conversion without the unnecessary `encoding/json`
  escapes (see rwxrob/json above); includes `pkg` with high-level
  `Convert` function

* 🌳 **Popular YAML Query Utility**  
  https://github.com/rwxrob/yq

  This is a duplicate of the `yq` tool (with the same `yqlib`
  dependency); includes `pkg` with high-level `Evaluate` and
  `EvaluateToString` functions with reasonable defaults; can be called
  from other Bonzai commands; dropped Cobra dependency

## Other Awesome Stuff

* **Tcell, Best Go Terminal Low-Level Library**  
  https://github.com/gdamore/tcell

  Pure-Go terminal "cell" (curses) library for text terminals; best in
  class at the moment

* **Tview, Best Go Terminal User Interface Library**  
  https://github.com/rivo/tview  
  https://code.rocketnine.space/tslocum/cview  

  It's like having CSS in your terminal (but not); makes short work of
  terminal applications that need regularly used widgets, used by K9S
  and others; `cview`, a forked version, is also good

* **Lodash in Go**  
  https://github.com/samber/lo

  If you are into `lodash` (from Node, I never was) you can try this;
  good for getting Go 1.18 ideas; seven times faster than equivalents
  using Go reflection

* **Grab, Highly Concurrent Downloads with Status**  
  https://github.com/cavaliercoder/grab

  When you need really good download ability

* **Only Truly Safe Way to Write a File in Go**  
  https://github.com/rogpeppe/go-internal

  The internal libraries used by the `go` binary itself; home of
  `lockedfile` (proposed standard addition); *truly* safe writes to a
  file on all operating systems; (You're probably doing it wrong.
  Creating a "lock" file is never enough.)

* **Protobuf Performant Serialization**  
  https://github.com/protocolbuffers/protobuf

  Best of breed way to turn a struct into a data stream or file and
  parse it (unmarshal) it back into a struct later; basis of gRPC and
  most Kubernetes communication; replaces JSON APIs for most things

## Learning Resources

There are a lot of bad Go learning resources out there. Most of them are
woefully out of date. Just be really careful. Nothing goes on this this
that isn't 100% relevant to modern Go 1.18+ and available for free
(although I encourage you to support them the best you can).

* **Go-Nuts USENET Newsgroup.**  
  https://groups.google.com/g/golang-nuts

  This is where the creators and Go project leaders are regularly
  answering questions and discussing the direction of the language. This
  resource is far better than Reddit and even the official Go Discord
  channel (which you can find from https://go.dev). Keep in mind that
  anything ever written here is permanently saved, forever. I prefer
  this because all submissions are moderated and people actually take a
  moment to consider what they write before posting toxic crap (unlike
  Reddit and Discord, etc.)

* **Beej's Guide to Network Programming**  
  https://beej.us/guide/bgnet

  The book is in C, but so much of Go programming overlaps with that
  domain --- especially with microservices --- that reading this book
  should be mandatory for Go developers (or any developer). It covers
  things like proper UNIX file system semaphores and other architectural
  design concerns that most people coming to coding from academia or
  otherwise just won't think about intuitively.

* **Why Go and Not Rust**  
  https://kristoff.it/blog/why-go-and-not-rust

  This is a very stoic and objective look (not my personal writing
  style) at why Go is *the* language of enterprise and cloud-native
  computing and why it will *never* lose that position to anything else
  --- especially Rust. I'll confess to a, "well duh" thought a time or
  two while reading it, but a lot of beginners and veterans alike might
  need to read the very practical reason why Go is the best tool for
  *most* things and Rust is perhaps the best tool for a few isolated
  things, which is why the most significant software applications of the
  cloud and container era were all written in Go, not Rust and, by
  extension, why there are tons of jobs for Go and almost zero for Rust
  developers.

* **Protocol Buffers**  
  https://developers.google.com/protocol-buffers

  Protobuf format is mandatory learning for any serious Go developer
  wanting to get into microservices or anything that communicates or
  caches with performance requirements.
