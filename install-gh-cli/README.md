
# Instalacion y configuracin inicial:

* [ ] Confirma que tengas `git` en tu maquina.
* [ ] Nos dirigimos a la pagina oficial de GitHub CLI: https://cli.github.com/
* [ ] Dependiendo el sistema operativo que detecte en nuestro equipo nos dara las indicaciones de instalacion.
* [ ] En nuestro caso el sistema operativo es Ubuntu y estos son los comandos a ejecutar en terminal:
        * [ ] `sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-key C99B11DEB97541F0`
        * [ ] `sudo apt-add-repository https://cli.github.com/packages`
        * [ ] `sudo apt update`
        * [ ] `sudo apt install gh`

##### En caso de errores de instalacion:
        * Mas informacion en: https://github.com/cli/cli/blob/trunk/docs/install_linux.md
        * Para la instalacion en otros sistemas: https://github.com/cli/cli#installation
        * Nota: Esta instalacion es sencilla en caso de un error abrir un Issue.

#### GH completion en la CLI:

* [ ] Instalar `gh completion` esto principalmente para usuarios de `zsh`. 
* [ ] En tu archivo `~/.zshrc` debes tener agregado las siguientes lineas al final del archivo:
  * [ ] `autoload -U compinit`
  * [ ] `compinit -i`
* [ ] Ejecutar en tu terminal el siguiente comando: `gh completion -s zsh > /usr/local/share/zsh/site-functions/_gh`
* [ ] Prueba el autocompletado en terminal. Debe usar la tecla `tab` para auto completado.
* [ ] Si eres usuario Windows este tema puede traer dificultad actualmente este issue esta abierto: https://github.com/cli/cli/issues/695


#### Configuracion `auth` y `config` basica de GH CLI:

* [ ] Autentificacion con `github` desde la CLI: `gh auth login`
* [ ] Te presentara 2 opciones elegir `GitHub.com`, recuerda usando las `flechas direcionales ` ↑ ↓ luego presiona `enter`.
* [ ] Completa los pasos siguientes, recomiendo la opcion del Buscador y colocar el codigo.
* [ ] Elige tu protocolo de conexion de preferencia en nuestro caso `https` con: `gh config set -h github.com git_protocol https`
* [ ] Revisa el estado de authenticacion con: `gh auth status`
* [ ] Pudes desconectarte con: `gh auth logout`
* [ ] Te pedira confirmar si deseas salir con `(y/n)`: `y` si o `n` no.
* [ ] Puedes refrescar tu auteticacion usando un codigo igual que el login: `gh auth refresh`
* [ ] Establece tu editor por defecto en nuestro caso usaremos `vim` comando: `gh config set editor vim`
* [ ] Confirmar mi configuraciones de editor con: `gh config get editor` debe retornar `vim`
        * Las `key` de configuracion validad son:  
          1. `editor`  
          2. `pager`  
          3. `prompt`  
          4. `git_protocol` 