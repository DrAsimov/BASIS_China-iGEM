# BASIS_China iGEM Wiki Repository

This page contains the basic information for the setup of our wiki page. You can find the full official iGEM requirements [here](https://competition.igem.org/deliverables/team-wiki). 

I cloned the [sample wiki](https://gitlab.igem.org/2022/example), and you can see the essential information below:

***
***

## How to edit

> You should probably only edit the files inside folders `static`, `wiki` and `wiki > pages`.
> 1. Open the Web IDE
> 2. Make the changes on the files you wish:
>     * For the menu, change the file [menu.html](wiki/menu.html)
>     * For the layout, change the file [layout.html](wiki/layout.html)
>     * For the pages, change the corresponding file in the folder [pages](wiki/pages)
> 3. Review the changes you made
> 4. Once you are done, save the changes by **committing** them to the *main branch* of the repository
> 5. An automated script will build, test and deploy your wiki, which should take less than 30 seconds.

## File layout

The static assets are in the `static` directory. The layout and templates are in the `wiki` directory, and the pages live in the `wiki > pages` directory. Unless you are an experienced and/or adventurous human, you probably shouldn't change other files.

    |__ static/             -> static assets (CSS and JavaScript files only)
    |__ wiki/               -> Main directory for the pages and layouts
        |__ footer.html     -> Footer that will appear in all the pages
        |__ layout.html     -> Main layout of your wiki. All the pages will follow its structure
        |__ menu.html       -> Menu that will appear in all the pages
        |__ wiki-tools.html -> Wiki tools to help getting started with this template
        |__ pages/          -> Directory for all the pages
            |__ *.html      -> Actual pages of your wiki
    |__ .gitignore          -> Tells GitLab which files/directories should not be uploaded to the repository
    |__ .gitlab-ci.yml      -> Automated flow for building, testing and deploying your website.
    |__ LICENSE             -> License CC-by-4.0, all wikis are required to have this license - DO NOT MODIFY
    |__ README.md           -> File containing the text you are reading right now
    |__ app.py              -> Python code managing your wiki
    |__ dependencies.txt    -> Software dependencies from the Python code

