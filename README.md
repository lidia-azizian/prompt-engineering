# Prompt Engineering

**A collection of 21 hands-on Jupyter notebooks exploring prompt design, LLM workflows, multimodal AI, evaluation, and optimization.**

This repository documents practical experiments with generative AI, progressing from fundamental prompting techniques to agentic workflows and automated prompt optimization.

The emphasis is on building working examples, comparing approaches, evaluating actual model outputs, and understanding their limitations.

## Topics Covered

| Area | Topics |
|---|---|
| Prompt Engineering Fundamentals | Prompt structure, instructions, context, examples, and output formatting |
| Advanced Prompting | Prompt chaining, reasoning strategies, structured outputs, and workflow design |
| LLM Applications | Function calling, multimodal inputs, and practical AI tasks |
| LangChain & LangGraph | LCEL, tool integration, stateful workflows, and human-in-the-loop agents |
| Applied AI | Classification, qualitative analysis, document summarization, and claim verification |
| Image Prompting | Text-to-image generation, structured visual prompts, and image-to-image transformation |
| Prompt Optimization & Evals | A/B testing, weighted metrics, held-out evaluation, and DSPy optimization |

## Selected Experiments

### LangChain and Agentic Workflows

- **[LangChain Fundamentals and LCEL](13_langchain_fundamentals_and_lcel.ipynb)** — Composable chains, document retrieval, and grounded responses.
- **[LangGraph AI-Driven Workflows](14_langgraph_ai_driven_workflows.ipynb)** — AI-based ticket classification, conditional routing, and checkpointing.
- **[LangGraph Agents with Human Oversight](15_langgraph_ai_agents_human_oversight.ipynb)** — Tool calling, approval interrupts, and controlled tool execution.

### Applied Prompt Engineering

- **[Qualitative Analysis and Classification](16_ai_qualitative_analysis_and_classification.ipynb)** — Theme discovery, structured classification, and reference-based evaluation.
- **[Document Summarization](17_prompt_engineering_for_document_summarization.ipynb)** — Direct versus map-reduce summarization and factual preservation.
- **[Evidence-Based Claim Verification](18_prompt_engineering_for_claim_verification.ipynb)** — Evidence grounding, supported and contradicted claims, and handling insufficient evidence.

### Multimodal Prompting

- **[Advanced Image Prompting and Editing](19_advanced_image_prompting_and_editing.ipynb)** — Stable Diffusion Turbo, structured visual prompts, subject preservation, and qualitative evaluation.

### Prompt Evaluation and Optimization

- **[Prompt Optimization and Evaluation Metrics](20_prompt_optimization_and_evaluation_metrics.ipynb)** — Baseline versus structured prompts, weighted compliance metrics, and held-out testing.
- **[Automated Prompt Optimization with DSPy](21_automated_prompt_optimization_with_dspy.ipynb)** — DSPy signatures, BootstrapFewShot, and held-out classification evaluation.

The earlier notebooks introduce the foundational concepts and workflows that support these more advanced experiments.

## Technologies

- **Language models:** Google Gemini
- **Prompting and orchestration:** LangChain, LangGraph, DSPy
- **Image generation:** Stable Diffusion Turbo, Hugging Face Diffusers
- **Development:** Python, Jupyter Notebook, Google Colab
- **Evaluation:** Custom Python metrics, structured output validation, reference labels, and human review

## Experimental Approach

The notebooks generally follow a consistent structure:

1. **Concepts** — Explain the technique and its purpose.
2. **Implementation** — Apply the technique using Python and AI models.
3. **Evaluation** — Compare outputs against explicit criteria.
4. **Findings and Limitations** — Document observed results, failures, and trade-offs.

Not every experiment demonstrates an improvement. For example, DSPy few-shot optimization matched an already-perfect classification baseline, while image-to-image editing only partially satisfied the requested transformation.

These outcomes are retained because understanding limitations is part of evaluating AI systems reliably.

## Getting Started

1. Open a notebook directly on GitHub to read its code, explanations, and saved outputs.
2. Open the notebook in **Google Colab** to execute the experiment.
3. Install the dependencies specified in the notebook.
4. Configure the required model API credentials when prompted.
5. Run the cells in order and review the generated results.

Most language-model experiments use Gemini. The Stable Diffusion notebook requires a GPU-enabled Colab runtime.

Dependencies and setup instructions are provided within individual notebooks. API keys are entered at runtime and should not be committed to the repository.

## Learning Reference

This project was developed as a hands-on learning portfolio, drawing on concepts and examples from the [BrightPool Prompt Engineering Course](https://github.com/BrightPool/udemy-prompt-engineering-course).

The notebooks adapt the learning material into individual experiments with custom examples, implementations, and evaluations.

This repository is an independent learning project and is not affiliated with the course provider.

## Final Note

Effective prompt engineering goes beyond writing detailed instructions. It requires defining expected behavior, testing actual outputs, measuring performance, and identifying where models fail.

This repository documents that process across 21 practical notebooks.
