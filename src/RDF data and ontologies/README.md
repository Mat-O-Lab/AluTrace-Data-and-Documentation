# What data is provided?
This is an introduction into the organization of the RDF data. The data in this repository is organized in a way so it can be reused in different [use cases](#Use-cases-of-this-data). An overview over the available RDF and ontology files can be found in the following image:

![Datafiles](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/blob/main/doc/Datafiles.png?raw=true)

In the AluTrace project raw data was semantically modelled using the top-level ontology [bfo2](https://github.com/bfo-ontology/BFO/wiki#news-bfo-20-now-released) and the mid-level ontology [BWMD_mid](https://matportal.org/ontologies/BWMD-MID). The raw data used originated from the previous Web4GenMet project and was purposefully supplemented with raw data produced in the AluTrace project itself. The raw data was semantically modeled per material-intensive subprocess that was performed at the corresponding executive institution (EMI, IWM or fem). One individual RDF data file results from one subprocess. The modelled subprocesses are:

### Subprocesses performed within the Web4GenMet project
- Laser powder bed fusion additive manufacturing process (**LPBFprocess**) using AlSi10Mg metal powder, performed at EMI
- Stress-relief annealing (**HeatTreatment**) of the specimen manufactured in the LPBF process, performed at EMI
- Materials characterization (**TensileTest**), performed at IWM
- Fatigue test on materials and defect analysis upon plastic deformation (**LowCycleFatigue+Defects**) and upon elastic deformation (**HighCycleFatigue+Defects**), performed at IWM

### Subprocesses performed within the AluTrace project
- Measurement of the exact composition of the AlSi10Mg Powder used as input for the LPBF process (**PowderComposition**), performed at fem
- Laser powder bed fusion additive manufacturing process (**LPBFprocess**) using AlSi10Mg metal powder, performed at fem
- Computer tomography and defects analysis of via LPBF manufactured parts (**CT+Defects**), performed at fem
- Separation of specimen/components and preparation for further analysis (**Separating**) , performed at IWM
- Solution Annealing and artificial aging of separated specimen/components (**HeatTreatment**), performed at IWM
- Measurement of the Brinell hardness of the processed specimen/components (**HardnessMeasurement**), performed at IWM
- Mechanical testing of the processed specimen (**TensileTest**), performed at IWM
- Mechanical testing of the processed components (**TensileTest**), performed at IWM

### Overview over RDF files
In this repo you will find the [individual RDF data files](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/tree/main/src/RDF%20data%20and%20ontologies/individual%20RDF%20files) which use ontology classes but do not contain ontological definitions. All ontologies can be found in the folder for the [individual ontology files](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/tree/main/src/RDF%20data%20and%20ontologies/individual%20ontology%20files). Each RDF data is produced using the bfo2, the BWMD_mid and one domain ontology. The corresponding domain ontology to each RDF data file can be exctracted from the image above. [Individual alignments](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/tree/main/src/RDF%20data%20and%20ontologies/individual%20alignments) of the RDF graphs e.g between nodes that represent the same specimen/component (identified by the same PartID) are provided. 

In this very folder, you can find RDF files that merge all RDF data files from each project and the necessary ontologies. You can find the specialties of each file described in the image above. The multitude of RDF files is provided so the data can be used for different purposes, that are described as follows.

## Use cases of this data
<!-- - Play around with decetralization of knowledge graphs
- Play around with alignments
- play around with different reasoning rulesets
- play around not having a good reasoner
- play around not being able to resolve named graphs
- dont want to play around, just get me the tables!! -->

## Ressources
Ontological ressources used in the project include:  

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





