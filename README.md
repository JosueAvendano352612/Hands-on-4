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

Archivos necesarios

El proyecto debe contener los siguientes archivos en la misma carpeta:

lexer.l — Archivo del analizador léxico

lex.yy.c — Archivo generado por Flex

lexer.exe — Ejecutable compilado

input.c — Archivo de prueba que será analizado

El analizador está configurado para leer automáticamente el archivo input.c.

Cómo compilar el analizador léxico

Usando Flex Windows (Lex and Yacc):

Abrir lexer.l en el programa

Menú Build → Compile Lex

Esto genera lex.yy.c y lexer.exe

Usando GCC desde consola:
flex lexer.l
gcc lex.yy.c -o lexer.exe

Cómo ejecutar el analizador léxico

Abrir la carpeta donde está lexer.exe

Escribir en la barra de ruta: cmd

Presionar ENTER

Ejecutar:
lexer.exe

Funcionamiento del analizador
