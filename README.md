# Contradictory, My Dear Watson

# Description
"…when you have eliminated the impossible, whatever remains, however improbable, must be the truth"

Sir Arthur Conan Doyle

Our brains process the meaning of a sentence like this rather quickly. We're able to surmise:
- Some things to be true: "You can find the right answer through the process of elimination.”
- Others that may have truth: "Ideas that are improbable are not impossible!"
- And some claims are clearly contradictory: "Things that you have ruled out as impossible are where the truth lies."

# The challenge
If you have two sentences, there are three ways they could be related: one could entail the other, one could contradict the other, or they could be unrelated. Natural Language Inferencing (NLI) is a popular NLP problem that involves determining how pairs of sentences (consisting of a premise and a hypothesis) are related.

Your task is to create an NLI model that assigns labels of 0, 1, or 2 (corresponding to entailment, neutral, and contradiction) to pairs of premises and hypotheses. To make things more interesting, the train and test set include text in fifteen different languages!

Today, the most common approaches to NLI problems include using embeddings and transformers like BERT. In this competition, we’re providing a starter notebook to try your hand at this problem using the power of Tensor Processing Units (TPUs). TPUs are powerful hardware accelerators specialized in deep learning tasks, including Natural Language Processing. Kaggle provides all users TPU Quota at no cost, which you can use to explore this competition.

# Evaluation
Goal:
Your goal is to predict whether a given hypothesis is related to its premise by contradiction, entailment, or whether neither of those is true (neutral). For each sample in the test set, you must predict a 0, 1, or 2 value for the variable. Those values map to the logical condition as:
- 0 == entailment
- 1 == neutral
- 2 == contradiction

Metric:
Your score is the percentage of relationships you correctly predict. This is known as accuracy.
