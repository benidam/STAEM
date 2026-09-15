<div align="center">

# 🎮 STAEM — Desktop Game Library Manager

**Simulador de gestión de biblioteca de videojuegos con persistencia en BBDD**

![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![Jackson](https://img.shields.io/badge/Jackson-JSON-black?style=for-the-badge)
![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)

</div>

---

##  El Problema que Resolvemos

Los jugadores actuales tienen su biblioteca fragmentada en múltiples plataformas (Steam, Epic, GOG) sin una forma unificada de gestionar su progreso de forma local y privada. **STAEM** resuelve esto centralizando la gestión mediante una arquitectura cliente-servidor sencilla utilizando Java y MySQL.

##  Core Features (Bajo el capó)

<details>
<summary>📂 Gestión Completa (CRUD)</summary>

- Lógica de negocio robusta en Java para instanciar, añadir, modificar y persistir datos de los videojuegos en la biblioteca.
- Motor de filtrado por categoría, nombre o estado.
</details>

<details>
<summary>⏱ Tracking de Progreso y RIR</summary>

- Estados dinámicos: `Jugado`, `En progreso`, `Pendiente`.
- Generación de estadísticas y visualización rápida del estado de cada título.
</details>

<details>
<summary>👤 Autenticación y Perfiles Aislados</summary>

- Sistema de registro y login.
- Relación 1:N en la base de datos MySQL para que cada usuario tenga su biblioteca, reseñas y configuraciones totalmente aisladas.
</details>

---

##  Despliegue y Ejecución

A diferencia del entorno de desarrollo clásico (Eclipse/IntelliJ), el proyecto está preparado para el usuario final.

**Opción 1: Ejecutable (Usuarios Windows)**
1. Descarga `STAEM-v1.exe` desde la raíz.
2. Ejecuta directamente (la conexión a la BD debe estar configurada en el entorno).

**Opción 2: Compilación manual**
```bash
git clone [https://github.com/benidam/STAEM.git](https://github.com/benidam/STAEM.git)
# Configurar dependencias de Jackson y el conector de MySQL
# Compilar y ejecutar Main.java
```

**El Equipo y mi Contribución**

## Este proyecto fue desarrollado bajo una simulación de entorno ágil por: Manuel Campos, Álvaro Benítez, Víctor Aguilera y Alejandro Bernal.


Mi enfoque técnico en el repositorio (Álvaro Benítez):

Configuración del empaquetado final (.exe) para despliegue nativo.

Resolución de conflictos en el control de versiones (Git).

Refactorización de lógica de backend en Java.
