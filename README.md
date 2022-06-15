This is the repository for the webpage of trust-cps-group at TU Vienna. This README is intended as a guide on how to test the site locally as well as on how to publish changes.

## <a name="setup"></a>Setup x

As we do not want to work in the browser, the first step is to clone the repository, e.g., via ssh

    git clone git@github.com:trust-cps-group/trust-cps-group.github.io.git

Now you can make changes as you like and commit them. I have set up a github workflow which takes care of rendering and publishing. This workflow is triggered everytime a new commit is pushed to the `main` branch. Note that rendering may take some seconds, so your changes will not directly be available. You can check the current state of the workflow [here](https://github.com/trust-cps-group/trust-cps-group.github.io/actions) or by manually navigating to the actions-tab. If there is a green checkmark before the last build, everything went fine and your changes are published. If not, please check the logs and/or contact me (Stefan).

### Testing locally

To avoid waiting for the workflow for every small change you can run a local server which directly renders all changes you made and you can check your changes directly. To set this up, follow these steps

1. Clone the repository (see [Setup](#setup))
2. [Install Ruby](https://www.ruby-lang.org/en/documentation/installation/)
2. [Install Jekyll](https://jekyllrb.com/docs/installation/), direct links to OS-dependend guides:
  - [Ubuntu](https://jekyllrb.com/docs/installation/ubuntu/)
  - [OSX](https://jekyllrb.com/docs/installation/macos/)
  - [Windows](https://jekyllrb.com/docs/installation/windows/)
3. [Install bundler](https://bundler.io/) by running `gem install bundler`
4. Navigate into the repository folder and run `bundler install` to install all dependencies required for our page.

These steps should only be executed once, after that you can run `bundle exec jekyll serve` which will render the page and start a local webserver. The bundler watches for changes and re-renders the page when you change pages and save your changes. Visit [http://127.0.0.1:4000/](http://127.0.0.1:4000/) to see a local version of the page.

Note that in some cases (if dependencies have changed) you need to re-run `bundler install` before being able to test locally. Similarly, if you change configuration files (usually *.yml files), you need to re-start the webserver to have those changes take effect.

### Structure of the Pages

For basic changes, the folder `pages` and its subfolders are of importance. You can modify most of the pages directly, note that the pages for research-projects (research.md) and the page showing the group (people.md) have their own layout and thus changes there might not have the desired effect (for those pages, look at _layouts/research-tiles.html or at _layouts/people-tiles.html).

All other pages are basic markdown pages - syntax see either my page (pages/people/stefan_schupp.md) or have a look at [this guide](https://www.markdownguide.org/basic-syntax/).

Your personal pages are in `pages/people/yourname.md`, the individual research projects are in `pages/research_projects/projectname.md`.
All images should be put in the `images` folder, maybe set up a subfolder, if it makes sense.

#### Adding new pages

If you need to add a new page, which should also be part of the navigation bar, take a look at the file `_data/navigation.yml` in which the items of the nav-bar are specified. The page itself can be added in the pages folder, make sure the naming is consistent.
