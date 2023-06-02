---
toc: true
layout: post
categories: [AP Notes, CSP Assignments]
title: Javascript Exit Ticket 
---

# Javascript Exit Ticket

<!DOCTYPE html>
<html>
<head>
  <title>Student Leaderboard</title>
  <style>
    table {
      font-family: Arial, sans-serif;
      border-collapse: collapse;
      width: 100%;
    }
  </style>
</head>
<body>
  <h2>Student Leaderboard</h2>
  <p>Sort by:</p>
  <select id="sort-select">
    <option value="index">Index</option>
    <option value="studentNumber">Student Number</option>
    <option value="studentName">Student Name</option>
    <option value="studentGPA">Student GPA</option>
    <option value="studentPercentage">Student Class Percentage</option>
  </select>
  <table id="leaderboard">
    <thead>
      <tr>
        <th>Index</th>
        <th>Student ID</th>
        <th>Student Name</th>
        <th>Student GPA</th>
        <th>Student Class Percentage</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>1</td>
        <td>1924520</td>
        <td>Dillon Lee</td>
        <td>3.5</td>
        <td>85%</td>
      </tr>
      <tr>
        <td>2</td>
        <td>1820352</td>
        <td>Steven</td>
        <td>3.8</td>
        <td>92%</td>
      </tr>
      <tr>
        <td>3</td>
        <td>1923509</td>
        <td>Noor</td>
        <td>3.2</td>
        <td>98%</td>
      </tr>
      <tr>
        <td>4</td>
        <td>1812350</td>
        <td>Lucas</td>
        <td>3.9</td>
        <td>75%</td>
      </tr>
    </tbody>
  </table>

  <script>
    function sortTable() {
      const select = document.getElementById("sort-select");
      const value = select.value;

      const table = document.getElementById("leaderboard");
      const tbody = table.getElementsByTagName("tbody")[0];
      const rows = tbody.getElementsByTagName("tr");

      let sortFunction;
      switch (value) {
        case "index":
          sortFunction = (a, b) => (a.cells[0].textContent > b.cells[0].textContent) ? 1 : -1;
          break;
        case "studentNumber":
          sortFunction = (a, b) => (a.cells[1].textContent > b.cells[1].textContent) ? 1 : -1;
          break;
        case "studentName":
          sortFunction = (a, b) => (a.cells[2].textContent > b.cells[2].textContent) ? 1 : -1;
          break;
        case "studentGPA":
          sortFunction = (a, b) => (parseFloat(a.cells[3].textContent) > parseFloat(b.cells[3].textContent)) ? 1 : -1;
          break;
        case "studentPercentage":
          sortFunction = (a, b) => (parseFloat(a.cells[4].textContent) > parseFloat(b.cells[4].textContent)) ? 1 : -1;
          break;
        default:
          return;
      }

      const sortedRows = Array.from(rows).sort(sortFunction);
      for (const row of sortedRows) {
        tbody.appendChild(row);
      }
    }

    const select = document.getElementById("sort-select");
    select.addEventListener("change", sortTable);
  </script>
</body>
</html>
