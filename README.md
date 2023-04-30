<H1><center>Guidance System For Retaliatory Violence in Rochester Using Network Analysis</center></H1>
<H3>Collaborators: Sreenidhi Sridhar, Ritambhara Jha, Carter Brazell</H3>

<H3> Objective:</H3> <p>To design a tool that offers the law enforcement community helpful directions, information and best practices for forecasting the level of violence in upcoming incidents that take place in Rochester.
</p>
<H3>Research Questions:</H3><ol><li>Can we develop dispute-level network indicators that explain violence outcomes for the disputes?</li>
<li>Is network analysis and centrality score a robust measure for prediction in retaliatory violence?</li>
<li>Holding network predictors constant, what other dispute characteristics drive the retaliatory violence?</li></ol>
<H3>Network Analysis:</H3> <P> We perform network analysis and created 2 types of networks. A node is any individual that is part of the network. A person’s or a group’s influence is inversely related to the size of that node. An edge is a link or bond between two individuals or groups.
Individual-level network has each suspect as a node and an edge is created between 2 Individuals when they both are involved in the same dispute.
Whereas, in Dispute-level network each dispute  is a nodes and an edge is created when we have common people involved in both the disputes.
With each network created, we generated different centrality scores as network measures.
To create these measures for dispute level, we used several aggregate functions for each measure in individual-level centrality scores.
We observed that the medians of centrality scores for each dispute gave an accurate representation of the network
</P> Measures used to analyze the networks are:
<ol><li>Closeness Centrality</li>
<li>Betweenness Centrality</li>
<li>Eigen Vector Centrality</li>
<li>Degree Centrality</li>
<li>Clustering Coefficient</li></ol>
Files and description:
<ul><li>Individual_Level_NetworkAnalysis.ipynb - This file displays the generation of networks at an individual-level, each individual (if involved in a dispute) being a node. Also, it displays the centrality scores.</li>
<li>Dispute_Level_Network.ipynb - This file displays the generation of networks at dispute-level, each dispute being a node. Edge is created when same suspects are involved in two disputes. Also, it displays the centrality scores.</li></ul>
<H3>Prediction:</H3>
<p>With all these averages, medians and other dispute level metrics we proceed with the prediction.</p> 
We performed 6 machine learning algorithms such as <ol><li>Linear regression
<li>Logistic Regression</li>
<li>Support vector regression</li>
<li>Decision Tree Regressor</li>
<li>Ada-boost</li>
<li>Random forest regression</li></ol>
<p>To analyze these algorithms we are using the root mean squared error as our performance metric. 
After performing grid search to enhance all the models, support vector regressor gave the best results.</p>
Files and description:
<ul><li>Prediction.ipynb - This files contains the execute of model and it's optimization</li>
<li>Justice_System_Factors_Prediction.ipynb - This file displays the execution of support vector regression model for justice system factors data such as - active disputants caught with weapon, shotspotter activation, jail intelligence and uncooperative witness.</li>
<li>Dispute_Violence_Enhancers_Prediction.ipynb - This file displays the execution of support vector regression model for dispute violence enhancer data such as - family retaliation, proxy attack, innocent bystander, family retaliation etc.</li>
<li>Dispute_Characteristic_Prediction.ipynb - This file displays the execution of support vector regression model for dispute characteristics data such as - gang involed, inter-gang feud, robbery, drugs/property, neighbor dispute etc.</li>
<li>Demographic_Prediction.ipynb - This file displays the execution of support vector regression model for the demographic indicator data such as - Percent Victim Male, Percent Victim Black, Percent Victim Latino, Percent Victim Age etc.</li></ul>
<H3>Conclusion:</H3><ul><li>After analyzing all the network-level measures we conclude that the violent attribute which is the variable that represents the total number of violent incidents has been a significant metric to analyze the disputes.</li>
<li>Violent incidents considered in this system are homicide, assault shooting, shots fired, robbery, menacing, fights with weapons, and fights. </li>
<li>Using Support Vector Regressor we can get accurate result (less error rate) in predicting the violent measure for future crimes.</li></ul>

