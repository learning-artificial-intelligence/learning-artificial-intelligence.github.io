---
layout: results
category: experimental-results
title: "Experimental Results for Quantum (Enhanced) Support Vector Machine (QSVM) with Quantum Kernel Training (QKT) on IRIS Dataset"
tagline: "Classification results obtained from tuning several hyperparameters of Quantum (Enhanced) Support Vector Machine (QSVM) with Quantum Kernel Training (QKT) on IRIS Dataset..."
author: Rúben André Barreiro
tags: [artificial-intelligence, computer-science, quantum-support-vector-machine, support-vector-machine, quantum-kernel-training, kernel-training,  quantum-kernel-alignment, kernel-alignment, quantum-machine-learning, machine-learning, supervised-learning, training, classification, iris-dataset, intermediate]
keywords: quantum support vector machine, support vector machine, quantum kernel training, kernel training,  quantum kernel alignment, kernel alignment, quantum machine learning, machine learning, training, supervised learning, training, classification, iris dataset, beginner, artificial intelligence, ai
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
      new TableFilter("quantum-svm-qkt-qka-adam-optimizer-iris-dataset-exp-results",
                      filtersConfig);

  tableFilter.init();
</script>
<script>
  function sortTable(n) {
    var table, rows, switching, i, x, y, shouldSwitch, dir, switchcount = 0;
    table = document.getElementById("quantum-svm-qkt-qka-adam-optimizer-iris-dataset-exp-results");
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

<h1> Experimental Results for Quantum (Enhanced) Support Vector Machine (QSVM) with Quantum Kernel Training (QKT)/Quantum Kernel Alignment (QKA) on IRIS Dataset </h1>

<hr>

<h2> Preface </h2>

<ul>
  <li> In this page... </li>
</ul>

<hr>

<h2> Experimental Results </h2>

<ul>
  <li> The experimental results will be available soon... </li>
</ul>


<hr>


<h3> Local Optimizers </h3>


<hr>


<h5> ADAptive Moment (ADAM) </h5>

<ul>
  <li> The experimental results... </li>
</ul>

<table id="quantum-svm-qkt-qka-adam-optimizer-iris-dataset-exp-results" border="1" class="tg">
  <thead>
    <tr style="text-align: center;">
      <th onclick="sortTable(0)">No.</th>
      <th onclick="sortTable(1)">MaxIter<sup>&yen;</sup></th>
      <th onclick="sortTable(2)">Tol<sup>&sect;</sup></th>
      <th onclick="sortTable(3)">LR<sup>&dagger;</sup></th>
      <th onclick="sortTable(4)">Accuracy<sup>&Dagger;</sup></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>20</td>
      <td>1e-08</td>
      <td>1e-06</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>1</th>
      <td>20</td>
      <td>1e-08</td>
      <td>5e-06</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>2</th>
      <td>20</td>
      <td>1e-08</td>
      <td>1e-05</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>3</th>
      <td>20</td>
      <td>1e-08</td>
      <td>5e-05</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>4</th>
      <td>20</td>
      <td>1e-08</td>
      <td>0.0001</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>5</th>
      <td>20</td>
      <td>1e-08</td>
      <td>0.0005</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>6</th>
      <td>20</td>
      <td>1e-08</td>
      <td>0.001</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>7</th>
      <td>20</td>
      <td>1e-08</td>
      <td>0.005</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>8</th>
      <td>20</td>
      <td>1e-08</td>
      <td>0.01</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>9</th>
      <td>20</td>
      <td>1e-08</td>
      <td>0.05</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>10</th>
      <td>20</td>
      <td>1e-08</td>
      <td>0.1</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>11</th>
      <td>20</td>
      <td>1e-08</td>
      <td>0.5</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>12</th>
      <td>20</td>
      <td>1e-08</td>
      <td>1.0</td>
      <td><span style="color:#17A589"><b>1.00000</b></span></td>
    </tr>
    <tr>
      <th>13</th>
      <td>20</td>
      <td>1e-07</td>
      <td>1e-06</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>14</th>
      <td>20</td>
      <td>1e-07</td>
      <td>5e-06</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>15</th>
      <td>20</td>
      <td>1e-07</td>
      <td>1e-05</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>16</th>
      <td>20</td>
      <td>1e-07</td>
      <td>5e-05</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>17</th>
      <td>20</td>
      <td>1e-07</td>
      <td>0.0001</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>18</th>
      <td>20</td>
      <td>1e-07</td>
      <td>0.0005</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>19</th>
      <td>20</td>
      <td>1e-07</td>
      <td>0.001</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>20</th>
      <td>20</td>
      <td>1e-07</td>
      <td>0.005</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>21</th>
      <td>20</td>
      <td>1e-07</td>
      <td>0.01</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>22</th>
      <td>20</td>
      <td>1e-07</td>
      <td>0.05</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>23</th>
      <td>20</td>
      <td>1e-07</td>
      <td>0.1</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>24</th>
      <td>20</td>
      <td>1e-07</td>
      <td>0.5</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>25</th>
      <td>20</td>
      <td>1e-07</td>
      <td>1.0</td>
      <td><span style="color:#17A589"><b>1.00000</b></span></td>
    </tr>
    <tr>
      <th>26</th>
      <td>20</td>
      <td>1e-06</td>
      <td>1e-06</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>27</th>
      <td>20</td>
      <td>1e-06</td>
      <td>5e-06</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>28</th>
      <td>20</td>
      <td>1e-06</td>
      <td>1e-05</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>29</th>
      <td>20</td>
      <td>1e-06</td>
      <td>5e-05</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>30</th>
      <td>20</td>
      <td>1e-06</td>
      <td>0.0001</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>31</th>
      <td>20</td>
      <td>1e-06</td>
      <td>0.0005</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>32</th>
      <td>20</td>
      <td>1e-06</td>
      <td>0.001</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>33</th>
      <td>20</td>
      <td>1e-06</td>
      <td>0.005</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>34</th>
      <td>20</td>
      <td>1e-06</td>
      <td>0.01</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>35</th>
      <td>20</td>
      <td>1e-06</td>
      <td>0.05</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>36</th>
      <td>20</td>
      <td>1e-06</td>
      <td>0.1</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>37</th>
      <td>20</td>
      <td>1e-06</td>
      <td>0.5</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>38</th>
      <td>20</td>
      <td>1e-06</td>
      <td>1.0</td>
      <td><span style="color:#17A589"><b>1.00000</b></span></td>
    </tr>
    <tr>
      <th>39</th>
      <td>20</td>
      <td>1e-05</td>
      <td>1e-06</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>40</th>
      <td>20</td>
      <td>1e-05</td>
      <td>5e-06</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>41</th>
      <td>20</td>
      <td>1e-05</td>
      <td>1e-05</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>42</th>
      <td>20</td>
      <td>1e-05</td>
      <td>5e-05</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>43</th>
      <td>20</td>
      <td>1e-05</td>
      <td>0.0001</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>44</th>
      <td>20</td>
      <td>1e-05</td>
      <td>0.0005</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>45</th>
      <td>20</td>
      <td>1e-05</td>
      <td>0.001</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>46</th>
      <td>20</td>
      <td>1e-05</td>
      <td>0.005</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>47</th>
      <td>20</td>
      <td>1e-05</td>
      <td>0.01</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>48</th>
      <td>20</td>
      <td>1e-05</td>
      <td>0.05</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>49</th>
      <td>20</td>
      <td>1e-05</td>
      <td>0.1</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>50</th>
      <td>20</td>
      <td>1e-05</td>
      <td>0.5</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>51</th>
      <td>20</td>
      <td>1e-05</td>
      <td>1.0</td>
      <td><span style="color:#17A589"><b>1.00000</b></span></td>
    </tr>
    <tr>
      <th>52</th>
      <td>20</td>
      <td>0.0001</td>
      <td>1e-06</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>53</th>
      <td>20</td>
      <td>0.0001</td>
      <td>5e-06</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>54</th>
      <td>20</td>
      <td>0.0001</td>
      <td>1e-05</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>55</th>
      <td>20</td>
      <td>0.0001</td>
      <td>5e-05</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>56</th>
      <td>20</td>
      <td>0.0001</td>
      <td>0.0001</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>57</th>
      <td>20</td>
      <td>0.0001</td>
      <td>0.0005</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>58</th>
      <td>20</td>
      <td>0.0001</td>
      <td>0.001</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>59</th>
      <td>20</td>
      <td>0.0001</td>
      <td>0.005</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>60</th>
      <td>20</td>
      <td>0.0001</td>
      <td>0.01</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>61</th>
      <td>20</td>
      <td>0.0001</td>
      <td>0.05</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>62</th>
      <td>20</td>
      <td>0.0001</td>
      <td>0.1</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>63</th>
      <td>20</td>
      <td>0.0001</td>
      <td>0.5</td>
      <td>0.95556</td>
    </tr>
    <tr>
      <th>64</th>
      <td>20</td>
      <td>0.0001</td>
      <td>1.0</td>
      <td><span style="color:#17A589"><b>1.00000</b></span></td>
    </tr>
  </tbody>
</table>


<br />
<b> Note(s): </b>
<ul>
  <li> For these results, it was used the <b>Quantum Support Vector Classifier (QSVC)</b> from <a href="https://www.ibm.com/quantum/qiskit"><b>Qiskit</b></a> library, namely through the <a href="https://qiskit-community.github.io/qiskit-machine-learning/index.html"><b>Qiskit Machine Learning</b></a> module. For more information, see the following link: </li>
  <ul>
    <li> <a href="https://qiskit-community.github.io/qiskit-machine-learning/stubs/qiskit_machine_learning.algorithms.QSVC.html">https://qiskit-community.github.io/qiskit-machine-learning/stubs/qiskit_machine_learning.algorithms.QSVC.html</a> </li>
  </ul>
  <li> Additionally, was also used the <b>Quantum Kernel Trainer</b> for the <b>Quantum Kernel Training (QKT)</b>/<b>Quantum Kernel Alignment (QKA)</b> complementar task, namely through the <a href="https://qiskit-community.github.io/qiskit-machine-learning/index.html"><b>Qiskit Machine Learning</b></a> module. For more information, see the following link: </li>
  <ul>
    <li> <a href="https://qiskit-community.github.io/qiskit-machine-learning/stubs/qiskit_machine_learning.kernels.algorithms.QuantumKernelTrainer.html">https://qiskit-community.github.io/qiskit-machine-learning/stubs/qiskit_machine_learning.kernels.algorithms.QuantumKernelTrainer.html</a> </li>
  </ul>
  <li> For the optimization algorithm chosen for the <b>Quantum Kernel Trainer</b>, it was used the <b>ADAptive Moment (ADAM)</b> optimizer. For more information, see the following links: </li>
  <ul>
    <li> <a href="https://qiskit-community.github.io/qiskit-algorithms/stubs/qiskit_algorithms.optimizers.ADAM.html">https://qiskit-community.github.io/qiskit-algorithms/stubs/qiskit_algorithms.optimizers.ADAM.html</a> </li>
  </ul>
</ul>
<br />
<b> Footnote(s): </b>
<ul>
  <li> &yen; - This hyperparameter represents the <b>Maximum Number of Iterations</b> of the optimizer. </li>
  <li> &sect; - This hyperparameter represents the <b>Tolerance Error</b> of the optimizer. </li>
  <li> &dagger; - This hyperparameter represents the <b>Learning Rate</b> of the optimizer. </li>
  <li> &Dagger; - The higher <b>Accuracy</b> values are highlighted in <span style="color:#17A589"><b>green</b></span> and the lowest <b>Accuracy</b> values are highlighted in <span style="color:#C0392B"><b>red</b></span>. </li>
</ul>


<hr>


<h5> AccuMulated Squared GRADient (AMSGRAD) </h5>

<ul>
  <li> The experimental results will be available soon... </li>
</ul>


<h5> Conjugate Gradient (CG) </h5>

<ul>
  <li> The experimental results will be available soon... </li>
</ul>


<h5> Constrained Optimization By Linear Approximation (COBYLA) </h5>

<ul>
  <li> The experimental results will be available soon... </li>
</ul>


<h5> Limited-memory - Broyden-Fletcher-Goldfarb-Shanno - Bound (L-BFGS-B) </h5>

<ul>
  <li> The experimental results will be available soon... </li>
</ul>


<h5> Gaussian-Smoothed Line Search (GSLS) </h5>

<ul>
  <li> The experimental results will be available soon... </li>
</ul>


<h5> Gradient Descent (GD) </h5>

<ul>
  <li> The experimental results will be available soon... </li>
</ul>


<h5> Nakanishi-Fujii-Todo (NFT) </h5>

<ul>
  <li> The experimental results will be available soon... </li>
</ul>


<h5> Nelder Mead (NM) </h5>

<ul>
  <li> The experimental results will be available soon... </li>
</ul>


<h5> Parallelized - limited-memory - Broyden-Fletcher-Goldfarb-Shanno (P-BFGS) </h5>

<ul>
  <li> The experimental results will be available soon... </li>
</ul>


<h5> Powell </h5>

<ul>
  <li> The experimental results will be available soon... </li>
</ul>


<h5> Sequential Least SQuares Programming (SLSQP) </h5>

<ul>
  <li> The experimental results will be available soon... </li>
</ul>


<h5> Simultaneous Perturbation Stochastic Approximation (SPSA) </h5>

<ul>
  <li> The experimental results will be available soon... </li>
</ul>


<h5> Quantum Natural - Simultaneous Perturbation Stochastic Approximation (QNSPSA) </h5>

<ul>
  <li> The experimental results will be available soon... </li>
</ul>


<h5> Truncated Newton Conjugate (TNC) </h5>

<ul>
  <li> The experimental results will be available soon... </li>
</ul>


<h5> (Continuous) Univariate Marginal Distribution Algorithm (UMDA) </h5>

<ul>
  <li> The experimental results will be available soon... </li>
</ul>


<hr>


<h3> Global Optimizers </h3>


<hr>


<h5> Controlled Random Search (CRS) </h5>

<ul>
  <li> The experimental results will be available soon... </li>
</ul>


<h5> DIviding RECTangles Locally-biased (DIRECT-L) </h5>

<ul>
  <li> The experimental results will be available soon... </li>
</ul>


<h5> DIviding RECTangles Locally-biased RANDndomized (DIRECT-L-RAND) </h5>

<ul>
  <li> The experimental results will be available soon... </li>
</ul>


<h5> Evolutionary Strategy-Carlos Henrique (ESCH) </h5>

<ul>
  <li> The experimental results will be available soon... </li>
</ul>


<h5> Improved Stochastic Ranking Evolution Strategy (ISRES) </h5>

<ul>
  <li> The experimental results will be available soon... </li>
</ul>


<hr>



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
