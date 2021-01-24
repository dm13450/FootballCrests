# FootballCrests

A csv file that contains a mapping between team name and their crest from Wikipedia.

## ggplot2

Scatter points can replaced with images using the `ggimage` package
and `geom_image`.

```r
ggplot(modelSummary, 
  aes(x=PreMatchSpread, y=PostMatchSpread, label=Team)) + 
  geom_vline(xintercept = 0) + 
  geom_hline(yintercept = 0) +
  xlab("Pre Match Spread") + 
  ylab("Post Match Spread") +
  geom_image(aes(image=URL))
```
