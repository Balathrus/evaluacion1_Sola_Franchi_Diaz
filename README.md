# Proyecto de Venta e Inventario - PSeInt

## Tipo de evaluación
Evaluación **1**

## Nombres de los integrantes del grupo
- Ariel Diaz
- Renato Franchi
- Fabian Sola

## Descripción detallada del proyecto
Este proyecto tiene como objetivo desarrollar un sistema de gestión de ventas e inventarios en PSeInt. Permite registrar productos, realizar ventas, actualizar el inventario en tiempo real y generar reportes básicos sobre las transacciones realizadas. El sistema es modular y permite la extensión de funcionalidades según las necesidades del usuario.

## Dependencias del proyecto
- **PSeInt**: Se utiliza el entorno PSeInt para la ejecución del pseudocódigo. Puede descargarse desde [aquí](https://pseint.sourceforge.io/).
- **Sistema Operativo**: Windows, macOS o Linux (dependiendo de la configuración de PSeInt en tu plataforma).

## Instrucciones para ejecutar el proyecto
1. **Descarga y configuración de PSeInt**:
   - Si no tienes PSeInt, descarga la última versión desde [su página oficial](https://pseint.sourceforge.io/).
   - Instala PSeInt según las instrucciones para tu sistema operativo.

2. **Cargar el proyecto**:
   - Abre PSeInt y carga los archivos de pseudocódigo del proyecto (`ventas.psc`, `inventario.psc`, etc.).

3. **Ejecución**:
   - Ejecuta los scripts de acuerdo a los procesos que desees simular, como registrar ventas o actualizar inventario.

## Estructura del proyecto
El proyecto se organiza en archivos de pseudocódigo (.psc), cada uno con una funcionalidad específica:

- **ventas.psc**: Script principal para gestionar las transacciones de ventas.
- **inventario.psc**: Script para controlar el inventario de productos.
- **reportes.psc**: Script opcional para generar informes sobre ventas e inventario.

## Funcionalidad adicional implementada
- **Gestión de inventario**: Los productos pueden ser añadidos, modificados o eliminados en el inventario.
- **Registro de ventas**: Se pueden realizar ventas que actualizan automáticamente el inventario.
- **Informes básicos**: Se generan reportes simples de las ventas y el estado del inventario.

## Breve explicación de las excepciones creadas y su jerarquía
En este proyecto se han implementado algunas excepciones básicas para manejar errores en la entrada de datos y la ejecución de operaciones:

1. **Excepción ProductoNoDisponible**: Se lanza cuando un producto solicitado no está disponible en el inventario.
2. **Excepción InventarioInsuficiente**: Se lanza cuando la cantidad de productos en inventario es insuficiente para cubrir una venta.
3. **Excepción EntradaInvalida**: Se utiliza para manejar errores en la entrada de datos por parte del usuario (como ingresar texto en lugar de números).

## Ejemplos de cómo se manejan las excepciones en el código
- **Ejemplo de ProductoNoDisponible**:
  ```pseint
  Si producto_no_disponible Entonces
      Escribir "Error: El producto no está disponible."
  FinSi
