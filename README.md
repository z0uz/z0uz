- 👋 Hi, I’m @z0uz
- 👀 I’m interested in python.
- i am a Cybersecurity specialist and a data analyst.
- 💞️ looking to collaborate on sharing progamming tips using python language.
- my tryhackme profile: https://tryhackme.com/p/elsiddik


```bash

import turtle

t = turtle.Turtle()
s = turtle.Screen()
s.bgcolor("black")
t.speed(0)  # Increase speed to the maximum
t.pensize(2)
t.pencolor("white")

def s_curve():
    for i in range(45):  # Reduce the number of points in the curve
        t.left(2)  # Increase the angle to make the curve smoother
        t.forward(2)  # Increase the forward distance

def r_curve():
    for i in range(45):  # Reduce the number of points in the curve
        t.right(2)  # Increase the angle to make the curve smoother
        t.forward(2)  # Increase the forward distance

def l_curve():
    s_curve()
    t.forward(40)  # Reduce the forward distance to make the curve smoother
    s_curve()

def l_curve1():
    s_curve()
    t.forward(45)  # Reduce the forward distance to make the curve smoother
    s_curve()

def half():
    t.begin_fill()  # Begin fill before drawing
    t.forward(25)  # Reduce the forward distance to make the curve smoother
    s_curve()
    t.forward(45)  # Reduce the forward distance to make the curve smoother
    l_curve()
    t.forward(20)  # Reduce the forward distance to make the curve smoother
    t.left(90)
    t.forward(40)
    t.right(90)
    t.forward(5)
    t.right(90)
    t.forward(60)  # Reduce the forward distance to make the curve smoother
    l_curve1()
    t.forward(15)  # Reduce the forward distance to make the curve smoother
    t.left(90)
    t.forward(25)
    r_curve()
    t.forward(20)  # Reduce the forward distance to make the curve smoother
    t.end_fill()  # End fill after drawing

def get_pos():
    t.penup()
    t.forward(20)
    t.right(90)
    t.forward(10)
    t.right(90)
    t.pendown()

def eye():
    t.penup()
    t.right(90)
    t.forward(160)
    t.left(90)
    t.forward(70)
    t.pencolor("black")
    t.dot(35)

def sec_dot():
    t.left(90)
    t.penup()
    t.forward(310)
    t.left(90)
    t.forward(120)
    t.pendown()
    t.dot(35)

t.fillcolor("#306998")
half()  # Only call the half function once, and it will draw the whole logo
get_pos()
t.fillcolor("#FFD43B")
half()  # Only call the half function once, and it will draw the whole logo

eye()
sec_dot()

t.hideturtle()  # Hide the turtle for a cleaner look
turtle.done()```
<!---
z0uz/z0uz is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
