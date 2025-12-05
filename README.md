# Contact-agenda-table 

Pequeña aplicación de consola desarrollada en Python que muestra una agenda de contactos en formato tabular.  
Este proyecto demuestra el uso de **listas**, **diccionarios**, **formateo de texto**, y **funciones modulares** en Python.

## Tabla de Contenido
- [Descripción](#descripción)
- [Características](#características)
- [Estructura del proyecto](#estructura-del-proyecto)
- [Tecnologías](#tecnologías)
- [Cómo ejecutar](#cómo-ejecutar)
- [Código principal](#código-principal)
- [Ejemplo de salida](#ejemplo-de-salida)
- [Autor](#autor)

## Descripción
Este proyecto implementa una agenda de contactos simple en interfaz de consola.  
Permite recorrer y visualizar una lista de contactos utilizando alineación con **f-strings** para mostrar una tabla ordenada.
## Características
- Recorrido de una lista de diccionarios.
- Impresión tabular con formatos `:<10` y `:>10`.
- Función modular `recorrer_Agenda()`.
- Código claro y fácil de entender para principiantes.
  
## Estructura del proyecto

contact-agenda-table/
- **agenda.py** - Script principal con la lógica de la agenda
- **README.md** - Documentación del proyecto (este archivo)

## Tecnologías
- Python 3
- Estructuras de datos (listas y diccionarios)
- f-strings avanzados

## Cómo ejecutar
```bash
git clone https://github.com/LeonidasDiaz/contact-agenda-table.git
cd contact-agenda-table
python agenda.py
```


## Código principal
```python
def recorrer_Agenda(contactos):
    """Función que recorre la agenda y muestra los contactos en una tabla"""
    print(f"{'Nombre':<10} | {'Telefono':>10}")
    print("-" * 23)
    for contacto in contactos:
        print(f"{contacto['nombre']:<10} | {contacto['telefono']:<10}")


def main():
    Agenda_contactos = [
        {"nombre": "Pedro", "telefono": 9381234490},
        {"nombre": "Ana", "telefono": 9382334490},
        {"nombre": "David", "telefono": 9381924490}
    ]
    
    recorrer_Agenda(Agenda_contactos)


if __name__ == "__main__":
    main()

```


## Ejemplo de salida
```
Nombre     |   Teléfono
-----------------------
Pedro      | 9381234490
Ana        | 9382334490
David      | 9381924490

```



## Autor
### Leonidas Diaz
GitHub: [@LeonidasDiaz](https://github.com/LeonidasDiaz)
