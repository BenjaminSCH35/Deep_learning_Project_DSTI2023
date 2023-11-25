# Deep_learning_Project_DSTI2023


The main idea of the project was to build a Pipeline to fine tune a Bert Model with a lot of different Hyperparameter.
The training loop can be adapted to a lot of different model. 

To reproduce the experiments, just follow the notebook in google colab :

step 1 : import library and set global var (cells 1 and 2)

step 2 : run the necessary functions (cell 3)

step 3 : mount your drive and run the code to get your dir ready for (Data, Model result) (cell 4)

step 4 : CSV to DataLoader - split to train 80% / validation 10% of train / test 20% (cell 4)

step 5 : Set pytorch lightning module ToxicCommentTagger  (Cell 5)

step 6 : Run the training loop for desired hyperparameters - This loop allow to save 3 best checkpoints and models metrics to your drive (Cell 6)

step 7 : Run the test loop with three best models to see which model perform better

step 8 : Re train your best model for more epochs to see if you can improve.



The metric we use to select best model is the AUCROC averaged. Which is simply the average of the individual AUCROC for each label (Multilabel classification)

