# sustainability_cdp_project
# Companies and Cities Driving Together Towards a Sustainable World

## Summary
### Motivation: 
Sustainability is a theme that all of us should reflect about. It's all about the planet we live and the future we want. The best way to do it is take our conclusions based on data. The reference for this project is the Kaggle Competition [“CDP - Unlocking Climate Solutions City-Business Collaboration for a Sustainable Future”](https://www.kaggle.com/c/cdp-unlocking-climate-solutions/overview)  

#### The main findings are summarized in a blog post you can read [here](https://reol.medium.com/how-companies-and-cities-can-work-together-towards-a-sustainable-future-5719f4ef365)

### Codes for Insights from CDP Survey Data
#### 1. The Data

The data used in this project can be downloaded using the [Kaggle API](https://github.com/Kaggle/kaggle-api) and typing the command:  
kaggle competitions download -c cdp-unlocking-climate-solutions  

#### 2. The project

The project was developed in a Python Jupyter Notebook: [2.1 - rco - cdp_survey - final.ipynb](https://github.com/rejaneol/sustainability_cdp_project/blob/main/2.1%20-%20rco%20-%20cdp_survey%20-%20final.ipynb)  

The **packages** and versions are listed below:  
pandas==1.0.3  
numpy==1.18.1  
matplotlib==3.1.3  
seaborn==0.10.1  
scikit-learn==0.22  

This project follows **CRISP-DM** phases.  

![image info](./pictures/crispdm.png)

In the _Business Understanding_ phase, the structure of the questionnaires is grabed and saved as Excel files.

In the _Data Understanding_ phase, some research questions were set and answered:
1. Is there an increase in the survey engagement by country over the years? More cities? More organizations?
2. How about the engagement with the survey itself? Do the respondents answer all the questions?
3. Do cities collaborate with companies? And do companies collaborate with cities?
4. Do organizations engage their value chain?
5. Can we estimate the level of engagement?

In the _Modeling_ phase, we propose to evaluate the engagement with enviromental issues by measuring how much the organizations have filled the questionnaires. We wonder if the number of missing values in the responses could be a latent variable for engagement. The hypothesis is: the less missing responses, the more engaged the organization is. A classifier model was fitted and showed 91% accuracy.

The main findings were:
* There were more engagement from corporations to fill the survey over the years, but the number of cities decreased in some countries.
* The cities say they collaborate with companies, but the companies don't say so, and the collaboration with cities happen mainly by trading associations.
* The collaboration within the companies' value chain is stronger with their suppliers and customers.
* The level of engagement needed to classify an organization as leadership (and its inclusion in A-list) can be predicted by how much it responds the previous year questionnaire.

## Acknowledgments

Kaggle Competition [“CDP - Unlocking Climate Solutions City-Business Collaboration for a Sustainable Future”](https://www.kaggle.com/c/cdp-unlocking-climate-solutions/overview)

This project was developed as part of the requirements for Data Scientist Udacity Nanodegree. 


