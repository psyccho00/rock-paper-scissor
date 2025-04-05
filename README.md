# ✊🤚✌️ Rock-Paper-Scissors Game

Welcome to the **Rock-Paper-Scissors Game** repository! This project is a simple yet interactive command-line game implemented in Python. Challenge the computer in this classic game and see if you can outsmart it.


![](https://github.com/psyccho00/rock-paper-scissor/blob/main/SPC.png)
---

## 📂 Repository Structure

```
rock-paper-scissor/
│
└── main.py   # The main script containing the game logic
```

---

## 🎮 How to Play

1. **Run the Game**: Execute the `main.py` script.
2. **Choose Your Move**: Input your choice - 'rock', 'paper', or 'scissors'.
3. **Computer's Turn**: The computer randomly selects its move.
4. **Result Announcement**: The game announces the winner based on the choices.
5. **Replay Option**: Choose to play again or exit the game.

**Winning Rules**:
- **Rock vs Scissors**: Rock wins.
- **Scissors vs Paper**: Scissors win.
- **Paper vs Rock**: Paper wins.

---

## 🚀 Getting Started

### Prerequisites

- Python 3.x installed on your system.

### Installation

```bash
git clone https://github.com/psyccho00/rock-paper-scissor.git
cd rock-paper-scissor
python main.py
```

---

## 🧩 Code Breakdown

### `main.py` – Game Logic

This script manages the entire game flow, from user input to determining the game's outcome.

**Key Components**:

- **Imports**:

```python
import random
```

- *Purpose*: Utilizes Python's built-in `random` module to allow the computer to make random choices.

- **Game Variables**:

```python
choices = ['rock', 'paper', 'scissors']
```

- *Purpose*: Defines the possible choices for both the player and the computer.

- **Game Loop**:

```python
while True:
    player_choice = input("Enter rock, paper, or scissors: ").lower()
    if player_choice not in choices:
        print("Invalid choice. Please try again.")
        continue

    computer_choice = random.choice(choices)
    print(f"Computer chose: {computer_choice}")

    if player_choice == computer_choice:
        print("It's a tie!")
    elif (player_choice == 'rock' and computer_choice == 'scissors') or          (player_choice == 'scissors' and computer_choice == 'paper') or          (player_choice == 'paper' and computer_choice == 'rock'):
        print("You win!")
    else:
        print("You lose!")

    play_again = input("Do you want to play again? (yes/no): ").lower()
    if play_again != 'yes':
        break
```

- *Purpose*: Manages the game's flow with:
  - **User Input** and validation
  - **Random Computer Choice**
  - **Result Evaluation**
  - **Replay Prompt**

---

## 🌟 Features

- ✅ Interactive command-line interface
- ✅ Input validation
- ✅ Randomized computer decisions
- ✅ Continuous play until user exits

---

## 🛠️ Potential Enhancements

- Add score tracking
- Add a GUI version using tkinter or PyGame
- Expand the game to include Rock-Paper-Scissors-Lizard-Spock

---

## 📸 Sample Gameplay

```
Enter rock, paper, or scissors: rock
Computer chose: scissors
You win!
Do you want to play again? (yes/no): yes
Enter rock, paper, or scissors: paper
Computer chose: rock
You win!
Do you want to play again? (yes/no): no
```

---

## 👨‍💻 Author

Created by [@psyccho00](https://github.com/psyccho00)

If you enjoyed this project, give it a ⭐ on GitHub!

---

Enjoy the game and may the odds be ever in your favor! ✨
