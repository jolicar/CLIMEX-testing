
## CLIMEX00CP002 Configuración de un proyecto.

### Descripción

Configurar el proyecto llamado **P1** con una lista de 3 estaciones, 11001, 11002 y 11003, y una época de 30 años comprendidos entre 1971 y 2000.

### Prerrequisitos

1. Tener instalado una versión de python igual o superior a la versión 3.8.
2. Tener instalado un interprete python o en su defecto utilizar la shell propia de la instalación.
3. Tener instalado una versión de la herramienta CLINMEX igual o superior a la versión 0.5.
4. Tener creado previamente un proyecto vacío llamado **P1**. *[(Ver CLIMEX00CP001 Creación de un proyecto)](https://github.com/jolicar/CLIMEX-testing/blob/main/cases/CLIMEX00CP001.md)*


### Pasos

1. Abrir el interprete de python.
2. Escribir el comando *import climex* y ejecutarlo.
3. Escribir el comando *P1* y ejecutarlo.
4. Escribir el comando *P1.stations=[11001,11002]* y ejecutarlo.
5. Escribir el comando *P1.stations=11003* y ejecutarlo.
6. Escribir el comando *P1.baseline=[1971,2000]* y ejecutarlo.
7. Escribir el comando *P1* y ejecutarlo.

### Resultado esperado

A continuación, se muestra una lista de resultados esperados para cada paso como consecuencia de estos.

**Paso 3** Como resultado se obtiene por pantalla en el interprete de python
un archivo **JSON** con la siguiente estructura.

{

	"created": "(fecha y hora de la creación del proyecto)",
	
	"updated": "(fecha y hora de la creación del proyecto)",
	
	"operating": "true",
	
	"baseline": [
	
		(año menor de la época a estudiar, valor por efecto 1961),
		
		(año mayor de la época a estudiar, valor por defecto 1990),
		
	],
	
	"stations": [(lista de estaciones incluidas en el proyecto)]
	
}

**Paso 7** Como resultado se obtiene por pantalla en el interprete de python
un archivo **JSON** con la siguiente estructura.

{

	"created": "(fecha y hora de la creación del proyecto)",
	
	"updated": "(fecha y hora de la creación del proyecto)",
	
	"operating": "true",
	
	"baseline": [
	
		1971,
		
		2000),
		
	],
	
	"stations": [
		"11001",
		
		"11002",
		
		"11003"
	]
	
}


### Reportar fallo

En caso de que los resultados obtenidos no sean los correctos puede reportar
una incidencia a la atención de *amarques@cgf.upv.es* indicando en el asunto el identificador CLIMEX00CP002.



