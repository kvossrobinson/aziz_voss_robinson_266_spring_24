# aziz_voss_robinson_266_spring_24

Our code is divided into four sections:
1. Data Preparation
   - Run these scripts to generate the data required to create our models.
   - We have omitted the data files themselves from our GitHub due to size constraints.
2. Model Creation
   - There are folders for each baseline and experiment and a folder for helper files.
   - We have included example code for each experiment (the code used to create our most successful model in each category). We have omitted code used to combine results from multiple experiments, as this can be built from the code we have uploaded.
3. Model Results
   - There are folders here matching those in the model creation folder; these contain the results of each example model run.
   - We have omitted the model weight files from our GitHub due to size constraints.
   - The "generic eval" folder within each model folder contains evaluation for the model on SQuAD. Our final evaluation on movie domain-specific QA data, which is cited in our paper, sits within the main model folders.
4. Evaluation
   - The movie_qa_eval file in this folder evaluates the model the user provides it on movie domain-specific QA data.
   - The loss_pattern_analysis script facilitates prediction comparisons between two models that the user provides.
