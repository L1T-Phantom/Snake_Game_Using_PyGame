# Snake_Game_Using_PyGame
A simple Snake Game in Python utilizing the PyGame package.

--- DEV LOGS ---

-- ALPHA --

v0.0.1 -> Created the screen.

v0.0.2 -> Stopped the screen from immediately closing [using while loop & event.get() function]. Also named the screen as "Snake Game by L1T Phantom" [using display.set_caption() function].

v0.0.3 -> Fixed the close button not working [using pg.quit() function].

v0.0.4 -> Created the Snake & colorized it [using draw.rect() and rgb = (x,y,z) functions].

v0.0.5 -> Added movement to the Snake [using the KEYDOWN class of PyGame]. Also created x1_change and y1_change in order to update values of the x and y coordinates.

-- BETA --

v0.0.6 -> Game Over when the Snake hits the boundaries [using an if statement that defines the x and y coordinate values to be either less than or equal to that of the screen]. Also removed hardcodes and utilized variables, to increase room for customization of the game later on.

v0.0.7 -> Addition of food [using round(random.randrange()) and draw.rect() functions], prints a message saying “Delicious!” when the Snake crosses over food [using an if statement to match the x and y coordinates of the food and the Snake and print() function]. Also, options to quit the game or to play again when the player loses have been added [using the KEYDOWN class of PyGame].

v0.0.8 -> Fixed major bugs, which didn't let the game start, and caused it to crash on opening. Also added increasing length of the Snake [by putting the length of the Snake in a list and the initial size is one block] upon eating food, and if the Snake collides with its own body, the game ends.

v0.0.9 -> Added and customized the score [using def and font_style].

-- RELEASE --

v1.0.0 -> Customized and changed the colors for the game.

---

--- REMOVED CODE SNIPPETS ---

"""

dis = pg.display.set_mode((400, 300))

pg.display.update()

pg.display.set_caption("Snake game by L1T Phantom")

green = (0, 255, 0)

game_over = False

x1 = dis_width / 2 # Previously: 300. Changed in v0.0.5.

y1 = dis_height / 2 # Previously: 300. Changed in v0.0.5.

snake_block = 10

"""

"""
x1_change = 0
y1_change = 0

clock = pg.time.Clock()
snake_speed = 30

font_style = pg.font.SysFont(None, 50)

"""

""" pg.draw.rect(dis, black, [x1, y1, snake_block, snake_block]) """

---

--- KNOWN BUGS ---

1. When starting the game, sometimes the food doesn't load (Occasional BUG)
   FIX - Either make the snake crash into the edge of the screen, and restart, until the food loads, or quit the game and reopen.

Please submit any other bugs to the GitHub repository: https://github.com/L1T-Phantom/Snake_Game_Using_PyGame.

---
