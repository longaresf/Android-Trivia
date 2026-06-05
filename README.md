# Android Navigation Flow & Trivia Challenge App

Este repositorio contiene una aplicación móvil nativa para la plataforma **Android** desarrollada en **Kotlin**. El proyecto implementa un sistema dinámico de cuestionarios (*Quiz*) diseñado para demostrar el control avanzado sobre el ciclo de vida de los componentes, la gestión de fragmentos y la arquitectura de flujos de navegación estructurados mediante buenas prácticas de desarrollo móvil.

## 🚀 Características y Capacidades Técnicas

* **Gestión de Flujos de Navegación:** Implementación de un árbol de pantallas optimizado mediante FragmentManager Component para controlar las transiciones entre el menú principal, el juego, la pantalla de victoria y la de fin de juego.
* **Arquitectura Basada en Fragmentos:** Uso eficiente de una arquitectura de actividad única (*Single-Activity Architecture*) donde múltiples fragmentos intercambian el estado de la lógica del juego de manera fluida.
* **Paso Seguro de Argumentos:** Configuración de envío de datos entre pantallas mediante Safe Args para transferir métricas del juego (como el número de respuestas correctas o el estado final) sin comprometer la memoria.
* **Diseño e Interfaz Reactiva:** Uso de componentes nativos de interfaz de usuario con soporte para navegación mediante gestos y botones de retroceso controlados (*Up Button*).

## 🛠️ Stack Tecnológico

* **Lenguaje Principal:** Kotlin
* **Plataforma:** Android SDK Nativo
* **UI & Layouts:** XML con componentes de Material Design
* **Arquitectura de Navegación:** FragmentManager.
* **Entorno de Desarrollo:** Android Studio

## ⚙️ Arquitectura de UI y Solución de Problemas

El desarrollo de este juego interactivo se centró en resolver desafíos críticos en la experiencia de usuario móvil:

1. **Control del Botón de Retroceso (Backstack Management):** Se configuró el flujo de pantallas para evitar que un usuario pueda regresar a la trivia una vez que el juego ha terminado (pantallas de *Win* o *Game Over*), limpiando correctamente la pila de navegación de Android.
2. **Preservación del Estado del Juego:** Manejo del ciclo de vida de los fragmentos para asegurar que rotaciones de pantalla u otras interrupciones del sistema no corrompan el progreso o las preguntas actuales del usuario.
3. **Desacoplamiento Lógico:** Separación estricta entre los datos del cuestionario (banco de preguntas y respuestas) y la lógica de renderizado visual de las vistas.

## 🔧 Configuración y Ejecución Local

Para compilar e inspeccionar el grafo de navegación en **Android Studio**, sigue estos pasos:

1. **Clonar el repositorio:**
```bash
   git clone [https://github.com/longaresf/android-navigation-flow-quiz.git](https://github.com/longaresf/android-navigation-flow-quiz.git)
````

2. Abrir el proyecto:
  Inicia Android Studio, selecciona File > Open y elige el directorio clonado.

3. Sincronización de dependencias:
  Deja que el sistema descargue los plugins de navegación y las dependencias de Gradle configuradas.

4. Despliegue:
  Ejecuta la aplicación en un emulador o dispositivo físico haciendo clic en el botón Run.

✒️ Autor

    Francisco Longares - Desarrollador Mobile Android - longaresf
