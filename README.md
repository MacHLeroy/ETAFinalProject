# ETAFinalProject
Code and Data for Final project for Exploratory Text Analytics

This Github Repo contains all the code and data I used to complete my final project for Exploratory Text Analytics. In this project, I explore the top 10 most popular novels (as measured by number of downloads on Project Gutenberg) of Jules Verne and H.G. Wells. Wells and Verne are referred to as the "Godfathers of Science Fiction," so this porject attempts to understand both the commonalities and differences in the way each wrote. 

## Code/Notebooks

* BookDownloader.Rmd - R Markdown file that pulls the Gutenberg numbers associated with each text in FinalSetVerneAndWells.csv and uses the gutenbergr package to downlaod and eport exports each book in .txt form to HGWellsAndVerne

* FP_1_TOKENIZE.ipynb: Notebook used to read in the 20 source texts from directory HGWellsAndVerne and tokenize each one. 
  * Outputs: wells-verne-LIB.csv, wells-verne-CORPUS.csv, wells-verne-VOCAB.csv
* FP_2_TFIDF.ipynb: Notebook used to find TFIDF of Vocab and explore patterns in Corpus
  * Outputs: wells-verne-CORPUS2.csv, wells-verne-VOCAB2.csv, wells-verne-BOW.csv, wells-verne-DTCM.csv, wells-verne-TFIDF.csv, wells-verne-SIGS.csv, wells-verne-TFIDF_REDUCED.csv
* FP_3_CLUSTERING.ipynb: Notebook that uses a range of methods to cluster documents in the corpus
  * Outputs: wells-verne-BOW_REDUCED.csv
* FP_4_PCA.ipynb: Notebook that uses TFIDF data to perform Principal Component Analysis on the Corpus
  * Outputs: wells-verne-LIB2.csv, wells-verne-PCA_COMPS.csv, wells-verne-PCA_COMPS.csv, wells-verne-PCA_THETA.csv, wells-verne-PCA_DCM.csv
* FP_5_TM1.ipynb: Notebook used to creat a and explore topic model for the entire corpus
  * Outputs: wells-verne-LDA_PHI-20.csv, wells-verne-LDA_THETA-20.csv, wells-verne-LDA_TOPIC-20.csv
* FP_6_TM2.ipynb: Notebook used to create and explore topic models created for each individual author
  * Outputs: WELLS-LDA_PHI-20.csv, WELLS-LDA_THETA-20.csv, WELLS-LDA_TOPIC-20.csv, VERNE-LDA_PHI-20.csv, VERNE-LDA_THETA-20.csv, VERNE-LDA_TOPIC-20.csv 
* FP_7_WE_1.ipynb: Notebook used to creat a and explore a word embedding model for the entire corpus
  * Outputs: wells-verne-W2V.csv, wells-verne-GENSIM_DOCS.csv
* FP_8_WE_2.ipynb: Notebook used to create and explore word embedding models created for each individual author
  * Outputs: WELLS-W2V.csv, WELLS-VOCAB.csv, WELLS-GENSIM_DOCS.csv, VERNE-W2V.csv, VERNE-VOCAB.csv, VERNE-GENSIM_DOCS.csv
* FP_9_SA.ipynb: Notebook used to perform sentiment analysis on a variety of documents on the corpus
  * Outputs: 

## Data

GitHub can be a tricky place to host data. I have pushed all created data to this repo, but recommend you pull the code on this repo and run in order to recreate the data locally. This is the best way to ensure that none is lost in the mix. You can also pull my data from INSERT BOX LINK. 

* HGWellsAndVerne: Source Text for the 20 (10 for Wells and 10 for Verne) books that comprise the Corpus. Books were downloaded using BookDownloader.Rmd, then books some had to be manually edited to make formatting work (change title names etc.) 
* outout: all the output created by the notebooks above. See DataDictionary file in output for more information on individual files

## Final Report

The final report can be found in XXX
