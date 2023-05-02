Download Link: https://assignmentchef.com/product/solved-cpe695-homework2-the-bias-variance-trade-off
<br>
<ol>

 <li>Please answer the following questions related to Machine Learning concepts:

  <ol>

   <li>[3 points] Explain what is the bias-variance trade-off?</li>

  </ol></li>

</ol>




<ol start="2">

 <li>[3 points] Describe few techniques to reduce bias and variance respectively.</li>

</ol>




<ol start="3">

 <li>[4 points] Describe following regression measures:

  <ul>

   <li>RMSE, 2) R<sup>2</sup></li>

  </ul></li>

</ol>




<ol start="4">

 <li>[10 points] Explain following concepts related to classification measures:

  <ul>

   <li>confusion matrix,</li>

   <li>precision,</li>

   <li>recall,</li>

   <li>F<sub>1</sub> score,</li>

   <li>ROC curve.</li>

  </ul></li>

 <li>Please answer the following questions related to Concept Learning:

  <ol start="5">

   <li>[<em>10 points</em>] Consider the following training examples (which is similar to EnjoySpt but with slightly different attributes) and the hypothesis space H that we described in lecture 3-2 (i.e., hypothesis is conjunction of attributes).</li>

  </ol></li>

</ol>

<table width="0">

 <tbody>

  <tr>

   <td width="60"> </td>

   <td width="108">Temp</td>

   <td width="102">Humidity</td>

   <td width="96">Water</td>

   <td width="102">Sky</td>

   <td width="108">EnjoySport</td>

  </tr>

  <tr>

   <td width="60">1</td>

   <td width="108">Warm</td>

   <td width="102">Normal</td>

   <td width="96">Warm</td>

   <td width="102">Sunny</td>

   <td width="108">Yes</td>

  </tr>

  <tr>

   <td width="60">2</td>

   <td width="108">Warm</td>

   <td width="102">Normal</td>

   <td width="96">Cold</td>

   <td width="102">Sunny</td>

   <td width="108">Yes</td>

  </tr>

  <tr>

   <td width="60">3</td>

   <td width="108">Cold</td>

   <td width="102">Normal</td>

   <td width="96">Warm</td>

   <td width="102">Rainy</td>

   <td width="108">No</td>

  </tr>

  <tr>

   <td width="60">4</td>

   <td width="108">Warm</td>

   <td width="102">High</td>

   <td width="96">Warm</td>

   <td width="102">Sunny</td>

   <td width="108">Yes</td>

  </tr>

 </tbody>

</table>




Trace the Candidate-Elimination algorithm to show the sequence of S and G boundary sets.




<ul>

 <li>Programming problem (40 points):

  <ol start="6">

   <li>In this programming problem, you will get familiar with building a decision tree, using cross validation to prune a tree, evaluating the tree performance, and interpreting the result.</li>

  </ol></li>

</ul>




Potential packages to use and short tutorials:

(1)http://scikit-learn.org/stable/modules/tree.html

(2)<u><a href="http://chrisstrelioff.ws/sandbox/2015/06/25/decision_trees_in_python_again_cross_validation.html">http://chrisstrelioff.ws/sandbox/2015/06/25/decision_trees_in_python_again_cross </a><a href="http://chrisstrelioff.ws/sandbox/2015/06/25/decision_trees_in_python_again_cross_validation.html">_validation.html</a></u>







<strong>classification tree </strong>




Use the titanic.csv dataset included in the assignment.




<strong>Step 1:</strong> read in Titanic.csv and observe a few samples, some features are categorical and others are numerical. Take a random 70% samples for training and the rest 30% for test.




<strong>Step 2:</strong> fit a decision tree model using independent variables ‘pclass + sex + age + sibsp’ and dependent variable ‘survived’. Plot the full tree. Make sure ‘survived’ is a qualitative variable taking 1 (yes) or 0 (no) in your code. You may see a tree similar to this one:







<strong>Step 3:</strong> check the performance of the full model: in‐sample and out-of‐sample accuracy, defined as:

in‐sample percent survivors correctly predicted (on training set) in-sample percent fatalities correctly predicted (on training set) out‐of‐sample percent survivors correctly predicted (on test set) out-of‐sample percent fatalities correctly predicted (on test set)




<strong>Step 4:</strong> use cross‐validation to find the best parameter to prune the tree. You should be able to plot a graph with the ‘tree size’ as the x-axis and ‘number of misclassification’ as the Y-axis. Find the minimum number of misclassification and choose the corresponding tree size to prune the tree. You may have a plot similar to:










<strong>Step 5:</strong> prune the tree with the optimal tree size. Plot the pruned tree. You may see a similar tree like this:







<strong>Step 6:</strong> Report as many details as you can on the final pruned tree.




Required reports on: in‐sample and out‐of‐sample accuracy, defined as




in‐sample percent survivors correctly predicted (on training set) in‐sample percent fatalities correctly predicted (on training set) out‐of‐sample percent survivors correctly predicted (on test set) out‐of‐sample percent fatalities correctly predicted (on test set)




Check whether there is improvement in out‐of‐sample for the full tree (bigger model) and the pruned tree (smaller model).





