# FakeNews
Group Fake News Project 

The project contains four Python notebooks:

DataPreparation.ipynb
DataAnalysis.ipynb
MachineLearning.ipynb
BBC_Data.ipynb

Notebooks were tested successfully on a Mac computer, in Colab environment and in Vertex AI Workbench environment. They are not expected to work properly on a Windows computer due to multiprocess library used. 16Gb of RAM should be enough to run the notebooks.

To work properly all the notebooks should be located in the same folder. It is assumed that main input files - news_sample.csv, 995,000_rows.csv and test.tsv are located in the same folder with the notebooks.

The following libraries are necessary for the notebooks to work properly: pandas, multiprocess, nltk, scikit-learn, matplotlib, selenium.

BBC_Data.ipynb should be executed first. It gets news articles from BBC website and stores them to CSV in work folder.

Then DataPreparation.ipynb should be executed, it preprocesses input files so that they can be used further for machine learning. This notebook is computationally heavy and creates about 8Gb of temporary files.

DataAnalysis.ipynb contains scripts gathering statistics on input files.

MachineLearning.ipynb contains all the machine learning models created for the assignment. It can be executed only after DataPreparation.ipynb is executed and temporary files are created.
