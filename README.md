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




