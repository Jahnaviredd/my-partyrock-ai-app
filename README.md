# 🎯 AI Marketing Captions Generator

A serverless Generative AI application built on the **AWS PartyRock** platform, leveraging foundation models via **Amazon Bedrock**. This tool automates social media copywriting by generating platform-optimized captions tailored to specific product descriptions, target demographics, and brand voices.

## 🔗 Live Application
* **Try the Live App:** [AWS PartyRock - Marketing Captions Generator](https://partyrock.aws/u/jahnavi-tirupathi/JvqC_Ixcd/Marketing-Captions-Generator)
**View App Snapshot:** [Click Here to See an Example Run](https://partyrock.aws/u/jahnavi-tirupathi/JvqC_Ixcd/Marketing-Captions-Generator/snapshot/KjOX6fwU0)
---

## 💡 Project Overview
Digital marketers and content creators often spend hours tailoring a single promotional message across multiple social media networks. This application eliminates that friction by providing a unified interface that accepts core marketing parameters and processes them concurrently to produce platform-specific, high-converting copy.

### Core Features:
* **Multi-Channel Adaptation:** Creates custom outputs for platforms with drastically different character limits, cultures, and formatting styles (e.g., professional LinkedIn posts vs. punchy, viral X/Twitter threads).
* **Context-Aware Formatting:** Intelligently incorporates relevant hashtags, emojis, and visual structural hierarchies (like hooks and bullet points) based on the target channel.
* **Variable Dynamic Mockups:** Allows users to test how a shift in brand voice completely changes the generated narrative.

---

## 🛠️ App Architecture & Prompt Engineering

As a cloud-hosted, no-code application, the "source code" consists of system architecture, interface layout, widget chaining logic, and advanced prompt engineering.

### 📥 1. User Input Widgets
* `Product / Service Details`: A rich text area capturing what is being marketed, its unique selling propositions (USPs), and features.
* `Target Audience`: Defines the primary demographic (e.g., B2B Executives, College Students, Tech Enthusiasts).
* `Brand Tone`: Instructs the AI on the narrative style (e.g., Bold, Friendly, Witty, Informative, Professional).

### ⚙️ 2. Core Processing Engines & System Prompts

#### 🔹 Platform Output: LinkedIn
* **Objective:** Professional networking alignment. Focuses on thought-leadership hooks, bold structuring, value-adds, and strategic industry tags.
* **Prompt Injection Logic:**
  > *"You are a senior B2B growth marketer. Analyze the product details: `{{Product / Service Details}}`. Write an authoritative LinkedIn post targeted directly at `{{Target Audience}}`. Use a `{{Brand_Tone}}` tone. Structure it with a compelling first line hook, 3 key bullet points for clarity, a distinct Call to Action (CTA), and 3-5 relevant professional hashtags."*

#### 🔹 Platform Output: Instagram
* **Objective:** Visual and emotional engagement. Focuses on high-energy copy, seamless emoji placement, and lifestyle-oriented hashtag clouds.
* **Prompt Injection Logic:**
  > *"You are an expert social media manager. Generate an engaging Instagram caption for the product: `{{Product / Service Details}}`. The copy must resonate with `{{Target_Audience}}` and maintain a `{{Brand_Tone}}` voice. Keep lines short, inject contextual emojis at the start of paragraphs, insert a strong CTA to click the link in bio, and separate a block of 5-7 trending hashtags at the absolute bottom."*

#### 🔹 Platform Output: X (Formerly Twitter)
* **Objective:** Micro-copy optimization. Focuses on extreme character constraints, stopping user scrolls, and maximizing click-through potential.
* **Prompt Injection Logic:**
  > *"You are a viral growth hacker. Condense the core essence of `{{Product / Service Details}}` into a punchy, single-tweet format. Ensure it stays strictly under 280 characters, speaks directly to `{{Target_Audience}}`, reflects a `{{Brand_Tone}}` persona, and relies on an intense hook without fluff."*

---

## 🚀 Key Takeaways & Skills Demonstrated

* **Prompt Engineering & Interpolation:** Mastered the use of bracketed variables (`{{Widget}}`) to orchestrate state and pass data between asynchronous interface layers.
* **AI Product Design:** Conceptualized a real-world tool matching practical SaaS business requirements with user-friendly cloud UI patterns.
* **LLM Capability Mapping:** Evaluated foundation model outputs via Bedrock to balance creative flair, factual adherence, and strict formatting constraints.
