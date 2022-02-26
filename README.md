# CRUD-Php-Mysqli
CRUD funcional con Php y Mysqli incluyendo Bootstrap 4

Tengo que hacer el comentario de que este proyecto no fue desarrollado por mí, simplemente es una manera de guardar dicho proyecto luego de ver un vídeo en inglés en Youtube, 
lo único que guardo aquí es un respaldo para cuando requiera utilizarlo, no con fines de lucro puesto que de ser así mejor busquen entonces el vídeo llamado
"PHP CRUD Tutorial with MySQL & Bootstrap 4 (Create, Read, Update, Delete)" de Clever Techie y acudan a su patreon para descargar el archivo original apoyando al autor original
de estos archivos.

Me he dedicado a hacer otras cosas más que el desarrollo web, pero todavía me sigue gustando así que en caso de tener una actualización de esto, es porque yo he añadido algunas
pocas características más para hacerlo más dinámico de lo que ya es.

Un saludo por si encontraste esto por casualidad :)
---------------
AÑADIRÉ QUE...
En caso de querer agregar algún DataTable, recomendadísimo que le quiten el >> colspan="2" << que está en la etiqueta <th></th> donde aparece "Action", es decir:

De: <th colspan="2">Action</th>
A: <th>Action</th>

Y verán que funciona
---------------
OTRA COSA MÁS
En dado caso de que también se requiera modificar la cantidad de registros que se muestren después de añadir el datatable, que en vez de 10, por defecto sean 5, se añada este fragmento de código

De: 
<script>
  $(document).ready(function(){
    $(¿#nombredelatabla').DataTable();
  } );
</script>

A:
<script>
  $(document).ready(function(){
    $('#nombredelatabla').DataTable();
  } );
  
  var table = $('#nombredelatabla').DataTable({
    pageLength: 5,
    lengthMenu: [[5,10,20,-1], [5,10,20, 'All']]
  });
</script>

Y con eso queda :D
