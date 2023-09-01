# FUNBIO_Grupo2
Trabajo realizado por el grupo 2 del horario B401 para Fundamentos de Biodiseño

## Proyecto
Crear un dispositivo ergonómico capaz de reconocer en poco tiempo patologías cardiacas basándose en los ruidos cardiacos. 
Con tecnologías como DTW (Dynamic time warping), MFCC (Mel-frequency cepstral coefficients) y la comparación en tiempo real de bases de datos, transformamos la señal sonora de los ruidos cardiacos que son señales de tensión analógica a señales discretas que si se pueden almacenar de manera digital generándoles una huella digital a cada una.
Podemos mejorar la precisión del dispositivo derivando a 4 bases de datos, cada una por punto de auscultación ( aortico, pulmonar, mitral , tricúspide ) 

 ![imagen de puntos de auscultacion](https://2.bp.blogspot.com/-py86LSAkiOs/XBVPghIt1lI/AAAAAAAAB7I/xJQcsX-Fv3c1lcXoAR7y8w-gOkYMRSYQACLcBGAs/s1600/focos%2Bauscultac%25C3%25AD%25C3%25B3n.png)

El dispositivo compara lo que escucha mediante un sensor de sonido y lo compara en la base de datos, reconociendo si las frecuencias corresponden a sonidos patológicos o saludables.


### Integrantes
* Renzo Alejandro Chafloque Bezares (Gestor del repositorio y GitHub)
* Ciro Jesús Francisco Rodriguez Córdova (Modelador de 3D)
* Carlos Andrés Ramos Guzmán (Electronica)
* Axel Nicolas Jarama Salazar (Programador)
* Andrea Morelia Valero Canaza (Sin definir rol)
* Camila Antonella Muchaypiña Mujica (Diseñadora del prototipo)

- ## Analizando el contexto
- ### Caso (ejemplo)
- ### Problemática
Detección de patologías cardíacas en base a la auscultulación de los ruidos cardíacos
- ## Estado del arte
| Equipos | Características | Imágenes |
|------------|-----------------|-------------|
| Fonendoscopio electrónico Fonodx | Aplicacion movil para la graficacion, grabacion y comparacion de sonidos fonocardiograficos| ![imagen_Fonodx](https://cdn.discordapp.com/attachments/754876450049622172/1147011137775337472/image.png)|
| Estetoscopio inteligente| Uso de dos principales algoritmos con machine learning los cuales usan un estetoscópio móvil el cual se conecta a un celular android para reconocer y clasificar los sonidos del pulmón con uno de los algoritmos mientras que el otro compara la información recibida con su base de datos para predecir la condición del paciente| ![imagen estetoscopio inteligente](https://www.bbvaopenmind.com/wp-content/uploads/2015/08/BBVA-OpenMind-estetoscopio-inteligente-MIT.ppal_-1-1.jpg)|
| Audio Search Algorithm | Tecnologia de busqueda de audio, que se puede utilizar en ambientes ruidosos. Se generan "huellas" transformando las frecuencias de los audios y guardandolas en bases de datos que se reconocen mediante algoritmos de comparacion. 
|Deep Neuronal Network DNN|Uso de machine learning para crear una red neuronal profunda que es entrenada alimentándola de datos para poder reconocer abnormalidades que aparecen en exámenes al corazón de diferentes pacientes equiparando la eficiencia de un electrocardiograma de 12 derivaciones| |
- ## Bibliografía
-  Avery Li-Chun Wang. Audio Search Algorithm https://www.ee.columbia.edu/~dpwe/papers/Wang03-shazam.pdf
-  Barbuzano J. A Smart Stethoscope you can Connect to a Mobile Phone to Diagnose Lung Diseases. Open Mind BBVA. 2015. URL: [https://www.bbvaopenmind.com/en/technology/innovation/a-smart-stethoscope-connects-to-a-mobile-phone-to-diagnose-lung-diseases/](https://www.bbvaopenmind.com/en/technology/innovation/a-smart-stethoscope-connects-to-a-mobile-phone-to-diagnose-lung-diseases/)
- D. B. Chamberlain, R. Kodgule and R. R. Fletcher, "A mobile platform for automated screening of asthma and chronic obstructive pulmonary disease," 2016 38th Annual International Conference of the IEEE Engineering in Medicine and Biology Society (EMBC), Orlando, FL, USA, 2016, pp. 5192-5195, doi: 10.1109/EMBC.2016.7591897.
- Ribeiro AH, Ribeiro MH, Paixão GMM, et al. Automatic diagnosis of the 12-lead ECG using a deep neural network. Nat Commun. 2020 [https://www.nature.com/articles/s41467-020-15432-4#citeas](https://www.nature.com/articles/s41467-020-15432-4#citeas)
- Jimenez Paz D.Prototipo de aplicacion movil para tratamiento de señales del fonendoscopio electronico Fonodx https://repository.unimilitar.edu.co/bitstream/handle/10654/32246/JimenezPazDanielDavid2019.pdf?sequence=1&isAllowed=y
