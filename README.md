# **Evidencia 1: Actividad Integradora - TC2008B**

## **Descripción del Proyecto**
Este proyecto corresponde a la **Actividad Integradora** de la materia **Modelación de Sistemas Multiagentes con Gráficas Computacionales**. El objetivo principal es demostrar la aplicación de conocimientos en **gráficas computacionales** y sistemas multiagentes mediante la implementación de un entorno 3D interactivo y elementos funcionales relacionados con un modelo urbano.

---

## **Objetivo**
Crear una escena 3D en Unity que represente elementos esenciales del entorno urbano y visualice vectores relacionados con un modelo de iluminación basado en Lambert y Phong. El enfoque incluye la correcta representación de vectores, materiales y luces, siguiendo una metodología clara y estructurada.

---

## **Requisitos Técnicos Implementados**

### **1. Elementos de la Escena**
- **Esfera (Sphere):** 
  - Posición: \((-1.99493, 0.88122, 0.04875)\).
  - Escala ajustada al radio: \(0.66375\).
  - Material con shader estándar, incluyendo propiedades de **Albedo**, **Metallic** y **Smoothness**.

- **Luz Puntual (Point Light):**
  - Posición: \((-3.02474, 3.77452, 4.22934)\).
  - Intensidad: \(1.5\).
  - Configuración adecuada para resaltar los elementos en la escena.

- **Cámara (Main Camera):**
  - Posición: \((-3.79225, 4.71999, -4.74818)\).
  - Rotación: \((35, 45, 0)\) para enfocar correctamente la esfera.

---

### **2. Visualización de Vectores**
El proyecto incluye la visualización de los siguientes vectores relacionados con la iluminación del modelo:
1. **Vector Normal (\(n\)):** Representado en color verde.
2. **Vector de Luz (\(l\)):** Representado en color amarillo.
3. **Vector Reflejado (\(r\)):** Representado en color azul.
4. **Vector de Vista (\(v\)):** Representado en color rojo.
5. **Vector Paralelo (\(lp\)):** Representado en color cian.
6. **Vector Ortogonal (\(lo\)):** Representado en color magenta.

---

## **Pasos para la Configuración en Unity**
1. **Crear Proyecto:**
   - Abre Unity Hub y selecciona `New Project > 3D Core`.
   - Nombra el proyecto como `LightingVectorsProject`.

2. **Crear la Escena:**
   - Agrega una esfera (`Sphere`) y ajusta su posición, escala y material.
   - Añade una luz puntual (`Point Light`) y configúrala.
   - Ajusta la cámara (`Main Camera`) para capturar la escena adecuadamente.

3. **Escribir el Script `VectorVisualizer`:**
   - Implementa un script en C# para dibujar los vectores en la escena mediante la función `OnDrawGizmos()`.

4. **Asignar Referencias:**
   - Vincula la esfera, luz y cámara al script para calcular y visualizar los vectores correctamente.

5. **Guardar y Exportar:**
   - Guarda la escena como `LightingScene`.
   - Exporta el proyecto como un archivo `.unitypackage`.

---

## **Estructura del Repositorio**
```
├── Assets/
│   ├── Scenes/
│   │   ├── LightingScene.unity
│   ├── Scripts/
│   │   ├── VectorVisualizer.cs
│   ├── Materials/
│   │   ├── SphereMaterial.mat
│   ├── Capturas/
│   │   ├── escena_game.png
│   │   ├── escena_scene.png
│   │   ├── configuraciones_inspector.png
├── README.md
```

---

## **Resultados y Validación**
1. **Vectores Representados:**
   - Cada vector calculado matemáticamente se visualiza en la escena con colores asignados.
2. **Configuraciones Correctas:**
   - Materiales y luces ajustados según el modelo de iluminación.
3. **Compatibilidad:**
   - El archivo `.unitypackage` incluye únicamente los elementos necesarios para la evaluación.

---

## **Instrucciones para Evaluación**
1. Descarga el archivo `.unitypackage` desde el repositorio.
2. Importa el archivo en Unity para verificar la escena y los vectores.
3. Abre la escena `LightingScene` para explorar la configuración y resultados.

---

## **Licencia y Créditos**
- Este proyecto es propiedad del autor, desarrollado como evidencia de aprendizaje en **TC2008B**.
- Elementos externos utilizados en la escena están acreditados en el archivo `credits.txt` ubicado en la carpeta de Assets.
