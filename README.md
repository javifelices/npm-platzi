# [Curso de Gestión de Dependencias y Paquetes con NPM](https://platzi.com/clases/npm/)


## Artículos

- [Terminal de Linux | Manz](https://terminaldelinux.com/terminal/)

- [https://medium.com/jmtorres/servicios-y-demonios-en-linux-a424366336ac](https://medium.com/jmtorres/servicios-y-demonios-en-linux-a424366336ac)

- [NPM (Node Package Manager) | Manz](https://lenguajejs.com/npm/)

- [NPM Tutorial | Coding Potions](https://codingpotions.com/npm-tutorial)

- [¿Qué es Node.js? | Devcode](https://devcode.la/blog/que-es-nodejs/)

- [¿Qué es npm? | Devcode](https://devcode.la/blog/que-es-npm/)

- [https://www.hamrodev.com/es/desarrollo-apps/como-funcionan-dependencias-npm](https://www.hamrodev.com/es/desarrollo-apps/como-funcionan-dependencias-npm)

- [What is npm? A Node Package Manager Tutorial for Beginners](https://www.freecodecamp.org/news/what-is-npm-a-node-package-manager-tutorial-for-beginners/)

- [npm Cheat Sheet - Most Common Commands and nvm](https://www.freecodecamp.org/news/npm-cheat-sheet-most-common-commands-and-nvm/)

- [5 npm Tips and Tricks to Help You Boost Your Productivity](https://www.freecodecamp.org/news/5-npm-tips-and-tricks/)

- [These NPM tricks will make you a pro](https://www.freecodecamp.org/news/10-npm-tricks-that-will-make-you-a-pro-a945982afb25/)

- [A guide to NPM version constraints for Rubyists | rossta](https://rossta.net/blog/npm-version-constraints-for-rubyists.html)

- [Resolving EACCES permissions errors when installing packages globally](https://docs.npmjs.com/resolving-eacces-permissions-errors-when-installing-packages-globally)

- [Different types of dependencies in a Node.js application explained](https://javascript.plainenglish.io/what-the-dependency-types-of-dependencies-in-a-node-js-application-explained-904a5424fbd3)

- [A Comprehensive Beginner’s Guide To NPM](https://www.tabnine.com/blog/a-comprehensive-beginners-guide-to-npm/)

- [npm-uninstall](https://docs.npmjs.com/cli/v6/commands/npm-uninstall)

- [npm uninstall –no-save does not work with devDependencies](https://npm.community/t/npm-uninstall-no-save-does-not-work-with-devdependencies/1039)

- [https://docs.npmjs.com/cli/v7/commands/npm-prune](https://docs.npmjs.com/cli/v7/commands/npm-prune)

- [npm-check](https://www.npmjs.com/package/npm-check)

- [package-lock.json](https://docs.npmjs.com/cli/v7/configuring-npm/package-lock-json)

- [Semantic Versioning](https://semver.org/)

- [¿Qué es versionamiento semántico?](https://fperez217.medium.com/qu%C3%A9-es-versionamiento-sem%C3%A1ntico-bf495b9eb028)

- [¿Cómo funcionan las versiones en NPM?](https://platzi.com/tutoriales/1763-npm/8399-como-funcionan-las-versiones-en-npm/)

- [About semantic versioning](https://docs.npmjs.com/about-semantic-versioning)

- [npm-shrinkwrap](https://docs.npmjs.com/cli/v7/commands/npm-shrinkwrap)

- [Scripts de NPM](https://lenguajejs.com/npm/administracion/scripts-de-npm/)

- [scripts](https://docs.npmjs.com/cli/v7/using-npm/scripts)

- [Diferencias entre librerías y frameworks | Viewnext](https://www.viewnext.com/diferencias-entre-librerias-y-frameworks/)

- [NPM | Notion por @Sstark97 (Aitor Santana)](https://keen-nannyberry-2b8.notion.site/NPM-7560cea59ece4a6c8dd939d24057fd6e)

[Licnecia de Software | Wikipedia](https://es.wikipedia.org/wiki/Licencia_de_software)

- [Introducción a los diferentes tipos de licencias de código abierto y software libre | Universo Abierto](https://universoabierto.org/2015/12/20/introduccion-a-los-diferentes-tipos-de-licencias-de-codigo-abierto-y-software-libre/)

## Vídeos

- [Protege tu código usando licencias de software | Platzi](https://www.youtube.com/watch?v=eWtjgfzpt6Y)

- [Curso Básico de Licencias de Software | SuGE3K](https://www.youtube.com/playlist?list=PLyLcPK3h0D7CJ4QT0wLsWFzlbUTq010kB)

## Recursos

![Infografía de comandos NPM](https://i.imgur.com/xh4Jtbm.jpg)

![NPM Notas Curso](https://i.imgur.com/PcIovO2.jpg)

![Recortable de comandos NPM](https://i.imgur.com/2VnQZ0z.jpg)

![Semantic Versioning](https://i.imgur.com/KZXk9g6.jpg)

> Puedes también especificar scripts con el prefijo “**pre**” que se ejecutarán automáticamente antes del comando que ejecutaste. Por ejemplo, si defines el comando **build** y **prebuild**, cuando corras `npm run build` el comando **prebuild** se ejecutará primero. Esto sirve para poder ejecutar tareas que hagan algún tipo de preparación necesaria para correr el comando principal.

> Sin embargo, hay que hacer notar que si el comando **pre** falla (retorna un valor que no es 0) el comando principal no se ejecutará. Esto es algo bueno ya que si nuestro proceso de preparación no se realiza de forma exitosa, puede que tengamos problemas al querer ejecutar la tarea principal.

> En algunas ocaciones, sin embargo, la tarea previa puede fallar sin que eso afecte la ejecución de la tarea principal. En esos casos puedes usar `|| exit 0` para retornar 0:

```
"presass-build": "(rm css/*.css; rm css/*.css.map) || exit 0"
```

> Ese es un ejemplo de un comando que hice hace un tiempo. **rm** puede fallar si el directorio css está vacio, y en ese caso no hay problema, la tarea principal puede funcionar sin ningún problema ya que **presass-build** tiene el propósito de vaciar ese directorio.

>Algo que también faltó mencionar es que `npm run` agrega el directorio `./node_modules/bin/` al **PATH**, de modo que para ejecutar un comando no es necesario agregar la ruta completa.

>Esto es porque en realidad el binario está ubicado en `node_modules/bin/`.
