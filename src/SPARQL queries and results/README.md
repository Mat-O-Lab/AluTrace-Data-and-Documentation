# What do these queries describe?
The queries are to be used with one of the aligned RDF data sets:
- If you use a triple store with reasoning capabilities: [AluTrace-Web4GenMet-LD.trig](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/blob/main/src/RDF%20data%20and%20ontologies/AluTrace-Web4GenMet-LD.trig). 
- If you use a triple store without reasoning capabilities: [AluTrace-Web4GenMet-LD-inferred.ttl](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/blob/main/src/RDF%20data%20and%20ontologies/AluTrace-Web4GenMet-LD-inferred.ttl)

The queries were developed using GraphDB 9.9.1 and the OWL-Horst (Optimized) ruleset.

You can find the queries that were necessary to fulfil the AluTrace use case:
- [**AluTrace_MaterialCharacteristicsDependentOnProcessParameters.sq**](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/blob/main/src/SPARQL%20queries%20and%20results/AluTrace_MaterialCharacteristicsDependentOnProcessParameters.sq)
  - This query retrieves from the AluTrace-LD data set the materials characteristics that were observed in dependency from varying process parameters in laser powder bed fusion. 
- [**Web4GenMet_MaterialCharacteristicsDependentOnProcessParameters.sq**](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation/blob/main/src/SPARQL%20queries%20and%20results/Web4GenMet_MaterialCharacteristicsDependentOnProcessParameters.sq)
  - This query retrieves from the Web4GenMet-LD data set the materials characteristics that were observed in dependency from varying process parameters in laser powder bed fusion. 
  
If any questions arise or if you have any feedback, please don't hesitate to [contact us](https://github.com/Mat-O-Lab/AluTrace-Data-and-Documentation#contact)!
