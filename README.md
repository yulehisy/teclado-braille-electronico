# Braille
# Proyecto: Teclado Braille Electrónico para personas invidentes
Proyecto integrador de Diseño Electrónico — Curso Integrador I
# integrantes
- Yulehisy Rodriguez - Rol: [Documentacion/ Redaccion/ Pruebas]
- Ana Laurente - Rol: [Pruebas/ Simulacion/ Hardware/ Software]

## ESTRUCTURA DEL PROYECTO

## Descripción General

Este proyecto consiste en el diseño y construcción de un **teclado Braille electrónico de bajo costo** que permite a personas con discapacidad visual escribir de manera autónoma. El sistema utiliza pulsadores para ingresar combinaciones Braille, procesadas por un microcontrolador Arduino UNO.  
la salida se realiza a través del monitor serial o mediante retroalimentación háptica/auditiva opcional[1].

---

## Índice

- [Planteamiento del Problema](#planteamiento-del-problema)
- [Objetivos](#objetivos)
- [Justificación](#justificación)
- [Marco Teórico](#marco-teórico)
- [Metodología](#metodología)
- [Componentes Utilizados](#componentes-utilizados)
- [Funcionamiento](#funcionamiento)
- [Resultados y Pruebas](#resultados-y-pruebas)
- [Conclusiones y Mejoras Futuras](#conclusiones-y-mejoras-futuras)
- [Créditos](#créditos)

---

## Planteamiento del Problema

El acceso a la información escrita sigue siendo un reto para personas con discapacidad visual, especialmente en contextos donde las soluciones tecnológicas son costosas o difíciles de implementar.  
El objetivo es **mejorar el acceso a la escritura** mediante el desarrollo de un teclado Braille electrónico accesible y funcional [1].

---

## Objetivos

**Objetivo General:**  
Diseñar y construir un sistema Braille electrónico de bajo costo que permita a personas con discapacidad visual escribir de forma autónoma[1].

**Objetivos Específicos:**  
- Analizar el costo y disponibilidad de los componentes electrónicos y materiales empleados.
- Evaluar el desempeño temporal del prototipo, midiendo el tiempo de respuesta ante la pulsación de teclas.
- Optimizar la precisión y sincronización en la activación de los pines Braille[1].

---

## Justificación

El proyecto responde a la necesidad de promover la **inclusión social y educativa** de las personas con discapacidad visual, facilitando su acceso a la escritura mediante un sistema accesible y económico.  
Su bajo costo permite la masificación y adopción en contextos educativos y comunitarios con recursos limitados[1].

---

## Marco Teórico

- **Braille:** Sistema de escritura táctil que utiliza combinaciones de puntos en relieve para representar letras, números y símbolos.
- **Teclado Braille Electrónico:** Dispositivo que permite la entrada de caracteres Braille mediante pulsadores electrónicos, traduciendo las combinaciones en texto digital.
- **Arduino UNO:** Microcontrolador utilizado para procesar las señales de los pulsadores y controlar la salida.
- **Pulsadores y Resistencias:** Cada pulsador representa uno de los seis puntos Braille, más un pulsador adicional para el espacio. Las resistencias de 220Ω se emplean como pull-down para asegurar la correcta lectura de las señales digitales.
- **Retroalimentación háptica/auditiva:** Opcional, mejora la experiencia del usuario al confirmar cada acción realizada[1].

---

## Metodología

1. **Análisis del sistema Braille:** Identificación de patrones válidos.
2. **Diseño electrónico:** Circuito con Arduino UNO, 6 pulsadores para puntos Braille y 1 para espacio, resistencias pull-down.
3. **Programación:** Código en Arduino IDE para reconocimiento y traducción de combinaciones Braille.
4. **Simulación:** Pruebas virtuales en Tinkercad para validar el diseño.
5. **Montaje:** Ensamblaje en protoboard y pruebas físicas.
6. **Validación:** Medición de tiempo de respuesta, tasa de error y facilidad de uso[1].

---

## Componentes Utilizados

| Componente               | Cantidad | Descripción / Función                       |
|--------------------------|----------|---------------------------------------------|
| Arduino UNO              | 1        | Procesamiento y control del sistema         |
| Pulsadores               | 7        | Entrada de datos (6 puntos + espacio)       |
| Resistencias 220Ω        | 7        | Pull-down para evitar lecturas erróneas     |
| Protoboard               | 1        | Montaje temporal del circuito               |
| Cables jumper            | varios   | Conexiones eléctricas                       |
| (Opcional) Buzzer/Vibrador | 1      | Retroalimentación sonora/háptica            |

---

## Funcionamiento

1. **Entrada:** El usuario presiona una combinación de pulsadores correspondiente a un carácter Braille.
2. **Procesamiento:** El Arduino detecta la combinación y determina el carácter.
3. **Salida:** El carácter se muestra en el monitor serial de la computadora o se comunica mediante retroalimentación sonora/háptica.
4. **Espacio:** Un pulsador adicional permite insertar espacios entre palabras[1].

---

## Resultados y Pruebas

- Reconocimiento preciso de las combinaciones Braille estándar (26 letras y espacio).
- Tiempo de respuesta promedio: **0.15 segundos** por pulsación.
- Tasa de error: **Inferior al 2%** durante pruebas de 100 ciclos.
- Simulación y montaje físico muestran resultados similares, validando la robustez del diseño.
- Mejoras implementadas: filtrado de señales y refuerzo del encofrado para mayor estabilidad y durabilidad[1].

---

## Conclusiones y Mejoras Futuras

- El prototipo cumple con los objetivos de accesibilidad, bajo costo y facilidad de uso.
- Futuras mejoras: agregar retroalimentación háptica/auditiva y explorar conectividad inalámbrica.
- El sistema es replicable y adaptable a contextos educativos, promoviendo la autonomía de personas con discapacidad visual[1].

---

## Créditos

**Alumnas:**  
- Rodriguez Vega Yulehisy Lizbeth  
- Ana Laurente Cochachi

**Profesor:**  
- Motta Zorrilla, Bryan

**Curso:**  
- Curso Integrador I: Diseño Electrónico
