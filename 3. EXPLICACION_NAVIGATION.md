### EL NAVIGATION SE COMPONE DE VARIAS ESTRUCTURAS

#### 1. DESTINATIONS: SON TODAS LAS PANTALLAS DE DESTINO EN LA APLICACION Y SE RECOMIENDA QUE SEAN FRAGMENTS

![Image](https://github.com/srodriguez9017/NavigationComponent/blob/master/images/DESTINATIONS.JPG?raw=true)

#### 2. ACTIONS: SON LAS FLECHITAS QUE CONECTAN LAS PANTALLAS Y CONTIENEN LA INFO HACIA DONDE TIENEN QUE DIRIGIRSE

![Image](https://github.com/srodriguez9017/NavigationComponent/blob/master/images/ACTIONS.JPG?raw=true)

#### De esta forma se verian en el proyecto en su vista diseño

![Image](https://github.com/srodriguez9017/NavigationComponent/blob/master/images/EJEMPLO_DESTINATION_ACTIONS.JPG?raw=true)

#### Y asi en la vista de xml

![Image](https://github.com/srodriguez9017/NavigationComponent/blob/master/images/EJEMPLO2_DESTINATION_ACTION.JPG?raw=true)

### Como se ve contiene:

#### 1. ID: Este seriael id del destination
#### 2. NAME: Seria el paquete donde esta el fragment como tal
#### 3. LAYOUT: Que es la vista de diseño asociada al fragment

### Ahora bien dentro de cada fragment se encuentran los actions que contienen:

#### 1. ID: Un identificador de la accion
#### 2. DESTINATION: Que es el id del destination al cual se quiere ir
#### 3. enterAnim: Tipo de animacion de entrada  // app:enterAnim="@android:anim/fade_in"
#### 4. popExitAnim: Tipo de animacion de salida // app:popExitAnim="@android:anim/slide_out_right"

### Hay que tener encuenta que dentro de un fragment o destination pueden haber varios actions


## COMO SE USA

#### LA IDEA ES QUE ASI COMO EN EL MAINACTIVITY PUEDE ESTAR COMPUESTO DE MUCHOS FRAGMENTS AHORA ESTE COMPUESTO POR EL NAVIGATION GRAPH

![](https://github.com/srodriguez9017/NavigationComponent/blob/master/images/MAINACTIVITY.JPG?raw=true)

#### ES DECIR DENTRO DEL  MAINACTIVITY.XML vA A VIVIR EL FRAGMENT QUE CONTIENE EL GRAFO DE NAVEGACION Y SE VA A CONOCER COMO EL NAVHOSTFRAGMENT

![](https://github.com/srodriguez9017/NavigationComponent/blob/master/images/NAV_INTO_MAINACTIVITY.JPG?raw=true)

#### EN ESTE EJEMPLO EL DEFAULTHOST INDICA QUE ESTE VA A SER EL PUNTO DE INICIO
#### Y EL NAVGRAPH INDICA CUAL VA A SER EL GRAFO DE NAVEGACION

#### AHORA BIEN PARA PODER ACCEDER A DICHOS ACTION Y DESTINATION VAMOS A USAR KOTLIN CON BOTONES Y ELMETODO ONCLICKLISTENER 
![](https://github.com/srodriguez9017/NavigationComponent/blob/master/images/XMLWITHKOTLIN.JPG?raw=true)




