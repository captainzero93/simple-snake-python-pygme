# .Py Snake Game 🐍

A simple implementation of the classic Snake game built with Python and Pygame. Detailed manual compile instructions. Building from source may work on Mac and Linux (untested). 


<p style="text-align:center;">
  <img src="Desktop Screenshot 2025.11.15 - 01.50.30.55 - Copy.png" width="228" height="128" style="vertical-align:middle;">
</p>

<p style="text-align:center;">
  <span style="display:inline-flex; align-items:center; gap:10px;">
    <img src="[https://github.com/captainzero93/simple-snake-python-pygme/blob/main/video-icon-13.jpg?raw=true](https://github.com/captainzero93/simple-snake-python-pygme/blob/main/Desktop%20Screenshot%202025.11.15%20-%2001.50.30.55%20-%20Copy.png?raw=true)] width="12" height="12">
    <a href="https://github.com/captainzero93/simple-snake-python-pygme/blob/main/snake2.gif"> !!! [Gameplay Video] !!! </a>
  </span>
</p>


## Features
- Classic snake mechanics: eat food to grow longer!
- Arrow keys for movement (Up/Down/Left/Right)
- Score tracking system
- Game over when hitting walls ( window boundaries ) or yourself
- Simple, clean UI with color-coded elements

## Requirements
- **Python 3.11** (required for precompiled wheel compatibility)
- Pygame (`pygame==2.6.1`)
- all other requirments are in the requirments.txt even if they are not needed
   
## Manual installation & Setup
### Step 1: Create Virtual Environment / Clone repo

Download and extract this repo, Install Python 11 - ensire you check 'Add to path in the installer. Open CMD from the extracted folder;

```bash
python -m venv snake_venv
python -m venv snake_venv --system-site-packages

# Create venv using Python 3.11 explicitly

```

### Step 2: Activate Virtual Environment
```powershell
# Windows (PowerShell):
.\snake_venv\Scripts\activate.ps1

Built for Pygame 2.6.1 and python 3.11 on Windows ( untested on linux )
```

### Step 3: Install Dependencies
```bash

pip install -r requirements.txt

or

pip install --user pygame==2.6.1  # Install from PyPI


or

pip install --user "folder_with_pygame.whl package\pygame-2.6.1-cp311-win_amd64.whl"
```

> ⚠️ **Important**: The wheel file requires Python 3.11. If you're using a different version, [download the correct wheel](https://www.pygame.org/download.html) or install from source.

## Running the Game
```bash
From inside the folder snake.py exists;

python snake.py

```
Or download the self contained Windows ( or Linux .PKG) build in Releases. ( Only do this if you trust the source)

### Controls
| Key | Action |
|-----|--------|
| ↑  | Move Up |
| ↓  | Move Down |
| ←  | Move Left |
| →  | Move Right |

RULES: You are the green snake, collect the fruit, do NOT backtrack on yourself or hit into yourself or the boundaries !

## Project Structure
```
Extracted_files/
├── README.md                                              # This file
├── snake.py                                               # Main game logic
├── Desktop Screenshot 2025.11.15 - 01.50.30.55 - Copy.png #Game screenshot
├── LICENSE                                                # Auto-generated License 
├── snake2.gif -                                           # Gameplay footage 
├── video-icon-13.png -                                    #Icon
├── requirments.txt -                                      #Requirments file for building
├── 
├── .gitignore - Allows release files over 25 mb, the game is just below 30mb compiled
     
```

## Technical Details
- Built using **Python 2.11** for compatibility with pygame
- Uses a simple grid-based movement system
- Score increases by a point per food item eaten
- Game ends when snake collides with wall or itself

---

**Note**: This implementation requires the precompiled wheel file (`pygame-2.6.1-cp311-win_amd64.whl`) due to Windows-specific build requirements. Do not attempt to compile from source on Python 3.12+ as it will fail.
The reccomended way to instal pygame-2.6.1-cp311-win-amd64.whl is pip install --user pygame==2.6.1  # Install from PyPI


Again, Windows users can use the Release .exe in the Releases section, ONLY do this if you trust the source, I recommend reading the code from this repo first.
Refer to the documentatiom for your Linux Distro for unzipping and instaling the .PKG zip.

Version: 0.1 | Author: captainzero93 |

GitHub: https://github.com/captainzero93/
