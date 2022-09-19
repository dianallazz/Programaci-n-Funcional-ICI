![image](https://camo.githubusercontent.com/35e9d7d200795e6ec6bbf764d7f700d8da81cb5bc28ef9787d104a22eb3293a6/68747470733a2f2f696d67732e7365617263682e62726176652e636f6d2f37315a705a5949444b4a46463468797a765a5f4b6133636f2d625875356d5330756f496a637635757679342f72733a6669743a313230303a3638373a312f673a63652f6148523063446f764c336433647935312f593239734c6d31344c324e76626e526c2f626e51765932317a4c7a6b76615731682f5a3255765657526c51305644556c4d342f4d4734756347356e)
# Universidad de Colima
### Facultad de Ingenieria Mecanica y Electrica
### Ingenieria en Computacion Inteligente
##### Estudiante: Diana Laura Llamas Alcaraz
##### Profesor: Dr. Walter Alexander Mata Lopez
---
## Introduccion:

Este es un portafolio de la primera parcial en la materia de programacion funcional de la carrera de ICI. 
Donde estaran adjuntos los diferentes codigos de las clases en las que trabajamos.


---
# Primera Parcial

### _Trabajos de/en clase_

- #### Print.
      
      print("Hola ICI")

- #### Markdown.

      # UNIVERSIDAD DE COLIMA
      ## FACULTAD DE INGENERIA MECANICA Y ELECTRICA
      ### INGENIERIA EN COMPUTACION INTELIGENTE
    
- #### Interpolacion de Cadenas.

      name="Laura"
      edad=52
      print("hola",name,"tienes",edad,"años")
    
- #### fstrings.

      mensaje=f"hola {name} ,tienes {edad} años"
      mensaje
      print(mensaje)
      print(f"hola {name},tienes {edad} años")

- #### Funciones.

      def saludo(): 
      
      print("Hola mundo") 
      mi_funcion=saludo()    #asignando la funcion
      saludo()               #Invocando la funcion  
      print(mi_funcion) 
      
      def saludo2():
      
      return"Hola mundo"
      saludo2() #Invocacion 
      mi_funcion2= saludo2()
      print(mi_funcion2)
      a=5
      b=10
      res = f" La suma de {a}+{b} = {a+b}"
      print(res)

      def suma(a,b):
      
      return a+b
      res = f"La suma de {a}+{b} = {suma(a,b)}
      print(res)

- #### Listas, tuplas, sets y diccionarios.

       lista_numeros = ["uno","dos","tres"]
      msg_numeros= f"Numeros:{lista_numeros}"
      print(msg_numeros)

##
      tupla_numeros=("uno","dos","tres")
      msg_numeros=f"numeros:{tupla_numeros}"
      print(msg_numeros)
##

      set_numeros={"1","2","3","4","5","6","7","8","9","10"}
      print(set_numeros)
##
      dict_numeros={"1":"uno","2":"dos","3":"tres"}
      msg_dict_numeros=f"numeros:{dict_numeros}"
      print(msg_dict_numeros)

      dos= f"Numeros:{dict_numeros['2']}"
      print(dos)
  
---
## _Ejercicio de lo aprendido en clase #1_

  Escriba una funcion que mediante fstrings retorne el mensaje "Hola -nombre- tienes -edad- años". 
  Los argumentos de la funcion: año actual, año de nacimiento y nombre.

    nombre="Diana"
    edad=52
  
    def msj(nombre,edad):
     return(nombre,edad)
     mensaje=f"hola {nombre} tienes {edad}"
     print(mensaje)
    
  
---
- #### Uso de las fstrings 

     Ejemplos:
     
      num_materia=["No. ",1,2,3,4]
      nom_materia=["Materia ","EDD","ED","PF","MN"]
      nom_profesor=["Profesor ","Francisco S.","Elizabeth S.","Walter M.","Edgar C."]              
      print (f"{num_materia[0]:^5}{nom_materia[0]:^30}{nom_profesor[0]:<6}")
      for i in range (1,5):
       print(f"{num_materia[i]:^5}{nom_materia[i]:<30}{nom_profesor[i]:<6}")




      alumnos=["Diana","Leonardo","Pedro","David","Jose"]
      materia=[6,8,6,8,7]
      materia2=[8,9,10,8,9]
      materia3=[8,8,7,6,9]
      materia4=[9,9,9,9,10]
      titulos=["Nombre","Programacion funcional","Metodos numericos","Estructura de datos","Ingles"]

      def reporte (fmt):
        print(f"{titulos[0]:^{fmt}}{titulos[1]:^{fmt}}{titulos[2]:^{fmt}}{titulos[3]:^{fmt}}{titulos[4]:^{fmt}}")
          for i in range (5):
          print(f"{alumnes[i]:*^{fmt}}{materia[i]:*^{fmt}}{materia2[i]:*^{fmt}}{materia3[i]:*^{fmt}}{materia4[i]:*^{fmt}}")
      reporte(20)

- #### Funciones y fstrings

   Ejemplos:
   
		    def saludo_edad_(nombre:str,a_nacimiento:int):
				 edad= 2022-a_nacimiento
				 print("Hola",nombre,"tienes",edad,"años")

		    def calcular_edad(a_actual:int,a_nacimiento:int)->int:
         return a_actual-a_nacimiento

		    def saludo(nombre:str,edad:int):
				 print ("Hola",nombre,"tienes",edad,"años")

        def cuadrados(numu:int,numd:int):
          return (numu*numu) + (numd*numd)
        if __name__=="__main__":
          print(cuadrados(2,2))
        
        def tabla(x):
          for i in range (11):
            print(x,"*",i,"=",x*i)

        if __name__=="__main__":
          print(tabla(3))
        
  ## 
   
		def tabla(t,n):
				for i in range (1,n+1):
					print(t,"*",i,"=",t*i)
		if __name__=="__main__":
				print(tabla(3,2))
        
		def tabla(t:int,n:int,spc:int):
				for i in range (1,t+1):
				  for j in range (1,n+1):
						print(f""i,"*",j,"=",i*j)
                
		t=int(input("¿Hasta que tablas quieres calcular?"))
		n=int(input("¿Hasta que numero quieres calcular?"))
		tabla(t,n)
    
		def tabla(t:int,n:int,spc:int):
				for i in range (1,t+1):
						for j in range (1,n+1):
							print(f"{i:^{spc}} * {j:^{spc}} = {i*j:^{spc}}")
                
		t=int(input("¿Hasta que tablas quieres calcular?"))
		n=int(input("¿Hasta que numero quieres calcular?"))
		spc=int(input("¿Que espaciado quieres?"))
		tabla(t,n,spc)

- #### Uso de librerías 

  Crear 5 librerias donde cada unas tenga solo una
  operacion basica(+,-,*,/ y cuadrado)
  probarlas de manera independiente y usarlas en el main.
  
  ##### main:
  
      import suma as a
      import resta as b
      import multiplicacion as c
      import division as d
      import cuadrado as e

      if __name__ == "__main__":
       print("Operaciones:")

       print("Suma:",a.suma(4,5))
       print("Resta:", b.resta(4, 5))
       print("Multiplicacion:",c.multiplicacion(4,5))
       print("Division:",d.division(20,5))
       print("Cuadrado", e.cuadrado(4))


      """
      from ops import *
      el asterisco es para importar todas las funciones de ops
      """
  ##### suma:
  
      def suma(n1:int,n2:int)-> int:
          return n1+n2


      if __name__ == "__main__":
          print("resultado: ",suma(3,5))
     
  ##### resta:
  
      def resta(n1:int,n2:int)-> int:
          return n1-n2


      if __name__ == "__main__":
          print("resultado: ",resta(3,5))
          
  ##### multiplicación:
  
      def multiplicacion(n1:int,n2:int)-> int:
          return n1*n2


      if __name__ == "__main__":
          print("resultado: ",multiplicacion(3,5))
          
  ##### division:
  
      def division(n1:float,n2:float)-> float:
          return n1/n2


      if __name__ == "__main__":
          print("resultado: ",division(3,5))
          
  ##### cuadrado:
  
      def cuadrado(n1:int)-> int:
       return n1*n1


      if __name__ == "__main__":
       print("resultado: ",cuadrado(3))


- #### Uso de listas

      mi_lista = [1,2,3,4]
      print(mi_lista)
      lista_vacia= []
      print(lista_vacia)

      mi_lista2=[1,"hola", True,3.5,[1,2,3],(1,2,3),{4,5,6}]
      print(mi_lista2)


      print(len(mi_lista2))
      print(f"Mi lista: {mi_lista}")
      print(f"No. de elementos: {len(mi_lista)}")
      print(f"Primer elemento: {mi_lista[-1]},{mi_lista[-2]},{mi_lista[-3]},{mi_lista[-4]}")

      print(mi_lista[1:-1])
      print(mi_lista[0:3])
      print(mi_lista[0:])
      print(mi_lista[:])

      #modificar los datos de mi lista
      mi_lista[2]="tres"
      print(mi_lista)


      #insertar la lista [5,"seis",7,8] al final de mi_lista

      mi_lista[len(mi_lista):]=[5,"seis",7,8]
      print(mi_lista)


      #slices

      mi_lista=[1,2,3,4]
      mi_lista.append("cinco")
      print(mi_lista)

      ml=[]
      for i in range(1,5):
          ml.append(i)
      #ml.append([6,7,8])
      #print(ml)
      ml.extend([6,7,8])
      print(ml)
      ml.insert(4,"5")
      print(ml)

      del ml[5]
      print(ml)

      ml.remove('5') 
      print(ml)

      ml.reverse()
      print(ml)

      print("------------")

      ld=[5,4,6,7,8,2,3,4,5,6,7]
      print(f"Desordenado: {ld}")
      ld.sort()   
      print(f"Ordenado: {ld}")    

      print("---------------------")

      ld=[5,4,6,7,8,2,3,4,5,6,7]
      s1=sorted(ld)
      print(s1)

      ld=[5,4,6,7,8,2,3,4,5,6,7]
      s2=sorted(ld,reverse=True)
      print(s2)
      ld

      ceros=[0,0,0,0,0,0,0,0,0]
      print(ceros)
      ceros=[0]*9
      print(ceros)

      valor_max=max(ld)
      print(valor_max)
      valor_min=min(ld)
      print(valor_min)

      cuatros=ld.count(4)
      print(cuatros)
      repetidos=[]
      print("------------------------")
      for i in range(1,9):
         repetidos.append(ld.count(i))

      print(repetidos)


## _Ejercicio de lo aprendido en clase #2_

Escribe una funcion que reciba como argumentos T y N donde T es el limite de tablas de multiplicar que se 
desean obtener y N hasta un valor de las tablas se desea. Todas empiezan desde el 1.

    def tablas(t:int,n:int):
    
     for i in range(1,t+1):
      tabla(i,n,10)

  	def tabla(t:int,n:int,spc:int):
    
  	 for i in range (1,n+1):
  		print(f"{t:^{spc}}x{i:^{spc}}={t*i:^{spc}}")

  	t=int(input("¿Hasta que tablas quieres calcular?"))
  	n= int(input("¿Hasta que numero quieres calcular?"))
  	tablas(t,n)

---
