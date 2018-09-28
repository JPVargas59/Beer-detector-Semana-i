## Beer-detector-Semana-i
Este archivo explica los pasos realizados para la creación del modelo detector de cervezas, la herramienta web para crear los XMLs necesarios para generar archivos TFRecords y por último la creación e implementación de el modelo exportado a CoreML para una aplicación iOS.

- [Herramienta etiquetado](#herramienta-web-para-etiquetado-etiquetado)
- [Modelo TF](#modelo)
- [Implenetación CoreML](#implenetación-coreml)
- [Autores](#autores)

# Herramienta web para etiquetado #etiquetado
Esta herramienta fue realizada en JS, HTML y CSS. Con ella se pueden generar archivos XML con el formato necesario para crear TFRecords. Además, permite descargar la misma información en JSON para poder manipular la información y convertirla a otros formatos de ser necesario e.g. formatos necesarios para YOLO y otros modelos.

El repositorio se encuentra [aquí](https://github.com/alfredofloresnt/label-images-tool)

# Modelo
Para crear el modelo, se utilizó Tensor Flow. Como modelo se escogió [mobilenet](https://arxiv.org/abs/1704.04861).
El dataset necesario fue creado por el equipo e incrementado mediante la modificación de algunos parametros de las fotografías como la temperatura para crear más información. Este modelo fue probado también en Raspberry Pi de manera exitosa. 

El repositorio se encuentra [aquí](https://drive.google.com/open?id=1VGBfodEMjlCZ6ZsxKyfoVOTxixXVbHHO)

# Implementación CoreML
Una vez creado el modelo, se exportó a CoreML para implementarlo en iOS. Esta aplicación detecta en vivo las cervezas, identifica el tipo de cerveza, permite pausar el "live feed" para ver detenidamente la imagen. También permite cambiar entre modelos para vizualizar cual funciona mejor. Otra de sus caracteristicas es que se puede utilizar una imagen del carrete.

El repositorio se encuentra [aquí](https://github.com/Alexhl09/ClasificadorCervezas)

# Autores
Los integrantes de el equipo "JPVR" quienes formaron parte de la creación de este proyecto son:
- Alejandro Hernández López
- Roberto Mendívil Castro
- Ricardo Adrían Cazares Rodríguez
- Alfredo Flores Nieto
- Juan Pablo Vargas Rodríguez
