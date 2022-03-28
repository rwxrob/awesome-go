# My Personal "Awesome" Go List

> "Oh really, Jessie, does it inspire awe?" (Jane, Breaking Bad)

I'm not a fan of most "awesome" lists. Most of them are full of shit and
are more about promoting that shit than anything else. My list has two
purposes, 1) so I can find my own awesome stuff later and keep it
organized when I discover some new way to do something simpler, and 2)
so I can curate a truly amazing list of awe-inspiring packages (usually
stuff I actual pay my own money to sponsor, it's that good).

## My Own Stuff

Here's where I keep track of all the little utilities I make for
different things and know where to put them at a glance (not everything
should go in `util`, \*cough\* "ioutils", right?)

* [rwxrob/bonzai](https://github.com/rwxrob/bonzai) - Go commander with
  command composition, recursive tab completion, rich embedded command
  documentation (markdown, formatted, pager-aware, color, interactive
  terminal detection), library of completers (files, dates, calculator)
  and composable commands (help, config)

* [rwxrob/z](https://github.com/rwxrob/z) - my personal, portable Bonzai
  command tree, use it for ideas to start your own composable command
  utility monolith (and replace all those shell scripts)

* [rwxrob/config](https://github.com/rwxrob/config) - universal
  YAML configuration management as a Bonzai branch (composable command),
  default for all bonzai.Cmds

* [rwxrob/scan](https://github.com/rwxrob/scan) - universal rune scanner
  and optional node-tree parser designed for rapid grammar and
  domain-specific language development with intuitive methods and
  traceable scan.X expression language interpreter in pure Go for easy
  code generation from meta languages such as PEGN

* [rwxrob/fn](https://github.com/rwxrob/fn) - my own collection of
  map/filter/reduce/each in Go with generics, `fn.A` functional array
  type, library of map functions (mapf), map transformations (maps),
  filters (filt) (you might prefer [samber/lo](https://github.com/samber/lo))

* [rwxrob/fs](https://github.com/rwxrob/fs) - supplements the
  standard filesystem functions with simplifications and extras

* [rwxrob/json](https://github.com/rwxrob/json) - supplements
  `encoding/json`, includes unmarshaling JSON from HTTP requests into
  any type that can be passed to `json.Unmarshal`

* [rwxrob/term](https://github.com/rwxrob/term) - VT100 ANSI terminal
  escapes, no wasteful function calls just to change colors or terminal
  state, interactive terminal detection, window size queries, reading
  user input

* [rwxrob/to](https://github.com/rwxrob/to) - library of converter
  utility functions

* [rwxrob/structs](https://github.com/rwxrob/structs) - traditional data
  structures (list, set, stack, node, tree, etc.) implemented with rapid
  applications development (replacing shell scripts) as design priority

* [rwxrob/y2j](https://github.com/rwxrob/y2j) - YAML to JSON Bonzai
  branch (composable command) including `pkg/y2j.Convert` high-level
  function for importing without Bonzai

* [rwxrob/yq](https://github.com/rwxrob/yq) - popular `yq` tool as a
  Bonzai branch (composable command, instead of Cobra), includes
  "batteries included" `pkg/yq.Evaluate` call to `yqlib` with reasonable
  defaults for importing without Bonzai

## Other Awesome Stuff

I curate this list myself and do not accept pull requests. I'm *very*
picky about what makes it onto it. I am open to suggestions if you'd
like to open an issue.

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
  of `lockedfile` (proposed standard addition), the only want to ever
  write safely to a file on all operating systems (hint: you're probably
  doing it wrong, creating a "lock" file is never enough)), this is
  currently how `go` binary handles system-wide file read/write locking

## Learning Resources

There are a lot of bad Go learning resources out there. Most of them
are woefully out of date. Just be really careful. Nothing goes on this
this that isn't 100% relevant to modern Go 1.18+.

* Go-Nuts USENET Newsgroup.  
  <https://groups.google.com/g/golang-nuts>

  This is where the creators and Go project leaders are regularly
  answering questions and discussing the direction of the language. This
  resource is far better than Reddit and even the official Go Discord
  channel (which you can find from <https://go.dev>). Keep in mind that
  anything ever written here is permanently saved, forever. I prefer
  this because all submissions are moderated and people actually take a
  moment to consider what they write before posting toxic crap (unlike
  Reddit and Discord, etc.)

* Get Programming with Go  
  <https://www.manning.com/books/get-programming-with-go>

  This book seems like the best for absolute beginners since it assumes
  you know nothing about programming at all and uses the Go playground
  and nothing more and doesn't get into the weeds about modules and
  project management and stuff (which is also its greatest weakness
  since you have to learn that stuff as well before doing anything
  significant with it). I intend to use this book (and the author has
  volunteered to help) during the [2022 Beginner
  Boost](https://github.com/rwxrob/boost) on May 4th.

* Go Code Review Comments  
  <https://github.com/golang/go/wiki/CodeReviewComments>

* Beej's Guide to Network Programming  
  http://beej.us/guide/bgnet/

  The book is in C, but so much of Go programming overlaps with that
  domain --- especially with microservices --- that reading this book
  should be mandatory for Go developers (or any developer). It covers
  things like proper UNIX file system semaphores and other architectural
  design concerns that most people coming to coding from academia or
  otherwise just won't think about intuitively.
