# Adding pages

This documentation is written and built with use of [MKdocs](https://www.mkdocs.org/).  

If you want to read about how to make pages using the proper format MKdocs support look here => [https://www.mkdocs.org/user-guide/writing-your-docs/](https://www.mkdocs.org/user-guide/writing-your-docs/)  

The gist of it all is MKdocs uses the Markdown format to write pages, and makes use of python to build the site and serve the files as static pages.

For full documentation visit [mkdocs.org](https://www.mkdocs.org).

## Commands

* `mkdocs new [dir-name]` - Create a new project.
* `mkdocs serve` - Start the live-reloading docs server.
* `mkdocs build` - Build the documentation site.
* `mkdocs -h` - Print help message and exit.

If you are working on windows, you may have to prefix your commands with  

```python -m```

For further MKdocs prerequisites check here => [https://www.mkdocs.org/user-guide/installation/](https://www.mkdocs.org/user-guide/installation/)

## Project layout

    mkdocs.yml    # The configuration file.
    docs/
        index.md  # The documentation homepage.
        ...       # Other markdown pages, images and other files.