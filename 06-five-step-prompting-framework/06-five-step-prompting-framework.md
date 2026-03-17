# Google Prompting Essentials: Comprehensive Summary
**Source:** Google Prompting Essentials Specialization (Google & Coursera)
**Compiled by:** dlastnoel (with DTI La Union sponsorship)
**Last Updated:** February 2026
**Program Duration:** Under 10 hours (self-paced)

---

## Program Overview

Google Prompting Essentials teaches how to give clear and specific instructions to generative AI—known as **prompting**. The program covers practical applications across industries with no prior experience required.

### What You'll Learn
- Save time: Craft emails, brainstorm, build tables/trackers, summarize documents
- Uncover insights: Identify patterns, create visualizations, rehearse presentations
- Tackle complex projects: Transform abstract ideas into actionable steps
- Use AI responsibly: Evaluate outputs for bias and errors, iterate for better results

### Program Structure

| Module | Title | Focus |
|--------|-------|-------|
| I | Start Writing Prompts like a Pro | TCREI Framework, iteration, multimodal prompting, responsible AI |
| II | Design Prompts for Everyday Work Tasks | Tone/style, writing, summarization, Gemini for Workspace |
| III | Speed Up Data Analysis and Presentation Building | Data analysis, spreadsheets, visualization, sampling parameters |
| IV | Use AI as a Creative or Expert Partner | Prompt chaining, meta-prompting, AI agents |

---

# MODULE I: Start Writing Prompts like a Pro

## The TCREI Prompting Framework

**Mnemonic:** "Thoughtfully Create Really Excellent Inputs"
```
T - Task
C - Context
R - References
E - Evaluate
I - Iterate
```

This framework provides clear and specific directions to ANY generative AI tool, regardless of platform.

---

### T — Task

**Definition:** The action or objective you want the gen AI tool to accomplish.

**Key principle:** Be clear and specific. Vague instructions = bad results.

#### Task Components

| Component | Description | Example |
|-----------|-------------|---------|
| **Action** | What you want done | Write, draft, create, summarize, explain |
| **Persona** | Role the AI should take | "You're a science expert..." |
| **Format** | Structure of output | Bulleted list, table, paragraph, 100 words |

#### Example Prompt with Task Components

**Basic:** "Write a list."

**Enhanced:** "You're a movie critic that specializes in Italian film. Create a table that contains the greatest Italian films of the 1970s, and separate them into genres like thrillers, dramas, and comedies. Provide a 100-word summary of each movie as well as details about the production including director and release year."

---

### C — Context

**Definition:** Background information, details, or guidelines that inform the AI's output.

**Key principle:** The more relevant details you include, the better your output will be.

#### What Context Provides
- Your goals
- The reason for the task
- What you've tried before
- Audience information
- Constraints or requirements

#### Example: Context in Action

**Without context:** "How was DNA discovered?"

**With context:** "You're a science expert developing a new curriculum at a local college. Tell me in a couple of engaging paragraphs how DNA was discovered and what kind of impact it had on the world. Write it in a way that people unfamiliar with science would understand. You have gotten feedback from students that they found this course dry and unintelligible before, so you want to make sure that the explanation grabs the students' attention and makes a good first impression."

**Pro tip:** Context has the potential to be the longest piece of a prompt.

---

### R — References

**Definition:** Examples or additional resources that guide an AI tool towards the output you want.

**Key principle:** Clearly label and structure your references so the tool knows exactly what they are and how to use them.

#### Best Practices for Structuring References

| Technique | Description | Example |
|-----------|-------------|---------|
| **Transitional phrases** | Signal upcoming reference | "Refer to these materials," "Use the following examples" |
| **Headings** | Label different types of references | "Sunglasses:", "Cardholder:" |
| **XML-style tags** | Mark beginning and end of each piece | `<example01>` ... `</example01>` |
| **Markdown tags** | Add formatting | `_italics_`, `**bold**` |

#### Reference Quantity
- 2 to 5 references should be enough
- No need to build an exhaustive set

#### Example: Using References
```
Prompt: Write a one-paragraph product description for a high-end watch with features 
like a scratch-resistant case and a water resistance rating of up to 30 meters. 
Base the description style on these examples from our website:

Sunglasses: Our latest collection of handcrafted, heritage-inspired sunglasses 
features details like UV-protective lenses in shades specifically chosen to 
complement each frame...

Cardholder: Crafted in smooth Italian leather, this double-sided cardholder is 
designed to carry your cash and credit cards without the bulk of a full wallet...
```

---

### E — Evaluate

**Definition:** Critically assessing an output before using it.

**Key principle:** Different AI models produce different results. The same prompt run multiple times may render different results.

#### Evaluation Criteria

| Criterion | Question to Ask |
|-----------|-----------------|
| **Accurate** | Is the information correct and factual? |
| **Unbiased** | Does it avoid stereotypes or unfair assumptions? |
| **Relevant** | Does it address what you asked for? |
| **Consistent** | Does it align with context provided? |
| **Sufficient** | Does it fully address the task? |

**Critical reminder:** Always evaluate outputs before using them in your work.

---

### I — Iterate

**Definition:** Clarifying and refining your prompt to better direct the AI tool towards the desired result.

**Key principle:** "Always Be Iterating" (ABI) — If an output is lacking, continue clarifying until it's just right.

**Important:** Iterate in the same chat so the tool can reference previous information.

#### Four Iteration Methods

| Method | Description | When to Use |
|--------|-------------|-------------|
| **Revisit the framework** | Ensure prompt includes task, persona, format, context, references | Output is too broad or unfocused |
| **Break into shorter prompts** | Address each step in a separate prompt | Complex tasks that overwhelm |
| **Tweak phrasing / analogous task** | Explain differently or try a similar task | Output misses the point |
| **Introduce constraints** | Add specific limitations | Output lacks precision |

#### Iteration Example: Introducing Constraints

**Before:** "Create a bulleted list including the latest developments in the restaurant industry specific to urban areas..."

**After:** "Create a bulleted list including the latest developments in the restaurant industry specific to urban areas... This list should only include trends from cities with a population of more than 500,000 people, and should only include trends relevant to vegetarian and vegan restaurants."

---

## TCREI Framework Visual Summary
```
┌─────────────────────────────────────────────────────────────┐
│                    TCREI FRAMEWORK                          │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│   ┌─────────┐    ┌─────────┐    ┌────────────┐             │
│   │  TASK   │ → │ CONTEXT │ → │ REFERENCES │             │
│   └─────────┘    └─────────┘    └────────────┘             │
│        │              │               │                     │
│        ▼              ▼               ▼                     │
│   ┌─────────────────────────────────────────┐              │
│   │              INPUT TO AI                 │              │
│   └─────────────────────────────────────────┘              │
│                        │                                    │
│                        ▼                                    │
│   ┌─────────────────────────────────────────┐              │
│   │               OUTPUT                     │              │
│   └─────────────────────────────────────────┘              │
│                        │                                    │
│            ┌───────────┴───────────┐                       │
│            ▼                       ▼                       │
│      ┌──────────┐           ┌──────────┐                   │
│      │ EVALUATE │ ────────→ │ ITERATE  │ ──┐              │
│      └──────────┘           └──────────┘   │              │
│            ▲                               │              │
│            └───────────────────────────────┘              │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

---

## Multimodal Prompting

**Definition:** Using multiple modalities (text, image, audio) in the same prompt.

### Benefits
- Reflects how humans experience the world
- Builds connections between different formats
- Provides clearer instructions to AI tools
- Enables transfer of information between media

### Multimodal Prompting Examples

| Scenario | Input | Output |
|----------|-------|--------|
| Recipe suggestions | Photo of fridge ingredients | Recipe list |
| Event promotion | Two brand logos + colors | Joint event visual |
| Story writing | Audio recording of forest | Atmospheric descriptions |
| Poem writing | Photo of sunset | Vivid, specific poem |

### Limitations
- AI may struggle with abstract ideas
- Complex combinations can be challenging
- Counting isn't reliable yet
- Not all tools support all modalities

### Adapting TCREI for Multimodal Prompts

| Component | Multimodal Consideration |
|-----------|-------------------------|
| **Task** | Be specific about how each modality should be used |
| **Context** | Consider constraints specific to each modality |
| **References** | Use visual or audio references (if tool supports) |
| **Evaluate** | Take extra care with how output looks or reads |
| **Iterate** | Use the four iteration methods as usual |

---

## Responsible Prompting

### Why It Matters
Gen AI tools are great at processing information and recognizing patterns but **lack critical-thinking skills and human awareness**.

### Ethical Risks and AI Limitations

#### 1. Biases and Stereotypes

**Problem:** AI can reproduce existing biases (ageism, racism, genderism).

**Solutions:**
| Strategy | Example |
|----------|---------|
| **Specify diversity** | "A table of delicious foods from all over the world" instead of "a table of delicious foods" |
| **Challenge assumptions** | Point out bias when iterating: "Include more food from West Africa or Northern Europe" |

---

#### 2. Hallucinations

**Definition:** When a gen AI tool provides an output with false information.

**When they occur:**
- Vague or unclear instructions
- Topics AI hasn't been trained well on
- Math calculations
- Specific factual details

**Solutions:**
| Strategy | How to Apply |
|----------|--------------|
| **Fact-check** | Use search engines to confirm information |
| **Cross-reference** | Run prompt through 2+ resources |
| **Use clearer language** | Avoid incorrect premises in prompts |
| **Consult experts** | When available |

**Example of problematic prompt:** "Why is Toronto the capital of Canada?" → AI may give false history instead of correcting the premise.

---

#### 3. Inconsistencies and Relevance Issues

**Problem:** AI may misinterpret idioms or colloquial phrases literally.

**Example:** "Think outside the box" → AI might suggest solutions about the outsides of boxes.

**Solutions:**
- Provide references
- Rephrase prompt (e.g., "consider unique, unconventional approaches")

---

### Responsible Prompting Checklist for Work

| ✓ | Consideration |
|---|---------------|
| □ | Consider effects of using AI — is it right for this task? |
| □ | Get approval from appropriate people before using on projects/clients |
| □ | Consider privacy and security implications |
| □ | Evaluate all AI-generated content before incorporating |
| □ | Disclose your use of AI to team and clients |

### Human-in-the-Loop Approach

**Definition:** A human verifies a gen AI tool's outputs before they are used anywhere.

**Key principle:** This must be at the forefront of how you use AI—at home, at work, or anywhere else.

---

### Clearing Memory

**Benefits of periodically clearing AI memory:**
- Protects privacy
- Avoids bias carryover
- Reduces confusion
- Troubleshoots stuck outputs

**Note:** Some tools automatically clear memory each session.

---

# MODULE II: Design Prompts for Everyday Work Tasks

## Prompting for Tone and Style

### How AI Handles Tone and Style: Contextual Understanding

**Definition:** Allows a gen AI tool to interpret information in a specific setting and use that comprehension to generate an output.

**What contextual understanding enables:**
- Identify audiences
- Recognize linguistic cues (question marks, etc.)
- Learn language from provided references
- Adapt to user preferences
- Stay consistent in language use

---

### Strategies for Tone and Style

#### 1. Specify Your Tone and Style

**Basic:** "Summarize this report into three short paragraphs."

**Enhanced:** "Summarize this report into three short paragraphs in a friendly, professional, and easy-to-comprehend tone."

#### Tone Descriptors (General → Specific)

| General | More Specific Alternative |
|---------|--------------------------|
| Humorous | "Witty banter" |
| Casual | "Like talking to a friend" |
| Academic | "Scholarly and in-depth, like a professor" |
| Persuasive | "Compelling and convincing" |
| Sarcastic | "Dryly funny, like a wry comedian" |
| Inspirational | "Motivating and uplifting" |
| Simple | "Like a kindergarten teacher explaining to students" |

**Pro tip:** Add constraints like "avoid using jargon that would be confusing to people who are unfamiliar with the subject."

---

#### 2. Provide Tone and Style References

**Example prompt with reference:**
```
Help me draft a description for a new line of rock climbing apparel. The target 
audience is young outdoor enthusiasts and climbers. I want the description to speak 
to the audience's desire for durable, attractive rock climbing apparel for indoor 
and outdoor climbing. Keep the language upbeat, informative, and inspiring. Imagine 
you're talking to a friend who's an avid rock climber.

Consider the tone and style of interviews with history's most renowned climbers 
as a reference.
```

---

#### 3. Iterate on Tone and Style

**Iteration example:**
```
I need this product line description to speak to the heart of young climbers of all 
kinds. I want to evoke their passion for pushing limits both indoors and out. The 
shirts, jackets, pants, shorts, tanks, and carabiners enable climbers to express 
their personal style without sacrificing quality, comfort, or durability. Channel 
the spirit of climbing legends, and inspire them to reach new heights. Make the 
language less cheeky and more reverent of the sport.
```

---

## Gemini for Google Workspace Applications

| App | Capabilities |
|-----|-------------|
| **Gmail** | Draft emails, refine existing drafts, adjust tone |
| **Google Docs** | Generate new text, refine existing work, writing assistance |
| **Google Sheets** | Track/organize data, fill cells, format tables, create templates |
| **Google Slides** | Generate custom images, create presentations |
| **Google Meet** | Custom backgrounds, video/audio quality, translated captions |
| **Google Drive** | Summarize and analyze materials across apps |

---

## Summarization Best Practices

### Adapting TCREI for Summarization

| Component | Summarization Application |
|-----------|--------------------------|
| **Task** | Specify content to summarize, format (bullets/paragraphs), length, tone, reading level |
| **Context** | Add what the summary is for, why you're creating it |
| **References** | Include example summaries + their source documents |
| **Evaluate** | Cross-reference output; consult subject matter experts |
| **Iterate** | Adjust format, length, or specific details |

---

### Long Context Windows

**Definition:** Allows gen AI tools to process large amounts of information in different formats at once.

#### Understanding Tokens

**Definition:** Fundamental building blocks of text that AI models use to process language.

| Aspect | Description |
|--------|-------------|
| Size | Can be a character, part of a word, or multiple words |
| Early models | Several thousand tokens |
| Current models | Can process millions |

#### Benefits of Long Context Windows
- Share more context and background in single input
- Complete complex tasks with nuanced details
- Process lengthy PDFs, reports, spreadsheets
- AI "remembers" earlier parts of conversation

**Note:** Memory typically only persists within the same conversation thread.

---

# MODULE III: Speed Up Data Analysis and Presentation Building

## Strategies for Data Analysis

### Types of Data Analysis AI Excels At

| Type | Description | Example |
|------|-------------|---------|
| **Text analysis** | Surface themes, determine tone, classify topics | Analyzing survey responses |
| **Data augmentation** | Expand limited datasets with simulated data | Fraud prevention patterns |
| **Question & answering** | Get answers in plain language | "Were Q3 sales up or down?" |
| **Scenario analysis** | Predict outcomes based on patterns | Traffic impact on commute |
| **Image/visual analysis** | Identify patterns in visual data | Analyzing charts and graphs |
| **Customer/market research** | Analyze surveys, social media, industry data | Understanding customer wants |

---

### Data Quality Checklist

Before entering data into a gen AI tool, ensure data is:

| ✓ | Quality Criterion |
|---|-------------------|
| □ | Up to date |
| □ | Accurate |
| □ | Complete |
| □ | Consistent |
| □ | Relevant |
| □ | Bias-free |

**Pro tip:** Use AI to help clean data:
```
Here's a sample of my data. Identify any potential issues or inconsistencies 
in the data, and suggest ways that I can address them.
```

---

### Encouraging Data Exploration

**Strategy:** Ask broad, open-ended questions to let AI identify unexpected patterns.

**Example prompt:**
```
You're a journalist investigating housing trends. How would you use this vacant 
property data to tell a compelling story about the real estate market?
```

---

## Using AI to Decipher Content

### Applications

| Task | Example Prompts |
|------|-----------------|
| **Translate** | "Translate this email to Spanish..." |
| **Define terms** | "What does 'hygge' mean in English?" |
| **Interpret jargon** | "What is compound interest in simple terms?" |
| **Explain formulas** | "Explain the formula in cell B12 in three sentences..." |
| **Identify errors** | "Are there any inconsistencies in this data?" |
| **Troubleshoot** | "My computer says 'Kernel Panic.' How can I fix this?" |
| **Explain code** | "What does this Python code do? Explain for a beginner..." |
| **Summarize trends** | "What are the main trends shown in this line graph?" |

---

## Sampling Parameters

**Definition:** Variables that expand or limit the pool of data AI chooses from.

### The Three Main Parameters

#### 1. Temperature (Creativity Dial)

| Setting | Effect | Best For |
|---------|--------|----------|
| **Low** (0.1–0.4) | Predictable, consistent | Factual tasks, summarizing, code |
| **High** (0.8–1.0) | Creative, unexpected | Brainstorming, creative writing |

**Example:** "This morning, I went to the..."
- Low temperature → "grocery store" (most likely)
- High temperature → "haunted house" or "moon" (surprising)

---

#### 2. Top-K (Fixed Word Pool)

**Definition:** Sets a fixed number of words AI can choose from.

**Example:** Top-K = 10 → Only considers top 10 most likely options.

---

#### 3. Top-P (Dynamic Word Pool)

**Definition:** Sets a dynamic number of words based on probability.

**Example:** Top-P = 0.9 → Considers words until cumulative probability reaches 90%.

**Pro tip:** When using Top-P, leave Top-K at default.

---

### Recipes for Success

| Recipe | Task Type | Temperature | Top-P/Top-K |
|--------|-----------|-------------|-------------|
| **Focused Analysis** | Factual, consistent, predictable | Low (0.1–0.4) | Default |
| **Creative Brainstorming** | Surprising, diverse, innovative | High (0.8–1.0) | High (0.95 for Top-P) |

**Warning:** High settings increase hallucination risk—always fact-check.

---

# MODULE IV: Use AI as a Creative or Expert Partner

## Prompt Chaining

**Definition:** Taking the output of one prompt and using it as context for a new prompt.

**Key principle:** Breaking complex tasks into smaller, interconnected tasks maintains human-in-the-loop oversight.

### Prompt Chaining Example: Onboarding Course
```
Prompt 1: Generate outline → Output: 7-point outline

Prompt 2: Expand bullet #2 into paragraph → Output: 100-word paragraph

Prompt 3: Create quiz from paragraph → Output: 3-question quiz

Prompt 4: Generate congratulations graphic → Output: Visual image
```

**Visual representation:**
```
┌──────────────────┐
│ Generate outline │
└────────┬─────────┘
         │
         ▼
┌──────────────────┐     ┌─────────────────────┐
│ Expand section   │────→│ Create quiz         │
│ into paragraph   │     └─────────────────────┘
└────────┬─────────┘              │
         │                        ▼
         │              ┌─────────────────────┐
         └─────────────→│ Generate image      │
                        └─────────────────────┘
```

---

## Advanced Prompt Chaining Techniques

### 1. Chain-of-Thought Prompting

**Definition:** Asking AI to retrace its path from input to output, listing reasoning step by step.

**Trigger phrases:**
- "Explain your reasoning"
- "Go step by step"
- "Walk me through your thinking"

**Example:**
```
Draft a paragraph of approximately 100 words detailing the major duties and 
responsibilities of a new entry-level design hire at an ad agency. 
Explain your reasoning step by step.
```

**Output structure:**
```
Reasoning:
- Step 1: Identify Core Responsibilities
- Step 2: Highlight Essential Skills
- Step 3: Emphasize Collaboration
- Step 4: Address Industry Standards

Paragraph: [Final output]
```

**Use case:** Troubleshoot why AI reached a particular conclusion; redirect from a specific step.

---

### 2. Tree-of-Thought Prompting

**Definition:** Exploring multiple possible solutions at once.

**How it works:**
1. Generate several responses to prompt
2. Evaluate and choose best ones to pursue
3. If one doesn't work, return to previous branch
4. Continue until finding best solution

**Example prompt:**
```
Imagine three different designers are pitching their design to me.

All designers will write down one step of their thinking, then share it with 
the group. Then all experts will go on to the next step, etc. If any expert 
realizes they're wrong at any point, then they leave.

The question is: Generate an image that's visually energetic, and features 
images of art supplies and computers. Show me three suggestions in very 
different styles from simple to detailed and complex.
```

**Visual representation:**
```
                    ┌─────────┐
                    │ Prompt  │
                    └────┬────┘
           ┌─────────────┼─────────────┐
           ▼             ▼             ▼
       ┌───────┐    ┌───────┐    ┌───────┐
       │Style 1│    │Style 2│    │Style 3│ ← Choose best
       └───┬───┘    └───────┘    └───────┘
           │
    ┌──────┼──────┐
    ▼      ▼      ▼
┌──────┐┌──────┐┌──────┐
│Var A ││Var B ││Var C │ ← Choose best
└──────┘└──────┘└──────┘
                    │
                    ▼
              ┌──────────┐
              │  OUTPUT  │
              └──────────┘
```

---

## Meta-Prompting

**Definition:** Using gen AI to help you craft or improve your prompts.

**Also called:** "Automatic prompt engineering"

### Prompt Generation Strategies

| Strategy | Use Case | Example |
|----------|----------|---------|
| **Direct generation** | Generate prompt from scratch | "Generate a prompt that could help write a job offer letter" |
| **Template request** | Get outline for prompt structure | "Create a template specifying the most important elements of a prompt meant to plan travel" |
| **Image reference** | Use image to shape prompt | [Paste image] "Generate a prompt I can use to create a logo that evokes this style" |
| **Text reference** | Use text to shape prompt | [Upload PDF] "Generate a prompt to explain the most important concepts in this manual" |
| **Meta-prompt chaining** | Break prompt creation into sub-prompts | "Generate a prompt that identifies the most important qualities of an intro paragraph for a grant proposal" |

---

### Prompt Refinement Strategies

| Strategy | Use Case | Solution |
|----------|----------|----------|
| **Leveling up** | Output isn't engaging enough | "How can I change my initial prompt to produce an ad campaign that uses more engaging language?" |
| **Remixing** | Multiple prompts each missing something | "Combine these prompts into a single prompt that retains the most important parts of each" |
| **Style swap** | Output is technically correct but boring | "Rewrite my prompt with an emphasis on emotionality, using more expressive, passionate language" |

---

## AI Agents

**Definition:** AI systems that can autonomously handle complex, multistep workflows with your guidance and oversight.

### What AI Agents Can Do

| Task | Example |
|------|---------|
| **Market research** | Analyze competitors, find features, synthesize reviews into weekly email |
| **Sales streamlining** | Go through inbox, identify leads, extract contacts, create database entries |
| **Demand forecasting** | Analyze sales/inventory data, predict demand, order supplies |

---

### How AI Agents Work

| Component | Description |
|-----------|-------------|
| **Models** | Trained to recognize patterns and predict necessary tasks |
| **Permissions** | Guardrails you set controlling how agent executes tasks |
| **Goals** | Broad objectives you provide |

#### Agent Operation Loop
```
┌─────────────┐
│   ANALYZE   │ ← Determine necessary task
└──────┬──────┘
       │
       ▼
┌─────────────┐
│     ACT     │ ← Execute task with granted permissions
└──────┬──────┘
       │
       ▼
┌─────────────┐
│   OBSERVE   │ ← Review result, ensure alignment with goal
└──────┬──────┘
       │
       └──────→ (Loop continues until goal complete)
```

---

### Responsible AI Agent Use

#### Decision Framework

| Factor | Question | Implication |
|--------|----------|-------------|
| **Risk** | What's the impact of a mistake? | High risk → tighter control |
| **Reversibility** | How easily can action be undone? | Low reversibility → more oversight |

#### Best Practices

| Practice | Description |
|----------|-------------|
| **Clear, specific goals** | "Draft a 3-email sequence for product launch" not "Plan a marketing campaign" |
| **Manage permissions** | Grant only specific, necessary permissions |
| **Always evaluate** | You're responsible for agent's work |
| **Iterate and refine** | Treat agent as collaborator |

---

# Glossary of Key Terms

| Term | Definition |
|------|------------|
| **Analogous task** | Similar problem used as guide for solving new problem |
| **Chain-of-thought prompting** | AI retraces reasoning step by step |
| **Constraints** | Parameters that direct AI toward particular result |
| **Context** | Background information informing output |
| **Contextual understanding** | AI's ability to interpret information within specific setting |
| **Delimiters** | Symbols (""", <>, **) that separate prompt components |
| **Evaluation** | Critically assessing output for accuracy, bias, relevance |
| **Few-shot prompting** | Providing 2+ examples in prompt |
| **Format** | Structure/layout of output |
| **Hallucinations** | AI output containing false information |
| **Human-in-the-loop** | Human verification of AI outputs before use |
| **Iteration** | Continuous refinement of prompts |
| **Long context window** | AI's ability to retain more information from past interactions |
| **Meta-prompting** | Using AI to help design prompts |
| **Modalities** | Different formats (text, image, audio, video) |
| **Multimodal prompting** | Using multiple modalities in same prompt |
| **One-shot prompting** | Providing single example in prompt |
| **Persona** | Role assigned to AI guiding its behavior/tone |
| **Prompt** | Input providing instructions to AI |
| **Prompt chaining** | Building on interconnected prompts |
| **Prompt versioning** | Tracking different versions of prompts |
| **References** | Supplementary resources resembling desired output |
| **Sampling parameters** | Variables controlling AI's selection pool |
| **Task** | Action/objective AI is meant to accomplish |
| **Temperature** | Degree of randomness in AI's selection |
| **Tokens** | Building blocks AI uses to process text |
| **Top-K** | Fixed number of tokens AI can select from |
| **Top-P** | Combined probability threshold for token selection |
| **Tree-of-thought prompting** | AI shows multiple possible outcomes at once |

---

# Key Takeaways Visual Summary

## The TCREI Framework at a Glance
```
┌─────────────────────────────────────────────────────────────────────────┐
│                         TCREI FRAMEWORK                                  │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│  T  ─  TASK: Clearly describe what you want (+ persona + format)       │
│                                                                         │
│  C  ─  CONTEXT: Provide all necessary background details               │
│                                                                         │
│  R  ─  REFERENCES: Include examples for AI to model                    │
│                                                                         │
│  E  ─  EVALUATE: Assess output for accuracy, bias, relevance           │
│                                                                         │
│  I  ─  ITERATE: Refine until it's just right                          │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

## Four Iteration Methods
```
         ┌──────────────────────┐
         │  Revisit framework   │
         └──────────┬───────────┘
                    │
┌───────────────────┼───────────────────┐
│                   │                   │
▼                   ▼                   ▼
┌─────────┐   ┌─────────────┐   ┌─────────────────┐
│ Tweak   │   │ Break into  │   │ Introduce       │
│ phrasing│   │ shorter     │   │ constraints     │
└─────────┘   │ prompts     │   └─────────────────┘
              └─────────────┘
```

## Responsible AI Checklist
```
□ Consider effects of using AI
□ Get approval to use AI
□ Consider privacy/security implications
□ Evaluate all AI-generated content
□ Disclose your use of AI
```

---

## Connection to Your Seminar Frameworks

### TCREI ↔ 4Ds Mapping

| TCREI | 4Ds Equivalent | Connection |
|-------|----------------|------------|
| **Task** | Delegation | Deciding what to ask AI to do |
| **Context + References** | Description | Providing clear instructions |
| **Evaluate** | Discernment | Critically assessing outputs |
| **Iterate** | Discernment + Description | Refining based on evaluation |
| (Throughout) | Diligence | Responsible use practices |

### For Pre-Service Teachers

| TCREI Application | Teaching Context |
|-------------------|------------------|
| **Task** | "Create a lesson plan for Grade 9 Araling Panlipunan on EDSA Revolution" |
| **Context** | "Students are visual learners; 45-minute period; DepEd curriculum aligned" |
| **References** | Provide sample lesson plans in preferred format |
| **Evaluate** | Check facts, cultural appropriateness, grade-level fit |
| **Iterate** | Adjust based on student needs, add Filipino terms |

---

## Source Information

**Document Title:** Google Prompting Essentials
**Program:** Specialization by Google and Coursera
**Provider:** Department of Trade and Industry La Union
**Compiled by:** dlastnoel
**Content last updated:** February 2026
**Estimated completion time:** Under 10 hours