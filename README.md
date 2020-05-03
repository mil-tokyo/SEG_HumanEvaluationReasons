# SEG_HumanEvaluationReasons

This is the appendix file of "Toward a Better Story End: Collecting Human Evaluation with Reasons" by Yusuke Mori, Hiroaki Yamane, Yusuke Mukuta and Tatsuya Harada (INLG 2019).

## Contents
It includes the following item.
    
- "qualitative_evaluation_results.csv":
    - The details of the columns are as below:
        - InputStoryid : The story id from Story Cloze Test test set.
        - context : Given four sentences, where the last sentence is excluded from a story comprising five sentences.
        - Option A : One of the two options to complement the missing 5th sentence. 
        - Option B : The other option to complement the missing 5th sentence. 
        - answer : The chosen option by an annotator.
        - reason : The reason why the annotator chose the answer.
        - RightEnding : The human-written ending (ground truth). This matches either A or B.
        - model1 : It indicates which A or B is the generated ending by H-Seq2seq.
        - answer_correspondence : It indicates the "answer" above is corresponding to which of "Human", "Generated", "Both" or "Neither".

## Correction of the Paper
There was a bug in the code that aggregated the data, and some numbers were wrong. This does not affect the assertion of the paper.

In Table 2 in the paper, the values below are incorrect.

| H-Seq2seq | Human  | both | neither |
| -------- | --- | ---- | ------- |
| 3         |180     |16      |1         |

The correct numbers are:

| H-Seq2seq | Human  | both | neither |
| -------- | --- | ---- | ------- |
| 4         |179     |16      |1         |

In the Discussion section, we wrote 
```
However, 20 stories were evaluated to be equal to or better than an ending written by humans.
```
and it should be
```
However, 21 stories were evaluated to be equal to or better than an ending written by humans.
```

## Copyright
This dataset will be published under the Creative Commons Attribution-ShareAlike 4.0 License.
