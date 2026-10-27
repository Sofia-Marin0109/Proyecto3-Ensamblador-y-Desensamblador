# Pruebas del Proyecto 3 - Organización de Computadores

## 1. Programas Válidos (Ensamblador)
* **CopyBlock.asm:** Genera CopyBlock.hack idéntico al oficial. Es un algoritmo que copia datos entre una memoria de origen y destino usando punteros.
* **DibujarPatron.asm:** Genera DibujarPatron.hack idéntico al oficial. Dibuja un patrón punteado vertical en el lado izquierdo de la pantalla iterando 256 veces.
* **LlenarMemoria.asm:** Genera LlenarMemoria.hack idéntico al oficial. Escribe el valor 7 en un bloque consecutivo de memoria, usando R0 como puntero base y R1 como longitud.

## 2. Programas Válidos (Desensamblador)
* **BucleSuma.hack:** Genera BucleSumaDis.asm. Prueba la reconstrucción de un bucle `while` con una etiqueta de retorno y una etiqueta de salida. Al ensamblarlo nuevamente, el binario es idéntico al original.
* **Intercambio.hack:** Genera IntercambioDis.asm. Prueba un bloque de manipulación de memoria lineal usando una variable temporal, finalizando con un salto infinito.
* **ValorAbsoluto.hack:** Genera ValorAbsolutoDis.asm. Prueba la reconstrucción de un salto condicional hacia adelante (bifurcación `if-else` implícita).

## 3. Casos de Error Esperados (Ensamblador)
* **ErrorInstruccionA.asm:** ERROR *** Línea 5: valor fuera de rango '32768' (máximo 32767)
* **ErrorEtiqueta.asm:** ERROR *** Línea 15: nombre de etiqueta inválido '%STOP'
* **ErrorDestino.asm:** ERROR *** Línea 21: destino inválido 'DM'
* **ErrorComputo.asm:** ERROR *** Línea 23: Cómputo inválido o no existe en la tabla 'M+D' (Asumiendo corrección de la línea 20)
* **ErrorSalto.asm:** ERROR *** Línea 18: salto inválido 'jmp'
* **ErrorEstructura.asm:** ERROR *** Línea 6: la instrucción tiene más de un '='

## 4. Casos de Error Esperados (Desensamblador)
* **ErrorLongitud.hack:** ERROR *** Línea 7: longitud inválida: tiene 15 caracteres y deben ser 16
* **ErrorCaracteres.hack:** ERROR *** Línea 6: carácter inválido 'A' en la posición 9
* **ErrorBits.hack:** ERROR *** Línea 5: los bits 14 y 13 de una instrucción C deben ser 11
* **ErrorComputoDis.hack:** ERROR *** Línea 6: código de cómputo inválido '0000001'