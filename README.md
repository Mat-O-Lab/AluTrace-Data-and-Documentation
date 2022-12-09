# AluTrace Data and Documentation
The AluTrace Project was a project funded by the german Ministry of Economics, Labor and Tourism Baden-Württemberg (Ministerium für Wirtschaft, Arbeit und Tourismus Baden-Württemberg) from January 21st 2020 through December 31st 2021 under the case number 34-4224.044/21. 

Aim of the project was to digitally link data and knowledge silos that arise over industrial product development and manufacturing cycles. This linked data was used in order to answer a particular use case, allowing a design engineer to optimize a component with regard to lightweight design for additive manufacturing. 

The project consortium, consisting of the [Fraunhofer Institute for High-Speed Dynamics, Ernst-Mach-Institut, EMI](https://www.emi.fraunhofer.de/en/business-units/automotive/research/digitales-datenmanagement.html), [Fraunhofer Institute for 
Mechanics of Materials IWM](https://www.iwm.fraunhofer.de/) and [fem Research Institute for Precious Metals and Metal Chemistry](https://www.fem-online.de/) used legacy data and supplemented it specifically to generate RDF data. The RDF data is provided decentrally via the very first implementation of the [Materials Data Space](https://www.materials.fraunhofer.de/de/strategische-initativen/materials-data-space-/aktuelles-/erste-mds-implementierung-.html).  

## Deliverables
This repository contains the deliverables for this project, including 
- src: 
  - the RDF data,   
  - the SPARQL queries written for the project along with the returns of those SPARQL queries, 
  - the process graphs as templates for the individual RDF data sets 

- doc:
  - the final report, 
  - a supporting set of presentation slides.

## Ressources
Other ressources used in the project include:  
**Top-level Ontology**  
- [BFO2](https://github.com/bfo-ontology/BFO/wiki#news-bfo-20-now-released)  
**Mid-level Ontology**  
- [BWMD_mid](https://matportal.org/ontologies/BWMD-MID)  
**Domain-level Ontologies**  
- [BWMD_domain](https://matportal.org/ontologies/BWMD-DOMAIN)
- [LPBFO](https://matportal.org/ontologies/LPBFO)
- emiHT 
- fatigue
- defects

## Related Literature
-   Focus on the data space implementation: [Position Paper](https://www.trusts-data.eu/wp-content/uploads/2022/06/01-The-AluTrace-Use-Case-Harnessing-Lightweight-Design-Potentials-via-the-Materials-Data-Space.pdf), [Lightning Talk](https://www.youtube.com/watch?v=4FoApZMCrSw)
-   Focus on the design algorithm: [Technical Article (German)](https://www.ingenieur.de/fachmedien/wt-werkstattstechnik/fraunhofer-gesellschaft/leichtbau-datenvernetzung-fuer-additive-fertigung/)

<!-- ## Evaluation of FAIRness of this data
https://www.fosteropenscience.eu/learning/assessing-the-fairness-of-data/#/id/5c52e8cf0d3def29462d8cb5
-->

## Contributors (alphabetically)

- Valerie Friedmann, [Fraunhofer IWM](https://www.iwm.fraunhofer.de)    
- Michael Dlugosch, [Fraunhofer EMI](https://www.emi.fraunhofer.de)  
- Elena Garcia Trelles, [Fraunhofer IWM](https://www.iwm.fraunhofer.de) 
- Klaus Hoschke, [Fraunhofer EMI](https://www.emi.fraunhofer.de)
- Martin Huschka, [Fraunhofer EMI](https://www.emi.fraunhofer.de) 
- Ulrich Klotz, [fem](https://www.fem-online.de)    
- Sankalp Patil, [Fraunhofer EMI](https://www.emi.fraunhofer.de)   
- Johannes Preußner, [Fraunhofer IWM](https://www.iwm.fraunhofer.de)  
- Christoph Schweizer, [Fraunhofer IWM](https://www.iwm.fraunhofer.de)   
- Dario Tiberto, [fem](https://www.fem-online.de)  

## Contact

**Martin Huschka**, Michael Dlugosch, Klaus Hoschke, Sankalp Patil  
Fraunhofer-Institut für Kurzzeitdynamik, Ernst-Mach-Institut, EMI  
Ernst-Zermelo-Str. 4, 79104 Freiburg  
*first-name* [.] *last-name* [at] emi [dot] fraunhofer [dot] de  
[www.emi.fraunhofer.de](https://www.emi.fraunhofer.de) 

**Christoph Schweizer**, Valerie Friedmann, Johannes Preußner, Elena Garcia Trelles  
Fraunhofer-Institut für Werkstoffmechanik IWM  
Wöhlerstr. 11, 79108 Freiburg  
*first-name* [.] *last-name* [at] iwm [dot] fraunhofer [dot] de  
[www.iwm.fraunhofer.de](https://www.iwm.fraunhofer.de) 

**Ulrich Klotz**, Dario Tiberto  
fem Forschungsinstitut Edelmetalle + Metallchemie  
Katharinenstr. 17, 73525 Schwäbisch Gmünd  
*last-name* [at] fem-online [dot] de  
[www.fem-online.de ](https://www.fem-online.de) 




