# My Personal "Awesome" Go List

🎉 Just learning Go? Never coded before? Welcome to the party! Here's what I recommend most people do to learn it well.

1.  [Tour of Go][1] (no setup, get coding, okay not to finish)
2.  [How to Write Go Code][3]
3.  [Effective go][4] (to understand why)
4.  Start a project of your own, doesn’t matter how big or small
5.  Start reading [Go 101][8] concurrently (600 pages) and [Go Modules][10] (not in book)
6.  Code something more advanced with concurrency (net/http, contexts)
7.  Read [Go Code Review Comments][7] for style guide
8.  Read [The Go Programming Language Specification][5] to fill any gaps
9.  Read and learn from the [Go standard library][6] source code
10. Read and learn from the [Bonzai core library] source code
11. Maybe read [Learning Go][9] (but you’ll have to buy it)
12. Read [100 Go Mistakes and How to Avoid Them][11]
13. Write a middleware API using any framework
14. Create a command line tool using Cobra
15. Create a command line tool using Bonzai

[1]: <http://go.dev/tour>
[2]: <https://github.com/rwxrob/bonzai>
[3]: <https://golang.org/doc/code.html>
[4]: <https://golang.org/doc/effective_go.html>
[5]: <https://golang.org/ref/spec>
[6]: <https://pkg.go.dev/std>
[Bonzai core library]: <https://github.com/golang/go/wiki/CodeReviewComments>
[8]: <https://go101.org/article/101.html>
[9]: <https://www.oreilly.com/library/view/learning-go/9781492077206/>
[10]: <https://go.dev/blog/using-go-modules>
[11]: <https://100go.co/>

💥 It is really important you get coding something you *want* to make, a project, as soon as possible. That will keep you motivated to learn. Obviously, you'll be writing a lot of your own code between reading books. But, by the time you read all of that, while coding at the same time, you'll be on your way to becoming a Go master for sure.

I'm not a fan of most "awesome" lists. Most of them are full of stuff that, um, really isn't awesome at all. A lot are there to promote stuff. My list has
three purposes:

1. Promote my own stuff and keep track of it
2. Easily find awe-inspiring modern code, idioms, and content
3. Help people get started with Go programming

Disclosure: I actually sponsor some of these with my own cash. They are
really that good.

Everything here is either Apache, BSD, or MIT licensed. I don't do GPLv3.

## My Own Stuff

* 🌳 **Go Bonzai™ composite commander and CLI toolbox**  
  <https://github.com/rwxrob/bonzai>

  A truly unique commander with recursive tab completion; no exported
  shell code required for completion; command aliases; multicall or
  monolith mode; rich embedded command documentation with markdown and
  templating; library of completers (files, dates, calculator); persisted variables to user local cache; library of "batteries included" commonly needed functions and data structures suitable for learning and porting your shell scripts to a Bonzai home kit monolith instead

* 🌳 **Personal Bonzai Command Tree Monolith**  
  <https://github.com/rwxrob/z>

  My personal replacement for a bunch of dot files and shell scipts. It's
  becoming almost like a BusyBox Linux distro as more branches are added to it.
  Everything I write now is a Bonzai branch with a standalone, a high-level
  function library, and a composable branch Cmd. I can easily copy my `z` to
  *any* system so I have all my favorite "scripts" --- including bundled
  configurations for `vi`/`vim`/`nvim`, `tmux`, `lynx` and such
  ([dot](https://github.com/rwxrob/dot)). By 2025, I hope to be 100% script
  free.

## Other Awesome Stuff

* **GitHub command line tool helper library**  
  <https://github.com/cli/go-gh>

* **Tcell, Best Go Terminal Low-Level Library**  
  <https://github.com/gdamore/tcell>

  Pure-Go terminal "cell" (curses) library for text terminals; best in
  class at the moment

* **Tview, Best Go Terminal User Interface Library**  
  <https://github.com/rivo/tview>  
  <https://code.rocketnine.space/tslocum/cview>

  It's like having CSS in your terminal (but not); makes short work of
  terminal applications that need regularly used widgets, used by K9S
  and others; `cview`, a forked version, is also good

* **Grab, Highly Concurrent Downloads with Status**  
  <https://github.com/cavaliercoder/grab>

  When you need really good download ability

* **Only Truly Safe Way to Write a File in Go**  
  <https://github.com/rogpeppe/go-internal>

  The internal libraries used by the `go` binary itself; home of
  `lockedfile` (proposed standard addition); *truly* safe writes to a
  file on all operating systems; (You're probably doing it wrong.
  Creating a "lock" file is never enough.)

* **Protobuf Performant Serialization**  
  <https://github.com/protocolbuffers/protobuf>

  Best of breed way to turn a struct into a data stream or file and
  parse it (unmarshal) it back into a struct later; basis of gRPC and
  most Kubernetes communication; replaces JSON APIs for most things

* Glamour, Themed Markdown Rendering for Terminal  
  <https://github.com/charmbracelet/glamour>

  This is the same used for `gh`.

* **modernc.org/sqlite**  
  <https://gitlab.com/cznic/sqlite>

  Package sqlite is a cgo-free port of SQLite. The 20% loss of performance is worth it for most people to have cross-compilation compatibility.

* **SQLX, the Missing SQL Package**  
  <https://github.com/jmoiron/sqlx>

  Without this `database/sql` is remarkably painful to use.

## Learning Resources

There are a lot of bad Go learning resources out there. Most of them are
woefully out of date. Just be really careful. Nothing goes on this this
that isn't 100% relevant to modern Go 1.18+ and available for free
(although I encourage you to support them the best you can).

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

* **Beej's Guide to Network Programming**  
  <https://beej.us/guide/bgnet>

  The book is in C, but so much of Go programming overlaps with that
  domain --- especially with microservices --- that reading this book
  should be mandatory for Go developers (or any developer). It covers
  things like proper UNIX file system semaphores and other architectural
  design concerns that most people coming to coding from academia or
  otherwise just won't think about intuitively.

* **Why Go and Not Rust**  
  <https://kristoff.it/blog/why-go-and-not-rust>>

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
  <https://developers.google.com/protocol-buffers>

  Protobuf format is mandatory learning for any serious Go developer
  wanting to get into microservices or anything that communicates or
  caches with performance requirements.
