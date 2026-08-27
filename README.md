# Agua Piazza

App de registro y monitoreo de consumo de agua para las 9 Piazzas.

Todo el proyecto es un solo archivo (`public/index.html`) con sus datos embebidos — no necesita servidor ni base de datos.

## Subir a GitHub

```
cd agua_piazza_deploy
git init
git add .
git commit -m "Agua Piazza"
```

Luego crea un repositorio vacío en https://github.com/new y conéctalo:

```
git remote add origin https://github.com/TU-USUARIO/TU-REPO.git
git branch -M main
git push -u origin main
```

## Subir a Firebase Hosting

1. Instala la herramienta de Firebase (una sola vez):
   ```
   npm install -g firebase-tools
   ```
2. Inicia sesión:
   ```
   firebase login
   ```
3. Reemplaza `TU-PROYECTO-FIREBASE` en el archivo `.firebaserc` con el ID real de tu proyecto (lo ves en la consola de Firebase, en el ícono de engranaje → Configuración del proyecto). Si aún no tienes un proyecto, créalo primero en https://console.firebase.google.com.
4. Publica:
   ```
   firebase deploy
   ```

Al terminar, la terminal te da la URL pública (algo como `https://TU-PROYECTO-FIREBASE.web.app`).

## Actualizar más adelante

Cada vez que tengas una versión nueva del `index.html`, reemplaza el archivo en `public/index.html` y repite:

```
firebase deploy
```

Y para GitHub:

```
git add .
git commit -m "actualización"
git push
```
