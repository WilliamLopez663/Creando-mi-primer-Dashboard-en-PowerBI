<h1 align="center"> Creando mi primer Dashboard en PowerBI</h1>
En este proyecto crearé mi primer dashboard en PowerBI basado en el siguiente ejercicio.

## :page_with_curl: Ejercicio

La empresa **MaxTecnology** especializada en ventas de productos de tecnología en Mexico desea conocer un análisis de las ventas realizadas por sus sucursales durante los años 2021, 2022 y 2023, debido a que las  ventas han estado en declive, y se ha tenido que cerrar una sucursal, lo que genera incertidumbre sobre su futuro. Adicional nos indica que debemos tener en cuenta el porcentaje de descuento para los clientes dependiente del nivel de cuenta.


Plata: 3% de descuento  
Oro: 8% de descuento  
Platino: 12% de descuento  

En el análisis la empresa desea resolver las siguientes dudas:
- ¿Cuáles son las sucursales con mejor y peor desempeño en ventas?
- ¿Existe una relación entre la variedad de productos y los niveles de ventas?
- ¿Cómo afecta la cantidad de vendedores al éxito de ventas de una sucursal?
- ¿Cómo varían las ventas durante diferentes temporadas o eventos del año?

Para ello nos proporcionan los siguientes datos:

:link: **[Datos-2021.xlsx](./assets/docs/Datos2021.xlsx)**  
:link: **[Datos-2022.xlsx](./assets/docs/Datos2022.xlsx)**  
:link: **[Datos-2023.xlsx](./assets/docs/Datos2022.xlsx)**

Tras cargar la información en `Power BI` y renombrar las tablas se puede visualizar de esta forma:
<br><br>
<img  src="https://raw.githubusercontent.com/WilliamLopez663/Creando-mi-primer-Dashboard-en-PowerBI/main/assets/images/datos-cargados.PNG">

- `Uniendo las tablas` de los datos de los tickets de las ventas de los años 2021, 2022 y 2023:
<div align="center">
  <img  src="https://raw.githubusercontent.com/WilliamLopez663/Creando-mi-primer-Dashboard-en-PowerBI/main/assets/images/uniendo-tablas.PNG">
</div>

- `Modificando el tipo de dato` de las columnas de la tabla tickets:
<div align="center">
  <img  src="https://raw.githubusercontent.com/WilliamLopez663/Creando-mi-primer-Dashboard-en-PowerBI/main/assets/images/uniendo-tablas.PNG">
</div>

- `Transformando tipo de dato` blank a tipo null usando la función reemplazar valores:
<div align="center">
  <img  src="https://raw.githubusercontent.com/WilliamLopez663/Creando-mi-primer-Dashboard-en-PowerBI/main/assets/images/transformando-celda-tipo-null-ejecutando.PNG">
</div>
<div align="center">
  <img  src="https://raw.githubusercontent.com/WilliamLopez663/Creando-mi-primer-Dashboard-en-PowerBI/main/assets/images/transformando-celda-tipo-null.PNG">
  <img  src="https://raw.githubusercontent.com/WilliamLopez663/Creando-mi-primer-Dashboard-en-PowerBI/main/assets/images/transformando-celda-tipo-null-final.PNG">
</div>

- Utilizando la función `rellenar abajo` para completar los datos de mi tabla:
<div align="center">
  <img  src="https://raw.githubusercontent.com/WilliamLopez663/Creando-mi-primer-Dashboard-en-PowerBI/main/assets/images/rellenar-abajo.png">
  <img  src="https://raw.githubusercontent.com/WilliamLopez663/Creando-mi-primer-Dashboard-en-PowerBI/main/assets/images/rellenar-abajo-final.png">
</div>

- `Transformando algunas columnas a tipo texto` debido a que Power BI las identifica como de tipo número:
<div align="center">
  <img  src="https://raw.githubusercontent.com/WilliamLopez663/Creando-mi-primer-Dashboard-en-PowerBI/main/assets/images/transformando-tipo-dato.PNG">
</div>

- Usando la función `dividir columna` para separar el tipo de cuenta del nivel de cuenta:
<div align="center">
  <img  src="https://raw.githubusercontent.com/WilliamLopez663/Creando-mi-primer-Dashboard-en-PowerBI/main/assets/images/dividir-columna.PNG">
</div>

- Este es el resultado tras dividir la columna:
<div align="center">
  <img  src="https://raw.githubusercontent.com/WilliamLopez663/Creando-mi-primer-Dashboard-en-PowerBI/main/assets/images/dividir-columna-final.PNG">
</div>

- Utilizando la función `usar primera fila como encabezado`:
<div align="center">
  <img  src="https://raw.githubusercontent.com/WilliamLopez663/Creando-mi-primer-Dashboard-en-PowerBI/main/assets/images/usando-primera-fila-como-encabezado.PNG">
</div>

- Este es el resultado de utilizar la opción usar primera fila como encabezado:
<div align="center">
  <img  src="https://raw.githubusercontent.com/WilliamLopez663/Creando-mi-primer-Dashboard-en-PowerBI/main/assets/images/usando-primera-fila-como-encabezado-final.PNG">
</div>

- Usando la función `crear columna a partir de ejemplos` para unir nuestra columna Categoría y subcategoría en una sola columna:
<div align="center">
  <img  src="https://raw.githubusercontent.com/WilliamLopez663/Creando-mi-primer-Dashboard-en-PowerBI/main/assets/images/crear-columna-a-partir-de-ejemplos.PNG">
</div>

- Tras usar la función esta esta nuestra columna unida:
<div align="center">
  <img  src="https://raw.githubusercontent.com/WilliamLopez663/Creando-mi-primer-Dashboard-en-PowerBI/main/assets/images/crear-columna-a-partir-de-ejemplos-final.PNG">
</div>

- Usando la función `columna personalizada` para crear una nueva columna sin la palabra sucursal debido a que puede no ser atractivo al momento de mostrar nuestros graficos:
<div align="center">
  <img  src="https://raw.githubusercontent.com/WilliamLopez663/Creando-mi-primer-Dashboard-en-PowerBI/main/assets/images/columna-personalizada.PNG">
</div>

- Para usar esta columna hago uso de la función `Text.Middle` de PowerQuery para traer el texto que se encuentra en la columna SUCURSAL_NOMBRE a partir del caracter 9:
<div align="center">
  <img  src="https://raw.githubusercontent.com/WilliamLopez663/Creando-mi-primer-Dashboard-en-PowerBI/main/assets/images/text-middle.PNG">
</div>

- Esta es la columna resultado:
<div align="center">
  <img  src="https://raw.githubusercontent.com/WilliamLopez663/Creando-mi-primer-Dashboard-en-PowerBI/main/assets/images/columna-personalizada-final.PNG">
</div>

- Usando la función `columna condicional` para crear una nueva columna que contenga los descuento que se aplican a los clientes dependiendo del nivel de cuenta:
<div align="center">
  <img  src="https://raw.githubusercontent.com/WilliamLopez663/Creando-mi-primer-Dashboard-en-PowerBI/main/assets/images/columna-condicional.PNG">
</div>

- Dentro de la función nombro la columna y asigno el porcentaje de descuento para cada nivel de cuenta:
<div align="center">
  <img  src="https://raw.githubusercontent.com/WilliamLopez663/Creando-mi-primer-Dashboard-en-PowerBI/main/assets/images/columna-condicional-ejecutando.PNG">
</div>

- Tras ejecutar la función `columna condicional` esta es la columna resultado:
<div align="center">
  <img  src="https://raw.githubusercontent.com/WilliamLopez663/Creando-mi-primer-Dashboard-en-PowerBI/main/assets/images/columna-condicional-final.PNG">
</div>

- Tras realizar la transformación a los datos al dirigirnos a la vista modelo se visualizan las tablas de esta forma:
<div align="center">
  <img  src="https://raw.githubusercontent.com/WilliamLopez663/Creando-mi-primer-Dashboard-en-PowerBI/main/assets/images/datos-transformados.PNG">
</div>

- Realizando un modelado de datos de tipo estrella para `relacionar la tabla` tickets con las demás, arrastrando el campo hacia la tabla que se quiere relacionar:
<div align="center">
  <img  src="https://raw.githubusercontent.com/WilliamLopez663/Creando-mi-primer-Dashboard-en-PowerBI/main/assets/images/creando-relacion.png">
</div>

- Se muestra un cuadro que indica el `tipo de relación` que se está ejecutando, para este caso es de muchos a uno debido a que muchos tickes pueden estar relacionados con el mismo vendedor:
<div align="center">
  <img  src="https://raw.githubusercontent.com/WilliamLopez663/Creando-mi-primer-Dashboard-en-PowerBI/main/assets/images/tipo-de-relacion.PNG">
</div>

- La `relación` se visualiza de esta forma:
<div align="center">
  <img  src="https://raw.githubusercontent.com/WilliamLopez663/Creando-mi-primer-Dashboard-en-PowerBI/main/assets/images/relacion-final.PNG">
</div>

- Ejecutando las relaciones con las demás tablas este es el resultado:
<div align="center">
  <img  src="https://raw.githubusercontent.com/WilliamLopez663/Creando-mi-primer-Dashboard-en-PowerBI/main/assets/images/relaciones-final.PNG">
</div>

- Haciendo uso de `DAX` para crear una columna calculada a partir de unir los datos de 2 columnas:
<div align="center">
  <img  src="https://raw.githubusercontent.com/WilliamLopez663/Creando-mi-primer-Dashboard-en-PowerBI/main/assets/images/dax-columna-calculada.PNG">
</div>

- La `columna calculada` queda así:
<div align="center">
  <img  src="https://raw.githubusercontent.com/WilliamLopez663/Creando-mi-primer-Dashboard-en-PowerBI/main/assets/images/dax-columna-calculada-final.PNG">
</div>

- Haciendo uso de `DAX` para crear una `medida` para el conteo de tickets:
<div align="center">
  <img  src="https://raw.githubusercontent.com/WilliamLopez663/Creando-mi-primer-Dashboard-en-PowerBI/main/assets/images/dax-crear-medida-conteo-tickets.PNG">
</div>

- Tras ejecutar la función se crea la `medida` en el panel de datos:
<div align="center">
  <img  src="https://raw.githubusercontent.com/WilliamLopez663/Creando-mi-primer-Dashboard-en-PowerBI/main/assets/images/dax-medida-conteo-tickets.PNG">
</div>
- 
