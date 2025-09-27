<p align="center">
  <img src="https://github.com/user-attachments/assets/c46fb7d1-80e3-4f68-a6ac-84ab6194f346" alt="Stroop Test Screenshot" width="600">
</p>

# Stroop Test Game

A cognitive psychology experiment built in Python using Pygame, designed to measure reaction time and cognitive interference (based on the classic Stroop effect).

---

## How It Works

Participants see a color word (for example RED or GREEN) shown in a font color that may match or conflict with the word. The task is to **click the button that matches the font color, not the word**.

For each trial the app records:
- Reaction time
- Correct vs incorrect response
- Trail number
- Average reaction time

A session summary is printed at the end of the run.

---

## Requirements

- Python
- [Pygame](https://www.pygame.org/)

Install:

```
pip install pygame
```

## Quick start

```
git clone https://github.com/sayuj0/stroop-test.git
cd stroop-test
python stroop_test.py
```

## Configuration
- **Number of trails**: inside the **main** block, edit:
```
stroop_test.run_test(trials=4)
```
- Default design: randomized mix of congruent and incongruent trials with clickable color buttons
- Timing: reaction time is measured from stimulus onset to click using Pygame timing
- GUI: single screen with large clickable buttons for mouse-based responses
  
## Output data
By default results are saved to reaction_times.txt in the project directory.
<p>
  <img src="https://github.com/user-attachments/assets/aab865ab-e982-494a-b7de-b54b3486c5d5" alt="Stroop Test Screenshot 2" width="600">
</p>

## Research notes
- Stroop effect: people are slower and less accurate when the word and its font color conflict. This app captures interference through per-trial RT and accuracy.
- Timing precision: Pygame timers are suitable for classroom and undergraduate research. For strict millisecond control across machines, document refresh rate and reduce background load.

## Features
- Clean Pygame UI
- Text input for paticipant ID
- Randomized congruent vs incongruent trials
- Click responses with sub-second timing
- Per-trial logging plus a session summary

## Roadmap
- Export to SQLite database
- Configurable congruent ratio and ITI
- Practice block and simple exclusion rules
- On-screen consent text and an optional pause screen

## License
This project is licensed under the **MIT License**.
Feel free to use, modify, and share it.
