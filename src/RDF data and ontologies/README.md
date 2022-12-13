# What data is provided?
This is an introduction into the organization and the content of the RDF data. The data in this repository is organized in a way so it can be reused for different purposes. An overview over the available RDF and ontology files can be found in the following image:

![Datafiles](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/blob/main/Datafiles.png?raw=true)

In the AluTrace project raw data was semantically modelled using the top-level ontology [bfo2](https://github.com/bfo-ontology/BFO/wiki#news-bfo-20-now-released) and the mid-level ontology [BWMD_mid](https://matportal.org/ontologies/BWMD-MID). The raw data used originated from the previous Web4GenMet project and was purposefully supplemented with raw data produced in the AluTrace project itself. The raw data was semantically modeled per material-intensive subprocess that was performed at the corresponding executive institution (EMI, IWM or fem). One individual RDF data file results from one subprocess which were the following:

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



