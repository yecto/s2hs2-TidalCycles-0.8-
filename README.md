# s2hs2-TidalCycles-0.8-
's2hs2' es una interfaz para comunicacion OSC entre TidalCycles y Processing. A traves de ella una forma visual puede ser asignada a cada letra del teclado en la computadora visualizando patrones de palabras (formas visuales) enviados desde Tidal. 's2hs2' es un proyecto colaborativo desarrollado por Alex McLean y Rodrigo Velasco en enero de 2015 en la Escuela de Música de la Universidad de Leeds. 

s2hs2 is an interface between TidalCycles and Processing. A visual form can be assigned to each letter on the computer keyboard, visualising patterns of words (visual forms) sent from Tidal. s2hs2 is a collaborative project undertaken by Rodrigo Velasco and Alex McLean in January 2015 in the School of Music, University of Leeds.

Instrucciones / Instructions:

- Para correr s2hs2 lo primero que necesitamos es instalar TidalCycles, aquí podemos seguir algunos sencillos pasos: http://tidalcycles.org/getting_started.html
- To run s2hs2 first we need to install TidalCycles, here we can follow some easy steps:
http://tidalcycles.org/getting_started.html

- Debemos estar seguros que hemos instalado Haskell, TidalCycles y el editor de texto de tu elección (Atom, Emacs, etc). Recomendamos Atom por su sencillez para ser instalado ( .
- We must be sure we have installed Haskell, Tidal Cycles and the text editor of our choice (Atom, Emacs, etc). Atom recommended for its simplicity to be installed (.

- Ahora necesitamos instalar Processing, en el siguiente enlace es muy sencillo descargar la versión más adecuada para nuestro sistema operativo - https://processing.org/download/?processing
- Now we need to install Processing, the following link is very simple download the appropriate version for your operating system - https://processing.org/download/?processing

- Ya instalado lo anterior, abrirémos Atom lo primero que necesitamos en caso de no haberlo hecho antes, es instalar el paquete "tidalcycles", el cual podemos buscar en las Preferencias de Atom y después en la pestaña de "+Install" ya instalado, necesitamos reiniciar Atom.
- Already installed the above, we will open Atom, first thing we need in case of not having done it before, is to install the "tidalcycles" which can search in Atom Preferences and then the tab "+ Install" when the package is installed, we need to restart Atom.

- Con Atom de nuevo en nuestra pantalla, abrirémos nuestro archivo 'cruel_laberinto.tidal' 
- With Atom back on our screen, we will open our 'cruel_laberinto.tidal' file

- Ahora necesitamos instalar y abrir Processing; descomprimir el archivo 's2hs2tidalcycles08.zip' y dar doble click sobre el archvo 's2hs2tidalcycles08.pde', lo que desplegará un sketch con 3 pestañas 's2hs2tidalcycles08', 'Letters' y 'Thing', ahora debemos correr éste archivo, dando play o presionando 'ctrl o cmd + enter'.
- Now we need to install and open Processing; uncompress the 's2hs2tidalcycles08.zip' file and double click on the file 's2hs2tidalcycles08.pde', which display a sketch with 3 tabs 's2hs2tidalcycles08', 'Letters' and 'Thing', now must run this file, giving play or pressing 'ctrl or cmd + enter'.

- Ahora volvemos a Atom y booteamos TidalCycles - 'Packages' - 'TidalCycles' - 'Boot TidalCycles'.
- Now we turn back to Atom and boot TidalCycles - 'Packages' - 'Tidal Cycles' - 'Boot TidalCycles'.

- Evaluamos la primer línea de código 'import Sound.Tidal.OscStream' con shift + enter.
- Evaluate the first line of code 'import Sound.Tidal.OscStream' with shift + enter.

- Las siguientes líneas de código sirven para establecer la conexión OSC entre TidalCycles y Processing, por lo que 
necesitan ser evaluadas con ctrl + enter - desde 'let poetry = Shape {' - hasta - 'str = makeI poetry "str"'.
- The following lines of code used to establish the OSC interconnection between TidalCycles and Processing, so
they need to be evaluated with 'ctrl + enter' - from 'let poetry = Shape {' - until - 'str = makeI poetry "str"'.

- Ahora evaluamos por separado las siguientes líneas de código de nuestro archivo.
- - Now we evaluate separately the following lines of code in our archive.

- Y por último evaluamos con 'ctrl + enter' nuestro patrón de palabras (formas visuales): 
- - And finally we need to evaluate with 'ctrl + enter' our pattern of words (visual forms):

p1 $ word "h o l a m u n d o" # x "0.1 0.2 0.3 0.4 0.5 0.6 0.7 0.8 0.9" # life "12" # r "0" # g (slow 2 $ scale 0 255 sine) # b "155"

- Si todo ha salido bien, en nuestro cuadrado de Processing comenzaremos a visualizar lo que hemos evaluado en TidalCycles.
- If all went well, in our Processing window, we begin to visualize what we have evaluated in TidalCycles.

- Ahora si a live codear y a divertirnos ( .
- Now is time to live code and put the funk into functions! ( .
