# Braille
# Proyecto: Teclado Braille Electrónico para personas invidentes
Proyecto integrador de Diseño Electrónico — Curso Integrador I
# integrantes
- Yulehisy Rodriguez - Rol: [Documentacion/ Redaccion/ Pruebas]
- Ana Laurente - Rol: [Pruebas/ Simulacion/ Hardware/ Software]

## ESTRUCTURA DEL PROYECTO

## Descripción

Este proyecto consiste en el diseño y construcción de un teclado Braille electrónico de bajo costo, orientado a personas con discapacidad visual. El objetivo es permitirles escribir de forma autónoma mediante un sistema accesible, económico y fácil de replicar, utilizando tecnologías abiertas como Arduino.

## Tabla de Contenidos

- [Planteamiento del Problema](#planteamiento-del-problema)
- [Objetivos](#objetivos)
- [Justificación](#justificación)
- [Marco Teórico](#marco-teórico)
- [Arquitectura del Sistema](#arquitectura-del-sistema)
- [Componentes](#componentes)
- [Instalación y Uso](#instalación-y-uso)
- [Pruebas y Validación](#pruebas-y-validación)
- [Contribuciones](#contribuciones)
- [Licencia](#licencia)

## Planteamiento del Problema

El acceso a la información escrita es un reto para personas con discapacidad visual, especialmente por el alto costo y la complejidad de los dispositivos comerciales. Este proyecto busca desarrollar una alternativa funcional y asequible, centrada en el contexto educativo y social de países en vías de desarrollo.

## Objetivos

- **General:** Diseñar y construir un sistema Braille electrónico de bajo costo que permita a personas con discapacidad visual escribir de forma autónoma.
- **Específicos:**
  - Analizar costos y disponibilidad de componentes.
  - Evaluar el desempeño temporal y la tasa de errores del prototipo.
  - Optimizar la precisión y la confiabilidad del sistema.

## Justificación

El proyecto promueve la inclusión social y educativa, facilitando la autonomía y la comunicación escrita de personas con discapacidad visual. Su bajo costo y facilidad de replicación lo hacen ideal para contextos de bajos recursos.

## Marco Teórico

El sistema Braille electrónico utiliza pulsadores que representan los seis puntos del código Braille, conectados a un microcontrolador Arduino UNO. Al presionar una combinación, el sistema traduce la señal a un carácter alfabético, que se muestra en una pantalla LCD 16x2. Se incorpora retroalimentación háptica y/o auditiva para mejorar la experiencia del usuario.

## Arquitectura del Sistema

- **Microcontrolador:** Arduino UNO
- **Entradas:** 6 pulsadores (puntos Braille) + 1 pulsador de espacio
- **Salidas:** Pantalla LCD 16x2, zumbador/vibrador para retroalimentación
- **Alimentación:** 5V DC

![Diagrama de conexión](docs/diagramas/diagrama_circuito.png)

## Componentes

- Arduino UNO
- Pulsadores x7
- Resistencias 220Ω x7 (pull-down)
- Pantalla LCD 16x2
- Zumbador o motor vibrador (opcional)
- Protoboard y cables

Ver el archivo [`hardware/lista_componentes.md`](hardware/lista_componentes.md) para el detalle completo.

## Instalación y Uso

1. **Montaje:** Siga los diagramas en `docs/diagramas/` para conectar los componentes.
2. **Carga de código:** Suba el archivo `software/arduino/braille_keyboard.ino` al Arduino usando el IDE de Arduino.
3. **Pruebas:** Realice las pruebas siguiendo las instrucciones en `test/`.
4. **Uso:** Presione las combinaciones de pulsadores para escribir en Braille; el carácter aparecerá en la pantalla LCD y se emitirá una señal de confirmación.

## Pruebas y Validación

- Se recomienda medir el tiempo de respuesta y la tasa de errores.
- Comparar los resultados con teclados Braille comerciales.
- Documentar los resultados en la carpeta `test/`.

## Contribuciones

Las contribuciones son bienvenidas. Por favor, abra un issue o un pull request para sugerencias o mejoras.

## Licencia

Este proyecto está bajo la licencia MIT. Consulte el archivo [`LICENSE`](LICENSE) para más detalles.
