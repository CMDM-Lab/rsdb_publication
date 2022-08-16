# rsdb_publication
## Introduction
This repository is the disease page of RSDB to display Cutis marmorata telangiectatica congenita (CMTC) for the source code for the network (starts from line 530) in the CMTC.html and the network json file in the 130.json file. 

## Prerequisite
1. Install Docker

## Steps to draw the network
1. `git@github.com:CMDM-Lab/rsdb_publication.git` or [directly download](https://github.com/CMDM-Lab/rsdb_publication/archive/refs/heads/main.zip)
2. Unzip the archive file if directly downloading the file.
3. Open terminal and run `docker build . -t rsdb-publication-image` to build the docker image.
4. Run `docker run -p 7777:80 rsdb-publication-image` to start web server
3. Open http://localhost:7777/CMTC.html to see the network
4. Open the CMTC.html or 130.json in the src folder with a text editor to see the source code and the network file.

## More network file
For more network files, please go to RSDB website: https://rsdb.cmdm.tw. 
1. Use search or browse to the specific info page. For example, the Dermatofibrosarcoma protuberans *https://rsdb.cmdm.tw/diseases/140*
2. Replace the plural entities in the url with the singular form (diseases → disease, genes → gene, or chemicals → chemical) and add a file extension ".json" on the end of the url. The url will be *https://rsdb.cmdm.tw/disease/140.json*
3. Press enter to display the network file.
