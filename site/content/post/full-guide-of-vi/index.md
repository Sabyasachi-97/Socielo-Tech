---
title: Full guide of VI
date: 2024-06-28T15:25:49.236Z
description: >
  Hello, this is Sabyasachi and here's a simple guide to get you started with
  using `vi` (or `vim`) in the terminal, along with an explanation of the
  commands written with my practical experience.
image: vim.png
---
# Getting Started with `vi`

`vi` is a text editor you can use in the terminal. Here are the basics to help you get started.

## Starting `vi`

To open `vi` or `vim`, type:

```bash
vi filename
```

If `filename` exists, it will open. If not, a new file with that name will be created.

## Modes in `vi`

`vi` operates in different modes:

1. **Normal mode**: For navigation and basic operations (default mode when you start).
2. **Insert mode**: For inserting text.
3. **Command-line mode**: For saving files, quitting `vi`, etc.

## Switching Modes

- **Normal mode**: Press `Esc` to enter Normal mode.
- **Insert mode**: Press `i` to enter Insert mode.
- **Command-line mode**: Press `:` in Normal mode to enter Command-line mode.

## Basic Navigation in Normal Mode

- `h` : Move left
- `j` : Move down
- `k` : Move up
- `l` : Move right
- `w` : Move to the next word
- `b` : Move to the previous word
- `0` : Move to the beginning of the line
- `$` : Move to the end of the line
- `gg` : Go to the beginning of the file
- `G` : Go to the end of the file
- `:n` : Go to line number `n`

## Inserting Text

To start typing text:

- Press `i` to enter Insert mode.
- Type your text.
- Press `Esc` to return to Normal mode.

## Editing Text in Normal Mode

- `x` : Delete the character under the cursor.
- `X` : Delete the character before the cursor.
- `dw` : Delete from the cursor to the end of the word.
- `dd` : Delete the current line.
- `d$` : Delete from the cursor to the end of the line.
- `yy` : Copy (yank) the current line.
- `yw` : Copy (yank) from the cursor to the end of the word.
- `p` : Paste after the cursor.
- `P` : Paste before the cursor.
- `u` : Undo the last action.
- `Ctrl+r` : Redo the undone action.

## Saving and Quitting

To save your work and quit:

- Press `Esc` to ensure you are in Normal mode.
- Press `:` to enter Command-line mode.
- Type `w` to save the file.
- Type `q` to quit `vi`.

Combining commands:

- `:wq` : Save and quit.
- `:q!` : Quit without saving.

## Visual Mode

For selecting text:

- `v` : Start visual mode (select text).
- `V` : Start visual line mode (select whole lines).
- `Ctrl+v` : Start visual block mode (select rectangular blocks of text).

## Search and Replace

- `/pattern` : Search for `pattern`.
- `?pattern` : Search backward for `pattern`.
- `n` : Repeat the search in the same direction.
- `N` : Repeat the search in the opposite direction.
- `:%s/old/new/g` : Replace all occurrences of `old` with `new` in the file.
- `:s/old/new/g` : Replace all occurrences of `old` with `new` in the current line.

## Exiting `vi`

To exit `vi`, make sure you are in Normal mode (press `Esc` if needed), then:

- `:wq` : Save and quit.
- `:q!` : Quit without saving.

This guide covers the basics. With practice, you'll become more comfortable using `vi` for your text editing needs.
