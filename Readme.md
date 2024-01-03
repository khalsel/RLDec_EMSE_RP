# Artifacts Package
This git repository includes all the code and data to validate the results of our paper titled "Extracting Microservices from Monolithic Systems using Deep Reinforcement Learning” which has been submitted the Empirical Software Engineering journal.

The repository provides :
* The detailed results achieved by our proposed approach and the baselines we compare with including the decomposition that they generated.
* The code used to generate the figures and tables in the paper and analyze the results.
* The figures showcased in the paper.
* A graph visualization of the examples analyzed in Research Question 3.
* names and ids of PetClinic-microservices' classes.
* The hyperparameters used for training the model

Description of the structure of the repository:
* data:
  * mono: The results for the monolithic applications for each decomposition approach (RQ1 and RQ2)
    * approach_name/app_name/results.csv: the evaluation metrics results
    * approach_name/app_name/decompositions.csv: the generated decompositions
  * micro: The results for the microservices applications (RQ3)
  * topicdecomp_decompositions: the decompositions generated by the baseline TopicDecomp for the application PetClinic-Microservices.
* figures: List of figures used in the paper
  * petclinic-microservices_rldec_micro.html: Interactive Graph visualization of the decomposition of RLDec discussed in RQ3 (created using pyviz)
  * petclinic-microservices_true_micro.html: Interactive Graph visualization of the actual architecture of PetClinic (created using pyviz)
  * petclinic-microservices_topicdecomp_micro.html: Interactive Graph visualization of the decomposition of TopicDecomp discussed in RQ3 (created using pyviz)
* analyze_results.ipynb: The notebook used with the code used to create the figures
* class_index_petclinic_microservices.json: the list of classes in PetClinic-microservices with the corresponding ids used in the paper 
* train_config.json: The hyperparameters used for training the model.

