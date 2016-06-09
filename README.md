# s2hs2-TidalCycles-0.8-
's2hs2' es una interfaz para comunicacion OSC entre TidalCycles y Processing. A traves de ella una forma visual puede ser asignada a cada letra del teclado en la computadora visualizando patrones de palabras (formas visuales) enviados desde Tidal. 's2hs2' es un proyecto colaborativo desarrollado por Alex McLean y Rodrigo Velasco en enero de 2015 en la Escuela de Música de la Universidad de Leeds. 

Instrucciones:

- Para correr s2hs2 lo primero que necesitamos es instalar TidalCycles, aquí podemos seguir algunos sencillos pasos: http://tidalcycles.org/getting_started.html

- Debemos estar seguros que hemos instalado Haskell, TidalCycles y el editor de texto de tu elección (Atom, Emacs, etc). Recomendamos Atom por su sencillez para ser instalado ( .

- Ahora necesitamos instalar Processing, en el siguiente enlace es muy sencillo descargar la versión más adecuada para nuestro sistema operativo - https://processing.org/download/?processing

- Ya instalado lo anterior, abrirémos Atom lo primero que necesitamos en caso de no haberlo hecho antes, es instalar el paquete "tidalcycles", el cual podemos buscar en las Preferencias de Atom y después en la pestaña de "+Install" ya instalado, necesitamos reiniciar Atom.

- Con Atom de nuevo en nuestra pantalla, abrirémos nuestro archivo 'cruel_laberinto.tidal' 

- Ahora necesitamos instalar y abrir Processing; descomprimir el archivo 's2hs2tidalcycles08.zip' y dar doble click sobre el archvo 's2hs2tidalcycles08.pde', lo que desplegará un sketch con 3 pestañas 's2hs2tidalcycles08', 'Letters' y 'Thing', ahora debemos correr éste archivo, dando play o presionando 'ctrl o cmd + R'.

- Ahora volvemos a Atom y booteamos TidalCycles - 'Packages' - 'TidalCycles' - 'Boot TidalCycles'.

- Evaluamos la primer línea de código 'import Sound.Tidal.OscStream' con shift + enter.

- Las siguientes líneas de código sirven para establecer la conexión OSC entre TidalCycles y Processing, por lo que 
necesitan ser evaluadas con ctrl + enter - desde 'let poetry = Shape {' - hasta - 'str = makeI poetry "str"'.

- Ahora evaluamos por separado las siguientes líneas de código de nuestro archivo.

- Y por último evaluamos con 'ctrl + enter' nuestro patrón de palabras (formas visuales): 

p1 $ word "h o l a m u n d o" # x "0.1 0.2 0.3 0.4 0.5 0.6 0.7 0.8 0.9" # life "12" # r "0" # g (slow 2 $ scale 0 255 sine) # b "155"

- Si todo ha salido bien, en nuestra pantalla de Processing comenzaremos a visualizar lo que hemos evaluado en TidalCycles.

- Ahora si a live codear y a poner el funk en funkciones! ( .
