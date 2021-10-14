
## CLIMEX00CP001 Creación de un proyecto.

### Descripción

Crear un nuevo proyecto llamado **P1** y comprobar que el proceso se ha realizado con éxito.

### Prerrequisitos

1. Tener instalado una versión de python igual o superior a la versión 3.8.
2. Tener instalado un interprete python o en su defecto utilizar la shell propia de la instalación.
3. Tener instalado una versión de la herramienta CLINMEX igual o superior a la versión 0.5.


### Pasos

1. Abrir el interprete de python.
2. Escribir el comando *import climex* y ejecutarlo.
3. Escribir el comando *P1=climex.Project(P1)* y ejecutarlo.
4. Escribir el comando *P1* y ejecutarlo.

### Resultado esperado

Como resultado de la secuencia de pasos anteriores se obtiene por pantalla en el interprete de python
un archivo **JSON** con la siguiente estructura.

{

	"created": "(fecha y hora de la creación del proyecto)",
	
	"updated": "(fecha y hora de la creación del proyecto)",
	
	"operating": "true",
	
	"baseline": [
	
		(año menor de la época a estudiar),
		
		(año mayor de la época a estudiar),
		
	],
	
	"stations": [(lista de estaciones incluidas en el proyecto)]
	
}

A parte de lo anterior, si el sistema operativo sobre el que se esta trabajando es windows,
 en la siguiente ruta, *C:\Users\username\AppData\Roaming\.CLIMEX\PROJECTS* se creará una carpeta llamada **P1**.



### Reportar fallo

En caso de que los resultados obtenidos no sean los correctos puede reportar
una incidencia a la atención de *amarques@cgf.upv.es*.



