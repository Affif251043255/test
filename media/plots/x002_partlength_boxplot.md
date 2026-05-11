library(plotly)
library(htmlwidgets)
p_boxplot <- plot_ly(X002, y = ~PartLength, type = 'box', 
                     marker = list(color = '#D55E00')) %>%
  layout(title = list(text = 'Box Plot of Part Length (X002)', font = list(size = 18)),
         yaxis = list(title = list(text = 'Part Length', font = list(size = 18)), tickfont = list(size = 14)),
         plot_bgcolor = 'white', paper_bgcolor = 'white')
