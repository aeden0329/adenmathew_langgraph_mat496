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
I learned how to set and use breakpoints in LangGraph Studio to pause graph execution and inspect state.
I used these breakpoints to debug my nodes interactively and understand the data flow more clearly.

LESSON 3:
I learned about the key tools and documentation links for debugging and improving LangGraph workflows.
I learned where to find resources for editing state, human feedback, and graph evaluation to enhance my projects.

LESSON 4:
I learned that breakpoints are really useful for human approval, for debugging and for editing graph state although often times it is helpful to interrupt the graph dynamically itself, which can be achieved using NodeInterrput
Dynamic breakpoints have an advantage over breakpoints as they can enable, disable or move breakpoints while the program is running without restarting the session.

LESSON 5:
I learned how to use time travel in LangGraph Studio to go back to previous states of graph execution.
I used this feature to replay and debug earlier steps, helping me understand how the graph evolved over time.

MODULE 4:

LESSON 1:

I learned how to split a complex task into parallel branches in LangGraph so different sub-tasks run simultaneously.
I learned to set up and combine these parallel nodes so the graph executes more efficiently and returns a synchronized result.

LESSON 2:

Subgraphs allow you to create and manage different states within
different parts of your graph 
I learned how sub-graphs let me reuse smaller workflows inside a larger LangGraph.
I understood how parent and sub-graphs share or pass state to make complex graphs easier to manage.

LESSON 3:
I learnt about MapReduce 
MapReduce is an efficient task breaking down and parallel processing method
where you take some task split into a bunch of subtasks and do them all in parallel(map phase)
and then combine the results from the parallel subtasks and bring them together(reduce phase).
MapReduce can easily handles very large datasets across multiple machines or nodes and is therefore very useful.

LESSON 4:
