# **CanBus Shield**

### _¿Quienes somos?_

![Don Bosco](http://www.donbosco.hezkuntza.net/image/layout_set_logo?img_id=1747802)

#### Somos Amets, Igor y Javi, tres alumnos de 2º del Grado Superior de Mantenimiento Electrónico, en Don Bosco, Errenteria (Guipuzcoa, España). 

### _¿Cual es el objetivo de este proyecto?_

####  El objetivo de este proyecto es realizar un cuadro de coche digital, moderno y así substituir el antiguo. En nuestro caso hemos simulado la velocidad del vehículo, las revoluciones por minuto y la temperatura mediante unos potenciometros que actúan como sensores. Y los datos obtenidos los plasmamos en una pequeña pantalla Nextion de 7". 

### _¿Que elementos se necesitan?_

#### Los elementos que necesitaremos para realizar este proyecto son, dos arduinos, dos CanBus, tres potenciometros, una pantalla y la alimentación, ya sea mediante una pila o un enchufe. 

### _Arduino_
![Arduino](https://store-cdn.arduino.cc/uni/catalog/product/cache/1/image/520x330/604a3538c15e081937dbfbd20aa60aad/a/0/a000066_featured_4.jpg)
#### Arduino es una plataforma electrónica de código abierto basada en hardware y software fácil de usar. Está destinado a cualquier persona que realice proyectos interactivos. 
#### Con los arduino, tenemos dos programas, uno el programa Write y en el otro el programa Read. Uno de ellos recibe la señal de los potenciometros y convierte los valores recibidos a los valores legibles para nosotros y valores que queremos visualizar. 
#### Tras pasar por los CanBus, lo recibe el otro arduino y este los manda a la pantalla Nextion para mostrarlos. 

### _CanBus_

![CanBus](https://cdn.sparkfun.com//assets/parts/1/0/4/6/6/13262-01.jpg)

#### El CanBus se basa en una topología bus para la transmisión de mensajes en entornos distribuidos. Antiguamente la electrónica de los vehículos iba conectada mediante cables punto a punto, esto causaba algunos problemas por las situaciones adversas que presenta un coche a lo largo de su uso, vibraciones, temperatura, etc... Y porque cada vez la electrónica de los vehículos era mayor y la conexión se hacia mas compleja.

#### Para ello se empezó a instalar los CanBus y gracias a su comunicación bus, con solamente un cable conseguimos conectar toda la electrónica del vehículo. 

#### De igual manera, nosotros con los CanBus mandamos los datos recibidos y convertidos de los potenciometros a la pantalla Nextion. 

### _Potenciometro_ 

![Potenciometro](https://www.cetronic.es/sqlcommerce/ficheros/dk_93/productos/451047005-1.jpg)

#### Hemos usado tres potenciometros como este, para simular tres sensores del vehículo. Uno para la velocidad, otro para las revoluciones por minuto y un ultimo para la temperatura del motor. 
#### Los potenciometros tienen 1024 valores legibles estando totalmente grado, y 0 cuando esta girado inversamente. Por ello gracias a un comando de arduino, transformamos los 1024 en 200 km/h. De esta forma, cuando giremos el potenciometro al máximo solo nos marcara el limite de 200. 
#### Para las revoluciones y la temperatura, hemos puesto otros margenes. Ya que estas dos funciones van con barras progresivas de Nextion, su máximo es 100. Por eso la conversión de estos potenciometros son 1024 igual a 100. 

### _Nextion_

![Nextion](https://images-na.ssl-images-amazon.com/images/I/612p3I1L21L._AC_SX466_.jpg)

#### Esta es la pantalla, que se nos ha proporcionado para realizar el cuadro del coche. Es una pantalla de 7" HMI inteligente. Es una interfaz de control y visualización entre un humano y un proceso. Es una pantalla fácil de usar, con un software, que se aprende rápido a usar y que tiene un sinfín de opciones y configuraciones. También para el proyecto se puede realizar con otro tipo de pantallas. 

### _Alimentación_ 

![Pila](https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcQW1fBVEIPv3gqW8ZktMTe-zrijqqr5HtEuFZSf5K6VjIIiJeSV&usqp=CAU)

#### Para que nuestro proyecto este funcionando, tenemos que alimentarlo, en nuestro caso, para realizar pruebas lo hacíamos mediante un cable conectado a arduino. Pero para presentar el proyecto, lo realizamos con una pila. Ya que queda mas estético que no se vea un cable y tener que estar con el ordenador al lado. Eso si, procurar siempre tener una pila de recambio, porque como todo, tiene su vida útil y se podría desgastar. 

