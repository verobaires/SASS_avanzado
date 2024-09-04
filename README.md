# SASS APLICACION

### EXTEND
Bloque de codigo fijo que reutilizamos 

Declaracion ➡️ %nombre {
                propiedad : valor}

                
Uso ➡️ .clase { 
        @extend nombre}
        
![image](https://github.com/user-attachments/assets/e508dc92-d25c-42dc-bd93-4d12c303f927)

![image](https://github.com/user-attachments/assets/17b4084a-a43f-4eb3-8a90-d1072e7807f4)



### MIXIN
Bloque de codigo en el que puedo colocar pametros diferentes

Declaracion ➡️ @mixin nombre ($variable1, $variable2, $variable3) { 
                propiedad: $variable1; 
                propiedad: $variable2, 
                propiedad: $variable3;}

                
Uso ➡️ .clase { 
        @include nombre (valor1, valor2, valor3); 
          propiedad: valor; 
          propiedad: valor;}

          
![image](https://github.com/user-attachments/assets/48a2ed2b-8b2b-4ca8-92e0-a5e607619c73)
![image](https://github.com/user-attachments/assets/9ef0d4b1-8896-4e1d-8b30-48586b2be57c)



### LISTA
Lista de valores 

Declaracion ➡️ $nombre_de_lista: valor1, valor2, valor3;


Uso ➡️ selector {
          propiedad: nth($list: $nombre_de_lista, $n: (posicion en la lista) );


          
![image](https://github.com/user-attachments/assets/f49160b9-066a-4972-9051-bf3b8d3e53e1)
![image](https://github.com/user-attachments/assets/cf82d92d-eb18-45a8-bf3a-1a8c33f1b21c)



### MAP-GET
Coleccion de variables

Declaracion ➡️ $nombre_de_mapa: (
                nombre: key,
                nombre: key,
                nombre: key)
                

Uso ➡️ propiedad : map-get($map: (nombre del mapa), $key: (valor) );


![image](https://github.com/user-attachments/assets/650a38c4-ea39-4a6e-b6a1-42c4c4d5eae7)
![image](https://github.com/user-attachments/assets/dbf2be76-b935-428f-8c31-ba55747d2a67)



### BUCLE EACH
Secuencia que se repite, cuando deja de cumplirse se termina

**Bucles con listas**

Declaracion ➡️  @each $variable-iterador, $variable-valor in $nombre-lista{
                  .clase-#{$variable-iterador}{
                    propiedad: $variable-valor; } //uso de calc que es mas moderno

                    
Resultado  ➡️ .clase-variable {
                propiedad : valor }

                
![image](https://github.com/user-attachments/assets/5aeccb57-c49a-4e3d-a195-2799ec513bd1)
![image](https://github.com/user-attachments/assets/64598ec7-8a15-4113-9d35-245ee10ab5e0)


### CONDICIONAL
Evalua el valor de una variable para la aplicacion de estilos, no es una interaccion con el usuario, la variable a evaluar debe ser modificada manualmente.
Se puede colocar tantos if else como se necesite, se abre con un @if y se cierra con un @else

Declaracion ➡️  $variable : valor-x;
                @if($variable == valor) { 
                  selector { propiedad : valor;
                }@else if ($variable == valor){
                  selector { propiedad : valor;
                }@else {
                   selector { propiedad : valor; }

                   
![image](https://github.com/user-attachments/assets/db32fa03-a9d2-409e-8fb5-1b5eff5c2ffc)
![image](https://github.com/user-attachments/assets/7ab779a7-d4f8-4f9c-9e25-0086b5aa01df)


                   
                              












