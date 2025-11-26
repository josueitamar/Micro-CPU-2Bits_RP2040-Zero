# Micro-CPU 2Bits

## Autores

1.

2. 


##  Objetivo
El objetivo de este proyecto es construir un modelo funcional y simplificado de una Unidad Central de Procesamiento (CPU) utilizando una placa RP2040 Zero. El proyecto simula:

1.  **El Ciclo de Instrucción:** Visualización de las fases *Fetch, Decode, Execute y Write-Back* mediante LEDs.
2.  **Banderas de Estado (Flags):** Indicadores visuales para *Zero, Negative* y *Overflow*.
3.  **Calculadora de 2 Bits:** Capacidad para realizar operaciones de suma y resta con números del 0 al 3.

Instrucciones de Uso:

 Carga del Código
1.  Conecta la placa RP2040 Zero a tu computadora mediante USB-C.
2.  Abre **Thonny IDE**.
3.  Asegúrate de tener instalado el intérprete de MicroPython en la placa.
4.  Abre el archivo `main.py` ubicado en la carpeta `CODE/`.
5.  Guarda el archivo en la placa con el nombre `main.py` para que se ejecute automáticamente al encenderla.

Operación de la Calculadora
El sistema funciona como una máquina de estados. Sigue esta secuencia:

1.  **Estado Inicial:** El sistema espera el primer número.
2.  **Paso 1 (Operando 1):** Presiona un botón numérico (0, 1, 2 o 3).
3.  **Paso 2 (Operación):** Presiona el botón de suma (`+`) o resta (`-`).
4.  **Paso 3 (Operando 2):** Presiona el segundo número (0, 1, 2 o 3).
5.  **Paso 4 (Resultado):** Presiona el botón igual (`=`).
    * Se iluminarán los LEDs correspondientes al ciclo de instrucción.
    * El resultado aparecerá en el display.
    * Si hay un error (Overflow), el LED RGB se encenderá en rojo.
6.  **Reinicio:** Presiona `=` nuevamente para reiniciar el sistema.
