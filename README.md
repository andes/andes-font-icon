# Webfont - Andes Desing Icons

Webfont de [Andes Design Icons](https://www.andes.gob.ar).

```
npm install @andes/icons
```

## Uso

Agregar en style.scss:

```scss
$adi-font-path: '~@andes/icons/fonts/';
@import '~@andes/icons/scss/andes-icons';
```

```html
<i class="adi adi-rup-semantic-plan">
```

## Agregar nuevo ícono

Diseñar los íconos [siguiendo esta guía](https://github.com/fontello/fontello/wiki/How-to-use-custom-images#importing-svg-images)

1. Instalar y correr Docker.

2. Sobre la consola, realizar: `npm run server`. Esta acción corre fontello en el navegador, se abre automáticamente en http://localhost:3000.

3. En fontello agregar íconos, cambiar configuraciones (nombres, etc).

4. Descargar el archivo config.json (dropdown rojo "Download webfont", arriba a la derecha) y reemplazarlo en la raíz de proyecto.

5. Considerar que fontello no se este ejecutando y sobre la consola, realizar: `npm run build`. Regenerar todo el paquete de íconos (lo hace usando el archivo config.json, previamente descargado).


6. Incrementar la versión package.json. Por ejemplo: "version": "1.1.17".

7. Hacer commit de los cambios.

8. Luego, crear un tag con la versión (git tag [NUEVA VERSION]), tiene que ser la misma que en package.json. Por ejemplo: `git tag 1.1.17`.

9. Hacer push de los cambios.

10. Públicar en npm la nueva versión de @andes/icons: 
- `npm login` (usando las credenciales de Andes)
- `npm publish` 