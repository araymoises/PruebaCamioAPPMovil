# Instrucciones de uso

- Clonar repositorio.
```bash
git clone https://github.com/araymoises/PruebaCamioAPPMovil.git
```

- Abrir el proyecto con Android Studio.

- Conectar el dispositivo o encender el emulador para pruebas.

## Nota

En caso de querer usar la api localmente, en lugar de Heroku, encender la API y reemplazar la URL en /app/build.gradle
```java
buildTypes {
        debug {
            buildConfigField "String", "API_URL", '"http://IpDeLaPC:8000/api/"'
        }
        release {
            minifyEnabled false
            proguardFiles getDefaultProguardFile('proguard-android-optimize.txt'), 'proguard-rules.pro'
            buildConfigField "String", "API_URL", '"http://IpDeLaPC:8000/api/"'
        }
    }
}
```
