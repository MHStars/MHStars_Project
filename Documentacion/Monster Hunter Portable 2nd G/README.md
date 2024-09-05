# Nephilim "Eclipse" - Documentación
## Monster Hunter Portable 2nd G

### 1. Desencriptación Completa

#### Desencriptación de DATA.BIN

**Requisito**: Instalar Java JDK v17 (versión utilizada para estas acciones)

```
java -jar mhtools.jar --dec-all \mhtools\data_bin\DATA.BIN \mhtools\data_bin\decrypted
```

- `mhtools.jar`: Herramienta para desencriptar
- `\mhtools\data_bin\DATA.BIN`: Ruta del archivo DATA.BIN
- `\mhtools\data_bin\decrypted`: Ruta de salida para los archivos desencriptados

### 2. Desencriptación de contenedores .pak

```
java -jar mhtools.jar --extract \mhtools\filename.pak 6
```

**Nota**: Los archivos .pak son contenedores de modelos 3D y sus texturas.

Ejemplo:
- `DATA.BIN\00\0058.pak`: Contiene el modelo 3D y las texturas del personaje femenino.

### 3. Desencriptación de contenedores .tmh

Para extraer:
```
java -jar mhtools.jar --extract \mhtools\filename.tmh 5
```

Para reconstruir:
```
java -jar mhtools.jar --rebuild \mhtools\carpeta_del_contenedor_desempacado 5
```

**Nota**: Los archivos .tmh son contenedores de texturas del juego, incluyendo mapas, HUD y menús.

Ejemplo:
- `DATA.BIN\00\0017.tmh`: Contiene texturas, posiblemente de alguna zona o interfaz de usuario.

---

Esta documentación proporciona los pasos básicos para desencriptar y manipular los archivos del juego Monster Hunter Portable 2nd G. Recuerda siempre hacer copias de seguridad antes de modificar cualquier archivo del juego.
