# SystemGPT
Control your computer using ChatGPT-3.5-turbo in a token efficient way. Edit `prompt` to provide more details about your system. This is very much new software. PRs and issues welcomed!
The program works by asking ChatGPT to write python code and then running that code, with a special prompt so you can ask gpt directly to interface with your computer. It also automatically installs the modules SystemGPT needs using pipreq. The prompt is currently for Fedora, a Linux distribution, but many things will work regardless and you should be able to change the prompt and bashRun() to work with your operating system.

SystemGPT will sometimes glitch and give an incorrect answer or refuse to give one. This will be improved, but for now just reword and/or try again. There are some planned ways to fix some of this, like improving the prompt, using venv to avoid dependency issues and only using package versions that meet the training data cutoff (especially usfeful for turtle.Terminator), and more.

There are some other programs that do some similar things, like AutoGPT. This has a slightly different goal (Instead of running continously, you ask it to do specific things), uses less tokens, and is better if you don't have access to or can't afford gpt-4 (More token efficient). This project has only just gotten started, and will hopefully have more features that make it a worthy program to use.
# Installation
Install by running the following: (On Linux, Macos or WSL, windows might be a bit different, also make sure you have python3 and pip3)
```bash
pip install openai pipreqs
```
and then cloning the repo or downloading from releases. Make sure to put your openai API key into sysGPT.py.
Run with `python sysGPT.py`.
# If you don't know what to ask the ai, try:
- Make a pdf called appleTutorial.pdf demonstrating how to eat apples.
- Download https://upload.wikimedia.org/wikipedia/en/9/9a/Among_Us_cover_art.jpg and flip it vertically. (You can also say flip among_us.jpg vertically if you have it downloaded and in the same folder)
- Install OBS studio. (will only work if you're running fedora or change the prompt/maybe some code)
- Draw "ChatGPT is cool!" 10 times in large bold blue text.
- Make 10 files named "NeverGonnaGiveYouUp", "NeverGonnaGiveYouU", "NeverGonnaGiveYou"... in a new folder called Rick Astley. The file contents should be a number from 1-10.
- Open the Wikipedia article about snakes.
