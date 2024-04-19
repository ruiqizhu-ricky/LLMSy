# LLMSy

## Neuro[Symbolic] AI

[Neuro-symbolic AI](https://en.wikipedia.org/wiki/Neuro-symbolic_AI), as its name indicates, is an AI approach that combines the [neural AI methods](https://en.wikipedia.org/wiki/Connectionism) and [symbolic AI methods](https://en.wikipedia.org/wiki/Symbolic_artificial_intelligence). Nevertheless, how to combine these 2 methods is still under exploration. Henry Kautz in his [AAAI 2020 Robert S. Engelmore Memorial Award Lecture](https://www.youtube.com/watch?v=_cQITY0SPiw)  pointed out that there are at least 5 categories. 

Personally, I am particularly advocating one of it, the *Neuro[Symbolic]* one, meaning "the embedding of symbolic reasoning inside a neural engine, where symbolic reasoning is understood as 'deliberative, type 2 reasoning' as common." An example would be using ChatGPT uas a neural engine to understand the problem, decompose the problem into sub-tasks, call the symbolic tools to solve these sub-tasks, and finally ChatGPT synthesise the results.

The reason why I am fond of this approach is that it directly mimics how human brains work. Our biological brains are naturally neural engines, and we use our brains to understand the problem, decompose the problem into sub-tasks, call the symbolic tools to solve these sub-tasks, and finally synthesise the results. In fact, we are encouraged to adhere to this workflow as much as possible, rather than solving the problem end-to-end, as we believe that this can not only increase accuracy but also transparency (and thus explainability plus debuggability). 

Today, the state-of-the-art neural engines are [Large Language Models (LLMs)](https://en.wikipedia.org/wiki/Large_language_model), or its generalised, multimodal version, [Fundation Models (FMs)](https://en.wikipedia.org/wiki/Foundation_model). Hence, I am keen to explore the idea of *LLM[Sy]* which understands and processes the problem using LLMs, and calls external symbolic tools when necessary.


### Tool-augmented LLMs
The study of Tool-augmented LLMs is to address the [hallucination](https://arxiv.org/abs/2311.05232) problem of LLMs, by equipping them with versatile tools such as calculators, theorem provers, code interpreters, search engines, or even physical robots. This is exactly the foxus of LLMSy, which is to understand the problem and extract sub-problems that can be solved by symbolic tools. 
- [ChatGPT-plugins](https://openai.com/blog/chatgpt-plugins)
- [Toolformer: Language Models Can Teach Themselves to Use Tools](https://proceedings.neurips.cc/paper_files/paper/2023/hash/d842425e4bf79ba039352da0f658a906-Abstract-Conference.html)
- [TALM: Tool Augmented Language Models](https://arxiv.org/pdf/2205.12255.pdf)
- [PAL: Program-aided Language Models](https://proceedings.mlr.press/v202/gao23f/gao23f.pdf)
- [Augmented Language Models: a Survey](https://openreview.net/pdf?id=jh7wH2AzKK)

### Auto-formalisation

In science, the process of *putting the blur ideas down on paper in formal language* is sometimes called [formalisation](https://en.wikipedia.org/wiki/Scientific_formalism), or more specifically, [logic translatioin](https://en.wikipedia.org/wiki/Logic_translation) which translate a problem from natural language (as well as image or other information) into formal language, that is, logic and math. The branch of AI research targetting on this process is auto-formalisation. Here are some selected papers on this topic: 
- [A Promising Path Towards Autoformalization and General Artificial Intelligence](https://link.springer.com/chapter/10.1007/978-3-030-53518-6_1)
- [Autoformalization with Large Language Models](https://arxiv.org/pdf/2205.12615.pdf)
- [Draft, Sketch, and Prove](https://openreview.net/pdf?id=SMa9EAovKMC)
- [Formal Specifications from Natural Language](https://arxiv.org/pdf/2206.01962v2.pdf)
- [Baldur: Whole-Proof Generation and Repair with Large Language Models](https://arxiv.org/pdf/2303.04910.pdf)
- [Don't Trust: Verify--Grounding LLM Quantitative Reasoning with Autoformalization](https://arxiv.org/pdf/2403.18120.pdf)

The above papers focus on a particular domain: converting informal math into formal math, and thus proving theorems automatically. More related resources are in [Tutorial on Machine Learning for Theorem Proving @ NeurIPS 2023](https://machine-learning-for-theorem-proving.github.io/). A natural generalisation of formalise math/proofs is to formalise scientific theories apart from abstract math, but also organic chemistry, genetics, behavoural modelling, etc. Math and proofs can be Represented by math formulas or theorem proving language, such as [Lean](https://lean-lang.org/), [Coq](https://coq.inria.fr/), and [Isabelle](https://isabelle.in.tum.de/). 



SImilarly, scientific theories can be represented by modelling languages ([PDDL](https://en.wikipedia.org/wiki/Planning_Domain_Definition_Language) for planning) or even general-purpose programming languages (Python or Javascript). The studies on how to do this is called [program synthesis](https://www.neurosymbolic.org/methods.html), or more fashinably, [(AI) code generation](https://github.blog/2024-02-22-how-ai-code-generation-works/).

[Large Language Model for Optimization Modeling](https://arxiv.org/pdf/2402.10172.pdf)

[Automating the process of generating scientific theories from data](https://www.neurosymbolic.org/index.html)
