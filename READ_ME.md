# Requirements Analysis Document
## Pysal - QGIS Integration

### 1. Introduction
  1. Purpose
    * Pysal contains methods for Markov chains and concordance measures that it inherited from the STARS Package. New methods concerning the testing of Spatial Markov chaining, will be created, tested, and added to Pysal.
    * Pysal - QGIS Integration intends to allow the integration of certain portions of the Pysal library within the GIS system, QGIS.
  2. Scope of your package
  
  Users of the software Pysal and/or QGIS.
  3. Objectives and success metrics 
    * The development of Spatial Markov chaining will use the modules already in existence within the Pysal library. It will combine traditional Markov chaining with spatial weighting. This method will then be tested using two methods:
      1. All permutations across the scope of the data would be calculated. This generates a uniform reference distribution from which a sample can be procured and be applied to a Monte Carlo test to determine the significance of the findings.
      2. Recently developed goodness-of-fit tests for Markov chaining will be used. These test significant statistics within the transition probability matrix. Again, Monte Carlo sampling can be used to determine significance, or Markov chain Monte Carlo can be used instead.
    * Spatial Markov chaining will be considered successful whether or not it shows a significant difference between itself and traditional Markov chaining. This is in regards to data that is spatially distributed. 
    * Pysal and QGIS can be considered successfully integrated when the (elements specified) can be accessed and utilized within QGIS with readable and meaningful results. 
  4. Definitions, terms
  
    * MC := Markov chain
    * DMC := Discrete Markov chain
    * SMC := Spatial Markov chain
  
  5. References
    * NSF Proposal
    * "Discover QGIS." Discover QGIS. QGIS, n.d. Web. 25 Oct. 2016. [QGIS](http://www.qgis.org/en/site/about/index.html)
    * Pysal Developers. "PySAL." PySAL — Python Spatial Analysis Library. Pysal Developers, 2014. Web. 25 Oct. 2016. [Pysal](http://pysal.readthedocs.io/en/latest/index.html)
  6. Overview
  
### 2. Current System
  1. Description of existing project
  
  PySAL is an open source library of spatial analysis functions written in Python intended to support the development of high level applications. PySAL is open source under the BSD License. [Pysal Link](http://pysal.readthedocs.io/en/latest/index.html)
  
  QGIS is a user friendly Open Source Geographic Information System (GIS) licensed under the GNU General Public License. [QGIS Link](http://www.qgis.org/en/site/about/index.html)
  2. How does the project extend existing work
  Spatial methods involving MC exist within the Pysal library. These are inherited from Space-Time 
  The project extends the functionality inherent within Pysal into the QGIS platform. This allows for functions not found within QGIS, but found within Pysal, to be used in QGIS' graphical interface.
  3. What tasks does the new system support
    * The new system will include the ability to use SMC
  The interoperability between Pysal and QGIS will result in the Pysal methods being usable by QGIS. This will allow QGIS to apply its loaded, spatial files with accompanying data to be analyzed by the methods developed in Pysal.
  
### 3. System Proposal
1. Overview
This system will provide the necessary integration between Pysal and QGIS.
2. Functional Requirements
  1. Listing of features to be implemented
  2. Mock-ups (sketches) of features
3. Nonfunctional Requirements
  1. Useability
  2. Reliability
  3. Performance
  4. Supportability
  5. Implementation
  6. Interface
  7. Packaging
  8. Licensing
           
### 4. Project Management
1. Schedule
  1. Detailed milestones for project
2. Repositories
  1. URL for project repository
