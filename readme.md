# VS Code Config for M1 Mac

1. Install [C++](https://marketplace.visualstudio.com/items?itemName=ms-vscode.cpptools), [Code Runner](https://marketplace.visualstudio.com/items?itemName=formulahendry.code-runner) VS Code extension
2. Install & Config timeout:

   > brew install coreutils

   > sudo ln -s /usr/local/bin/gtimeout /usr/local/bin/timeout

3. Then do this:

   > cd ~/Documents/

   > mkdir input_output

   > touch input.txt output.txt

4. Install gcc & Config it:

   > brew install gcc

   > cd /opt/homebrew/bin/

   > ln -s gcc-11 gcc

   > ln -s g++-11 g++

   Run this to ensure your mac recognize the homebrew's gcc & g++ compiler:

   > where gcc g++

5. In VS Code navigate to:

   > Settings > Extensions > Run Code Configuration > Executor Map > settings.json

   Copy everything from the settings.json in the repo and paste it there.

6. Create a layout (by opening a cpp file, ~/Documents/input_output/input.txt & ~/Documents/input_output/output.txt) and save that as a workspace. Save and Run by Ctrl+Alt+N & Stop by Ctrl+Alt+M

# Configure Debugger

1. Install [lldb](https://marketplace.visualstudio.com/items?itemName=lanza.lldb-vscode) VS Code Extension
2. Copy everything from the gdb_macm1 folder and paste it in your <b>working directory’s .vscode</b> folder.

# For more info

Read this:

> https://dev.to/ayushpattnaik/running-c-17-on-mac-m1-47cp

# Snippets

1. Goto:

   > Code > Preferences > User Snippets

   > Select Language

   > Copy the snippets from the snippets folder and paste it there
