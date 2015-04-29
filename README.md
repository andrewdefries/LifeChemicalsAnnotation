# LifeChemicalsAnnotation
Annotation of the Life Chemical stock compound library using several cheminformatic and full text mining approaches

This repository contains code and documentation to subset the Life Chemicals Stock compounds (http://www.lifechemicals.com/downloads/9353/9360) into custom collections.

![Subsetting the Life Chemicals library](https://github.com/andrewdefries/LifeChemicalsAnnotation/blob/master/LifeChemicalsBioactiveSubset.png)


Motivation
==========

Life Chemicals has a large collection of ~380,000 diverse small molecule compounds. The entire compeound library may be interrogated one-by-one by experimentation. This would require purchasing the whole stock, which is not a frugal option. Therefore, I have pre-assembled a number of custom collections for specific chemical genetics research subtypes. In addition, the user may assemble a custom collection based on custom filters on using a web application that will be described.

Procedural explanation
======================

Several lists, see table, are used to search for structurally similar molecules in the Life Chemicals stock. To learn more about the cheminformatics operations please see the folder R/ for executable code to perform various Tanimoto searches based on seed lists.

The following are several lists used to assemble subsets of the Life Chemicals stock:

Annotation | Seed txt | Seed SDF | Stock TXT | Stock SDF 
-----------|----------|----------|-----------|-----------
PubChem Bioassay Bioactives | TXT | SDF | TXT | SDF
Plant Growth Regulators | TXT | SDF | TXT | SDF
Agrochemicals | TXT | SDF | TXT | SDF
Pesticides | TXT | SDF | TXT | SDF
Herbicides | TXT | SDF | TXT | SDF

Theme | Seed txt | Seed SDF | Stock TXT | Stock SDF 
-----------|----------|----------|-----------|-----------
Author | TXT | SDF | TXT | SDF
PDF | TXT | SDF | TXT | SDF
Book  | TXT | SDF | TXT | SDF

Custom | Seed txt | Seed SDF | Stock TXT | Stock SDF 
-----------|----------|----------|-----------|-----------
Target library via Protein query
test with pyr/pyls

To provide a sample of chemical space the Life Chemicals library has been subset into themed collections based on a seed list containing compounds of interest. Feel free to browse these collections by using the following R Shiny web application.

![Shiny web app](https://github.com/andrewdefries/LifeChemicalsAnnotation/blob/master/LifeChemicalsAnnotationViewer.png)




