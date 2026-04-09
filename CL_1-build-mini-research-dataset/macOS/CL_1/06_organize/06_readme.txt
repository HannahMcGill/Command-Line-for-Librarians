🧭 06) Organize the Outputs
=============================
🏆 Goal: Create subfolders and move files into a tidy structure.

1️⃣ Type: cd .. and then cd research_project (or use cd and the tab key) to navigate to the research project file.

2️⃣ Type: mkdir raw_data 

3️⃣ Type: mkdir processed

💡 Why: These commands will create two new folders in your research project parent folder; one new folder for raw data and one new folder for processed data.

4️⃣ Type (or copy and paste): mv papers.json raw_data/

💡 Why: mv means "move" and will relocate the JSON payload you downloaded and saved as papers.json to the new folder you created for raw data.

✨ Tip: mv can be used to move files or folders around your computer. To move a file or folder into a new folder type: mv filename newfoldername/

5️⃣ Type (or copy and paste): mv titles.txt processed/

💡 Why: mv means "move" and will relocate the titles you extracted and saved as a text file to the new folder you created for processed data.

✨Tip: mv can be used to move files or to rename files! If you want to rename a file, use "mv filename new_filename".

6️⃣ Confirm that everything is where it should be by checking the file structure. Type: tree 2>/dev/null || ls -R

💡 Why: "tree 2>/dev/null || ls -R" tries to show your folder structure in a nice tree format, and if the tree command isn’t available. You use it so your project structure is displayed reliably on any system, even if tree isn’t installed.

✨ Tip: Now that you have Homebrew installed, you can easily install tree by typing brew install tree and after you have successfully installed tree you will only need the tree command to display the folder structure wherever you are along your path.

🎉🎉🎉 CONGRATULATIONS! 🎉🎉🎉 You’ve completed your first command line project and learned fundamental skills that you can reuse and repurpose within the library and beyond!