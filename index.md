<html>
<head>

</head>

<body>

<table id="equipo">

  
    <script>

  var jugador1 = prompt ("Inserta jugador 1","jugador1");
  var jugador1_partidos = prompt("Cuántas veces ha jugado?");
  
  var jugador2 = prompt ("Inserta jugador 2","jugador2");
  var jugador2_partidos = prompt("Cuántas veces ha jugado?");
 document.getElementById("equipo").innerHTML = "<tr>"+"<th>Jugador campo</th>"+"<th>Jugador banquillo</th>"+ "</tr>";
 
  if(jugador1_partidos>jugador2_partidos){
      document.getElementById("equipo").innerHTML ="<td>"+jugador2+"</td>"; 
  } else{
      document.getElementById("equipo").innerHTML ="<td>"+jugador1+"</td>"; 
  }

  </script>
  


</table>
 

<iframe src="https://docs.google.com/spreadsheets/d/e/2PACX-1vQOE_9bEOm09uCWQ1869mcVtVKttCmfhV9adduXEB2GXcGXpkUUioH9YP53r_o71KQ8PsJasVpGpPXw/pubhtml?widget=true&amp;headers=false"></iframe>
 
 </body>
</html>



