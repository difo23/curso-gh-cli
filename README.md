# Curso GitHub CLI

## Descripcion:
Curso básico del uso de GitHub CLI.

Repo oficial de GitHub CLI: 
https://github.com/cli/cli


### Git CLI and GitHub CLI son aliados:

Estas dos herramientas trabajan muy bien juntas, puedes aumentar drasticamente la eficiencia   
de tu trabajo  como desarrollador si aprendes a implementarlas correctamentamente.

## Objetivos del curso:

* Alcanzar un domino basico de la herramienta GitHub CLI. 
* Empezar a trabajar usando las ventajas de un programa CLI.
* Agilizar nuestro flujo de trabajo remoto con PR.
* Agilizar nuestro flujo de trabajo con los issues.

### Lista de tareas:

#### Instalacion:
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
 
#### Usando `help`:

Usar las ayudas con `help` es fundamental para dominar una herramienta de la CLI. Es bueno comprender 
la documentacion que se presenta.
* [ ] Usa ayuda para el comando para saber los comandos basicos de `gh` con: `gh --help`
* [ ] Confirma las variables de enviroment soportadas por `gh` comando: `gh enviroment`
* [ ] Lee la documentacion de ayuda para autenticacion con: `gh auth login --help`

#### Trabajando con `repo`:
* [ ] Clonar un proyecto de GitHub usando la CLI: `gh repo clone user-github/repo-name`
  * Ejm: `gh repo clone difo23/curso-gh-cli`
* [ ] Clonar un proyecto e inidica la carpeta donde deseas clonarlo: `gh repo clone user-github/repo-name <directory>`
  * Ejm: `gh repo clone difo23/curso-gh-cli ./nuevor_dir`
* [ ] Crea un nuevo repo en GitHub: 
  * [ ] Crea una carpeta local para tu proyecto con: `git init gh-create-project`
  * [ ] Luego luego muevete al proyecto creado con: `cd gh-create-project`
  * [ ] Finalmente puedes crear el repo remoto con: `gh repo createg`
  * [ ] Personaliza tu repo con el selector de opciones, el nombre por defecto del remoto es `origin`. 
  * [ ] Confirma que tu remoto sea agregado a tu repo con: `git remote -v`
  * [ ] Crea un fork y clonalo con el comando: `gh repo fork difo23/curso-gh-cli`
  * [ ] Puedes ver los repos que tienes creado o los repos de un colega usando: `gh repo list difo23` usa la tecla `q` para salir de la lista.
  
#### Trabajando con `issues`:

#### Trabjando con `pr`:
#### Trabjando con `release`:
#### Trabajando con `gist`:

#### Agregando `alias` para los `pr`, `gist`, `help`, `release`, `repo`, `secret`, `ssh-key`  y `issue`:








