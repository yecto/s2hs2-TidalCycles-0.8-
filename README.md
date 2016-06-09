# s2hs2-TidalCycles-0.8-
's2hs2', una interfaz para comunicacion OSC entre TidalCycles y Processing. A traves de ella una forma visual puede ser asignada a cada letra del teclado en la computadora visualizando patrones de palabras (formas visuales) enviados desde Tidal.

Instrucciones:

- Para correr s2hs2 lo primero que necesitamos es instalar TidalCycles, aquí podemos seguir algunos sencillos pasos: http://tidalcycles.org/getting_started.html

- Debemos estar seguros que hemos instalado Haskell, TidalCycles y el editor de texto de su elección (Atom, Emacs, etc).

- Ahora necesitamos instalar Processing, en el siguiente enlace es muy sencillo descargar la versión más adecuada para nuestro sistema operativo - https://processing.org/download/?processing

- Ya instalado lo anterior, abrirémos Atom lo primero que necesitamos en caso de no haberlo hecho antes, es instalar el paquete "tidalcycles", el cual podemos buscar en las Preferencias de Atom y después en la pestaña de "+Install" ya instalado, necesitamos reiniciar Atom.

- Con Atom de nuevo en nuestra pantalla, abrirémos nuestro archivo cruel_laberinto.tidal 

- Ahora necesitamos instalar y abrir Processing, así que procederemos a abrir un archivo nuevo de processing que llamaremos comotuquieras.pde - ahora le daremos guardar - y arrojaremos nuestra carpeta 'Data' dentro de la carpeta que 
Processing ha generado para nuestro archivo, más tarde en nuestro sketch copiaremos y pegaremos lo que encontramos 
aquí en el archivo 'themucusoffmybrain.pde', ahora necesitamos crear una nueva pestaña llamada 'Letters' en donde copiaremos y pegaremos lo que encontramos aquí en 'Letters.pde' y por último necesitamos crear una nueva pestaña llamada 'Thing',
en donde de igual manera necesitamos copiar y pegar lo que aquí encontramos en 'Thing', corremos el sketch con 'ctrl o cmd + R' y ahora estamos listos para ir a TidalCycles.

- Ahora volvemos a Atom y booteamos TidalCycles - 'Packages' - 'TidalCycles' - 'Boot TidalCycles'

- Evaluamos la primer línea de código 'import Sound.Tidal.OscStream' con shift + enter.

- Las siguientes líneas de código sirven para establecer la conexión OSC entre TidalCycles y Processing, por lo que 
necesitan ser evaluadas con ctrl + enter - desde 'let poetry = Shape {' - hasta - 'str = makeI poetry "str"'

- Ahora evaluamos por separado cada línea de código de nuestro archivo.

Y por último evaluamos con ctrl + enter nuestro patrón de formas visuales - 

p1 $ word "h o l a m u n d o" # x "0.1 0.2 0.3 0.4 0.5 0.6 0.7 0.8 0.9" # life "12" # r "0" # g (slow 2 $ scale 0 255 sine) # b "155"

- Si todo ha salido bien, en nuestro cuadrado de Processing comenzaremos a visualizar lo que hemos evaluado en TidalCycles.

- Ahora si a live codear y a divertirnos ( .

