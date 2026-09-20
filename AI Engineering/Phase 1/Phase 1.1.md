## AI Prerequisites

## 1.1 What is Artificial Intelligence?

Today we officially begin the AI Engineering roadmap.

The goal of this topic isn't to memorize a definition. You should finish knowing **what AI actually means, why it exists, how an AI system differs from normal software, and how this connects to LLMs and the rest of our roadmap.**

---

# 1. Concept

Let's start with the simplest idea.

Traditional software usually works like:

**Human writes rules → Computer follows rules → Output**

For example:

```
Input
  ↓
if marks >= 40
  ↓
"Pass"
else
  ↓
"Fail"
```

The programmer explicitly defines the logic.

AI tries to solve problems where explicitly writing every rule becomes difficult or impractical.

For example:

> "Is this image a cat?"

There isn't a practical list of rules like:

```
IF ears are pointed
AND fur exists
AND four legs
AND ...
THEN cat
```

Instead, an AI system can learn patterns from examples and use those patterns to produce an output.

So the fundamental idea is:

> **AI enables computers to perform tasks that normally require aspects of human intelligence.**

---

# 2. Standard Definition ⭐

### Interview-ready definition

> **Artificial Intelligence (AI) is a field of computer science focused on creating systems that can perform tasks that typically require human intelligence, such as learning, reasoning, perception, language understanding, and decision-making.**

This is the definition you should remember.

### Short version

> **AI is the field of creating machines that can perform tasks requiring human-like intelligence.**

For interviews, use the first definition when asked **"What is AI?"**

---

# 3. Why Does AI Exist?

The basic motivation is:

### Problem

Some problems are extremely difficult to solve using manually written rules.

Examples:

- Understanding human language
- Recognizing faces
- Understanding images
- Speech recognition
- Translating languages
- Detecting fraud
- Predicting patterns
- Generating text
- Making decisions from huge amounts of data

Instead of explicitly programming every possible situation, we want systems capable of handling complex patterns.

---

# 4. Intuition 🧠

Think about teaching a child to recognize a dog.

You don't give the child thousands of rules:

> Four legs + fur + tail + specific ears = dog.

Instead, you show examples.

```
🐕 Dog
🐕 Dog
🐕 Dog
🐕 Dog
🐈 Not Dog
🐈 Not Dog
```

Eventually, the child develops an internal understanding of what makes something look like a dog.

AI systems can similarly learn patterns from data.

That's the key idea behind modern AI.

---

# 5. Traditional Programming vs AI

This distinction is **very important for interviews**.

### Traditional Programming

```
Rules + Data
     ↓
  Program
     ↓
  Output
```

The programmer creates the rules.

---

### Machine Learning

```
Data + Expected Outputs
          ↓
       Learning
          ↓
         Model
          ↓
     New Input
          ↓
      Prediction
```

The system learns patterns from examples.

This is one of the fundamental transitions from traditional programming toward modern AI.

---

# 6. How Does an AI System Work?

At a very high level:

```
        DATA
          ↓
    AI / ML MODEL
          ↓
   LEARNED PATTERNS
          ↓
       NEW INPUT
          ↓
       OUTPUT
```

For example, consider an image classification system.
 
```
Thousands of images
        ↓
      Training
        ↓
   Trained Model
        ↓
   New Image
        ↓
 "This is a dog"
```

The important word here is **model**.

A model is the learned computational representation that allows the system to make predictions, generate outputs, or perform a task.

We'll study models much more deeply in later phases.

---

# 7. AI Is Much Bigger Than ChatGPT

This is an important misconception to avoid.

AI includes many areas:

```
                    AI
                     │
        ┌────────────┼────────────┐
        ↓            ↓            ↓
     Robotics       ML       Rule-based AI
                     │
              ┌──────┴──────┐
              ↓             ↓
             DL       Other ML
              │
        ┌─────┴─────┐
        ↓           ↓
   Transformers    CNNs
        │
   ┌────┼─────────────┐
   ↓    ↓             ↓
  LLMs Vision       Multimodal
   │
   ├── Chatbots
   ├── RAG
   └── Agents
```

The exact boundaries can vary depending on how the field is described, but the important mental model is:

> **LLMs are one part of the much larger AI ecosystem.**

---

# 8. Types of AI

You'll often hear three terms in interviews.

## 8.1 Narrow AI / Weak AI

An AI system designed for a specific task or limited range of tasks.

Examples:

- Face recognition
- Recommendation systems
- Spam detection
- Chess engines
- Voice assistants
- Image classifiers

Almost all practical AI systems today fall into this category.

---

## 8.2 AGI — Artificial General Intelligence

A hypothetical AI capable of performing a broad range of intellectual tasks at a level comparable to or beyond humans.

The key word is **general**.

Instead of being designed primarily for one task, AGI would have broad capabilities across many domains.

AGI remains a research goal/concept rather than a universally agreed-upon achieved system.

---

## 8.3 ASI — Artificial Superintelligence

A hypothetical form of intelligence that would substantially exceed human intelligence across essentially all relevant intellectual domains.

This is primarily a theoretical/future concept.

### Interview tip

If asked:

> "What type of AI do we have today?"

A safe answer is:

> **Most deployed AI systems are narrow or specialized AI systems, even when they have broad capabilities across multiple tasks. AGI and ASI refer to hypothetical levels of general or superhuman intelligence.**

---

# 9. What Makes a System "Intelligent"?

There isn't one universally accepted checklist, but AI systems commonly involve capabilities such as:

### Perception

Understanding information from the environment.

Examples:

- Images
- Video
- Audio

### Learning

Improving behavior based on data or experience.

### Reasoning

Using information to derive conclusions.

### Decision-making

Selecting actions based on inputs and objectives.

### Language

Understanding or generating human language.

### Planning

Determining a sequence of actions to accomplish a goal.

These capabilities will become extremely important when we reach **LLMs and Agents**.

---

# 10. Real-World AI Examples 🌍

|Application|AI Capability|
|---|---|
|Face Recognition|Computer Vision|
|Google Maps ETA|Prediction|
|Netflix Recommendations|Recommendation|
|Spam Detection|Classification|
|Voice Assistant|Speech + Language|
|ChatGPT|Language Generation|
|Self-driving systems|Perception + Decision-making|
|Fraud Detection|Pattern Detection|
|Medical Image Analysis|Computer Vision|
|AI Coding Assistants|Language + Code Generation|

---

# 11. AI vs Automation

This is a common interview confusion.

### Automation

A predefined workflow executes predefined rules.

```
Event
 ↓
Rule
 ↓
Action
```

Example:

> If an email arrives from X → move it to folder Y.

---

### AI

The system can use learned patterns or computational reasoning to handle inputs that aren't fully specified through explicit rules.

Example:

> Analyze this email and determine whether it is a complaint, refund request, or sales inquiry.

### Important distinction

**Automation doesn't necessarily require AI.**

**AI can be used to make automation more flexible and intelligent.**

Modern systems often combine both:

```
AI
 ↓
Decision
 ↓
Automation
 ↓
Action
```

---

# 12. AI vs Normal Software

This is another important interview concept.

|Traditional Software|AI System|
|---|---|
|Rules explicitly programmed|Behavior may be learned or generated|
|Usually deterministic for same conditions|Can be probabilistic/non-deterministic|
|Logic defined by developer|Model parameters encode learned patterns|
|Works well for clearly defined rules|Useful for complex pattern-based tasks|
|Example: Calculator|Example: Image classifier|

However, don't say:

> "Traditional software is deterministic and AI is always non-deterministic."

That's too absolute.

AI systems can include deterministic components, and traditional software can also contain randomness.

---

# 13. AI Does NOT Mean Human Intelligence

Another important point.

AI systems don't necessarily:

- Think like humans
- Understand the world exactly like humans
- Possess consciousness
- Have emotions
- Have human common sense

When we say a system performs an "intelligent task," we mean it can **perform a capability associated with intelligent behavior**, not necessarily that it has a human mind.

This distinction becomes especially important when we study LLMs.

---

# ⭐ Important Points to Remember

These are your **revision points**:

1. **AI is a field of computer science.**
2. AI aims to create systems capable of performing tasks associated with human intelligence.
3. AI includes capabilities such as perception, learning, reasoning, language, planning, and decision-making.
4. **AI is broader than Machine Learning.**
5. **Machine Learning is a major approach used to build AI systems.**
6. Deep Learning is a subset of Machine Learning.
7. Modern LLMs are based on Deep Learning.
8. Most deployed AI today is specialized/narrow AI.
9. AGI refers to hypothetical general-purpose intelligence.
10. Automation and AI are not the same thing.
11. AI systems don't necessarily think or understand exactly like humans.
12. **Model** is a central concept in modern AI.
13. Training and inference are different stages.
14. LLMs are only one part of the broader AI ecosystem.

---

# 🎯 Interview Preparation

## Q1. What is Artificial Intelligence?

### Interview Answer

> Artificial Intelligence is a field of computer science focused on creating systems that can perform tasks that typically require human intelligence, such as learning, reasoning, perception, language understanding, and decision-making.

---

## Q2. What are the main goals of AI?

### Interview Answer

> The main goal of AI is to develop systems capable of performing intelligent tasks such as perception, learning, reasoning, planning, language understanding, and decision-making.

---

## Q3. What is Narrow AI?

### Interview Answer

> Narrow AI refers to AI systems designed to perform specific tasks or a limited range of tasks. Examples include recommendation systems, face recognition systems, spam filters, and image classifiers.

---

## Q4. What is AGI?

### Interview Answer

> Artificial General Intelligence refers to a hypothetical AI system capable of performing a broad range of intellectual tasks with general-purpose intelligence comparable to or exceeding human capabilities.

---

## Q5. What is the difference between AI and Machine Learning?

### Interview Answer

> AI is the broader field of creating systems capable of intelligent behavior, while Machine Learning is an approach within AI where systems learn patterns from data rather than relying entirely on explicitly programmed rules.

---

## Q6. Is Machine Learning the same as AI?

### Interview Answer

> No. Machine Learning is a subset of AI. AI is the broader field, while ML is one of the major techniques used to build AI systems.

---

## Q7. What is the difference between AI and automation?

### Interview Answer

> Automation generally executes predefined rules or workflows, while AI can perform tasks involving learned patterns, perception, prediction, generation, or decision-making. AI can also be used as a component within an automated workflow.

---

## Q8. Is ChatGPT AI?

### Interview Answer

> Yes. ChatGPT is an AI application built around large language models. The underlying models use deep learning and Transformer-based architectures to process and generate language.

---

## Q9. What is a model in AI?

### Interview Answer

> An AI model is a computational representation that has learned patterns from data or has been designed to perform a particular computational task, allowing it to produce predictions, classifications, generations, or other outputs from inputs.

---

## Q10. Why can't we simply program rules for every AI problem?

### Interview Answer

> Many real-world problems involve complex, high-dimensional, or ambiguous patterns that are difficult to express through manually written rules. Machine learning and other AI techniques allow systems to learn useful patterns from data instead.

---

# ⚠️ Common Mistakes

### ❌ Mistake 1

> "AI means robots."

No.

Robotics is one application area that can use AI.

---

### ❌ Mistake 2

> "AI = Machine Learning."

Incorrect.

ML is a subset/approach within AI.

---

### ❌ Mistake 3

> "Deep Learning is separate from AI."

Incorrect.

```
AI
└── ML
    └── DL
```

---

### ❌ Mistake 4

> "All AI thinks like humans."

Not necessarily.

AI systems perform specific computational tasks associated with intelligent behavior.

---

### ❌ Mistake 5

> "ChatGPT is AGI."

Don't make this claim casually.

A conversational model can have broad capabilities without that establishing that it has achieved AGI.

---

# 🌍 Real-World Connection

Now connect today's topic to our roadmap.

Eventually we'll build:

```
AI
 ↓
Deep Learning
 ↓
Transformers
 ↓
LLMs
 ↓
LLM APIs
 ↓
Embeddings
 ↓
Vector Database
 ↓
RAG
 ↓
Agents
 ↓
Production AI Application
```

Right now we're at the very top:

**AI → What is it?**

In **Phase 3**, we'll go much deeper into the Transformer/LLM portion of this chain.

---

# 📝 NOTION NOTES — 1.1 What is Artificial Intelligence?

## Definition

**Artificial Intelligence (AI)** is a field of computer science focused on creating systems that can perform tasks that typically require human intelligence, such as learning, reasoning, perception, language understanding, and decision-making.

## Core Idea

Traditional programming:

**Rules + Data → Output**

Machine Learning:

**Data + Examples → Learning → Model → Prediction**

## Major AI Capabilities

- Perception
- Learning
- Reasoning
- Decision-making
- Language understanding
- Planning

## Types of AI

**Narrow AI:** Designed for specific or limited tasks.

**AGI:** Hypothetical general-purpose intelligence capable of broad intellectual tasks.

**ASI:** Hypothetical intelligence substantially exceeding human intelligence across intellectual domains.

## AI Hierarchy

```
AI
└── Machine Learning
    └── Deep Learning
        └── Transformers
            └── LLMs
                └── Generative AI Applications
                    ├── RAG
                    └── Agents
```

## Important Terms

- AI
- Machine Learning
- Deep Learning
- Model
- Training
- Inference
- Narrow AI
- AGI
- ASI
- Generative AI

## Interview Points

- AI is broader than ML.
- ML is a major approach within AI.
- DL is a subset of ML.
- LLMs are modern deep learning models.
- Most deployed AI is specialized/narrow AI.
- Automation and AI are different concepts.
- AI doesn't necessarily imply human-like consciousness or understanding.

## One-Line Revision

> **AI is the broader field of building systems capable of intelligent behavior; ML is one major way of achieving it, and modern LLMs are built using deep learning and Transformer architectures.**

---

# 🔵 Missing / Advanced Topics

Not needed yet:

- Search algorithms
- Knowledge representation
- Expert systems
- Fuzzy logic
- Genetic algorithms
- Planning algorithms
- AI research history in detail

We'll only revisit these if they become relevant to the AI Engineering path or interviews.

---
