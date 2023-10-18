# FUNBIO_Grupo2
Trabajo realizado por el grupo 2 del horario B401 para Fundamentos de Biodiseño.

## Proyecto
Crear un dispositivo ergonómico capaz de reconocer en poco tiempo patologías cardíacas basándose en los ruidos cardíacos. 

Con tecnologías como DTW (Dynamic time warping), MFCC (Mel-frequency cepstral coefficients) y la comparación en tiempo real de bases de datos, transformamos la señal sonora de los ruidos cardíacos que son señales de tensión analógica a señales discretas que sí se pueden almacenar de manera digital generándoles una huella digital a cada una.

Podemos mejorar la precisión del dispositivo derivando a 4 bases de datos, cada una por punto de auscultación ( aortico, pulmonar, mitral , tricúspide ).

![imagen de puntos de auscultacion](https://2.bp.blogspot.com/-py86LSAkiOs/XBVPghIt1lI/AAAAAAAAB7I/xJQcsX-Fv3c1lcXoAR7y8w-gOkYMRSYQACLcBGAs/s1600/focos%2Bauscultac%25C3%25AD%25C3%25B3n.png)

El dispositivo compara lo que escucha mediante un sensor de sonido y lo compara en la base de datos, reconociendo si las frecuencias corresponden a sonidos patológicos o saludables.


### Integrantes
* Renzo Alejandro Chafloque Bezares (Gestor del repositorio y GitHub)
* Ciro Jesús Francisco Rodriguez Córdova (Modelador de 3D)
* Carlos Andrés Ramos Guzmán (Electrónica)
* Axel Nicolas Jarama Salazar (Programador)
* Andrea Morelia Valero Canaza (Investigación y redacción)
* Camila Antonella Muchaypiña Mujica (Diseñadora del prototipo)

- ## Análisis 
- ### Problemática
Deficiencia en la detección de problemas cardíacos que desembocan en el empeoramiento de la salud de los afectados.

- ## Estado del arte
| Equipos | Características | Imágenes |
|------------|-----------------|-------------|
| Fonendoscopio electrónico Fonodx | Aplicación móvil para la graficación, grabación y comparación de sonidos fonocardiográficos.| ![imagen_Fonodx](https://cdn.discordapp.com/attachments/754876450049622172/1147011137775337472/image.png)|
| Estetoscopio inteligente| Uso de dos principales algoritmos con machine learning los cuales usan un estetoscopio móvil el cual se conecta a un celular android para reconocer y clasificar los sonidos del pulmón con uno de los algoritmos mientras que el otro compara la información recibida con su base de datos para predecir la condición del paciente.| ![imagen estetoscopio inteligente](https://www.bbvaopenmind.com/wp-content/uploads/2015/08/BBVA-OpenMind-estetoscopio-inteligente-MIT.ppal_-1-1.jpg)|
| Audio Search Algorithm | Tecnología de búsqueda de audio, que se puede utilizar en ambientes ruidosos. Se generan "huellas" transformando las frecuencias de los audios y guardandolas en bases de datos que se reconocen mediante algoritmos de comparación. |![imagen04](https://cdn.discordapp.com/attachments/754876450049622172/1147013698037223525/image.png)|

- ## Estado del arte 
- ### Productos Comerciales
- #### The 3M™ Littmann® CORE Digital Stethoscope
Un dispositivo de auscultacion cuya parte que entra en contacto con el paciente tiene un lado pediátrico y otro para adultos. Contiene un módulo de procesamiento de señales, un sensor de sonidos cardíacos y un módulo de comunicación inalámbrica. El dispositivo transmite los datos de ondas y sonidos cardíacos a un dispositivo para mostrar la información recogida. Con esto, el dispositivo logra enseñar los datos recogidos en tiempo real como si hubieran sido obtenidos por un electrocardiograma o un fonocardiograma. Además cuenta con una app el cual ofrece una IA que analiza en tiempo real los datos obtenidos mientras realiza una detección automática de patrones.

![Littman](https://m.media-amazon.com/images/I/610d1RfgHDL._AC_UF894,1000_QL80_.jpg)

- #### Shazam
Aplicación para dispositivos móviles capaz de reconocer canciones simplemente escuchando una breve muestra de la música. Los usuarios pueden activar la aplicación y hacer que escuche una canción que esté sonando en su entorno, ya sea en un lugar silencioso o con ruido, y la aplicación intentará identificarla.

![Shazam](https://i.blogs.es/75c220/shazam-android/1366_2000.jpg)

- #### MIT - App Estetoscopio
  Se le acopló un celular a un estetoscopio común para que evalúe los sonidos.

- ### Patentes
- The 3M™ Littmann® CORE Digital Stethoscope: WO2022123397A1
Es un estetoscopio el cual contiene un módulo de procesamiento de señales, un sensor de sonidos cardíacos y un módulo de comunicación inalámbrica. El dispositivo transmite los datos de ondas y sonidos cardíacos a un dispositivo para mostrar la información recogida. Con esto, el dispositivo logra enseñar los datos recogidos en tiempo real como si hubieran sido obtenidos por un electrocardiograma o un fonocardiograma. Además cuenta con una app el cual ofrece una IA que analiza en tiempo real los datos obtenidos mientras realiza una detección automática de patrones.


- The smart sthetoscope  (WO2016206704A1): Se le añade a un estetoscopio comun un dispositivo capaz de leer su señal y mostrarla al especialista medico para que este la pueda estudiar.

- Smart Telemedicine equipment (KR20140194385A): Dispositivo inteligente comprendido en un estetoscopio inteligente capaz de comprender y producir datos acerca de la hipofonesis (disminución de ruido torácico), a su vez, se encuentra conectada a una aplicación para su análisis.
- ## Lista de requerimientos




| Requerimientos funcionales | Requerimientos no funcionales |
|-----------------------------|--------------------------------|
| Crear una "huella digital" para los corazones de los pacientes | Fácil de usar |
| Monitorear continuamente | Ergonómico |
| Notificar cuando se detecten anomalías | Portable para el uso continuo |
| Almacenar la información obtenida | Inalámbrico |
| Adhesión al cuerpo del paciente | Barato |

- ### Propuesta de solución
Dispositivo que se utilice para auscultar pacientes capaz de comparar lo que escucha con una base de datos y de esta manera identificar patologías cardiacas . 
Este dispositivo encontrará el diagnostico sin importar la interferencia de ruido ambiental. 

![Caja negra](https://cdn.discordapp.com/attachments/754876450049622172/1153910115955658802/image.png)

![Caja negra - Esquema de funciones](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/9c570c1f-8b85-44c4-b78b-511716966165)

![Esquema de funciones](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/06f893c9-6282-40be-9b22-5bf38cef684a)

![Matriz morfológica](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/2246ce6d-696b-45ce-bf9d-36d4684211f6)

![Tabla de valoración](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/9d71ad04-f501-4eff-bf24-053842bc94ea)

![Conclusiones](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/f7807b66-64c0-4ebf-8463-250fca8e11cd)

![Boceto 1](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/f7b021aa-4864-424e-924c-a64bc4134fc9)


![Boceto 2](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/016701fb-c9fb-4050-bd94-4d645ccec4ad)


![Boceto 3](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/4be44a94-042f-4fd8-84e3-313632376551)

![image](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/cb2cc2f4-7e61-42a6-a19b-a0303403aaca)

![image1](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/3049a53a-8981-4359-9ce8-24c376a8683e)

![image2](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/6d321162-c7ab-4ad5-a111-383c04f52467)

## Presentación en OnShape
![OnShape](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/f18fc6b5-3ece-4fb1-92e7-ba6e3dfe90d7)
### https://cad.onshape.com/documents/ccb4649f5167b573fc4d6c1f/w/62f20a78f541022f94d4cff0/e/3bf2f79eb559771c0a301136?renderMode=0&uiState=652f6f370c57500896b0f2d9
## Presentación en Sketchfab
![Sketchfab](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/13a88922-0c86-4166-b476-f8fb5fa6f512)
### https://sketchfab.com/3d-models/entregable-5-e858c156c9ff40208f248848fea408b7

- ## Bibliografía
-  Avery Li-Chun Wang. Audio Search Algorithm https://www.ee.columbia.edu/~dpwe/papers/Wang03-shazam.pdf
-  Barbuzano J. A Smart Stethoscope you can Connect to a Mobile Phone to Diagnose Lung Diseases. Open Mind BBVA. 2015. URL: [https://www.bbvaopenmind.com/en/technology/innovation/a-smart-stethoscope-connects-to-a-mobile-phone-to-diagnose-lung-diseases/](https://www.bbvaopenmind.com/en/technology/innovation/a-smart-stethoscope-connects-to-a-mobile-phone-to-diagnose-lung-diseases/)
- D. B. Chamberlain, R. Kodgule and R. R. Fletcher, "A mobile platform for automated screening of asthma and chronic obstructive pulmonary disease," 2016 38th Annual International Conference of the IEEE Engineering in Medicine and Biology Society (EMBC), Orlando, FL, USA, 2016, pp. 5192-5195, doi: 10.1109/EMBC.2016.7591897.
- Ribeiro AH, Ribeiro MH, Paixão GMM, et al. Automatic diagnosis of the 12-lead ECG using a deep neural network. Nat Commun. 2020 [https://www.nature.com/articles/s41467-020-15432-4#citeas](https://www.nature.com/articles/s41467-020-15432-4#citeas)
- Jimenez Paz D.Prototipo de aplicacion movil para tratamiento de señales del fonendoscopio electronico Fonodx https://repository.unimilitar.edu.co/bitstream/handle/10654/32246/JimenezPazDanielDavid2019.pdf?sequence=1&isAllowed=y

