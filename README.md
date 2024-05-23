# HTML Y CSS HERRAMIENTAS I : PEC 2- IMAGENES Y ANIMACIONES EN LA WEB

## LINK DEMO


## INSTALACIONES REALIZADAS

### BREW

```text
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
echo "export PATH=/opt/homebrew/bin:$PATH" >> ~/.zshrc
source ~/.zshrc

```

### NVM

```text
brew install nvm
mkdir ~/.nvm
echo "export NVM_DIR=~/.nvm\nsource \$(brew --prefix nvm)/nvm.sh" >> .zshrc
source ~/.zshrc

```

### NODE JS

```text
nvm install 20
nvm use 20.12.2
```

### PARCEL

```text
npm install --save-dev parcel
npm install --save-dev rimraf 
npm install npm-run-all --save-dev

```

### PACKAGE.JSON

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

### POST HTML

```text
npm i -D posthtml-include
/// Añadir archivo .posthtmlrc
```

## COMPILAR WEB

```text
npm start
```

## PREPARACIÓN DESPLIEGUE

```text
npm build
```
