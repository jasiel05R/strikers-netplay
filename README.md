# Strikers Android — Netplay LAN (experimental)

Una modificación del port de **Super Mario Strikers** para Android que añade
**partida de 2 jugadores por el mismo WiFi**, un teléfono por jugador.

> Requiere tu propia copia del juego. **No incluye ningún archivo del juego.**

## Qué añade
- Netplay en red local (UDP, lockstep): solo se intercambian los controles.
- El host juega con el control 1 y quien se une con el control 2.
- Detección de desincronización y recuperación ante pérdida de paquetes.

**Estado: sin probar en teléfonos reales.** El protocolo se probó con un
juego simulado, pero falta confirmar que el juego sea 100 % determinista.

## Cómo compilar el APK
1. Pestaña **Actions** → **Build APK (netplay)** → **Run workflow**.
2. Espera ~30–60 min y descarga el artifact `strikers-netplay-apk`.

El proyecto está en `smstrikers-port-netplay.zip`; el workflow lo descomprime
y compila. Instrucciones de uso del netplay: `README-netplay.md` dentro del zip.

## Créditos
Este trabajo se apoya en el de otros:
- [Yannick Suter](https://github.com/yannicksuter) y colaboradores: la decompilación.
- [new-coke/strikers](https://github.com/new-coke/strikers): el port nativo y su versión Android.
- [encounter/aurora](https://github.com/encounter/aurora): capa gráfica y de entrada.
- [bylaws/libadrenotools](https://github.com/bylaws/libadrenotools): carga de drivers.

Super Mario Strikers es de Nintendo / Next Level Games. Proyecto de fans, sin afiliación.
