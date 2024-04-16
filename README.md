import turtle

# Pencereyi ayarla
wn =turtle.Screen()
wn.setup(width=600, height=600)
wn.bgcolor("white")

# Kalp çizimi fonksiyonu
def draw_heart():
    turtle.penup()
    turtle.goto(0,-200)
    turtle.pendown()
    turtle.color("red","red")
    turtle.begin_fill()
    turtle.left(140)
    turtle.forward(224)
    for _ in range(200):
        turtle.right(1)
        turtle.forward(2)
    turtle.left(120)
    for _ in range(200):
        turtle.right(1)
        turtle.forward(2)
    turtle.forward(224)
    turtle.end_fill()

# Çizimi yap
turtle.speed(2)
draw_heart()
turtle.hideturtle()

# Pencereyi kapat
wn.mainloop()
