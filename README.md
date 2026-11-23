# 📺 DiPlay: CarPlay en tu pantalla Android (BYD) sin dongle — guía rápida

> 📚 **Colección / Coleção**: esta hoja forma parte de [cheatsheets](https://github.com/Ezra-Zhao/cheatsheets) — 100 hojas de referencia en un solo repositorio. / Esta folha faz parte de [cheatsheets](https://github.com/Ezra-Zhao/cheatsheets) — 100 folhas de referência em um só repositório. ⭐

[![Stars](https://img.shields.io/github/stars/shihabal3amri/DiPlay?style=social)](https://github.com/shihabal3amri/DiPlay/stargazers) ![License](https://img.shields.io/badge/licencia-MIT-green.svg) ![Languages](https://img.shields.io/badge/idiomas-ES%20%C2%B7%20PT-blue)

Apoyo y más: [GitHub Sponsors](https://github.com/sponsors/Ezra-Zhao) · [Gumroad — plantillas y cuadernos que uso](https://ezraflow28.gumroad.com) · [Ko-fi](https://ko-fi.com/ezra777zhao)

> 🌍 [Português](README.pt.md)

Una **guía de una sola página** sobre **DiPlay**: la app que convierte la pantalla Android de tu coche en un receptor de CarPlay, con cable o sin cable. Todo lo que necesitas para decidir si te sirve y conectarlo: compatibilidad real, los dos métodos de conexión en tres pasos y las advertencias del propio proyecto.

**Autor:** Ezra-Zhao · Octubre de 2026

Proyecto original: https://github.com/shihabal3amri/DiPlay · Descargas: https://github.com/shihabal3amri/DiPlay/releases · Web: https://shihabal3amri.github.io/DiPlay/

> **Nota de autoría:** esta es una guía original de síntesis, escrita con palabras propias a partir de la documentación pública del proyecto; no reproduce su texto. La compatibilidad citada es la que el proyecto declara en su README y su documento de compatibilidad (versión 0.2.21, vista previa pública).

---

## En 20 segundos

- DiPlay se instala **en el coche** (en la pantalla Android), **no en el iPhone**.
- **Sin dongle, sin jailbreak, sin Mac, sin cuenta y sin servidor de autenticación.** La autenticación de CarPlay es local.
- Funciona **con cable USB** o **inalámbrico**: Wi-Fi Direct, el hotspot del propio coche o la misma red Wi-Fi/LAN.
- El proyecto está **centrado en BYD (DiLink)**. En otras marcas puede funcionar, pero el autor declara que no tienen soporte.
- Es una **vista previa pública** (0.2.21), no un producto terminado ni certificado.

## Compatibilidad (lo verificado, sin adornos)

| Pieza | Qué dice el proyecto |
|---|---|
| Sistema de la pantalla | Android **7.0+ (API 24)** para instalar el APK. **Android 6.0 o anterior: no compatible.** |
| Condición previa | La unidad **debe permitir instalar APK**. Sin eso, nada de lo demás aplica. |
| Android 7.0–8.1 | El APK se instala, pero el proyecto indica que **aún no está confirmado en un vehículo real**. |
| Alcance principal | Coches **BYD con DiLink**. Evidencia citada por el proyecto: coche de desarrollo con DiLink 5.1, un BYD Tang con DiLink 5.0 e instalación desde cero validada en DiLink 4.0 / Android 10. |
| Otras marcas | **Sin soporte oficial**: el proyecto se centra en BYD y no promete corregir incompatibilidades de otras marcas. Hay informes comunitarios mixtos entre generaciones de DiLink; **no existe una lista certificada de modelos**. |
| iPhone | iPhone normal, **sin jailbreak**, con CarPlay activado. La compatibilidad exacta varía según modelo e iOS. |
| Inalámbrico | Wi-Fi Direct, hotspot del coche o Wi-Fi existente / misma LAN. En **Android 7.0–9**, Wi-Fi Direct usa una vía heredada que **depende del firmware**; en **Android 10+** se verifica la frecuencia negociada del grupo. |
| Recomendación del proyecto | El **hotspot integrado del coche** es la conexión recomendada: con Wi-Fi Direct, la búsqueda de redes del propio coche puede causar microcortes de audio. |
| Puerto USB | Tiene que ser un puerto **de datos**. Un puerto solo de carga no transmite nada y la conexión no arranca. |
| ADB | **No hace falta** para el CarPlay básico. Solo lo piden funciones opcionales (panel, batería, velocidad de rueda, vídeo en parado). |

## Conexión con cable (3 pasos)

1. **Instala DiPlay en la pantalla del coche**: descarga el APK desde la página de *Releases* del proyecto y permite la instalación de APK en la unidad.
2. **Conecta el iPhone a un puerto USB de datos** del coche con su cable.
3. **Abre DiPlay y elige CarPlay con cable**: la autenticación es local y la sesión arranca en la pantalla.

## Conexión inalámbrica (3 pasos)

1. **Instala DiPlay en la pantalla** (igual que arriba) y ábrelo.
2. **Activa el hotspot del coche** (la opción recomendada) o Wi-Fi Direct en la pantalla. Ojo: en Android 7–9, Wi-Fi Direct depende del firmware de cada unidad.
3. **Conecta el iPhone a ese hotspot o red** y elige CarPlay inalámbrico en DiPlay; deja activada la conexión automática a ese hotspot para que reconecte solo.

## Avisos honestos (léelos antes de instalar)

- **No es un producto certificado por Apple.** Sin afiliación ni respaldo de Apple o BYD: CarPlay es marca de Apple y el proyecto lo usa solo para describir la función.
- **Identidad de accesorio experimental:** el APK incluye una identidad recuperada de firmware público de Carlinkit; no es una identidad MFi nueva creada para DiPlay, y su clave privada incluida se puede extraer. Que futuras versiones de iOS la sigan aceptando **no está garantizado**.
- **Vista previa pública:** puede haber cortes de audio y comportamientos distintos según el firmware. El propio proyecto pide probar en la versión actual y reportar con su herramienta de diagnóstico.
- **Otras marcas = terreno no verificado:** fuera de BYD, si algo falla, el proyecto declara que no hay soporte ni planes de añadirlo.
- **Antes de perder una tarde:** confirma primero que tu unidad permite instalar APK y que tienes un puerto USB de datos; son los dos bloqueos más comunes.

## Enlaces

- Proyecto original: https://github.com/shihabal3amri/DiPlay
- Descargas (Releases): https://github.com/shihabal3amri/DiPlay/releases
- Documento de compatibilidad del proyecto: https://github.com/shihabal3amri/DiPlay/blob/main/docs/COMPATIBILITY.md
- Web del proyecto: https://shihabal3amri.github.io/DiPlay/

## Licencia

Esta guía se publica bajo licencia MIT (© 2026 Guangyi Zhao). DiPlay es un proyecto independiente de su autor, con licencia GPL-3.0; esta guía no forma parte de ese proyecto ni lo sustituye: para instalar, usa siempre los enlaces oficiales de arriba.
