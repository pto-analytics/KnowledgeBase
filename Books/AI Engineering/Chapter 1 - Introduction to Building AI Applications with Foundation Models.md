# Building AI Applications with Foundation Models

*Source: AI Engineering - Chapter 1*

------------------------------------------------------------------------

# Executive Summary

1.  **Foundation models fundamentally changed AI development.** Instead
    of training models from scratch, most applications are now built by
    adapting powerful pre-trained models.
2.  **AI Engineering is primarily about building systems around models,
    not building the models themselves.** Success comes from integrating
    prompting, retrieval, external tools, evaluation, and application
    logic.
3.  **Language models predict the next token probabilistically.**
    Everything---from conversations to code generation---is an emergent
    behavior of next-token prediction at scale.
4.  **Scaling laws matter.** Larger models generally learn richer
    representations and solve more tasks, but they require significantly
    more compute, data, and inference cost.
5.  **Foundation models are generalists.** They perform well across many
    tasks, but task-specific optimization (prompt engineering, RAG,
    fine-tuning) often produces substantially better results.
6.  **Model-as-a-Service democratized AI.** API access removed the need
    for organizations to train and host large models, dramatically
    lowering barriers to building AI products.
7.  **Competitive advantage is shifting toward proprietary data, product
    design, distribution, and execution.**
8.  **AI applications should begin with business value, not
    technology.**
9.  **Many useful AI systems require external tools; these become AI
    agents when they can reason and act.**
10. **Build AI systems that evolve as foundation models improve.**

# Why This Matters

Foundation models shifted software development from building
intelligence to integrating intelligence. Modern AI engineering focuses
on system design, orchestration, retrieval, evaluation, and product
integration rather than training large models.

# Mental Model

``` text
Large Training Dataset
          │
          ▼
 Foundation Model
          │
 ┌────────┼────────┐
 │        │        │
Prompt   RAG   Fine-Tuning
          │
          ▼
 Application Logic
          │
          ▼
 Users / APIs / Tools
```

# Key Concepts

## Scaling Foundation Models

-   Larger models generally learn richer representations.
-   Larger models require more compute and inference cost.
-   Bigger is not always better; choose the smallest model that meets
    requirements.

## Language Models

-   Predict the next token based on previous context.
-   Tokens are the basic processing unit.
-   Tokenization converts text into tokens.
-   Vocabulary is the complete set of tokens a model understands.

## Self-Supervised Learning

-   Learns from unlabeled data by generating labels from the data
    itself.
-   Eliminates much of the manual labeling bottleneck.
-   Enables training on internet-scale datasets.

> **AI Clarification:** Self-supervised learning creates prediction
> targets directly from the input data (e.g., predicting missing or next
> tokens).

## Foundation Models

-   Large pre-trained, general-purpose models.
-   Adapted rather than retrained for most applications.
-   Includes Large Language Models (LLMs) and Large Multimodal Models
    (LMMs).

## Multimodal Models

Process and reason across multiple data types:

-   Text
-   Images
-   Audio
-   Video

## Adapting Foundation Models

### Prompt Engineering

Improve instructions without retraining.

### Retrieval-Augmented Generation (RAG)

Inject external knowledge during inference.

### Fine-Tuning

Continue training to modify model behavior for a specific domain or
task.

# AI Engineering vs Machine Learning Engineering

**Machine Learning Engineering**

-   Collect data
-   Train models
-   Optimize algorithms

**AI Engineering**

-   Build applications using existing foundation models
-   Integrate APIs
-   Design prompts and retrieval
-   Evaluate systems
-   Deliver business value

> **Key Insight:** AI Engineering is about applying intelligence, not
> creating it.

# AI Agents

AI agents:

1.  Reason
2.  Decide
3.  Use external tools
4.  Observe results
5.  Continue until the objective is achieved

# Planning AI Applications

Consider:

-   Business value
-   AI's role (core vs enhancement)
-   Human oversight
-   Latency
-   Cost
-   Quality
-   Fairness
-   Maintainability

# Work Applications

## Software Engineering

-   Code generation
-   Documentation
-   Testing
-   Code review

## AI Engineering

-   Enterprise RAG systems
-   Internal copilots
-   AI agents
-   Prompt/RAG/Fine-tuning decisions

## Analytics

-   Natural-language BI
-   Automated reporting
-   Insight generation

## Supply Chain

-   Planner copilots
-   BOM/document understanding
-   ERP workflow automation
-   Risk summarization

## Teaching

-   Personalized learning
-   Lesson generation
-   Question creation
-   Content summarization

## Productivity

-   Meeting summaries
-   Email drafting
-   Research synthesis
-   Workflow automation

# Personal Insights

-   Model-as-a-Service dramatically lowered barriers to entry.
-   AI Engineering is distinct from Machine Learning Engineering.
-   Model selection is an engineering tradeoff, not simply choosing the
    biggest model.
-   Business value matters more than technical novelty.
-   AI products should expect rapid model improvement.

# Enduring Principles

-   Build around foundation models.
-   Start with prompting.
-   Add RAG before fine-tuning when knowledge is the problem.
-   Optimize for business value.
-   The surrounding system often matters more than the model.

# Common Misconceptions

-   Bigger models are always better.
-   Fine-tuning is always required.
-   AI Engineering equals Machine Learning Engineering.
-   Foundation models replace software engineering.
-   A good demo guarantees a good product.

# Connections

-   Transformers
-   Attention
-   Tokenization
-   Embeddings
-   Prompt Engineering
-   RAG
-   Fine-Tuning
-   Context Windows
-   AI Agents
-   Tool Calling
-   Inference
-   Vector Databases
-   Model Evaluation

# Questions for Review

1.  Why did foundation models change AI development?
2.  Why does next-token prediction enable complex behaviors?
3.  When should you use prompting vs RAG vs fine-tuning?
4.  What tradeoffs come with larger models?
5.  How does self-supervised learning work?
6.  How is AI Engineering different from ML Engineering?
7.  Where will competitive advantage come from?
8.  When should humans remain in the loop?
9.  Which metrics matter most in production?
10. Why should AI systems be designed to evolve?

# Future Reading

-   Transformers
-   Scaling Laws
-   Embeddings
-   Vector Databases
-   RAG
-   Fine-Tuning
-   AI Agents
-   Prompt Optimization
-   Model Evaluation

# One-Sentence Takeaway

> **Foundation models transformed AI from building models to building
> intelligent systems around pre-trained models.**
