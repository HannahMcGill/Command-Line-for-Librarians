🧭 3) Download a Small Dataset
================================
🏆 Goal: Fetch a small JSON payload of article metadata from OpenAlex and save it in your project folder.

📋 Some useful definitions:

“Fetch” = download  
“JSON payload” = structured data  
“small” = only a handful of results, not the entire database  
“article metadata” = information about articles, not the articles themselves  

❗ This set of instructions contains a command line (an entire string of commands input together at the prompt) that looks very long and complicated. You do not need to understand how to put together a command line like this (although you will see the component parts broken down for you so that you can understand the command line as it is written). The goal of using such a long command line as a beginner is to understand that even more advanced prompts are available to you. You can use these sorts of command lines to complete a task, even if you could not write them yourself...that is what the internet is for! A quick search can lead you to whatever prompt you might need to perform a task. And so, the purpose of this lesson is to get comfortable using command lines to perform a task without learning to use each of the component parts individually.

1️⃣ Type cd .. to return to your parent folder.

2️⃣ Type cd research_project (or use cd and the tab key).

💡 Why: You need to be located inside the directory you created so that the files you download will appear within that folder.

✨ Tip: Check to make sure you are in the right folder by running "pwd".

3️⃣ Run the command line:  
   curl -s "https://api.openalex.org/works?search=urban+wildlife&per-page=20" -o papers.json

💡Why: This command line downloads metadata for 20 articles about urban wildlife from OpenAlex and saves it as a JSON file called papers.json.

✨Tip: To better understand how this command works, let's break it down piece by piece:

👉 curl is command‑line tool that gets data from the internet (think “download something from a URL”).

👉 -s means "silent" and works to hide progress messages so the terminal doesn’t get cluttered.

👉 "https://api.openalex.org/works?..." points to the OpenAlex API, which returns data instead of a webpage.

👉 works tells OpenAlex: “I want scholarly works (articles)”.

👉 ?search=urban+wildlife asks the API to search for articles related to “urban wildlife”.

👉 &per-page=20 limits the results to 20 articles.

👉 -o papers.json means “save the result into a file titled papers.json". Without this part of the command, the data would just appear in the terminal window.

👉 When you put all these pieces together, you end up with a new file in your current folder titled "papers.json" that contains metadata for 20 articles from OpenAlex.

4️⃣ To check your results, type ls and make sure you see papers.json.

🚀 TO GET TO THE NEXT LESSON: 

1️⃣ Type cd .. to return to the parent folder.

2️⃣ Type cd 04_read (or use cd and the tab key) to get to the fourth instructional folder.

3️⃣ Type cat 04_readme.txt (or use cat and the tab key) for instructions.
