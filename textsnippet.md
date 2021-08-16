---
layout: default
title: the TEI page
nav_order: 2
description: "Some xml text"
permalink: text
---
# I am trying to convert XML in the Browser

<div>
<h3>This is the XML block</h3>
<script src="includes/CETEI.js"></script>
    <script>
      var CETEIcean = new CETEI();
      CETEIcean.getHTML5('testTEI.xml', function(data) {
        document.getElementById("TEI").innerHTML = "";
        document.getElementById("TEI").appendChild(data);
        CETEIcean.addStyle(document, data);
      });
    </script>
  </div>
