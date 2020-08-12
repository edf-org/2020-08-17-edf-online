# The Carpentries Workshop Template

This repository is based on The Carpentries' ([Software Carpentry][swc-site], [Data Carpentry][dc-site], and
[Library Carpentry][lc-site]'s) template for creating websites for workshops.


## Customizing The Website

If you are already familiar with Git, you can clone the repository to your desktop, edit `index.md`,
`_config.yml`, and `schedule.html` following the instruction above there, and push your changes back to the repository.

```shell
git clone https://github.com/your_username/YYYY-MM-DD-site
```

In order to view your changes once you are done editing, if you have bundler installed (see the
[installation instructions below](#installing-software)), you can preview your site locally with:

```shell
make serve
```
and go to <http://0.0.0.0:4000> to preview your site.

Before pushing your changes to your repository, we recommend that you also check for any potential
issues with your site by running:

```shell
make workshop-check
```

Once you are satisfied with the edits to your site, commit and push the changes to your repository.
A few minutes later, you can go to the GitHub Pages URL for your workshop site and preview it. In the example above, this is `https://gvwilson.github.io/2016-12-01-miskatonic`. The finished
page should look [something like this](fig/completed-page.png?raw=true).


## Additional Notes

**Note:**
this template includes some files and directories that most workshops do not need,
but which provide a standard place to put extra content if desired.
See the [design notes][design] for more information about these.

Further instructions are available in [the customization instructions][customization].
This [FAQ][faq] includes a few extra tips (additions are always welcome)
and these notes on [the background and design][design] of this template may help as well.


## Creating Extra Pages

In rare cases,
you may want to add extra pages to your workshop website.
You can do this by putting either Markdown or HTML pages in the website's root directory
and styling them according to the instructions give in
[the lesson template][lesson-example].


## Installing Software

If you want to set up Jekyll so that you can preview changes on your own machine before pushing them
to GitHub, you must install the software described in the lesson example [setup
instructions](https://carpentries.github.io/lesson-example/setup.html#jekyll-setup-for-lesson-development).


## Setting Up a Separate Repository for Learners

If you are teaching Git,
you should create a separate repository for learners to use in that lesson.
You should not have them use the workshop website repository because:

* your workshop website repository contains many files that most learners don't need to see during
  the lesson, and

* you probably don't want to accidentally merge a damaging pull request from a novice Git user into
  your workshop's website while you are using it to teach.

You can call this repository whatever you like, and add whatever content you need to it.

## Getting and Giving Help

We are committed to offering a pleasant setup experience for our learners and organizers.
If you find bugs in our instructions,
or would like to suggest improvements,
please [file an issue][issues]
or [mail us][email].

[email]: mailto:team@carpentries.org
[customization]: https://carpentries.github.io/workshop-template/customization/index.html
[dc-site]: https://datacarpentry.org
[design]: https://carpentries.github.io/workshop-template/design/index.html
[faq]: https://carpentries.github.io/workshop-template/faq/index.html
[github-project-pages]: https://help.github.com/en/github/working-with-github-pages/creating-a-github-pages-site
[issues]: https://github.com/carpentries/workshop-template/issues
[lesson-example]: https://carpentries.github.io/lesson-example/
[self-organized-workshop-form]: https://amy.carpentries.org/forms/self-organised/
[swc-site]: https://software-carpentry.org
[lc-site]: https://librarycarpentry.org
