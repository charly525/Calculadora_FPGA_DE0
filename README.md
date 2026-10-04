# Calculadora_FPGA_DE0
Este repositorio contiene el diseño, código VHDL y archivos de síntesis de una calculadora digital con arquitectura modular, desarrollada e implementada sobre la tarjeta de desarrollo **Terasic DE0 (Altera/Intel Cyclone III EP3C16F484)**.

## Características principales
- **Operaciones soportadas:** Suma, Resta (con representación de signo-magnitud), Multiplicación BCD y operaciones lógicas.
- **Entradas:** Configuración mediante los interruptores (`SW[9..0]`) y selección/prioridad de funciones mediante botones/pulsadores (`BTN`).
- **Salidas:** Visualización del estado, operandos y resultado traducido a BCD en los 4 displays de 7 segmentos de ánodo común (`HEX3..HEX0`).
- **Gestión de Errores e Indicadores:** Detección de sobreflujo (*overflow*), representación de números negativos (`-`) e indicación de error de entrada fuera del rango BCD (representado con `E` en pantalla y `LEDG9`).
- **Modo de prueba:** Rutina de testeo de segmentos (*hardware test*) al presionar el botón de prueba (`BTN2`).

## Herramientas y Tecnologías
- **Lenguaje de Descripción de Hardware:** VHDL
- **EDA / Software de Síntesis:** Intel Quartus Prime / Quartus II 13.0sp1
- **Dispositivo Objetivo:** FPGA Cyclone III - EP3C16F484C6 (Terasic DE0)
