library(httr)
library(jsonlite)
library(plotly)

Datos = fromJSON("Nomina-Nivel-Central-2017-2021.json")

Datos <- data.frame(Datos)
colnames(Datos)<- c("Nombre","Departamento","Sueldo","Mes","Año")

p = plot_ly(Datos, x = ~Nombre,y = ~Sueldo,
            name = 'Nombre',
            type = 'scatter',
            mode = 'lines+markers')

p %>% layout(title="Sueldo de cada empleado")


p1 = plot_ly(Datos, x = ~Año,y = ~Departamento,
            name = 'Departamento',
            type = 'scatter',
            mode = 'lines+markers')

p1 %>% layout(title="Departamento Por Año")