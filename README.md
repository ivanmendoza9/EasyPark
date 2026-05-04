# 🚗 Sistema de Estacionamiento Inteligente  
## Implementación del Patrón State

## 👨‍💻 Autor

**Ivan Mendoza**

---

## 📌 Introducción
Este proyecto consiste en la simulación de un sistema de estacionamiento inteligente, enfocado en el control de una pluma de acceso.  

Se implementa el **patrón de diseño State**, el cual permite modelar el comportamiento dinámico del sistema dependiendo de su estado actual.

El objetivo principal es representar cómo un objeto puede cambiar su comportamiento sin utilizar múltiples estructuras condicionales, logrando un diseño más limpio y escalable.

---

## 🎯 Objetivo
Desarrollar una simulación interactiva que represente el funcionamiento de una pluma automática, aplicando el patrón State para gestionar sus diferentes estados.

---

## ⚙️ Funcionamiento del Sistema

El sistema simula el comportamiento de una pluma de estacionamiento mediante los siguientes eventos:

- 🚗 **Entrada de vehículo** → solicita apertura  
- 🚙 **Salida de vehículo** → libera espacio  
- ⏱️ **Cierre automático** → la pluma se cierra después de un tiempo  

Además, se incluye:

- Control de espacios disponibles  
- Indicador visual (semáforo)  
- Registro de eventos en tiempo real  

---

## 🔄 Estados del Sistema

El sistema se compone de los siguientes estados:

- **Cerrada**: bloquea el acceso  
- **Abriéndose**: transición de apertura  
- **Abierta**: permite el paso  
- **Cerrándose**: transición de cierre  

Los estados intermedios no aceptan acciones, evitando inconsistencias en el sistema.

---

## 🧠 Implementación del Patrón State

El patrón State se implementa mediante:

- **Clase Contexto (`Pluma`)**  
  Mantiene el estado actual y delega las acciones.

- **Método `request()`**  
  Centraliza las acciones del sistema.

- **Método `handle()` en cada estado**  
  Define cómo responde cada estado a una acción.

- **Transiciones dinámicas**  
  Se realizan mediante el método `setEstado()`.

---

## 🔥 Influencia del Patrón en el Proyecto

El uso del patrón State permite:

- Eliminar múltiples estructuras condicionales  
- Separar responsabilidades por estado  
- Facilitar el mantenimiento y escalabilidad  
- Representar comportamientos dinámicos de forma clara  

Gracias a este patrón, el sistema es más organizado y adaptable a futuros cambios.

---

## 📊 Conclusión

La implementación del patrón State en este proyecto demuestra cómo es posible modelar sistemas dinámicos de manera estructurada y eficiente.

El sistema logra simular un entorno realista de control de acceso, destacando la importancia de los patrones de diseño en el desarrollo de software limpio, escalable y mantenible.

---

## 🚀 Tecnologías Utilizadas

- HTML  
- CSS  
- JavaScript  

