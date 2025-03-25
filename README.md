# criptografia-tarea-DE
Tarea de Diffie Helman
Aquí tienes un ejemplo de texto para el `README.md` en GitHub para tu tarea de criptografía sobre el algoritmo de intercambio de claves Diffie-Hellman:

```markdown
# Intercambio de Claves Diffie-Hellman

Este programa implementa el algoritmo de intercambio de claves Diffie-Hellman en lenguaje C. El objetivo principal de este programa es permitir a dos partes (Alice y Bob) generar una clave secreta compartida de manera segura, a través de un canal no seguro, sin necesidad de que intercambien directamente la clave.

## Descripción

El algoritmo Diffie-Hellman permite que dos partes acuerden una clave secreta mediante el uso de un número primo y un generador. Ambas partes generan claves públicas mediante el cálculo de potencias modulares, y luego intercambian estas claves públicas. Finalmente, calculan la clave compartida utilizando la clave privada de cada uno y la clave pública del otro. Si ambas partes hacen los cálculos correctamente, terminarán con la misma clave secreta compartida.

## Funcionamiento

El programa realiza los siguientes pasos:
1. Solicita al usuario ingresar un número primo \( p \) y un generador \( g \) tal que \( 0 < g < p \).
2. Pide a los usuarios (Alice y Bob) ingresar sus claves privadas \( a \) y \( b \).
3. Calcula las claves públicas \( A \) y \( B \) de Alice y Bob, respectivamente, utilizando la función de exponentiación modular.
4. Permite que Alice y Bob calculen la clave secreta compartida usando las claves públicas del otro.
5. Verifica si ambas partes calculan la misma clave secreta.

## Ejemplo de Ejecución

```
=== Intercambio de claves Diffie-Hellman ===
Escribe 'X' en cualquier momento para salir.

Ingresa un número primo (p): 23
Ingresa un generador (g) tal que 0 < g < p: 5
Ingresa la clave privada (a): 6
Ingresa la clave privada (b): 15

Clave pública de Alice (A): 8
Clave pública de Bob (B): 19

Clave compartida calculada por Alice: 2
Clave compartida calculada por Bob: 2

Ambas partes tienen la misma clave secreta.
```

## Requisitos

Este programa está escrito en C y utiliza las siguientes librerías estándar:
- `<stdio.h>`
- `<stdlib.h>`
- `<string.h>`

## Instrucciones para Ejecutar

1. Clona este repositorio en tu máquina local:

   git clone https://github.com/tu_usuario/cryptography-diffie-hellman.git
   ```
   
2. Accede al directorio del proyecto:

   cd cryptography-diffie-hellman
   ```

3. Compila el programa:
   ```bash
   gcc Deffie_Helman.c -o diffie_hellman
   ```

4. Ejecuta el programa:
   ```bash
   ./diffie_hellman
   ```

## Notas

- El programa permite al usuario elegir sus propios valores para el número primo \( p \), el generador \( g \), y las claves privadas \( a \) y \( b \).
- El programa verifica que el generador sea válido y que las claves privadas sean positivas.
- Si las claves secretas compartidas coinciden, el intercambio de claves fue exitoso.

## Licencia

Este proyecto está bajo la Licencia MIT. Consulta el archivo `LICENSE` para más detalles.
```
