Modelling an Islandora Newspaper Solution Pack
This repo contains a discussion document, content models, drush scripts, 
sample data and objects.

GenericNewspaperSP.pdf
- discussion document 

content_models
- islandora_newspaperCModel.xml
-- a content model that describes the newspaper itself
- islandora_issueCModel.xml
-- a content model that describes a newspaper issue
- islandora_pageCModel.xml
-- a content model that describes a newspaper page

drush_scripts
- drush_script_README.txt
-- describes how to use the drush scripts
- islandora_newspapers.drush.inc
-- script used to read a csv file and pull from a directory of associated TIFF files
- islandora_newspapers_check.drush.inc
-- script used to verify objects processed by the islandora_newspapers.drush.inc

sample_drush_data
- 19010812-19011101.csv
-- metadata file
- 19010812-19011101.zip
-- zip of TIFF files

sample_objects
These are complete FOXML objects with their associated binaries
- guardian_19200412-001.xml
-- a newspaper page object
- guardian_19200412.xml
-- a newspaper issue object
- newspapers_guardian.xml
-- a newspaper object

forms
- newspaper_form.xml
-- is an islandora xml formbuilder form that can be used to create MODS that describes a newspaper.
The form would be associated with the islandora:newspaperCModel content model.