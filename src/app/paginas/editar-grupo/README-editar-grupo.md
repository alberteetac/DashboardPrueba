# OBJETIVO: editar la información del grupo o sus alumnos de manera sencilla


<!-- editar-grupo.component.ts -->

La pantalla de editar-grupo será muy parecida a la de grupo. Por lo que el controlador y el html serán muy parecidos también. Volvemos a recibir el grupo seleccionado al iniciar el componente y los alumnos. También recuperamos el id del profesor del grupo.

La pantalla es parecida a editar-grupo, pero el funcionamiento es parecido a cuando creabamos equipo y volviamos hacia atrás en el segundo paso (porque editabamos) o al segundo paso (porque agregabamos alumnos).

Los parámetros de nombreGrupo y descripcionGrupo los asociamos a los dos inputs que tenemos. Al principio serán iguales a al nombre y descripcion actual del grupo, por eso los igualamos.


# EditarGrupo()

Hace un PUT introduciendo el nombre, descripcion, identificador del profesor y del grupo.

# AlumnosDelGrupo())

Utilizaremos esta función para hacer un GET de los alumnos del grupo para actualizar la tabla en caso de eliminar/agregar algun alumno.

# AbrirDialogoAgregarAlumnos()

Al igual que en el segundo paso de cuando creabamos un grupo, tendremos un botón que abre el mismo diálogo. Con lo que le funcionamiento es el mismo (explicación README-agregar-alumno-dialog.md). Al cerrar el diálogo ejecutaremos la función AlumnosDelGrupo() para actualizar la tabla.



<!-- editar-grupo.component.html -->

El html es muy parecido al grupo.component.html. La explicación se encuentra en su README.


