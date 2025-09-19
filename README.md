# AgentAIAutomationN8N
Created the N8N automation pipeline for scheduling the mail which triggeres with the chatbot
Here’s how the flow works end-to-end:

1️⃣ Chat Trigger
The process starts when a chat message is received. This acts as the entry point for the entire workflow.

2️⃣ AI Agent (Tools Agent)
The incoming chat is passed to the AI Agent, which acts as the brain of the workflow. The agent can reason over the input and decide which external tools to use next.

3️⃣ OpenAI Chat Model
The agent connects to the OpenAI Chat Model to understand the intent of the message, extract key details, and decide what actions need to be taken.

4️⃣ Simple Memory
The agent uses memory to keep track of the conversation context, ensuring it remembers user details and past queries during the workflow.

5️⃣ MongoDB (Find)
When required, the agent queries MongoDB to fetch structured information (like user records, compliance data, or any stored details). This makes the flow dynamic — not just relying on static responses but retrieving live data.

6️⃣ Gmail (Send Message)
Finally, based on the processed input and retrieved data, the agent automatically drafts and sends a personalized email to the user via Gmail.

✨ The outcome:

A chat message triggers the workflow

The AI agent understands and reasons over it

Context is stored and reused

Relevant data is pulled from MongoDB

A Gmail message is sent out to the user — all in one seamless automation flow.

This was my first end-to-end AI-powered automation — connecting chat, memory, database, and email into a working agentic system.
![WhatsApp Image 2025-09-19 at 8 54 38 PM](https://github.com/user-attachments/assets/30ea2bf0-32d6-4337-b4cf-2fafe91f22fb)
