### Tool deployment and sustainability <br>in bioinformatics <br>:fa-check: Fixed<br><br>

**Bérénice Batut**, Jonas Weber, Rolf Backofen, Björn Grüning

::: small
University of Freiburg<br><br>Bioinformatics for Human Health and Disease<br>Heidelberg - November 2016
::: 

---

### Biomedical research

Generation of massive amounts of diverse data

:fa-long-arrow-right: Need of bioinformatic solutions and tools

----

### How to develop a tool?

![](http://localhost:8000/images/tool_development_1.png){no-border}

Note: Development of some source code that can be distributed as it is

----

### How to develop a tool?

![](http://localhost:8000/images/tool_development_packaging.png){no-border}

Note: To help its deployment and ease the usage of the tools, the code is packaged in various package formats.
The tool behind the code is then deployed and used by the targeted users.
 
----

### How to develop a tool?<br>The Golden Path

![](http://localhost:8000/images/tool_development_training_doc_support.png){no-border}

Note: documentation, training and support are also provided to help users, spread the solution and advertise it. 

----

### But...

Who has never deal with a missing tool dependencies?<br>
Or an older version of a tool could not be installed?

### :fa-exclamation-triangle: Major issues in <br>deployment and sustainability

Note: a major issue for productivity and reproducibility in science

---

## Deployment issue

----

### :fa-bullseye: Wanted

A package manager
- Programming language agnostic
- OS independent
- Needed no root privileges
- Managing multiple versions
    
Note: Development of bioinformatic tools in mostly all available languages and Tools used on every major operating systems

----

### A good solution<br>![](http://localhost:8000/images/conda_logo.png){no-border}

- Open Source package manager
- Independent of any programming language and OS
- Fast, robust and easy package installation

  ```
  $ conda install deeptools
  ```
  
- Installation and management of multiple versions

Note: No need for root privileges, Less than 1 minute to install deeptools with conda

----

### A Conda package

![](http://localhost:8000/images/conda_package.png){no-border}

:fa-long-arrow-right: Easy to write!

Note: Extensive documentation

----

### Bioinformatics tools<br>![](http://localhost:8000/images/bioconda_logo.png){no-border}

![](http://localhost:8000/images/tool_development_bioconda_solution.png){no-border}

- More than 1,500 bioinformatic packages
- Big, fast-growing and newcomer-friendly community

Note: Bioconda: a distribution of bioinformatics softwares using Conda

----

### Wants a Docker image?<br>![](http://localhost:8000/images/mulled.png){no-border}

![](http://localhost:8000/images/tool_development_mulled_solution.png){no-border}

Note: Wants an higher layer of abstraction and isolation of the base system?

----

### Mulled

A layer donning project to build Docker container

![](http://localhost:8000/images/mulled_scheme_without_bioconda.png){no-border}

----

### Mulled

![](http://localhost:8000/images/mulled_scheme.png){no-border}

Note: less than 10Mb for samtools

----

### Deployment issue

![](http://localhost:8000/images/tool_development_deployment.png){no-border}

### :fa-check:Fixed!

---

## Sustainability issue

----

### :fa-bullseye: Wanted

A storage allowing
- Reachability of all packages
- Cache of all versions of the packages
- Permanent access

Note: Permanent cache of all available packages to be always reachable and enable reproducibility

----

### A solution<br>Cargo Port

- [A Public repository](https://depot.galaxyproject.org/software/) of the Galaxy Project
- Stable and long term storage
- Daily archives of the BioConda packages

----

### Sustainability issue

![](http://localhost:8000/images/tool_development_sustainability.png){no-border}

### :fa-check:Fixed!

---

### Tool deployment and sustainability <br>in bioinformatics 

![](http://localhost:8000/images/tool_development_solution_scheme.png){no-border}

### :fa-check:Fixed! 

Note: Community effort to create 
  - a flexible, 
  - scalable
  - sustainable system 
to fix the tool deployment problem once and for all
Development of conda packages through the Bioconda community eases the packaging and the deployment of any bioinformatic tool. The interface with Cargo Port enables sustainability by mirroring all sources. Building efficient Linux containers automatically ensures an even higher layer of abstraction and isolation of the base system. Thanks to these collaborative projects, their community and their collaborations, bioinformatics tools can be easily packaged, deployed and will be always available to help biomedical research.

---

### Thank You<br>Questions?

![](http://localhost:8000/images/tool_development_final_scheme.png){no-border}
