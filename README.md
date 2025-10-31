# 🐍 Day 20 & Day 21 — Classic Snake Game (Python Turtle)

Do you remeber the snake game that used to be on the nokia phones? The snake would start out small and you move it around the screen eating "food" making it grow longer and longer. The objective was to make it get as loooong as possible without crashing into yourslef or the wall.

We recreated this nostalgic game using Python's Turtle module, creating different classes to make the snake move, eat food, grow and track the score on scree. This was a very cool project to do.

# What we learned:
**Day 20 (Part 1)** We built the foundation of the game:
- Set up the screen window and game environment
- Created the snake body and animated the segments
- Built a `Snake` class and moved to Object-Oriented Programming
- Mapped keyboard keypresses to control the snake (Up, Down, Left, Right)
- Learned that programming isn’t memorising but it's understanding logic + Googling smartly

**Day 21 (Part 2)** We expanded the game with real mechanics:
- **Class Inheritance** — Scoreboard class inherits from Turtle 🧠
- Detecting **collisions with food**
- Making the snake grow when it eats 🐍➕
- Creating a scoreboard and updating score
- Saving **high score to a text file**
- Detecting wall collisions
- Detecting collisions with your own tail 😭 (self-sabotage energy)
- Learning to **slice lists & tuples** in Python and why that's useful

## 🧾 How the Code Works (Simple Breakdown)

The game is cleanly organized into **three classes**:

✅ `Snake` Class (handles everything about the snake)
- Builds the initial snake body
- Moves each segment forward (by following the segment ahead of it)
- Extends the snake when it eats
- Resets when you crash (by hiding the old segments and making new ones)
- Handles key movements (up, down, left and right)

✅ `Food` Class (creates the food the snake eats)
- Creats the food in a turtle shape (so cute btw 🐢)
- Randomly teleports to new coordinates when eaten
- Makes gameplay unpredictable & challenging

✅ `Scoreboard` Class (handles score display and saving high score)
- Shows score at the top of the screen
- Inherits from `Turtle`
- Updates score when food is eaten
- Reads & writes high scores to `data.txt`
- Resets score on game over without closing game

✅ Inside `main.py` we control the game flow:
- Create screen, snake, food & scoreboard
- Keep updating screen so animation looks smooth
- Move snake continuously
- Check if snake touches food → extend + update score
- Check if snake hits walls → reset game
- Check if snake hits its own tail → reset game
- Exit when clicking screen


