<img src="https://siceuc2.ucol.mx/becatitulaciongobiernodelestado/Assets/images/03UdeC_publi_80.png">

# Universidad de Colima 
## Facultad de Ingeniería Mecánica y Eléctrica 
### "Ingenieria en Computacion Inteligente"
### Alumno:
  * Jason Humberto Garcia Camacho 
### Maestro:
  *  Walter Alexander Mata Lopez

---------------------------------------------------

# Portafolio de programas relalizado en la primera parcial en lenguage python 

---------------------------------------------------------

## impreción de un mensaje

      print("hola ICI")   

-------------------------------------------------------------

## Titulos y Subtitulos 

    # universidad de colima
    ## Facultad de ingenieria mecánica y electrica
    ### ingenieria en computacion inteligente
    #### contenidos
    * introduccion a los tipos de programacion en python  
    
 ------------------------------------------------------------
 
 ## interpolacion de cadenas
       name ="jason"
       edad= 18
       print("hola",name,"tienes",edad,"años")
-----------------------------------------------------------------
 ## fstrings
    mensaje = f"hola {name}, tienes {edad} años"
    mensaje
    print (mensaje) 
    print(f"hola {name}, tienes {edad} años")
 ---------------------------------------------------------------
  ## Funciones
  
      def saludo():
          print("hola mundo!!!")
          
    saludo() #asignado el saludo
    
    mi_funcion = saludo() #aignado la funcion 
    
    print(mi_funcion)
    
    def saludo2():
       return "HOLA MUNDO!!"
       
    saludo2() #invocacion 
    
    mi_funcion2 =saludo2()
    
    print(mi_funcion2)
    
    
    a = 5
    b= 10
    res= f"la suma de  {a} + {b} = {a+b}"
    print(res)
    
    def suma (a,b):
       return a+b
       
    res = f"la suma de  {a} + {b} = {suma(a,b)}"
    print (res)
    
 --------------------------------------------------------------
  ## Listas
       lista_numeros = ["uno","dos","tres"]
       msg_numeros = f"numeros: {lista_numeros}"
       print(msg_numeros)
 -------------------------------------------------------------------
  ## tuplas
       tupla_numeros =("uno","dos","tres","tres")
       msg_numeros =f"numeros: {tupla_numeros}"
       print(msg_numeros)
  -----------------------------------------------------------------
  ## set
       set_numeros = {"uno","dos","tres","tres"}
       print(set_numeros)
  -----------------------------------------------------------------
    ## diccionario
    
       dic_numero ={"1": "uno","2":"dos","3":"tres"}
       msg_dic_numeros = f"numeros: {dic_numero}"
       print(msg_dic_numeros)
       
   ---------------------------------------------------------------------
   ## Operaciones basicas 
   
   suma
   
      def suma(num:int,num2:int)->int: return num+num2

  	       if __name__ == "__main__":
  			          print(suma(4,5))
   Resta

  	     def resta(num: int, num2: int) -> int: return num - num2

                      	if __name__ == "__main__":
  		                       	print(resta(3, 7))
               
   División

  	      def divisi(num: int, num2: int) -> float: return num / num2

  	                    if __name__ == "__main__":
  			                     print(divisi(4, 5))
               
   Multiplicación

  	    def multi(num: int, num2: int) -> int: return num * num2

                	if __name__ == "__main__":
  	                  print(multi(4, 5))
   Cuadrado

  	              def cuadrado(num: int) -> int: return num*num

  	                       if __name__ == "__main__":
  			                        print(cuadrado(5))
   
   
   
   
   ----------------------------------------------------------------------
   ## EJERCICIO EN CLASE
   
   Escriba una funcion que mediante fstrings retorne el mensaje "Hola -nombre- tienes -edad- años". Los argumentos de la      funcion: año actua, año de nacimiento y nombre
   
   1-
   
          name ="jason"
          edad= 19
          mensaje = f"hola {name} , tienes {edad} años"
          print (mensaje)
          
   2-
    
          def mensaje(name:str,edad:int)->str:
                return f"hola {name }, tienes {edad} años"
                
          print (mensaje("Jason",19))
          
   ----------------------------------------------------------------------------------
   
   
  ## Ejemplos en clase con Fstrings aplicadas
  
1-

      num_materia=["No. ",1,2,3,4]
      name_materia=["Materia","Estructura de datos","Ecuaciones diferenciales","Programacion funcional","Metodos numericos"]
      name_profesor=["Profesor","Soto","Eli","Walter","Edgar"]              
      print (f"{num_materia[0]:^5}{name_materia[0]:^30}{name_profesor[0]:<6}")
      for i in range (1,5):
  	       print(f"{num_materia[i]:^5}{name_materia[i]:<30}{name_profesor[i]:<6}")
          
2-  
           
    alumnos = ["jason","josue","alexis","andy","diana"]
    materia1 =[10,9,10,8,10]
    materia2 = [7,7,8,7,9]
    materia3 = [6,7,8,9,5]
    materia4 = [6,6,7,7,6]

    encabezado = ["nombre ALM","ESc. de datos","ecuaciones diferenciales","metodos numericos","programacion funcional"]

    def reporte(fmt):
        print(f"{encabezado[0]:^{fmt}} {encabezado[1]:^{fmt}} {encabezado[2]:^{fmt}} {encabezado[3]:^{fmt}}{encabezado[4]:^{fmt}}")
        for i in range (5): 
           print(f"{alumnos[i]:^{fmt}} {materia1[i]:^{fmt}} {materia2[i]:^{fmt}} {materia3[i]:^{fmt}} {materia4[i]:^{fmt}}")
        
            reporte(20)
       
 ---------------------------------------------------------------------------------------------
 
 ## funciones con manejo de fstrings 
   
    #%%
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
    
		# %%
		def tabla(x):
				for i in range (11):
						print(x,"*",i,"=",x*i)

		if __name__=="__main__":
				print(tabla(3))
    
  tablas de multiplicar
   
   
    def tabla(t,n):
				             for i in range (1,n+1):
						                        print(t,"*",i,"=",t*i)
		if __name__=="__main__":
			           	print(tabla(3,2))
		# %%
		def tabla(t:int,n:int,spc:int):
				              for i in range (1,t+1):
						                           for j in range (1,n+1):
								                                   print(f""i,"*",j,"=",i*j)
		t=int(input("¿Hasta que tablas quieres calcular?"))
		n=int(input("¿Hasta que numero quieres calcular?"))
		tabla(t,n)
  
		# %%
		def tabla(t:int,n:int,spc:int):
			             	for i in range (1,t+1):
						                      for j in range (1,n+1):
							                                	print(f"{i:^{spc}} * {j:^{spc}} = {i*j:^{spc}}")
		t=int(input("¿Hasta que tablas quieres calcular?"))
		n=int(input("¿Hasta que numero quieres calcular?"))
		spc=int(input("¿Que espaciado quieres?"))
		tabla(t,n,spc)
  
  ------------------------------------------------------------------------------------------------
    ## listas
    
       mi_lista = [1,2,3,4]
       print (mi_lista)
       lista_vacia =[]
       print(lista_vacia)

       mi_lista2 =[1, "hola", True, 3.14,[1,2,3] ,(1,2,3),{4,5,6}]
       print(mi_lista2)

        print(len(mi_lista))
       print(len(mi_lista2))
       print(mi_lista[0])


       print(len(mi_lista2))
       print(f"mi lista: {mi_lista}")

       print(f"no de elementos:  {len(mi_lista)}")
       print(f"primer elemento:  {mi_lista[0]}")
       print(f"todos los elemento:  {mi_lista[0]},{mi_lista[1]},{mi_lista[2]},{mi_lista[3]}")
  
  
  partes de una lista por pociciones
          
          
          print(mi_lista[1:-1])
          print(mi_lista[0:3])
          print(mi_lista[0:])
           print(mi_lista[:])
           
 modificar elementos de la lista

           mi_lista[2]= "tres"
           print (mi_lista)
           
 insertar la lista [5,"seis",7,8] al final de la lista mi_lista

         mi_lista[len(mi_lista):]=[5,"seis",7,8]
         print (mi_lista)
         
 #slices

          mi_lista = [1,2,3,4]
          mi_lista.append("CINCO")
          print(mi_lista)
          
          
          ml= []
         for i in range (1,5):
          ml.append(i)
          ml.append([6,7,8])
          print(ml)
          ml.extend([6,7,8])

          ml.insert(4,"5")
          print(ml)

           del ml[5]
           print(ml)

           ml.remove("5")
          print(ml)
          

lista desordenada

     ld=[5,4,6,7,8,2,1,3,4,5,6,7]
     print(f"desordenado: {ld}")
     ld.sort()
    print(f"ordenado: {ld}")

lista desordenada con corchetes

     ld=[[5,4,6],[7,8,2],[1,3,4,5],[6,7]]
     print(f"desordenado: {ld}")
     ld.sort()
     print(f"ordenado: {ld}")
        ld=[5,4,6,7,8,2,1,3,4,5,6,7]
        print(f"desordenado: {ld}")
        ld.sort()
        print(f"ordenado: {ld}")

sorted sirve para ordenar una lista 

    ld=[5,4,6,7,8,2,1,3,4,5,6,7]
    s1=sorted(ld)
    print(s1)

sorted 2 es para ordenar de mayor a menor 

      ld=[5,4,6,7,8,2,1,3,4,5,6,7]
      s2 =sorted(ld,reverse=True)
      print(s2)

listas de dos formas con elementos iguales 
forma1

      ceros =[0,0,0,0,0,0,0,0,0]
      print(ceros)

forma2

     ceros=[0]*9
     print(ceros)

segun matris de 9*9

    ceros=[[[0]*9]*9]
    print(ceros)

valor maximo de una lista o el mayor dse todos 

       valor_max= max(ld)
       print(valor_max)

valor minimo de una lsita 

    valor_min= min(ld)
    print(valor_min)          
-------------------------------------------------------------------------------

## Ejercicio en clase  tablas de multiplicar

escriba una funcion que reciba como argumentos t y N donde t es el limite de tabalas que se desa obtener y las tablas  y m m que valor de las tablas se deseada . todas empiezan iniciom uno 

     print("Programa para sacar las tablas de multiplicar")

     iniciot = 1
     t = int(input("ingresa el limite de las tablas de multiplicar: "))
     iniciom = 1
     m= int(input("ingrese el limite de multiplicacion de las tablas : "))

     def multiplicacion (t,m):
         for factor1 in range (iniciot,t+1):
             print(f"tabla de multiplicar del {factor1}:")
             for factor2 in range(iniciom,m+1):
                 print (f"{factor1} x {factor2} = {factor1*factor2}")
             print()
      multiplicacion(t,m)        

