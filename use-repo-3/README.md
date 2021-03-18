
# Trabajando con `repo`:
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