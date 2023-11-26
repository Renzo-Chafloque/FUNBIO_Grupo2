# FUNBIO_Grupo2
![Introducción](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/b3adea1a-0cb6-4d95-a49e-5f50b8332582)


## Proyecto
Crear un dispositivo ergonómico capaz de reconocer en poco tiempo patologías cardíacas basándose en los ruidos cardíacos. 

Con tecnologías como DTW (Dynamic time warping), MFCC (Mel-frequency cepstral coefficients) y la comparación en tiempo real de bases de datos, transformamos la señal sonora de los ruidos cardíacos que son señales de tensión analógica a señales discretas que sí se pueden almacenar de manera digital generándoles una huella digital a cada una.

Podemos mejorar la precisión del dispositivo derivando a 4 bases de datos, cada una por punto de auscultación (aórtico, pulmonar, mitral, tricúspide ).

![imagen de puntos de auscultacion](https://2.bp.blogspot.com/-py86LSAkiOs/XBVPghIt1lI/AAAAAAAAB7I/xJQcsX-Fv3c1lcXoAR7y8w-gOkYMRSYQACLcBGAs/s1600/focos%2Bauscultac%25C3%25AD%25C3%25B3n.png)

El dispositivo compara lo que escucha mediante un sensor de sonido y lo compara en la base de datos, reconociendo si las frecuencias corresponden a sonidos patológicos o saludables.


- ## Análisis
![contexto1](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/b0ef2d5f-01c6-420e-9da5-01a9ccf8b63b)
![contexto2](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/9a597962-7199-4f98-b301-1542e5944528)
![contexto3](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/d85ff84d-8453-40ba-bdbd-6eaf7a19d478)
![contexto4](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/2064fb92-e5a7-4c5a-b2c5-d26820188d18)
![contexto5](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/046da19a-49ac-40e7-9361-57676e00e108)


- ### Problemática
Deficiencia en la detección de problemas cardíacos que desembocan en el empeoramiento de la salud de los afectados.

- ## Estado del arte
| Equipos | Características | Imágenes |
|------------|-----------------|-------------|
| Fonendoscopio electrónico Fonodx | Aplicación móvil para la graficación, grabación y comparación de sonidos fonocardiográficos.| ![imagen_Fonodx](https://cdn.discordapp.com/attachments/754876450049622172/1147011137775337472/image.png)|
| Estetoscopio inteligente| Uso de dos principales algoritmos con machine learning los cuales usan un estetoscopio móvil el cual se conecta a un celular android para reconocer y clasificar los sonidos del pulmón con uno de los algoritmos mientras que el otro compara la información recibida con su base de datos para predecir la condición del paciente.| ![imagen estetoscopio inteligente](https://www.bbvaopenmind.com/wp-content/uploads/2015/08/BBVA-OpenMind-estetoscopio-inteligente-MIT.ppal_-1-1.jpg)|
| Audio Search Algorithm | Tecnología de búsqueda de audio, que se puede utilizar en ambientes ruidosos. Se generan "huellas" transformando las frecuencias de los audios y guardandolas en bases de datos que se reconocen mediante algoritmos de comparación. |![imagen04](https://cdn.discordapp.com/attachments/754876450049622172/1147013698037223525/image.png)|
