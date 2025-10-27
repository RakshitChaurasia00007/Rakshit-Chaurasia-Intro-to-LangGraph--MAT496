# Rakshit-Chaurasia-Intro-to-LangGraph--MAT496
This repository will include each and every detail of what I have learned and self reflected throughout my journey of learning  Langgraph from basic .

## Learnings of Video 1
I learned that LangGraph helps language models work better by giving them control flow and access to tools or extra information like documentation.
It solves the limits of normal LLMs and makes their process smoother and safer.
Overall, it helps manage and connect chains and agents so the model works clearly and efficiently.
### (Since the video talks about the general info about LangGraph we haven't uplaoded any file or done any changes as it is just teaching us the basics)


# Beginning of Video 2 for Foundation: Introduction to LangGraph

## Learnings of Video 2
### What have I learned through the Video 2 ?
Well ! I learned how to make a simple graph with the nodes and edges and how to control which path it takes using the conditions.
I also saw how the state changes as the graph moves from one node to the another.

### What were some of the changes that I made different than what was given ?
Earlier in the original file, the graph only had three nodes and randomly chose between happy or sad. So, to change that I added more nodes like the node_4 saying “but!” and the node_9 saying “well” to make it longer and more interesting. Further I added a new function to choose between more paths and made the final output fixed as “Hi, this is Lance. I am excited for the party.” I also cleared the code and added comments such that it’s easier to understand and comprehend.

### Below I am attaching the link to the Updated code file for the video 2 .
Link => https://github.com/RakshitChaurasia00007/Rakshit-Chaurasia-Intro-to-LangGraph--MAT496/blob/main/simple_graph_UPDATED.ipynb


# Beginning of Video 4 for Foundation: Introduction to LangGraph

### What have I learned in the Video 4 ?

Now in the Video 4 I learned how to simply create a simple chain in the Lang Graph where the chat messages act as the state of the graph After that I learned about how we can connect a tool to a chat model such that it can automatically perform different task like calculations and etc. whenever required. Other than that I saw how the messages are added to the graph step by step using the reducer such that nothing gets overwritten.

### What were some of the changes which I have done to make things different than the original file ?
Well! if we take a look at  the original code, the example messages were about "orcas in the USA" . I changed them to ask about the "best observatories in the US". After that I just set the OpenAI API key directly in the code instead of entering it manually again and again one by one in each turn .
This way the model was called was updated from .invoke(messages) to the newer llm (messages) method. After that I added a few extra example messages, such as  “Good morning!” and “Tell me about the solar system,” to see how the chain will be handling the different inputs.
I also kept the tool example but updated it slightly to fit the new context.

# Beginning of Video 3 for Foundation: Introduction to LangGraph
### What I learned in Video 3 ?
I used langgraph for the first time for which I wrote "Yo I am Bobby"  while using it I learned how to see graphs as flowcharts which can help you understand the flow . Since the video did not have any code hence it was mostly about visual appealness which can be depicted through the ss given below.
<img width="872" height="335" alt="image" src="https://github.com/user-attachments/assets/5aaad719-45fc-4a31-92dc-ab22f73fe42b" />

#### The file are alredy uploaded.

# Beginning of Video 5 for Foundation: Introduction to LangGraph
### What I learned in Video 5 ?
Well in Video 5 we learned how how the system decides whether to use a tool or just respond on its own. Based on what I am typing .  


### What were some of the changes which I have done to make things different than the original file ?
Modification made is that  I changed the original multiplication tool into an addition tool hence instead of calculating 2 * 2 it will be modified in trying 3 + 3  and it will correctly give 6.

Link => https://github.com/RakshitChaurasia00007/Rakshit-Chaurasia-Intro-to-LangGraph--MAT496/blob/main/router_Updated_ishere.ipynb


# Beginning of Video 6 for Foundation: Introduction to LangGraph
What I learned

I learned how the assistant (LLM) decides whether to respond directly or use a tool based on input. I also saw how messages flow through nodes in MessagesState and how a system message can guide the LLM’s responses. It was helpful to understand how to combine user messages with system instructions and visualize the flow in a graph-like structure.

Modifications done

I set up the OpenAI API key so the LLM works smoothly, added multiple math tools (add, subtract, multiply, divide) with checks like division by zero, and created an assistant node that combines system and user messages to generate responses. I included examples for each tool and prepared the code so the LLM can later choose the right tool automatically, making it easy to expand with more operations.


# Beginning of Video 7 for Foundation: Introduction to LangGraph

### We learned that guess what every tool function always needs a certain short description known as (docstring) so that the assistant will understand
what it does. Without it, the tool can’t be used in the graph. 

### What were the modifications done in the video 7 ?
The docstrings for all math functions (`add`, `subtract`, `multiply`, `divide`) were added or updated such that they will be used to describe what the 
each function does. The `divide` function was updated to include a check for division by zero .



# Module 2 
## Lesson 1 State Schema

### What are the Lessons that we learned from State Schema ?
Well ! from this video on state schema we talked about what we’ll be doing in module 2 and went back to the simple graph from module 1 to make it look better.
We learned how to use the Python’s data class to easily make classes for storing data and added Pydantic State to catch the mistakes while running the code. 
This really helped us understand how the state and the memory work more clearly.

### What are the changes which we have performed in this Video  for State schema Lesson 1 ?
I changed everything from name and mood to city and condition to work with weather instead of feelings.
After that I have updated the nodes and decision logic to use the words "sunny", "rainy", "cloudy", "stormy" instead of using the below 
"happy", "sad".
I have also updated the pydantic state such that passing any wrong value like "crazy" now throws a ValidationError.

Link of the Updated State schema FIle => https://github.com/RakshitChaurasia00007/Rakshit-Chaurasia-Intro-to-LangGraph--MAT496/blob/main/state_schema_Updated_Correctly.ipynb

After this we will begin with Lesson 2 ...


## Lesson 2 State Reducers

### What are the Lessons that we learned from State Reducers
Well ! after watching this lesson on State Reducers, I learned that reducers control how the state updates are applied to the different keys.
They also ensure that multiple nodes can safely update state using overwrite, append, or custom merge behaviors.
We have also used the reducers to append values, handle edge cases with custom merges, and the update or remove messages by ID, giving full control over the state.

### What are the changes which I have performed in this Video for State Reducers in the Lesson 2 ?
After watching the video on State Reducers I swapped all foo keys for bar across every reducer example to make the state naming consistent and clearer.
Further I polished the text, added Markdown formatting, and included helpful links to docs for easier reading.

Link of the Updated State Reducers File =>  https://github.com/RakshitChaurasia00007/Rakshit-Chaurasia-Intro-to-LangGraph--MAT496/blob/main/state_reducers_updated_correctly_.ipynb


After this we will begin with Lesson 3 which is Multiple Schemas...


## Lesson Multiple Schemas 

### What are the Lessons that we learned after watching video on Multiple Schemas ?
Now after watching this lesson's video I learned how nodes can share the temporary information without changing the graph’s main inputs or outputs.
I also saw how I can set the graph to only show the important results while keeping all extra data for its work.


### What are the changes which I have performed in after watching the Video for Multiple Schemas in the Lesson 3 ?

After watching the lesson on Multiple Schema I added the summary and reasoning steps fields to demonstrate how custom schema flow.
Further I have updated node logic to give different outputs and included debug print statements .
I have also enhanced the output to show both the final answer and the summary, showing the full data transformation.

Link for the Updated file on Multiple Schema => https://github.com/RakshitChaurasia00007/Rakshit-Chaurasia-Intro-to-LangGraph--MAT496/blob/main/multiple_schemas_Updated.ipynb

After this we will begin with the Lesson 4 of this module 2 which is Trim and Filter Messages ....


## Lesson Trim and Filter Messages 
Well after watching the lesson on Trim and Filter Messages I learned how to customize and use the different graph state schemas, create our own state 
reducers, and manage the messages better with reducers, filters, and trimmers. These help control how much of the chat history is sent to the model while 
keeping the message channel consistent for smooth chatbot performance in the LangGraph.

### What were the changes which were done in the Updated file for Trim and Filter Messages after watching it ?
So, I have used trim_messages to send only recent messages within a token limit.
Further I the last AIMessage and new HumanMessage are appended automatically for multi-turn chat.
FOr tweaking I have also made sure that responses are pretty-printed, and the stateGraph shows the chat node flow in one cell.


Link for the Updated file is here => https://github.com/RakshitChaurasia00007/Rakshit-Chaurasia-Intro-to-LangGraph--MAT496/blob/main/trim_filter_messages_Updated_.ipynb

## Lesson Chatbot w/ Summarizing Messages and Memory
Now I have watched the lesson and completed the coding part as well so while completing the work I have learned to build a chatbot with memory using a 
running summary to compress long conversations and reduce token cost.Further I learned tha LangGraph’s persistence maintains context across steps efficiently. I also learned that conditional edges decide when to refresh the summary to keep responses accurate and context-aware.

### What are some of the changes which were done after learning from Chatbot w/ Summarizing Messages and Memory lesson?
For modifications I have changed the state key from summary to context_recap so the chatbot keeps short bullet-point recaps of the conversation. I have also updated the model calls and prompts to work with the context_recap instead of the full narrative summaries. Further I have also foccused on renameing nodes and cleaning up how responses and recaps are shown, while keeping the graph flow and memory features working.

Link for all the updates which are done in the Updated File 
Link =>  https://github.com/RakshitChaurasia00007/Rakshit-Chaurasia-Intro-to-LangGraph--MAT496/blob/main/chatbot_summarization_Updated_.ipynb

Now this will be our last Lesson which we will eventually start Chatbot w/ Summarizing Messages and External Memory ....


## Lesson Chatbot with message summarization & External DB Memory
Well! after completing our last lesson of this module known as "Chatbot with message summarization & External DB Memory" I have learned to build a chatbot with persistent memory using SQLite checkpointers that store each conversation’s state. This allows the bot to retain context and resume chats seamlessly even after the restarts. It also helps us to optimize 
the token usage for better performance.


### What were some changes which were done to show implementation of our learnings afetr watching and completing the code file for Chatbot with message summarization & External DB Memory Lesson ?

So, after completing the lesson on Chatbot with message summarization & External DB Memory I have changed the context to a cosmic theme to make the conversation more creative and different from the original one. I have also improved the state structure such that it clearly shows the messages, memory summary, and last update in a simple way.
Further I have tweaked the prompt and memory flow to show how the state updates smoothly while keeping it easy to follow and understand every detail of our lesson.

Link for the Updated code file after watching the leasson on Chatbot with message summarization & External DB Memory is given below 

# End Note => https://github.com/RakshitChaurasia00007/Rakshit-Chaurasia-Intro-to-LangGraph--MAT496/blob/main/chatbot_external_memory_updated_is_here.ipynb

# End Note 
 ## Well It was actually fun completing Module 2 of Langgraph, I believe I have learned many skills which I will implement in my future projects in life. :)


# Well! Let's Begin with MODULE 3 which is UX & Human in the Loop

## Lesson STREAMING
 After completing the lesson I have learned that human-in-the-loop enhances the memory by allowing the users to interact with the graph execution in real time. Further I saw that LangGraph streaming provides live state updates through different modes like updates and values. Wit the '.astream_events`, we can stream LLM tokens and track key details such as the event type, name, data, and metadata from each node, making the process more transparent and interactive.

### After watching what were the modifications which you have done to depict your learnings ?
Now since I have watched I have made changes to improve how the events and messages flow during streaming.To add to that I have also worked on making the output display clearer when tokens or states update.After that  I have also foccused on refining the conversation setup so it connects better with the rest of the process.

Link of the Updated code file => https://github.com/RakshitChaurasia00007/Rakshit-Chaurasia-Intro-to-LangGraph--MAT496/blob/main/streaming_interruption_UPDATED.ipynb

### Next lesson will be Breakpoints which we will begin in a while...

## Lesson BREAKPOINT
From the lesson I learned that Human-in-the-Loop lets humans stay involved by using the breakpoints to pause the graph for feedback. It enables many components like
approval, debugging, and editing, where users can approve actions, rewind the graph using graph.stream(), or even modify the agent’s state.
This alsotaught me that it makes the overall workflow more controlled and reliable.

### What were some tweakings which I have done in after learning from this lesson ?
After watching the lesson I have used the MemorySaver to add the checkpoints for betterment of debugging and state tracking. Further I have, included interrupt_before=(tool) 
to pause the graph for user approval before tool execution. In the end I finally thought to simplify the overall graph flow to make Human-in-the-Loop
interactions faster and more efficient in use.

Here I have provided the link for the upadeted file  =>  https://github.com/RakshitChaurasia00007/Rakshit-Chaurasia-Intro-to-LangGraph--MAT496/blob/main/breakpoints_UPDATED.ipynb

### Next Lesson is of EDITING STATE & HUMAN FEEDBACK

## LESSON Edit-State-Human-Feedback

Well! I watched and completed the lesson and I learned to use the breakpoints to directly edit the graph state and insert the human feedback instead
of just waiting for the user approval. Further I learned that about the LangGraph UI, I understood real-time workflow update as well. This totally 
helped me in gaining better control over the state flow for smoother human-in-the-loop interaction.

## What were some changes or modifications which I have done after watching and completing the whole lesson on Edit-State-Human-Feedback ?
Now In this lesson for my modifications I have added a stop function to end the loop once the final feedback is reached.
Further I have set a recursion limit using the MemorySaver() to avoid the endless executions. In the end I 
lastly,made the feedback loop smoother and improved how the events are streamed and displayed for us .
I tried to do the best I could from my side in this updated file.

Link for the updated file has been provided here => https://github.com/RakshitChaurasia00007/Rakshit-Chaurasia-Intro-to-LangGraph--MAT496/blob/main/edit_state_human_feedback_UPDATED.ipynb

### Next Lesson is about Dynamic Breakpoints...
















