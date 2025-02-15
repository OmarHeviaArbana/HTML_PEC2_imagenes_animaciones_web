# Twenty one pilots site

<image style="box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 29px 0px;" src="src/img/miniatura.png" alt="Twenty one pilots site">

## Link

https://twentyonepilotssite.netlify.app

## Descripción

Desarrollo de un sitio web, de diseño y contenido libre sobre un grupo de música, implementando adecuadamente las técnicas de dirección de arte, clipping, imágenes responsive y animación web, y hacerlo de forma accesible. Aquí se presenta el resultado final tras diferentes mejoras de rendmientos

## Mejoras implementadas

- Mejora del rendimiento, gracias a que los recursos gráficos (imagenes y svg) han sido adaptados a al tamaño de pantalla y densidad de pixeles. Para ello, se han utilizado técnicas como imaganes adaptativas, imagenes responsive y dirección de arte.
  
- Introducción de diferentes animaciones para mejorar el dinamismo del sitio.
  
- Se introduce el nombre del grupo en la navbar y un recursos gráfico svg en el footer. Además en el footer, se modifican los links para dar acceso a las páginas del sitio.
  
- Revisión del responsive general del sitio.
  
- Se presenta de forma más amigable en link de netlify del sitio.

---

# Twenty one pilots site

## Description

Development of a website with free design and content about a music group, properly implementing techniques such as art direction, clipping, responsive images, and web animation, while ensuring accessibility. This is the final result after various performance improvements.

## Implemented Improvements

- Performance optimization: Graphic resources (images and SVGs) have been adapted to screen size and pixel density using techniques such as adaptive images, responsive images, and art direction.

- Enhanced animations: Various animations have been introduced to improve the site's dynamism.

- Navbar and footer updates: The band's name has been added to the navbar, along with an SVG graphic in the footer. Additionally, the footer links have been modified to provide access to different pages on the site.

- General responsiveness review: The site's responsiveness has been improved.
  
- Netlify link presentation: The Netlify site link is now displayed more clearly.

---

## Instalaciones necesarias / Required Installations

### Brew

```text
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
echo "export PATH=/opt/homebrew/bin:$PATH" >> ~/.zshrc
source ~/.zshrc

```

### Nvm

```text
brew install nvm
mkdir ~/.nvm
echo "export NVM_DIR=~/.nvm\nsource \$(brew --prefix nvm)/nvm.sh" >> .zshrc
source ~/.zshrc

```

### Node

```text
nvm install 20
nvm use 20.12.2
```

### Parcel

```text
npm install --save-dev parcel
npm install --save-dev rimraf 
npm install npm-run-all --save-dev

```

### Package Json

```text
{
  "name": "twenty-one-pilots-web",
  "source": "src/index.html",
  "browserslist": "> 0.5%, last 2 versions, not dead",
  "scripts": {
    "start": "npm-run-all clean parcel:dev",
    "build": "npm-run-all clean parcel:build",
    "parcel:dev": "parcel", 
    "parcel:build": "parcel build", 
    "clean": "rimraf dist .parcel-cache"
  },
  "devDependencies": {
    "npm-run-all": "^4.1.5",
    "parcel": "^2.12.0",
    "posthtml-include": "^2.0.1",
    "rimraf": "^5.0.5"
  }
}
```

### Post Html

```text
npm i -D posthtml-include
/// Añadir archivo .posthtmlrc
```

### Convertir imagenes a webp / Convert Images to WebP

```text
cwebp -q 100 src/img/presentacion/presentacion.png -o src/img/presentacion/presentacion.webp
```

### Compilar web / Compile the Website

```text
npm start
```

### Preparación despliegue / Deployment Preparation

```text
npm build
```
