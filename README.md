AI Moderation Project
This project was developed as part of the Foundations course in the MS Data Journalism program at Columbia University (Fall 2024). The objective is to explore, integrate, and evaluate various AI content moderation tools and models, providing insights into their strengths, weaknesses, and potential applications in journalism and media analysis.

Project Overview
This application combines multiple content moderation tools to assess their performance and reliability in identifying harmful or toxic content. The project explores APIs and models from major providers and open-source platforms, with a focus on their practical use in journalism.

Features
Integrated Moderation APIs:

OpenAI Content Moderation API: Flags categories such as hate speech, harassment, and violence. Provides nuanced feedback on flagged content. Documentation
Anthropic/Claude API: Offers simple "ALLOW" or "BLOCK" classifications for user-generated text. Documentation
Azure Content Moderation API: Provides severity ratings (0–6) for flagged content in categories like hate, self-harm, and violence. Documentation
HuggingFace Integration:

Integrated Toxic-BERT, an open-source model designed to detect toxic comments while minimizing bias. Offers confidence scores for nuanced moderation results. Model
Key Observations
Context Sensitivity: Most tools struggle to account for context, flagging keywords without fully understanding their intent.
Bias in Moderation:
Some tools over-flag neutral mentions of identities, such as religion or ethnicity.
Tools reflect a Western-centric perspective, with better detection of widely-publicized conflicts over lesser-known ones.
Transparency:
OpenAI and Azure APIs offer detailed feedback on flagged categories.
HuggingFace models provide transparency in design and confidence scoring, enabling better understanding of results.
Potential Enhancements
Safe Text Suggestions: Automatically generate unflagged versions of flagged content.
Flagged Text Highlighting: Pinpoint specific words or phrases flagged by moderation tools.
Comparison Visualizations: Develop charts or metrics to compare the outputs of different tools.
Future Goals
Integrate additional content moderation APIs and HuggingFace models.
Build a custom moderation model tailored to journalistic needs, addressing the limitations identified in existing tools.
Expand the app with features to improve usability, such as interactive visualizations and content rewriting tools.
This project highlights the challenges and possibilities of content moderation in journalism, reflecting the values of Columbia Journalism School's commitment to ethical reporting and technology integration. Contributions and feedback are welcome to help improve the tool!

