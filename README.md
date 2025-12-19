# Métodos numéricos en R: Implementación de algoritmos fundamentales 🧮📊

## 📖 Descripción
Este repositorio implementa ocho métodos numéricos esenciales en R Markdown. El proyecto abarca dos áreas principales del cálculo numérico: **integración aproximada** y **búsqueda de raíces de ecuaciones**. Cada método está implementado de forma modular con ejemplos prácticos, visualizaciones y análisis de error. Ideal para estudiantes y profesionales que deseen comprender y aplicar estos algoritmos fundamentales.

---

## 🚀 Ejecución rápida

### Prerrequisitos
```r
# Instalar paquetes necesarios
install.packages(c("ggplot2", "dplyr", "knitr", "rmarkdown"))
```

### Archivos principales
- **`MetodosParaCalcularRaicesDeFunciones.Rmd`** - Documento principal que contiene todos los métodos implementados
- **`Metodos_Numericos_para_Aproximacion_e_Integracion.R`** - Funciones auxiliares y de utilidad (si aplica)

### Ejecutar en RStudio
1. Clonar el repositorio
2. Abrir el archivo en RStudio
3. Hacer clic en "Knit" para generar el informe HTML/PDF

### Visualización rápida de los códigos:

---

## ⚙️ Métodos Implementados

### 📈 Métodos de Integración Numérica
| Método | Breve Descripción | Precisión | Uso Típico |
|--------|-------------------|-----------|------------|
| **Interpolador de Lagrange** | Aproxima funciones mediante polinomios que pasan por puntos dados | Exacto en puntos dados | Interpolación de datos experimentales |
| **Regla del Trapecio Compuesta** | Aproxima integrales sumando áreas de trapecios | O(h²) | Integrales de funciones suaves |
| **Regla del Punto Medio de Riemann** | Usa rectángulos con altura en el punto medio | O(h²) | Alternativa simple al trapecio |
| **Método de Simpson** | Usa arcos parabólicos para mayor precisión | O(h⁴) | Alta precisión con funciones suaves |

### 🔍 Métodos de Búsqueda de Raíces
| Método | Breve Descripción | Convergencia | Requisitos |
|--------|-------------------|--------------|------------|
| **Método de la Bisección** | Divide intervalos sucesivamente | Lineal | Cambio de signo en [a,b] |
| **Método de la Secante** | Aproxima con líneas secantes | Superlineal (1.618) | Dos puntos iniciales |
| **Método de Newton-Raphson** | Usa derivadas para convergencia rápida | Cuadrática | Derivada conocida |
| **Método de Horner** | Evalúa polinomios eficientemente | - | Forma polinómica |

---

## 📊 Resultados Destacados

El análisis comparativo de los métodos implementados revela las siguientes conclusiones fundamentales:

### Para Integración Numérica
- **Simpson vs. Trapecio**: El método de Simpson proporciona significativamente mayor precisión con el mismo número de subdivisiones, especialmente para funciones suaves y polinómicas.
- **Costo-Computación vs. Precisión**: La regla del trapecio compuesta ofrece un equilibrio óptimo entre simplicidad y precisión para muchas aplicaciones prácticas.
- **Error por Subdivisión**: Todos los métodos muestran reducción de error al aumentar el número de subintervalos, pero con tasas distintas (O(h²) vs O(h⁴)).

### Para Búsqueda de Raíces
- **Velocidad de Convergencia**: Newton-Raphson converge más rápido (cuadráticamente) cuando la aproximación inicial es buena y la derivada está disponible.
- **Robustez vs. Velocidad**: La bisección es el método más robusto (siempre converge si hay cambio de signo) pero el más lento.
- **Sin Derivadas**: La secante proporciona una excelente alternativa cuando la derivada es difícil de calcular, con convergencia superlineal.
- **Eficiencia en Polinomios**: La combinación de Horner para evaluación con Newton para refinamiento es óptima para raíces de polinomios.

### Hallazgos Clave
1. **Compensación Fundamental**: Existe una compensación inevitable entre robustez y velocidad de convergencia en métodos de búsqueda de raíces.
2. **Importancia de la Suavidad**: Los métodos de integración de orden superior (Simpson) son notablemente más eficientes para funciones suaves.
3. **Selección Contextual**: No existe un "mejor método" universal; la elección depende del problema específico, recursos computacionales y requisitos de precisión.

---

## 🧠 Habilidades Demostradas

El proyecto refleja dominio en las siguientes áreas técnicas y analíticas:

| Área | Competencias Demostradas |
|------|---------------------------|
| **Programación en R** | Implementación modular, uso de funciones, manejo de estructuras de datos |
| **Análisis Numérico** | Comprensión de errores, estabilidad, convergencia y complejidad algorítmica |
| **Visualización** | Gráficos de convergencia, diagramas de error, comparaciones visuales con ggplot2 |
| **Documentación** | Explicaciones claras, ejemplos reproducibles, comentarios en código |
| **Pensamiento Crítico** | Análisis comparativo, identificación de ventajas/desventajas por método |
| **Reportes Técnicos** | Generación de documentos profesionales con R Markdown |

---

## 📈 Visualizaciones Incluidas

- **Comparación de métodos de integración**: Error vs. número de subdivisiones
- **Convergencia de métodos de raíces**: Error vs. iteraciones
- **Ilustraciones geométricas**: Interpretación visual de cada método
- **Gráficos de funciones**: Funciones originales vs. aproximaciones
- **Mapas de calor de error**: Distribución espacial del error
- **Diagramas de flujo**: Visualización del algoritmo de cada método

---

## 🔬 Casos de Prueba

El proyecto incluye ejemplos con diversas funciones para demostrar el comportamiento de cada método:

1. **Funciones polinómicas** (fácil integración analítica para validación)
2. **Funciones trascendentales** (seno, exponencial, logaritmo)
3. **Funciones con singularidades** (para probar robustez)
4. **Polinomios de alto grado** (para demostrar eficiencia de Horner)
5. **Funciones oscilatorias** (para probar métodos de integración)

---

## 👤 Autor

**Juan Pablo Gómez Morales**  
📧 *[prxvxjpg@gmail.com]*  
🎓 Estudiante de Ciencias/Ingeniería/Matemáticas  
📍 Bogotá, Colombia  

💡 *Proyecto académico desarrollado para el curso de Métodos Numéricos o Análisis Numérico.*

---
