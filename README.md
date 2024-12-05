# CS440_Final
This respository is for Johnathon VanAken's CS440 Final attempt to improve upon the NLBSE25 base model for code comment classification 

This project uses SciKit Learn Pipelines to create a tokenizer and custom Nerual Network which classifies a code comment sentence into one of the following categories. The goal of this code is to create a lightweight model which requires minimal compute while still achieving modest performance metrics.

java: [summary, Ownership, Expand, usage, Pointer, deprecation, rational],
python: [Usage, Parameters, DevelopmentNotes, Expand, Summary],
pharo: [Keyimplementationpoints, Example, Responsibilities, Classreferences, Intent, Keymessages, Collaborators]

The notebook converts the imported labels into a single integer for classification for each language where:
Java                       Python                      Pharo
summary = 0                Usage = 0                   Keyimplementationpoins = 0
Ownership =1               Parameters = 1              Example = 1
Expand = 2                 Developments = 2            Responsibilities = 2
usage = 3                  Expand = 3                  Classreference = 3
Pointer = 4                Summary = 4                 Intent = 4
deprecation = 5                                        Keymessages = 5
rational = 6                                           Collaboraors = 6

The neural network architecture 
