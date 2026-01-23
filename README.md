# Squirrelsyphus

# Downloading and Running the Unreal Project

## What You'll Need

Before starting, make sure you have:
- Unreal Engine 5.5 installed
- A GitHub account

---

## Step 1: Install Git and Git LFS
Git LFS is for large files, which we'll be dealing with a lot in this project. Please double check if you have Git LFS installed with `git lfs --version` even if you already have Git!

### Windows:
1. Go to https://git-scm.com/install/windows
2. Download and run the installer
3. During installation, just click "Next" through all the options (the defaults are fine)
4. Go to https://git-lfs.com/
5. Download and run the Git LFS installer
6. Open Command Prompt (search for "cmd" in Windows start menu)
7. Type `git lfs install` and press Enter

### Mac:
1. Open Terminal (find it in Applications > Utilities)
2. Type `git --version` and press Enter
   - If Git is already installed, you'll see a version number
   - If not, macOS will prompt you to install it
3. Install Git LFS by typing: `brew install git-lfs`
   - If you don't have Homebrew, first run: `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`
4. Type `git lfs install` and press Enter

---

## Step 2: Download the Project

1. **Get the repository URL:**
   - `https://github.com/jenny-moore/Squirrelsyphus.git`
   - (You can also find this by clicking <> Code -> HTTPS -> Copy to clipboard)
   ![Screenshot of the repository link](/readmeImages/githubLink.png)

2. **Choose where to save the project:**
   - Navigate to the `Unreal Projects` folder on your laptop
   - Example: `C:\Users\user\Documents\Unreal Projects` on Windows or `~/Documents/Unreal Projects/` on Mac
   - Save this path somewhere! We will be using it a lot.
      - On Windows, right click and choose "Copy as path"


3. **Clone (download) the repository:**
   - **Windows:** Open Command Prompt
   - **Mac:** Open Terminal
   - Navigate to your chosen folder - `cd` stands for change directory (folder):
     ```
     cd "<path>"
     ```
     (Replace with your actual path from before - should end with Unreal Projects. 
     
     Make sure to use quotations "")
   - Download the project by typing:
     ```
     git clone https://github.com/jenny-moore/Squirrelsyphus.git
     ```
   - Press Enter and wait. This might take 10-30 minutes depending on project size

---

## Step 3: Open the Project in Unreal Engine

1. **Launch Unreal Engine**
   - Once in Unreal Engine, open SquirrelDemo from the Unreal Project Browser.
   - Note: If you launch through Epic Games, you may see SquirrelDemo in your Projects. 
   - **If it has the Unreal logo and no graphics, you must launch Unreal before opening it.**
   - Otherwise Unreal will not know that it needs to generate project files before running and throw an error.

2. **First-time setup:**
   - The first time you open the project, Unreal may take a long time to set everything up
   - **Don't close Unreal during this process!** Just let it finish

3. **Success!**
   - Once everything loads, you should see the Unreal Editor
   - You're ready to start working!

---

## Making Changes and Uploading Your Work

### Before You Start Working:
Always get the latest changes first:
1. Open Command Prompt/Terminal
2. Navigate to your project folder: `cd "C:<path>\Unreal Projects\Squirrelsyphus"`
3. Run: `git pull`
4. Wait for it to finish

### After You Make Changes:
1. Save your work in Unreal Engine (Ctrl+S or Cmd+S)
2. Close Unreal Engine
3. Open Command Prompt/Terminal
4. Navigate to your project folder: `cd "C:<path>\Unreal Projects\Squirrelsyphus"`
5. Type these commands one at a time:
   ```
   git add .
   git commit -m "Brief description of what you changed"
   git push
   ```

**Important:** Always coordinate with your team! If two people edit the same file, you might have conflicts that need to be resolved.