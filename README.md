# web-iaw · Git y GitHub desde cero

Proyecto desarrollado para la unidad de **Git y GitHub** del módulo de **Implantación de Aplicaciones Web (IAW)** de 2.º ASIR.

## Descripción del Proyecto
Este proyecto es una aplicación web básica estructurada de forma modular, diseñada para poner en práctica el control de versiones con Git, el trabajo remoto en GitHub, la gestión de ramas, resolución de conflictos y el uso asistido de Inteligencia Artificial como asistente de desarrollo profesional.

## Estructura del Repositorio
```text
web-iaw/
├── .gitignore                    # Exclusión de archivos confidenciales (.env) y logs (*.log)
├── README.md                     # Documentación principal del proyecto
├── index.html                    # Página principal con resolución de conflictos de ramas
├── contacto.html                 # Página de contacto con formulario desarrollada en feature/contacto
├── estilos.css                   # Hoja de estilos visuales
└── ACTIVIDADES_IAW_GIT_GITHUB.md # Memoria completa de actividades, resolución y reflexiones
```

## Requisitos
- Navegador web moderno (Google Chrome, Mozilla Firefox, Microsoft Edge).
- Git 2.30+ instalado localmente.
- Cuenta en GitHub y autenticación mediante clave SSH o Git Credential Manager.

## Instalación y Clonación
Para clonar este repositorio en tu equipo local:
```bash
git clone git@github.com:marcelomoralgutierrez/web-iaw.git
cd web-iaw
```

## Ejecución
Abrir el archivo `index.html` en cualquier navegador web o mediante la extensión *Live Server* en Visual Studio Code.

## Documentación de uso de Inteligencia Artificial (Paso 20)
En cumplimiento de la **Práctica integradora individual (Paso 20)**, se ha documentado el uso de IA en dos momentos clave:

1. **Uso 1: Asistencia en la interpretación del estado del repositorio y revisión de diffs (Ejercicios 21 y 22)**
   - **Qué hizo la IA**: Analizó las salidas de `git status` y `git diff`, identificando con precisión qué archivos se encontraban en el Working Directory y cuáles en Staging, y propuso mensajes de commit claros, atómicos y semánticos.
   - **Decisiones tomadas por el alumno**: Verifiqué manualmente con `git diff --staged` que sólo los archivos correspondientes entraran en el commit antes de autorizarlo, descartando mensajes genéricos y manteniendo la trazabilidad del historial.

2. **Uso 2: Análisis de riesgos en instrucciones peligrosas y resolución de conflictos (Ejercicios 18 y 23)**
   - **Qué hizo la IA**: Explicó la estructura de los marcadores de conflicto (`<<<<<<< HEAD`, `=======`, `>>>>>>>`) y desaconsejó el uso de comandos destructivos como `git reset --hard HEAD~3`, recomendando `git revert` para historiales compartidos.
   - **Decisiones tomadas por el alumno**: Resolví el conflicto de fusión en `index.html` unificando el código, eliminé las marcas de conflicto, preparé el archivo resuelto y concluí la fusión con un commit explicativo.

---
**Autor:** Marcelo Moral Gutiérrez  
**Curso:** 2.º ASIR - Implantación de Aplicaciones Web (IAW)
