# Artificial intelligence text generators: fairytales

In this folder PIAT models of LSTM and Transformer are presented.

*LSTM.ipynb* and *Transformer.ipynb* notebooks contain the code itself, links and the process of reasoning leading to subsequent trials.

*LSTM - attempts description.docx* and *Transformer - attempts description.docs* documents describe shortly the dataset, model, parameters used for each attempt made and present sample results.

**LSTM models** were trained on 5 different datasets (from 1.5 MB to 30 MB) - Polish fairytales, stories and novels, with punctuation excluded or included, using two different sample creation approaches, basically choosing simple or advanced model, sometimes including samples normalization, with batch equal to 32 or 512. As a result, 17 LSTM models were created.

**Transformer models** were trained on 4 different datasets (from 2.3 MB to 30 MB) - Polish fairytales, stories and novels, with batch size equal to 8, embedding dimension equal to 32, 4 or 8 heads and adjusted Adam learning rate. Models had usually the restricted number of words set. The samples length was chosen according to the dataset sentences length, based on quantiles values.  As a result, 17 Tranformer models were created, and even more were tried to run, but often resulted in the exhaustion of available computer resources.

The best models (in my opinion) have been uploaded to OneDrive:
- LSTM (attempt 10, first model):
  https://tulodz-my.sharepoint.com/:u:/g/personal/244815_edu_p_lodz_pl/EYQJCo71wYhFh_ZzoFIpc44BBZtsdLlRBDNXY2mJmwBHLw?e=fAMLaA
- Transformer (the last attempt made):
  https://tulodz-my.sharepoint.com/:u:/g/personal/244815_edu_p_lodz_pl/ESiTKg5O305GnF5lD5vJKfcBSNzOqjeXih2ufIA3VBGq9A?e=phWQLS

The small text dataset that has given promising results was collected manually and is included in the *Dataset.zip* file.

The environmental packages and their versions used are listed in *requirements.txt* file.
