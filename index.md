<html>
<head>

</head>

<body style="background-image: url('https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTF73x8GmqEv2lO-tfKg-KrLkfXzwC-yq3A1A&usqp=CAU');background-repeat: no-repeat; background-size: cover;opacity: 0.7;">

<h1 align="center"><strong>Alineación titular</strong></h1>

<table align="center" id="equipo" width="100" cellspacing="1" cellpadding="3" border="0">


<script type="text/javascript">

var jugadores = [
{nombre: [],partidos_jugados:[],},
{nombre: [],partidos_jugados:[],},
{nombre: [],partidos_jugados:[],},
];


for (var i = 0; i <jugadores.length; i++) {
  jugadores[i].nombre= prompt("Nombre del jugador?");
  jugadores[i].partidos_jugados=prompt("Cuantas veces ha jugado "+jugadores[i].nombre+"?");
}



//Math.max.apply(Math, jugadores.map(o => o.partidos_jugados));


var index_valor_mayor= jugadores.findIndex(x => x.partidos_jugados==Math.max.apply(Math, jugadores.map(o => o.partidos_jugados)));

//var jugadores_titulares = jugadores.splice (index_valor_mayor,1);
//function posicion_mayor(jugadores){

  //var maximo= Math.max.apply(null,jugadores);
//  return maximo;

//}
//for (var i = 0; i <2; i++) {

  //jugadores_nombres.splice(0,1);
//}
//jugador_partidos_jugados.filter(number => number > 10 );
console.log(jugadores);
console.log (i);
console.log (index_valor_mayor);
//console.log(posicion_mayor());
//console.log(jugador_partidos_jugados);
//console.log(jugador_max);


//if(jugador_partidos>jugador_partidos){

  //
//for (var k=0;k<jugadores.lenght;k++){
  //document.getElementById("equipo").innerHTML =jugadores[k].nombre;
  document.getElementById("equipo").innerHTML ="<tr>"+"<th>Jugadores</th>"+"</tr>"+"<tr>"+"<td>"+jugadores[0].nombre+"</td>"+"</tr>"+"<tr>"+"<td>"+jugadores[1].nombre+"</td>"+"</tr>"+"<tr>"+"<td>"+jugadores[2].nombre+"</td>"+"</tr>";
//}

  //} else{
  //document.getElementById("equipo").innerHTML ="<tr>"+"<th>Jugador campo</th>"+"</tr>"+"<tr>"+"<td>"+jugador1+"</td>"+"</tr>";
  //}

</script>


</table>

<br><br>


<iframe src="https://docs.google.com/spreadsheets/d/e/2PACX-1vQOE_9bEOm09uCWQ1869mcVtVKttCmfhV9adduXEB2GXcGXpkUUioH9YP53r_o71KQ8PsJasVpGpPXw/pubhtml?widget=true&amp;headers=false"></iframe>

 </body>
</html>


