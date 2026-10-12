# Linux `man` Commands Explained

`man` opens the **manual (help pages)** for a command. These notes explain each command I practiced, in the order I ran them.

## Commands

| # | Command | What it does |
|---|---------|--------------|
| 1 | `man` | Used alone, it does nothing useful. It asks which manual page you want, because you must give a name. |
| 2 | `man man` | Opens the manual for the `man` command itself. |
| 3 | `man ls` | Opens the manual for the `ls` command. |
| 4 | `man 8 ls` | Tries to open the `ls` page in **section 8** (system administration commands). `ls` has no page there, so it shows "No manual entry". |
| 5 | `man -f ls` | `-f` shows a **one-line description** of every manual page named `ls`, without opening the full page. |
| 6 | `man -f intro` | Shows the one-line descriptions of all `intro` pages. There is one for each section (1, 2, 3 and so on). |
| 7 | `man intro` | Opens the first `intro` page found (section 1), an introduction to user commands. |
| 8 | `man -f ls` | Same as command 5. I repeated it to compare the result. |

## Manual sections

Manual pages are grouped into numbered sections. This is why `man 8 ls` gave an error.

| Section | Contents |
|---------|----------|
| 1 | User commands (like `ls`) |
| 2 | System calls |
| 3 | Library functions |
| 4 | Special files (devices) |
| 5 | File formats and configuration files |
| 6 | Games |
| 7 | Miscellaneous |
| 8 | System administration commands |

## Moving around inside a manual page

| Key | Action |
|-----|--------|
| `Space` | Go down one page |
| `b` | Go back one page |
| `/word` | Search for a word, then press `n` for the next match |
| `q` | Quit and return to the terminal |

## What I learned

- `man <command>` is the quickest way to see how a command works and what options it has.
- `man -f <name>` gives a short summary and shows which sections have a page with that name.
- `man <section> <command>` opens a page from one specific section.
- Press `q` to leave a manual page.
