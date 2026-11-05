# Evaluador de puntos dropoff · Red Puntos Colab

Herramienta web para evaluar nuevos puntos dropoff: mapa de sellers y puntos, cobertura por radio, propuesta de puntos nuevos y análisis de distancias.

**Este repositorio solo contiene código. No contiene datos.** Los datos (sellers, ventas, direcciones, puntos) viven en Firebase Firestore. Las reglas de [firestore.rules](firestore.rules) solo permiten leerlos a quien inició sesión con un correo verificado que la owner autorizó.

## Acceso
- Las personas invitadas entran con Google o con correo y clave (verificando el correo).
- La owner gestiona quién tiene acceso desde la pestaña **Administración**.

## Actualizar datos (owner)
1. En el computador local, con los Excel actualizados, correr `python preparar_datos.py`.
2. En la página, ir a **Administración → Datos** y subir `datos_firestore.json`.

El archivo de datos nunca se sube a este repositorio.
