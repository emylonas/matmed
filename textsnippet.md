---
layout: default
title: the TEI page
nav_order: 2
description: "Some xml text"
permalink: text
---
# I am trying to convert XML in the Browser

<script src="/includes/CETEI.js"></script>
    <script>
      var CETEIcean = new CETEI();
      CETEIcean.getHTML5('testTEI.xml', function(data) {
        document.getElementById("TEI").innerHTML = "";
        document.getElementById("TEI").appendChild(data);
        CETEIcean.addStyle(document, data);
      });

      // Alternatively, use then()
      // (new CETEI).getHTML5('testTEI.xml').then(function(data){
      //   document.getElementById("TEI").appendChild(data);
      // });
    </script>
