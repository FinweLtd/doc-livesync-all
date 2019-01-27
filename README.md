LiveSYNC™ Public Documentation
==============================

Abstract
--------

This public repository contains the public documentation of Finwe Ltd.'s LiveSYNC™ software product.
It is targeted for end-users of the product.

Please do not confuse this with Finwe Ltd.'s internal SW documentation, which is targeted for 
software developers and resides in another private repository.

The documentation is intended to be used in a compiled form. The source files, which reside in
the main branch of this repository, consist of a set of textual Markdown (.md) files and related
images, videos etc. files that are referenced from the text files.

Writing
-------

All the docs should be under /docs folder. 

The documentation is written Markdown syntax. Read about it from here:

https://daringfireball.net/projects/markdown/syntax

Try to avoid compiler specific Markdown extensions. As an exception to this rule, we use admonition extension for easily creating notes, warnings, etc. that are typical to user guides:

https://python-markdown.github.io/extensions/admonition/

Examples (these may not show up correctly here but will work in rendered documentation site)
that you can use:

!!! note
    You should note that the title will be automatically capitalized.

!!! caution
    Life is dangerous. People do not survive of it.

!!! danger
    Don't try this at home!

!!! tip
    It is a good idea to sleep sometimes.

To avoid typos and keep the grammar in good shape, it is a good idea to check everything with
tools such as Grammarly and Hemingway Editor. Unfortunately, they cannot be integrated to text
editors or other apps; you must copy-paste text back and forth. It is still worth it!

https://www.grammarly.com

http://www.hemingwayapp.com/

Mkdocs does not have any kind of multi-language support. To keep the markdown files simply, our
approach is simply to fork this documentation site and re-write everything to create a copy of
the site in another language. Remember that also screen captures usually need to be taken again,
hence there is not much other than site structure and some generic images that remains the same.

If *absolutely necessary*, it is possible to mix HTML code (and even CSS code) simply by writing
the tags to their own lines. See /docs/support/support.md as an example where a contact form has 
been embedded to docs. Notice that when the documentation is deployed to GitHub Pages (static pages)
or to GitBook (third party size), it is not really possible to use server side code at all.

**IMPORTANT: Do not touch the CNAME file in /docs folder! This must be left exactly as it is, else
the documentation cannot be found via our custom domain** https://docs.livesync.app

**IMPORTANT: Do not touch file google09912a46c2733839.html! This must be left exactly as it is, else
Google admin tools cannot verify that this domain/website belongs to us.**

If you need to add a comment, use this syntax:

[//]: # (Comment text)

Images
------

Images should be resized to max 1024 pix wide and copied to /docs/img directory or similar
image directories in the directory tree. Please use .jpg or .png images; .png only when alpha 
(transparency) is required as .jpg files are smaller and download much faster.

If you want to use stock images, use archives that provide them royalty free also for commercial
purposes and without attribution requirement. Here are a few good sources:

https://freestocks.org/

https://stocksnap.io/

Using Android Studio as text editor
-----------------------------------

Android Studio IDE is the de facto IDE for software development for Android devices. It is based
on Intellij IDEA and therefore supports plugins developed for it.

The benefits of using Android Studio for writing documentation with MkDocs:

* Familiar tool (for Android developers)

* Good text editor with built-in spell checker

* Easy integration with GitHub repository: pull/commit/push, comparison, branches etc.

* Possibility to put MkDocs 'deploy' and 'serve' commands Tools/External tools menu

* Possibility to add markdown plugin to see rendered markdown side-by-side when editing markdown files

* Possibility to add web browser plugin and see the result side-by-side when editing markdown files

https://plugins.jetbrains.com/plugin/10750-embedded-web-browser-for-idea
NOTE: currently the browser plugin does not seem to work.

Deploying to GitHub Pages via MkDocs
------------------------------------

The documentation can be viewed in a compiled HTML format via this project's public GitHub Pages:
https://finweltd.github.io/doc-livesync-all/

To compile the documentation from .md source files, first commit the changes to the repository, 
and then run 'mkdocs deploy' script - this script will compile the documentation to HTML format
and update the compiled files into the repository's gh-pages branch, where from GitHub Pages 
automatically picks them up.

Notice that you can also preview the documentation live before publishing it by running 
'mkdocs serve' script and opening the documentation locally in a web browser (highly recommended): 

http://localhost:8000/

Local previewing is very handy when writing the documentation, as the web browser will auto-update
content every time a source file is changed and saved.

MkDocs configuration is in mkdocs.yml file. Use it for selecting theme, configuring navigation etc.

MkDocs tool must be installed before it can be used. More info about mkdocs: 

https://www.mkdocs.org/

Deploying to GitBook via GitHub hooks
-------------------------------------

The documentation can also be viewed in GitBook online service:
https://finweltd.gitbook.io/livesync/

Simply commit your changes to the main branch; the GitBook version will be automatically updated 
as it is sync'ed with this GitHub repository.

Notice that it is also possible to use GitBook online editor for writing the documentation, and
to synchronize it back to GitHub repository. However, with this workflow the GitHub Pages version
must be still manually compiled by pulling the source files from the repository and compiling and
deploying them with 'mkdocs deploy' script.

GitBook configuration is in book.json file. See also .bookignore for filtering files from the book.

More info about GitBook: https://docs.gitbook.com/

NOTE: We are currently not making any use of this option. It seems that GitBook cannot produce
a similar structure as easily as it initially seemed, and there is little benefit as site generated
with MkDocs is so good.
