---
title: "Stimulating the use of FAIR data sharing in the lifesciences"
date: "November 29, 2023"
excerpt: "The ASPAR_KR project hopes to promote the FAIRification of the Aspergillus field"
collection: portfolio
tags: 
  - "Master thesis"
  - "FAIR principles"
  - "ASPAR_KR platform"
---

# Why  do *Aspergillus* researcher need better data sharing?

*Aspergillus fumigatus* is a opportunistic pathogen of humans that usually lives saprotrophically in agricultural waste (Figure 1). In modern agriculture, the use of fungicides to combat diseases such as *Botrytis* in tulips is common. The fungicides end up together with *A. fumigatus* in the compost heaps. These compost heaps are quite extreme, within the heap, temperatures can reach up to 50°C. Luckily for *A. fumigatus* (and unluckily for us), *A. fumigatus* actually likes these temperatures, so it ends up being the only fungus in the heap.  As the azole concentration in the heap is quite high, *A. fumigatus* quickly develops azole resistance.

<figure>
<img src='/images/aspar-Aspergillus-fumigatus-thrives-in-numerous-environmental-niches-Spores-from-diverse.jpeg' alt="Spread and effects of A. fumigatus.">
<figcaption> Figure 1: Image from <a href="https://journals.asm.org/doi/10.1128/mbio.00135-17">Keller. (2017)</a> </figcaption>
</figure> 

Azole resistance in *A. fumigatus* is an issue, as the mould is quite lethal in patients with a repressed immune system, since azole resistant stains are quite difficult to treat. Many researchers are investigating how the resistance works, how it occurs and where it occurs and much knowledge has been obtained using modern biology methods, such as CRISPR-CAS9, and sequencing technologies. 

However, there is a issue in the data sharing: researchers usually put their data in an excel sheet or zip file and place this on the website of the publisher. While this is perfectly suitable for judging the quality of the scientific work, and perhaps for analysing the data for a different question, it is very difficult to get an overview of these disconnected datasets. The lack of overview causes unneeded work: people may "new" collect data that already exists, and a lot of unneeded work is put into merging data sets.

The main way to solve this limitation, is to adopt [FAIR data principles](https://www.go-fair.org/fair-principles/) within the *Aspergillus fumigatus* domain.  According to FAIR, data should be indexed at a searchable location, this location must be publicly available (perhaps with authenication), the stored data must be described in a standard format that can be combined with other FAIR data sources. 

<figure>
<img src='/images/aspar-fair.png' alt="The 5 star model for FAIR data quality">
<figcaption> Figure 2: Diagramme of FAIR <a href="https://www.nlm.nih.gov/oet/ed/cde/tutorial/02-200.html">(from NLM)</a> </figcaption>
</figure> 



<!-- 

<figure>
<img src='/images/aspar-5-star_deployment_scheme_for_Open_Data.png' alt="The 5 star model for FAIR data quality">
<figcaption> The 5 star model of FAIR data quality, devised by<a href="https://5stardata.info/en/">Sir Tim Berners-Lee</a> </figcaption>
</figure> 

-->

# What will be done about it?

Currently, me, [Mariana Santos](https://www.linkedin.com/in/marianasilva9/) and [Anna Fensel](https://sites.google.com/site/annafensel/) are working on a system to ease data sharing for *Aspergillus* researchers, called the *Aspergillus fumigatus* knowledge repository (ASPAR_KR). The [FAIRDS](https://fairds.fairbydesign.nl/)  as been offered as a possible solution, as it can use excel sheets with generated templates for generating a linked data file. 

The programme models each aspect of a general experimental workflow (see image below). In *investigation*, the paper for which all the experiments are done, is described. *Study* describes all the subquestions of an investigation. *Observation unit* describes what was observed to answer a question. The *Sample* and *Assay* classes are used to note down the results.

<figure>
<img src='/images/aspar-main-classes.png' alt="The main data classes of the FAIRDS.">
<figcaption> Figure 3: The main data classes of the FAIRDS. </figcaption>
</figure> 

When the user fills the aforementioned data in an [excel sheet](https://docs.google.com/spreadsheets/d/1ilkm_1ZYc3tN-mLB-UQDwIQiUL4QqRdC/edit?usp=sharing&ouid=106029892893667737101&rtpof=true&sd=true) an [rdf](https://en.wikipedia.org/wiki/Resource_Description_Framework) file is made that can be uploaded to a graph database, or analysed with an rdf library in [R](https://cran.r-project.org/web/packages/rdflib/index.html) or [python](https://rdflib.readthedocs.io/en/stable/).



# Where can I find more information?

* [My talk about this topic](/talks/2023-11-03-aspar-kr).
* [The documentation of ASPAR_KR](https://bookdown.org/sibbe_l_bakker/aspar_kr/intro.html#what-is-fair-data).
* [The website of ASPAR_KR](https://www.aspar.website/).



 
