## Calculadora
En este trabajo se nos mandó a hacer una calculadora que funcione con un servidor y un cliente, el primero hace la función de resolver las operaciones, mientras que el segundo se encarga de que el usuario introduzca esas operaciones.

# Servidor
Como ya se indico anteriormente, en el servidor se encuentra el código con el que podremos realizar las operaciones que el cliente quiera.

El principio de esta tarea es igual a una de los ejercicios que hicimos anteriormente de servidor-cliente.

<img width="800" height="1026" alt="Captura de pantalla 2025-12-02 232037" src="https://github.com/user-attachments/assets/6be33466-39b5-40cf-a8b8-765ff3aacd84" />

Como podemos ver, a partir de este código ya podemos conectarnos con el cliente, ya que indicamos cual es el puerto al que irá el servidor, en este caso es el 8080.
Dentro del bucle se aprecia como se declara la función resolviendoOP, esta misma la crearemos más adelante y es la que contiene el tipo de operación que podremos hacer:

<img width="776" height="1240" alt="Captura de pantalla 2025-12-02 232354" src="https://github.com/user-attachments/assets/ed1e06b2-2ff5-4a8b-91d9-a56faa1dcfbd" />

Ahora, dentro de esta función, se utiliza switch-case para poder tomar decisiones múltiples (es algo parecido a un if-else pero mucho más robusto y legible). En cada case tendremos que declarar las operaciones y lo que harán cada una, es decir, si se usa "mult" se busca multiplicar los números.


# Cliente
Ya terminado el servidor, podemos pasar al cliente, el cual se encarga de introducir las operaciones que queramos.

<img width="792" height="1070" alt="Captura de pantalla 2025-12-02 233000" src="https://github.com/user-attachments/assets/9daeeaab-adb8-4738-b6f3-286c065df33f" />

Cuando el servidor ya esté esperando a un cliente, se ejecuta este código para poder realizar esta conexión. 

La principal función de este código se encuentra en el bucle, ya que es aquí donde podremos indicarle las operaciones al servidor, además de, si escribimos "ejemplos", se abrirá una lista con todas las operaciones disponibles.
