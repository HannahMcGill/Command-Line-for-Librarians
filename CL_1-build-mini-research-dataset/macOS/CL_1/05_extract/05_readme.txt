🧭 5) Extract and Save Titles in a Text File
==============================================
🏆 Goal: Create a readable list of article titles.

1️⃣ Type cd .. and then cd research_project (or use cd and the tab key) to navigate to the research project file.

2️⃣ Check if you have jq installed by typing jq --version If you see something like "jq-1.6" then jq is installed. If not, you will need to install jq via the command line.

💡 Why: jq a tool that lets you read and extract information from JSON files using the command line. The jq tool is like "command f" but for JSON files.

✨ Tip: Command line can be use used to easily install software, especially software that doesn't have a graphical user interface (GUI). Although this is a beginner tutorial, it can be very useful to understand that there are a number of tools available to aid you in your work with the command line, and installing those  tools may be a regular part of your work with command line.

❗If you don't already have jq installed, the easiest way to install it on a Mac is to use a package manager. A package manager lets you install and manage command‑line tools and software using simple commands. Homebrew is one of the most popular package managers for Mac, and you will download and install Homebrew to help you download and install jq. This might sound like a lot of work, but the process is relatively simple, and once you have Homebrew installed, future software downloads and installations will be very straight forward. 

To download and install Homebrew, run the Homebrew installation command line: /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

⚠️ During installation:

👉 You may be asked for your Mac password. When you type your password nothing will appear on screen. That's normal!

👉 You might be prompted to install Xcode Command Line Tools (which is normal and required).

⚠️ After you install Homebrew, you need to add Homebrew to your PATH by inputting two commands:

First, type (or copy and paste): echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> ~/.zprofile
Then, type (or copy and paste): eval "$(/opt/homebrew/bin/brew shellenv)"

⚠️ Check to see if Homebrew is installed correctly by typing: brew --version and looking for output like "Homebrew 4.x.x". 

🎉 If terminal responds to your command by displaying Homebrew and a version  number, you have successfully installed Homebrew and now you can simply and easily install jq by typing: brew install jq

3️⃣ When you have jq installed, run: jq -r '.results[].title' papers.json > titles.txt

💡 Why: This command line is used to read a JSON file, extract the title of every article, and save those titles into a new text file.

✨ Tip: To better understand how this command line works, let's break it down piece by piece:

👉 " jq" is command‑line tool for working with JSON. It understands JSON structure (objects, lists, fields).

👉 "-r" asks for plain text, not JSON‑formatted strings. Without -r, titles would appear with quotes ("Title"). With -r, they appear cleanly.

👉 "'.results[].title'" is the instruction telling jq what to extract. You can read it left to right: ".results" means go to the results section of the JSON file; [] means look at each item in that list; .title means get the title for each item.

👉 "papers.json" is the file where jq searches for the data we have requested.

👉 "> titles.txt" sends the results to a new file with the name "titles.txt" rather than displaying the titles in Terminal.

4️⃣ Type ls to verify that the titles.txt file has been created.


5️⃣ Type less titles.txt to verify that the file is populated with article titles.❗Remember; you will need to type q to return to Terminal when you are finished❗

🚀 TO GET TO THE NEXT LESSON: 

1️⃣ Type cd .. to return to the parent folder.

2️⃣ Type cd 06_organize (or use cd and the tab key) to get to the sixth project folder.

3️⃣ Type cat 06_readme.txt (or use cat and the tab key) for instructions.
