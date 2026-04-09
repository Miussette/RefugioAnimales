# 🐾 Refugio de Animales (Sistema en Consola)

Este proyecto consiste en un sistema en consola desarrollado en Java que permite gestionar un refugio de animales.

El sistema está diseñado para ser simple, robusto y fácil de usar, pensado para voluntarios que necesitan registrar y administrar animales rescatados.

---

## 🎯 Funcionalidades

El sistema permite:

- Registrar especies
- Registrar animales
- Marcar animales como adoptados
- Ver animales disponibles
- Ver animales adoptados
- Generar un reporte general

---

## 🧩 Estructuras de datos utilizadas

Se utilizaron distintas estructuras de Java para representar la información:

- List<Integer> ids → almacena los IDs únicos de los animales
- Map<Integer, String> nombreAnimal → relaciona ID con nombre del animal
- Map<Integer, String> estadoAnimal → relaciona ID con estado (Disponible / Adoptado)
- Map<Integer, String> animalEspecie → relaciona ID con especie
- Set<String> especies → almacena especies sin duplicados
- String[] estados → array con estados fijos

---

## 🧠 Decisión importante (ID único)

Para permitir animales con el mismo nombre, se implementó un ID único por animal.

Ejemplo:

1 → Luna → Perro → Disponible  
2 → Luna → Gato → Adoptado  

Esto evita conflictos y mejora la estructura del sistema.

---

## ▶️ Cómo ejecutar el programa

### 1. Compilar

```bash
javac RefugioAnimales.java
2. Ejecutar
java RefugioAnimales
🖥️ Ejemplo de menú

=== REFUGIO DE ANIMALES ===

Registrar animal
Registrar especie
Marcar animal como adoptado
Mostrar animales disponibles
Mostrar animales adoptados
Mostrar reporte general
Salir
📊 Ejemplo de reporte

=== REPORTE GENERAL ===
Total animales: 2
Disponibles: 1
Adoptados: 1

ID | Nombre | Especie | Estado
1 | Luna | Perro | Disponible
2 | Luna | Gato | Adoptado

⚠️ Validaciones implementadas
No permite registrar animales con especies inexistentes
No permite adoptar animales que no existen
No permite adoptar animales ya adoptados
No permite ingresar datos inválidos en el menú
🎓 Objetivo del proyecto

Este proyecto tiene como objetivo practicar:

Uso de estructuras de datos (List, Map, Set)
Manejo de menús con do-while
Validaciones de entrada
Organización del código en métodos
Pensamiento lógico para sistemas reales

🚀 Posibles mejoras futuras
Implementar Programación Orientada a Objetos (POO)
Crear clase Animal
Persistencia con base de datos
Interfaz gráfica
Búsqueda y edición de animales