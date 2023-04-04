var standings = JSON.parse(Standings);
var standingsTable = document.getElementById('standings-table');

standingsTable.innerHTML = standings.standings.map(function(standing) {
  return "<tr>" +
    "<td>" + standing.team + "</td>" +
    "<td>" + standing.wins + "</td>" +
    "<td>" + standing.losses + "</td>" +
    "<td>" + standing.pct + "</td>" +
    "<td>" + standing.gb + "</td>" +
  "</tr>";
}).join('');
