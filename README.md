# Exam Template Using R Markdown

This repo contains a customizable R Markdown exam template.

# Downloading the Repo

## Method 1: Using R

### Method 1 a): `usethis::use_course()`

Install and load the `usethis` package and download with `use_course`:

```{r}
# install.packages("usethis")
library("usethis")
usethis::use_course("hubchev/temp_exam", destdir = getwd())
```

By default it downloads the repo into a directory and stores it in your working directory. Feel free to replace `getwd()` with `"path/to/destination"`, i.w., the desired location on your system where you want to download the repo.

### Method 1 b): `quarto_use_template()`

Install the [quarto package](https://quarto-dev.github.io/quarto-r/) (version = 1.4 or higher). The quarto package is not Quarto itself, but it provides
convenient functions to interact with Quarto and R Markdown.

If the quarto package is not installed, you can can install it by
running this code in the console:

``` r
install.packages("quarto")
```

Once the quarto package is installed, you can copy the template by setting your working directory to the directory where you want the template to be installed (e.g., `setwd("path/to/my/folder")`). Make sure that the directory is empty and run this command:

```{r}
quarto::quarto_use_template("hubchev/temp_exam")
```

A prompt will ask if you trust the author (me) not to run malicious
code. To proceed, answer `Yes` or just `Y`.


## Method 2: Using the Git

If you have Git installed on your system, you can download this repository using the command line:

- Open the _Terminal_ in R Studio (In RStudio, the terminal is in a tab next to the console.) or the _Command Prompt_ of your OS.
- Navigate to the directory where you want to download the repo using the cd command (e.g., cd ~/Documents).
- Run the following command to clone the repo: 

```{git}
git clone https://github.com/hubchev/temp_exam.git
``` 

## Method 3: Using the Terminal

Use the _Terminal_ (In RStudio, the terminal is in a tab next to the console.) to navigate to the directory where you want to copy the template (e.g., cd path/to/my/folder). Make sure that the directory is empty and run this command:

```{bash}
quarto use template hubchev/temp_exam
```


## Method 4: Using the mouse

### Method 4a: Click in GitHub

In GitHub click the green `<> Code v` button that you find at this repo. In the context menu that opens, you find a button named `Download ZIP`. Click that and you have the a zipped copy of the repo which you can unzip and use.

### Method 4a: Click this [this link](https://github.com/hubchev/temp_exam/zipball/HEAD)

You can download the repo in zipped file using [this link](https://github.com/hubchev/temp_exam/zipball/HEAD). Now, you can unzip it into a directory of your choice.

# How to Use the Template

Once you've downloaded the repo, navigate to the directory where you downloaded it and open the `exam_template.Rmd` file in RStudio or your preferred R Markdown editor. Customize the template to create your own exam!

To convert the R Markdown file into a formatted document (such as a PDF or HTML), knit the exam_template.Rmd file. You can do this in RStudio by opening the file and clicking the "Knit" button, or by running the following command in the R console:

```{r}
rmarkdown::render("path/to/temp_exam.Rmd")
```

Replace "path/to/exam_template.Rmd" with the actual path to the file.
Contribute

If you have any questions or need help with the template, feel free to open an issue or contact me. Happy exam-writing!
