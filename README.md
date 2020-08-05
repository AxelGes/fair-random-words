# REALLY Random Words

Que hace:
Con este script podrá verificar la verdadera aleatoridad de una generación de palabras soportada por una encriptación SHA-256.


Como funciona:
Se genera desde un inicio una cadena de 1 millones de hashes SHA256, siendo el primero un secreto del servidor el cual se autoalimenta repetidamente con su salida de SHA256 1 millon de veces.

El SHA256 del hash final para esto es: 5bf9a3fae704667be2d3704ea8b6e703796defaa5f328e1a8d46b3a0fa12269f

Al publicarlo aqui, se evita cualquier posibilidad de elegir una cadena SHA256 alternativa.

A la hora de utilizar este script esta cadena de hashes se reproduce en orden inverso, es decir que una vez generado el usuario puede comprobar si esta generación se corresponde con la versión anterior.



Como verificar:
Cualquiera puede verificar fácilmente la integridad de la cadena.

A la hora de la muestra del resultado aleatorio se muestra el hash de esa palabra inmediatamente.

Al verificar que el hash SHA256 del hash de esa palabra es en efecto el hash de la palabra anterior, queda demostrado que no existió modificación de la cadena y que esta palabra ya había sido generada desde antes.



Legitimidad:
Con este script se demuestra que los resultados de todas las palabras futuras ya estan predefinidas y normalmente distribuidos debido a las matemáticas que respaldan la fuerte función criptográfica SHA256. Esta cadena de resultados no podrá ser manipulada sin que el público lo note.