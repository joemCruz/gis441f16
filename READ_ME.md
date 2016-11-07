# Requirements Analysis Document
## PySAL - QGIS Integration

### 1. Introduction
  1. Purpose
    * PySAL - QGIS Integration intends to allow the integration of certain portions of the PySAL library within the GIS system, QGIS.
    * This project focuses on the addition of the Spatial Dynamics - Markov based methods library to the PySAL-QGIS integration toolkit.
  2. Scope of your package
  
  Users of the software PySAL and/or QGIS.
  3. Objectives and success metrics 
    * PySAL and QGIS can be considered successfully integrated when the Markov based methods can be accessed and utilized within QGIS with readable and meaningful results.
    ..* The data located within QGIS is readable and can be analyzed by PySAL methods.
    ..* Additional data columns are added to the existing data within QGIS that will depict the result of one of the Markov based methods.
    ..* A map is produced that accurately reflects the results calculated above.
    * The interface that allows a QGIS user to use the Markov based methods within PySAL allows the user to use the three forms of Markov based analysis located within the library. i.e. Class Markov, Spatial Markov, and LISA Markov
  4. Definitions, terms
    
  5. References
    * "Discover QGIS." Discover QGIS. QGIS, n.d. Web. 25 Oct. 2016. [QGIS](http://www.qgis.org/en/site/about/index.html)
    * PySAL Developers. "PySAL." PySAL — Python Spatial Analysis Library. PySAL Developers, 2014. Web. 25 Oct. 2016. [PySAL](http://pysal.readthedocs.io/en/latest/index.html)
  6. Overview
  This project focuses on combining the strengths of PySAL and QGIS. Inherently, PySAL is a library of spatial analytics methods, developed in Python, of which QGIS lacks in some areas. QGIS, on the other hand, has a ready to use graphical user interface. For example, QGIS lacks the ability to analyze data using any form of Markov chaining, however, PySAL contains methods to do just that. PySAL, as of this moment, lacks the ability to display its own maps whereas QGIS can. By combining the functionality of the two, a user will be able to analyze a geospatial problem and draw a map without having to go between QGIS and PySAL or some other set of libraries as everything will be handled within the QGIS interface.
  
### 2. Current System
  1. Description of existing project
  
  PySAL is an open source library of spatial analysis functions written in Python intended to support the development of high level applications. PySAL is open source under the BSD License. [PySAL](http://pysal.readthedocs.io/en/latest/index.html)
  
  QGIS is a user friendly Open Source Geographic Information System (GIS) licensed under the GNU General Public License. [QGIS](http://www.qgis.org/en/site/about/index.html)
  
  PySAL
  2. How does the project extend existing work
  The project extends the functionality inherent within PySAL into the QGIS platform. This allows for functions not found within QGIS, but found within PySAL, to be used in QGIS' graphical interface.
  3. What tasks does the new system support
  The interoperability between PySAL and QGIS will result in the PySAL methods being usable by QGIS. This will allow QGIS to apply its loaded, spatial files with accompanying data to be analyzed by the methods developed in PySAL.
  
### 3. System Proposal
1. Overview
This system will provide the necessary integration between PySAL and QGIS.
2. Functional Requirements
  1. Features to be implemented
    * All programming will be done in Python.
    * The modules will be done in Python 2.7 since QGIS does not use Python 3.
    * PySAL-QGIS integration is a module that will be modifiable.
    ..* The actual code will be well-commented.
    * Markov based methods within PySAL's spatial dynamics library will be given the ability to interact with QGIS.
    * A toolkit for QGIS will be developed:
    * A drop down menu in the QGIS toolkit will list the three forms of Markov based methods (Classic Markov, Spatial Markov, and LISA Markov) will be included.
    ..* From this drop down menu, only one method will be selectable at a time.
  2. Mock-ups (sketches) of features
3. Nonfunctional Requirements
  1. Useability
    PySAL-QGIS interoperability will be available only on Linux (as of October 24, 2016)
  2. Reliability
  3. Performance
  4. Supportability
  5. Implementation
    Both modules will be built utilizing Python 2.7
  6. Interface
    PySAL-QGIS Integration will be handled with QGIS' package handling software.
  7. Packaging
    PySAL-QGIS Integration will be an on its own package. It will need to be manually added to QGIS for the time being.
  8. Licensing
    BSD
           
### 4. Project Management
1. Schedule
  1. Detailed milestones for project
2. Repositories
  1. URL for project repository
