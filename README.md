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


##### En caso de errores de instalacion:
        

#### GH completion en la CLI:

#### Configuracion `auth` y `config` basica de GH CLI:

 
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








