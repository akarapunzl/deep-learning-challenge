*Overview of the analysis:*
The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. I used my knowledge of machine learning and neural networks to create a binary classifier that can predict wheather applicants will be successful if funded by Alaphabet Soup.

*Data Preprocessing*

*Targets*
- The target for both models was "Is Successful" as the desired outcome was to know if the applicants would be successful.
  
*Features*
- For both models, APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, and ASK_AMT were used as features

*Niether Targets nor Features*
- For both models, removed EIN and NAME as these did not affect the preformance of the applicants and are just identifiers.

*Compiling, Training, and Evaluating the Model*

*How many neurons, layers, and activation functions did you select for your neural network model, and why?*
For model 1, I tried two deep layers with 80 and 30 units.
For model 2, I tried three deep layers with 12, 6, and 1 units
For model 3, I tried three deep layers with 80, 30, and 15 units.

*Were you able to achieve the target model performance?*
I was unable to achieve the target model performance. I got to a 72.5% accuracy. 

*What steps did you take in your attempts to increase model performance?*
For model 2, I tried adding more Classifications back into the table, by filtering out the ones with less than 100 vs 1000. And then I tried smaller units for my layers. For model 3, I tried adding a third layer with higher units. Each time I ran it with 100 EPOCHs. Each was an attempt to see if more or less data would help the prediction run more accurately. 

*Summary:*
Overall, I was unable to achieve the 75% accuracy. The model ended up being 72.5% accurate at its peak performance. To potentially get better results, I would potentially try to use KerasTuner to optomize further and get a higher accuracy. 
