library(plotly)
library(htmlwidgets)
p_scatter <- plot_ly(X002, x = ~PartLength, y = ~PartResistance, 
                     type = 'scatter', mode = 'markers',
                     marker = list(color = '#0072B2', size = 8, opacity = 0.8)) %>%
  layout(title = list(text = 'Part Length vs Part Resistance (X002)', font = list(size = 18)),
         xaxis = list(title = list(text = 'Part Length', font = list(size = 18)), tickfont = list(size = 14)),
         yaxis = list(title = list(text = 'Part Resistance', font = list(size = 18)), tickfont = list(size = 14)),
         plot_bgcolor = 'white', paper_bgcolor = 'white')
