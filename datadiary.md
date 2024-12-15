AI MODERATION PROJECT – DATA DIARY

25/11 - 02/12

Watched tutorials and researched different AI moderation APIs

04/12

Built basic gradio app - had to delete from HuggingFace space because I didn't know how to not make it interfere with ChatGPT test

10/12

I integrated the gradio app code with OpenAI's content moderation API. I encountered an error because I needed to 'migrate' OpenAI.
I installed OpenAI using the command line. Before I could execute 'openai migrate' I had to download Grit CLI,
a command-line tool that OpenAI integrates with its library to assist developers in tasks such as migration, debugging,
and interacting with OpenAI services. It simplifies certain development workflows by providing utilities directly in the command line.
I solved this by resorting to using the 0.28 version of OpenAI



Questions for Soma
- Show OpenAI moderation error message - resolved on 04/12
- Difference between API offered by an AI company vs. the content moderation API they use for their chatbot
- Text only vs. text and image
- How to have different "boxes" if one app? Can each huggingface space only have one space?

*CODE FOR MODERATION TOOLS*

OpenAI/ChatGPT

https://platform.openai.com/docs/guides/moderation?moderation-quickstart-examples=text
from openai import OpenAI
client = OpenAI()

response = client.moderations.create(
    model="omni-moderation-latest",
    input="...text to classify goes here...",
)

print(response)

Anthropic/Claude

https://docs.anthropic.com/en/docs/about-claude/use-case-guides/content-moderation
https://github.com/anthropics/anthropic-cookbook/blob/main/misc/building%5Fmoderation%5Ffilter.ipynb

Azure
https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/contentsafety/azure-ai-contentsafety/samples/sample_analyze_text.py

Gemini
https://ai.google.dev/gemini-api/docs/safety-settings?utm_source=chatgpt.com

Perplexity

Doesn't seem to offer one?

POTENTIAL USES

Feed a specific text? Just make the app and people can try different things? 