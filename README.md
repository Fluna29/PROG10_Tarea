Descripción funcional
El objetivo de esta tarea es crear un programa sencillo que permita editar el contenido de un archivo de texto, guardar su contenido y crear un nuevo fichero de texto de forma similar a la aplicación del bloc de notas.

Cuando el programa se inicie mostrará una pantalla inicial similar a esta:



El menú Archivo contendrá a su vez las siguientes opciones:


El menú Ayuda contendrá a su vez la siguiente opción:


Inicialmente el contenido de la caja de texto que ocupa la mayor parte de la pantalla estará vacío y el título de la ventana será “<Fichero no guardado>”. El usuario podrá escribir cualquier texto dentro de la caja de texto varias líneas:


A continuación se describe lo que debe hacer cada una de las opciones del menú:

1. Menú Archivo→ Crear
Cuando se seleccione esta opción el contenido que hubiera en la caja de texto principal se borrará y el título de la ventana pasará a ser “<Fichero no guardado>” independientemente del que tuviera.

2. Menú Archivo → Abrir
Cuando se seleccione esta opción aparecerá un cuadro de diálogo de selección de ficheros que permitirá al usuario seleccionar un fichero de texto para ser mostrado en la aplicación.


Si el usuario pulsa el botón “Cancel” o la X de la esquina superior derecha no se hará nada, pero si pulsa el botón “Open” se mostrará el contenido del fichero seleccionado en la caja de texto multilínea y el título de la ventana cambiará para mostrar la ruta completa del fichero seleccionado.


3. Menú Archivo→ Guardar
Cuando se seleccione esta opción si ya hay un fichero abierto tras usar la opción Abrir o ya guardado con esta opción o la opción “Guarda Como” simplemente se escribirá todo el contenido de la caja de texto en el fichero como un fichero de texto. Si no hay un fichero abierto, se solicitará seleccionar un fichero para guardar el contenido actualmente mostrado en la caja de texto:


Si en este cuadro de selección se pulsa el botón “Cancel” o la X de la esquina superior derecha no se hará nada, pero si pulsa el botón “Save” se escribirá el contenido de la caja de texto multilínea en el fichero seleccionado sobreescribiendo cualquier contenido previo y el título de la ventana cambiará para mostrar la ruta completa del fichero seleccionado.

4. Archivo→ Guardar Como
Cuando se seleccione esta opción se hará exactamente el mismo comportamiento que en la opción “Guardar” pero como si no hubiera ningún archivo abierto.

5. Archivo → Salir
Cuando se seleccione esta opción se pedirá se mostrará al usuario una ventana de confirmación indicando si está seguro que quiere salir de la aplicación:



Si se pulsa el botón “No” la X de la esquina superior derecha no se hará nada. Si se pulsa el botón “Yes” se cerrará la ventana principal de la aplicación y finalizará.

6. Ayuda → Acerca de
Cuando se seleccine esta opción se mostrará una ventana con el nombre de la aplicación así como el nombre y apellidos del alumno que ha hecho la práctica:


Descripción técnica
Para mostrar cuadros de diálogo puedes consultar este enlace.

Para mostrar cuadros de selección de ficheros puedes consultar este enlace.

Para finalizar la aplicación desde la opción de menú de la Salir asegúrate de usar estas 2 líneas de código:

setVisible(false);

System.exit(0);
