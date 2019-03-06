## Ejercicio Nómina

### Datos

~~~~
[
{idEmployee: 1, name: "Mike", salario: 5000, role: "React Developer"},
{idEmployee: 2, name: "Sergio", salario: 5000, role: "UX Designer"},
{idEmployee: 3, name: "Rogelio", salario: 5000, role: "UX Designer"},
{idEmployee: 4, name: "Maria Fernanda", salario: 6000, role: "Product Manager" },
{idEmployee: 5, name: "Enrique", salario: 6000, role: "Operations Manager"},
{idEmployee: 6, name: "Laura", salario: 6000, role: "Backend Developer"},
{idEmployee: 7, name: "Cecilia", salario: 6000, role: "Backend Developer"},
{idEmployee: 8, name: "Arturo", salario: 11000, role: "CTO"},
{idEmployee: 9, name: "Gaby", salario: 14000, role: "CEO"},
{idEmployee: 10, name: "Lorena", salario: 11000, role: "CFO"}
]
~~~~

### Instrucciones:
Utiliza los diferentes comandos para ejecutrar dentro del "Shell" de MongoDB los siguientes instrucciones para alterar la base de datos. :

1. Crea una base de datos
> use EjercicioMongo01

2. Crea una colección
> db.createCollection('nomina')

3. Inserta el arreglo de datos como documentos en la colección creada
> db.nomina.insert({idEmployee: 1, name: "Mike", salario: 5000, role: "React Developer"})
// y así cada uno

4. Despliega datos en el formato correcto
{ "_id" : ObjectId("5c7f28a9a10b442724b765fe"), "idEmployee" : 1, "name" : "Mike", "salario" : 5000, "role" : "React Developer" }
{ "_id" : ObjectId("5c7f28e4a10b442724b765ff"), "idEmployee" : 2, "name" : "Sergio", "salario" : 5000, "role" : "UX Designer" }
{ "_id" : ObjectId("5c7f28fea10b442724b76600"), "idEmployee" : 3, "name" : "Rogelio", "salario" : 5000, "role" : "UX Designer" }
{ "_id" : ObjectId("5c7f2916a10b442724b76601"), "idEmployee" : 4, "name" : "Maria Fernanda", "salario" : 6000, "role" : "Product Manager" }


5. Actualiza el salario del empleado donde el "name" sea "Mike" por $5000 USD más

6. Actualiza los salarios de todos los empleados dando un incremento de $3000 a cada uno

7. Actualiza el rol de "UX Designer" a "Product Manager" de "Sergio"

8. Agrega un nuevo campo llamado "bonificacion" a "Rogelio" con un valor de "true"

9. Agrega un nuevo documento que incluya a "Mariana" en la nómina. Salario por $5500 USD, como "role" de 
"Marketing Manager", verificando que no haya un documento existente con estos datos.

10. Quita el campo de bonificacion del documento de "Rogelio"

11. Multiplica el salario de "Lorena" por 2.

12. Encuentra dentro de la colección todos los salarios que tengan menos de $5500 USD de salario.
