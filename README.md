# Plantilla para usar LaTex en Visual Code Studio (Sistema Linux)

## Guía para LaTex en Visual Code Studio

### Configuración básica
- **Instalar Visual Studio Code** <br>
  Accede a [Instalar VSC para Linux](https://code.visualstudio.com/docs/setup/linux) y seguir los pasos
- **Instalar extensiones en VSC** <br>
  `Ctrl + Shift + X` Accedes a extensiones y seleccionas **LaTex Workshop** de James Yu <br>
- **Instalar paquetes en Linux** <br>
  Al no usar esta vez un compilador online tenemos que instalar los paquetes necesarios por nuestra cuenta <br>
  `sudo apt install texlive-full -y` para los paquetes de LaTex

### Recomendación
- Al tener cuenta de estudiante, el **Copilot de Github** se puede usar gratuitamente <br>
  En caso de querer usarlo, instalar **Github Copilot** y **Github Copilot Chat** en el apartado de extensiones <br>
  Para conectar con su cuenta de estudiante, sería clickear en tu perfil, y en el apartado de `setting`, ir a <br>
  la parte de `Emails` y añadir tu cuenta de estudiante
- `Ctrl + S` para guardar/compilar <br>
- `Ctrl + Alt + V` para visualizar <br>
- Si tienes el `main.pdf` abierto, al compilar puedes ver los cambios directamente en el PDF <br>
- `Ctrl + Alt + X` abrirá una ventana asociada al compilador de Latex con snippet abajo izquierda <br>
- `Ctrl + I` para abrir **Copilot**(en caso de habérselo instalado) <br>
- **(Muy recomendable)** Para una mejor visualización del entorno, `Ctrl + ,` para abrir configuración <br>
  Para que a la anchura de 80 caracteres le aparezca una línea de delimitación y se ajuste automáticamente, busca en configuración **rulers** y abre **Edit in setting.json**, luego añade tras `"workbench.colorTheme": "Default Light Modern",` lo siguiente: <br>
    `"editor.rulers": [80],` <br>
    `"editor.wordWrap": "wordWrapColumn",` <br>
    `"editor.wordWrapColumn": 80,` <br>
- **(Muy recomendable)** Configure la salida de los archivos de compilación a la carpeta, pulse `Ctrl + ,` para abrir configuración <br>
  y busque `Latex: Out Dir` y cambie la salida por `./build`. Una vez compilado el proyecto (con botón de build o `Ctrl + Alt + B`) la salida en formato pdf se verá en la carpeta [build](https://github.com/L-51/Plantilla-Latex-VSC/tree/main/build) <br>
  llamado [main.pdf](https://github.com/L-51/Plantilla-Latex-VSC/blob/main/build/main.pdf)

## Conectar con el repositorio Git
1. Instalación de **Git** si no lo tenían previamente instalado, `sudo apt install git -y` <br>
2. Configurar tu usuario y correo: <br>
   `git config --global user.name "Tu Nombre"` <br>
   `git config --global user.email "tuemail@dominio.com"` <br>
3. Accede a la carpeta donde quieras tener este proyecto guardado y clónalo escribiendo en la terminal de VSC: <br>
   `git clone https://github.com/L-51/Plantilla-Latex-VSC` <br>
4. Abre la carpeta usando **OpenFolder** de VSC o clic derecho → abrir con **code** <br>
5. Tras realizar un cambio o recibir una modificación hecha por otro usuario, abre control de código con `Ctrl + Shift + G`. Para guardar cambios, escribe un mensaje de commit y realiza **commit** con `Ctrl + Enter`. Para subir al repositorio, usa **push**, y para recibir cambios, usa **pull**.

## Organización del proyecto (Hay texto de ejemplo en los ficheros)
- **bibliografia** Aquí guardará las referencias en el fichero [ref.bib](https://github.com/L-51/Plantilla-Latex-VSC/blob/main/bibliografia/ref.bib) <br>
- **build** Aquí guardará los archivos temporales a la hora de la compilación y el [pdf de salida](https://github.com/L-51/Plantilla-Latex-VSC/blob/main/build/main.pdf) <br>
- **config** Aquí están los [paquetes](https://github.com/L-51/Plantilla-Latex-VSC/blob/main/config/packages.tex) que usarás y [comandos](https://github.com/L-51/Plantilla-Latex-VSC/blob/main/config/command.tex) <br>
- **secciones** Carpeta con las distintas secciones que forman parte del trabajo <br>
- **images** Carpeta de imágenes del proyecto <br>
- [**portada.tex**](https://github.com/L-51/Plantilla-Latex-VSC/blob/main/portada.tex) Contiene la portada del trabajo en LaTeX <br>
- [**main.tex**](https://github.com/L-51/Plantilla-Latex-VSC/blob/main/main.tex) El main donde se incluirá todo <br>
- [**.gitignore**](https://github.com/L-51/Plantilla-Latex-VSC/blob/main/.gitignore) Útil cuando crees un repositorio y hayas configurado guardar los archivos de compilación en [build](https://github.com/L-51/Plantilla-Latex-VSC/tree/main/build)

---

## ⚠️ Recomendación:
Se recomienda que cada usuario solo edite la parte que le corresponda, salvo correcciones, para evitar **sobreescritura** del trabajo de otros
