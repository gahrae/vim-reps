# Vim Reps

Short Vim editing drills that run in the browser, scored in keystrokes.

**Try it: https://gahrae.github.io/vim-reps/**

Each exercise gives you a buffer and a target. Make the buffer match the target (or land the cursor on the marked spot) in as few keys as you can. Your count is compared with a par, which is the length of a reference solution, and you earn up to three stars. Hints and solutions are there if you get stuck, though peeking at the solution caps that attempt at one star.

There are 56 exercises in 10 lessons. Drill mode picks eight of them and leans towards the ones you haven't got three stars on yet.

## What it covers

This is not an exhaustive Vim tutorial. It only covers the commonly used features, the ones that save the most keystrokes in everyday editing. A lot of Vim is left out on purpose.

| Lesson | Roughly |
| --- | --- |
| Get there faster | `f` and `t`, counts, `%`, `{` and `}`, `G`, search, `*` |
| Operator + motion | `d`, `c`, `gU` and `>` combined with a motion |
| Text objects | `ciw`, `ci"`, `dib`, `cit`, `dap` and friends |
| The dot command | making a change once and repeating it with `.` |
| Small fixes | swapping, joining and duplicating characters and lines |
| Visual and block mode | column edits with `Ctrl-v`, plus sorting a selection |
| Yank, put and registers | `p` with counts, pasting over a selection, the `"0` register |
| Search and replace | `:s`, `:%s`, `:g` and `cgn` |
| Macros | recording with `q` and replaying with `@` |
| Putting it together | a few longer edits that mix the above |

The editor is CodeMirror's Vim emulation, not Vim itself, so the odd command may behave a little differently from what you're used to.

## Running it locally

The whole thing is one file. Clone the repo and open `index.html` in a browser. CodeMirror and the fonts load from CDNs, so you need to be online. Progress is kept in your browser's local storage and nothing is sent anywhere.

## Where to go next

The drills stop at editing a single buffer. Once they feel comfortable, the next step is moving around a whole codebase, which is better practised in a real project in Vim or Neovim. Some topics to look into:

- The jumplist: getting back to where you were with `Ctrl-o` and `Ctrl-i`
- Marks, especially uppercase marks that work across files
- LSP navigation: go to definition, list references, rename a symbol
- Fuzzy-finding files and grepping a project
- The quickfix list, and how to fill it from a grep or a picker
- Project-wide edits with `:cdo` and `:cfdo`, including replaying a macro on every match
