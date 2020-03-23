# swirl

This packages adds more functionalities to swirl. swirl is a platform for learning (and teaching) statistics and R simultaneously and interactively. It presents a choice of course lessons and interactively tutors a user through them. A user may be asked to watch a video, to answer a multiple-choice or fill-in-the-blanks question, or to enter a command in the R console precisely as if he or she were using R in practice. Emphasis is on the last, interacting with the R console. User responses are tested for correctness and hints are given if appropriate. Progress is automatically saved so that a user may quit at any time and later resume without losing work.

swirl leans heavily on exercising a student's use of the R console. A callback mechanism, suggested and first demonstrated for the purpose by Hadley Wickham, is used to capture student input and to provide immediate feedback relevant to the course material at hand.

[swirlify](https://github.com/swirldev/swirlify) is a separate R package that provides a comprehensive toolbox for swirl instructors. Content is authored in [YAML](http://en.wikipedia.org/wiki/YAML) using the handy tools described on the [instructors page](http://swirlstats.com/instructors.html) of our website.

The program is initiated with `swirl()`. Functions which control swirl's behavior include `bye()` to quit, `main()` to return to the main menu, `play()` to allow experimentation in the R console without interference from swirl, `nxt()` to resume interacting with swirl, and `info()` to display a help menu.


## Installing this package

To access the most recent features and content, you can install and run the development version of swirl using the [devtools](https://github.com/hadley/devtools) package:

```
install.packages("devtools")
devtools::install_github("ahdvnd/swirlplus")
library(swirl)
swirl()
```

