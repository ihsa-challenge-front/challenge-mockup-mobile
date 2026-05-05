# React Native Challenge: Data Dashboard & Real-Time Visualization

¡Bienvenido al desafío técnico para Mobile! Este challenge está diseñado para evaluar no solo tus habilidades escribiendo código, sino también tus decisiones de arquitectura, manejo de estado complejo, optimización de rendimiento y buenas prácticas en React Native.

## El Objetivo

Tu misión es construir una **Aplicación Móvil Analítica** que muestre datos de entidades complejas (por ejemplo, activos financieros, monitorización de servidores o métricas de e-commerce).

No buscamos un diseño "pixel-perfect" basado en un mockup estricto, sino una interfaz limpia, accesible y con un rendimiento fluido donde demuestres tu dominio técnico y sensibilidad por la UX/UI en dispositivos móviles.

## Requerimientos Técnicos

1. **Stack Tecnológico:**
   - **Framework:** React Native (Expo o React Native CLI).
   - **Tipado:** TypeScript estricto de uso obligatorio (sin `any` injustificados).
   - **Estilos:** StyleSheet, NativeWind, styled-components, o herramientas similares.

2. **Funcionalidades Clave:**
   - **Data Fetching & Caching:** Conéctate a una API pública (ej. CoinCap para criptomonedas o Rick and Morty/PokeAPI si prefieres un dominio más sencillo manejando un volumen alto de datos).
   - **Real-Time Data:** Implementa WebSockets (o polling secundario persistente usando TanStack Query/SWR) para actualizar la información sin bloquear la UI ni causar re-renders innecesarios.
   - **Filtros e Interacción:** El usuario debe poder buscar, aplicar filtros múltiples y visualizar los datos mediante listas virtualizadas (*Infinite Scroll* usando `FlatList` o `FlashList`).
   - **Visualización Gráfica:** Integra gráficos (ej. `react-native-chart-kit`, `victory-native` o `react-native-svg`) para mostrar métricas o históricos de la entidad seleccionada.

3. **Arquitectura y Calidad de Código:**
   - **Patrones de Diseño:** Aplica principios SOLID y diseña componentes reutilizables, separando la lógica de negocio (hooks/servicios) de las vistas.
   - **Manejo de Estado:** Utiliza las herramientas adecuadas para cada caso: estado local vs estado global (Zustand, Context, Redux) vs estado de servidor (TanStack Query, SWR).
   - **Testing:** 
     - Tests unitarios y de componentes críticos usando Jest y React Native Testing Library.
     - (Opcional) Al menos un flujo End-to-End con Detox o Maestro.

4. **Experiencia de Usuario (UX) y Performance:**
   - **Rendimiento Móvil:** Optimizaciones clave para 60fps, uso eficiente del *bridge* (o JSI en Nueva Arquitectura), renderizado eficiente de listas grandes y animaciones fluidas (recomendado `react-native-reanimated`). Implementación de `useMemo`/`useCallback`/`memo` solo donde aporte valor real.
   - **Manejo de Errores:** Implementación de *Error Boundaries*, *skeleton loaders* y manejo de pérdida de conexión de red para una experiencia robusta.

## Entregables
1. Repositorio en Git.
2. Un archivo `README.md` propio dentro del proyecto que incluya:
   - Instrucciones claras para inicializar el proyecto en local.
   - **Decisiones de arquitectura:** Un breve apartado justificando tu elección de stack tecnológico, librerías y patrones utilizados.
   - **Trade-offs:** ¿Qué cosas hubieras hecho diferente de contar con más tiempo?
3. **[Bonus]** Generación de APK/AAB o despliegue a través de Expo (EAS Build / Expo Go) facilitando un QR para probarlo.

## Criterios de Evaluación
- **Estructura del Proyecto:** Qué tan escalable y mantenible es la base de código.
- **Resiliencia:** Cómo la aplicación maneja caídas de red, latencia alta, y visualización de errores controlados.
- **Madurez de TypeScript:** Uso y creación de interfaces complejas, utilidades de tipos y genéricos.
- **Testing Estratégico:** No te pedimos 100% de coverage, sino pruebas que aseguren el comportamiento principal y aporten valor.
- **Autonomía:** Capacidad de comunicar el "por qué" detrás del código escrito.

---

*Nota:* Sabemos que tu tiempo libre es valioso. No esperamos que le inviertas una cantidad de horas desmesurada. Enfócate en estructurar una base sólida, modular, que cumpla con los requisitos esenciales y demuestre tu nivel de experiencia. ¡Mucho éxito!