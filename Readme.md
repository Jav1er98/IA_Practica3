## Práctica 3: Modificación del proyecto RobotGuard.
## Objetivo: Modificar el proyecto de RobotGuard para hacer el que el NPC vuelva a la última posición donde vio al jugador antes de huir. Debe volver después de que su salud se haya recuperado por encima de 40.

1. He creado 2 Tasks dentro del script AI.cs, primero "SaveLastKnownTargetPosition", se guarda la posición del jugador en el momento en que el NPC hace "Flee":

      ![captura1](/gifs/Captura1.png)
      
2. La segunda Task "SetLastKnownTargetDestination" selecciona como destino la posición guardada:

      ![captura2](/gifs/Captura2.png)
   
3. En el árbol de comportamiento añado "SetLastKnownTargetDestination" dentro de "Flee" (momento en que sale huyendo del jugador):
       
      ![captura3](/gifs/Captura3.png)
       
4. Resultado:

      ![gif ejercicio 5](/gifs/gif.gif)
      

