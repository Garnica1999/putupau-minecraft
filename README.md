# putupau-minecraft
Repositorio para alojar todo el servidor de minecraft de putupau, junto con sus configuraciones.

## Descripcion
Este repositorio es exclusivamente para el alojamiento del servidor de minecraft de putupau. Para aprovechar su reusabilidad, se crearán varias ramas (branch) las cuales tiene diversas funcionalidades.

Este servidor tiene función de crossplay habilitada. Jugadores de minecraft en PC, Bedrock, Consola y celular (Android y iOS) pueden jugar dentro de este servidor sin problemas. Esto hace que el servidor siempre tenga que estar en la última versión, y, adicionalmente, que no sea compatible para mods.

## Dependencias del servidor
- Paper 1.21.8
- Java JDK 21
- Puede usar este servidor con Spigot sin problema.

## Versión del servidor
- **Bedrock:** 1.21.101
- **Java:** 1.21.8
- **Repositorio:** 0.1.0.09.2025
    
## Cómo ejecutar?
Para ejecutar la versión de este repositorio, simplemente clone el repositorio completamente usando el siguiente comando:
```git clone https://github.com/Garnica1999/putupau-minecraft.git```
Posteriormente, cambiamos de rama usando el siguiente comando:
```git checkout develop/2025```
Para evitar errores de sincronziación y archivos faltantes, ejecutar el siguiente comando:
```git pull origin develop/2025```
Luego, sólamente basta con ejecutar el script `run.sh` o `run.fish` si tienes como shell a fish.
```
chmod +x ./run.sh
./run.sh
```
Cabe aclarar que estos scripts son para ejecutar el servidor en linux. Para windows puede utilizar:
```java -Xms2048m -Xms2048m -jar paper-1.21.8-50.jar nogui```

### Dependencias de ejecución.
Necesitas el JDK de Java 21 para ejecutar el servidor. Recomendamos OpenJDK para poderlo ejecutar. SI lo vas a ejecutar en Windows, asegurate de que tengas la variable de entorno `%JAVA_HOME%` y en el path la carpeta bin que está adentro de la variable anteriormente mencionada.

En caso de linux esto no es encesario. Generalmente los repositorios de paquetes que tienen los JDK ya crean las variables de entorno, y/o utilizan `/usr/bin` para guardar los binarios y que puedas ejecutar java desde consola sin problemas.

### Entornos de ejecución
Recomendamos alquilar un servidor dedicado para minecraft si no tienes muchos conocimientos para ejecutar aplicaciones y administración de servidores. Adicionalmente, si vas a manejar un servidor grande, también es una solución más elástica que armar tu propio servidor.

Si lo quieres hacer localmente lo puedes hacer siguiendo los puntos anteriores que están en este readme. Generalmente los proveedores de servidores de minecraft hacen este procedimiento de manera automática, esto hace que sea más facil para cualquier usuario crearse su propio servidor.

#### Servidores externos dedicados

Puede usar este repositorio para montar tu propio servidor. Tenga en cuenta que algunos proveedores maneja el archivo lanzador del servidor `.jar` así que necesita cargar todos los archivos excluyendo el archivo .jar.

Si quiere cargar mundo nuevo tenga en cuenta lo siguiente:
- **world**: Es el overworld, o mundo principal.
- **world_nether**: Es el mapa generado para el mundo del nether.
- **world_the_end**: Es el mapa generado para el mundo del End.
Solamente no suba la carpeta que no quiere que se cargue el mundo a su servidor. Cuando inicie el servidor, paper/spigot, o el gestor de servidor que tengas, no encontrará el mundo correspondiente y lo regenerará desde cero.

## Repositorio
Este repositorio guarda la versión en deesarrollo del servidor de minecraft corespondiente al año 2025.
    
### Ramas (Branch)
Las ramas de este repositorio describen mediante la siguiente especificación:
- **main**: Se encuentra la versión definitiva desplegada en el servidor host de minecraft. Esta rama no es modificable, y sólamente se puede modificar mediante pull request
- **develop/latest**: Esta rama se encuentra la última versión del servidor. Es decir, se encuentra el año más reciente actualizado. Si la última versión del servidor es del año 2025, **develop/latest** tendría una copia del servidor **develop/2025**
- **develop/{YEAR}**: En esta rama se encuentra la versión correspondiente al año donde se ha creado el servidor. POr ejemplo, en la rama **develop/2025** se encontraría el servidor que está en desarrollo para el año 2025.

## Colaboradores
- HardwareELite (administración)

