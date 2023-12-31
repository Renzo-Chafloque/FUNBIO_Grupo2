# FUNBIO_Grupo2
![Introducción](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/b3adea1a-0cb6-4d95-a49e-5f50b8332582)


## Proyecto
Crear un dispositivo ergonómico capaz de reconocer en poco tiempo patologías cardíacas basándose en los ruidos cardíacos. 

Con tecnologías como DTW (Dynamic time warping), MFCC (Mel-frequency cepstral coefficients) y la comparación en tiempo real de bases de datos, transformamos la señal sonora de los ruidos cardíacos que son señales de tensión analógica a señales discretas que sí se pueden almacenar de manera digital generándoles una huella digital a cada una.

Podemos mejorar la precisión del dispositivo derivando a 4 bases de datos, cada una por punto de auscultación ( aortico, pulmonar, mitral , tricúspide ).

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

![introducción2](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/8f18f125-933b-4f59-bae7-9d464c5aa3a3)

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
| Adherir al cuerpo del paciente | Barato |

- ### Propuesta de solución
Dispositivo que se utilice para auscultar pacientes capaz de comparar lo que escucha con una base de datos y de esta manera identificar patologías cardiacas . 
Este dispositivo encontrará el diagnostico sin importar la interferencia de ruido ambiental. 

![introducción3](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/b8f8f0b1-0c7a-429d-9455-ff4960b0964d)


![Caja negra](https://cdn.discordapp.com/attachments/754876450049622172/1153910115955658802/image.png)

![Caja negra - Esquema de funciones](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/9c570c1f-8b85-44c4-b78b-511716966165)

![Esquema de funciones](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/06f893c9-6282-40be-9b22-5bf38cef684a)

![Matriz_morfológica](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/eb520460-b3c0-4af9-9f88-491a073422e7)

![Tabla de valoración](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/7e93854a-18b4-4fbc-a6f8-7ad85995d696)


![Conclusiones](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/f7807b66-64c0-4ebf-8463-250fca8e11cd)

![introducción4](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/3a132815-5cde-4e2d-ac32-2f6704448ea7)


![Boceto 1](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/f7b021aa-4864-424e-924c-a64bc4134fc9)


![Boceto 2](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/016701fb-c9fb-4050-bd94-4d645ccec4ad)


![Boceto 3](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/4be44a94-042f-4fd8-84e3-313632376551)


![Matriz_evaluación_técnica](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/2a242f1b-7a4e-4355-98ac-9785b64ae54e)
![Matriz_evaluación_económica](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/6c34e991-c6d6-4878-88e4-e0add3c78573)
![Proyecto_óptimo](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/5dea3e07-bf5d-49ab-99ff-ff87ac9c63c6)

![introducción5](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/cb1addce-73b8-4343-82ef-2e6636b9b681)

## Esquema electrónico
![Esquema_electrónico](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/68ddb5d3-6c65-4dec-b951-7e2604b6e2a7)


## Presentación en OnShape
![OnShape](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/f18fc6b5-3ece-4fb1-92e7-ba6e3dfe90d7)
### https://cad.onshape.com/documents/ccb4649f5167b573fc4d6c1f/w/62f20a78f541022f94d4cff0/e/3bf2f79eb559771c0a301136?renderMode=0&uiState=652f6f370c57500896b0f2d9
## Presentación en Sketchfab
![Sketchfab](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/13a88922-0c86-4166-b476-f8fb5fa6f512)
### https://sketchfab.com/3d-models/entregable-5-e858c156c9ff40208f248848fea408b7

## Presentación del hito 1:
[Presentación - Hito 1 (2).pptx](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/files/13170926/Presentacion.-.Hito.1.2.pptx)

![Introducción 6](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/8984b467-5674-4b4f-a692-705cc2e6598f)

![imagen circuito](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/a5cc597e-8f98-4bbf-9f5b-994a5c6605ce)

[Diagrama del circuito.pdf](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/files/13246999/Diagrama.del.circuito.pdf)

![imagen aplicación](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/cf576534-f159-4b10-a43c-682f459c6809)

[Diagrama de aplicación.pdf](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/files/13247000/Diagrama.de.aplicacion.pdf)

![Hardware](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/334b2adb-fe1d-40e1-9e43-af05de16a398)

![Edge impulse](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/309df0fd-b7fc-47d5-9f53-48f0d335d6b6)

![Características](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/f416a5ae-d611-4539-94eb-1e4c2a4d3234)

![Uso características](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/539eb086-dd4e-4add-b515-b19c5199faef)

![Precisión](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/dbffbccb-bafd-4b58-b37d-4b0d14402488)

![Librería](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/47be7b7a-2075-4a62-b7ec-3a534602ad27)

![Electrónico](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/c94da5b7-44d7-4b5c-8251-7f27473554d8)

![Introducción_7](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/5bf89350-a2b4-400f-9e6b-735127820105)

![Retos y limitaciones](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/3129409e-e898-4c72-bf1a-31f03470bb6d)

# Pruebas de la funcionalidad:

![Clasificación](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/0529df4c-c7b1-42bd-9b07-288fb39c8a36)
### Se entrena a la máquina para que reconozca cada punto de auscultación, se usa como clasificador MFCC y el tipo de red neuronal convolucional.

![Edge impulse](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/309df0fd-b7fc-47d5-9f53-48f0d335d6b6)
### La máquina genera espectrogramas de los ruidos.

![Características](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/f416a5ae-d611-4539-94eb-1e4c2a4d3234)
### Genera caractéristicas generales y busca patrones.
![Uso características](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/539eb086-dd4e-4add-b515-b19c5199faef)
### Se selecciona el tipo de arduino para el entrenamiento.
![Precisión](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/dbffbccb-bafd-4b58-b37d-4b0d14402488)
### La máquina encuentra patrones similares por cada punto de auscultación.

![Test](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/df0459bb-e6a0-42e9-884a-7612ecc664d6)
### Una vez generado el código, se hace un test con otros audios de válvulas cardíacas, y como vemos en el resultado, acierta en un 89%. 



https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/54504a19-603e-4f02-8baf-6e57e6a95476

![introducción 8](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/54f2a29e-7014-493f-a170-cbac13133c90)

![software](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/d2d63882-dff9-45fb-8231-2943c2d0e8cb)

![preguntas](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/4e52cfe9-7672-4f6c-ba50-02e52c1d79ec)

![hardware](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/e183e592-1c40-4302-b95a-d55fb2cf0244)

![tabla hardware](https://github.com/Renzo-Chafloque/FUNBIO_Grupo2/assets/143019492/45a92d17-2fd8-4015-8b7d-5f0d1820f2eb)

- ## Bibliografía
- World-heart-federation.org. https://world-heart-federation.org/wp-content/uploads/2017/05/spanish-press-release.pdf
- Sanabria-Montañez C, Cabrejos Polo J, Olortegui Yzu AR, San Juan Lezama H, Lama More MA, Villamonte Blas R. Patrones de costos de atención a
pacientes con enfermedades isquémicas del corazón en el Instituto Nacional Cardiovascular, 2019. An Fac Med (Lima, Peru: 1990). 2022  http://www.scielo.org.pe/scielo.php?script=sci_arttext&pid=S1025-55832022000200104 
- World-heart-federation.org.. https://world-heart-federation.org/wp-content/uploads/2017/05/spanish-press-release.pdf
- Enfermedades cardiovasculares. https://www.who.int/es/health-topics/cardiovascular-diseases
- Chambergo-Michilot, D., Velit-Rios, B., & Cueva-Parra, A. (2020). Prevalencia de enfermedades cardiovasculares en el Hospital Nacional Dos de
Mayo de Perú. Revista mexicana de angiología. https://doi.org/10.24875/rma.20000012
- Vigo-Ramos J. Muerte súbita y emergencias cardiovasculares: problemática actual. Rev Peru Med Exp Salud Publica. 2008. http://www.scielo.org.pe/scielo.php?script=sci_arttext&pid=S1726-46342008000200014
- Guerrero MH. UNIVERSIDAD RICARDO PALMA. Edu.pe
https://repositorio.urp.edu.pe/bitstream/handle/20.500.14138/1830/SL%c3%b3pezVictorio.pdf?sequence=1&isAllowed=y
-  Avery Li-Chun Wang. Audio Search Algorithm https://www.ee.columbia.edu/~dpwe/papers/Wang03-shazam.pdf
-  Barbuzano J. A Smart Stethoscope you can Connect to a Mobile Phone to Diagnose Lung Diseases. Open Mind BBVA. 2015. URL: [https://www.bbvaopenmind.com/en/technology/innovation/a-smart-stethoscope-connects-to-a-mobile-phone-to-diagnose-lung-diseases/](https://www.bbvaopenmind.com/en/technology/innovation/a-smart-stethoscope-connects-to-a-mobile-phone-to-diagnose-lung-diseases/)
- D. B. Chamberlain, R. Kodgule and R. R. Fletcher, "A mobile platform for automated screening of asthma and chronic obstructive pulmonary disease," 2016 38th Annual International Conference of the IEEE Engineering in Medicine and Biology Society (EMBC), Orlando, FL, USA, 2016.
- Ribeiro AH, Ribeiro MH, Paixão GMM, et al. Automatic diagnosis of the 12-lead ECG using a deep neural network. Nat Commun. 2020 [https://www.nature.com/articles/s41467-020-15432-4#citeas](https://www.nature.com/articles/s41467-020-15432-4#citeas)
- Jimenez Paz D.Prototipo de aplicacion movil para tratamiento de señales del fonendoscopio electronico Fonodx https://repository.unimilitar.edu.co/bitstream/handle/10654/32246/JimenezPazDanielDavid2019.pdf?sequence=1&isAllowed=y

