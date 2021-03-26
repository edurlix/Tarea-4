library(httr)
library(jsonlite)
library(plotly)


Datos = fromJSON("Tabla1/asesorias-legales-a-turistas-cestur-2020-3.json")

Datos <- data.frame(Datos)
colnames(Datos)<- c("Tipo_de_asesoria", "Cantidad", "Mes", "Año")

p = plot_ly(Datos, x = ~Mes,y = ~Cantidad,
            name = 'Mes',
            type = 'scatter',
            mode = 'lines+markers')

p %>% layout(title="Cantidad de Asesoria turistica al mes")

p1 = plot_ly(Datos, x = ~Tipo_de_asesoria,y = ~Cantidad,
            name = 'Tipo_de_asesoria',
            type = 'scatter',
            mode = 'lines+markers')

p1 %>% layout(title="Cantidad de asesoria por asesoria")