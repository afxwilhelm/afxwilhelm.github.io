# Adalbert FX Wilhelm's Blog

# How to update the stats tutorial
First we have to understand that the statsTutorial is a git submodule
embedded in this github site, which allows people to access the content at [Stats with R](http://afxwilhelm.github.io/r/t_home/).

If one wants to update the tutorial repository, the best way is to modify the `*.rmd` files and use RStudio to generate the corresponding
html, and then move the generated html files to the `tutorials` folder. This is where all the html files are stored and the `*.rmd` files are the source
files for all the both the descriptions and the R code. When one runs it in RStudio, it would automatically generate the corresponding R output for the code snippets that we have.

After the changes have been pushed to the remote for `statsWithR` repo, one needs to update the commit history of statsWithR as well and push it to the
github page remote so that the github page knows which version of statsWithR to show.

I would highly recommend you to read [working with a git repository within another repository](http://stackoverflow.com/questions/1811730/how-do-i-work-with-a-git-repository-within-another-repository), if you are not sure about how the two-stage git process works.

# Recommended workflow
Since this site is built using [jekyll](https://jekyllrb.com). It is the best to have a local jekyll serve that enables you to run the website locally, otherwise if you need to debug, pushing every single change to the remote is not the best way to find out where the potential error might be and also it will pollute the commit history as well. Look [https://jekyllrb.com/docs/quickstart/] to have a quick-start on how to run jekyll site with localhost.

## License

Open sourced under the [MIT license](LICENSE.md).

