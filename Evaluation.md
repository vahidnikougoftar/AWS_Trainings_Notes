Model Evaluation for RAG and Fine-Tuning have different methodolgies:

* RAG has two common methodologies: <b>Human Evaluation</b> and <b>Benchmark Datasets</b>
1. Human Evaluation: Mainly for qualitative performance (i.e. User Experience, Contextual appropriateness, Creativity and flexibility)
2. Benchmark Datasets : Mainly for quantitative etrics using standard question/answer datasets (metrics such as Accuracy, speed and effieciency and scalability)

* Fine-Tuning has 3 common methodologies
1. ROGUE (Recall-Oriented Understudy for Gisting Evaluation) : The main idea behind ROUGE is to count the number of overlapping units. This includes words, N-grams, or sentence fragments between the computer-generated output and a set of reference (human-created) texts.
   1.1. ROUGE-N: This metric measures the overlap of n-grams between the generated text and the reference text. For example, ROUGE-1 refers to the overlap of unigrams, ROUGE-2 refers to bigrams, and so on. This metric primarily assesses the fluency of the text and the extent to which it includes key ideas from the reference.
   1.2. ROUGE-L: This metric uses the longest common subsequence between the generated text and the reference texts. It is particularly good at evaluating the coherence and order of the narrative in the outputs.
   
2. BLEU (Bilingual Evaluation Understudy) : Quality of translation from one natural language to another, by measuring the precision of N-grams in the machine-generated translation that appears in the reference texts and applies a penalty for overly short translations.
3. BERTScore : Because BERTScore evaluates the semantic similarity rather than relying on exact lexical matches, it is capable of capturing meaning in a more nuanced manner. BERTScore is less prone to some of the pitfalls of BLEU and ROUGE. An example of this is their sensitivity to minor paraphrasing or synonym usage that does not affect the overall meaning conveyed by the text.
BERTScore is increasingly used alongside traditional metrics like BLEU and ROUGE for a more comprehensive assessment of language generation models. This is especially true in cases where capturing the deeper semantic meaning of the text is important. 
