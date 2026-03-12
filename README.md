# Segmentación de Red y Enrutamiento Inter-VLAN: Sucursal Logística 🚢🌐

## 1. El Escenario de Negocio
En la operación de una terminal aduanal, la **VLAN de Operaciones (pedimentos)** y la **VLAN de Administración (Nóminas/RRHH)** deben estar aisladas para reducir el dominio de broadcast y mejorar la seguridad, permitiendo comunicación solo a través de una puerta de enlace (Gateway) controlada.

**Objetivo** Implementar la arquitectura "Router-on-a-Stick" para permtir el flujo de datos eficiente entre departamentos

## 2. Arquitectura y Segmentación
Se definieron los siguientes segmentos de red para la sucursal:

| Departamento | VLAN | Interfaz Lógica | Dirección IP (Gateway) | Máscara |
| :--- | :---: | :--- | :--- | :--- |
| **Operaciones** | 10 | G0/0.10 | 192.168.10.1 | 255.255.255.0 |
| **Administración** | 20 | G0/0.20 | 192.168.20.1 | 255.255.255.0 |

