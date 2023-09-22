#Importas la librerias
from turtle import*
import colorsys

#Agregar texto
penup()
goto(0,310)#posición donde deseas agregar el texto
pendown()
color("light yellow")#color del texto
write("BUENOS DIAS MI NIÑA HERMOSA", align="center", font=("Stencil",11,"italic"))
#color de fondo
speed(20)
bgcolor("black")
h=0

#Armado de tallo
penup()
goto(0,-100)
pendown()
color("green")# Pueden cambiar el color
begin_fill()
rt(90)
fd(400)
lt(90)
fd(20)
lt(90)
fd(400)
lt(90)
fd(20)
end_fill()

#Armado de los petalos
penup()
goto(0,0)
pendown()
for i in range(16):
    for j in range(18):
        color("yellow")
        h += 0.005
        rt(90)
        circle(150-j*6,90)
        lt(90)
        circle(150-j*6,90)
        rt(180)
    circle(40,24)

 #Armado del boton   
penup()
goto(-20,0)
pendown()
color("brown")
begin_fill()
circle(44)
end_fill()
done()

 #Disfruten su dia
