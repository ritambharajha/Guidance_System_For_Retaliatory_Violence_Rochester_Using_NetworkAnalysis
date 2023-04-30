# Guidance_System_For_Retaliatory_Violence_Rochester_Using_NetworkAnalysis

This project aim is to design a tool that offers the law enforcement community in Rochester helpful direction, information, and best practices on crucial problem-oriented policing, strategic policing principles, and retaliatory violence.

Networks are graphical representations of the connections (edges) between variables (nodes). Network analysis can predict complicated patterns of linkages, and the network structure may be analyzed to reveal key network elements.

We have a Python file to analyze the data and generate a network which is included with this document.

The coding environment used is Google Colab and will require python3 as well as the following packages: networkx, pandas, matplotlib, scikit-learn.

Dataset is a pair of 2 excel files containing nodes and edges.

Node file contains - MCAC ID(number assigned to dispute bulletins by MCAC analysts), ID, Names and victim, suspect, witness.

Edge file contains - MCAC ID , ID, Name.

After the notebook is set up, the python file(.IPYNB) can be executed cell by cell.

Following files are executed - 
1. Individual_Level_NetworkAnalysis.ipynb - This file displays the generation of networks at an individual-level, each individual (if involved in a dispute) being a node. Also, it displays the centrality scores.
2. Dispute_Level_Network.ipynb - This file displays the generation of networks at dispute-level, each dispute being a node. Edge is created when same suspects are involved in two disputes. Also, it displays the centrality scores.
3. Prediction.ipynb - This files contains the execute of model and it's optimization
4. Justice_System_Factors_Prediction.ipynb - This file displays the execution of support vector regression model for justice system factors data such as - active disputants caught with weapon, shotspotter activation, jail intelligence and uncooperative witness.
5. Dispute_Violence_Enhancers_Prediction.ipynb - This file displays the execution of support vector regression model for dispute violence enhancer data such as - family retaliation, proxy attack, innocent bystander, family retaliation etc.
6. Dispute_Characteristic_Prediction.ipynb - This file displays the execution of support vector regression model for dispute characteristics data such as - gang involed, inter-gang feud, robbery, drugs/property, neighbor dispute etc.
7.Demographic_Prediction.ipynb - This file displays the execution of support vector regression model for the demographic indicator data such as - Percent Victim Male, Percent Victim Black, Percent Victim Latino, Percent Victim Age etc.
