# QuantumCoders

# IntelliPrice


## Tabla de contenidos

1. [Nombre](#Nombre)
2. [Descripción](#descripción)
3. [Arquitectura](#Arquitectura)
4. [Proceso](#Proceso)
5. [Funcionalidades](#Funcionalidades)
6. [Estado del proyecto](#EstadoDelProyecto)
7. [Agradecimientos](#Agradecimientos)


* IntelliPrice
Este proyecto se basa en un sofware que permite conocer a los usuarios donde conseguir sus productos preferidos a menor precio. El usuario tendrá la capacidad de preguntar sobre: Qué productos hay en la base de datos, qué sucursales pueden consultar, que productos hay en la sucursal específica y en que sucursales se encuentra un producto a menor precio.
![image](https://github.com/repositoriosHackaton/QuantumCoders/assets/158361126/83a1c5f0-5c7b-4317-a4df-58c01025e5fb)


* Arquitectura del proyecto
El proyecto se basa en un entorno de python que involucra un procesamiento de lenguaje natural para las solicitudes del usuario, luego seguido de un modelo de redes neuronales para conocer que exactamente el usuario necesita y luego semuestra la respuesta a la solicitud de la mano de una interfaz gráfica amigable e intuitiva.
![image](https://github.com/repositoriosHackaton/QuantumCoders/assets/158361126/4a34c6c9-a89b-47d2-9089-35f4d5cdc65c)


* Proceso de desarrollo:

1. El dataset fue extraido de esta fuente: https://www.kaggle.com/datasets/tinnqn/precios-claros-precios-de-argentina?select=productos.csv
2. En cuanto a la limpieza de datos se trabajo principalmente desde el csv en excel, pero, la mayor parte de la limpieza de los datos se realizo en la lematización de o y el procesado de los promts del usuario. Esto con procesamiento de lenguaje natural con ayuda de NLTK.
![image](https://github.com/repositoriosHackaton/QuantumCoders/assets/158361126/02156bf8-641c-44a1-9a29-2cef634ca385)
![image](https://github.com/repositoriosHackaton/QuantumCoders/assets/158361126/60cc9611-2782-4468-ae2d-21915dcb4cea)

3. ¿Qué modelo de Machine Learning están usando?
En este proyecto se está utilizando una red neuronal en tensorflow son 5 capas:
- Capa de entrada densa con 128 neuronas con activación ReLU
- Dos capas ocultas densas con activación  ReLU y dropout del 50% para evitar overfits
- Capa densa con activación softmax con un número de neuronas igual a train_y
Este modelo se entrena en base a intents que pasan por su debido procesamiento para entrenar el modelo.
4. En este modelo se evalua en base a metrica de accuracy

* Funcionalidades extra:

Desarrollo de interfaz gráfica de usuario
- Para el desarrollo de la interfaz gráfica se utilizó la librería tkinter siguiendo la línea gráfica utilizada a lo largo del proyecto.
![image](https://github.com/repositoriosHackaton/QuantumCoders/assets/158361126/3185a247-7750-4e3f-856c-517128e087e1)



