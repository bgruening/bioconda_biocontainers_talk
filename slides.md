### Tool deployment and sustainability <br>in bioinformatics <br><i class="fa fa-check"></i> Fixed<br><br>

**Bérénice Batut**, Jonas Weber, Rolf Backofen, Björn Grüning

<small>
University of Freiburg<br><br>Bioinformatics for Human Health and Disease<br>Heidelberg - November 2016
</small> 

---

### Biomedical research

Generation of massive amounts of diverse data

<i class="fa fa-long-arrow-right"></i> Need of bioinformatic solutions and tools

----

### How to develop a tool?

![](images/tool_development_1.png)

Note: Development of some source code that can be distributed as it is

----

### How to develop a tool?

![](images/tool_development_packaging.png)

Note: To help its deployment and ease the usage of the tools, the code is packaged in various package formats.
The tool behind the code is then deployed and used by the targeted users.
 
----

### How to develop a tool?<br>The Golden Path

![](images/tool_development_training_doc_support.png)

Note: documentation, training and support are also provided to help users, spread the solution and advertise it. 

----

### But...

Do not you already have to deal with <br>a missing tool dependencies?

Or an older version of a tool could not be installed <br>due to various reasons?

**Major issues in deployment and sustainability**

Note: a major issue for productivity and reproducibility in science

---

# Deployment issue

----

### <i class="fa fa-bullseye"></i> Wanted

A package manager
- Programming language agnostic
- OS independent
- Needed no root privileges
- Managing multiple versions
    
Note: Development of bioinformatic tools in mostly all available languages and Tools used on every major operating systems

----

### A good solution<br>![](images/conda_logo.png)

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

![](images/conda_package.png)

<i class="fa fa-long-arrow-right"></i> Easy to write!

Note: Extensive documentation

----

### Bioinformatics tools<br>![](images/bioconda_logo.png)

![](images/tool_development_bioconda_solution.png)

- More than 1,500 bioinformatic packages developed in one year
- Big, fast-growing and newcomer-friendly community

Note: Bioconda: a distribution of bioinformatics softwares using Conda

----

### Wants a Docker image?<br>![](images/mulled.png)

![](images/tool_development_mulled_solution.png)

Note: Wants an higher layer of abstraction and isolation of the base system?

----

### Mulled

A layer donning project to build Docker container

![](images/mulled_scheme_without_bioconda.png)

----

### Mulled

![](images/mulled_scheme.png)

Note: less than 10Mb for samtools

----

### Deployment issue

![](images/tool_development_deployment.png)

### <i class="fa fa-check"></i>Fixed!

---

# Sustainability issue

----

### <i class="fa fa-bullseye"></i> Wanted

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

![](images/tool_development_sustainability.png)

### <i class="fa fa-check"></i>Fixed!

---

# Conclusion

----

### Tool deployment and sustainability <br>in bioinformatics 

![](images/tool_development_solution_scheme.png)

### <i class="fa fa-check"></i>Fixed! 

Note: Community effort to create 
  - a flexible, 
  - scalable
  - sustainable system 
to fix the tool deployment problem once and for all
Development of conda packages through the Bioconda community eases the packaging and the deployment of any bioinformatic tool. The interface with Cargo Port enables sustainability by mirroring all sources. Building efficient Linux containers automatically ensures an even higher layer of abstraction and isolation of the base system. Thanks to these collaborative projects, their community and their collaborations, bioinformatics tools can be easily packaged, deployed and will be always available to help biomedical research.

---

### Thank You<br>Questions?

![](images/tool_development_final_scheme.png)
