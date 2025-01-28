
# **Dashboard: Análisis de Manufactura - Industria Textil**

Este dashboard tiene como objetivo mostrar un análisis detallado de la industria textil mediante un conjunto de datos ficticios. Utilizando Power BI y conectando directamente con una base de datos MySQL, este reporte permite explorar y visualizar diferentes aspectos de la manufactura, ventas, stock, tiempos de entrega y calidad de insumos por proveedor. El análisis es fundamental para la toma de decisiones en la cadena de suministro y la optimización de la operación en la industria textil.

## **Conexión de Datos:**
- La base de datos está conectada a **Power BI** mediante **DirectQuery** con un origen de datos en **MySQL**, lo que permite que los datos se actualicen automáticamente cada vez que haya cambios en la base de datos.
- **ETL**: Se realizó la ingesta de datos a través de procesos de **extracción, transformación y carga (ETL)** utilizando herramientas de Power BI.

---

## **Gráfico 1: Reporte de Ventas por Fecha**
**Tipo de gráfico:** Gráfico de línea con línea de tendencia.  
**Descripción:** Este gráfico muestra la evolución de las ventas desde el 10 de enero hasta el 24 de enero del presente año. Se puede observar que las ventas comenzaron a subir desde el 10 de enero hasta el 13 de enero, luego sufrieron una caída a partir del 15 de enero. Sin embargo, las ventas se recuperaron el 16 de enero, pero volvieron a descender hasta el 24 de enero.  
**Insight:** La línea de tendencia indica que la mayoría de los datos están por encima de la línea de tendencia, lo que sugiere que en general las ventas fueron mayores de lo esperado. Las caídas pueden estar relacionadas con factores como **problemas en el suministro** o **fluctuaciones en la demanda**.

---

## **Gráfico 2: Top de Productos Más Vendidos**
**Tipo de gráfico:** Gráfico de barras apiladas.  
**Descripción:** En este gráfico se visualizan los productos más vendidos, destacando al **Jean Stretch** como el más vendido con 25 unidades. Otros productos como la **Camiseta de algodón**, **Pantalón Denim** y **Zapatos de cuero** siguen con 20 unidades cada uno, mientras que la **Chaqueta Invierno** fue el producto menos vendido con solo 3 unidades.  
**Insight:** La visualización revela que ciertos productos tienen una mayor rotación, lo que puede ser importante para **gestionar el stock** y enfocar esfuerzos de marketing en los productos más populares. El bajo desempeño de la **Chaqueta Invierno** podría indicar una baja demanda en ciertas temporadas.

---

## **Gráfico 3: Control de Stock por Producto**
**Tipo de gráfico:** Gráfico de tabla.  
**Descripción:** Esta tabla muestra el stock de cada producto con una columna adicional que clasifica el stock como **bajo**, **normal** o **alto**. Los productos con menos de 10 unidades tienen el estado **bajo**, indicando que deben ser reabastecidos pronto.  
**Insight:** Este gráfico es útil para mantener un control en tiempo real sobre los niveles de inventario y gestionar el riesgo de **agotamiento de stock**. Alertas tempranas pueden ser configuradas para prevenir desabastecimientos.

---

## **Gráfico 4: Calidad de Insumos por Proveedor (3MAP)**
**Tipo de gráfico:** Gráfico 3MAP (Mapa tridimensional).  
**Descripción:** Este gráfico clasifica a los proveedores según la calidad de los insumos, categorizados en **alta**, **media** y **baja**. Se usa un sistema de colores: verde para calidad alta, amarillo para calidad media y rojo para calidad baja.  
**Insight:** Este gráfico permite identificar qué proveedores ofrecen los insumos de mejor calidad y cuáles necesitan atención. Un proveedor con **baja calidad** podría estar afectando el rendimiento de la producción, y una **mejora en la calidad** de insumos podría ser una estrategia para optimizar la manufactura.

---

## **Gráfico 5: Tiempo de Entrega por Proveedor**
**Tipo de gráfico:** Gráfico de barras apiladas.  
**Descripción:** Este gráfico muestra los tiempos de entrega por proveedor, donde **Industrias de Algodón** tiene el tiempo de entrega más largo con 21 días, mientras que otros proveedores como **Fábricas Mundo** tienen un tiempo de entrega de 14 días. Los tiempos de entrega se categorizan en **rápido**, **medio** y **lento** según el número de días.  
**Insight:** Los proveedores con tiempos de entrega largos, como **Industrias de Algodón**, podrían estar afectando la **eficiencia operativa**. Esto podría influir en las decisiones de **selección de proveedores** para mejorar la **eficiencia logística**.

---

## **Filtros y Relaciones entre Gráficos**
Durante el análisis, se utilizaron filtros para explorar diferentes dimensiones de los datos, tales como la **calidad de insumos** y los **proveedores**. A través de estas segmentaciones, se pudo detectar patrones significativos:

1. **Relación entre calidad de insumos y tiempos de entrega**: Proveedores con baja calidad de insumos, como **Industrias de Algodón**, tienen tiempos de entrega más largos, lo que podría estar relacionado con problemas en la **gestión de la cadena de suministro**.
2. **Relación entre productos y proveedores**: Aunque el **top de productos vendidos** está claro, aún falta una relación más detallada entre los **productos** y sus respectivos **proveedores**. Esto permitirá identificar qué proveedor suministra cada producto y ajustar las decisiones de compras basadas en la calidad y los tiempos de entrega.

---

## **Conclusiones y Recomendaciones**
- **Optimización de Proveedores:** Basado en los tiempos de entrega y la calidad de los insumos, se recomienda revisar a los proveedores que ofrecen insumos de baja calidad o aquellos que tardan mucho en entregar.
- **Gestión de Inventarios:** Los productos con stock bajo deben ser priorizados para evitar desabastecimientos. Implementar alertas para los productos con **bajo stock** es clave.
- **Ajuste en Producción:** Considerar el desempeño de los productos en función de la venta y la calidad de los insumos para tomar decisiones sobre **ajustes de producción** o promoción de ciertos productos.

---

### **Tecnologías Utilizadas**
- **Power BI**: Para la visualización de datos.
- **MySQL**: Como base de datos para la conexión de los datos.
- **DirectQuery**: Para obtener los datos en tiempo real y permitir su actualización automática.

---

