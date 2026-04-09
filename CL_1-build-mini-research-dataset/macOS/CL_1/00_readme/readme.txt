CL_1 Build a Mini Research Dataset (macOS Edition) 
=================================================

👋 Welcome! This self-guided, introductory tutorial will teach you command-line basics as you complete a library-relevant project in 40 minutes or less.

🧰 Project: Organize and Explore a Mini Research Dataset

📚 You'll learn to:

- Locate where you are (pwd)
- Identify all the files and folders in your current location (ls)
- Move to a new location (cd)
- Open/read a text file (cat) (less)
- Download data from the web (curl)
- Create new folders (mkdir)
- Run simple text searches (/term)
- Install and run software (brewInstall)
- Clean and extract information (jq)
- Move/rename files (mv)
- Display a clear folder structure (tree)

🛠️ How this works:

The CL_1 project folder you have downloaded and saved to your Desktop contains 6 folders with instructions. You will use the command line to move through each of the instructional folders in order. 

🏆 Your first goal: Get to the CL_1 folder using the command line

1️⃣ Open the Terminal app: 🔍 Spotlight Search > Terminal > Enter

2️⃣ Identify where you are: Type pwd

💡 Why: pwd means "print working directory". It shows you where you are in your computer's file structure by providing the path to your current location. A path is just an address to a location on your computer.

✨ Tip: If you're lost, pwd is your friend. 

3️⃣ Read your prompt: Look at the text before your cursor in Terminal.

💡 Why: It usually shows something like: "[yourname]@MacBook-Air-3 Desktop"

✨ Tip: The last part (Desktop) is your current location. If you see ~ as the last part, that means you are in your home directory, which is the start of every path.

4️⃣ Identify what files and folders are in your current location: Type ls

💡 Why: ls means "list what's here" and shows you all the files and folders in your current location.

✨ Tip: Combine pwd and ls often so that you know where you are and what's there.

5️⃣ Navigate to the CL_1 folder by moving step by step along the necessary path using the command cd

💡 Why: cd means "change directory" and will move you step by step along your path. In order to use cd you type the command followed by the name of the folder you want to move into.

✨ Tip: When you use the cd command followed by the name of the folder you want to move into, you are always moving one step forward along a path. You can use cd .. to move one step backward along your path (to the parent folder) and you can use cd on its own, with no corresponding folder name, to move all the way back to your home directory (the very start of every path).

6️⃣ To follow the path to the CL_1 folder from your home directory: Type cd Desktop

💡 Why: cd Desktop moves you from your home directory to your Desktop.

✨ Tip: If you have successfully moved to your desktop, then the prompt you see before your cursor should end with Desktop. If you want to check where you are, enter the command pwd and then enter the command ls to see all the files folders on your desktop. You should see the CL_1 folder listed.

7️⃣ To navigate into your CL_1 folder: Type cd CL_1

💡 Why: cd CL_1 will move you from your Desktop into the CL_1 folder where you found these instructions. Now that you are in the CL_1 parent folder, you can use cd to move through the instructional folders (in order!) to complete the project.

✨ Tip: Pressing tab at any time will prompt the command line to attempt to auto-complete your input based on the options available to you. So, if you want to change directories (cd) and you don't want to type in the name of the folder you want to navigate into, try cd and then the tab key to cycle through your options. Keep pressing tab until you find the one you want. 

❗ Remember! When you are using the cd command you can only move to a folder nested within the folder where you are currently located. You cannot jump from, say, your home directory all the way to the CL_1 folder using cd. 

🚀 NEXT LESSON: 

1️⃣ Type cd 01_cat (or use cd and then the tab key) to navigate into the first instructional folder.

2️⃣ Type cat 01_readme.txt (or use cat and then the tab key).