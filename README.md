<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=220&section=header&text=ZEROX%20AI&fontSize=90&fontColor=ffffff&fontAlignY=38&desc=Godot%204%20AI%20Addon&descColor=8b9cf4&descSize=22&animation=twinkling" width="100%" />

<br/>

[![Typing SVG](https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=22&duration=2800&pause=1200&color=8B9CF4&center=true&vCenter=true&width=750&lines=AI-Powered+Scene+Generation+for+Godot+4;Describe+your+scene.+ZEROX+builds+it.;Natural+Language+to+Game+Scene+in+Seconds;Built+by+Paras+Sharma+%E2%80%94+Team+Zerox)](https://github.com/zeroxn8877021/ZEROX-AI-GODOT-ADDONS-)

<br/>

![Godot](https://img.shields.io/badge/Godot_4.x-478cbf?style=flat-square&logo=godot-engine&logoColor=white)
![AI](https://img.shields.io/badge/AI_Powered-All_Major_APIs-8b9cf4?style=flat-square&logo=openai&logoColor=white)
![Version](https://img.shields.io/badge/Version-1.0.0-20c997?style=flat-square)
![License](https://img.shields.io/badge/License-MIT-6c757d?style=flat-square)
![Stars](https://img.shields.io/github/stars/zeroxn8877021/ZEROX-AI-GODOT-ADDONS-?style=flat-square&color=ffd700)
![Developer](https://img.shields.io/badge/Dev-Paras_Sharma-e05252?style=flat-square)

</div>

---

<div align="center">
<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%" />
</div>

---

## Overview

**ZEROX AI** is a Godot 4 Editor Plugin that generates complete game scenes from plain text prompts using AI. Type a description, click Execute — nodes are created, scripts are written, and your scene is ready.

No drag-and-drop. No boilerplate. Just describe what you want.

---

## Before / After

<div align="center">

**Without ZEROX AI**

<img src="Assets/Images/before.jpg" width="80%" alt="Before — Empty Godot scene" />

<br/><br/>

**With ZEROX AI**

<img src="Assets/Images/after.jpg" width="80%" alt="After — AI generated scene with nodes and scripts" />

</div>

---

## How It Works

```
User writes prompt
        |
        v
ZEROX AI Panel (Godot Plugin)
        |
        v
API call to AI model (OpenAI / Claude / Gemini / Mistral / Groq / any compatible)
        |
        v
AI returns structured scene data
        |
        v
Script sanitizer validates output
        |
        v
GDScript executes in Godot Editor
        |
        v
Nodes created + scripts attached
        |
        v
Scene is ready
```

---

## Features

| Feature | Description |
|---|---|
| **AI Scene Generation** | Describe any 2D or 3D scene in plain text and it builds automatically |
| **Auto Node Creation** | Adds MeshInstance3D, DirectionalLight3D, Camera3D, CharacterBody3D, and more |
| **Script Generation** | Writes and attaches GDScript to nodes automatically |
| **Script Sanitization** | AI output is validated before execution — no broken code runs |
| **Built-in Inspector Panel** | Clean UI with API Key input, prompt field, status, and response output |
| **Universal API Support** | Works with any AI API — OpenAI, Claude, Gemini, Mistral, Groq, DeepSeek, and more |
| **One-Click Execute** | Single button triggers the entire scene generation pipeline |

---

## Repository Structure

```
ZEROX-AI-GODOT-ADDONS-/
|
|-- Assets/
|   |
|   |-- Images/
|   |   |-- before.jpg          # Scene before using ZEROX AI
|   |   `-- after.jpg           # Scene after AI generation
|   |
|   `-- Source/
|       `-- addons.zip          # The addon package — download this
|
`-- README.md
```

---

## Installation

### Step 1 — Download Godot 4

ZEROX AI requires Godot Engine 4.x.

<div align="center">

[![Download Godot 4](https://img.shields.io/badge/Download_Godot_4-478cbf?style=for-the-badge&logo=godot-engine&logoColor=white)](https://godotengine.org/download)

</div>

---

### Step 2 — Download the Addon

<div align="center">

[![Download addons.zip](https://img.shields.io/badge/Download_addons.zip-8b9cf4?style=for-the-badge&logo=github&logoColor=white)](https://github.com/zeroxn8877021/ZEROX-AI-GODOT-ADDONS-/raw/main/Assets/Source/addons.zip)

</div>

Or clone the repository:

```bash
git clone https://github.com/zeroxn8877021/ZEROX-AI-GODOT-ADDONS-.git
```

---

### Step 3 — Add to Your Godot Project

Extract `addons.zip` into your project's `addons/` folder:

```
YourGodotProject/
`-- addons/
    `-- zerox_ai/
        |-- plugin.cfg
        `-- ...
```

If the `addons/` folder does not exist, create it manually in your project root.

---

### Step 4 — Enable the Plugin

```
1. Open Godot
2. Go to:  Project  >  Project Settings  >  Plugins
3. Find "ZEROX AI" in the plugin list
4. Toggle the checkbox to Enable
5. The "Zerox" tab will appear in the top-right Inspector area
```

---

### Step 5 — Get an API Key

ZEROX AI accepts API keys from all major AI providers. Paste any key and it works.

| Provider | Models | Get API Key |
|---|---|---|
| OpenAI | GPT-4o, GPT-4, GPT-3.5 | https://platform.openai.com/api-keys |
| Anthropic | Claude 3.5, Claude 3 Opus | https://console.anthropic.com |
| Google | Gemini 1.5 Pro, Gemini Flash | https://aistudio.google.com/app/apikey |
| Mistral AI | Mistral Large, Mixtral | https://console.mistral.ai |
| Groq | LLaMA 3, Mixtral (fast) | https://console.groq.com/keys |
| DeepSeek | DeepSeek Coder, DeepSeek Chat | https://platform.deepseek.com |
| Together AI | 50+ open-source models | https://api.together.xyz |
| Cohere | Command R+ | https://dashboard.cohere.com/api-keys |

Any OpenAI-compatible API endpoint is supported.

---

### Step 6 — Use ZEROX AI

```
1. Click the "Zerox" tab in the Godot Editor (top-right)
2. Paste your API Key in the API Key field
3. Type your prompt in Enter Prompt
4. Click  EXECUTE ZEROX
5. Watch the scene build itself in the Scene Tree

Status bar will confirm:
  "Script generated & sanitized. | Created X nodes."
```

---

## Example Prompts

```
# 3D Scene with lighting and animation
Create a 3D scene with DirectionalLight3D, a WorldEnvironment,
and a Cube (MeshInstance3D) at center. Add a rotation script to the cube.

# Player character
Create a CharacterBody3D player with collision shape and basic WASD movement script.

# Environment setup
Add a sky with sun, fog, and ambient lighting to the current scene.

# Platformer level
Create a platform level with 5 StaticBody3D platforms at different heights.

# HUD / UI
Create a HUD with a health bar, score label, and pause button using Control nodes.
```

---

## Requirements

| Item | Requirement |
|---|---|
| Godot Engine | 4.x (tested on 4.6.3 stable) |
| Internet | Required for AI API calls |
| API Key | Any major AI provider — OpenAI, Claude, Gemini, Mistral, Groq, DeepSeek, and more |
| OS | Windows, Linux, macOS | Android 

---

## Troubleshooting

**Addon not visible in Project Settings > Plugins**

Verify the folder structure is correct and `plugin.cfg` exists at:
```
res://addons/zerox_ai/plugin.cfg
```
Restart Godot and check again.

---

**EXECUTE ZEROX does nothing**

- Confirm the API Key is pasted correctly with no extra spaces
- Check your internet connection
- Open the Output panel at the bottom of Godot for error messages

---

**Nodes created but no script attached**

Be more specific in your prompt:

```
Add a GDScript rotation script to the cube node.
```

---

## Credits

| Role | Name | GitHub |
|---|---|---|
| Lead Developer | Paras Sharma | [@zeroxn8877021](https://github.com/zeroxn8877021) |
| Team | Zerox | [github.com/zeroxn8877021](https://github.com/zeroxn8877021) |

---

<div align="center">

![Stars](https://img.shields.io/github/stars/zeroxn8877021/ZEROX-AI-GODOT-ADDONS-?style=for-the-badge&color=ffd700&logo=github&label=Star+this+repo)

[![Follow](https://img.shields.io/github/followers/zeroxn8877021?style=for-the-badge&logo=github&color=8b9cf4&label=Follow+zeroxn8877021)](https://github.com/zeroxn8877021)

</div>

---

```
MIT License
Copyright (c) 2026 Paras Sharma / Team Zerox
```

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=120&section=footer&text=Team+Zerox&fontSize=20&fontColor=8b9cf4&fontAlignY=65&animation=twinkling" width="100%" />
</div>
