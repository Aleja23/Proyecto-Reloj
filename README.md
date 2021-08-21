# Proyecto-Reloj
Agregar las variables
 vertical_position = 0
 vertical_position_2 = 0
 vertical_position_3 = 0
 
dentro del def setup :
agregar variables globales
    global vertical_position
    global vertical_position_2
    global vertical_position_3
    
despues poner un background:
 background(map(second(),0,60,0,300))
    noStroke()
    fill(map(second(), 0 ,59 , 300 ,0))
        


