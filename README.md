<h1 align="center"> Creando mi primer Dashboard en PowerBI</h1>
En este proyecto crearé mi primer dashboard en PowerBI basado en el siguiente ejercicio.

## :page_with_curl: Ejercicio
<p>
La empresa MaxTecnology especializada en ventas de productos de tecnología de Mexico desea conocer un análisis de las ventas realizadas por sus sucursales durante los años 2021, 2022 y 2023, debido a que las  ventas han estado en declive, y se ha tenido que cerrar una sucursal, lo que genera incertidumbre sobre su futuro. En el análisis la empresa desea resolver las siguientes dudas:
</p>

- ¿Cuáles son las sucursales con mejor y peor desempeño en ventas?
- ¿Existe una relación entre la variedad de productos y los niveles de ventas?
- ¿Cómo afecta la cantidad de vendedores al éxito de ventas de una sucursal?
- ¿Cómo varían las ventas durante diferentes temporadas o eventos del año?

Para ello nos proporcionan los siguientes datos:

📎 **[Datos-2021.xlsx](./assets/docs/Datos2021.xlsx)**  
📎 **[Datos-2022.xlsx](./assets/docs/Datos2022.xlsx)**  
📎 **[Datos-2023.xlsx](./assets/docs/Datos2022.xlsx)**

Tras cargar nuestra información en `Power BI` y renombrar las tablas podemos ver nuestras información de esta forma:
<br><br>
<img  src="https://raw.githubusercontent.com/WilliamLopez663/Creando-mi-primer-Dashboard-en-PowerBI/main/assets/images/datos-cargados.PNG">

- Uniendo las tablas de los datos de los tickets de las ventas de los años 2021, 2022 y 2023:
<div align="center">
  <img  src="https://raw.githubusercontent.com/WilliamLopez663/Creando-mi-primer-Dashboard-en-PowerBI/main/assets/images/uniendo-tablas.PNG">
</div>

- Modificando el tipo de dato de las columnas de mi tabla tickets:
<div align="center">
  <img  src="https://raw.githubusercontent.com/WilliamLopez663/Creando-mi-primer-Dashboard-en-PowerBI/main/assets/images/uniendo-tablas.PNG">
</div>

- Transformando tipo de dato blank a tipo null usando la función reemplazar valores:
<div align="center">
  <img  src="https://raw.githubusercontent.com/WilliamLopez663/Creando-mi-primer-Dashboard-en-PowerBI/main/assets/images/transformando-celda-tipo-null-ejecutando.PNG">
</div>
<div align="center">
  <img  src="https://raw.githubusercontent.com/WilliamLopez663/Creando-mi-primer-Dashboard-en-PowerBI/main/assets/images/transformando-celda-tipo-null.PNG">
  <img  src="https://raw.githubusercontent.com/WilliamLopez663/Creando-mi-primer-Dashboard-en-PowerBI/main/assets/images/transformando-celda-tipo-null-final.PNG">
</div>

- Utilizando la función rellenar abajo para completar nuestra tabla:
<div align="center">
  <img  src="https://raw.githubusercontent.com/WilliamLopez663/Creando-mi-primer-Dashboard-en-PowerBI/main/assets/images/rellenar-abajo.png">
  <img  src="https://raw.githubusercontent.com/WilliamLopez663/Creando-mi-primer-Dashboard-en-PowerBI/main/assets/images/rellenar-abajo-final.png">
</div>

- Transformando algunas columnas a tipo texto debido a que Power BI la identifica como de tipo número:
<div align="center">
  <img  src="https://raw.githubusercontent.com/WilliamLopez663/Creando-mi-primer-Dashboard-en-PowerBI/main/assets/images/transformando-tipo-dato.PNG">
</div>

- Usando la función dividir columna para separar el tipo de cuenta del nivel de cuenta:
<div align="center">
  <img  src="https://raw.githubusercontent.com/WilliamLopez663/Creando-mi-primer-Dashboard-en-PowerBI/main/assets/images/dividir-columna.PNG">
</div>

- Este es el resultado tras dividir nuestra columna:
<div align="center">
  <img  src="https://raw.githubusercontent.com/WilliamLopez663/Creando-mi-primer-Dashboard-en-PowerBI/main/assets/images/dividir-columna-final.PNG">
</div>

- Usando la función usar primero fila como encabezado:
<div align="center">
  <img  src="https://raw.githubusercontent.com/WilliamLopez663/Creando-mi-primer-Dashboard-en-PowerBI/main/assets/images/usando-primera-fila-como-encabezado.PNG">
</div>

- Este es el resultado de utilizar la opción usar primera fila como encabezado:
<div align="center">
  <img  src="https://raw.githubusercontent.com/WilliamLopez663/Creando-mi-primer-Dashboard-en-PowerBI/main/assets/images/usando-primera-fila-como-encabezado-final.PNG">
</div>
  
