# SNA
## Social Network Analysis of all commits to eclipse/che repository
This code uses the metadata of over 8000 commits to make a network of developers that have worked together in the eclipse/che repository. An edge exists between two developers if one developer uploaded a file and a second developer made a commit to it. Only the developers that have edges are graphed in the final representation of the network as there are many nodes already and nodes without edges do not provide much insight in this context.

To run SNAFinal you will need Python, Networkx, matplotlib and Jupyter Notebook installed. To not exceed the default data limit of jupyter notebook, open jupyter notebook from the Command Prompt with the following line (Windows OS):

jupyter notebook --NotebookApp.iopub_data_rate_limit=1.0e10 

Add commitsF.json to the same folder as SNAFinal.ipynb within your jupyter notebook. To run the program, open SNAFinal.ipynb in your jupyter notebook and choose Kernel->Restart and run all

Occassionally the last cell must be run twice for the graph to show. If this happens, simply click within the last cell and hold shift while pressing enter. This should display the graph.
