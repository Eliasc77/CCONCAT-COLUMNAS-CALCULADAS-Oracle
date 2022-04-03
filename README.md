# CCONCAT-COLUMNAS-CALCULADAS-Oracle
#### Operadores aritmeticos
#### nos permiten realizar calculos con valores numericos (* / + - ) es posible obtener salidas en las cuales una columna sea el resultado de un calculo y no un campo de una tabla.

```sql
select * from libros;
```
 | titulo            | autor           |  editorial   |   precio   |    cantidad    |
 | ------------------|:----------------:|---------------:|-----------:|-----------:|
 | El quijote   | Miguel de Cervantes         |  La casa del Libro   |   650.00   | 10  |
 | Guerra yPaz  | Desconocido        |  Mensajero RUSO  |   500.00  | 5  |
 
 >crearemos una nueva columna donde calcularemos el precio x la cantidad
 ```sql
 select titulo, precio, cantidad, precio * cantidad from libros;
 
 ```
  | titulo            | autor           |  editorial   |   precio   |    cantidad    |  PRECIOxCANTIDAD    |
 | ------------------|:----------------:|---------------:|-----------:|-----------:|-----------:|
 | El quijote   | Miguel de Cervantes         |  La casa del Libro   |   650   | 10  |   6500|
 | Guerra yPaz  | Desconocido        |  Mensajero RUSO  |   500  | 5  | 2500|
