# Hands-on-4
Crear Analizador Léxico

Josue Avendaño Galarza

Descripción
Este proyecto implementa un analizador léxico utilizando Flex para reconocer los tokens principales de un subconjunto del lenguaje C.
El analizador procesa un archivo de entrada escrito en C y muestra los tokens identificados junto con su lexema correspondiente.

Objetivo
Reconocer los siguientes elementos del lenguaje C: Palabras reservadas: int, float, double, char, void, short, return, include, define
Identificadores
Literales numéricos
Operadores: +, -, *, /, ++, =
Delimitadores: ( ), { }, ; ,
Comentarios: /* */ y //
Espacios en blanco (ignorados)
Archivos del proyecto
lexer.l — Archivo principal del analizador léxico
input.c — Código en C utilizado como entrada de prueba
lex.yy.c — Archivo generado por Flex
lexer.exe — Ejecutable generado (después de compilar)

Tecnologías utilizadas
Flex
GCC (o compilador equivalente)
Entorno: Flex Windows (Lex and Yacc)

Instrucciones de uso
1. Generar lex.yy.c con Flex
Abrir el archivo lexer.l en Flex Windows y usar la opción
Tools → Run Flex / Lex-Flex
Esto generará el archivo lex.yy.c.

Ejemplo de salida
Para la línea:
globalA = 3;
