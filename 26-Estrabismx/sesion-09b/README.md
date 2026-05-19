# sesion-09b

## KiCad pt3: El regreso ##

Se inicio con una revisión de dudas generales, donde lo que más rescato es la nomenclatura de los chips o tambien llamados IC

![Descarga](./imagenes/ic.webp)

> Nosotros estamos trabajando con los tipo DIP

<br>

Otro punto fue la distinción de los botones, donde tenemos _push botton_ y _switch_

- Push botton: Existen los NO (Normally Open) y NC (Normally Close), estos se diferencian en cual es el estado que se mantiene como base (sin presionar)

> Los NO son los más comunes, que la energía solo fluye al presionar. En cambio los NC al presionar se detiene el flujo de electrones

![Switch](./imagenes/buttons.jpg)

<br>

- Switch:  A diferencia de los botones, estos recuerdan el estado en el que se los deja, existen diversas configuraciones

![Switch](./imagenes/switch.png)

> S: Single / Único
>
> D: Double / Doble
>
> P: Pole / Polo
>
> T: Throw / Tiro 

![Switch](./imagenes/switch.webp)

> Tanto PushBotton como Switchs SPST se pueden representar con el mismo símbolo

<br>

### Edición de huellas, símbolos y modelos 3D ###

#### Huellas ####




### Investigación Secunciador ###



- Considerar que el 4017 utilizado es un **CONTADOR**, buscar funcionamiento detrás de esta cuenta, para saber que chips tienen funciones similar o algo que nos pueda servir

- Encontré un chip que nos podría servir, el 4520, es un contador binario,  es decir que vamos a tener por ej 4 luces

    + A prende cada tick
 
    + B prende cada 2 tick
 
    + C Prende cada 4 tick
 
    + D Prende cada 8 tick
 
  Por lo que podemos tener 4 _"ritmos posilbes"_

- Otro posible IC es el 4510

- 74LS90

- 4006 ????

- 4020

- **4022** >> https://www.youtube.com/watch?v=5Trjze02Wm4

- **4013**


- Pagínas de referencia:

  * https://www.youtube.com/watch?v=7lM8bY7qF8U >>> UTILIZA TRANSISTORES PARA LOS LED 

  + https://www.quora.com/Is-there-any-equivalent-chip-for-IC-4017-used-in-a-frequency-divider-circuit-using-a-555-timer
  
  + https://audiomaquinas.com/86-sintetizadores-diy/

  + https://www.birthofasynth.com/Scott_Stites/Pages/Klee_Birth.html
    
    + https://djjondent.blogspot.com/2017/08/cmos-useful-chips-for-lunetta-synths.html?m=1

      + https://www.youtube.com/watch?v=2KUbxQgD6hk
