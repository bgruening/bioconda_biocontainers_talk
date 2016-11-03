### Tool deployment and sustainability <br>in bioinformatics <br>:fa-check: Fixed

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

Do not you already have to deal with <br>a missing tool dependencies?

Or an older version of a tool could not be installed <br>due to various reasons?

**Major issues in deployment and sustainability**

Note: a major issue for productivity and reproducibility in science

---

# Deployment issue

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
  $ conda install package_name (+ time, take a huge package)
  ```
  
- Installation and management of multiple versions

Note: No need for root privileges

----

### A Conda package

![](http://localhost:8000/images/conda_files.png){no-border}

:fa-long-arrow-right: Easy to write!

Note: Extensive documentation

----

### Bioinformatics tools<br>![](http://localhost:8000/images/bioconda_logo.png){no-border}

![](http://localhost:8000/images/tool_development_bioconda_solution.png){no-border}

- More than 1,500 bioinformatic packages developed in one year
- Big and fast-growing community
- Newcomer welcoming

Note: Bioconda: a distribution of bioinformatics softwares using Conda

----

### Wants a Docker image?<br>![](http://localhost:8000/images/mulled.png){no-border}

![](http://localhost:8000/images/tool_development_mulled_solution.png){no-border}

Note: Wants an higher layer of abstraction and isolation of the base system?

----

### ![](http://localhost:8000/images/mulled.png){no-border}

A layer donning project to build <br>Docker container from conda package

*auto-mulled, simple scheme to explain mulled, cron..., give exemple of samtools container...*

----

### Deployment issue

![](http://localhost:8000/images/tool_development_mulled_solution.png){no-border}
### <br>:fa-check:Fixed!

*add rocket, singularity, ...*

---

# Sustainability issue

----

### :fa-bullseye: Wanted

A storage allowing
- Reachability of all packages
- Cache of all versions of the packages
- Permanent access

Note: Permanent cache of all available packages to be always reachable and enable reproducibility

----

### Cargo Port<br>An easy solution

*image*

Note: These packages are long-term stored in a public repository (Cargo Port), the distribution center of the Galaxy Project, resolving the sustainability issue

----

### Sustainability issue

*scheme summary*

### <br>:fa-check:Fixed!

---

# Conclusion

----

### Tool deployment and sustainability <br>in bioinformatics 

![](http://localhost:8000/images/tool_development_solution_scheme.png){no-border}

### <br>:fa-check:Fixed! 

Note: Community effort to create 
  - a flexible, 
  - scalable
  - sustainable system 
to fix the tool deployment problem once and for all
Development of conda packages through the Bioconda community eases the packaging and the deployment of any bioinformatic tool. The interface with Cargo Port enables sustainability by mirroring all sources. Building efficient Linux containers automatically ensures an even higher layer of abstraction and isolation of the base system. Thanks to these collaborative projects, their community and their collaborations, bioinformatics tools can be easily packaged, deployed and will be always available to help biomedical research.

---

## Thank You.

### Questions?

![](http://localhost:8000/images/tool_development_final_scheme.png){no-border}
