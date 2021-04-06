-- [Graph in R](#graph-in-r)
  - [Distribution plot](#distribution-plot)

# Graph in R

## Distribution plot

```R
library("ggplot2")
mine.data <- read.delim(file = "SP")
p <- ggplot(mine.data, aes(x = x, group = y)) + geom_density(aes(fill = y), alpha= 0.4)
png("SP.png")
p
dev.off()
```
![alt text](https://github.com/mwbioinfo/tutorial/blob/main/SP.png)
