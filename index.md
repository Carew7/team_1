<html>
<head>

</head>

<body>

<table id="equipo">

    
<script>

<script type="text/javascript">

var jugadores = ["jugador1","jugador2","jugador3","jugador4","jugador5","jugador6","jugador7"];
var jugadores_partidos= ["jugador_partidos1","jugadorpartidos2","jugadorpartidos3","jugadorpartidos4","jugadorpartidos5","jugadorpartidos6","jugadorpartidos7"];

for (var i = 1; i < 8; i++) {
var jugadores[i]= prompt ("Inserta jugador"+i,"jugador"+i);
var jugador_partidos[i] = prompt("Cuántas veces ha jugado?");
}
 
 
  if(jugador1_partidos>jugador2_partidos){
      document.getElementById("equipo").innerHTML ="<tr>"+"<th>Jugador campo</th>"+"</tr>"+"<tr>"+"<td>"+jugador2+"</td>"+"</tr>"; 
  } else{
      document.getElementById("equipo").innerHTML ="<tr>"+"<th>Jugador campo</th>"+"</tr>"+"<tr>"+"<td>"+jugador1+"</td>"+"</tr>"; 
  }

  </script>
  


</table>
 

<iframe src="https://docs.google.com/spreadsheets/d/e/2PACX-1vQOE_9bEOm09uCWQ1869mcVtVKttCmfhV9adduXEB2GXcGXpkUUioH9YP53r_o71KQ8PsJasVpGpPXw/pubhtml?widget=true&amp;headers=false"></iframe>
 
 </body>
</html>



