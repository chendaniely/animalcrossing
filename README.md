# animalcrossing

R package for animal crossing data

See here for the data collection scripts: https://github.com/chendaniely/animal_crossing

## Installation

```r
if (!require("remotes")){install.packages("remotes")}
remotes::install_github("chendaniely/animalcrossing")
```

## Changelog

### 0.0.2

Fixed issues with datasets

- Fixed missing images and values in datasets (discovered by looking at high NA values in villagers dataset)
  - Only the bugs and fish data are scraped with a phantomjs script
  - The other tables are pulled using the html directly from the page

- Crafting dataset has been split into has yearly and seasonal materials datasets

- Created the diy unconfirmed dataset

### 0.0.1

Cleaned up all the datasets:

- column names were all passed through janitor::clean_names
- pull out the `src` from `<img>` tags
- converted and cleaned and price column to be a double (e.g., removed "Bells" and "," from text, etc)
