# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

A browser-based Tic Tac Toe game. The entire application is a single self-contained HTML file (`tictactoe.html`) with inline CSS and JavaScript — no build tools, dependencies, or server required.

## Running

Open `tictactoe.html` directly in a browser, or from the command line:

```
start tictactoe.html   # Windows
open tictactoe.html    # macOS
```

## Architecture

Everything lives in `tictactoe.html`:
- **`<style>`** — Dark theme UI, grid layout, animations
- **`<script>`** — Game logic: board state (`cells` array), turn management, win detection against 8 winning combinations (`wins` array), score tracking across rounds

Key functions: `init()` resets the board, `handleClick()` handles moves/win/draw detection.

## Git Workflow

All changes should be committed with clean messages and pushed to GitHub (`origin/master`) after each update.
