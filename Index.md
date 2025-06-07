# Guía Completa: Configura tu Nodo de Pi Network

---

## 🚀 ¿Qué es Pi Network y por qué un Nodo?

Pi Network es una criptomoneda innovadora diseñada para ser accesible en dispositivos móviles, permitiendo a millones de personas participar en el espacio blockchain. A diferencia de las criptomonedas tradicionales que requieren hardware costoso, Pi busca la inclusión.

**¿Y un nodo?** Un nodo de Pi Network es un pilar fundamental para la descentralización y seguridad de la red. Al operar un nodo, tu computadora ayuda a:

* **Validar transacciones:** Confirmando las operaciones que ocurren en la blockchain de Pi.
* **Asegurar la red:** Contribuyendo a la integridad y resistencia de la blockchain.
* **Mantener la copia de la blockchain:** Almacenando una réplica de toda la historia de transacciones de Pi.

En pocas palabras, tu nodo es un eslabón vital que fortalece la infraestructura de Pi Network, permitiendo que la red crezca y funcione de manera estable para todos los pioneros.

---

## 🌳 Menú de Navegación (Guía Paso a Paso)

Usa este índice para saltar directamente a la sección que te interese.

* [**1. Requisitos Previos para tu Nodo**](#1-requisitos-previos-para-tu-nodo)
    * [**1.1. Hardware del Servidor (VPS)**](1.1-hardware-vps.md)
    * [1.2. Sistema Operativo](#12-sistema-operativo)
    * [1.3. Herramientas y Cuentas Necesarias](#13-herramientas-y-cuentas-necesarias)

* [**2. Configuración Inicial del VPS**](#2-configuracion-inicial-del-vps)
    * [2.1. Conexión Vía SSH](#21-conexion-via-ssh)
    * [2.2. Actualización del Sistema](#22-actualizacion-del-sistema)
    * [2.3. Configuración del Firewall (UFW)](#23-configuracion-del-firewall-ufw)

* [**3. Instalación de Docker**](#3-instalacion-de-docker)
    * [3.1. Pasos para la Instalación de Docker](#31-pasos-para-la-instalacion-de-docker)
    * [3.2. Verificación de Docker](#32-verificacion-de-docker)
    * [3.3. Añadir Usuario al Grupo Docker](#33-añadir-usuario-al-grupo-docker)

* [**4. Implementación del Nodo de Pi Network**](#4-implementacion-del-nodo-de-pi-network)
    * [4.1. Obtener la Imagen de Docker del Nodo Pi](#41-obtener-la-imagen-de-docker-del-nodo-pi)
    * [4.2. Ejecutar el Contenedor del Nodo Pi](#42-ejecutar-el-contenedor-del-nodo-pi)

* [**5. Vinculación del Nodo con tu Cuenta de Pi Network**](#5-vinculacion-del-nodo-con-tu-cuenta-de-pi-network)
    * [5.1. Desde la Aplicación Móvil de Pi](#51-desde-la-aplicacion-movil-de-pi)

* [**6. Monitoreo y Mantenimiento Básico**](#6-monitoreo-y-mantenimiento-basico)
    * [6.1. Comandos Útiles para Monitorear](#61-comandos-utiles-para-monitorear)
    * [6.2. Actualizaciones del Nodo](#62-actualizaciones-del-nodo)

* [**7. Solución de Problemas Comunes (FAQ)**](#7-solucion-de-problemas-comunes-faq)

---

### Puntos Clave de esta Estructura

1.  **Nombre del Archivo:** Lo nombrarás `index.md`.
2.  **Encabezado Principal (`#`):** Un título claro y llamativo para tu guía.
3.  **Sección de Introducción (`##`):** Aquí colocas la descripción del proyecto Pi Network y la importancia del nodo. Usa **emojis** y **negritas** para hacerlo más atractivo.
4.  **Menú de Navegación (`##`):** Este es tu "árbol".
    * Cada elemento principal (ej. "1. Requisitos Previos") es un enlace a un **encabezado de nivel 2** (`##`) en el mismo documento.
    * Los sub-elementos (ej. "1.1. Hardware del Servidor") son enlaces a **encabezados de nivel 3** (`###`) dentro de esa sección principal.
5.  **Enlaces Internos (`[Texto del Enlace](#id-del-encabezado)`):**
    * **GitHub (y la mayoría de los renderizadores de Markdown) automáticamente generan un `id` para cada encabezado.**
    * La regla general para el `id` es: el texto del encabezado en **minúsculas**, **espacios reemplazados por guiones `-`**, y **sin caracteres especiales** (a veces los números y puntos pueden ser problemáticos, por eso en el ejemplo usé `--` para los sub-encabezados).
    * **¡Muy importante!** Asegúrate de que los `id` en tus enlaces del menú (`#1-requisitos-previos-para-tu-nodo`) coincidan **exactamente** con los `id` generados por los encabezados reales más abajo en el documento.
6.  **Contenido Detallado:** **TODO el contenido de los pasos que te di previamente** (desde "Requisitos Previos" hasta "Solución de Problemas") lo pegarás *después* de este menú en el mismo archivo `index.md`, asegurándote de usar los encabezados `##` y `###` que coincidan con los enlaces del menú.

---

### Pasos Siguientes

1.  **Crea o Edita `index.md`:** En tu repositorio de GitHub, haz clic en "Add file" -> "Create new file" y nombra el archivo `index.md`. O si ya tienes un `README.md` y prefieres que sea tu principal, puedes renombrarlo a `index.md` (y luego, si quieres, crear un nuevo `README.md` más simple que solo apunte a `index.md`).
2.  **Pega la Estructura:** Copia y pega el ejemplo de estructura de `index.md` que te di arriba.
3.  **Añade el Contenido Detallado:** Debajo del menú, pega todo el texto detallado de los pasos que te di anteriormente, asegurándote de que tus encabezados (`##` y `###`) coincidan con los `id`s que usaste en los enlaces del menú.
4.  **Revisa los Enlaces:** Una vez guardado el archivo en GitHub, ábrelo en el navegador y haz clic en cada enlace del menú para asegurarte de que te lleva a la sección correcta. Si alguno no funciona, es probable que haya un error en el `id` (minúsculas, guiones).

Con esto, tendrás un `index.md` funcional, interactivo y muy fácil de usar para tus afiliados. ¡Será una guía excelente!
