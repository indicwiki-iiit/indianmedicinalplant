# Indian Medicinal Plants - HindiWiki

This repository contains all the work that was done as a part of enriching hiWiki wikipedia in the Indian Medicinal Plants domain.

## Stages of the project

The following ordered list will give an idea as to what stage the project currently is in:

- [x] Scrape Data from Web sources - Wikipedia, Wikidata, indiabiodiversity.org , flowersofindia.net & iucnredlist.org
- [x] Clean and Format the data
- [x] Translate and Transliterate the data to Hindi
- [x] Scrape image names from Wiki commons
- [x] Create a sample article
- [x] Review of the sample article
- [x] Work on feedback from review of sample article
- [x] Review of the dataset
- [x] Create template for article generation and get it reviewed
- [x] Work on feedback from review of template
- [x] Create XML dump for 50 articles and get it review
- [x] Create the XML dump for all the plants to be published

## Folders

- `Datasets`: Contains the dataset files that have been used for this project.
- `Code`: Contains all the code that has been used in the project.
- `Template`: Contains the jinja template for the XML generation of a plant article.
- `XML Dump`: Contains XML dumps rendered through code,which is uploaded to Sandbox.

### Datasets

This folder contains the final dataset as well as some other dataset that have been used in the project:
- [wikiplant_final.xlsx](./Datasets/wikiplant_final.xlsx) : This is the master datasheet used to generate XML dump.

### Code

This folder contains various files:

- [get_plant_urls](.Code/scrap/get_plant_urls.ipynb) : For generating Website (indiabiodiversity) URLs manually
- [wikipage_scraping_selenium](.Code/scrap/wikipage_scraping_selenium.ipynb) : Scrape main web source 
- [Flowers_india_id_scraping](.Code/scrap/Flowers_india_id_scraping.ipynb) : Scrape Features from flowersofindia.net
- [IUCN_Scrapping](.Code/scrap/IUCN_Scrapping.ipynb) : Scrape Features from iucnredlist.org
- [Wikiplant_features](.Code/scrap/Wikiplant_features.ipynb) : Data Cleaning & Creating New features from existing ones.
- [plant_wiki_intro_scrapping](.Code/scrap/plant_wiki_intro_scrapping.ipynb) : Scrape English Wikipedia introduction section
- [Article XML Generation](.Code/Article XML Generation.ipynb) : XML Generation and Render Code
- [Translate_Transliterate](.Code/Wikiplant_translate.ipynb) : Translate & Transliterate Code



### Template

- [template](./Template/wikiplant_template.j2): it contains the jinja template for the structure of a Medicinal plant article

## XML Dump

- [XML Dump](./XML Dump/wikiplant_hindi_50.XML): XML Dump of first 50 articles.
- [XML Dump](./XML Dump/wikiplant_hindi.XML): Full XML Dump of all articles.
