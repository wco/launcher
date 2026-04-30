# WOW-COLOMBIA Launcher

Launcher oficial de [WOW-COLOMBIA](https://www.wow-colombia.com) — requerido para jugar.

## Descarga

| Archivo | Descripción |
|---------|-------------|
| [wow-colombia-pack.zip](https://github.com/wco/launcher/releases/download/v3.4.1/wow-colombia-pack.zip) | **Paquete completo** (recomendado): launcher + desbloqueador |
| [wow-colombia.exe](https://github.com/wco/launcher/releases/download/v3.4.1/wow-colombia.exe) | Solo el launcher |
| [wow-colombia.zip](https://github.com/wco/launcher/releases/download/v3.4.1/wow-colombia.zip) | Launcher comprimido (clave: `wowco`) |

> Contraseña del ZIP: `wowco`

## Instalación

1. Descarga **wow-colombia-pack.zip** y ábrelo (contraseña: `wowco`)
2. Extrae **todos los archivos** en la carpeta donde está tu **Wow.exe**
3. Ejecuta **iniciar-wow-colombia.bat**
4. Te pedirá permisos de administrador → haz clic en **Sí**
5. El script desbloquea el launcher automáticamente y abre el juego

> Las siguientes veces puedes abrir directamente `wow-colombia.exe` o seguir usando `iniciar-wow-colombia.bat`. El launcher se actualiza automáticamente.

## Contenido del paquete

| Archivo | Función |
|---------|---------|
| `wow-colombia.exe` | Launcher principal con auto-actualización |
| `iniciar-wow-colombia.bat` | Iniciador: desbloquea y lanza el launcher |
| `desbloquear-wow-colombia.bat` | Wrapper del desbloqueador |
| `desbloquear-wow-colombia.ps1` | Script universal de desbloqueo (Windows 7-11) |

## ¿Qué hace el desbloqueador?

Windows bloquea aplicaciones sin firma digital. El script `iniciar-wow-colombia.bat` desactiva automáticamente estas protecciones para el launcher:

- Smart App Control (Windows 11)
- SmartScreen y marca de descarga de Internet
- Exclusión en Windows Defender
- Reglas de firewall para el juego
- Compatibilidad y permisos de ejecución

Compatible con Windows 7, 8, 8.1, 10 y 11.

## Auto-Actualización

Integrada desde v3.0.8. Cuando hay una nueva versión disponible, el launcher la descarga y aplica automáticamente mostrando un diálogo con notas de versión y barra de progreso.

## Novedades v3.4.1

- Mejoras internas de detección y estabilidad.
- Correcciones menores.

## Advertencia de SmartScreen

Windows puede mostrar una alerta de SmartScreen al ejecutar el launcher por primera vez. Esto es normal para aplicaciones nuevas sin firma digital. Haz clic en "Más información" → "Ejecutar de todas formas", o usa el desbloqueador incluido en el paquete.

## SHA256

```
wow-colombia.exe       4038fd6f75879c7731b7210f6bf5155a76f2a72a45ca06df235fba0356d479d1
wow-colombia.zip       23b8358fa7dd64731193ac0335f4d5f78a1e3fed0f5b8629bb7d5529726989b5
wow-colombia-pack.zip  44d6db51677daa886fbf1ca70a1197282e75e5b943e0a164ddb08867ba6db1c5
```

## Requisitos

- Windows 7/8/10/11
- WoW 4.3.4 instalado
- Cuenta activa en WOW-COLOMBIA

## ¿Necesitas ayuda?

- **Discord**: [dc.wow-colombia.com](https://dc.wow-colombia.com)
- **Errores comunes**: [wow-colombia.com/post/errores-comunes](https://www.wow-colombia.com/post/errores-comunes)
- **Modo offline**: [wow-colombia.com/post/launcheroffline](https://www.wow-colombia.com/post/launcheroffline)
- **Foros**: [foros.wow-colombia.com](https://foros.wow-colombia.com)
- **Email**: info@wow-colombia.com
