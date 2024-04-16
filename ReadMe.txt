This is an anonymous REPO for the paper:
"Patent Drafting with Large Language Models"

** Code and environment Set-up for each method:
- For GPT-2 we used transformers from huggingface github repository. 
- For GPT-3.5 we used OpenAI api for the generation.
- For Llama2 we used langchain and huggingface

** Data Processing:
- All the data has been downloaded from patentsview.org
- We processed g_patent.tsv, g_claims_2022.tsv, g_cpc_current.tsv to get our desired data
- All the processed data has the following information as columns:
 ptent_id, patent_abstract, patent_title, claim_text, cpc_subclass
** Generating Abstracts: 
- For generating the abstracts GPT2.ipynb, GPT3.5.ipynb and Llama2.ipynb have been used.
- Different data (csv files) has been used to generate the abstracts and stored in a new csv file for each subclass
- Claim1 was provided as input, and abstract was the generated output
** Generating Claims:
- For generating the claim GPT2.ipynb, GPT3.5.ipynb and Llama2.ipynb have been used.
- Different data (csv files) has been used to generate the abstracts and stored in a new csv file for each subclass
- Abstract was provided as input, and calim1 was the generated output
** Evaluation: 
- To calculate BERTScores, we utilized the BERTScore package
- We used the nltk package to compute the BLEU 
- Rouge package has been used for  calculating Rouge scores 
- For cosine calculations, we employed the 'cosine_similarity' function provided by the scikit-learn package
** Task:
- Classification has been done using pre trained BERT model
- For ranking we used BERT embedding and jaccard coefficient
Note: all the requirements installation command has been provided in each of the ipynb file





