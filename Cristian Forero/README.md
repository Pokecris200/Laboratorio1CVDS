# **_CRISTIAN CAMILO FORERO MONROY_**
## **INFORMACION PERSONAL**
+ _Edad:_ 20 años
+ _Fecha de Nacimiento:_ 10 de Septiembre de 2001
+ _Universidad:_ Escuela Colombiana De Ingeniería Julio Garavito
	![](https://redvalorcompartido.com/wp-content/uploads/2020/04/escuela-ingenieria.png)
+ _Carrera:_ [Ingeniería de Sistemas](https://www.escuelaing.edu.co/es/programas/ingenieria-de-sistemas/)
+ _Habilidades principales:_
	1. Liderazgo
	2. Trabajo en equipo
	3. Adaptacion Facil
+ _Frase del Dia_
	> No Dejes de Soñar
+ _Algoritmo Favorito_
	def busquedaBinaria(unaLista, item):
		primero = 0
		ultimo = len(unaLista)-1
			encontrado = False

		while primero<=ultimo and not encontrado:
			puntoMedio = (primero + ultimo)//2
			if unaLista[puntoMedio] == item:
				encontrado = True
			else:
				if item < unaLista[puntoMedio]:
					ultimo = puntoMedio-1
				else:
					primero = puntoMedio+1

		return encontrado