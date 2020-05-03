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

## Copyright
This dataset will be published under the Creative Commons Attribution-ShareAlike 4.0 License.
