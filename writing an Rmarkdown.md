---
title: "MarkyMark"
author: "Cathy Do"
date: "2026-09-24"
output:
  html_document: default
  pdf_document: default
  word_document: default
---

```{r setup, include=FALSE}
knitr::opts_chunk$set(echo = TRUE)
```

# Headings
You can make levels of headings in Rmarkdown documents using hash

# One hash for big headings
## Two hash for smaller headings
### Three hash for even smaller headings
#### and so on and so on ....


# Bold and italics
You can also make things bold and italic using asteriks on either side of the text. Use two asteriks for bold and 1 asterik for italic.

**I want this to be bold**

*I want this to be italic*

# Bullet points

You can make bullet points with dashes

- bullet 1
- bullet 2
- bullet 3

Don't forget to put a space after the dash to get bullets.

# Quotes

Get quotes using a >

> "There is no such thing as a silly question - Jen Richmond, R-Ladies Sydney"

# Links

You can insert links with a combination of square and round brackets. Put the text in square brackets and the url in round brackets.

You can find references at my github, [cathybiocodes](https://github.com/cathybiocodes).

# Pictures/gifs/tweets

It is pretty easy to embed all kinds of things in Rmarkdown documents.

### Pictures

Use a "! [] (nameofimage.png)" without the spaces in between 

### Tweets

Use the embed code from X to insert tweets

### Gifs

Use the embed code 

<iframe src="https://giphy.com/embed/c09yiyePL8zo25DqPf" width="480" height="480" style="" frameBorder="0" class="giphy-embed" allowFullScreen></iframe><p><a href="https://giphy.com/gifs/frog-capybara-capybaras-c09yiyePL8zo25DqPf">via GIPHY</a></p>


# Embedding code in chunks

We can intersperse notes and code "chunks" by using the green insert drop down in R or the hot keys alt-control-I. Run the code in each chunk using the green arrow or hotkey ctrl-shift-enter.

#load packages
```{r message=FALSE, warning=FALSE}
library(tidyverse)
library(readr)
library(here)
```

#read in the beaches data
```{r message=FALSE, warning=FALSE}
beaches <- read_csv(here("data","sydneybeaches.csv"))
```

#plot mean bug levels by site
```{r message=FALSE, warning=FALSE}
beaches %>%
  group_by(Site) %>%
  summarise(meanbugs = mean('Enterococci (cfu/100ml)', na.rm =TRUE)) %>%
  ggplot(aes(x = Site, y = meanbugs)) +
  geom_col() +
  coord_flip()
```



# Export formats

The default format is html, you can also export to pdf or word using the dropdown.

#to be used when exporting to pdf, since pdf is more finnicky.
```{r}
install.package("tinytex")
library(tinytex)
```





