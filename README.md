## Notice
This is a copied and edited README from the starter repository provided by Manning.

## Project: Natural Language Processing (NLP) of Job Postings Data
Repository contains an implementation of the Manning liveProject [Decoding Data Science Job Postings to Improve Your Resume](https://www.manning.com/liveproject/decoding-data-science-job-postings-to-improve-your-resume). To restate the title more elaborately, the main goal is to glean insights of the data science job market (also with respect to the resume of a given individual or job seeker); then job seekers could use these insights to improve their chances of success, by helping them prioritize which skill sets to develop and what to include on their resumes.

An overview of the project's objectives:
- extracting job postings dataset from web scraped HTML
- processing data with Pandas; NLP and machine learning with Scikit-learn
- TF-IDF vectorization of all the text documents (a user's resume and job postings)
- ranking similarity of a user’s resume document with entries in the job postings dataset
- k-means clustering of the job postings dataset (a subset of it): allowing the analysis of different types of job requirements
- visualizing contents of the clusters, that is, most frequent words: to represent desired skills from employers 
- ranking similarity of a user’s resume to a cluster

The two main techniques used in the analysis are cosine similarity comparisons and a k-means clustering. Conversely, the techniques used in this project can be used from the perspective of a hiring manager or so forth, who is looking to filter job applicants down to a workable level or to group them based on similarity to other applicants for a better idea of the available talent pool. 

The repository's owner was provided the job postings sample data by Manning, with no knowledge of its collection. So no assumptions were made about how well it represents its population: that was not part of the project. That being said the purpose of this project is educational more than practical so from the project's perspective it's being assumed that the data was properly sampled.

## Instructions

### 1. Setup
Project runs on Python 3.7, and it's recommend to use the [Anaconda Python Distribution](https://www.anaconda.com/distribution/#download-section). Once you have Anaconda installed, you can run `conda env create -f environment.yml` to create a conda environment called `job-posting-nlp`. Then you can activate the environment with `conda activate job-posting-nlp`, and deactivate the environment with `conda deactivate`. Once you have activated the environment, you can run jupyter notebooks from within that terminal window with `jupyter notebook`.

### 2. Data
`data` contains what is necessary to run the Jupyter notebooks as instructed in the Code section below; however `data/html_jop_postings.zip` needs to be unzipped beforehand. 

### 3. Code
Jupyter notebooks are meant to be run in the order indicated by their file name prefix, 1-4. Comments in the code mostly serve to state explicitly the general flow of tasks; but they are also used to self-document some of the methods and reflections of the analysis. Each notebook's objective is stated at the top of the file.
