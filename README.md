# Plantilla para usar LaTex en Visual Code Studio
## Guía para LaTex en Visual Code Studio
- **Instalar Visual Studio Code** <br>
  Accede a [Instalar VSC para Linux](https://code.visualstudio.com/docs/setup/linux) y seguir los pasos
- **Instalar extensiones en VSC** <br>
  `Ctrl + Shift + X` Accedes a extensiones y seleccionas **LaTex Workshop** de James Yu <br>
- **Instalar paquetes en Linux** <br>
  Al no usar esta vez un compilador online tenemos que instalar los paquetes necesarios por nuestra cuenta <br>
  `sudo apt install texlive-full -y` para los paquetes de LaTex
- **Recomendación** <br>
  * Al tener cuenta de **UGR**, el **Copilot de Github** se puede usar gratuitamente<br>
    En caso de querer usarlo, instalar **Github Copilot** y **Github Copilot Chat** en el apartado de extensiones
  * `Ctrl + Alt + B` para compilar
  * `Ctrl + Alt + V` para visualizar
  * `Ctrl + Alt + X` le abrirá una ventana asociado al compilador de Latex y abajo izquierda con snippet
  * `Ctrl + I` para abrir **Copilot**(en caso de haberselo instalado)
  * **(Muy recomendable)** `Ctrl + ,` para abrir configuración y aquí hay un par de cosas interesantes que destacar:<br>
     Para que a la anchura de 80 caracteres le aparezca una línea de delimitación y que si llegas a ese tope <br>
     se ajuste automáticamente busca en configuración **rulers** y abrir **Edit in setting.json**, luego <br>
     añadir tras `"workbench.colorTheme": "Default Light Modern",` lo siguiente: <br>
     `"editor.rulers": [80],` <br>
     `"editor.wordWrap": "wordWrapColumn",` <br>
     `"editor.wordWrapColumn": 80,` <br>
  * **(Muy recomendable)** Configure la salida de los archivos de compilación a la carpeta, pulse `Ctrl + ,` para abrir configuración <br>
    y busque `Latex: Out Dir` y cambié la salida por `./build`
  * Una vez compilado el proyecto sea dándole al botón de `build` o pulsando `Ctrl + Alt + B` la salida en formato <br>
    pdf se verá en la carpeta [build](https://github.com/L-51/Prac_2_Algoritmica/tree/main/build) llamado [main.pdf](https://github.com/L-51/Prac_2_Algoritmica/blob/main/build/main.pdf)
## Conectar con el repositorio Git
1. Instalación de **Git** si no lo tenián previamente instalado, `sudo apt install git -y`
2. Configurar tu usuario y correo: <br>
   `git config --global user.name "Tu Nombre"` <br>
   `git config --global user.email "tuemail@dominio.com"`
3. Accede a la carpeta donde quieras tener este proyecto guardado y clónalo escribiendo en la terminal <br>
   de VSC y poner `git clone https://github.com/L-51/Prac_2_Algoritmica.git`
4. Abre la carpeta usando **OpenFolder** de VSC o la carpeta que te interesa hacer _click derecho_ y abrir con <br>
   y escribir **code**
5. Tras realizar un cambio o recibir una modificación hecha por otro usuario, abrir control de código con <br>
   `Ctrl + Shift + G`. Para guardar cambios escriba un mensaje de su última modificación y realice un **commit** <br>
   o `Ctrl + Enter` y si quieres subirlo al repositorio realice push que estará al lado de _GRAPH_ _auto_ el <br>
   penúltimo símbolo que al pasar el cursor verás **push**, y al su izquierda estará **pull** para recibir cambios
## Organización del proyecto
- **bibliografia** Aquí guardará las referencias en el fichero [ref.bib](https://github.com/L-51/Prac_2_Algoritmica/blob/main/bibliografia/ref.bib)
- **build** Aquí guardará los archivos temporales a la hora de la compilación y el [pdf de salida](https://github.com/L-51/Prac_2_Algoritmica/blob/main/build/main.pdf)
- **config** Aquí está los [paquetes](https://github.com/L-51/Prac_2_Algoritmica/blob/main/config/packages.tex) que usaremos y [comandos](https://github.com/L-51/Prac_2_Algoritmica/blob/main/config/command.tex)
- **ejercicios** Aquí es donde está los dinstintos ejercicios que se incluirá en el trabajo
- **images** Carpeta de las imágenes que se usará para el proyecto
- [**portada.tex**](https://github.com/L-51/Prac_2_Algoritmica/blob/main/portada.tex) Esta es la portada
- [**main.tex**](https://github.com/L-51/Prac_2_Algoritmica/blob/main/main.tex) El main donde se incluirá todo
---  
## ⚠️Recomendación:
Se recomienda que cada usuario solo edite la parte que le corresponda salvo correcciones para evitar **sobreescritura** del trabajo de otros
