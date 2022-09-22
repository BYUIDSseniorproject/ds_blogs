# Creating a Quarto Blog (Github.io style)

## The steps

0. Make sure you have a GitHub account and Git installed on your computer.
1. [Install Quarto CLI](https://quarto.org/docs/get-started/).
2. [Install VS Code](https://code.visualstudio.com/).
3. [Install the Quarto extension](https://marketplace.visualstudio.com/items?itemName=quarto.quarto)
4. Create a GitHub repo. We recommend the repo be [username].github.io (see [Github guidance](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site))
5. Clone your repo.
6. Open that folder in VS Code and execute `quarto create-project --type website:blog` in the Terminal. ([quarto create-project command](https://quarto.org/docs/projects/quarto-projects.html))
7. Now navigate to the `index.qmd` file and Render the file (hotkey: ctrl-shift-k (Windows), cmd-shift-k (Mac)) to see the default material created with the command from step 6.
7. Now, edit the files created.
    A. `profile.jpg` should be a picture of you.
    B. Edit `about.qmd` with your links and text.   
    C. Edit your `_quarto.yml` to improve the title, [icons](https://icons.getbootstrap.com/), links and your default [theme](https://bootswatch.com/).   
    D. Add `output-dir: docs` to line three of `_quarto.yml` at the correct tab set.   
8. Delete one of the folders in `/posts` and update the other folder name and `.qmd` to start your first post.
9. Rerender your site again (hotkey: ctrl-shift-k (Windows), cmd-shift-k (Mac))
10. Commit your changes and push your changes to GitHub
11. Navigate to your repository on Github and click on `Settings`.
12. Navigate using `Pages` in the left navigation, change the `branch` settings to `main` and `/docs` and finalize with the `save` button.
13. Copy your URL and then use that URL to reference your website (note: can take a little time to build or refresh)
14. Start writing about data science.

## Details

- [Quarto: Get Started](https://quarto.org/docs/get-started/)
- [Quarto: Creating a blog](https://quarto.org/docs/websites/website-blog.html)
- [Quarto: website options](https://quarto.org/docs/reference/projects/websites.html)
- [Quarto: themes](https://quarto.org/docs/output-formats/html-themes.html)
- [Quarto: GitHub Pages](https://quarto.org/docs/publishing/github-pages.html)
- [External preview in VS Code](https://quarto.org/docs/get-started/hello/vscode.html#external-preview)
- [Quarto: Github actions](https://github.com/quarto-dev/quarto-actions)

## What is ...

Here are a few details on each of the key tools used to build your Quarto blog.

### [VS Code](https://code.visualstudio.com/)

VS Code is a free code editor that has taken over the developer world. It is a great replacement for the RStudio IDE.

### [Quarto](https://quarto.org/)

Quarto `.qmd` is ~~RStudio's~~ Posit's evolution of an RMarkdown file (`.qmd`). It is an open-source scientific and technical publishing system built on [Pandoc](https://pandoc.org/)

- Create dynamic content with [Python](https://quarto.org/docs/computations/python.html), [R](https://quarto.org/docs/computations/r.html), [Julia](https://quarto.org/docs/computations/julia.html), and [Observable](https://quarto.org/docs/computations/ojs.html).
- Author documents as plain text markdown or [Jupyter](https://jupyter.org/) notebooks.
- Publish high-quality articles, reports, presentations, websites, blogs, and books in HTML, PDF, MS Word, ePub, and more.
- Author with scientific markdown, including equations, citations, crossrefs, figure panels, callouts, advanced layout, and more.

### [Github](https://github.com/)

The place where code is shared.  It is owned by Microsoft. We use it heavily in the DS program.

### [Github Actions](https://docs.github.com/en/actions/learn-github-actions/understanding-github-actions)

GitHub Actions is a continuous integration and continuous delivery (CI/CD) platform that allows you to automate your build, test, and deployment pipeline. You can create workflows that build and test every pull request to your repository, or deploy merged pull requests to production.

GitHub Actions goes beyond just DevOps and lets you run workflows when other events happen in your repository. For example, you can run a workflow to automatically add the appropriate labels whenever someone creates a new issue in your repository.

GitHub provides Linux, Windows, and macOS virtual machines to run your workflows, or you can host your own self-hosted runners in your own data center or cloud infrastructure.

