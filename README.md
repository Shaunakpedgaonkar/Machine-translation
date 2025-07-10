Project Overview
This dissertation investigates the performance of diverse Machine Translation (MT) models across both well-resourced (English-French) and under-resourced (Bulgarian-English) language pairs. The research provides a comprehensive assessment of their effectiveness using various evaluation metrics.





Research Questions
The study addresses the following interrelated research questions:


Performance Evaluation: How do machine translation models perform in translating between resource-rich and under-resourced language pairs? 


Challenges Identification: What specific challenges arise when translating under-resourced languages? 


Metrics Effectiveness: How effectively do evaluation metrics evaluate translation quality in the context of under-resourced languages? 

Research Objectives
To address the research questions, this study has four objectives:


Implement and Compare Machine Translation Models: Implement and compare the performance of MT models on resource-rich and under-resourced language pairs to identify their strengths and limitations in different linguistic contexts.


Assess the Effectiveness of Evaluation Metrics: Analyze how well evaluation metrics capture translation quality by examining semantic accuracy, fluency, and structural alignment.


Address Challenges in Handling Linguistic Complexity: Investigate how MT models handle unique linguistic challenges, such as grammar and syntax, in under-resourced language pairs, focusing on the accuracy and structure of translations.


Provide Insights for Future MT Development: Propose practical recommendations to improve MT models and evaluation metrics, particularly for better handling of under-resourced languages.

Models Examined
The research focuses on four distinct MT models:




Seq2Seq with Attention: Used as a baseline model, aiming to enhance translation quality by focusing on attentively selected parts of the input sequence.



BERT-based MarianMT (Opus-MT): A Transformer model optimized for specific translation tasks, performing well even with low-resource languages like Bulgarian due to pre-training on a wide variety of languages.



Customized LSTM-based Seq2Seq: Developed to test the boundaries of usual Seq2Seq structures and address challenges in traditional models by retaining information over longer texts.






NAS and MoE-Based Model: A state-of-the-art model that adapts the translation architecture on-the-fly, integrating Neural Architecture Search (NAS) and Mixture of Experts (MoE) to dynamically optimize translation accuracy and efficiency.




Evaluation Metrics
The performance of these models is assessed using various important measures of translation proficiency:






BLEU (Bilingual Evaluation Understudy): Measures the precision of n-grams in the candidate translation relative to the reference translation, with a penalty for shorter translations.






TER (Translation Edit Rate): Calculates the number of edits (insertions, deletions, substitutions, and shifts) required to change the system output into the reference translation.






ROUGE (Recall-Oriented Understudy for Gisting Evaluation): Predominantly used for summarization, it measures the overlap between candidate and reference translations, emphasizing recall.






CHRF (Character n-gram F-score): Calculates the F-score based on the precision and recall of character-level n-grams, useful for languages with rich morphology.





METEOR (Metric for Evaluation of Translation with Explicit ORdering): Improves BLEU by considering synonyms, stemming, and paraphrases.

Datasets
The study utilizes two primary datasets for training and evaluation:



English-French Dataset: Consists of over 300,000 parallel English and French sentence pairs, ideal for model training due to substantial linguistic differences and high-quality professional translations.




Europarl Bulgarian-English Dataset: Contains approximately 406,934 aligned sentence pairs from European Parliament proceedings, supporting machine translation tasks between these less-studied languages.


Preprocessing steps for both datasets include tokenization, padding and truncation, normalization, data augmentation (e.g., back-translation), and stopword removal .

Key Findings

MT Model Performance: The MarianMT pre-trained model generally outperformed custom MT models, highlighting the benefits of extensive pre-training on diverse multilingual datasets.



Evaluation Metrics: The study highlighted limitations of relying solely on BLEU scores, demonstrating that TER, ROUGE, and CHRF provided a more nuanced view of translation quality.


Challenges Faced
The project encountered several challenges:


Model Design and Development: Iterative design, evaluation, and redesign were often necessary to refine MT models.


Dataset Selection: Identifying large and diverse datasets for various language pairs was difficult.


Prolonged Training Periods: Training MT models is time-consuming, often requiring days or weeks, along with significant computational resources.


Repeated Trials and Error Handling: Multiple training cycles and continuous monitoring were common due to complexities in machine translation.

Future Work
Future work could explore the inclusion of more advanced metrics or hybrid evaluation approaches to fully capture all dimensions of translation quality. Further research is needed to optimize translation processes, ensuring MT tools not only translate accurately but also resonate culturally and contextually with all users.
