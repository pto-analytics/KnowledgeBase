# Chapter 1 --- Introduction to Building AI Applications with Foundation Models

> **Source:** Based on my handwritten notes from Chapter 1. Any
> additional explanations are marked as **💡 Added Context**.

## Summary

The rapid scaling of AI models has fundamentally changed software
development. Instead of building machine learning models from scratch,
developers can leverage large pre-trained **foundation models** through
APIs and customize them for specific tasks using techniques such as
prompt engineering, Retrieval-Augmented Generation (RAG), and
fine-tuning.

This shift has lowered barriers to entry, created the discipline of **AI
Engineering**, and enabled entirely new categories of applications.

------------------------------------------------------------------------

# Key Concepts

## Scaling AI Models

-   Larger models solve more complex tasks.
-   More applications become possible.
-   Training requires enormous computation.
-   Models are increasingly delivered as **Model-as-a-Service (MaaS)**.
-   Lower barriers to entry have accelerated the rise of AI Engineering.

## Foundation Models

Foundation models are large pre-trained, general-purpose models that can
be adapted to many downstream tasks.

Examples:

-   GPT
-   Claude
-   Gemini
-   Llama

## Language Models

Language models learn statistical relationships between words and
predict the most likely next token.

### Definitions

  -----------------------------------------------------------------------
  Term                    Definition
  ----------------------- -----------------------------------------------
  Token                   The basic unit processed by an LLM (word,
                          subword, punctuation, etc.).

  Tokenization            Breaking text into tokens before processing.

  Vocabulary              The complete set of tokens recognized by the
                          model.
  -----------------------------------------------------------------------

------------------------------------------------------------------------

# Types of Language Models

## Masked Language Models

-   Predict missing tokens.
-   Used primarily for understanding tasks.
-   Example: **BERT**

## Autoregressive Models

-   Predict one token at a time.
-   Used for text generation.
-   Examples include GPT, Claude, and Gemini.

------------------------------------------------------------------------

# Self-Supervised Learning

Traditional supervised learning relies on labeled data, which is
expensive and time-consuming.

Self-supervised learning instead creates labels from the data itself,
allowing models to learn from enormous unlabeled datasets.

> 💡 **Added Context:** AlexNet's 2012 ImageNet victory helped launch
> the modern deep learning revolution, while self-supervised learning
> later enabled today's large language models.

------------------------------------------------------------------------

# Model Size

Model size is typically measured by **parameters**.

  Model                     Parameters
  ----------------------- ------------
  GPT-1                           117M
  GPT-2                           1.5B
  GPT-5 *(course note)*            2T+

Larger models generally:

-   Learn richer patterns
-   Require more compute
-   Require more training data

Smaller models may still be preferable when they provide similar
performance at lower cost.

------------------------------------------------------------------------

# Multimodal Models

Large Multimodal Models (LMMs) process multiple modalities
simultaneously:

-   Text
-   Images
-   Audio
-   Video

------------------------------------------------------------------------

# Adapting Foundation Models

## Prompt Engineering

Provide better instructions.

## Retrieval-Augmented Generation (RAG)

Connect the model to external knowledge sources such as databases or
documentation.

## Fine-Tuning

Continue training a foundation model on a specialized dataset.

------------------------------------------------------------------------

# AI Engineering vs ML Engineering

**Machine Learning Engineering**

-   Builds and trains models.

**AI Engineering**

-   Uses existing models to build valuable applications.

------------------------------------------------------------------------

# Why AI Engineering is Growing

-   New applications are possible.
-   Existing applications improve dramatically.
-   APIs eliminate hosting complexity.
-   Faster development.
-   Lower costs.
-   Higher ROI.

------------------------------------------------------------------------

# Why Few Companies Train Foundation Models

Training frontier models requires enormous resources.

Examples include:

-   OpenAI
-   Google
-   Microsoft
-   Meta
-   Anthropic
-   Mistral
-   Tencent
-   Baidu

------------------------------------------------------------------------

# Common AI Use Cases

-   Software development
-   Image and video generation
-   Writing assistance
-   Education
-   Conversational bots
-   Information aggregation
-   Data extraction and organization
-   Workflow automation

------------------------------------------------------------------------

# AI Agents

AI systems that can reason, use tools, call APIs, and perform actions
autonomously.

> 💡 **Added Context:** Agents combine an LLM with external tools to
> complete multi-step workflows.

------------------------------------------------------------------------

# Planning AI Applications

Consider:

-   Business value
-   AI's role
-   Reactive vs proactive behavior
-   Dynamic vs static experiences
-   Human involvement

Human involvement often progresses from:

1.  Human in the loop
2.  Human on the loop
3.  Human out of the loop

------------------------------------------------------------------------

# Competitive Advantages

1.  Technology
2.  Distribution
3.  Proprietary Data

------------------------------------------------------------------------

# Product Evaluation

Measure:

-   Quality
-   Latency
-   Cost
-   Interpretability
-   Fairness

Choose the smallest model that meets business requirements.

------------------------------------------------------------------------

# Long-Term Maintenance

Foundation models improve rapidly.

Plan for:

-   Better reasoning
-   Larger context windows
-   Lower inference costs
-   Product evolution over time

------------------------------------------------------------------------

# Examples

### Prompt Engineering

``` text
Summarize this report in three executive bullet points.
```

### RAG

``` text
Answer using our internal documentation.
```

### AI Agent

``` text
Read emails
→ Find unpaid invoices
→ Generate reminders
→ Send emails
```

------------------------------------------------------------------------

# Work Applications

-   AI copilot for planning tools
-   RAG over internal documentation
-   AI-powered SQL assistant
-   BOM and PDF extraction
-   Daily operational summaries
-   Supply chain AI agents

------------------------------------------------------------------------

# Related Topics

-   Transformers
-   Attention
-   Embeddings
-   Prompt Engineering
-   RAG
-   Fine-Tuning
-   AI Agents
-   Context Windows
-   Model Evaluation

------------------------------------------------------------------------

# Questions for Review

1.  What is a foundation model?
2.  Why are autoregressive models used for generation?
3.  How does self-supervised learning differ from supervised learning?
4.  Why isn't the largest model always the best?
5.  When should you use RAG instead of fine-tuning?
6.  How does AI Engineering differ from ML Engineering?
7.  What defines an AI agent?
8.  What are the three major competitive advantages in AI?
