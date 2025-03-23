# Simulación de Fiabilidad de un Sistema de Propulsión Naval

## Descripción

Este notebook realiza una simulación de la **fiabilidad de distintos sistemas de propulsión de un buque**, compuestos por motores diésel y una turbina. A partir de distribuciones de probabilidad asociadas al fallo de cada componente, se simulan escenarios de funcionamiento para identificar cuál de las vías de propulsión (y sus combinaciones) ofrece mayor confiabilidad a lo largo del tiempo.

## Estructura del Notebook

1. **Definición del sistema:** Se describen las tres vías de propulsión del buque:
   - Motor Diésel 1
   - Motor Diésel 2
   - Turbina
2. **Modelado de componentes:** Se simula la fiabilidad de cada componente individual usando funciones de distribución de probabilidad.
3. **Cálculo de fiabilidad por bloques y sistemas:** Combinación de componentes en serie/paralelo para obtener la fiabilidad global de cada vía.
4. **Comparativa entre sistemas:** Evaluación de qué sistema individual presenta mayor confiabilidad.
5. **Simulación de combinaciones múltiples:** Estudio de la fiabilidad de configuraciones mixtas (ej. Motor 1 + Motor 2, o todos los sistemas a la vez).
6. **Visualización de resultados:** Gráficos detallados de evolución de la fiabilidad en el tiempo.

## Resultados Esperados

El análisis permite identificar la configuración más robusta del sistema de propulsión del buque. Se concluye que la combinación de **todos los sistemas trabajando en paralelo** ofrece la mayor fiabilidad, seguida por aquellas que incluyen el **Motor Diésel 2**, que demuestra ser el más confiable de forma individual.

## Tecnologías utilizadas

- Python
- Jupyter Notebook
- Bibliotecas: `numpy`, `scipy.stats`, `matplotlib`
