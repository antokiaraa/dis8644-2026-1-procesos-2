# sesion-10b

## Referencias
- Tega Brain  
- Everest Pipkin

En esta clase vimos diferentes dudas, entre todos nos ayudamos y se resulvieron muchas que yo también tenía:) a si que esta clase fue de mucha ayuda!!!!!!!!!

---

##  Conceptos de PCBs
- Las PCBs se conectan de diferentes maneras a la electricidad.  
- Se pueden unir circuitos en una misma placa, pero **Aaron recomendó hacerlo por separado**, ya que cada una actúa sola.  

---

##  chips
- **Dual In-Line Package (DIP)**  
- **SOIC Package**  
- El **DIP 7.62 mm (longpads)** es el más típico y el que usaremos.  

---

## edición de símbolos en KiCad
- Seleccionar chip → tecla **E** → *Edit Symbol*.  
- Cambiar orden del chip, letra, nombre de pines.  
- Mover con tecla **M**.  
- Guardar con **Ctrl+S**.  

---

## Botones 
- **Temporales**: pulsadores, timbres, pushbuttons.  
- **Tipos**:  
  - NO (Normally Open / Abierto).  
  - NC (Normally Closed / Conectado).
   ![nonc](./imagenes/nonc.png).
- **Interruptores**:  
  - SPST → 2 patitas  
  - SPDT → 3 patitas  
  - DPST → 4 patitas  
  - DPDT → 6 patitas  
- **Toggle**: palanca / switch.  
- Para encontrarlos: buscar **SW_SPST** o **SW_SPDT**.  
- Asignar huella: `[Button_Switch_THT:SW_PUSH_6mm]`.  


## Bibliotecas de símbolos
- Crear carpeta propia en **Symbol Editor** dentro del proyecto `.pro`.  
- Menú: **View → Panels → Library Tree**.  
- Activar bibliotecas → **File → New Library** → guardar.  
- Copiar componente → pegar en carpeta → editar → guardar.  


## Etiquetas
- Conectar sin cableado en esquemático: tecla **L** (Label).  
- Evita error de pin no conectado.  
- Desde batería: usar etiqueta **PWG_FLAG**.  

- Cambiar de cara componentes: seleccionar → tecla **F**.  

---

## 3D
- Seleccionar huella en `.pcb` → tecla **E** → menú **3D Models** → cargar modelos descargados.  
- Exportar placa completa: **File → Export → STEP/STL/etc.**

Cap 2 y 3 

  
 
