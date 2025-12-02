# Calculadora
En este trabajo se nos mandó a hacer una calculadora que funcione con un servidor y un cliente, el primero hace la función de resolver las operaciones, mientras que el segundo se encarga de que el usuario introduzca esas operaciones.

## Servidor
Como ya se indico anteriormente, en el servidor se encuentra el código con el que podremos realizar las operaciones que el cliente quiera.

El principio de esta tarea es igual a una de los ejercicios que hicimos anteriormente de servidor-cliente.

<img width="800" height="1026" alt="Captura de pantalla 2025-12-02 232037" src="https://github.com/user-attachments/assets/6be33466-39b5-40cf-a8b8-765ff3aacd84" />

Como podemos ver, a partir de este código ya podemos conectarnos con el cliente, ya que indicamos cual es el puerto al que irá el servidor, en este caso es el 8080.
Dentro del bucle se aprecia como se declara la función resolviendoOP, esta misma la crearemos más adelante y es la que contiene el tipo de operación que podremos hacer:

<img width="776" height="1240" alt="Captura de pantalla 2025-12-02 232354" src="https://github.com/user-attachments/assets/ed1e06b2-2ff5-4a8b-91d9-a56faa1dcfbd" />

Ahora, dentro de esta función, se utiliza switch-case para poder tomar decisiones múltiples (es algo parecido a un if-else pero mucho más robusto y legible). En cada case tendremos que declarar las operaciones y lo que harán cada una, es decir, si se usa "mult" se busca multiplicar los números.


## Cliente
Ya terminado el servidor, podemos pasar al cliente, el cual se encarga de introducir las operaciones que queramos.

<img width="792" height="1070" alt="Captura de pantalla 2025-12-02 233000" src="https://github.com/user-attachments/assets/9daeeaab-adb8-4738-b6f3-286c065df33f" />

Cuando el servidor ya esté esperando a un cliente, se ejecuta este código para poder realizar esta conexión. 

La principal función de este código se encuentra en el bucle, ya que es aquí donde podremos indicarle las operaciones al servidor, además de, si escribimos "ejemplos", se abrirá una lista con todas las operaciones disponibles.


## Resultado
Los posibles resultados serían los siguientes, comprobando también que las operaciones funcionan correctamente:

Aquí el servidor está esperando que el cliente se conecte.

<img width="310" height="172" alt="Captura de pantalla 2025-12-02 233850" src="https://github.com/user-attachments/assets/1eec66e6-69c5-4110-ad8d-9956ac3b2f00" />

Aquí muestra el mensaje del cliente una vez ya se haya conectado:

<img width="742" height="242" alt="Captura de pantalla 2025-12-02 233902" src="https://github.com/user-attachments/assets/58784cf6-074d-4a62-a1c6-9ee7847ef5a8" />

Una vez realizada la conexión, ya podremos realizar todas estas operaciones:

- Escribir "ejemplos":

<img width="677" height="198" alt="Captura de pantalla 2025-12-02 233937" src="https://github.com/user-attachments/assets/1b44f8f6-10d5-41d7-9c60-0d4ae3e40c45" />


- Suma:

<img width="686" height="88" alt="Captura de pantalla 2025-12-02 234000" src="https://github.com/user-attachments/assets/24e34dce-0da1-4bff-bae1-3e6a65e35ae6" />


- Resta:

<img width="681" height="90" alt="Captura de pantalla 2025-12-02 234110" src="https://github.com/user-attachments/assets/bf78b7e8-599d-4000-87cd-f5c7823f1622" />


- Multiplicación:

<img width="675" height="87" alt="Captura de pantalla 2025-12-02 234220" src="https://github.com/user-attachments/assets/9c5de30e-cbf7-40da-ba65-180a79d61a75" />


- División:

<img width="677" height="85" alt="Captura de pantalla 2025-12-02 234233" src="https://github.com/user-attachments/assets/f802b92f-4faa-4627-a747-15d10a11fb1f" />


- Cerrar conexión con "adios":

<img width="683" height="129" alt="Captura de pantalla 2025-12-02 234247" src="https://github.com/user-attachments/assets/3f3ac374-0746-4fde-80c4-667abf04a74c" />


La parte del servidor se debe ver así:

<img width="493" height="363" alt="Captura de pantalla 2025-12-02 234255" src="https://github.com/user-attachments/assets/875cd174-cdfd-49de-a2cf-e4d34ba4c4c8" />
