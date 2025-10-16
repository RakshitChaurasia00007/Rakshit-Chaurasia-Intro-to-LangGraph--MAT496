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

# Beginning of Video 3 for Foundation: Introduction to LangGraph
### What I learned in Video 5 ?
Well in Video 5 we learned how how the system decides whether to use a tool or just respond on its own. Based on what I am typing .  


### What were some of the changes which I have done to make things different than the original file ?
Modification made is that  I changed the original multiplication tool into an addition tool hence instead of calculating 2 * 2 it will be modified in trying 3 + 3  and it will correctly give 6.

Link => https://github.com/RakshitChaurasia00007/Rakshit-Chaurasia-Intro-to-LangGraph--MAT496/blob/main/router_Updated_ishere.ipynb









