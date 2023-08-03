# ProcessMining-Loans

Fake update for web tests

 Loans use case from BPI 2017

This data set comes from BPI challenge 2017 https://www.win.tue.nl/bpi/doku.php?id=2017:challenge You are invited to read the articles from the contesters, that relate their approach and their findings.

The Loan process is made out events coming from 3 origins:
- Application: started by the applicant who requests a Loan
- Workflow: a BPM system that drives the human activities requested
- Offer: started when one or several offers are created
We can't consider the end-to-end process as a multi-level process as these 3 origins are interlaced.

The original data set [BPI Challenge 2017.xes.gz](https://github.com/Patrick-Megard/ProcessMining-Loans/Datasets/BPI Challenge 2017.xes.gz) needs to be transformed to remove some errors and to make some changes.

We are using this Jupyter Note book [Loans/ipynb](Loans/ipynb) to transform the original data set and to create a series of new datasets.

At the end of the transformation, we obtain 4 datasets that are can be loaded in IBM Process Mining:
- [Loan_all_events.csv.zip](Loan_all_events.csv.zip) includes events from the 3 origins above.
- [Loan_Application_events.csv.zip](Loan_Application_events.csv.zip) focuses on the Application process.
- [Loan_Workflow_events.csv.zip](Loan_Workflow_events.csv.zip) focuses on the Worfklow process.
- [Loan_Application_events.csv.zip](Loan_Application_events.csv.zip) focuses on the Offer process.
