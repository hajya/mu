# Documentation Sample / Test file / Advanced doc features

## mkdocs macros plugin

This plugin allows providing some variables in mkdocs.yml file and then reference those variables using jinja2 syntax in md files.  Most of these variables are populated and created during the DocBuild step and inserted into the yml file.

* Docs: https://mkdocs-macros-plugin.readthedocs.io/en/latest/

* Src Project: https://github.com/fralau/mkdocs_macros_plugin

## Material theme

This theme provides the skin for the site.  This also provides capabilities thru plugins.

https://squidfunk.github.io/mkdocs-material/

## Markdown Extensions

The Material theme supports markdown extensions.  Check the yml file for what extensions are currently on.  Below is more specific info.

https://squidfunk.github.io/mkdocs-material/extensions/permalinks/
https://squidfunk.github.io/mkdocs-material/extensions/pymdown/

### Admonition plugin

This plugin in combo with the material theme provides great looking ways for doc developers to highlight parts of their message.
Please check out: https://squidfunk.github.io/mkdocs-material/extensions/admonition/ for the capabilities and syntax.

One example:

!!! note
    Sample note here.

### emoji support

Who doesn't love using emojis. Icon usage has shown to help communicate directions and cross language barriers.
https://facelessuser.github.io/pymdown-extensions/extensions/emoji/

:smile: :alien:
:material-airplane:
:material-ambulance:
:material-github:

Twitter, github, and emojione tags available.

### Tab support

You can now use tabs to organize your content.

=== "Basic Example Tab1"
    Some content in tab1
=== "Example Tab2"
    More content in tab2
=== "Link to More details"
    https://facelessuser.github.io/pymdown-extensions/extensions/tabbed/

### Mermaid Charts

A picture is worth 1000 words so lets make a few. :smile:
Mermaid supports a rich, easily integrated set.
https://mermaid-js.github.io/mermaid/

This is done with custom superfences configuration.
See here: https://github.com/squidfunk/mkdocs-material/issues/693#issuecomment-591933381

To support this the Mermaid format is supported.

=== "Chart Result"

    ```mermaid
    graph TD;
        A-->B;
        A-->C;
        B-->D;
        C-->D;
    ```

=== "Markdown Syntax"

    ``` md
        ```mermaid
        graph TD;
            A-->B;
            A-->C;
            B-->D;
            C-->D;
        ```
    ```

### Others

Check out the mkdocs.yml file for other extensions and details can be found in the links above.
