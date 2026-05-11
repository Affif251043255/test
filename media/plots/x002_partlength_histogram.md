library(plotly)
library(htmlwidgets)
p <- plot_ly(X002, x = ~PartLength, type = 'histogram',
             marker = list(color = '#0072B2', line = list(color = 'white', width = 1)))
p <- p %>%
  layout(title = list(text = 'Distribution of Part Length (X002)', font = list(size = 18)),
         xaxis = list(title = list(text = 'Part Length', font = list(size = 18)), tickfont = list(size = 14)),
         yaxis = list(title = list(text = 'Frequency', font = list(size = 18)), tickfont = list(size = 14)),
         plot_bgcolor = 'white', paper_bgcolor = 'white')
