import turtle

# Create a turtle object
my_turtle = turtle.Turtle()

# Set the turtle's speed
my_turtle.speed(100)  # Fastest speed

# Set the turtle's color
my_turtle.color("red")

# Function to handle key presses
def move_forward():
    my_turtle.forward(10)

def move_backward():
    my_turtle.backward(10)

def turn_left():
    my_turtle.left(15)

def turn_right():
    my_turtle.right(15)

# Bind functions to key presses
screen = turtle.Screen()
screen.listen()
screen.onkey(move_forward, "Up")
screen.onkey(move_backward, "Down")
screen.onkey(turn_left, "Left")
screen.onkey(turn_right, "Right")

# Keep the window open
turtle.done()
