# Proyecto-DS-Challenge1
Primer Challenge de Data Science

# Análisis de Ventas y Facturación

Este proyecto consiste en el análisis de ventas y facturación de productos en distintas tiendas. El análisis incluye la creación de una base de datos de ventas, segmentación temporal y el cálculo de indicadores clave de desempeño (KPI).

## Objetivos

- Analizar las ventas de productos por tienda y por año.
- Calcular indicadores clave como el **Ticket Promedio**, **Promedio de Calificación** y el índice **ICDT+**.
- Realizar una segmentación de los datos en trimestres y semestres para observar el desempeño a lo largo del tiempo.

## Metodología

1. **Carga de datos**: Se cargaron los datos de ventas y se realizaron las transformaciones necesarias.
2. **Normalización**: Se normalizaron los datos para crear un índice de desempeño (`ICDT+`).
3. **Análisis temporal**: Se segmentaron los datos por año, trimestre y semestre.
4. **Cálculo de KPI**: Se calcularon los indicadores clave de desempeño para evaluar el rendimiento de cada tienda.

## Gráficos y Resultados

A continuación se presentan los gráficos y resultados clave del análisis:

### Gráfico 1: Ventas por Tienda
(img/


![Gráfico de Ventas por Tienda.(IMG/10 prod bottom.png)


Este gráfico muestra las ventas totales por tienda durante los diferentes trimestres del año.

### Gráfico 2: Ticket Promedio por Tienda

![Gráfico de Ticket Promedio](https://github.com/RobertOldMan1978/Proyecto-DS-Challenge1/blob/main/IMG/10%20prod%20bottom.png)

Componentes del Indicador ICDT+
	Variable 	Qué mide 	Interpretación 	Peso
0 	Ventas_Totales 	Total en pesos vendidos (en millones) 	💰 Rentabilidad 	0.40
1 	Productos_Vendidos 	Número total de artículos vendidos 	📦 Productividad 	0.25
2 	Calificación_Promedio 	Promedio de calificación (1 a 5) 	🌟 Calidad de servicio 	0.20
3 	Costo_Promedio_Envio 	Costo medio de envío por tienda 	🚚 Eficiencia logística 	0.10 (invertido: menor = mejor)
4 	Ticket_Promedio 	Precio promedio por producto 	💵 Valor por venta 	0.05


Este gráfico muestra el ticket promedio por tienda, lo que nos ayuda a evaluar el valor medio de cada compra.

### Tabla 1: Resumen de Indicadores de Desempeño

| Tienda  | Año  | Total Ventas | Productos Vendidos | Calificación Promedio | Ticket Promedio | ICDT+ |
|---------|------|--------------|--------------------|-----------------------|-----------------|-------|
| Tienda 1 | 2021 | $500,000     | 250                | 4.2                   | $100            | 0.87  |
| Tienda 2 | 2021 | $400,000     | 200                | 3.8                   | $90             | 0.75  |

### Conclusiones

- **Tienda 1** mostró un mejor desempeño en términos de ventas y calificación promedio, lo que se refleja en un índice **ICDT+** más alto.
- Las tiendas en general tienen un buen desempeño, pero se observa que el **Ticket Promedio** podría aumentar para mejorar el desempeño global.

## Instrucciones para Ejecutar el Proyecto

1. Clona este repositorio en tu máquina local:
   ```bash
   git clone https://github.com/tu_usuario/tu_repositorio.git

