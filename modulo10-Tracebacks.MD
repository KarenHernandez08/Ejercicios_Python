
# Uso de tracebacks para buscar errores
## Tracebacks
Un traceback es el cuerpo del texto que puede apuntar al origen (y al final) de un error no controlado. Comprender los componentes de un traceback hará que seas más eficaz al corregir errores o depurar un programa que no funciona bien.

Intenta crear un archivo de Python y asígnale el nombre open.py, con el contenido siguiente:

![alt text](https://github.com/KarenHernandez08/Ejercicios_Python/blob/main/Imagenes/open.PNG)

Se trata de una sola función main() que abre el archivo inexistente, como antes. Al final, esta función usa un asistente de Python que indica al intérprete que ejecute la función main() cuando se le llama en el terminal. Ejecútala con Python y podrás comprobar el siguiente mensaje de error:

![alt text](https://github.com/KarenHernandez08/Ejercicios_Python/blob/main/Imagenes/error.PNG)

## Try y Except de los bloques
Vamos a usar el ejemplo de navegador a fin de crear código que abra archivos de configuración para la misión de Marte. Los archivos de configuración pueden tener todo tipo de problemas, por lo que es fundamental notificarlos con precisión cuando se presenten. Sabemos que, si no existe un archivo o directorio, se genera FileNotFoundError. Si queremos controlar esa excepción, podemos hacerlo con un bloque try y except:
![alt text](https://github.com/KarenHernandez08/Ejercicios_Python/blob/main/Imagenes/try.PNG)

Después de la palabra clave try, agregamos código que tenga la posibilidad de producir una excepción. A continuación, agregamos la palabra clave except junto con la posible excepción, seguida de cualquier código que deba ejecutarse cuando se produce esa condición. Puesto que config.txt no existe en el sistema, Python imprime que el archivo de configuración no está ahí. El bloque try y except, junto con un mensaje útil, evita un seguimiento y sigue informando al usuario sobre el problema.

Aunque es común un archivo que no existe, no es el único error que podemos encontrar. Los permisos de archivo no válidos pueden impedir la lectura de un archivo, incluso si este existe. Vamos a crear un archivo de Python denominado config.py. El archivo tiene código que busca y lee el archivo de configuración del sistema de navegación:
![alt text](https://github.com/KarenHernandez08/Ejercicios_Python/blob/main/Imagenes/config.PNG)

