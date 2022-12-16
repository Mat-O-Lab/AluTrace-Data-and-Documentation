# What is the process model useful for?
The workflow for semantic modeling of data is based on the [IWM-GDTool](https://gitlab.cc-asp.fraunhofer.de/gf7_public/iwm-gdtool). According to the author is GDTool a lightweight approach to creating ontology-oriented datasets in a scientific workflow environment. The tool supports three steps:

**1. Creation of a process model that is based on an OWL-ontology and to be used with the [Knowledgebase Builder](https://inforapid.org/webapp/login.php). In the Knowledgebase Builder the user draws a process schema similar to a SPARQL INSERT statement. This process model is a template for a knowledge graph and defines its structure.**
2. Transformation of the graphical process model to an Excel file. In Excel the user enters Literal values similar to binding values to the variables of the SPARQL INSERT statement.
3. Transformation of the Excel file with the Literal values to a RDF data file (knowledge graph) for further validation and processing.

The process model is not only necessary to create the RDF data with this worklow, but it is also very useful to understand the data structure. You can either just few a PNG-image of the process model or upload it to the [Knowledgebase Builder](https://inforapid.org/webapp/login.php) and explore it. 

## Further Reading
- [GDTool-documentation](https://gitlab.cc-asp.fraunhofer.de/gf7_public/iwm-gdtool/-/wikis/GDTool-documentation).
- [Digital Workflow using the GDTool](https://gitlab.cc-asp.fraunhofer.de/gf7_public/iwm-gdtool/-/wikis/GDTool-documentation)
