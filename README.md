# CS440_Final
This respository is for Johnathon VanAken's CS440 Final attempt to improve upon the NLBSE25 base model for code comment classification 

This project uses SciKit Learn Pipelines to create a tokenizer and custom Nerual Network which classifies a code comment sentence into one of the following categories. The goal of this code is to create a lightweight model which requires minimal compute while still achieving modest performance metrics.

To run the notebok ensure the corresponding Scikit Learn and pandas dependencies are installed using the below command should install all dependencies.
pip install scikit-learn
pip install pandas

Once installed run the NLBSE25 Dense Network.ipynb file

java: [summary, Ownership, Expand, usage, Pointer, deprecation, rational],
python: [Usage, Parameters, DevelopmentNotes, Expand, Summary],
pharo: [Keyimplementationpoints, Example, Responsibilities, Classreferences, Intent, Keymessages, Collaborators]

The notebook converts the imported labels into a single integer for classification for each language where:

Java: summary = 0, Ownership =1, Expand = 2, usage = 3, Pointer = 4, deprecation = 5, rational = 6               
Python: Usage = 0, Parameters = 1, Developments = 2, Expand = 3, Summary = 4      
Pharo: Keyimplementationpoins = 0, Example = 1, Responsibilities = 2, Classreference = 3, Intent = 4, Keymessages = 5, Collaboraors = 6

The neural network architecture consists of multiple hidden dense layers for classification.

Overall the model scores a 0.5 using the NLBSE25 score calculation which is a 29% decrease in performance. However, the dense model outperforms the NLBSE model by 99.99% and 62% when comparing GFLOPs and runtime respectively.
