# mapea-template
Facilite el uso de Ionic con VanillaJS gracias a esta plantilla y componentes web nativos

#### :warning: En construcción :warning:

## Empezando

**Requisitos previos**
* Node & npm: https://nodejs.org/en/download/
  - Version node: 10.20.1
  - Version npm: 6.14.13 
* Ionic CLI:
  - Version Ionic CLI: 6.16.3

  ```javascript
  npm i -g ionic
  ```
    
## Aplicación en desarrollo
```javascript
  ionic serve
```

## Variables de entorno
Establecer variables de entorno:

**_Linux_** (Terminal de comandos)

* export ANDROID_SDK_ROOT=/home/user/Android/Sdk/
* export PATH=${PATH}:$ANDROID_HOME/tools:$ANDROID_HOME/platform-tools

Aceptar licencias SDK:
* yes | /home/user/Android/Sdk/tools/bin/sdkmanager --licenses

Java8 en la ruta del sistema:
* export JAVA_HOME= /home/user/jvm/jdk1.8.0_231/
* export PATH=${PATH}:$JAVA_HOME

Instale Gradle y agréguelo a la ruta:
* export PATH=${PATH}:/home/user/gradle-6.7/bin

**_MacOS_** (Terminal de comandos)

Sustituir "export" por "let"

**_Windows_** 

Ir a "Menú de inicio > Sistema > Configuración avanzada del sistema > Opciones avanzada > Variables de entorno". Introducir las variables sin el "export"

## Generación de aplicaciones

* Cordova en modo "global":

  ```javascript
  npm i -g cordova
  ```
* Plataforma:

  ```javascript
  cordova platform add android --save
  ```
  
* Generar archivo: app-mapea-templates/platforms/android/app/build/outputs/apk/debug/app-debug.apk

  ```javascript
  ionic cordova build android
  ```
 
## Platafoma Andorid
Para crear paquetes de aplicaciones, consulte el documento oficial de Ionic:
* Android Setup: https://ionicframework.com/docs/developing/android

## ¡ IMPORTANTE !
Los componentes que tienen un mapa no pueden usar shadowDOM porque la importación de Mapea es global y no tendrá acceso al componente DOM
 
