# Simulación de Red (PARTE 2) en Python

Este proyecto es una simulación básica de una red de comunicación implementada en Python utilizando **Programación Orientada a Objetos (POO)**. Se modela la comunicación entre un **servidor** y **tres clientes**, permitiendo la transmisión de mensajes entre ellos.

## Características
- Implementa la clase `Nodo`, que representa un dispositivo en la red.
- Permite conectar y desconectar nodos dinámicamente.
- Simula el envío y recepción de mensajes.
- Uso de `time.sleep()` para representar retrasos en la reconexión.

## Explicación del Código
### 1. **Clase `Nodo`**
Cada nodo en la red tiene:
- Un `nombre` que lo identifica.
- Una lista `conexiones` para almacenar los nodos conectados.

### 2. **Métodos de la Clase `Nodo`**
- `agregar_conexion(nodo)`: Conecta el nodo con otro.
- `eliminar_conexion(nodo)`: Desconecta el nodo de otro.
- `enviar_mensaje(mensaje)`: Envía un mensaje a todos los nodos conectados.
- `recibir_mensaje(mensaje, emisor)`: Recibe un mensaje y muestra el emisor.

### 3. **Flujo del Programa**
1. Se crean un servidor y tres clientes.
2. Se establecen las conexiones entre el servidor y los clientes.
3. Se envía un mensaje inicial desde el servidor a todos los clientes.
4. Se simula la desconexión del Cliente2.
5. Se espera 2 segundos antes de reconectar al Cliente2.
6. Se envía un nuevo mensaje tras la reconexión.
