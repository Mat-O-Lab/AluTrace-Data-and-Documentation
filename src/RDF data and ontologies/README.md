# What data is provided?
This is an introduction into the organization and the content of the RDF data. 

In the AluTrace project raw data was semantically modeled using the top-level ontology [bfo2](https://github.com/bfo-ontology/BFO/wiki#news-bfo-20-now-released) and the mid-level ontology [BWMD_mid](https://matportal.org/ontologies/BWMD-MID). The raw data used originated from the previous Web4GenMet project and was purposefully supplemented with raw data produced in the AluTrace project itself. The raw data was semantically modeled per material-intensive subprocess that was performed at the corresponding executive institution (EMI, IWM or fem). One individual RDF data file results from one subprocess which were the following:

### Subprocesses performed within the Web4GenMet project
- Laser powder bed fusion additive manufacturing process (**LPBFprocess**) using AlSi10Mg metal powder, performed at EMI
- Stress-relief annealing (**HeatTreatment**) of the specimen manufactured in the LPBF process, performed at EMI
- Materials characterization (**TensileTest**), performed at IWM
- Fatigue test on materials and defect analysis upon plastic deformation (**LowCycleFatigue+Defects**) and upon elastic deformation (**HighCycleFatigue+Defects**) 

### Subprocesses performed within the AluTrace project
- Measurement of the composition of the aluminium powder used as input for the LPBF process (**PowderComposition**)
- 
