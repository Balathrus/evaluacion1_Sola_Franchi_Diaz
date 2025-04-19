# Proyecto Snake Case

## Tipo de Evaluación
Evaluación Tipo 1

## Integrantes del Grupo
- Ariel Diaz
- Renato Franchi
- Fabian Sola

## Descripción del Proyecto
Este proyecto es un sistema de gestión de ventas e inventario desarrollado utilizando PSeInt, un intérprete de pseudocódigo diseñado para ayudar a los principiantes a aprender lógica de programación. El sistema permite a los usuarios gestionar las ventas de productos, hacer un seguimiento de los niveles de inventario y generar informes básicos.

## Dependencias del Proyecto
Este proyecto no requiere dependencias externas, ya que está basado en pseudocódigo y diseñado para ejecutarse en PSeInt. Asegúrese de tener PSeInt instalado en su computadora.

### Instrucciones para Ejecutar el Proyecto
1. **Instalar PSeInt**:
   - Puede descargar PSeInt desde su [sitio oficial](https://pseint.sourceforge.io/).
   
2. **Ejecutar los Scripts**:
   - Abrir PSeInt.
   - Cargar los archivos de pseudocódigo (.psc) desde el directorio del proyecto.
   - Ejecutar los scripts para realizar operaciones de ventas e inventario.

## Estructura del Proyecto
Este proyecto está organizado en los siguientes archivos:
- `ventas.psc`: Script para gestionar las transacciones de ventas.
- `inventario.psc`: Script para gestionar los datos del inventario.
- Otros archivos de pseudocódigo adicionales según se necesiten para funcionalidades adicionales.

## Funcionalidad Adicional Implementada
- **Gestión de productos**: Agregar, actualizar y eliminar productos del inventario.
- **Registro de ventas**: Registrar transacciones de ventas.
- **Seguimiento de inventario**: Realizar un seguimiento de los niveles de inventario de productos.
- **Generación de reportes**: Generar informes básicos sobre ventas e inventario.

## Excepciones Creadas y su Jerarquía
El proyecto ha implementado algunas excepciones para manejar errores comunes durante las operaciones de ventas e inventario.

### Ejemplos de Excepciones:
1. **Producto no encontrado**: Si se intenta realizar una venta de un producto que no existe en el inventario, se lanza una excepción de "Producto no encontrado".
2. **Stock insuficiente**: Si se intenta registrar una venta cuando no hay suficiente stock del producto, se lanza una excepción de "Stock insuficiente".

### Ejemplo de Manejo de Excepciones:
```pseudocode
Si stock < cantidad_a_vender Entonces
    Lanzar Excepción "Stock insuficiente"
Sino
    Realizar venta
Fin Si
