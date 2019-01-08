LiveSYNC Public Documentation
=============================



This repository contains public documentation for Finwe's LiveSYNC software product. It is intended
to be used by end-users. Finwe's internal software documentation is in another private repository.

The source files of the documentation consist of a set of textual Markdown files and related 
images, videos etc. media files that are referenced from the text files.

The documentation can be viewed in compiled HTML format via this project's GitHub Pages. To compile
the documentation, commit the changes to the repository and run 'mkdocs deploy' script; this will
update the documentation into the repository's gh-pages branch where from GitHub Pages picks it up.
The result will appear here: https://finweltd.github.io/doc-livesync-all/

Notice that you can also preview the documentation live by running 'mkdocs serve' script and opening
the documentation locally in a web browser: http://localhost:8000/

MkDocs configuration is in mkdocs.yml file. More info about mkdocs: https://www.mkdocs.org/

The documentation can also be viewed in GitBook online service, where it is automatically sync'ed
from this GitHub repository. Simply commit your changes to the main branch. The result will appear
here: https://finweltd.gitbook.io/livesync/

GitBook configuration is in book.json file. See also .bookignore for filtering files from the book.

All the docs should be in /docs folder. More info about GitBook: https://docs.gitbook.com/
