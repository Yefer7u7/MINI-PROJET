# MINI-PROJET
MINI PROJET
# Proyecto de Operaciones Matemáticas Aleatorias

Este proyecto genera operaciones matemáticas aleatorias (como suma, resta, multiplicación, división y potenciación) y guarda los resultados en un archivo CSV. Las operaciones se realizan con operandos generados aleatoriamente, y se aplican condiciones para evitar errores como la división por cero o exponentes muy grandes.

## Estructura del Proyecto

El proyecto contiene los siguientes archivos y carpetas:


### Descripción del Código

1. **Operaciones Matemáticas**: 
   Se definen cinco operaciones: suma (`SUM`), resta (`SUB`), multiplicación (`MUL`), división (`DIV`) y potenciación (`POW`). 
   
   Las operaciones se calculan usando funciones lambda para cada tipo de operación:
   - **Suma (SUM)**: Suma de dos números.
   - **Resta (SUB)**: Resta de dos números.
   - **Multiplicación (MUL)**: Producto de dos números.
   - **División (DIV)**: División de dos números (se maneja el caso de división por cero).
   - **Potenciación (POW)**: Potencia de un número (se limita el exponente a 10 para evitar números muy grandes).

2. **Generación de Datos**:
   - El código genera 1000 operaciones matemáticas aleatorias.
   - Los operandos para cada operación son números enteros aleatorios entre 1 y 1000.
   - El resultado de cada operación se calcula y se guarda junto con los operandos y la operación en un DataFrame de Pandas.

3. **Archivo CSV de Resultados**:
   - Los resultados se guardan en un archivo CSV llamado `math_operations_with_results.csv`.
   - El archivo CSV contiene cuatro columnas:
     - `operation`: El tipo de operación (SUM, SUB, MUL, DIV, POW).
     - `operand_1`: El primer operando.
     - `operand_2`: El segundo operando.
     - `result`: El resultado de la operación.
   
4. **Manejo de Errores**:
   - La división por cero se maneja devolviendo `None`.
   - Los exponentes para la operación de potencia se limitan a 10 para evitar que los resultados sean demasiado grandes.

## Requisitos

Para ejecutar este proyecto, necesitarás tener instalado Python y la librería Pandas. Si aún no tienes Pandas, puedes instalarla usando pip:

```bash
pip install pandas
