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
        
Crear cada elipse y ponerle el tiempo de desplazamiento:

    ellipse(width / 5 , vertical_position , 20, 20)
    
    if vertical_position > height:
       vertical_position = 0 
    else:
        vertical_position = map(second(),0,60, 0, height) 
        
    fill(map(second(), 0 ,3600 , 300 ,0))
    
    ellipse(width / 3 , vertical_position_2 , 30, 30)
    
    
    if vertical_position_2 > height:
       vertical_position_2 = 0 
    else:
        vertical_position_2 = map(second(),0,3600, 0, height) 
             
    ellipse(width / 1.5 , vertical_position_3 , 40, 40)
    
    if vertical_position_3 > height:
        vertical_position_3 = 0 
    else:
        vertical_position_3 = map(second(),0,86400, 0, height)

