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

* [rwxrob/bonzai](https://github.com/rwxrob/bonzai) - BusyBox-like
  (multi-call binary) command composition, recursive tab completion,
  rich embedded command documentation (markdown, formatted, pager-aware,
  color, interactive terminal detection), library of completers (files,
  dates, calculator) and composable commands (help, config) 

* [rwxrob/scan](https://github.com/rwxrob/scan) - universal rune
  scanner and optional parser designed for rapid applications
  development without sacrificing performance, batteries included, zero
  function recursion, intuitive methods, optional JSON ASTs, clean
  rooted node tree structure, easy to generate code from PEGN, PEG,
  ABNF, EBNF, regular expressions

* [rwxrob/fn](https://github.com/rwxrob/fn) - map/filter/reduce/each in
  Go with generics, `fn.A` functional array type, library of map
  functions (mapf), map transformations (maps), filters (filt)

* [rwxrob/http](https://github.com/rwxrob/http) - basically `curl` in
  Go, all the most common simple request with generic marshaling
  including HTTP pipelines to populate fields in single struct between
  multiple, chained HTTP requests of any type

* [rwxrob/structs](https://github.com/rwxrob/structs) - traditional data
  structures (list, set, stack, node, tree, etc.) implemented with rapid
  applications development (replacing shell scripts) as design priority

* [rwxrob/term](https://github.com/rwxrob/term) - VT100 ANSI terminal
  escapes, no wasteful function calls just to change colors or terminal
  state, interactive terminal detection, window size queries, reading
  user input

* [rwxrob/to](https://github.com/rwxrob/to) - library of converter
  utility functions

* [rwxrob/json](https://github.com/rwxrob/json) - supplements
  `encoding/json`, no unnecessary escapes

* [rwxrob/fs](https://github.com/rwxrob/fs) - supplements the
  standard filesystem functions with simplifications and extras

## Other Awesome Stuff

I curate this list myself and do not accept pull requests. I'm *very*
picky about what makes it onto this list. I am open to suggestions if
you'd like to open an issue.

* [gdamore/tcell](https://github.com/gdamore/tcell) - cell-based view
  for text terminals, favorite library for creating terminal apps

* [rivo/tview](https://github.com/rivo/tview) - it's like having CSS in
  your terminal (but not), makes short work of terminal applications
  that need regularly used widgets
