MODULE 1:
LESSON 1(motivation):
LangGraph was made to build agentic, stateful, branching AI workflows
(not just linear chains), enabling loops, memory, and human oversight —
providing more control, reliability, and observability for complex LLM applications.
LESSON 2:
 I learned how to build a basic LangGraph using nodes and edges to define the flow of data between components.
 I also understood how the StateGraph manages state transitions across nodes.
 Changes made:
    Added own example for StateGraph
LESSON 3:
I learned how studio works letting me visually build and test agent workflows, making debugging and tweaking much easier.
I also saw how I can get real-time feedback on my LangGraph applications.
LESSON 4:
I learned how to build and manage chains;sequences of interconnected nodes that define the flow of data and logic in your langgraph applications.


MODULE 2:
LESSON 1:
I learned what a state schema is in LangGraph: it defines the structure and types of data shared in your workflow graph.
I also learned how to define state schemas using TypedDict, dataclasses, or Pydantic—with Pydantic enabling runtime data validation.
Changes made: 
changed example(TypedDictState)
LESSON 2:
I learnt how LangGraph state reducers work: by default, state gets overwritten, 
but you can specify reducers like operator.add or custom functions so updates are accumulated
 (e.g., appended to lists instead of replaced) when nodes run concurrently.
 LESSON 3:
 I learnt that LangGraph supports using multiple schemas for state, 
 allowing me to separate private/internal state from what flows into the graph’s final input and output—making my graph logic cleaner and more controlled.
 LESSON 4:
 I learned how to use message trimming and filtering to control the chat history size by removing or keeping only relevant messages for better performance management.
 I also saw how to customize the trimmer function to handle conversation history dynamically based on message type, length, or role.
 LESSON 5:
 I learned how to build a chatbot that maintains long-term memory by summarizing older messages into concise context using a summarizer node. 
 I also saw how the MemorySaver checkpointer allows the chatbot to recall context efficiently.
 Changes made:
 changed example
 LESSON 6:
I learned how to extend the chatbot’s summarization logic using external memory (like a file or database) to persist conversation history beyond a single session. 
I also saw how to integrate a custom checkpointer for saving and loading summaries, enabling long-term memory for your chatbot.

MODULE 3:

LESSON 1:

In this lesson, I learned how to use streaming with LangGraph to receive model outputs in real-time as they’re generated,
rather than waiting for the full response. 
I also explored how streaming improves interactivity and responsiveness in chatbots or agent workflows.

LESSON 2:
