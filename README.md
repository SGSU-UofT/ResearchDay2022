# ResearchDay2022

This website is made using the R package distill. Information about how to make a website with this package is available [here](https://rstudio.github.io/distill/website.html). I will provide a brief summary of how to modify this website, but the distill documentation is the best resource for making changes.

You can create a new distill webpage by creating a project using the distill template in RStudio (make sure you install distill first). To build the website locally and preview your changes before pushing your updates, click "Build Website" on the Build panel in RStudio. Building the website creates all the html from the Rmarkdown files, which are stored in the docs folder, and actually form the website.

The _site.yml controls the site layout and the theme.css file controls its look. To add a new page, create a new Rmarkdown file newpage.Rmd and add it to the .yml:
```
    - text: "My new page"
      href: newpage.html
```

To make a new version of this website (ex. Research Day 2023), make another repository with this name and copy over these contents, or start from scratch by creating an RStudio project with the distill template. To launch the website, turn on GitHub pages and make sure it is being built from the docs folder. You also need to make sure the .nojkeyll file is in the repo. More info [here](https://rstudio.github.io/distill/publish_website.html). Your repository name will set the url for your new website (ex. if we create a repo called ResearchDay2023, it will be at https://sgsu-uoft.github.io/ResearchDay2023/).
