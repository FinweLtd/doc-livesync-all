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

All the docs should be in /docs folder. Try to avoid compiler specific Markdown extensions.

If *absolutely necessary*, it is possible to mix HTML code (and even CSS code) simply by writing
the tags to their own lines. See /docs/support.md as an example where a contact form has been
embedded to docs. Notice that when the documentation is deployed to GitHub Pages (static pages)
or to GitBook (third party size), it is not really possible to use server side code at all.

**IMPORTANT: Do not touch the CNAME file in /docs folder! This must be left exactly as it is, else
the documentation cannot be found via our custom domain** https://docs.livesync.app

**IMPORTANT: Do not touch file google09912a46c2733839.html! This must be left exactly as it is, else
Google admin tools cannot verify that this domain/website belongs to us.**

Images
------

Images should be resize to max 1024 pix wide and copied to /docs/img directory. Please use .jpg
or .png images; .png only when alpha (transparency) is required.

If you want to use stock images, use archives that provide them royalty free also for commercial
purposes and without attribution requirement. Here are a few good sources:

https://freestocks.org/
https://stocksnap.io/

Deploying to GitHub Pages via MkDocs
------------------------------------

The documentation can be viewed in a compiled HTML format via this project's public GitHub Pages:
https://finweltd.github.io/doc-livesync-all/

To compile the documentation from .md source files, first commit the changes to the repository, 
and then run 'mkdocs deploy' script - this script will compile the documentation to HTML format
and update the compiled files into the repository's gh-pages branch, where from GitHub Pages 
automatically picks them up.

Notice that you can also preview the documentation live before publishing it by running 
'mkdocs serve' script and opening the documentation locally in a web browser: http://localhost:8000/

Local previewing is very handy when writing the documentation, as the web browser will auto-update
content every time a source file is changed and saved.

MkDocs configuration is in mkdocs.yml file. Use it for selecting theme, configuring navigation etc.

MkDocs tool must be installed before it can be used. More info about mkdocs: https://www.mkdocs.org/

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
