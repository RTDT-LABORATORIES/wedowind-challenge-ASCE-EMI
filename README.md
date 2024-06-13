# The WeDoWind ASCE-EMI Structural Health Monitoring for Wind Energy Challenge
Create a branch to work on your solution.


## RDA guidelines for FAIR open source code
Research Data Aliance -  FAIR Principles for Research Software can be found [here.](https://zenodo.org/record/6623556#.YqCJTJNBwlw)

Clarification of the criteria:

- F1 Software is assigned a globally unique and persistent identifier.
  - F1.1. Components of the software representing levels of granularity are assigned distinct identifiers.  
    This is handled by GitHub.
  - F1.2. Different versions of the software are assigned distinct identifiers.      
    We recommend to use semantic versioning. E.g. `version = "1.5.3"` defined in `pyproject.toml`  
    
- F2. Software is described with rich metadata.  
  This is difficult to implement atm, but if you want to talk about it, contact @time-trader  
  
- F3. Metadata clearly and explicitly include the identifier of the software they describe.  
  Requires F2
- F4. Metadata are FAIR, searchable and indexable.  
  Requires F2  
  
- A1. Software is retrievable by its identifier using a standardized communications protocol.
  These are handled by git and GitHub. E.g. `git clone <githubrepo>` and password-protected SSH key. 
  - A1.1. The protocol is open, free, and universally implementable.  
  - A1.2. The protocol allows for an authentication and authorization procedure, where
necessary.  
- A2. Metadata are accessible, even when the software is no longer available.  
   Requires F2    
  
- I1. Software reads, writes and exchanges data in a way that meets domain-relevant community standards.  
  We recommend creating building docs and publishing it with Read the Docs, API pages are automatically generated if the code is documented properly.
- I2. Software includes qualified references to other objects.    
  We recommend linking to papers and publications (DOI) used during the code development.  

- R1. Software is described with a plurality of accurate and relevant attributes.
  - R1.1. Software is given a clear and accessible license    
  Include license file. GitHub usaully automatically parses this information an makes it machine readable. Commonly used licences: MIT, Apache, GPL, Creative Commons.  
  - R1.2. Software is associated with detailed provenance.    
  This recommendation is partilally addressed by git commit history. Additionally, "good provenance metadata clarifies the origins and *intent* behind the development of the software, and establishes authenticity and trust." Therefore a paragraph on the overall intent should be added into the read me. Git commit messages should be expressive. We also highly reccomentd the use of commit type tags. E.g: FEA for new feature commit, FIX for bugfix commit, etc, We leave it open to choose your preferred tag system.  
  
- R2. Software includes qualified references to other software.  
  Include all the requirements needed for the code to compile and run. E.g. `[tool.poetry.dependencies]` in `pyproject.toml` and `poetry.lock` file 
- R3. Software meets domain-relevant community standards.  
  Not community standards available atm. 
