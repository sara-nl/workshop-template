# Initial acknowledgement

The present for SURF workshops has been imported originally from the template available from [The Carpentries][carpentries]. The information included in this README file and the rest of content in this template has been adapted to be used by workshops (co-)organized at [SURF][surf]. Please feel free to read and contribute!

# workshop-template

This repository is the SURF template for creating websites for workshops.

1.  Please *do not fork this repository directly on GitHub.*
    Instead, please use GitHub's importer following [the instructions below](#creating-a-repository)
    to copy this `workshop-template` repository and customize it for your workshop.

2.  Please *do your work in your repository's `gh-pages` branch*,
    since that is what is
    [automatically published as a website by GitHub][github-project-pages].

3.  Once you are done, please also [let us know][email] the workshop URL.

## Creating a Repository

1.  Log in to GitHub.
    (If you do not have an account, you can quickly create one for free.)
    You must be logged in for the remaining steps to work.

2.  Go to <a href="https://github.com/new/import" target="_blank">GitHub's importer</a>.

3.  Paste the url of this repo as the old repository to clone:
    <https://github.com/carpentries/workshop-template>.

4.  Select the owner for your new repository.
    (This will probably be you, but may instead be an organization you belong to.)

5.  Choose a name for your workshop website repository.
    This name should have the form `YYYY-MM-DD-site`,
    e.g., `2016-12-01-miskatonic`,
    where `YYYY-MM-DD` is the start date of the workshop.

6.  Make sure the repository is public.

7.  At this point, you should have a page like this:

    ![](fig/using-github-import.png?raw=true)

    You can now click "Begin Import".
    When the process is done,
    you will receive a message like
    "Importing complete! Your new repository jules32/2015-07-01-miskatonic is ready."
    and you can go to the new repository by clicking on the name.

**Note:**
some people have had intermittent errors during the import process,
possibly because of the network timing out.
If you experience a problem, please re-try;
if the problem persists,
please [get in touch](#getting-and-giving-help).

## Customizing Your Website

1.  Go into your newly-created repository,
    which will be at `https://github.com/your_username/YYYY-MM-DD-site`.
    For example,
    if your username is `gvwilson`,
    the repository's URL will be `https://github.com/gvwilson/2016-12-01-miskatonic`.

3.  Ensure you are on the gh-pages branch by clicking on the branch under the drop 
    down in the menu bar (see the note below):

    ![](fig/select-gh-pages-branch.png?raw=true)

3.  Edit the header of `index.md` to customize the list of instructors,
    workshop venue, etc. 
    You can do this in the browser by clicking on it in the file view on GitHub
    and then selecting the pencil icon in the menu bar:

    ![](fig/edit-index-file-menu-bar.png?raw=true)
    
    Editing hints are embedded in `index.md`,
    and full instructions are in [the customization instructions][customization].
    
4.  Edit `_config.yml` to customize certain site-wide variables, such as: `carpentry` (to tell us which carpentry workshop this is), `title` (overall title for all pages), `workshop_repo` (the URL of the workshop repository on GitHub) and `workshop_site` (the repository's GitHub Pages URL).

    Editing hints are embedded in `_config.yml`,
    and full instructions are in [the customization instructions][customization].
    
5. Edit the `schedule.html` file to edit the schedule for your upcoming workshop. This file is located in the `_includes` directory, make sure to choose the one from the appropriate `dc` (Data Carpentry workshop), `lc` (Library Carpentry), or `sc` (Software Carpentry) subdirectory.

6.  Alternatively,
    if you are already familiar with Git,
    you can clone the repository to your desktop,
    edit `index.md`, `_config.yml`, and `schedule.html` there,
    and push your changes back to the repository.

    ~~~
    git clone -b gh-pages https://github.com/your_username/YYYY-MM-DD-site
    ~~~

    You should specify `-b gh-pages` to checkout the gh-pages branch because the imported 
    repository doesn't have a `master` branch.

    In order to view your changes once you are done editing,
    you must push to your GitHub repository:

    ~~~
    git push origin gh-pages
    ~~~

7.  When you are done editing,
    go to the GitHub Pages URL for your workshop and preview your changes.
    In the example above, this is `https://gvwilson.github.io/2016-12-01-miskatonic`.
    The finished page should look [something like this](fig/completed-page.png?raw=true).

8.  Optional: you can now change the README.md file in your website's repository, which contains these instructions, so that it contains a short description of your workshop and a link to the workshop website.

9.  Optional: Add a link to your workshop website on the repository main page in the description/website section (look for the `Edit` button on the right to add).  

**Note:**
please do all of your work in your repository's `gh-pages` branch,
since [GitHub automatically publishes that as a website][github-project-pages].

**Note:**
this template includes some files and directories that most workshops do not need,
but which provide a standard place to put extra content if desired.
See the [design notes][design] for more information about these.

Further instructions are available in [the customization instructions][customization].
This [FAQ][faq] includes a few extra tips (additions are always welcome)
and these notes on [the background and design][design] of this template may help as well.

## (Optional) Linking to Your Page

At the top of your repository on GitHub you'll see

~~~
No description, website, or topics provided. — Edit
~~~

Click 'Edit' and add:

1.  A very brief description of your workshop in the "Description" box (e.g., "Miskatonic University workshop, Dec. 2016")

2.  The URL for your workshop in the "Website" box (e.g., `https://gvwilson.github.io/2016-12-01-miskatonic`)

This will help people find your website if they come to your repository's home page.

## Getting and Giving Help

The best way for communication is to [send a mail][email]

[carpentries]: https://github.com/carpentries/workshop-template/
[email]: mailto:training@surfsara.nl
[customization]: https://sara-nl.github.io/workshop-template/customization/
[surf]: http://www.surf.nl
[design]: https://carpentries.github.io/workshop-template/design/
[faq]: https://carpentries.github.io/workshop-template/faq/
[github-project-pages]: https://help.github.com/articles/creating-project-pages-manually/
