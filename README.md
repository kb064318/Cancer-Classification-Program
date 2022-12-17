# Cancer Classification Program
Classifies patients in an excel sheet as having or not having cancer based on which gene mutations they have.

This program utilizes the random forest classification technique. Each tree in the forest is created by sorting genes by Phi value. The random forest is depth 3, meaning each tree uses the top gene based on Phi value to classify the patient, then repeats this process on the resulting tables until a tree depth of 3 is reached. At the end of the program, statistics are displayed showing the effectiveness of the forest.

The excel sheet used is not included in this repo, as I do not have permission to share it. To give a general overview of its layout, the rows are labeled using patient tags, and the column are labeled using the names of each gene mutation. If an excel cell contains a 1, the patient at the row the cell is in has the gene mutation at the column the cell is in. If it contains a 0, the patient does not have the gene mutation.
