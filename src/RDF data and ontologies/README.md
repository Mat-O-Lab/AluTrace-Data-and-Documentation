# What data is provided?
This is an introduction into the organization of the RDF data. The data in this repository is organized to be reused for different [purposes](#How-to-use-this-data-for-different-purposes). 

## Overview of RDF files
In this folder you can find: 
- the [individual data files](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/tree/main/src/RDF%20data%20and%20ontologies/individual%20data%20files) (RDF) that contain the data instances. In these files ontology concepts are used but do not contain their definitions. 
- The [individual ontology files](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/tree/main/src/RDF%20data%20and%20ontologies/individual%20ontology%20files) (OWL) that contain the ontological definitions that were used to model the data semantically. The [bfo2](https://github.com/bfo-ontology/BFO/wiki#news-bfo-20-now-released), the [BWMD_mid](https://matportal.org/ontologies/BWMD-MID) and one domain ontology per RDF data set was used. The corresponding domain ontology of each RDF data file can be exctracted from the image above and is described in more detail in the [ontology folder](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/tree/main/src/RDF%20data%20and%20ontologies/individual%20ontology%20files). 
- The [individual alignment files](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/tree/main/src/RDF%20data%20and%20ontologies/individual%20alignment%20files) (RDF) serve to link different RDF data with each other semantically, e.g to link nodes that represent the same specimen/component with the same PartID but have different IRIs. 

- In this very folder ([RDF data and ontologies](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/edit/main/src/RDF%20data%20and%20ontologies)) you find RDF files in which all individual data files and the necessary ontologies are merged. Different versions are provided. You can find the specialties of each version described in the image below.

The multitude of different RDF files are provided so the data can be used for different [purposes](#How-to-use-this-data-for-different-purposes).

<!-- add link to purposes here -->

An overview of the available RDF and ontology files can be found in the following image:

![Datafiles](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/blob/main/doc/Datafiles.png?raw=true)

In the AluTrace project raw data was semantically modelled using the top-level ontology [bfo2](https://github.com/bfo-ontology/BFO/wiki#news-bfo-20-now-released) and the mid-level ontology [BWMD_mid](https://matportal.org/ontologies/BWMD-MID). The raw data originates from the previous Web4GenMet project and was purposefully supplemented with raw data produced in the AluTrace project itself. The raw data was semantically modeled per material-intensive process executed at the corresponding institution (EMI, IWM or fem). The colors highlight the institution where the owner of the data (EMI, IWM or fem). One individual RDF data file results from one [process model](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/tree/main/src/process%20models%20of%20RDF%20data). 

## Overview of process models  
The data was modeled using the following material-intensive processes that generated it. The process models themselves can be found in the [process models of RDF data](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/tree/main/src/process%20models%20of%20RDF%20data) folder. 

### Modelled processes of the Web4GenMet project
- Laser powder bed fusion additive manufacturing process ([**LPBFprocess**](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/blob/main/src/process%20models%20of%20RDF%20data/Web4GenMet_EMI_LPBFprocess.png)) using AlSi10Mg metal powder, performed at EMI
- Stress-relief annealing ([**HeatTreatment**](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/blob/main/src/process%20models%20of%20RDF%20data/Web4GenMet_EMI_HeatTreatment.png)) of the specimen manufactured in the LPBF process, performed at EMI
- Materials characterization ([**TensileTest**](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/blob/main/src/process%20models%20of%20RDF%20data/Web4GenMet_IWM_TensileTest.png)), performed at IWM
- Fatigue test on materials and defect analysis upon plastic deformation ([**LowCycleFatigue+Defects**](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/blob/main/src/process%20models%20of%20RDF%20data/Web4GenMet_IWM_LCF%2BDefects.png)) and upon elastic deformation ([**HighCycleFatigue+Defects**](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/blob/main/src/process%20models%20of%20RDF%20data/Web4GenMet_IWM_HCF%2BDefects.png)), performed at IWM

### Modelled processes of the AluTrace project
- Measurement of the exact composition of the AlSi10Mg Powder used as input for the LPBF process ([**PowderComposition**](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/blob/main/src/process%20models%20of%20RDF%20data/AluTrace_fem_PowderComposition.png)), performed at fem
- Laser powder bed fusion additive manufacturing process ([**LPBFprocess**](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/blob/main/src/process%20models%20of%20RDF%20data/AluTrace_fem_LPBFprocess.png)) using AlSi10Mg metal powder, performed at fem
- Computer tomography and defects analysis of via LPBF manufactured parts ([**CT+Defects**](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/blob/main/src/process%20models%20of%20RDF%20data/AluTrace_fem_CT%2BDefects.png)), performed at fem
- Separation of specimen/components and preparation for further analysis ([**Separating**](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/blob/main/src/process%20models%20of%20RDF%20data/AluTrace_IWM_Separating.png)) , performed at IWM
- Solution Annealing and artificial aging of separated specimen/components (**HeatTreatment** ([SolutionAnnealing](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/blob/main/src/process%20models%20of%20RDF%20data/AluTrace_IWM_HeatTreatment_SolutionAnnealing.png)+[ArtificialAging](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/blob/main/src/process%20models%20of%20RDF%20data/AluTrace_IWM_HeatTreatment_ArtificialAging.png))), performed at IWM
- Measurement of the Brinell hardness of the processed specimen/components ([**HardnessMeasurement**]()), performed at IWM
- Mechanical testing of the processed specimen ([**TensileTest**](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/blob/main/src/process%20models%20of%20RDF%20data/AluTrace_IWM_TensileTest.png)), performed at IWM
- Mechanical testing of the processed components ([**ComponentTest**](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/blob/main/src/process%20models%20of%20RDF%20data/AluTrace_IWM_ComponentTest.png)), performed at IWM

## Overview of ontological resources
The data was modeled with the following ontologies according to the material-intensive process in which they were generated. The ontologies can be found in the [individual ontology files](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/tree/main/src/RDF%20data%20and%20ontologies/individual%20ontology%20files) folder.

![Ontologicalresources](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/blob/main/doc/Ontologicalresources.png?raw=true)

**Top-level Ontology**  
- [bfo2](https://github.com/bfo-ontology/BFO/wiki#news-bfo-20-now-released)  
  
**Mid-level Ontology**  
- [BWMD_mid](https://matportal.org/ontologies/BWMD-MID)  
  
**Domain-level Ontologies**  
- [BWMD_domain](https://matportal.org/ontologies/BWMD-DOMAIN)
- [LPBFO](https://matportal.org/ontologies/LPBFO)
- [emiHT](https://gitlab.cc-asp.fraunhofer.de/EMI_datamanagement/LPBFO/-/raw/emiHT/EMIHT_ontology.owl) 
- [fatigue](https://raw.githubusercontent.com/Mat-O-Lab/AluTrace-Data-and-Documentation/main/src/RDF%20data%20and%20ontologies/individual%20ontology%20files/fatigue.owl)
- [defects](https://raw.githubusercontent.com/Mat-O-Lab/AluTrace-Data-and-Documentation/main/src/RDF%20data%20and%20ontologies/individual%20ontology%20files/defects.owl)

## Overview of alignment files
In the [individual alignment files](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/tree/main/src/RDF%20data%20and%20ontologies/individual%20alignment%20files) folder the following alignments can be found. 

**Alignment on PartIDs**
- The alignment [AluTrace_alignment_PartIDs.ttl](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/blob/main/src/RDF%20data%20and%20ontologies/individual%20alignment%20files/AluTrace_alignment_PartIDs.ttl) was automatically created for data from the AluTrace project. Each instance of an object is matched by owl:sameAs to the instance of an object that has the same PartID as identifier. Alignments were generated between all individual AluTrace RDF data files where specimen/components were used across different processes. According to the overview of RDF files, this alignment is contained in the files [AluTrace-LD.trig](https://raw.githubusercontent.com/Mat-O-Lab/AluTrace-Data-and-Documentation/main/src/RDF%20data%20and%20ontologies/AluTrace-LD.trig), [AluTrace-LD-inferred.ttl](https://raw.githubusercontent.com/Mat-O-Lab/AluTrace-Data-and-Documentation/main/src/RDF%20data%20and%20ontologies/AluTrace-LD-inferred.ttl), [AluTrace-Web4GenMet-LD.trig](https://raw.githubusercontent.com/Mat-O-Lab/AluTrace-Data-and-Documentation/main/src/RDF%20data%20and%20ontologies/AluTrace-Web4GenMet-LD.trig) and [AluTrace-Web4GenMet-LD-inferred.ttl](https://raw.githubusercontent.com/Mat-O-Lab/AluTrace-Data-and-Documentation/main/src/RDF%20data%20and%20ontologies/AluTrace-Web4GenMet-LD-inferred.ttl).

- The alignment [Web4GenMet_alignment_PartIDs.ttl](https://raw.githubusercontent.com/Mat-O-Lab/AluTrace-Data-and-Documentation/main/src/RDF%20data%20and%20ontologies/individual%20alignment%20files/Web4GenMet_alignment_PartIDs.ttl) was created automatically for data from the Web4GenMet project. Each instance of an object is matched by owl:sameAs to the instance of an object that has the same PartID as identifier. Also each instance of a set of objects is matched by mid:hasPart to those instances of objects that are contained in that set. According to the overview of RDF files, this alignment is contained in the RDF data [Web4GenMet-LD.trig](https://raw.githubusercontent.com/Mat-O-Lab/AluTrace-Data-and-Documentation/main/src/RDF%20data%20and%20ontologies/Web4GenMet-LD.trig), [Web4GenMet-LD-inferred.ttl](https://raw.githubusercontent.com/Mat-O-Lab/AluTrace-Data-and-Documentation/main/src/RDF%20data%20and%20ontologies/Web4GenMet-LD-inferred.ttl), [AluTrace-Web4GenMet-LD.trig](https://raw.githubusercontent.com/Mat-O-Lab/AluTrace-Data-and-Documentation/main/src/RDF%20data%20and%20ontologies/AluTrace-Web4GenMet-LD.trig) and [AluTrace-Web4GenMet-LD-inferred.ttl](https://raw.githubusercontent.com/Mat-O-Lab/AluTrace-Data-and-Documentation/main/src/RDF%20data%20and%20ontologies/AluTrace-Web4GenMet-LD-inferred.ttl).

**Alignment on Identifier**
- The alignment [Web4GenMet_alignment_allIdentifier.ttl]([AluTrace_alignment_PartIDs.ttl](https://raw.githubusercontent.com/Mat-O-Lab/AluTrace-Data-and-Documentation/main/src/RDF%20data%20and%20ontologies/individual%20alignment%20files/Web4GenMet_alignment_allIdentifiers.ttl)) was created automatically for data from the Web4GenMet project. Each instance of an identifier is matched by owl:sameAs to the instance of an identifier that has the value. This alignment is not contained yet in other RDF data.  

# How to use this data for different purposes
**Purpose1: I am not interested in RDF data but in the materials characteristics that were observed.**
  - Please direct yourself to the [SPARQL queries and results](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/tree/main/src/SPARQL%20queries%20and%20results) folder and retrieve the csv-files with materials characteristics.  
  
**Purpose2: I want to use the whole set of RDF data and perform exploratory queries on it.**
  - If you use a triple store with reasoning capabilites, choose [AluTrace-Web4GenMet-LD.trig](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/raw/main/src/RDF%20data%20and%20ontologies/AluTrace-Web4GenMet-LD.trig).
  - If you use a triple store without reasoning capabilities, choose [AluTrace-Web4GenMet-LD-inferred.ttl](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/raw/main/src/RDF%20data%20and%20ontologies/AluTrace-Web4GenMet-LD-inferred.ttl).
  - You can start with the queries provided in the [SPARQL queries and results](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/tree/main/src/SPARQL%20queries%20and%20results) folder. 
  - The structure of the RDF data can be explored via the [process models of RDF data](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/tree/main/src/process%20models%20of%20RDF%20data).
    
**Purpose2-1: I want to use the whole set of RDF data to experiment with rulesets for reasoning.**
  - You can choose [AluTrace-Web4GenMet-LD.trig](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/raw/main/src/RDF%20data%20and%20ontologies/AluTrace-Web4GenMet-LD.trig) and experiment with rulesets according to your needs. 
  - If you plan to investigate how your query behaves upon the interaction between alignment and ruleset, you should choose [AluTrace.trig](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/raw/main/src/RDF%20data%20and%20ontologies/AluTrace.trig), [Web4GenMet.trig](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/raw/main/src/RDF%20data%20and%20ontologies/Web4GenMet.trig) and experiment with alignments and rulesets according to your needs.
    - If your triple store doesn't support the query over all named graphs you can choose [AluTrace.ttl](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/raw/main/src/RDF%20data%20and%20ontologies/AluTrace.ttl) and [Web4GenMet.ttl](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/raw/main/src/RDF%20data%20and%20ontologies/Web4GenMet.ttl) instead.
  
**Purpose3: I want to query the individual RDF data.**
  - Please direct yourself to the [individual data files](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/tree/main/src/RDF%20data%20and%20ontologies/individual%20data%20files) folder and choose the data you want.  
  -  The structure of the RDF data can be explored via the [process models of RDF data](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/tree/main/src/process%20models%20of%20RDF%20data).
  
**Purpose3-1: I want to use the individual RDF data and experiment with the ontologies chosen for the RDF data.**
  - Please direct yourself to the [individual ontology files](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/tree/main/src/RDF%20data%20and%20ontologies/individual%20ontology%20files) folder and choose the ontologies you need. Remember that all data uses bfo2 and BWMD_mid, the corresponding domain-ontology for each data file you can find in the image above.   
    
**Purpose3-2: I want to use the individual RDF data and and experiment with the alignment of the RDF data.**
  - You can find prepared alignments in the folder [individual alignment files](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/tree/main/src/RDF%20data%20and%20ontologies/individual%20alignment%20files). 

**Purpose4: I want to use the individual RDF data from different sources to experiment with decetralized data management architectures.**
  - Please direct yourself to the [individual data files](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/tree/main/src/RDF%20data%20and%20ontologies/individual%20data%20files) folder, choose the data you want and place it where you need it.   
  - Please direct yourself to the [individual ontology files](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/tree/main/src/RDF%20data%20and%20ontologies/individual%20ontology%20files) folder, choose the ontologies you need and place it where you need it. Remember that all data uses bfo2 and BWMD_mid, the corresponding domain-ontology for each data file you can find in the image above.   
  - Please direct yourself to the [individual alignment files](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/tree/main/src/RDF%20data%20and%20ontologies/individual%20alignment%20files) folder and place the alignment where you need it. 





