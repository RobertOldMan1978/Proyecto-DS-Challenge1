# Proyecto-DS-Challenge1
## Primer Challenge de Data Science

El propósito del presente análisis es ayudar a Don Juan a decidir cuál de sus cuatro tiendas debería vender para invertir en un nuevo negocio.

Para ello, se realizará un análisis basado en cinco aspectos clave:

- Facturación total de cada tienda: Determinar cuál tienda tiene las mayores ventas.
- Categorías más populares: Identificar qué productos se venden más en cada tienda.
- Promedio de evaluación de clientes: Evaluar la satisfacción de los clientes en cada tienda.
- Productos más y menos vendidos: Analizar cuáles son los productos que tienen mejor y peor desempeño en ventas.
- Costo promedio de envío: Calcular el costo de enviar productos desde cada tienda hasta los clientes.

## La estructura del proyecto y organización de los archivos.

- Se importaron las bases de datos y se juntaron en un solo dataframe
- Se agregaron mas campos, principalmente de fechas para poder trabajar de manera optima los informes


## Análisis Totales

Este proyecto consiste en el análisis de ventas, facturación, categorias y productos, costos de despacho e indicadores de satisfaccion de clientes. El análisis incluye la creación de una base de datos de ventas, segmentación temporal y el cálculo de indicadores clave de desempeño (KPI).

## Objetivos

- Analizar las ventas de productos por tienda y por año.
- Calcular indicadores clave como el **Ticket Promedio**, **Promedio de Calificación** y el índice **ICDT+**.
- Realizar una segmentación de los datos en trimestres y semestres para observar el desempeño a lo largo del tiempo.

## Metodología

1. **Carga de datos**: Se cargaron los datos de ventas y se realizaron las transformaciones necesarias.
2. **Normalización**: Se normalizaron los datos para crear un índice de desempeño (`ICDT+`).
3. **Análisis temporal**: Se segmentaron los datos por año, trimestre y semestre.
4. **Cálculo de KPI**: Se calcularon los indicadores clave de desempeño para evaluar el rendimiento de cada tienda.


# 📊 Informe Análisis de Ventas - ICDT+

Este informe evalúa el desempeño de las tiendas mediante un índice compuesto (ICDT+) que considera:
- Ventas en millones 💰
Se analiza desde 2020, con foco especial en el desempeño desde 2022.


## 🗓️ Ventas Anuales por Tienda (en millones COP)

| Tienda   |   2020 |   2021 |   2022 |   2023 |   Total General |
|:---------|-------:|-------:|-------:|-------:|----------------:|
| Tienda_1 | 368.93 | 362.12 | 316.57 | 103.26 |         1150.88 |
| Tienda_2 | 320.47 | 351.22 | 358.23 |  86.43 |         1116.34 |
| Tienda_3 | 321.71 | 362.95 | 350.44 |  62.92 |         1098.02 |
| Tienda_4 | 330.85 | 347.82 | 302.22 |  57.48 |         1038.38 |

## 🗓️ Ventas Trimestrales por Tienda (en millones COP)

| Trimestre  | 2023 T1 | 2022 T4 | 2022 T3 | 2022 T2 | 2022 T1 | 2021 T4 | 2021 T3 | 2021 T2 | 2021 T1 | 2020 T4 | 2020 T3 | 2020 T2 | 2020 T1 |
|------------|---------|---------|---------|---------|---------|---------|---------|---------|---------|---------|---------|---------|---------|
| **Tienda_1** | $103,26M | $72,54M | $92,16M | $72,47M | $79,40M | $77,03M | $116,32M | $81,25M | $87,52M | $69,23M | $96,46M | $98,55M | $104,70M |
| **Tienda_2** | $86,43M | $91,89M | $85,61M | $93,09M | $87,64M | $89,87M | $96,57M  | $83,67M | $81,10M | $84,12M | $78,15M | $79,17M | $79,03M  |
| **Tienda_3** | $62,92M | $87,59M | $87,88M | $85,69M | $89,28M | $133,05M| $75,57M  | $83,44M | $70,89M | $75,24M | $86,15M | $78,93M | $81,38M  |
| **Tienda_4** | $57,48M | $67,34M | $72,66M | $64,33M | $97,89M | $85,66M | $92,20M  | $77,48M | $92,48M | $75,47M | $86,33M | $98,34M | $70,71M  |

Tanto en el analisis acumulado como en detalle el orden de ingresos son Tienda_1 a Tienda_4 Descendente

### Gráfico de Venta Mensual y media de tres meses

![Gráfico de Venta Mensual y media de tres meses](https://github.com/RobertOldMan1978/Proyecto-DS-Challenge1/blob/main/IMG/vta_mens_xtienda%20movil.png)

### Gráfico de Venta Mensual y media de tres meses, tienda por tienda

![Gráfico de Venta Mensual y media de tres meses](https://github.com/RobertOldMan1978/Proyecto-DS-Challenge1/blob/main/IMG/vta_mens_xtienda_barras.png)



# Análisis de Venta por Categoría 📦

### 📊 Ventas Totales por Categoría (2020–2023)

Las cifras están expresadas en millones de pesos colombianos (COP).

| Categoría del Producto     | 2020     | 2021     | 2022     | 2023     |
|----------------------------|----------|----------|----------|----------|
| **Electrónicos**           | $496,08M | $559,41M | $486,30M | $118,78M |
| **Electrodomésticos**      | $423,74M | $435,33M | $386,63M | $79,05M  |
| **Muebles**                | $231,40M | $227,57M | $235,76M | $62,93M  |
| **Instrumentos musicales** | $93,45M  | $111,72M | $119,38M | $24,22M  |
| **Deportes y diversión**   | $45,83M  | $39,16M  | $45,91M  | $12,07M  |
| **Juguetes**               | $21,95M  | $21,98M  | $24,18M  | $5,49M   |
| **Artículos para el hogar**| $17,85M  | $17,13M  | $18,40M  | $4,21M   |
| **Libros**                 | $11,65M  | $11,81M  | $10,90M  | $3,34M   |


![Gráfico de Venta Mensual y media de tres meses](https://github.com/RobertOldMan1978/Proyecto-DS-Challenge1/blob/main/IMG/Partic_xCat_xTda)















- Calificación del cliente 🌟
- Costo promedio de envío 🚚
- Ticket promedio 💵


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
Instrucciones para ejecutar el notebook

## Instrucciones para Ejecutar el Proyecto

1. Clona este repositorio en tu máquina local:
   ```bash
   git clone https://github.com/tu_usuario/tu_repositorio.git

