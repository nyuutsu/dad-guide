# intro

This website is generated using [mdBook](https://github.com/rust-lang/mdBook).

"```mdBook is a command line tool to create books with Markdown```" - [mdBook's introduction](https://rust-lang.github.io/mdBook/index.html)

[The repository you are currently looking at](https://github.com/nyuutsu/dad-guide) is meant to be fed to mdBook, which generates the content for the website. That content should then be deployed by copying it to a server.

This is going to be difficult to use if you are new to using a command line.

*be on a desktop/laptop & not a phone*

## one-off setup actions

### get mdbook

* [download](https://github.com/rust-lang/mdBook/releases) the most recent version for your OS.

* extract the file to somewhere

* add the location of that file, to your $PATH. You'll know this worked if, upon reopening the terminal, running `mdbook` does stuff instead of just printing a "command not found"-ish error.

### get the extensions the project uses

* [install rust](https://www.rust-lang.org/tools/install)

* run `cargo install mdbook-admonish`

* run `cargo install mdbook`

Congratulations; you made it.

## preview site

* Clone / download the repository

* Be in / `cd` to the project directory

* Run `mdbook serve --open` to open a live-updating preview (that is: when you save one of the files in the project, the preview is updated to reflect the change) of the book.

## edit site

*you need a text/source code editor for this to be pleasant; Word is insufficient; Notepad is insufficient*

Edit things in `src/`. The site content is made out of the `.md` "markdown" text files and any images or videos referenced in them. The site knows which markdown files to use and where to put them in the table of contents based on the structure in `src/SUMMARY.md`.

## generate site files to put online

* Be in / `cd` to the project directory

* Run `mdbook build`; this will generate a bunch of stuff in `book/`. This stuff is *your website*.

* Put the stuff in `book/` on your server

    * e.g. `cd book/ && scp -r * root@nyuu.page:/var/dadbooktest`


## modification date footers (optional, but nice)

To get the modification date footers to work you'll also want to use git to track your changes, host the repository online, and point the thingy in `book.toml` to your repository