library(plotly)
library(htmlwidgets)
agg_X002 <- aggregate(PartLength ~ Machine, data = X002, FUN = mean)
p_barchart <- plot_ly(agg_X002, x = ~Machine, y = ~PartLength, type = 'bar',
                      marker = list(color = '#009E73', line = list(color = 'white', width = 1))) %>%
  layout(title = list(text = 'Average Part Length by Machine (X002)', font = list(size = 18)),
         xaxis = list(title = list(text = 'Machine', font = list(size = 18)), tickfont = list(size = 14), type = 'category'),
         yaxis = list(title = list(text = 'Average Part Length', font = list(size = 18)), tickfont = list(size = 14)),
         plot_bgcolor = 'white', paper_bgcolor = 'white')
