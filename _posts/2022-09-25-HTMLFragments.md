---
toc: true
layout: post
description: 
categories: [CSP Assignments, Week 6]
title: HTML Fragments
---

<div id="JavaScriptTable">
</div>

<script>

let teamates = ["Dillon", "Rohan", "Derek", "Saavan"];

const table = document.createElement("table");
const row = document.createElement("tr");

for (let i = 0; i < teamates.length; i++) {
    let data = document.createElement("td");
    let node = document.createTestNode(teamates[i]);
    data.appendChild(node);
    row.appendChild(data);
}

table.appendChild(row);
const div = document.getElementById("JavaScriptTable");
div.appendChild(table);

</script>