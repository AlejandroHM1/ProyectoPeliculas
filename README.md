#Proyecto Hilos

##Introduccion

En este prouecto se busca resolver la problematica que surgió en una pagina de streaming de la platoaforma de Netflix.
Netflix busca que su pagina muestre la lista de peliculas que tiene en su biblioteca, cuando el usuario escriba el nombre de la pelicula que quiere ver.
Aparte de mostrar la pelicula se debe mostrar una descripcion y posiblemente algun otor dato.


##Metodologia

###Hilos vs Procesos

###Proceso

Un proceso es una instacioa de un inetprete de Python que tiene al menos un holo llamado MainThread. Un proceso tiene dos funciones principales; la primera es actuar como el manejador del recurso de la aplicación; la segunda es ejecutar las intrucciones de la aplicación.

###Hilo

Un hilo de ejecucion en un proceso de Pyhton, tal como el MainThread o un nueco hilo. Se representa como una instacia de la clase threading.Tread. Un hilo es la representacion de un objeto de un hilo nativo proporcionado por el sistema operativo.

##Creaion de un Hilo

Para crear un hilo:

   thread = threading.Thread(target=foo, args=(7, 'Hello World'))
   
   thread.start()
   
   thread.join()
   
Para crear una lista de hilos:

thread_lst = [threading.Thread(target=foo) for i in range(5)]

for i in thread_lst:
  i.start()

for i in thread_lst:
  i.join()
  print('return')
