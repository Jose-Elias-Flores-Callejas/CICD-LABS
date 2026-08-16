# CICD-LABS

Laboratorio 1 de CI/CD - GitHub Actions

## Descripcion

Repositorio de practica para el curso de Integracion y Despliegue Continuo (CI/CD).

## Estructura

- `app/` - Aplicacion de ejemplo
- `.github/workflows/` - Pipelines de GitHub Actions

## Laboratorio 2 - Flujo con ramas y pull requests

Este laboratorio agrega el flujo de trabajo colaborativo con Git:

- Creacion de una rama de trabajo (`feature/lab2-readme`) independiente de `main`.
- Modificacion del archivo README en la rama.
- Publicacion de la rama en el repositorio remoto.
- Creacion de un pull request hacia `main`.
- Ejecucion automatica del pipeline de CI al subir la rama.
- Proteccion de la rama `main` para impedir modificaciones directas (solo mediante pull requests).

## Laboratorio 3 - Pruebas unitarias automatizadas

- Proyecto de ejemplo en `app/` (calculadora en Python).
- Pruebas unitarias con `pytest` en `app/tests/`.
- El pipeline ejecuta: compilacion (`compileall`), pruebas con cobertura y publica reportes como artefactos.
- Quality Gate: si alguna prueba falla, el pipeline se detiene y el merge queda bloqueado.