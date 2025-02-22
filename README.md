# Awesome LLM Mechanism Analysis

![PRs Welcome](https://img.shields.io/badge/PRs-Welcome-green) 

Accompanied repositories for our paper [A Survey to Recent Progress Towards Understanding In-Context Learning](https://arxiv.org/abs/2402.02212). This paper list is still incomplete. feel free to add any relevant papers! PRs are welcome 🙌📚 Thanks!

- <a href="#skill-recognition"> Skill Recognition
- <a href="#skill-learning"> Skill Learning
- <a href="#skill-recognition-learning"> Skill Recognition & Skill Learning
- <a href="#skill-composition"> Skill Composition (Reasoning)
- <a href="#Knowledge"> Knowledge
- <a href="#Mechanism Analysis"> Mechanism Analysis
- <a href="#origin"> The origin of ICL ability
- <a href="#probe"> Probing Analysis
- <a href="#correction"> Self Correction
- <a href="#empirical"> More empirical studies





<div id="skill-recognition"></div>

## Skill Recognition
The skill recognition ability selects one data generation function from the learned function class during pre-training

- (**ICLR'21**)[Empirical] An Explanation of In-context Learning as Implicit Bayesian Inference  [[Paper](https://arxiv.org/abs/2111.02080)]
- (**NeurIPS'23**)[Empirical & Theoretical] Large Language Models Are Latent Variable Models: Explaining and Finding Good Demonstrations for In-Context Learning[[Paper]](https://arxiv.org/abs/2301.11916)
- (**ICLR'24**)[Empirical] Function vectors in large language models[[Paper]](https://arxiv.org/abs/2310.15213)
- (**Arxiv'24**)[Empirical] In-context Vectors: Making In Context Learning More Effective and Controllable Through Latent Space Steering[[Paper]](https://arxiv.org/abs/2311.06668)
- (**Arxiv'23**)[Theoretical] What and How does In-Context Learning Learn? Bayesian Model Averaging, Parameterization, and Generalization[[Paper]](https://arxiv.org/abs/2305.19420)
- (**Arxiv'23**)[Theoretical] The learnability of in-context learning[[Paper]](https://arxiv.org/abs/2303.07895)
- (**Arxiv'23**)[Theoretical] In-Context Exemplars as Clues to Retrieving from Large Associative Memory[[Paper]](https://arxiv.org/abs/2311.03498)
- (**Arxiv'24**)[Theoretical] An Information-Theoretic Analysis of In-Context Learning[[Paper]](https://arxiv.org/abs/2401.15530)


<div id="skill-learning"></div>

## Skill Learning
The skill learning ability learns a new data generation function in context.

### Function Approximatation and Generalization


- (**NeurIPS'23**)[Empirical] Pretraining task diversity and the emergence of non-Bayesian in-context learning for regression[[Paper]](https://arxiv.org/abs/2306.15063)
- (**ICLR'24**)[Theoretical] How Many Pretraining Tasks Are Needed for In-Context Learning of Linear Regression? [[Paper]](https://arxiv.org/abs/2310.08391)
- (**NeurIPS'22**)[Empirical] What Can Transformers Learn In-Context? A Case Study of Simple Function Classes[[Paper]](https://arxiv.org/abs/2208.01066)
- (**NeurIPS'23**)[Theoretical] Transformers as Statisticians: Provable In-Context Learning with In-Context Algorithm Selection[[Paper]](https://arxiv.org/abs/2306.04637)
- (**NeurIPS'23**)[Theoretical] What can a single attention layer learn? a study through the random features lens[[Paper]](https://arxiv.org/abs/2307.11353)
- (**ICLR'24**)[Theoretical & Empirical] In-Context Learning through the Bayesian Prism[[Paper]](https://arxiv.org/abs/2306.04891)
- (**ICLR'24**)[Theoretical & Empirical] Simplicity Bias of Transformers to Learn Low Sensitivity Functions[[Paper]](https://arxiv.org/abs/2403.06925)
- (**Arxiv'23**)[Empirical] Can Transformer Models Generalize Via In-Context Learning Beyond Pretraining Data?[[Paper]](https://arxiv.org/abs/2208.01066)
- (**Arxiv'23**)[Empirical] Pretraining Data Mixtures Enable Narrow Model Selection Capabilities in Transformer Models [[Paper]](https://arxiv.org/abs/2311.00871)
- (**Arxiv'24**)[Empirical] In-Context Learning State Vector with Inner and Momentum Optimization [[Paper]](https://arxiv.org/abs/2404.11225)


### The Internal Mechanisms of ICL

- (**ICLR'24**) [Empirical] Linear attention is (maybe) all you need to understand transformer optimization [[Paper]](https://arxiv.org/abs/2310.01082)
- (**Arxiv'23**) [Empirical] Uncovering mesa-optimization algorithms in Transformers[[Paper]](https://arxiv.org/abs/2309.05858)
- (**NeurIPS'24**)[Theoretical] On Mesa-Optimization in Autoregressively Trained Transformers: Emergence and Capability[[Paper]](https://arxiv.org/abs/2405.16845)
- (**ACL'23 findings**)[Empirical] Why can gpt learn in-context? language models secretly perform gradient descent as meta optimizers[[Paper]](https://arxiv.org/abs/2212.10559)
- (**ICASSP'24**)[Theoretical] Revisiting the Equivalence of In-Context Learning and Gradient Descent: The Impact of Data Distribution[[Paper]]()
- (**ICML'22**)[Theoretical & Empirical] The dual form of neural networks revisited: Connecting test time predictions to training patterns via spotlights of attention[[Paper]](https://arxiv.org/abs/2202.05798)
- (**ICML'23**)[Theoretical & Empirical] Transformers learn in-context by gradient descent[[Paper]](https://arxiv.org/abs/2212.07677)
- (**ICML'24**)[Empirical] Do pretrained Transformers Really Learn In-context by Gradient Descent?[[Paper]](https://arxiv.org/abs/2310.08540)
- (**Arxiv'23**)[Theoretical] Trained Transformers Learn Linear Models In-Context[[Paper]](https://arxiv.org/abs/2306.09927)
- (**ICLR'24**)[Theoretical] One step of gradient descent is provably the optimal in-context learner with one layer of linear self-attention[[Paper]](https://arxiv.org/abs/2307.03576)
- (**NeurIPS'23**)[Theoretical] Transformers learn to implement preconditioned gradient descent for in-context learning[[Paper]](https://arxiv.org/abs/2306.00297)
- (**ICLR'23**)[Theoretical] What learning algorithm is in-context learning? investigations with linear models[[Paper]](https://arxiv.org/abs/2211.15661)
- (**Arxiv'23**)[Theoretical] The Closeness of In-Context Learning and Weight Shifting for Softmax Regression[[Paper]](https://arxiv.org/abs/2304.13276)
- (**KDD'24**)[Theoretical] In-context Learning with Transformer Is Really Equivalent to a Contrastive Learning Pattern[[Paper]](https://arxiv.org/abs/2310.13220)
- (**ICML'24**)[Theoretical] Transformers Implement Functional Gradient Descent to Learn Non-Linear Functions In Context[[Paper]](https://arxiv.org/abs/2312.06528#:~:text=This%20paper%20provides%20theoretical%20and%20empirical%20evidence%20that,enable%20them%20to%20learn%20non-linear%20functions%20in%20context.)
- (**Arxiv'23**)[Empirical] On the Role of Unstructured Training Data in Transformers' In-Context Learning Capabilities[[Paper]](https://openreview.net/forum?id=aBeZ3jid9i)
- (**ICLR'24**)[Theoretical & Empirical] How Do Transformers Learn In-Context Beyond Simple Functions? A Case Study on Learning with Representation[[Paper]](https://arxiv.org/abs/2310.10616)
- (**Arxiv'24**)[Theoretical] In-Context Learning of a Linear Transformer Block: Benefits of the MLP Component and One-Step GD Initialization[[Paper]](https://arxiv.org/abs/2402.14951)
- (**ICLR'24**)[Theoretical & Empirical] How Do Transformers Learn In-Context Beyond Simple Functions? A Case Study on Learning with Representations[[Paper]](https://arxiv.org/abs/2310.10616)
- (**NeurIPS'24**)[Theoretical & Empirical] In-context learning with transformers: Softmax attention adapts to function lipschitzness[[Paper]](https://arxiv.org/abs/2402.11639)
- (**Arxiv'24**) In-Context Language Learning: Arhitectures and Algorithms[[Paper]](https://arxiv.org/abs/2401.12973)



<div id="skill-recognition-learning"></div>

## Skill Recognition & Skill Learning

- (**ICLR'24**) In-Context Learning through the Bayesian Prism[[Paper]](https://arxiv.org/abs/2306.04891)
- (**Arxiv'23**) Schema-learning and rebinding as mechanisms of in-context learning and emergence[[Paper]](https://arxiv.org/abs/2307.01201)

<div id="skill-composition"></div>

## Skill Composition (Reasoning)
- (**Arxiv'23**) A Theory for Emergence of Complex Skills in Language Models[[Paper]](https://arxiv.org/abs/2307.15936)
- (**EMNLP'22**) Rethinking the Role of Demonstrations: What Makes In-Context Learning Work[[Paper]](https://arxiv.org/abs/2202.12837)
- (**EMNLP'22**) Ground-Truth Labels Matter: A Deeper Look into Input-Label Demonstrations[[Paper]](https://arxiv.org/abs/2205.12685)
- (**Arxiv'23**) The capacity for moral self-correction in large language models[[Paper]](https://arxiv.org/abs/2302.07459)
- (**NeurIPS'23**) Why think step-by-step? Reasoning emerges from the locality of experience[[Paper]](https://arxiv.org/abs/2304.03843)
- (**NeurIPS'23**) Towards Revealing the Mystery behind Chain of Thought: a Theoretical Perspective[[Paper]](https://arxiv.org/abs/2305.15408)
- (**NeurIPS'23**) Dissecting Chain-of-Thought: Compositionality through In-Context Filtering and Learning [[Paper]](https://arxiv.org/abs/2305.18869)
- (**Arxiv'23**) Parrot Mind: Towards Explaining the Complex Task Reasoning of Pretrained Large Language Models with Template-Content Structure[[Paper]](https://arxiv.org/abs/2310.05452)
- (**Arxiv'23**) What Algorithms can Transformers Learn? A Study in Length Generalization[[Paper]](https://arxiv.org/abs/2310.16028)
- (**ICML'21**) Thinking like transformers[[Paper]](https://arxiv.org/abs/2106.06981)
- (**ACL'21**) Self-Attention Networks Can Process Bounded Hierarchical Languages[[Paper]](https://aclanthology.org/2021.acl-long.292/)
- (**Arxiv'23**) Length generalization in arithmetic transformers[[Paper]](https://arxiv.org/abs/2306.15400)
- (**TMLR'23**) Representations and Computations in Transformers that Support Generalization on Structured Tasks[[Paper]](https://openreview.net/forum?id=oFC2LAqS6Z)
- (**Arxiv'23**) Embers of autoregression: Understanding large language models through the problem they are trained to solve[[Paper]](https://arxiv.org/abs/2309.13638)
- (**ICLR'22**) Transformers Learn Shortcuts to Automata[[Paper]](https://arxiv.org/abs/2210.10749)
- (**ICLR'23**) Language Models Are Greedy Reasoners: A Systematic Formal Analysis of Chain-of-Thought[[Paper]](https://arxiv.org/abs/2210.01240)
- (**NeurIPS'23**) Faith and Fate: Limits of Transformers on Compositionality[[Paper]](https://arxiv.org/abs/2305.18654)
- (**Naacl'24**) Reasoning or Reciting? Exploring the Capabilities and Limitations of Language Models Through Counterfactual Tasks[[Paper]](https://aclanthology.org/2024.naacl-long.102/)
- (**ICLR'23**) Language models are greedy reasoners: A systematic formal analysis of chain-of-thought[[Paper]](https://arxiv.org/abs/2210.01240)
- (**Arxiv'22**) Text and patterns: For effective chain of thought, it takes two to tango[[Paper]](https://arxiv.org/abs/2209.07686)
- (**ACL'23**) Towards understanding chain-of-thought prompting: An empirical study of what matters[[Paper]](https://arxiv.org/abs/2212.10001)
- (**COLM'24**) Do large language models have compositional ability? an investigation into limitations and scalability[[Paper]](https://arxiv.org/abs/2407.15720)
- (**Arxiv'24**) Do Large Language Models Perform Latent Multi-Hop Reasoning without Exploiting Shortcuts?[[Paper]](https://arxiv.org/abs/2411.16679)
- (**ICLR'23**) Language Models Are Greedy Reasoners: A Systematic Formal Analysis of Chain-of-Thought [[Paper]](https://arxiv.org/abs/2210.01240)
- (**Arxiv'23**) Large Language Models are In-Context Semantic Reasoners rather than Symbolic Reasoners [[Paper]](https://arxiv.org/abs/2305.14825#:~:text=Our%20findings%20reveal%20that%20semantics%20play%20a%20vital,counter-commonsense%20reasoning%20tasks%20by%20leveraging%20in-context%20new%20knowledge.)
- (**Arxiv'22**) Impact of Pretraining Term Frequencies on Few-Shot Reasoning [[Paper]](https://arxiv.org/abs/2202.07206)
- (**Human Behaviour'23**) Emergent Analogical Reasoning in Large Language Models[[Paper]](https://arxiv.org/abs/2212.09196)
- (**NeurIPS'24**) Understanding Transformer Reasoning Capabilities via Graph Algorithms[[Paper]](https://arxiv.org/abs/2405.18512)

<div id="Knowledge"></div>

## Knowledge
- (**ICLR'24**) How do Language Models Bind Entities in Context?[[Paper]](https://arxiv.org/abs/2310.17191)
- (**ICML'23**) Large Language Models Struggle to Learn Long-Tail Knowledg [[Paper]](https://arxiv.org/abs/2211.08411)
- (**ICLR'24**) Linearity of Relation Decoding in Transformer Language Models [[Paper]](https://arxiv.org/abs/2308.09124)
- (**EMNLP'21**) Transformer feed-forward layers are key-value memories [[Paper]](https://arxiv.org/pdf/2012.14913)
- (**EMNLP'23**) Dissecting Recall of Factual Associations in Auto-Regressive Language Models[[Paper]](https://arxiv.org/abs/2304.14767)
- (**ACL'23**) Analyzing Transformers in Embedding Space[[Paper]](https://arxiv.org/abs/2209.02535)
- (**EMNLP'22**) Transformer Feed-Forward Layers Build Predictions by Promoting Concepts in the Vocabulary Space[[Paper]](https://arxiv.org/abs/2203.14680)

<div id="Mechanism Analysis"></div>

## Mechanism Analysis

- (**Arxiv'22**) In-context learning and induction heads[[Paper]](https://arxiv.org/abs/2209.11895)
- (**EMNLP'24**) Label Words are Anchors: An Information Flow Perspective for Understanding In-Context Learning [[Paper]](https://arxiv.org/abs/2305.14160)
- (**NeurIPS'23**) Towards Automated Circuit Discovery for Mechanistic Interpretability[[Paper]](https://arxiv.org/abs/2304.14997)



<div id="origin"></div>

### The origin of ICL ability

- (**NeurIPS'23**) Birth of a Transformer: A Memory Viewpoint [[Paper]](https://arxiv.org/abs/2306.00802)
- (**NeurIPS'22**) Data distributional properties drive emergent in-context learning in transformers[[Paper]](https://arxiv.org/abs/2205.05055)
- (**Arxiv'23**) Larger language models do in-context learning differently[[Paper]](https://arxiv.org/abs/2303.03846)
- (**Arxiv'23**) The mechanistic basis of data dependence and abrupt learning in an in-context classification task[[Paper]](https://arxiv.org/abs/2312.03002)
- (**ACL'24**) Parallel Structures in Pre-training Data Yield In-Context Learning[[Paper]](https://arxiv.org/abs/2402.12530#:~:text=In%20this%20work%2C%20we%20study%20what%20patterns%20of,following%20similar%20templates%20in%20the%20same%20context%20window.)
- (**NeurIPS'23**) The Transient Nature of Emergent In-Context Learning in Transformers[[Paper]](https://arxiv.org/abs/2311.08360)
- (**ICLR'24**) The mechanistic basis of data dependence and abrupt learning in an in-context classification task [[Paper]](https://arxiv.org/abs/2312.03002)
- (**ICML'24**) Breaking through the Learning Plateaus of In-context Learning in Transformer[[Paper]](https://arxiv.org/pdf/2309.06054)
- (**Arxiv'22**) Transformers generalize differently from information stored in context vs in weights[[Paper]](https://arxiv.org/abs/2210.05675#:~:text=In%20transformers%20trained%20on%20controlled%20stimuli%2C%20we%20find,rule-based%20whereas%20generalization%20from%20context%20is%20largely%20exemplar-based.)
- (**ACL'23**) Understanding In-Context Learning via Supportive Pretraining Data [[Paper]](https://aclanthology.org/2023.acl-long.708/)
- (**Arxiv'22**) ORCA: Interpreting Prompted Language Models via Locating Supporting Data Evidence in the Ocean of Pretraining Data [[Paper]](https://arxiv.org/abs/2205.12600)

<div id="probe"></div>

## Probing Analysis
- (**EMNLP'24**) Discovering Knowledge-Critical Subnetworks in Pretrained Language Models[[Paper]](https://aclanthology.org/2024.emnlp-main.376/)
- (**Arxiv'23**) Eliciting Latent Predictions from Transformers with the Tuned Lens [[Paper]](https://arxiv.org/abs/2303.08112)
- (**Arxiv'23**) Representation Engineering: A Top-Down Approach to AI Transparency [[Paper]](https://arxiv.org/abs/2310.01405)
- (**ICML'24**) Patchscopes: A Unifying Framework for Inspecting Hidden Representations of Language Models [[Paper]](https://arxiv.org/abs/2401.06102)
- (**EMNLP'24**) Backward Lens: Projecting Language Model Gradients into the Vocabulary Space [[Paper]](https://aclanthology.org/2024.emnlp-main.142/)


<div id="correction"></div>

### Self Correction
- (**ICLR'24**) Large Language Models Cannot Self-Correct Reasoning Yet[[Paper]](https://arxiv.org/abs/2310.01798)
- (**Arxiv'22**) Language models (mostly) know what they know[[Paper]](https://arxiv.org/abs/2207.05221)
- (**Arxiv'24**) On the Intrinsic Self-Correction Capability of LLMs: Uncertainty and Latent Concept [[Paper]](https://arxiv.org/abs/2406.02378)
- (**EMNLP'24**) Intrinsic Self-correction for Enhanced Morality: An Analysis of Internal Mechanisms and the Superficial Hypothesis[[Paper]](https://aclanthology.org/2024.emnlp-main.918/)


<div id="empirical"></div>

### More empirical studies
- (**ICML'23**) Large language models can be easily distracted by irrelevant context[[Paper]](https://arxiv.org/abs/2302.00093)
- (**NAACL'22**) Do prompt-based models really understand the meaning of their prompts?[[Paper]](https://arxiv.org/abs/2109.01247)
- (**Arxiv'23**) When does In-context Learning Fall Short and Why? A Study on Specification-Heavy Tasks[[Paper]](https://arxiv.org/abs/2311.08993)
- (**Arxiv'23**) How do Language Models Bind Entities in Context?[[Paper]](https://arxiv.org/abs/2310.17191)
- (**ACL'23 Findings**) What In-Context Learning “Learns” In-Context: Disentangling Task Recognition and Task Learning [[Paper]](https://aclanthology.org/2023.findings-acl.527/)
- (**ACL'23 findings**) Large Language Models Can be Lazy Learners: Analyze Shortcuts in In-Context Learning[[Paper]](https://aclanthology.org/2023.findings-acl.284/)
- (**ACL'22 findings**) Can language models learn from explanations in context? [[Paper]](https://arxiv.org/abs/2204.02329)
- (**ACL'23 findings**) Complementary Explanations for Effective In-Context Learning [[Paper]](https://aclanthology.org/2023.findings-acl.273/)
- (**naacl'23**) Do Prompt-Based Models Really Understand the Meaning of Their Prompts? [[Paper]](https://arxiv.org/abs/2109.01247)
- (**Arxiv'23**) Larger language models do in-context learning differently [[Paper]](https://arxiv.org/abs/2303.03846)
- (**NeurIPS'23**) Lexinvariant Language Models [[Paper]](https://arxiv.org/abs/2305.16349)
- (**ACL'23**) Measuring Inductive Biases of In-Context Learning with Underspecified Demonstrations[[Paper]](https://arxiv.org/abs/2305.13299)
- (**naacl'24**) How are Prompts Different in Terms of Sensitivity?[[Paper]](https://arxiv.org/abs/2311.07230)
- (**ICLR'23**) Emergent World Representations: Exploring a Sequence Model Trained on a Synthetic Task[[Paper]](https://arxiv.org/abs/2210.13382)
- (**ICLR'24**) Efficient Streaming Language Models with Attention Sinks[[Paper]](https://arxiv.org/abs/2309.17453)
- (**EMNLP'22**) Are All Spurious Features in Natural Language Alike? An Analysis through a Causal Lens [[Paper]](https://aclanthology.org/2022.emnlp-main.666/)
- (**Arxiv'23**) Analyzing Text Representations by Measuring Task Alignment[[Paper]](https://arxiv.org/abs/2305.19747)
- (**ICLR'24**) Understanding In-Context Learning from Repetitions[[Paper]](https://arxiv.org/abs/2310.00297)
- (**EMNLP'21**) Surface Form Competition: Why the Highest Probability Answer Isn’t Always Right [[Paper]](https://aclanthology.org/2021.emnlp-main.564/)
- (**ICML'23**) A Toy Model of Universality: Reverse Engineering How Networks Learn Group Operations[[Paper]](https://arxiv.org/abs/2302.03025)
- (**ACL'23**) Rethinking the Role of Scale for In-Context Learning: An Interpretability-based Case Study at 66 Billion Scale [[Paper]](https://arxiv.org/abs/2212.09095)
- (**ICLR'23**) Progress measures for grokking via mechanistic interpretability[[Paper]](https://arxiv.org/abs/2301.05217)
- (**ACL'23**) Mitigating Label Biases for In-context Learning[[Paper]](https://arxiv.org/abs/2305.19148)
- (**TACL'24**) Lost in the Middle: How Language Models Use Long Contexts [[Paper]](https://aclanthology.org/2024.tacl-1.9/)
- (**Arxiv'20**) What Happens To BERT Embeddings During Fine-tuning?[[Paper]](https://arxiv.org/abs/2004.14448)
- (**Arxiv'19**) What Does BERTLookAt? An Analysis of BERT’s Attention[[Paper]](https://aclanthology.org/W19-4828/)
- (**ACl'20**) Similarity Analysis of Contextual Word Representation Models[[Paper]](https://arxiv.org/abs/2005.01172#:~:text=This%20paper%20investigates%20contextual%20word%20representation%20models%20from,Critically%2C%20these%20models%20come%20from%20vastly%20different%20architectures.)
(**Arxiv'24**) From Insights to Actions: The Impact of Interpretability and Analysis Research on NLP [[Paper]](https://arxiv.org/pdf/2406.12618)
- (**'**) [[Paper]]()
- (**'**) [[Paper]]()
- (**'**) [[Paper]]()


