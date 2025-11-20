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

# Analizador Léxico en Flex
Proyecto académico realizado por Josue Avendaño Galarza.

## 1. Archivos necesarios
El proyecto requiere los siguientes archivos en la misma carpeta:

- lexer.l
- lex.yy.c
- lexer.exe
- input.c

El analizador está configurado para leer automáticamente el archivo input.c.

## 2. Cómo compilar el analizador léxico

### Usando Flex Windows (Lex and Yacc)
1. Abrir lexer.l en el programa
2. Menú Build → Compile Lex
3. Se generan los archivos:
   - lex.yy.c
   - lexer.exe

### Usando consola con GCC

## 3. Cómo ejecutar el analizador léxico
1. Abrir la carpeta donde está lexer.exe
2. En la barra de ruta del explorador escribir:
3. Presionar ENTER
4. Ejecutar:

## 4. Funcionamiento del analizador
El analizador:

- Abre automáticamente input.c
- Lee y analiza línea por línea
- Identifica y clasifica tokens
- Imprime cada token en el formato:

### Ejemplo de salida:
<RESERVED, int>
<ID, globalA>
<DELIM, ;>
<OPERATOR, =>
<NUMBER, 3>
