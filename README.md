# EXP-3-PROMPT-ENGINEERING-

## Aim: 
Evaluation of 2024 Prompting Tools Across Diverse AI Platforms: 
ChatGPT, Claude, Bard, Cohere Command, and Meta
Experiment:
Within a specific use case (e.g., summarizing text, answering technical questions), compare the performance, user experience, and response quality of prompting tools across these different AI platforms.

## Algorithm:

Step	ChatGPT (GPT-4o/5)	Claude (3.5/4)	Bard (Gemini 1.5 Pro)	Cohere Command R+	Meta AI (LLaMA 3)
1. Input Parsing	Tokenizes input with advanced attention tuning for user tone and metadata	Strong parsing with emphasis on safety and coherence	Breaks down input and uses contextual memory across sessions	Extracts entities and structure via RAG preprocessing	Token-based parsing with core focus on safety alignment
2. Intent Inference	Uses reward model for goal inference (summarization → simplification)	Infers emotional intent + topic-specific purpose	Matches intent with search-injected context if available	Maps to summarization pipeline with domain detection	Maps to meta-prompted structure (task → action plan)
3. Context Expansion	Embeds the text, compares against internal memory + prompt	Embeds input into knowledge graph + summary modules	Applies context-widening via search + Gemini Pro knowledge	RAG pipeline expands with citation candidates	Aligns with model’s training metadata + output goal
4. Output Generation	Multi-stage decoding, with beam search & temperature tuning	Controlled decoder output with high grammar + clarity	Real-time generation with self-checks for contradictions	Outputs fact-based summary with tool-injected citations	Decodes based on modular prompt routing (e.g., “summarizer” head)
5. Quality Filter	Ranked outputs pass through RLHF filters and safety guardrails	Passes empathy/safety classifiers and clarity checks	Filtered through safety + style models	Validated through citation cross-checks	Reinforcement-augmented filters ensure safe phrasing
## Prompt:
“Summarize this scientific text for a high schooler:
‘The Higgs boson is a fundamental particle associated with the Higgs field, a field that gives mass to other particles. It was confirmed by the Large Hadron Collider in 2012. Without the Higgs field, particles like protons and neutrons wouldn’t have mass, and atoms couldn’t form.’”

## Output:

Here’s a refined evaluation comparing prompting tools across ChatGPT, Claude, Bard, Cohere Command, and Meta’s AI (e.g., LLaMA-based models), focused on use cases like summarization, technical Q&A, and creative generation:

ChatGPT (e.g., GPT‑4o / GPT‑5)
Strengths

Versatile and practical: ChatGPT excels in creative writing, planning, and practical tasks—think vivid storytelling, structured travel or meal plans, and actionable brainstorming 
Tom's Guide
.

Speed and accessibility: Interface is intuitive, load times are light, and integration with plugins, multimodal features (like DALL·E, Custom GPTs, Canvas), and data analysis make it a flexible, creative workhorse 
Knack
eWeek
.

High performance on reasoning benchmarks: ChatGPT (4o/5) often matches or slightly exceeds Claude on MMLU and coding benchmarks like HumanEval (around 90% pass rate) 
Data Studios ‧Exafin
Tom's Guide
.

Strong in math/calculus: Particularly effective at procedural differentiation tasks (94.7% success in a 2025 study) 
arXiv
.

Limitations

Shorter context window compared to Claude (128K vs. 200K tokens) 
Kowalah
.

Can feel formulaic or "sterile" in style, especially for creative prose 
BytePlus
.

Less emotional nuance: Often overshadowed by Claude in emotional intelligence or structured reasoning depth 
Tom's Guide
+1
.

Claude (Anthropic, e.g., Claude 3.7 Sonnet, Claude 4)
Strengths

Deep reasoning & emotional nuance: Prized for empathy, structure, and clarity in complex or emotional tasks—winning evaluations in reasoning, summarization, and EQ 
Tom's Guide
+2
Tom's Guide
+2
The Washington Post
.

Huge context window: Handles up to 200K tokens, excellent for long documents, summarization, or coding across large files 
Kowalah
hothandmedia.com
.

Coding and documentation: Claude Code and Opus versions integrate with IDEs, deliver in-depth explanations, robust debugging, and handle multi-file codebases well 
Neontri
The Verge
.

Controlled interface & artifacts: Features like “Artifacts” to isolate structured outputs (code, docs) add clarity 
Knack
Writesonic
.

Broad user acclaim: Developers frequently describe Claude’s coding as more accurate, polished, and intuitive than ChatGPT 
Reddit
+2
Reddit
+2
.

Limitations

Slower or limited in high-demand periods; users note lags or usage caps 
Reddit
+1
.

Cost and usage limits: Paid tiers offer higher throughput but still capped compared to ChatGPT 
Reddit
eWeek
.

Less creative flair: While structured and precise, Claude’s imaginative expression may lag behind ChatGPT’s vivid prose 
Tom's Guide
Get Prompting
.

Google Bard (including Gemini under the hood)
Strengths

Creative brainstorming: Users report Bard shines in imaginative prompts, names, high-level lists, and creative flow 
Reddit
.

Integrated search capabilities: Real-time web integration aids factual tasks, especially in detail-oriented queries 
Reddit
.

Educational tools: Gemini Advanced allows editing and running Python code inline—useful for learning and verification 
Reddit
.

Clinical use: In medical decision tasks, ChatGPT and Bard perform similarly for open-ended prompts, though ChatGPT edged ahead on multi-select formats (83% vs. 70%) 
ScienceDirect
.

Limitations

Inconsistency in depth: Some users feel the analysis lacks depth or feels surface-level—“basic and bland” outputs reported post-updates 
Reddit
.

Erratic refusal behaviors: Some prompts trigger overly cautious refusals, limiting creative or harmless engagement 
Reddit
+1
.

Cohere Command (R / R+ / Command A)
Strengths

Enterprise-grade RAG and tool use: Command R+ excels in retrieval-augmented generation with accurate citations and seamless integration of tools (calculators, modules) 
TIME
metaailabs.com
SuperAnnotate
.

High benchmark scores with efficiency:

Command R+: ~88% on MMLU; nearly GPT-4 level but at much lower compute cost 
theregularizer.com
Business Insider
.

HumanEval: ~71–72% pass rate, solid and comparable to Claude’s ~72.6% 
theregularizer.com
.

Tool benchmarks (ToolTalk, function calling) show performance on par or exceeding GPT‑4/Turbo and Claude 3 
theregularizer.com
.

Command A (2025): Newest model, 111B parameters, 256K context window, blazing-fast performance (156 tokens/s), supports 23 languages, deployable on just two GPUs, strong in agentic RAG tasks 
Venturebeat
+1
Som2ny Network
Reddit
arXiv
.

Community praise: Users describe R+ as deep, insightful ("mature"), and high-quality—especially remarkable for being fine-tuned and affordable 
Reddit
.

Limitations

Mixed visibility & licensing constraints: R+ hasn't seen widespread coverage, and commercial use licensing can be restrictive 
Reddit
.

Some user disappointment: A few users expected R+ to outperform GPT-4 but were underwhelmed in certain creative tasks 
Reddit
.

Meta AI (e.g., LLaMA 3.1, Meta AI)
Strengths

Strong benchmarks: LLaMA 3.1 (405B parameter) reportedly outperforms GPT‑4o on several benchmarks and features Tool use capability, safety enhancements 
Reddit
.

Academic clarity: In calculus exams, Meta AI trailed others: ChatGPT (~94.7%), Claude (~85.7%), Meta (~56.8%) 
arXiv
.

Prompting research: Meta in academic circles runs meta‑prompting frameworks that enhance model breakdown of tasks—improving standard prompting by ~17%+ 
arXiv
+1
.

Limitations

Less real-world UX data: Fewer firsthand user reports on prompting effectiveness compared to ChatGPT and Claude.

Weaker in math tasks per academic evaluation
<img width="1580" height="1180" alt="image" src="https://github.com/user-attachments/assets/41c5ec66-589d-41a2-82c2-f46617ab2aba" />
<img width="1580" height="1180" alt="image" src="https://github.com/user-attachments/assets/9d384739-5726-4f24-9173-3b00012cc15f" />


## Result:

ChatGPT: Top performer for polished, friendly summaries.

Claude: Best at structured, emotionally aware simplifications.

Bard (Gemini): Great for quick, easy explanations, especially for younger users.

Cohere: Excels in fact-based, tool-augmented summaries with citations.

Meta AI: Basic but efficient—ideal in low-resource or embedded settings.

