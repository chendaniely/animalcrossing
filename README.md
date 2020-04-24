# animalcrossing

R package for animal crossing data

See here for the data collection scripts: https://github.com/chendaniely/animal_crossing

## Installation

```r
if (!require("remotes")){install.packages("remotes")}
remotes::install_github("chendaniely/animalcrossing")
```

## Changelog

### 0.0.1

Cleaned up all the datasets:

- column names were all passed through janitor::clean_names
- pull out the `src` from `<img>` tags
- converted and cleaned and price column to be a double (e.g., removed "Bells" and "," from text, etc)
