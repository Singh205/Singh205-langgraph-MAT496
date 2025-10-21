Starting module 2 of langgraph
--

Video 1:In LangGraph, the state schema basically defines how data is structured and passed between different parts of the graph. It’s like a blueprint that tells the system what information to keep, update, or share as the graph runs.

source file:https://github.com/langchain-ai/langchain-academy/blob/main/module-2/state-schema.ipynb

---

Video 2:State reducers handle how the state changes over time. They take the current state and new inputs, then decide what updates or modifications should be made before passing the state along.


source file:https://github.com/langchain-ai/langchain-academy/blob/main/module-2/state-reducers.ipynb


---

Video 3:In LangGraph, you can have multiple schemas to handle different types of data or processes within the same graph. This helps keep things organized and allows different parts of the graph to work with their own structured state.

source file:https://github.com/langchain-ai/langchain-academy/blob/main/module-2/multiple-schemas.ipynb

---

Video 4:Filter removes messages based on rules (like keeping only the last two) to control what the model sees.
Trim shortens the chat by token count, keeping only the most recent context within limits.
Both prevent token overflow and keep the AI focused on relevant information

source file:https://github.com/langchain-ai/langchain-academy/blob/main/module-2/trim-filter-messages.ipynb

---


Video 5: A chatbot with summarizing messages and memory uses state schemas to store conversation history and automatically condenses past interactions into summaries. These summaries help maintain context across graph nodes, enabling the AI to respond intelligently without reprocessing the entire chat. Memory updates are managed through state reducers, keeping the graph efficient and context-aware.

Source file:https://github.com/langchain-ai/langchain-academy/blob/main/module-2/chatbot-summarization.ipynb

---
Video 6: a chatbot with message summarization and external DB memory basically keeps things light — it summarizes recent chats so the graph doesn’t get bloated, and dumps older or important stuff into a database like Redis or Postgres. That way, it can remember things across sessions without dragging the whole chat history around every time.


Source file:https://github.com/langchain-ai/langchain-academy/blob/main/module-2/chatbot-external-memory.ipynb


---
