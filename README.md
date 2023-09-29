<h1 style="color: green">TareaAPI</h1>
<h2>Importante: </h2>
<p>Para registrar o crear nuevos usuarios que tengan una llave foránea<span style="color: yellow">(FK)</span> 
<strong><p><br>Se debe crear un <u>Comentario</u>:</strong> <br></p>

```JSON
{
    "texto": "Este es un comentario de ejemplo.",
    "fechaCreacion": "Septiembre 2023",
    "tarea": 1

}
```

<p>El <span style="color: yellow">ID</span> de la tarea a asignar la llave foránea<span style="color: yellow">(FK)</span> se ingresa de esta manera <span style="color: yellow">"Tarea": {valor}</span>.</p><br>
<p><strong>Para crear una <u>Tarea</u>:</strong></p>

```JSON
{
  "titulo": "Bug",
  "descripcion": "Arreglar el bug del boton en index.html",
  "fechaVencimiento": "Septiembre 2023",
  "usuario":1
}
```

<p>El <span style="color: yellow">ID</span> del comentario para asignar una llave foranea<span style="color: yellow">(FK)</span> se ingresa de esta manera <span style="color: yellow">Comentario {valor}</span>.</p><br>

<p><strong><u>Para crear un Usuario</u>:</strong> </p>

```JSON
{
  "nombreUsuario": "Papitas",
  "email": "Papitas@grupo6.com"
}
```

<h2>Notas:</h2>
<p>Para el <span style="color: yellow">Endpoint</span> de borrar(en todos los controllers) se ingresa con parametros así:<br><i style="color: yellow">/api/usuario/borrar?id=7</i><br><br>
Y para los de editar se pasa el <span style="color: yellow">ID</span> por el path.<br>
<i style="color: yellow">/api/usuario/editar/1</i></p>

<h3>Endpoints:</h3>
<h4>GET</h4>
<span style="color: yellow">/api/usuario/lista</span><br>
<span style="color: yellow">/api/comentario/lista</span><br>
<span style="color: yellow">/api/tarea/lista</span><br><br>
<h4>POST</h4>

<span style="color: yellow">/api/usuario/registrar</span><br>
<span style="color: yellow">/api/comentario/registrar</span><br>
<span style="color: yellow">/api/tarea/registrar</span><br><br>

<h4>PUT</h4>
<span style="color: yellow">/api/usuario/editar/{id}</span><br>
<span style="color: yellow">/api/comentario/editar/{id}</span><br>
<span style="color: yellow">/api/tarea/editar/{id}</span><br><br>
<h4>DELETE</h4>
<span style="color: yellow">/api/usuario/borrar?id=</span><br>
<span style="color: yellow">/api/comentario/borrar?id=</span><br>
<span style="color: yellow">/api/tarea/borrar?id=</span><br>

<h2 style="color: green">Objetos utilizados:</h2>
<h3>ResponseEntity<?> : </h3>
<p>Se utiliza para manejar mejor los errores de los métodos <span style="color: yellow">CRUD</span> dentro de <strong><u>UsuarioServiceImpl</u>, <u>ComentarioServiceImpl</u>, <u>TareaServiceImpl</u></strong> en los casos en que se ingrese un <span style="color: yellow">ID</span> inexistente dentro de la base de datos.</p>

<h3>Optional<?> :</h3>
<p>Acá este objeto sirve para manejar los resultados <span style="color: yellow">Null</span> dentro de los metodos <span style="color: yellow">CRUD</span>  en <strong><u>UsuarioServiceImpl</u>, <u>ComentarioServiceImpl</u>, <u>TareaServiceImpl</u></strong> al momento de buscar dentro de la base de datos una tupla inexistente.</p>

<h3> Participantes:</h3>
<a href="https://github.com/papitas-grupo6">
  <img src="https://avatars.githubusercontent.com/u/142447730?s=96&v=4" alt="papitas"></p>
  PapitasGroup6
</a>:</p>
<p>🍟<a href="https://github.com/AngelSmithlgs">Angel Smith</a></p>
🍟<a href="https://github.com/sq1m">Matías Quevedo</a></p>
<p>🍟<a href="https://github.com/Nosst-bot">Kevin Peña Salvatierra</a></p>
🍟<a href="https://github.com/PauletteDoll">Paulette Doll</a></p>
🍟<a href="https://github.com/Rosa-Enco-Perez">Rosa Enco Perez</a></p>

