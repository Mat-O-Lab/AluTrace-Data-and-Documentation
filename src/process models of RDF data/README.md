# What is the process model useful for?
The workflow for semantic modeling of data is based on the [IWM-GDTool](https://gitlab.cc-asp.fraunhofer.de/gf7_public/iwm-gdtool). According to the author, GDTool is a lightweight approach to creating ontology-oriented datasets in a scientific workflow environment. The tool supports three steps:

1. Creation of a process model that is based on an OWL-ontology and to be used with the [Knowledgebase Builder](https://inforapid.org/webapp/login.php). In the Knowledgebase Builder the user draws a process schema similar to a SPARQL INSERT statement. This process model is a template for a knowledge graph and defines its structure.  

2. Transformation of the graphical process model to an Excel file. In Excel the user enters Literal values similar to binding values to the variables of the SPARQL INSERT statement.  

4. Transformation of the Excel file with the Literal values to a RDF data file (knowledge graph) for further validation and processing.  


**The process model is not only necessary to create the RDF data within workflow, but it is also very useful to understand the RDF data structure. You can either just view a PNG-image of the process model or upload it to the [Knowledgebase Builder](https://inforapid.org/webapp/login.php) and explore it.**

Each process model is named just like the [individual RDF data file](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/tree/main/src/RDF%20data%20and%20ontologies/individual%20data%20files) it was used as template for. 

## Further Reading
- [GDTool-documentation](https://gitlab.cc-asp.fraunhofer.de/gf7_public/iwm-gdtool/-/wikis/GDTool-documentation).
- [Digital Workflow using the GDTool](https://gitlab.cc-asp.fraunhofer.de/gf7_public/iwm-gdtool/-/wikis/GDTool-documentation)
