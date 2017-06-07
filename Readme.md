# Install XCode-Select
Launch the terminal (it should be within the Utilities folder inside your Applications folder). Run this command inside the terminal to install XCode-Select, which is a bundle of useful command line tools:
`xcode-select --install`

# Install Google Chrome
https://www.google.com/chrome/browser/desktop/ Best browser for web development

# Install ITerm 2
https://www.iterm2.com/downloads.html It's free and much better looking than the default terminal.

# Install YADR + Prezto
YADR is a set of dotfiles that are great for customizing your terminal environment. You can install it by running this command
```sh -c "`curl -fsSL https://raw.githubusercontent.com/skwp/dotfiles/master/install.sh`"```

After installing this, open the `.zshrc` file in your home directory (this should be the directory you start in when you open your terminal) with this command:
`vim .zshrc`

Vim is difficult to use because it's not like your typical code editor. some people swear by it once they become experts, but you should at least know a little bit about it because you'll almost definitely need to use a command line editor at some point while developing.

Common commands:
`i` Insert mode. This mode is like the typing mode you are used to in Microsoft Word or everywhere else. When you type characters, they appear.
`Esc` Visual mode. This is also the mode you start Vim in. you use `h`,`j`,`k`,`l` to move around.
`:w` Save. Save the file.
`:q` Quit. If you made changes and haven't saved, Vim won't let you just quit.
`:wq` Save and Quit. Saves the file first, then quits out of Vim.
`:q!` Force quit. Forces you to quit Vim even if you have unsaved changes.

If you want to learn more about vim, you can type `vimtutor` into your command line. BEWARE... Vim has a steep learning curve and is better learned after you're a seasoned programmer.
After you've figured out how to use Vim basically, add these lines at the bottom:
```
#Disable autocorrect
unsetopt correct_all
unsetopt correct
```


This disables the autocorrect suggestions that ZSH makes, which are often wrong and annoying.

YADR includes Homebrew:
https://brew.sh/ Homebrew is a package manager for macOS. It allows you to easily install many programs from the command line, and you will come across many examples during development where you will use a `brew install` command.

# MacOS Quirks
It's worth noting that MacOS comes bundled with Ruby, Python, and Git (through XCode-Select) but all of these are out of date. If you are using any of these languages, you may want to update them.

# Install a code editor
Suggestions: 
Visual Studio Code (VSCode) https://code.visualstudio.com/
Sublime Text https://www.sublimetext.com/
Atom https://atom.io/

In this doc, I will assume that you choose Visual Studio Code, which I recommend unless you have strong preferences for other editors. VSCode is free and generally faster than Atom. The packages I suggest will be VS Code extensions, although usually the other editors will have equivalent packages. Some people swear by command line code editors such as `emacs` or `vim`. They are convenient because they are accessible in most environments, but I find them to be far less friendly to new programmers, as they are far more difficult to set up.

Side note: if you install Visual Studio Code via the above link, you should be able to start VSCode just by typing `code` in your command line. If you can't, then while you are in VSCode, hold `Cmd + Shift + P` to open the Command Palette and type in `shell`. This should give you the option to install the `code` command in PATH. Run this and you'll be able to run VSCode from your command line.

# Install Yarn
https://yarnpkg.com/lang/en/docs/install/
Yarn is a package manager similar to `npm`. It has a few advantages, most notably local caching of packages for offline development.
If you install Yarn, this will also install NodeJS, which is necessary for running servers in JavaScript. If you choose not to install Yarn, you'll need to install NodeJS separately.

https://nodejs.org/en/ npm comes bundled with NodeJS.

# Useful VSCode Extensions
Must have:
ESLint(vscode-eslint) - This will lint (check for errors) your code according to the code style conventions we set in our .eslintrc file
HTML Snippets(html-snippets) - This will let you complete HTML tags using tab. For example, typing "html" then "tab" will turn into "<html></html>"
TSLint(tslint) - This will lint your TypeScript code. While we won't use TypeScript to begin with, we will incorporate TypeScript into the codebase at some point after we have the basic app completed.

Advanced (Hold off on these until you're comfortable - you'll know when you want these additions):
Prettier(prettier-vscode) - I suggest using this after you're more experienced at JavaScript because it formats your code for you, but you *should* know how to format it yourself first.
Auto Import(autoimport) - Lets you automatically import something by searching through your codebase for dependencies.
Debugger for Chrome(debugger-for-chrome) - Lets you debug using VS Code instead of your browser.






