---
layout: home
description: "读书活动列表"
permalink: /sf/events/
---


<section id="services">
    <div class="container">
        <div class="row text-center">
            <div class="col-lg-12 text-center">
                <h4 class="service-heading">分享的书目</h4>
                <script src="//ajax.googleapis.com/ajax/libs/jquery/1.11.1/jquery.min.js"></script>
                <div id="container1"></div>
                <script >
                $.get('/sheet1.csv', function(data) {

                // start the table
                var html = '<table class="table table-striped table-bordered">';

                // split into lines
                var rows = data.trim().split("\n");

                // parse lines
                rows.forEach( function getvalues(ourrow) {
                // start a table row
                html += "<tr>";

                // split line into columns
                var columns = ourrow.split(",");

                html += "<td>" + columns[0] + "</td>";
                html += "<td>" + columns[1] + "</td>";
                html += "<td>" + columns[2] + "</td>";
                html += "<td>" + columns[3] + "</td>";

                // close row
                html += "</tr>";
                })
                // close table
                html += "</table>";

                // insert into div
                $('#container1').append(html);

                });
                </script>

            </div>
        </div>
    </div>
</section>

