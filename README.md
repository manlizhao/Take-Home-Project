# Take-Home-Project
Loan Repay Prediction 

Note: 
EDA is in EDA.ipynb, and the Nerual Network Model Training is in Model_training.ipynb.
- during EDA, the `bad_falg` column is renamed as `target`.

Summaries: 
- I inspected all the columns, and found out a lot of string data need to be cleaned through extraction or regular expression. Found out some predictive features like `purpose`, `home_ownership` and `annual_inc`, `mths_since_last_major_derog`, etc. But some have a lot of missing value like `mths_since_last_major_derog`.
- the `desc` column is used to generate sentence embedding features. Here, I chose a sentence transformer model (all-MiniLM-L6-v2). It maps sentences & paragraphs to a 384 dimensional dense vector space and can be used for tasks like clustering or semantic search. The model card link: https://huggingface.co/sentence-transformers/all-MiniLM-L6-v2
  

