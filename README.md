Hello 👋, this is live-in document, might be updated as you are reading this 🌎🧠

# Resources to get started with Large Language Models (LLMs)

## Table of Contents
- [Introduction](#introduction)
- [Model Context Protocol (MCP)](#model-context-protocol)
- [Types of LLMs](#types-of-llms)
- [Getting Started Resources](#getting-started-resources)
  - [Videos and Courses](#videos-and-courses)
  - [Prompt Engineering](#prompt-engineering)
  - [Frameworks](#frameworks)
  - [RAG Implementation](#rag-implementation)
- [AI Assistants](#ai-assistants)
- [Important Links](#important-links)

## Introduction
- To be clear, this is not a roadmap for `getting started` with LLMs.
- I am not covering the books you should study, university studies, certificates, etc.
- I assume you have basic understanding of NLP stuffs, programming knowledge (mainly Python and Maths).
  - You might argue, why Maths as everything is automated. Well, well, behind the scene, almost everything is Maths 🧠
  - Calculus, Probability, Linear Algebra
  - You need to know, let's say what is matrix, how dot product works, etc.
- These are some of the resources which I suggest you to get started.
- After knowing the basics and how things work, it's upon you, what to do (Or let's say if it's your cup of tea/coffee or not).
> Remember one thing, using LLMs and implementing are two different things, you need not necessarily know how to implement, but you need to know how to use it in the right way.

## Model Context Protocol
The Model Context Protocol (MCP) is an emerging standard for AI model interactions that simplifies integration compared to traditional APIs.

### Key MCP Resources
- [All about MCP](https://modelcontextprotocol.io/introduction)
- [MCP announcement from Claude](https://www.anthropic.com/news/model-context-protocol)
- [Claude for Desktop](https://claude.ai/download)
- [Claude code](https://docs.anthropic.com/en/docs/agents-and-tools/claude-code/overview)
- [Official Github MCP Servers](https://github.com/modelcontextprotocol/servers)
- [Awesome MCP Servers](https://github.com/punkeye/awesome-mcp-servers)
- [MCP server Directory](https://www.pulsemcp.com/servers)
- [What is MCP, and Why Is Everyone Suddenly Talking About It](https://huggingface.co/blog/Kseniase/mcp)

## Types of LLMs
1. Base Models
   - Foundation models trained on raw text data
   - Examples: GPT-3, LLaMA, Claude
   - Best for: Further fine-tuning, specialized tasks

2. Instruction-tuned Models
   - Fine-tuned to follow instructions
   - Examples: GPT-4, Claude 3, Gemini
   - Best for: Direct task completion, chat applications

3. Domain-specific Models
   - Specialized for particular domains
   - Examples: CodeLlama (coding), Med-PaLM (medical)
   - Best for: Industry-specific applications

### Evaluation Metrics
- Accuracy: Correctness of responses
- Perplexity: Model's confidence in predictions
- ROUGE scores: Text generation quality
- Helpful/Honest/Harmless (HHH) metrics
- Task-specific benchmarks (e.g., MMLU, GSM8K)

### Cost Considerations
- Token pricing varies by provider
- Input vs. output token costs
- Model size vs. performance tradeoffs
- Batch processing for efficiency

## Getting Started Resources

### Videos and Courses
#### Videos in Neural Networks and LLMs
- [A Hacker's Guide to Language Models](https://youtu.be/jkrNMKz9pWU?si=-PLRJrXB80E27Q_m) by Jeremy Howard.
- [[1hr Talk] Intro to Large Language Models](https://youtu.be/zjkBMFhNj_g?si=hw-BLphS85ORXL7i) by Andrej Karpathy.
- [Neural Networks: Zero to Hero](https://youtube.com/playlist?list=PLAqhIrjkxbuWI23v9cThsA9GvCAUhRvKZ&si=eTu3ESyFvq7JFdPD) by Andrej Karpathy.
- [Building RAG from scratch Using Python, LangChain and OpenAI API](https://youtu.be/BrsocJb-fAo?si=13-fYpjIBp9rmdhw) by Santiago.

#### Free Courses
- [fast.ai courses](https://www.fast.ai/) --> `Optional but highly recommended`
- [DeepLearning.AI short courses](https://www.deeplearning.ai/short-courses/) -- My request, try to complete all these free short courses.
- [DeepLearning.AI Specializations](https://www.deeplearning.ai/courses/)

### Prompt Engineering
- [Prompt Engineering Guide](https://www.promptingguide.ai/)
- [OpenAI doc about Prompt Engineering](https://platform.openai.com/docs/guides/prompt-engineering)
- [Strategies to harness the power of LLMs](https://towardsdatascience.com/how-i-won-singapores-gpt-4-prompt-engineering-competition-34c195a93d41)
- [Prompt Engineering](https://github.com/NirDiamant/Prompt_Engineering)
- There is one from deeplearning.ai free short courses too about ChatGPT Prompt Engineering for Developers.
- There are many courses, articles, videos about this topic, it needs constant learning and experimenting.

### Frameworks
#### Frameworks which I have explored until now, there are many, you can give a try (your world, your rules)
- [LangChain](https://www.langchain.com/)
  - [All you need to know about LangChain](https://youtu.be/EIejozA1W7I?si=rPBJnh7uEWVRa8ce)
- [LlamaIndex](https://www.llamaindex.ai/)
  - [All you need to know about LlamaIndex](https://youtu.be/FbQowFipEP4?si=GIZI73RzJZy1B_cj)

### RAG Implementation
#### Make RAG work properly
- First, think on tweaking basic stuffs
    - Cleaning document (choose right parsing, e.g., LlamaParse, Unstructured)
    - Better Chunking strategies
    - Choosing right embeddings model
    - Choosing right Vectorstore
    - Passing parsing Instructions, Reranking
    - Choosing right Large Language Models

#### Vector Database Comparison
- Pinecone: Fully managed, production-ready
- Weaviate: Open-source, scalable
- Chroma: Lightweight, easy setup
- Milvus: High performance, distributed
- pgvector: PostgreSQL extension

#### Popular Embedding Models
1. OpenAI
   - text-embedding-3-small
   - text-embedding-3-large
2. Cohere
   - embed-english-v3.0
   - embed-multilingual-v3.0
3. Open Source
   - all-MiniLM-L6-v2
   - bge-large-en-v1.5

#### RAG Evaluation Metrics
- Retrieval Precision/Recall
- Answer Relevance
- Context Utilization
- Latency and Performance
- Hallucination Rate

Links to follow for better understanding:
- [Chunk visualizer](https://huggingface.co/spaces/m-ric/chunk_visualizer)
- [Tokenizer, from OpenAI](https://platform.openai.com/tokenizer)
- [Huggingface Massive Text Embedding Benchmark (MTEB) Leaderboard](https://huggingface.co/spaces/mteb/leaderboard)
- [What is a Vector Database & How Does it Work? Use Cases + Examples](https://www.pinecone.io/learn/vector-database/)
- [Chunking Strategies for LLM Applications](https://www.pinecone.io/learn/chunking-strategies/)
- [🤗 Open LLM Leaderboard](https://huggingface.co/spaces/HuggingFaceH4/open_llm_leaderboard)
- [🏆 LMSYS Chatbot Arena Leaderboard](https://chat.lmsys.org/)
- [12 RAG Pain Points and Proposed Solutions](https://towardsdatascience.com/12-rag-pain-points-and-proposed-solutions-43709939a28c)
- [Optimizing RAG with Hybrid Search & Reranking](https://superlinked.com/vectorhub/optimizing-rag-with-hybrid-search-and-reranking)
- [Improving RAG performance with Knowledge Graphs](https://superlinked.com/vectorhub/improving-rag-performance-with-knowledge-graphs)
- [Enhancing RAG with a Multi-Agent System](https://superlinked.com/vectorhub/enhancing-rag-with-a-multi-agent-system)

## AI Assistants (Remember, personal use or enterprise use)
- [Perplexity AI](https://perplexity.ai/pro?referral_code=YAWB6JNV) --> let's put this way, it's Google Search with LLMs with it.
- [Perplexity Labs, For Open Source models](https://labs.perplexity.ai/)
- [ChatGPT](https://chat.openai.com/) --> Based on your need, free or paid version. (Team, Enterprise, etc.)
- [Bing Chat](https://www.bing.com/search?q=Bing+AI&showconv=1&FORM=hpcodx), Bing Enterprise.
- [Hugging Chat](https://huggingface.co/chat/)
- [Le Chat Mistral](https://chat.mistral.ai)

## Important Links
### Updated (22 August 2024)
- [Llama-3-Groq-Tool-Use Models](https://wow.groq.com/introducing-llama-3-groq-tool-use-models/)
- [Berkeley Function Calling Leaderboard](https://gorilla.cs.berkeley.edu/leaderboard.html#leaderboard)
- [Independent analysis of AI models and API providers](https://artificialanalysis.ai/) :pushpin:

### Updated (02 September 2024)
#### AWS
- [Evaluating RAG applications with Amazon Bedrock knowledge base evaluation](https://aws.amazon.com/blogs/machine-learning/evaluating-rag-applications-with-amazon-bedrock-knowledge-base-evaluation/)
- [AWS Samples](https://github.com/aws-samples)

#### Microsoft
- [LangChain Azure Integration](https://devblogs.microsoft.com/azure-sql/langchain-with-sqlvectorstore/)
- [RAG vs Agentic RAG](https://www.analyticsvidhya.com/blog/2024/11/rag-vs-agentic-rag/)
- [Comprehensive Guide in RAG Implementation](https://newsletter.armand.so/p/comprehensive-guide-rag-implementations)

#### RAG and Agents
- [RAG_Techniques](https://github.com/NirDiamant/RAG_Techniques)
- [GenAI Agents](https://github.com/NirDiamant/GenAI_Agents)

#### General
- [2024 AI Timeline Huggingface Space](https://huggingface.co/spaces/reach-vb/2024-ai-timeline)

### LLM Docs
- [Anthropic Docs](https://docs.anthropic.com/en/home)
- [OpenAI Docs](https://platform.openai.com/docs/overview)

> Cheers !!
Last Updated: May 2024