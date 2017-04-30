# TP N°2 - MONGODB
persistencia ODM.

Principales funciones del proyecto.
- Login al sistema
- Búsqueda de POIs: <br> Líneas de colectivo, CGP, Sucursal de un Banco, Local Comercial
- Vista de Detalle de un POI
  * Opinión (Review) de un POI por parte de un usuario
  * Agregar un POI como favorito de un usuario

# Parte 1: Login al sistema
2 Integrantes ( Julian y Leon )

# Mapeo OD/M
Se pide que genere un log ante cada login del sistema, indicando
- fecha y hora
- usuario
- si el login fue exitoso o no
Debe persistir dicha información en una base documental y mapearla al modelo de objetos.

# Consultas a resolver directamente en la base

- Queremos saber los logueos (fallidos y exitosos) de un usuario la última semana
- Queremos saber el total de logins fallidos por usuario, ordenado en forma decreciente (si el usuario pepe se equivocó 5 veces, el usuario celeste 4 veces y el usuario tojol 10, deben aparecer tojol, pepe y celeste con sus respectivas cantidades)

# Parte 2: Reviews de un POI
Cantidad de integrantes estimada : 3 ( Estefania, Chris, Dai)

# Mapeo OD/M
Se pide que modifique el sistema de manera de registrar las opiniones de un POI en una base documental, 
mapeándola al modelo de objetos existente.<br> 
sin eliminar el componente que almacena la información en el motor relacional, solo se pide que quede momentáneamente desactivado pero que pueda fácilmente ser vuelto a activar.

Recordamos que una opinión o review de un POI contiene:
- el POI
- el usuario
- la nota numérica de 1 a 5
- el comentario

Luego de la modificación, la UI debe mostrar y agregar la información que contenga la base documental.

# Consultas a resolver directamente en la base
- Queremos saber el promedio de calificaciones general de un POI
- Queremos traer los POIs que hayan tenido un 5 de calificación, de la siguiente manera: <br>(POI, lista de comentarios de cada uno de los usuarios)
- Queremos saber el promedio de las calificaciones de un usuario <br>(ej: si calificó a la parada del 134 como 2, y al CGP 10 como 4, debe indicar un 3 de promedio)







