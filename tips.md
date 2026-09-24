# Some Tips for Lab (and Project) Work

1. Clearly mark each Question in each Lab. There is no need to repeat the question before answering it, although you are permitted to do so.
2. Be sure you carefully go through the HTML result of your Lab before you submit it to ensure that everything looks OK, and that, for instance, the Table of Contents works properly.
3. Use the templates provided by Dr. Love when you can.
4. Use the [version of R that Dr. Love recommends](https://thomaselove.github.io/431-2026/software.html). 
5. [Update your R packages](https://thomaselove.github.io/431-2026/software.html#updating-your-r-packages).
6. Make sure your YAML has an appropriate title (431 Lab 1 is fine for Lab 1) and author setup, so that this prints nicely in the HTML.
7. Do not source in files (like R scripts) using directories that we don't have. Use a `data` subdirectory of your R Project directory for this Lab, so you can use `source("data/Love-431.R")` rather than `source("D/DirectoryPathNoOneElseHas/data/Love-431.R")`.
8. Do not use `opts_chunk$set` to turn off warnings and messages throughout a Lab document or any other work you submit to us. We need to see those warnings if they exist anywhere, and it is only OK to turn off messages for the R package setup, not the work after that point.
9. **Do** turn the messages off in your package loading chunk with `#| message: FALSE`.
10. Leave a blank line in your Quarto file **before** and **after**:
    - every code chunk
    - every heading
    - every new paragraph of text
11. Hit ENTER after every pipe and + in your code so that you avoid scrollable windows for code in your HTML output.
12. Use the tidyverse to manage data, whenever possible.
13. Hit F7 to use spell-check in RStudio on your Quarto file. It's not perfect, especially with headers, but at least it might help.
14. If you decide to get help from a large language model (like ChatGPT) to help with your phrasing of ideas, or building code, OK, but you need to describe what you did carefully in the designated **AI Usage** section (just before the Session Information) of your submission.
15. Ensure that the Session Information is available as a section in the Table of Contents.

## About Loading R Packages

These are the things I look for in a proper R Setup in your Quarto file.

1. Your Quarto includes `#| message: false` at the start of the code chunk.
2. You include `knitr::opts_chunk$set(comment = NA)` at the start of your code.
3. If you are going to source in a script, like `Love-431.R`, you do it next.
4. You then load packages. I typically start with janitor, patchwork and naniar, assuming I am going to use them.
5. Your last two packages loaded are **easystats** then **tidyverse**.
6. You **do not** load packages that are part of easystats or part of the tidyverse separately - this is an extremely common problem for people who use AI to help them code, and makes it really easy for us to take away some points for not being tidy about what you're doing.
    - The [list of packages contained in easystats is here](https://easystats.github.io/easystats/#getting-started). It includes report, correlation, modelbased, bayestestR, effectsize, see, parameters, performance, insight and datawizard.
    - The list of [core packages loaded by tidyverse is here](https://tidyverse.org/packages/#core-tidyverse). It includes ggplot2, dplyr, tidyr, readr, purrr, tibble, stringr, forcats and lubridate.
7. You set a theme for your ggplots last, with `theme_set(theme_bw())`, or another option. Some I like include `theme_modern()`, `theme_lucid()`, `theme_light()`, as well as some of the options [described here](https://ggplot2-book.org/themes#sec-themes) and elsewhere.


Be sure to again carefully go through the HTML result of your Lab before you submit it to ensure that everything looks OK, and that, for instance, the Table of Contents works properly.
