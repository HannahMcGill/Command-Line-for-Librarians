🧭 5) Extract and Save Titles in a Text File
==============================================
🏆 Goal: Create a readable list of article titles.

1️⃣ Type cd .. and then cd research_project (or use cd and the tab key) to navigate to the research project file.

2️⃣ Check if you have jq installed by typing jq --version  
If you see something like "jq-1.6" then jq is installed. If not, you will need to install jq via the command line.

💡 Why: jq is a tool that lets you read and extract information from JSON files using the command line. The jq tool is like "command f" but for JSON files.

✨ Tip: Command line can be used to easily install software, especially software that doesn't have a graphical user interface (GUI). Although this is a beginner tutorial, it can be very useful to understand that there are a number of tools available to aid you in your work with the command line, and installing those tools may be a regular part of your work with command line.

❗If you don't already have jq installed, the easiest way to install it on Windows is to use a package manager. A package manager lets you install and manage command‑line tools and software using simple commands. Winget is the built‑in Windows package manager, and you will use it to download and install jq. This might sound like a lot of work, but the process is relatively simple, and once you have Winget available, future software downloads and installations will be very straight forward. 

To download and install jq using Winget, run the command:  
winget install jqlang.jq

⚠️ During installation:

👉 You may be prompted to confirm the installation. Follow the on‑screen instructions.

👉 You may be asked to allow the app to make changes to your device. This is normal.

⚠️ Check to see if jq is installed correctly by typing: jq --version and looking for output like "jq-1.6". 

🎉 If the terminal responds to your command by displaying jq and a version number, you have successfully installed jq and can move on.

3️⃣ When you have jq installed, run:  
jq -r '.results[].title' papers.json > titles.txt

💡 Why: This command line is used to read a JSON file, extract the title of every article, and save those titles into a new text file.

✨ Tip: To better understand how this command line works, let's break it down piece by piece:

👉 "jq" is a command‑line tool for working with JSON. It understands JSON structure (objects, lists, fields).

👉 "-r" asks for plain text, not JSON‑formatted strings. Without -r, titles would appear with quotes ("Title"). With -r, they appear cleanly.

👉 "'.results[].title'" is the instruction telling jq what to extract. You can read it left to right: ".results" means go to the results section of the JSON file; [] means look at each item in that list; .title means get the title for each item.

👉 "papers.json" is the file where jq searches for the data we have requested.

👉 "> titles.txt" sends the results to a new file with the name "titles.txt" rather than displaying the titles in Terminal.

4️⃣ Type ls to verify that the titles.txt file has been created.

5️⃣ Type less titles.txt to verify that the file is populated with article titles.  
❗Remember; you will need to type q to return to Terminal when you are finished❗

🚀 TO GET TO THE NEXT LESSON: 

1️⃣ Type cd .. to return to the parent folder.

2️⃣ Type cd 06_organize (or use cd and the tab key) to get to the sixth project folder.

3️⃣ Type cat 06_readme.txt (or use cat and the tab key) for instructions.