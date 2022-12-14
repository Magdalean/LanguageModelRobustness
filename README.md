# LanguageModelRobustness
This paper demonstrates a comparison between language models with varying degrees of privacy preservation in binary sentiment classification. 

The code for this project is divided into two segments. Note that for successful execution, the first cell of each note book must be run, followed by a runtime restart. 

(1)	IMDb_Custom_Data_Augmentation.ipynb 
	This is the notebook that is used to create the augmented test set. 
	In total, it was run 6 times:
-	With 3 varying percentages of words to swap (25, 35, and 45%). 
-	With the first 500 test set samples, and then next 500 test set samples. 


(2)	Robustness_Testing.ipynb 
	This is the notebook which is used to create the base language model for sentiment prediction, along with the 4 differentially private versions of this model. 
  The models are then all tested using the clean and augmented data sets referenced in notebook (1) which have been saved in the CustomAttack folder
