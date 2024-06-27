# Gilded Rose Kata

Este proyecto implementa la Kata Gilded Rose, un ejercicio diseñado para practicar la refactorización de código y el desarrollo guiado por pruebas (TDD).

# Contexto del Proyecto

La Kata Gilded Rose simula un sistema de gestión de inventario para una tienda de artículos diversos. El objetivo es actualizar el estado de los artículos diariamente según reglas específicas de degradación y mejora de la calidad.

# Descripción de la Kata

La tienda Gilded Rose maneja diferentes tipos de artículos con reglas específicas de actualización:
- Todos los artículos tienen una propiedad `sellIn` que indica los días restantes para su venta.
- Todos los artículos tienen una propiedad `quality` que determina su valor.
- Después de la fecha de venta (`sellIn`), la calidad disminuye al doble de velocidad.
- La calidad de un artículo nunca es negativa.
- "Aged Brie" mejora su calidad con el tiempo.
- "Sulfuras" es un artículo legendario y no cambia en calidad ni días para vender (`sellIn`).
- "Backstage passes" incrementa su calidad a medida que se acerca la fecha del concierto.
- "Conjured" es una nueva categoría que degrada en calidad el doble de rápido que los artículos normales.

# Requisitos del Proyecto

- Desarrollar la lógica de programación siguiendo las reglas especificadas.
- Utilizar pruebas unitarias para verificar el comportamiento de cada tipo de artículo.
- No alterar la estructura del objeto `Item` ni sus propiedades.

# Estructura del Proyecto

El proyecto está estructurado en las siguientes partes:
- `com.gildedrose`: Contiene las clases principales del sistema.
- `com.gildedrose.Item`: Define la clase `Item` con sus propiedades básicas y métodos.
- `com.gildedrose.GildedRose`: Implementa el sistema de gestión de calidad de los artículos.
- `com.gildedrose.GildedRoseTest`: Contiene pruebas unitarias para verificar el comportamiento del sistema.

# Ejecución

Para ejecutar el programa y ver la simulación de la gestión de calidad de los artículos, puedes ejecutar la clase `TexttestFixture` desde tu IDE o línea de comandos. Asegúrate de tener configurado Java en tu entorno de desarrollo.


# Tests

Las pruebas unitarias están implementadas usando JUnit 5 en la clase `GildedRoseTest`. Cada método de prueba verifica el estado de los artículos después de una actualización de calidad, asegurando que se cumplan las reglas especificadas para cada tipo de artículo.



# Créditos Adicionales

- El código inicial y los requisitos fueron proporcionados como parte del ejercicio de aprendizaje.
- Las categorías de artículos se determinan por la cadena contenida en sus nombres.
