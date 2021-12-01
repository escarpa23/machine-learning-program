# Planificacion

# Sesion

**Duración Estimada:**

- **Sesión:** `90 minutos`
- **Tarea:** `60 minutos`
- **Corrección:** `60 minutos`

## Machine Learning, qué significa?

> Por muy esotérico que suene, ¿qué significa en **español, literal**?

```python
%%HTML
<blockquote class="twitter-tweet"><p lang="es" dir="ltr">Machine Learning, qué significa? 🧵<br><br>- La máquina aprende.<br><br>Qué aprende?<br><br>- Una ecuación matemática. Por ejemplo: <a href="https://t.co/6esK5NNy7l">pic.twitter.com/6esK5NNy7l</a></p>&mdash; Jesús López (@sotastica) <a href="https://twitter.com/sotastica/status/1432738023825940481?ref_src=twsrc%5Etfw">August 31, 2021</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>
```

## Funciones Matemáticas

> ¿Qué representa una ecuación matemática?

## Cargar Datos

> - Simplemente, copiamos y pegamos las siguientes líneas de código para cargar los datos.
> - La tabla contiene **estadísticas sobre Coches** (columnas).
> - Para distintas **Marcas/Modelos de coche** (filas).

```python
import seaborn as sns

df = sns.load_dataset(name='mpg', index_col='name')
df.sample(10)
```

## Seleccionar Variables para el Modelo

> 1. Explicativas/Features/Input `X`
> 2. Objetivo/Class/Target `y`

## Visualizar Selección de Variables

> Las dos variables son numéricas. Por tanto, usaremos un **scatterplot** para visualizar la relación entre ellas.

## Modelo de Regresión Lineal en Python

### Entrenar Modelo

> 1. **Necesidad**: Entrenar Modelo
> 2. **Solución**: Función `fit()`

### Jerarquía de las Librerías

> 1. `Librería`
> 2. `Módulo1.Módulo2.`
> 3. `Función()` / `Objeto()`
>
> - **Si es Objeto**
>   - 3.1 `Función()`

### Ecuación Matemática del Modelo

> Los modelos no son más que ecuaciones matemáticas que nos ayudan a calcular algo. Por ejemplo:
>
> 1. La probabilidad de que un cliente deje de acudir a mi tienda.
> 2. La probabilidad de que un cliente del banco pueda afrontar un préstamo.
> 3. La probabilidad de que un atleta se lesione.
> 4. El número de bicicletas que se alquilarán hoy.
> 
> Por tanto, ¿cuál es la ecuación matemática de **nuestro modelo**?

### Predicciones con el Modelo

> En nuestro caso, ¿cómo usamos la ecuación matemática para **predecir el total de accidentes**?

### Visualización del Modelo

> 1. Los **datos reales**.
> 2. **Modelo: las predicciones** con la ecuación matemática.

### Interpretación del Modelo

> ¿Qué **influencia tiene el alcohol** en el número de accidentes?

## Explicación Algoritmo Regresión Lineal

```python
%%HTML
<blockquote class="twitter-tweet"><p lang="es" dir="ltr">Estoy creando una ODA a la regresión lineal, me encanta como está quedando.<br><br>Sobretodo, la conexión entre matemáticas, derivadas, optimización, estadística y Machine Learning que pongo en valor en menos de 30 segundos. <a href="https://t.co/ZdOqFeFCKI">pic.twitter.com/ZdOqFeFCKI</a></p>&mdash; Jesús López (@sotastica) <a href="https://twitter.com/sotastica/status/1437389800504451080?ref_src=twsrc%5Etfw">September 13, 2021</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>
```

## Cómo se ha Calculado el Modelo con el Código?

> ¿Qué sucede por dentro al ejecutar la función `.fit()`?

## ¿Cómo de Bueno es mi Modelo? **Bondad de Ajuste**

> Tan solo comparamos la predicción con la realidad.

## Otros Modelos de Regresión

### `RandomForestRegression()`

-

### `SVR()`

-

# Tarea

## Cargar Datos

> Si ejecutamos los siguientes comandos:

```python
import seaborn as sns
sns.get_dataset_names()
```

> Veremos una lista de posibles `datasets` que podemos descargar desde internet y convertirlos directamente a un `DataFrame` de `pandas`. Por ejemplo:

```python
sns.load_dataset(name='mpg')
```

## Seleccionar 2 Variables para la Regresión

> - Variable Objetivo `y`
> - Variable Explicativa `X`

## Scatterplot con las Variables

> Deberíamos observar en la gráfica que los puntos podrían relacionarse a través de una línea que los cruce.
>
> Si no es así, debemos seleccionar otras variables.

## Modelo de Regresión Lineal `LinearRegression()`

### Entrenar Modelo

> 1. **Necesidad:** Entrenar Modelo
> 2. **Solución: Función** `fit()`

### Realizar Predicciones

> - `model.predict()`

## Visualizar Modelo

> 1. Los **datos reales**.
> 2. **Modelo: las predicciones** con la ecuación matemática.

## Interpretar Modelo

> 1. Especifica la **Fórmula Matemática** del Modelo.
> 2. **Interpreta los Coeficientes** de la Ecuación Matemática.

## Realidad vs Predicciones

> ¿Cómo de bueno es nuestro modelo?
>
> 1. Si pasamos las predicciones como una nuevo columna del `DataFrame`, podremos observar que **las predicciones de nuestro modelo pueden no coincidir con la realidad**.
>
>    - `df['pred'] = predicciones`
>
> 2. ¿Cómo medimos el **error de nuestro modelo**? ¿Cómo de bueno es nuestro modelo para describir la realidad?
>    - `df.sample(10)` para comprobar si las predicciones de nuestro modelo coinciden con la realidad...

## Objetivos Alcanzados

_Haz doble click sobre esta celda y pon una `X` dentro de las casillas [X] si crees que has superado los objetivos:_

- [ ] Entender **cómo la máquina optimiza un modelo**, que no es más que encontrar **los números** una ecuación matemática.
- [ ] La `función` como elemento indivisible de la programación. Como un **átomo**: el núcleo de todo.
- [ ] Entender **qué sucede dentro del ordenador** cuando ejecutamos una función. Descargamos código de internet, o es un proceso local del ordenador?
- [ ] Usar **la programación como una herramienta**, como un medio hacia un fin. No como el fin en sí mismo.
- [ ] Entender que la estadística no es una ciencia perfecta. Sino que trata de **aproximarse a la realidad** de la mejor forma posible.
- [ ] **Medir el error** del modelo no es más que comparar la predicción contra la realidad.
- [ ] De la misma manera que en el código existen diversas formas de obtener el mismo resultado, en la programación existen **diversos algoritmos/modelos/ecuaciones para predecir la misma variable**.-