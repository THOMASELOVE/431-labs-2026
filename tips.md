# Some Tips for Lab (and Project) Work

1. Clearly mark each Question in each Lab. There is no need to repeat the question before answering it, although you are permitted to do so.
2. Be sure you carefully go through the HTML result of your Lab before you submit it to ensure that everything looks OK, and that, for instance, the Table of Contents works properly.
3. Use the templates provided by Dr. Love when you can.
4. Use the [version of R that Dr. Love recommends](https://thomaselove.github.io/431-2026/software.html). 
5. [Update your R packages](https://thomaselove.github.io/431-2026/software.html#updating-your-r-packages).
6. Make sure your YAML has an appropriate title (431 Lab 1 is fine for Lab 1) and author setup, so that this prints nicely in the HTML.
7. Do not load in individual packages from the tidyverse that are in the core tidyverse (auto-loaded when you load the tidyverse). The list of core packages is [available here](https://www.tidyverse.org/packages/#core-tidyverse). It includes dplyr, ggplot2, forcats and several others.
8. Do not load in R packages that you do not wind up using.
9. Do not source in files (like R scripts) using directories that we don't have. Use a `data` subdirectory of your R Project directory for this Lab, so you can use `source("data/Love-431.R")` rather than `source("D/DirectoryPathNoOneElseHas/data/Love-431.R")`.
10. Do not use `opts_chunk$set` to turn off warnings and messages throughout a Lab document or any other work you submit to us. We need to see those warnings if they exist anywhere, and it is only OK to turn off messages for the R package setup, not the work after that point.
11. **Do** turn the messages off in your package loading chunk with `#| message: FALSE`.
12. Leave a blank line in your Quarto file **before** and **after**:
    - every code chunk
    - every heading
    - every new paragraph of text
13. Hit ENTER after every pipe and + in your code so that you avoid scrollable windows for code in your HTML output.
14. Use the tidyverse to manage data, whenever possible.
15. Hit F7 to use spell-check in RStudio on your Quarto file. It's not perfect, especially with headers, but at least it might help.
16. If you decide to get help from a large language model (like ChatGPT) to help with your phrasing of ideas, or building code, OK, but you need to describe what you did carefully in the designated **AI Help** section (just before the Session Information) of your submission.
17. Ensure that the Session Information is available as a section in the Table of Contents.

Be sure to again carefully go through the HTML result of your Lab before you submit it to ensure that everything looks OK, and that, for instance, the Table of Contents works properly.
