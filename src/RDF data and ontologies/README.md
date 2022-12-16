# What data is provided?
This is an introduction into the organization of the RDF data. The data in this repository is organized to be reused for different [purposes](#How-to-use-this-data-for-different-purposes). 

## Overview of RDF files
In this repo you will find 
- the [individual RDF data files](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/tree/main/src/RDF%20data%20and%20ontologies/individual%20data%20files) that contain the data instances. In these files ontology concepts are used but do not contain their definitions. 
- The [individual OWL ontology files](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/tree/main/src/RDF%20data%20and%20ontologies/individual%20ontology%20files) that contain the ontological definitions to model the data semantically. The bfo2, the BWMD_mid and one domain ontology per RDF data set was used. The corresponding domain ontology of each RDF data file can be exctracted from the image above. 
- The [individual RDF alignment files](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/tree/main/src/RDF%20data%20and%20ontologies/individual%20alignment%20files) serve to link different RDF data with each other semantically, e.g between nodes that represent the same specimen/component (identified by the same PartID), are provided. 

- In this very folder ([RDF data and ontologies](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/edit/main/src/RDF%20data%20and%20ontologies)) you find RDF files in which all individual data files and the necessary ontologies are merged. Different versions are provided. You can find the specialties of each version described in the image above. The multitude of RDF files is provided so the data can be used for different purposes, that are described below.

<!-- add link to purposes here -->

An overview of the available RDF and ontology files can be found in the following image:

![Datafiles](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/blob/main/doc/Datafiles.png?raw=true)

In the AluTrace project raw data was semantically modelled using the top-level ontology [bfo2](https://github.com/bfo-ontology/BFO/wiki#news-bfo-20-now-released) and the mid-level ontology [BWMD_mid](https://matportal.org/ontologies/BWMD-MID). The raw data used originated from the previous Web4GenMet project and was purposefully supplemented with raw data produced in the AluTrace project itself. The raw data was semantically modeled per material-intensive subprocess executed at the corresponding institution (EMI, IWM or fem). The colors highlight the institution where the owner of the data (EMI, IWM or fem). One individual RDF data file results from one subprocess. The modelled subprocesses are:

## Subprocesses performed within the Web4GenMet project
- Laser powder bed fusion additive manufacturing process (**LPBFprocess**) using AlSi10Mg metal powder, performed at EMI
- Stress-relief annealing (**HeatTreatment**) of the specimen manufactured in the LPBF process, performed at EMI
- Materials characterization (**TensileTest**), performed at IWM
- Fatigue test on materials and defect analysis upon plastic deformation (**LowCycleFatigue+Defects**) and upon elastic deformation (**HighCycleFatigue+Defects**), performed at IWM

## Subprocesses performed within the AluTrace project
- Measurement of the exact composition of the AlSi10Mg Powder used as input for the LPBF process (**PowderComposition**), performed at fem
- Laser powder bed fusion additive manufacturing process (**LPBFprocess**) using AlSi10Mg metal powder, performed at fem
- Computer tomography and defects analysis of via LPBF manufactured parts (**CT+Defects**), performed at fem
- Separation of specimen/components and preparation for further analysis (**Separating**) , performed at IWM
- Solution Annealing and artificial aging of separated specimen/components (**HeatTreatment**), performed at IWM
- Measurement of the Brinell hardness of the processed specimen/components (**HardnessMeasurement**), performed at IWM
- Mechanical testing of the processed specimen (**TensileTest**), performed at IWM
- Mechanical testing of the processed components (**TensileTest**), performed at IWM

## Ontolgical ressources
The data was modeled per subprocess using the following ontologies:  

**Top-level Ontology**  
- [BFO2](https://github.com/bfo-ontology/BFO/wiki#news-bfo-20-now-released)  
  
**Mid-level Ontology**  
- [BWMD_mid](https://matportal.org/ontologies/BWMD-MID)  
  
**Domain-level Ontologies**  
- [BWMD_domain](https://matportal.org/ontologies/BWMD-DOMAIN)
- [LPBFO](https://matportal.org/ontologies/LPBFO)
- [emiHT](https://gitlab.cc-asp.fraunhofer.de/EMI_datamanagement/LPBFO/-/raw/emiHT/EMIHT_ontology.owl) 
- fatigue
- defects

## How to use this data for different purposes
**Purpose1: I am not interested in RDF data but in the materials characteristics you observed.**
  - Please direct yourself to the [SPARQL queries and results](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/tree/main/src/SPARQL%20queries%20and%20results) folder and retrieve the csv-files with materials characteristics.  
  
**Purpose2: I want to use the final RDF data and perform exploratory queries on it.**
    - If you use a triple store with advanced reasoning capabilites, choose AluTrace-Web4GenMet-LD.trig 
    - If you use a triple store without advanced reasoning capabilities, choose AluTrace-Web4GenMet-LD-inferred.ttl 
    - You can start with the queries provided in the [SPARQL queries and results](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/tree/main/src/SPARQL%20queries%20and%20results) folder. 
    
**Purpose3: I want to use the whole set of RDF data to experiment with rulesets for reasoning.**
  - You can choose AluTrace-Web4GenMet-LD.trig and choose the ruleset according to your needs. 
  - If you plan to investigate how your query behaves upon the interaction between alignment and ruleset, you should choose AluTrace.trig, Web4GenMet.trig, create your own alignment or choose alignments from the [individual alignment files](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/tree/main/src/RDF%20data%20and%20ontologies/individual%20alignment%20files) folder. 
    - If your triple store doesn't support to query over all named graphs you can choose AluTrace.ttl and Web4GenMet.ttl instead.
  
**Purpose4: I want to query the individual RDF data.**
  - Please direct yourself to the [individual data files](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/tree/main/src/RDF%20data%20and%20ontologies/individual%20data%20files) folder and choose the data you want.  
  
**Purpose4-1: I want to experiment with the ontologies chosen for the RDF data.**
  - Please direct yourself to the [individual ontology files](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/tree/main/src/RDF%20data%20and%20ontologies/individual%20ontology%20files) folder and choose the ontologies you need. Remember that all data uses bfo2 and BWMD_mid, the corresponding domain-ontology for each data file you can find in the image above.   
    
**Purpose4-2: I want to experiment with the alignment of the RDF data. **
  - You can find prepared alignments in the folder [individual alignment files](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/tree/main/src/RDF%20data%20and%20ontologies/individual%20alignment%20files). 

**Purpose5: I want to use the data from different sources to experiment with decetralized data management architectures.**
  - Please direct yourself to the [individual data files](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/tree/main/src/RDF%20data%20and%20ontologies/individual%20data%20files) folder, choose the data you want and place it where you need it in the architecture.   
  - Please direct yourself to the [individual ontology files](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/tree/main/src/RDF%20data%20and%20ontologies/individual%20ontology%20files) folder, choose the ontologies you need and place it where you need it in the architecture. Remember that all data uses bfo2 and BWMD_mid, the corresponding domain-ontology for each data file you can find in the image above.   
  - Please direct yourself to the [individual alignment files](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/tree/main/src/RDF%20data%20and%20ontologies/individual%20alignment%20files) folder and place the alignment where you need it in the architecture. 





