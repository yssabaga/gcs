# **Comandos usados en Google Cloud Platfform**

## Creación de Bucket

`gsutil mb -p sit-devops-training -c Nearline -l us-east4 -b on gs://sit-devops-training-bkt03`

Con esto se esta creando el Bucket "sit-devops-training-bkt03" bajo el Proyecto "sit-devops-training" en un ambiente "Regional US-EAST4" y un Tipo de Almacenamiento "Nearline".

## Asignación de etiquetas a un Bucket

`gsutil label ch -l equipo:autobots-01 gs://sit-devops-training-bkt03`
`gsutil label ch -l ejercicio:ejercicio-1 gs://sit-devops-training-bkt03`

Con estos comandos se creo la etiqueta "equipo" nombrada como: "autobots-01" y una etiqueta "ejercicio" nombrada como: "ejercicio-1" en el Bucket "sit-develops-training-bkt03"

## Creación de archivo

`touch yusef.txt`
`touch rodrigo.txt`

Estos commandos crean un archivo en blanco llamado "yusef.txt" y "rodrigo.txt", en la cloud shell del propietario.

## Agregar contenido a un archivo

`echo "Trabajando con Buckets" > yusef.txt`
`echo "Este archivo es de Rodrigo" > rodrigo.txt`

Este commando guardara el texto "Trabajando con Buckets" en el archivo "yusef.txt" y el texto "Este archivo es de Rodrigo" en el archivo "rodrigo.txt"

## Concatenar información a un archivo existente

`echo "Por primera vez" >> yusef.txt`

Este commando agregara una nueva linea con el texto "Por primera vez" en el archivo "yusef.txt"

## Copiar un archivo a un Bucket

`gsutil cp yusef.txt gs://sit-devops-training-bkt03`
`gsutil cp rodrigo.txt gs://sit-devops-training-bkt03`

Estos commandos copian los archivo "yusef.txt" y "rodrigo.txt" ubicados en la cloud shell del propietario al bucket "sit-devops-training-bkt03"

## Copiar un archivo de un Bucket

`gsutil cp gs://sit-devops-training-bkt03/rodrigo.txt .`
`gsutil cp gs://sit-devops-training-bkt03/yusef.txt .`

Estos commandos copian los archivo "yusef.txt" y "rodrigo.txt" del Bucket "sit-develops-training-bkt03" al cloud shell del propietario que lo ejecuto.

## Eliminar un Bucket

`gsutil rm -r gs://sit-devops-training-bkt03`

Con este comando borramos el Bucket "sit-devops-training-bkt03"  

- - -
  

   
| **Participantes** |
| :--       | 
| Rodrigo    | 
| Yusef      |