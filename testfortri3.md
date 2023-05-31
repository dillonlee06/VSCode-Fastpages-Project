---
title: Leaderboard Test
layout: default 
permalink: /lbtest
type: pbl
---
<div class="secondary">
  <button id="read_button" type="button" onclick="read_leaderboard()" class="read-button">Show Leaderboard</button>
</div>

<table class="readtable">
  <thead>
    <tr>
      <th>Rank</th>
      <th>Name</th>
      <th>Score</th>
    </tr>
  </thead>
  <tbody id="result">
  </tbody>
</table>

<style>
  .readtable {
    background-color: #FFFFFF;
  }
</style>

<div class="form-box">
  <form action="javascript:create_ranking()" class="createForm">
    <p>
      <label class="form-label">
        Name:
        <input class="input-boxes" type="text" name="name" id="name" required>
      </label>
    </p>
    <p>
      <label class="form-label">
        Score:
      </label>
    </p>
    <p>
      <button class="form-button">Submit</button>
    </p>
  </form>
</div>

<script>
  const resultContainer = document.getElementById("result");
  const read_button = document.getElementById("read_button");
  const apiURL = "https://octolb.duckdns.org/api/leaderboards/";

  // READ
  function read_leaderboard() {
    const read_options = {
      method: 'GET',
      mode: 'cors',
      cache: 'default',
      credentials: 'omit',
      headers: {
        'Content-Type': 'application/json'
      },
    };

    fetch(apiURL, read_options)
      .then(response => {
        if (response.status !== 200) {
          const errorMsg = 'API read error: ' + response.status;
          console.log(errorMsg);
          const tr = document.createElement("tr");
          const td = document.createElement("td");
          td.innerHTML = errorMsg;
          tr.appendChild(td);
          resultContainer.appendChild(tr);
          return;
        }

        response.json().then(data => {
          resultContainer.innerHTML = '';
          data.forEach((row, index) => {
            add_row(index + 1, row.name, row.score);
          });
        });
      })
      .catch(err => {
        console.error(err);
        const tr = document.createElement("tr");
        const td = document.createElement("td");
        td.innerHTML = err;
        tr.appendChild(td);
        resultContainer.appendChild(tr);
      });
  }

  function add_row(rank, name, score) {
    const tr = document.createElement("tr");
    const rankCell = document.createElement("td");
    const nameCell = document.createElement("td");
    const scoreCell = document.createElement("td");

    rankCell.innerHTML = rank;
    nameCell.innerHTML = name;
    scoreCell.innerHTML = score;

    tr.appendChild(rankCell);
    tr.appendChild(nameCell);
    tr.appendChild(scoreCell);

    resultContainer.appendChild(tr);
  }

  // CREATE
  function create_ranking() {
    const body = {
      name: document.getElementById("name").value,
      score: document.getElementById("score").value,
    };

    const requestOptions = {
      method: 'POST',
      body: JSON.stringify(body),
      headers: {
        "Content-Type": "application/json"
      },
    };

    fetch(apiURL + 'create', requestOptions)
      .then(response => {
        if (response.status !== 200) {
          const errorMsg = 'API create error: ' + response.status;
          console.log(errorMsg);
          const tr = document.createElement("tr");
          const td = document.createElement("td");
          td.innerHTML = errorMsg;
          tr.appendChild(td);
          resultContainer.appendChild(tr);
          return;
        }
        return response.json();
      })
      .then(data => {
        add_row(data.rank, data.name, data.score);
      })
      .catch(err => {
        console.error(err);
        const tr = document.createElement("tr");
        const td = document.createElement("td");
        td.innerHTML = err;
        tr.appendChild(td);
        resultContainer.appendChild(tr);
      });
  }
</script>

