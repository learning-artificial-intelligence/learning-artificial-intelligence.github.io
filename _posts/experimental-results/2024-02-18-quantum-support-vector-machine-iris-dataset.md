---
layout: results
category: experimental-results
title: "Experimental Results for Quantum (Enhanced) Support Vector Machine (QSVM) on IRIS Dataset"
tagline: "Classification results obtained from tuning several hyperparameters of Quantum (Enhanced) Support Vector Machine (QSVM) on IRIS Dataset..."
author: Rúben André Barreiro
tags: [artificial-intelligence, computer-science, quantum-support-vector-machine, support-vector-machine, quantum-machine-learning, machine-learning, supervised-learning, training, classification, iris-dataset, intermediate]
keywords: quantum support vector machine, support vector machine, quantum machine learning, machine learning, training, supervised learning, training, classification, iris dataset, beginner, artificial intelligence, ai
bgcolor: ff5a71
canonical: https://learning-artificial-intelligence.github.io/
css:
js:
---
<script type="text/javascript" language="javascript" src="https://github.com/learning-artificial-intelligence/learning-artificial-intelligence.github.io/blob/main/_posts/experimental-results/tablefilter/tablefilter.js"></script>
<script>
  var filtersConfig = {
        base_path: "tablefilter/",
        col_1: "none",
        col_2: "select",
        col_3: "select",
        col_4: "select",
        col_5: "select",
        col_6: "select",
        alternate_rows: true,
        rows_counter: true,
        btn_reset: true,
        loader: true,
        status_bar: true,
        no_results_message: true,
        extensions:[{
            name: "sort"
        }]
    };
    
  var tableFilter = 
      new TableFilter("quantum-svm-iris-dataset-exp-results",
                      filtersConfig);

  tableFilter.init();
</script>
<script>
  function sortTable(n) {
    var table, rows, switching, i, x, y, shouldSwitch, dir, switchcount = 0;
    table = document.getElementById("quantum-svm-iris-dataset-exp-results");
    switching = true;
    // Set the sorting direction to ascending:
    dir = "asc";
    /* Make a loop that will continue until
    no switching has been done: */
    while (switching) {
      // Start by saying: no switching is done:
      switching = false;
      rows = table.rows;
      /* Loop through all table rows (except the
      first, which contains table headers): */
      for (i = 1; i < (rows.length - 1); i++) {
        // Start by saying there should be no switching:
        shouldSwitch = false;
        /* Get the two elements you want to compare,
        one from current row and one from the next: */
        x = rows[i].getElementsByTagName("TD")[n];
        y = rows[i + 1].getElementsByTagName("TD")[n];
        /* Check if the two rows should switch place,
        based on the direction, asc or desc: */
        if (dir == "asc") {
          if (x.innerHTML.toLowerCase() > y.innerHTML.toLowerCase()) {
            // If so, mark as a switch and break the loop:
            shouldSwitch = true;
            break;
          }
        } else if (dir == "desc") {
          if (x.innerHTML.toLowerCase() < y.innerHTML.toLowerCase()) {
            // If so, mark as a switch and break the loop:
            shouldSwitch = true;
            break;
          }
        }
      }
      if (shouldSwitch) {
        /* If a switch has been marked, make the switch
        and mark that a switch has been done: */
        rows[i].parentNode.insertBefore(rows[i + 1], rows[i]);
        switching = true;
        // Each time a switch is done, increase this count by 1:
        switchcount ++;
      } else {
        /* If no switching has been done AND the direction is "asc",
        set the direction to "desc" and run the while loop again. */
        if (switchcount == 0 && dir == "asc") {
          dir = "desc";
          switching = true;
        }
      }
    }
  }
</script>

{% include JB/setup %}

<hr>

<h1> Experimental Results for Quantum (Enhanced) Support Vector Machine (QSVM) on IRIS Dataset </h1>

<hr>

<h2> Preface </h2>

<ul>
  <li> In this page... </li>
</ul>

<hr>

<h2> Experimental Results </h2>

<ul>
  <li> The results... </li>
</ul>


<br />
<b> Note(s): </b>
<ul>
  <li> For these results, was used the <b>Quantum Support Vector Classifier (QSVC)</b> from <a href="https://www.ibm.com/quantum/qiskit"><b>Qiskit</b></a> library, namely through the <a href="https://qiskit-community.github.io/qiskit-machine-learning/index.html"><b>Qiskit Machine Learning</b></a> module. For more information, see the following link:</li>
  <ul>
    <li> <a href="https://qiskit-community.github.io/qiskit-machine-learning/stubs/qiskit_machine_learning.algorithms.QSVC.html">https://qiskit-community.github.io/qiskit-machine-learning/stubs/qiskit_machine_learning.algorithms.QSVC.html</a> </li>
  </ul>
</ul>
<br />
<b> Footnote(s): </b>
<ul>
  <li>TODO</li>
</ul>

<hr>

<h2> License </h2>

<ul>
  <li> <a href="http://www.opensource.org/licenses/MIT"><b> MIT </b></a> </li>
</ul>

<hr>