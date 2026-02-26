# 1.1 Historia y Evolución de la Graficación por Computadora

La graficación por computadora es una disciplina de la informática que se encarga de la creación, manipulación y representación de imágenes digitales mediante algoritmos matemáticos y procesos computacionales. Su evolución ha estado estrechamente ligada al desarrollo del hardware y del software.

## Orígenes (Década de 1950)

En los años cincuenta, las computadoras comenzaron a utilizar tubos de rayos catódicos (CRT) para representar información visual básica. Estos sistemas eran capaces de dibujar líneas simples mediante el control de haces electrónicos. Los gráficos eran vectoriales y muy limitados en complejidad.

## Sketchpad y la Interacción Gráfica (1963)

Un hito fundamental fue el desarrollo de Sketchpad por Ivan Sutherland en el MIT. Este sistema permitió la interacción directa con objetos gráficos mediante un lápiz óptico. Introdujo conceptos como:

- Representación jerárquica de objetos.
- Restricciones geométricas.
- Interacción hombre-máquina.

Sketchpad es considerado el precursor del diseño asistido por computadora (CAD).

## Avances en los años 70 y 80

Durante este periodo se desarrollaron algoritmos fundamentales como:

- Algoritmo de Bresenham para trazado de líneas.
- Algoritmos de rasterización.
- Modelos de sombreado (Gouraud y Phong).
- Técnicas de eliminación de superficies ocultas.

También comenzaron las primeras películas con gráficos generados por computadora y simuladores de vuelo.

## Era de las GPU (Década de 1990)

Con la aparición de las Unidades de Procesamiento Gráfico (GPU), el procesamiento de gráficos se volvió más eficiente. Esto permitió:

- Videojuegos 3D en tiempo real.
- Renderizado acelerado por hardware.
- Texturización avanzada.
- Modelado tridimensional complejo.

## Actualidad

Hoy en día la graficación incluye:

- Ray Tracing en tiempo real.
- Inteligencia artificial aplicada a renderizado.
- Realidad virtual (VR) y realidad aumentada (AR).
- Simulación física avanzada.
- Motores gráficos como Unreal Engine y Unity.

La evolución continúa impulsada por la necesidad de mayor realismo y eficiencia computacional.

![Magnavox Odyssey_thumb](https://github.com/user-attachments/assets/7eef34f5-0518-4d78-94f2-060c50e316e1)


# 1.2 Áreas de Aplicación

La graficación por computadora se aplica en diversos campos:

## Videojuegos
Creación de entornos 3D, personajes y efectos visuales.

![download](https://github.com/user-attachments/assets/fdba0e78-2d93-4a38-a3b9-59cb3824c66b)


## Cine y Animación
Producción de efectos especiales (CGI).

![download](https://github.com/user-attachments/assets/6fb67ed6-f450-416c-9721-bf6575c626ef)


## Diseño Asistido por Computadora (CAD)
Utilizado en arquitectura e ingeniería.

<img width="512" height="320" alt="unnamed" src="https://github.com/user-attachments/assets/23871ddb-e710-4d85-a17c-f7bd9d8b5882" />


## Medicina
Visualización de tomografías y modelos anatómicos 3D.

![images](https://github.com/user-attachments/assets/3ffb6b9c-eaf3-4b18-8c36-f6c6494c6394)


## Realidad Virtual y Aumentada
Aplicaciones educativas y de entretenimiento.

![download](https://github.com/user-attachments/assets/600fb97f-012f-44ca-a277-adc9ed38cf3d)


# 1.3 Aspectos Matemáticos de la Graficación

Las matemáticas son el fundamento principal de la graficación por computadora.

## Sistemas de Coordenadas

Se utilizan sistemas cartesianos bidimensionales (x,y) y tridimensionales (x,y,z). Cada objeto se representa mediante un conjunto de vértices definidos por coordenadas.

## Vectores

Un vector representa dirección y magnitud. En gráficos 3D se utilizan vectores para:

- Representar posiciones.
- Calcular iluminación.
- Determinar normales de superficies.

## Matrices de Transformación

Las transformaciones geométricas se realizan mediante multiplicación de matrices:

### Traslación

| 1 0 Tx |
| 0 1 Ty |
| 0 0 1  |

### Rotación (2D)

| cosθ -sinθ 0 |
| sinθ cosθ  0 |
| 0     0    1 |

### Escalamiento

| Sx 0  0 |
| 0  Sy 0 |
| 0  0  1 |

## Producto Punto y Producto Cruz

El producto punto se usa para calcular ángulos entre vectores y determinar iluminación.

El producto cruz permite calcular vectores normales en superficies 3D.

## Curvas y Superficies

Se utilizan ecuaciones paramétricas para representar:

- Curvas Bézier
- Superficies NURBS
- Splines

Estos elementos permiten generar formas suaves y complejas.

| 1 0 Tx |
| 0 1 Ty |
| 0 0 1  |

También intervienen conceptos de trigonometría para calcular ángulos y orientación en espacios tridimensionales, así como cálculo diferencial para modelar curvas y superficies suaves.

![download](https://github.com/user-attachments/assets/db50d23a-36db-433a-a166-e398c4cdeccf)



# 1.4 Modelos de Color: RGB, CMY, HSV y HSL

Los modelos de color permiten representar matemáticamente la percepción del color.

## Modelo RGB

Modelo aditivo basado en la mezcla de luz roja, verde y azul. Es utilizado en pantallas y dispositivos electrónicos.

Cada color se representa con valores entre 0 y 255.

Ejemplo:
Rojo puro = (255,0,0)

## Modelo CMY

Modelo sustractivo usado en impresión. Se basa en la absorción de luz.

Cian absorbe rojo.
Magenta absorbe verde.
Amarillo absorbe azul.

## Modelo HSV

Representa el color de forma más intuitiva:

- Hue: Ángulo en la rueda de color (0°–360°).
- Saturation: Intensidad.
- Value: Brillo.

## Modelo HSL

Similar al HSV, pero utiliza luminosidad en lugar de valor.

---

## Iluminación en Blender

La iluminación en Blender se basa en:

- Tipo de luz (Point, Sun, Spot).
- Intensidad.
- Sombras.
- Materiales PBR.

Se pueden modificar parámetros como rugosidad, especularidad y reflexión para obtener mayor realismo.

![maxresdefault](https://github.com/user-attachments/assets/a2f2e730-76f5-4518-a14f-e4bd499ced84)


# 1.5. Representación y trazo de líneas y polígonos
Este tema explica cómo la computadora "une los puntos". Los archivos muestran dos formas de representar geometría:

### A. Primitivas Geométricas (Flor de vida.py)
Blender ya tiene funciones predefinidas para crear formas básicas.

* Uso de primitive_circle_add: Es una función de alto nivel que genera automáticamente los vértices y aristas de un círculo.

* Resolución: El parámetro vertices=64 define qué tan "suave" se ve el polígono que imita al círculo.

### B. Representación de Datos de Malla (Poligono2d.py)
Este script es mucho más técnico y cercano a cómo funcionan los motores de renderizado internamente:

* Vértices (Vertices): La lista de puntos en el espacio.

* Aristas (Edges): La conexión lógica entre índices de vértices. En el código: aristas.append((i, (i + 1) % lados)).

  * Nota Pro: El uso de % lados (módulo) es un truco de programación para cerrar el polígono, uniendo el último vértice con el primero.

* Estructura de Datos: Se usa malla.from_pydata(vertices, aristas, []), que es la forma fundamental de construir objetos geométricos desde cero en sistemas computacionales.
<img width="682" height="538" alt="image" src="https://github.com/user-attachments/assets/687d72e4-9746-4680-882b-7a14ae1bb038" />
<img width="862" height="566" alt="image" src="https://github.com/user-attachments/assets/0f9b2bc9-483a-4e40-8c95-c40cbc5962b5" />


## 1.6 Formatos de Imagen

Aunque los scripts están enfocados en trabajar con geometría basada en vectores, el último paso dentro del proceso de graficación es el **rasterizado**, que consiste en transformar esos vectores en píxeles para generar una imagen final.

### Vectores vs. Mapas de Bits

Los archivos `.py` generan gráficos vectoriales. Esto significa que dentro de Blender puedes hacer zoom sin que la imagen pierda calidad o se pixele.

Sin embargo, cuando el proyecto se renderiza a un formato como `.PNG`, el resultado se convierte en un mapa de bits (bitmap), es decir, una imagen formada por píxeles.

### Espacio de Color

Blender trabaja por defecto con el modelo de color **RGB** (Red, Green, Blue).

Si se desea modificar un color mediante código, es necesario asignar valores normalizados a cada canal de color, dentro de un rango de:

0.0 a 1.0

Por ejemplo:

```python
color = (1.0, 0.0, 0.0)  # Rojo puro en RGB normalizado
```

Tabla comparativa
| Concepto    | Flor_de_vida.py                            | Poligono2d.py                                |
| ----------- | ------------------------------------------ | -------------------------------------------- |
| Lógica      | Utiliza un bucle `while` basado en ángulos | Utiliza un bucle `for` según número de lados |
| Abstracción | Alta (usa funciones propias de Blender)    | Baja (define vértices manualmente)           |
| Propósito   | Generar patrones geométricos complejos     | Crear estructuras básicas de polígonos       |

### Recomendación Técnica

En el script Flor_de_vida.py, es importante verificar que el valor del paso_angular sea un divisor exacto de 360°.

Esto garantiza que la figura cierre correctamente sin dejar espacios abiertos.

Por ejemplo, usar 60 grados permite obtener una simetría hexagonal perfecta, ya que:

360 / 60 = 6

### Parámetros de la Figura
```python
# Parámetros principales
radio = 3
angulo_actual = 0
paso_angular = 60
```
