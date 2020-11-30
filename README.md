### Overview

Clink combines the native Windows shell `cmd.exe` with the powerful command line editing features of the GNU Readline library, which provides rich completion, history, and line-editing capabilities. Readline is best known for its use in the well-known Unix shell Bash, the standard shell for Mac OS X and many Linux distributions.

### Download

Downloads are available from the [releases](https://github.com/chrisant996/clink/releases) page.

> There are no production releases yet; currently only pre-release builds are available, for testing purposes.

See the [issues](https://github.com/chrisant996/clink/issues) page for known issues or to file new issues.

### Features

- The same line editing as Bash (from the [GNU Readline library](https://tiswww.case.edu/php/chet/readline/rltop.html) version 8.0).
- History persistence between sessions.
- Context sensitive completion;
    - Executables (and aliases).
    - Directory commands.
    - Environment variables
    - Thirdparty tools; Git, Mercurial, SVN, Go, and P4.
- New keyboard shortcuts;
    - Paste from clipboard (<kbd>Ctrl</kbd>+<kbd>V</kbd>).
    - Incremental history search (<kbd>Ctrl</kbd>+<kbd>R</kbd>/<kbd>Ctrl</kbd>+<kbd>S</kbd>).
    - Powerful completion (<kbd>Tab</kbd>).
    - Undo (<kbd>Ctrl</kbd>+<kbd>Z</kbd>).
    - Automatic `cd ..` (<kbd>Ctrl</kbd>+<kbd>PgUp</kbd>).
    - Environment variable expansion (<kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>E</kbd>).
    - Doskey alias expansion (<kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>F</kbd>).
    - (press <kbd>Alt</kbd>+<kbd>H</kbd>) for many more...)
- Scriptable completion with Lua.
- Coloured and scriptable prompt.
- Auto-answering of the "Terminate batch job?" prompt.

### Usage

There are a variety of ways to start Clink;

1. If you installed the auto-run, just start `cmd.exe`. Run `clink autorun --help` for more info.
2. To manually start, run the Clink shortcut from the Start menu (or the clink.bat located in the install directory).
3. To establish Clink to an existing `cmd.exe` process, use `<install_dir>\clink.exe inject`

### Extending Clink

Clink can be extended through its Lua API which allows easy creation of context sensitive match generators, prompt filtering, and more. More details can be found in Clink's documentation [here](https://chrisant996.github.io/clink/clink.html).
