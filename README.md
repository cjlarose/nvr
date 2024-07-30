# nvr

If invoked outside of Neovim, `nvr [*args]` just invokes `nvim [*args]`. If invoked from within Neovim (such as in a terminal buffer), `nvr [*args]` will open a new split window in the existing Neovim session.

## Usage

`nvr` is intended to be usable as your `$EDITOR` or `$GIT_EDITOR`, so that when you invoke commands like `git commit` within a Neovim terminal buffer, a new split window appears in the existing Neovim session (instead of in a nested Neovim session). After writing a commit message, exit the window with `:q`. That will delete the temporary buffer and signal to `git commit` that you're finished authoring your commit message.
