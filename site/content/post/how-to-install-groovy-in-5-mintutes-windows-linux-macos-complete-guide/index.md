---
title: "How to install Groovy in 5 mintutes[Windows, Linux, MacOs] (Complete Guide) "
date: 2024-06-28T15:36:48.408Z
description: "Hello, this is Sabyasachi. In today's tutorial, i will guide you
  how you can install Groovy in cross platform(Windows, Linux, MacOs). "
image: groovy.jpg
---
## Installing Groovy

### Windows

1. **Install Java Development Kit (JDK)**:
   - Groovy needs Java to run. Download and install JDK from [Oracle](https://www.oracle.com/java/technologies/javase-jdk11-downloads.html).

2. **Download Groovy**:
   - Go to [Groovy download page](https://groovy.apache.org/download.html).
   - Get the Windows installer.

3. **Run the Installer**:
   - Double-click the installer file.
   - Follow the steps to install Groovy.

4. **Set Environment Variables**:
   - Open `Control Panel` > `System and Security` > `System` > `Advanced system settings`.
   - Click `Environment Variables`.
   - In `System variables`, find `Path`, click `Edit`, and add `C:\Groovy\bin` (or where you installed Groovy).

5. **Verify Installation**:
   - Open Command Prompt.
   - Type `groovy -version`.
   - You should see the Groovy version number if it's installed correctly.

### Linux

1. **Install Java Development Kit (JDK)**:
   - Use your package manager. Example for Ubuntu:

   ```bash
   sudo apt update
   sudo apt install openjdk-11-jdk (Can use any other version)
   ```

2. **Install Groovy**:
   - Use SDKMAN for easy installation:

   ```bash
   curl -s "https://get.sdkman.io" | bash
   source "$HOME/.sdkman/bin/sdkman-init.sh"
   sdk install groovy
   ```

   - Alternatively, download from [Groovy website](https://groovy.apache.org/download.html) and extract:

   ```bash
   tar -xvzf groovy-X.Y.Z.zip
   sudo mv groovy-X.Y.Z /usr/local/groovy
   ```

3. **Set Environment Variables**:
   - Add to your `~/.bashrc` or `~/.zshrc`:

   ```bash
   export GROOVY_HOME=/usr/local/groovy
   export PATH=$PATH:$GROOVY_HOME/bin
   source ~/.bashrc  # or ~/.zshrc
   ```

4. **Verify Installation**:
   - Open a terminal.
   - Type `groovy -version`.
   - It should show the Groovy version installed.

### macOS

1. **Install Java Development Kit (JDK)**:
   - Use Homebrew:

   ```bash
   brew install openjdk
   ```

2. **Install Groovy**:
   - Use Homebrew:

   ```bash
   brew install groovy
   ```

3. **Verify Installation**:
   - Open Terminal.
   - Type `groovy -version`.
   - You should see the Groovy version number displayed.

### Notes:

- **Setting JAVA_HOME**: Ensure `JAVA_HOME` is set to your JDK path.
  - Windows: Control Panel > System > Advanced System Settings > Environment Variables.
  - Linux/macOS: Add to `~/.bashrc` or `~/.zshrc`: `export JAVA_HOME=/path/to/your/jdk`.

- **Updating Groovy**:
  - Windows: Download the latest installer.
  - Linux: Use SDKMAN (`sdk upgrade groovy`).
  - macOS: Use Homebrew (`brew upgrade groovy`).


I Hope this tutorial helped you to install Groovy. Thank you so much! 
