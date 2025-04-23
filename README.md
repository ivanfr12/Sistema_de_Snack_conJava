# 🥪 Máquina de Snacks en Java

Este es un proyecto simple de consola en Java que simula una máquina expendedora de snacks. Permite al usuario comprar productos, ver un ticket de compra, agregar nuevos snacks e inspeccionar el inventario actual. Hay dos implementaciones posibles: una basada en archivos (`ServicioSnackArchivos`) y otra en memoria (`ServicioSnacksLista`).

## 🚀 Funcionalidades

- Comprar snacks por ID
- Mostrar ticket con el total de la compra
- Agregar nuevos productos al sistema
- Mostrar el inventario actual
- Persistencia de datos en archivo de texto (`snacks.txt`)

## 🧱 Estructura del Proyecto

bash
maquina-snacks-java/
│
├── maquina_snacks_archivos/
│   ├── dominio/
│   │   └── Snack.java
│   ├── presentacion/
│   │   └── MaquinaSnacks.java
│   └── servicio/
│       ├── IServicioSnacks.java
│       ├── ServicioSnackArchivos.java
│       └── ServicioSnacksLista.java
└── snacks.txt  # Se crea automáticamente si no existe

🛠️ Tecnologías Usadas
Java 17+ (o compatible con versiones anteriores)

Programación orientada a objetos

Manejo de archivos (java.io y java.nio.file)

▶️ Cómo Ejecutar
Clona este repositorio:

git clone https://github.com/ivanfr12/Sistema_de_Snack_conJava.git
cd maquina-snacks-java

Compila el proyecto:

bash
javac maquina_snacks_archivos/**/*.java

Ejecuta la aplicación:
java maquina_snacks_archivos.presentacion.MaquinaSnacks

📄 Ejemplo de Uso:
*** Maquina de Snacks ***
--- Snacks en el Inventario ---
Snack{idSnack=1, nombre='Papas', precio=70.0}
Snack{idSnack=2, nombre='Refresco', precio=50.0}
...

Menu:
1. Comprar snack
2. Mostrar ticket
3. Agregar Nuevo Snack
4. Inventario de Snack
5. Salir
Elige una opcion:


📦 Persistencia de Datos
Si se utiliza ServicioSnackArchivos, los snacks se guardan en un archivo snacks.txt, lo que permite mantener el inventario entre sesiones.

✨ Autor
Proyecto desarrollado por Ivan Rodriguez como parte de un ejercicio de práctica en Java.
