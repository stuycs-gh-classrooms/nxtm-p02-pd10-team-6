[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/jiVqpuMN)
[![Open in Codespaces](https://classroom.github.com/assets/launch-codespace-2972f46106e565e64193e422d61a12cf1da4916b45550586e14ef0a7c637dd04.svg)](https://classroom.github.com/open-in-codespaces?assignment_repo_id=22153756)
# NeXtCS Final Project
### Name 0: bryan

### Project Description
Provide a high-level description of your project. Include explanatory links if you think they will be helpful.

gonna make a game where you control a little square that moves around and shoots bullets at circle enemies that try to kill you by touching you.
might add some more stuff if i have time such as power ups, score, and different enemy types.

### Skill Usage
Explain what skills from this semester you will be using in this project, and how they will be used.

Using Processing to create a graphical program. (game)
Using keyboard/mouse for input. (moving and shooting)
Writing classes. (All projects must include at least 2 Thinker-written classes) (player class, bullet class and enemy class)
1-dimensional arrays. (storing player and enemy positions)
2-dimensional arrays. (game area)


### Controls
How will your program be controlled? List all keyboard commands and mouse interactions.

wasd for movement, space to shoot

Keyboard Commands:
- LIST OF COMMANDS HERE

Mouse Control:
- Mouse movement: nah
- Mouse pressed: nah


### Classes
What classes will you be creating for this project? Include the instance variables and methods that you believe you will need. You will be required to create at least 2 different classes. If you are going to use classes similar to those we've made for previous assignments, you will have to add new features to them.

i will have a player class, bullet class, and an enemy class.

class Player {
  float x, y; // positiom of the player
  float speed;

  Player(float startX, float startY) {
    x = startX;
    y = startY;
    speed = 5;
  }

  void keyPressed() {
    if (key == 'w') { // up
      y -= speed;
    } else if (key == 's') { // down
      y += speed;
    } else if (key == 'a') { // left
      x -= speed;
    } else if (key == 'd') { // right
      x += speed;
    }
  }

  void display() {
    fill(255, 0, 0);
    square(x, y, 30); // draw the player as a square
  }
}

class Bullet {
}

class Enemy {
}

