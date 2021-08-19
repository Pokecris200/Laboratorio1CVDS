# **_José Manuel Gamboa Gómez_**

## Datos Básicos

+ **Edad:** 20 años

+ **Fecha de Nacimiento:** 08-11-2000

+ **Ciudad de Nacimiento:** Tame, Arauca

+ **Lugar donde estudio:** [Escuela Colombiana de Ingenieria Julio Garavito](https://www.escuelaing.edu.co/es/)  

+ **Frase Favorita:**

   > ¡Sólo los que están preparados para morir deberían tener el poder de matar!

+ **Lugares que deseo Visitar:**

![](https://media.istockphoto.com/photos/aerial-view-of-tokyo-cityscape-with-fuji-mountain-in-japan-picture-id1131743616?k=6&m=1131743616&s=612x612&w=0&h=9NMsEs972mKE1QS1eDkN7I_nMoYyfLk_N9gtmvB07kc=)
   
    1. Japón  
   
![](https://canalhistoria.es/wp-content/uploads/2018/06/rusia.jpg)
   
    2. Rusia  
   
![](https://www.deutschland.de/sites/default/files/styles/crop_cover_top/public/media/image/Spezialseite_Pillarpage_Wegweiser_20102020_0.jpg?itok=E6U8K_KV)
   
    3. Alemania  

## **Code Ultra-Quicksort**  


	from sys import stdin
	
	def mezclar(arreglo,inicio,mitad,final):
	
		 """Funcion que cuenta el numero de cambios al rodenar un arreglo
		 Args:
			 arreglo: arreglo de enteros
			 inicio: entero
			 mitad: entero
			 final: entero
		 Returns:
			 Numero de cambios para ordenar arreglo"""
			 
		 iterador_izquierda,iterador_derecha,cambios = 0,0,0
		 parte_izquierda = arreglo[inicio:mitad+1]
		 parte_derecha = arreglo[mitad+1:final+1]
		 cambios = 0
		 parte_izquierda.append(1E9)
		 parte_derecha.append(1E9)  
		 
		 for k in range(inicio,final+1):
			 if parte_izquierda[iterador_izquierda] <= parte_derecha[iterador_derecha]:
				 arreglo[k] = parte_izquierda[iterador_izquierda]
				 iterador_izquierda = iterador_izquierda + 1
			 else:
				 arreglo[k] = parte_derecha[iterador_derecha]
				 iterador_derecha = iterador_derecha + 1
				 cambios = cambios + mitad - inicio - iterador_izquierda + 1
		 return cambios

	def mergesort(arreglo,inicio,final):
		cambios = 0
		if inicio < final:
			mitad = (inicio + final)//2
			#Mezclamos las 2 mitades del arreglo y contamos cuantos cambios se realizan
			cambios=mergesort(arreglo,inicio,mitad) + mergesort(arreglo,mitad+1,final) + mezclar(arreglo,inicio,mitad,final)
		return cambios

	def main():
		while True:
			cantidad_numeros = int(stdin. readline().strip())
			if cantidad_numeros == 0:
				break
			arreglo = []
			for i in range(cantidad_numeros):
				arreglo.append(int(stdin.readline().strip()))
			print(mergesort(arreglo,0,cantidad_numeros-1))        
	main()
	
## Learn Git Branching

### Main

![](https://github.com/Pokecris200/Laboratorio1CVDS/blob/master/Jose/Main%20completo.PNG)

### Remote

![]()