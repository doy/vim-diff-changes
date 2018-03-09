# Overview

This plugin adds commands which diff the current buffer against the file it
was loaded from, either the state on disk or the state in version control
(similar to `vimdiff` except without requiring writing the buffer state to
disk).

# Installation

This plugin can be installed as a standard Vim package (see `:help packages`).
Simply clone this repository into ~/.vim/pack/plugins/start/vim-diff-changes to
install the Vim files for this plugin.

# Commands

## `:DiffAgainstFilesystem`

Opens a diff window which diffs the buffer contents against the contents of
the file on disk. Use `:DiffStop` to close the diff window.

## `:DiffAgainstVCS`

Opens a diff window which diffs the buffer contents against the contents of
the file in the most recent commit in version control. Use `:DiffStop` to
close the diff window. Supports git, svn, darcs, and cvs.

## `:DiffStop`

Closes an active diff window.
