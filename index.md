<html>
<head>

</head>

<body style="background-image: url('https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTF73x8GmqEv2lO-tfKg-KrLkfXzwC-yq3A1A&usqp=CAU');background-repeat: no-repeat; background-size: cover;opacity: 0.7;">

<h1 align="center"><strong>Alineación titular</strong></h1>

<!--encabezado tabla y formato-->

<table cellpadding="2" cellspacing="2" border="0" bgcolor="#dfdfdf" width="40%" align="center">
<thead>
    <tr align="center">
        <th width="20%">Jugador</th>
        <th width="12%">Partidos</th>
    </tr>
</thead>
    <tbody id="tableData"></tbody>
</table>

<!--empieza javascript-->

<script type="text/javascript">

//declaració objecto de datos
var jugadores = [
{nombre: [],partidos_jugados:[],},
{nombre: [],partidos_jugados:[],},
{nombre: [],partidos_jugados:[],},
{nombre: [],partidos_jugados:[],},
{nombre: [],partidos_jugados:[],},
{nombre: [],partidos_jugados:[],},
{nombre: [],partidos_jugados:[],},
{nombre: [],partidos_jugados:[],},
{nombre: [],partidos_jugados:[],},
{nombre: [],partidos_jugados:[],},
{nombre: [],partidos_jugados:[],},
{nombre: [],partidos_jugados:[],},
];

//cada vez declaramos el número de suplentes (lo has de saber en cada partido)
const numero_suplentes=4;

//inicializamos la variable quitar_maximos que nos servirá para recorrer los partidos de cada jugador y quitar los jugadores con máximos partidos hasta llegar al número de suplentes
var quitar_maximos=0;

//este for sirve para pedir insertar el nombre del jugador y cuántos partidos ha jugado cada uno
for (var i = 0; i <jugadores.length; i++) {
  jugadores[i].nombre= prompt("Nombre del jugador?");
  jugadores[i].partidos_jugados=prompt("Cuantas veces ha jugado "+jugadores[i].nombre+"?");
}


//este while recorre los datos de partidos jugados y quita los jugadores que han jugado más partidos
while (quitar_maximos<numero_suplentes){
  var index_valor_mayor= jugadores.findIndex(x => x.partidos_jugados==Math.max.apply(Math, jugadores.map(o => o.partidos_jugados)));
  var jugadores_suplentes = jugadores.splice (index_valor_mayor,1);
  quitar_maximos++;
}

//representación de la tabla de jugadores titulares (una vez que se han quitado los que han jugado más partidos)
var k = '<tbody>'
    for(i = 0;i < jugadores.length; i++){
        k+= '<tr align="center">';
        k+= '<td>' + jugadores[i].nombre + '</td>';
        k+= '<td>' + jugadores[i].partidos_jugados + '</td>';
        k+= '</tr>';
    }
    k+='</tbody>';
    document.getElementById('tableData').innerHTML = k;

//imprimir datos en la consola para ver si los resultados están bien
console.table(jugadores);
console.table(jugadores_suplentes);
console.log (i);
console.log (index_valor_mayor);
console.log (quitar_maximos);

</script>

<br><br>

<!--archivo de hoja de cálculo con los partidos de cada jugador -->

<iframe src="https://docs.google.com/spreadsheets/d/e/2PACX-1vQOE_9bEOm09uCWQ1869mcVtVKttCmfhV9adduXEB2GXcGXpkUUioH9YP53r_o71KQ8PsJasVpGpPXw/pubhtml?widget=true&amp;headers=false"></iframe>

 </body>
</html>
