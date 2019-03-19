---
title: "sanfran"
author: "Hector Medeiros"
date: "18 de março de 2019"
output: html_document
---

```{r setup, echo=FALSE, warning=FALSE, message=FALSE}
library(tidyverse)
library(here)
theme_set(theme_bw())
```

## R Markdown

Este é um trabalho que visa ver o desempenho do San Francisco 49ers na NFL nos ultimos 10 anos

```{r}

SF_games = reg_games_2018 %>% 
    filter(home_team == "SF" | away_team == "SF") 
```


```{r}
vitorias_em_casa = SF_games %>%
  filter(home_team == "SF" & home_score > away_score)



```

