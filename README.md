# aeropuertos

Disponemos de un fichero de texto con la información de los vuelos que salen de un determinado
aeropuerto, de forma que cada vuelo ocupa una línea del fichero separándose los campos por comas.
Es decir, la típica estructura csv. Las primeras líneas del fichero son las siguientes:

Madrid,12.37,155,100,IB1123,22,11,2007,1,5

Barcelona,19.56,200,150,VLG256,22,11,2007,1,20

Valencia,2.1,150,150,RYA803,22,11,2007,1,10

Paris,10.0,85,85,UA894,23,11,2007,2,30

Madrid,22.37,155,154,IB2365,23,11,2007,1,10

Los campos de cada línea en orden son:  
  Destino de tipo cadena de caracteres  
  Precio de tipo numérico real  
  Número de plazas de tipo numérico entero 
  Número de pasajeros de tipo numérico entero  
  Código del vuelo de tipo cadena de caracteres  
  Tres valores numéricos enteros que representan día, mes y año del vuelo  
  Dos valores numéricos enteros que representan duración del vuelo en horas y minutos.  


Ejercicio 1. Defina una estructura namedtuple para guardar en una tupla los valores de cada línea del
fichero

Ejercicio 2. Defina una función que reciba el nombre de un fichero con una estructura como la
descrita y devuelva una lista de tuplas de tipo Vuelo con la información leída del fichero.

Ejercicio 3. Dada una lista de tuplas de tipo Vuelo devuelve una lista con los códigos de los vuelos
que están completos.

Ejercicio 4. Dada una lista de tuplas de tipo Vuelo y un destino devuelve una lista con los códigos y
las fechas de los vuelos que vayan a ese destino.

Ejercicio 5. Dada una fecha devuelva los distintos destinos de los vuelos del aeropuerto en ese día.
Solución: Damos dos soluciones por comprensión y desplegada.

Ejercicio 6. Dado un destino devuelve ordenados por fecha los códigos de los vuelos con plazas
libres para ese destino.

Ejercicio 7. Tengo vacaciones a partir de una fecha y no me importa el destino del viaje siempre que
el vuelo sea barato (y haya plazas). Devuelve un conjunto ordenado con los n destinos más baratos
de los vuelos a partir de una fecha.

Ejercicio 8. Dado un valor n devuelve una lista con los destinos y porcentaje de ocupación de los n
vuelos con mayor porcentaje de ocupación.

Ejercicio 9. Dado un destino devuelve sin repetir las fechas en las que hay vuelos a ese destino
ordenadas de más cercana a más lejana en el tiempo.

Ejercicio 10. Dado un destino devolver una lista de tuplas con la fecha, el código y el precio de los
vuelos libres a ese destino ordenados por precio de menos a más.

Ejercicio 11. Defina una función que reciba una fecha y devuelva el número de vuelos anteriores a
esa fecha.

Ejercicio 12. Dado un destino devuelve el número de plazas libres en los vuelos a ese destino.

Ejercicio 13. Dada una fecha devuelva la duración total de los vuelos de ese día.

Ejercicio 14. Implemente una función tal que dado un destino devuelva la recaudación total a ese

Ejercicio 15. Dado un destino devuelva el precio medio de los vuelos a ese destino

Ejercicio 16. En ocasiones hay que hallar la media de valores que se obtienen relacionando dos o más
valores de la lista de tuplas. Por ejemplo, si preguntamos cuántos días transcurren entre dos vuelos,
hay que hallar la diferencia entre fechas y después convertirla a día. En Python esa operación se
puede hacer restando las dos fechas mediante el operador – (lo que devuelve un tipo timedelta y
después invocando a la función days para convertir ese periodo a días. Por ejemplo el siguiente
código mostraría un 2 en la consola.  
undia=datetime(2007,11,24).date()  
otrodia=datetime(2007,11,26).date()  
print((otrodia-undia).days)  
Con esa cuestión presente, se pide implementar una función tal que dado un destino devuelva el
número medio de días que transcurren entre dos vuelos a ese destino.

Ejercicio 17. Implemente una función que devuelva si existe algún vuelo con overbooking, es decir,
con más pasajeros que plazas. 

Ejercicio 18. Implemente una función tal que dado un número n devuelva si todos los vuelos tienen al
menos n pasajeros.

Ejercicio 19. Implemente una función tal que dada una fecha y un destino devuelva el vuelo de menor
precio a ese destino partir de la fecha.

Ejercicio 20. Puede ocurrir que el mínimo o máximo no se alcance en un único valor, sino que haya
empates en el menor valor. La función min devuelve el primer valor de la lista que alcanza el
mínimo, para el caso de querer devolverlos todos, necesitaríamos una función como esta:
Implemente una función tal que devuelva una lista con los códigos de los vuelos con el mínimo
número de plazas.

Ejercicio 21. Defina una función que reciba una lista de vuelos y devuelva un diccionario que
relacione cada fecha con el número de vuelos de ese día.

Ejercicio 22. Defina una función que reciba una lista de vuelos y devuelva un diccionario que
relacione cada destino con el número de pasajeros a ese destino.

Ejercicio 23. Defina una función que reciba una lista de vuelos y devuelva un diccionario que
relacione cada destino con la recaudación de los vuelos a ese destino.

Ejercicio 24. Defina una función que reciba una lista de vuelos y devuelva un diccionario que
relacione cada destino con la lista de códigos de los vuelos a ese destino.

Ejercicio 25. Defina una función que reciba una lista de vuelos y devuelva un diccionario que
relacione cada fecha con el conjunto de destinos de los vuelos de esa fecha.

Ejercicio 26. Implemente una función que devuelva un diccionario tal que para destino devuelva el
precio medio de los vuelos a ese destino

Ejercicio 27. Escriba una función que devuelva un diccionario que relacione cada destino con el vuelo
más barato a ese destino.

Ejercicio 28. Escriba una función que devuelva un diccionario que relacione cada destino con el
código del vuelo más barato a ese destino.

Ejercicio 29. Escriba una función que devuelva un diccionario que relacione cada destino con una
tupla con el código y el precio del vuelo más barato a ese destino.

Ejercicio 30. Implemente una función que devuelva el destino con mayor número de pasajeros.

Ejercicio 31. Defina una función que devuelva el destino con mayor número de vuelos.

Ejercicio 32. Defina una función que reciba un valor de n y devuelva una lista con los n destinos con
más vuelos ordenada por número de vuelos de mayor a menor. Tenga en cuenta que n puede tomar el
valor None en cuyo caso devolverá la lista de todos los destinos ordenada por número de vuelos

Ejercicio 33. Defina una función que reciba una lista de vuelos y devuelva el mes en el que hay más
vuelos a destinos distintos.

Ejercicio 34. Defina una función que devuelva un diccionario en el que las claves sean los meses y
como valor el destino con más viajeros de cada mes.

Ejercicio 35. Defina una función que reciba una lista de vuelos y un número n y devuelva un diccionario
que relacione cada mes con una lista ordenada alfabéticamente de los distintos destinos en los que haya
más de n vuelos ese mes.

Ejercicio 36. Escriba una función que devuelva un diccionario que relacione cada destino con el número
media de pasajeros de los vuelos a ese destino.

Ejercicio 37. Defina una función tal que dadas dos fechas que pueden ser None devuelva un diccionario
que relacione cada destino con el porcentaje de ocupación de los vuelos a ese destino entre esas dos
fechas. Si la primera fecha es None, se tendrán en cuenta los vuelos anteriores a la segunda, si la
segunda fecha es None, se tendrán en cuenta los vuelos posteriores a la primera y si las dos fechas son
None no habrá restricción de fechas.

Ejercicio 38. Implemente una función que devuelva un diccionario tal que a cada mes-año como clave
le haga corresponder el precio medio de los vuelos y el número de pasajeros total. Las claves serán
cadenas de texto formadas por el mes, un guion y el año (por ejemplo10-2017). Los valores del
diccionario serán tuplas formadas por dos elementos: media del precio de los vuelos y el número total
de pasajeros.

Ejercicio 39. Implemente una función tal que dado n devuelva un diccionario tal que a cada destino le
hace corresponder una lista con los n códigos de vuelo de menor ocupación.

Ejercicio 40. Cuál es la fecha con mayor incremento del número de pasajeros respecto del día anterior.
El concepto del día anterior se refiere al anterior que hubo vuelos.
