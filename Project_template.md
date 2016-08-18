**Date: 2016-08-10**

*Andrew -- testing out my first branch and commit edits in Github. I'll put all my comments in italics to distinguish them. Let me know if I should change the way we do this. -Steve*

# Working titles:    
1. Quantitative genetic architecture of growth under dynamic/multiple stressors in Poplar.

*This is by far my favorite title. We may want to tweak it a bit down the road to bring in some or all of the following ideas: function-valued traits, genomic prediction, gradient of growing season length*


2. Understanding evolutionary constraints in growth under multiple stressors in Poplar.
3. Persistance of Poplar in a the face of a changing environment.
4. Determinants of resiliency to environmental change in Poplar.  

# Table of Contents: 
* [Question 1. How does the quantitative genetic architecture of (woody biomass -- see my comment below TOC) shift alongside a variable environment? ](#id-section1).   

*Woody biomass is a trait that agro-foresters care about and therefore should be part of the "sell" here, but I would not focus specifically on this in terms of setting up your questions. Instead, I would focus on the ecologically interesting traits that may affect how much biomass trees are able to attain. Traits like stress tolerance (heat, drought, freezing), vegetative phenology, and growth/photosynthetic rates. We have data on lots of these traits from the common garden that we could help motivate this project with, as well as being able to use GBS-SNPs to enable genomic prediction of what phenotypes -should- look like for these same genotypes when grown in the field*

 
* [Question 2. Are there new shifts in episodic selection regimes in poplar?](#id-section2). 

*New in what sense? B/c of climate change? Relative to what -- selection in the source environment now? Historically? I think answers to these questions point to important directions to take the research.*


* [Broader Impacts](#id-section3). 
* [Intellectual merit](#id-section4). 
* [Timeline](#id-section5)




<div id='id-section1'/>
## **Question 1:** How does the quantitative genetic architecture of woody biomass shift alongside a variable environment? 

*QG architecture would only be expected to change if GxE was important. If all was Va for example, then the QG architecture is invariant with respect to the environment, but does set up different opportunities for selection to shape phenotypic distributions.*


**Hypothesis:** Local adaptation has produced constraints on certain genotypes to persist outside of their optimal operating environmental envelopes.

*Right, I think we set this up as a constraint problem, which is interesting from the evol-genetics perspective of what limits adaptation and how we can predict outcomes of selection in the field given knowledge of genetic architecture and history of local adaptation. This then has applied value in being able to make genomically-informed predictions of where a set of genotypes will optimize their growth trajectories given a set of environments (i.e., it becomes a fitness landscape problem).*

**Approach:** Leverage the ability to clone genotypes and rear 30-50 clones across a gradient of 9-12 common gardens to capture the ability for genotypes to operate under varying climates (growing degree day?).   

*Issue here is power for the QG variance (requires >N genotypes) vs. power to estimate the functional response (requires >N planting sites).  I think N=30 geno's is probably a good minimum #*

**Part 1. Next, we will assess growth performance (function-valued trait) across these common gardens and identify constraints within a quantitative genetic framework.**  

We will do this by estimating the broad-sense variance-covariance G-matrix and identify trade-offs by decomposing **G** with a PCA to quantify the correlational structure. Plot PCA loadings as a function of environment. 

*The key here is in choice of traits where correlations are expected, and in particular, where you might expect tradeoffs. I think the phenology traits are important (sprig bud flush and late-summer bud set) b/c they define the effective growing season for a genotype. Then the tradeoffs come with stress tolerance, both over-wintering (freeze tolerance) and during the growing season (heat/drought). Geno's that possess phenology that has them starting late and ending growth early tend to be more stress tolerant (and/or stress avoidance), but at the tradeoff of compromising some of the available season for active growth and biomass accrual. That's what we want to highlight and estimate. Can you select for a long-growing AND stress tolerant genotype???*

Predictions: 

[Kingsolver et al. 2015](http://www.jstor.org/stable/10.1086/681083)       

![](https://cloud.githubusercontent.com/assets/4654474/17571995/8eb6f062-5f20-11e6-9cf0-162845d307a8.png)

1. If we see A-B, no constraints among genotypes    
2. If we see C-D, constraints between low-high environmental axis   
3. If we see E-F, generalist-specialist axis of variation    

The cool thing here is that any of these possibilities can be captured by PC1, which explains the most variation. 

*It's cool that a PCA on the G-matrix can result in these qualitatively different scenarios. I'll need to read the Kingsolver paper and chat with you to see the underlying basis for these predictions.*

A different approach: [Template mode variation](http://www.ncbi.nlm.nih.gov/pubmed/16032579)

**Part 2. Correlate responses of genotypes to where they were found (source population)**    

We could fit functions to growth curves and then extract parameters. Plot parameters against source climate. This will get at the local adaptation part. 

*Yes! Also, we should think about these parameters as traits themselves, and potentially try and associate them with genomic data, either using genomic prediction (have a GWAS model that specifies causal SNPs, and then predict an ind's breeding value based on it's genotypes).

OR.... we could use transcriptomics to define "phenotypes" based on DEG's. Then look at the G-matrix of gene expression and analyze how expression as a set of function-valued traits shows tradeoffs across the environmental gradient. I think this would be super cool! Maybe couple that with some path analysis to connect DEGs with associated trait variation and how they covary with environment.*

Notes:        

1. **We can also couple a viability experiment in this project**     
2. Genomics part to develop: **Function valued traits are dynamic, are the same loci always involved?**, do QTL?        
3. I do want to add an additional 3 levels of moisture(or other important environmental parameter), but just kept the 9-12 common gardens for now. I do have ideas and resources for how to analyze the added factors [here](https://github.com/adnguyen/Dissertation_temperature_adaptation_ants/blob/master/General_Notebook.md#page-2-2016-05-13-comparing-g-matrices-of-different-populations).     

*I think a manipulative treatment would be interesting, but doubles (or triples) the replication level. We'll need to think through this carefully.*


<div id='id-section2'/>
## **Question 2:** Are there novel shifts in episodic selection regimes in poplar?     

**Hypothesis:** Human-induced climate change is altering selective regimes in natural populations. And can we predict future responses to climate change to determine genotypes that are resilient or susceptible? 

*So, is the hypothesis here that current selection in a given environment no longer reflects past selection to that environment? The former estimated from phenotypic selection gradients, and the latter from selection scans across the genome?*


**Approach:** Overlay and compare historical and contemporary selection regimes. Phenotype and collect samples out in the field and compare with common garden. When in the field, estimate historical selection. 

*got it. But I'm unsure about how you get historical selection from the field....*

Prediction:     
1. Selection could be targeting regions of the genome which have not experienced selection before.    
2. 

*John Kelly (Kansas) has a cool new method on how to estimate genomic regions experiencing contemporary selection --> integrates genome scans with Lande-Arnold type phen sel'n. We can get in touch with him for a pre-print, and I think he is working on software too....

<div id='id-section3'/>

# Broader Impacts    

```How well does the activity advance discovery and understanding while promoting teaching, training, and learning? How well does the proposed activity broaden the participation of underrepresented groups (e.g., gender, ethnicity, disability, geographic, etc.)? To what extent will it enhance the infrastructure for research and education, such as facilities, instrumentation, networks, and partnerships? Will the results be disseminated broadly to enhance scientific and technological understanding? What may be the benefits of the proposed activity to society?```

**Strategies:**     
1. Develop my own skills as a scientist by honing my skills in genomics     
2. As an under represented group, I will be able to attract other ethnicities to engage in research. I will mentor undergraduate researchers.     
3. Collaborate with local high schools to help me phenotype, take physiological measurements. Burlington high school has a large refugee community. Kids don't know you can be a scientist. 


*I like this idea a lot...we should develop it more, especially since it also works towards your goal of trying to take measurements in many different places. Kind of a citizen science angle.*

        
4. Construct shiny app so that citizens can follow our science.  

*This could be interesting. Maybe combine this with (4) so that students could have a way of following your project, and how you're integrating and using their observations to address your hypotheses.*

5. If we do proteomics, utilize the proteomics facility at UVM 

*Probably not considered by NSF as a broader impact*

<div id='id-section4'/>    

# Intellectual Merit  

```How important is the proposed activity to advancing knowledge and understanding within its own field or across different fields? How well qualified is the proposer (individual or team) to conduct the project? (If appropriate, the reviewer will comment on the quality of the prior work.) To what extent does the proposed activity suggest and explore creative, original, or potentially transformative concepts? How well conceived and organized is the proposed activity? Is there sufficient access to resources?```  

**Strategies:**    
1. I will utilize evolutionary theory to understand basic principles about what limits organisms to persist; these findings will extend to large-scale production of woody biomass   

*suggest: ...about what limits adaptation to changing environments when the genetic architecture of adaptation involves integration of multiple funciton-valued traits, and pleiotropy constrains selection through tradeoffs.*

2. This work will help us understand the determinants of resiliency or susceptibility *of ...* to human-induced environmental change.   

<div id='id-section5'/>
## Timeline
|Task                       |2017 |2018 |2019 |2020 |
|:-----------------------|:-----|:-----|:-----|:-----|
|Common Garden/field     |x     |x     |x     |x     |
|Phenotyping             |      |x     |x     |x     |
|Genomic Analyses        |      |x     |x     |x     |
|Attending Conferences   |      |      |x     |x     |
|Writing for publication |      |      |x     |x     |
|Public Outreach         |      |x     |x     |x     |

