---
toc: true
layout: post
categories: [AP Notes, CSP Assignments]
title: Javascript Exit Ticket 
---

# Javascript Exit Ticket

<script>

export default class LeaderboardScene extends Phaser.Scene {
    constructor() {
        super('LeaderboardScene');
    }

    preload() {
        
    }

    create() {
        const url = 'https://octolb.duckdns.org/api/leaderboards/';

        fetch(url)
            .then(response => response.json())
            .then(data => {
                // Process the retrieved data
                let tableData = [['Place', 'Name', 'Time']];
                for (let i = 0; i < Math.min(data.length, 10); i++) {
                    let point = data[i];
                    let place = i + 1;
                    let name = point.name;
                    let time = point.time;
                    tableData.push([place, name, time]);
                }

                const table = this.add.table(300, 200, tableData, {
                    fontFamily: 'Arial',
                    fontSize: '24px',
                });
                table.setOrigin(0.5);

                table.add([this.add.text(0, 0, 'Place'), this.add.text(0, 0, 'Name'), this.add.text(0, 0, 'Time')]);

                table.layout();

            })
            .catch(error => {
                // Handle any errors
                console.error('Error:', error);
            });

        this.add.text(300, 10, 'Leaderboard', { fontSize: '69px', align: 'center', fontFamily: "pressStart" });
    }

    update() {

    }

}
</script>
