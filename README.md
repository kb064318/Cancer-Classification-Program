# Cancer Classification Program
Classifies patients in an excel sheet as having or not having cancer based on which gene mutations they have using supervised learning.

This program utilizes the random forest classification technique. Each tree in the forest is created by sorting genes by Phi value. The random forest is depth 3, meaning each tree uses the top gene based on Phi value to classify the patient, then repeats this process on the resulting tables until a tree depth of 3 is reached. At the end of the program, statistics are displayed showing the effectiveness of the forest.

The excel sheet used is not included in this repo, as I do not have permission to share it. To give a general overview of its layout, the rows are labeled using patient tags, and the column are labeled using the names of each gene mutation. If an excel cell contains a 1, the patient at the row the cell is in has the gene mutation at the column the cell is in. If it contains a 0, the patient does not have the gene mutation.

## Evaluator sample results
Accuracy:  0.6705882352941176<br>
Sensitivity:  0.5263157894736842<br>
Specificity:  0.7872340425531915<br>
Precision:  0.6666666666666666<br>
Miss Rate:  0.47368421052631576<br>
False Discovery Rate:  0.3333333333333333<br>
False Omission Rate:  0.32727272727272727<br>
TP:  20<br>
TN:  37<br>
FP:  10<br>
FN:  18<br>

![newplot](https://user-images.githubusercontent.com/54725373/208223010-90f23ae0-595f-437a-bf5e-9772f959a4f1.png)
