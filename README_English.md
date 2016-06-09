# s2hs2-TidalCycles-0.8-

s2hs2 is an interface between TidalCycles and Processing. A visual form can be assigned to each letter on the computer keyboard, visualising patterns of words (visual forms) sent from Tidal. s2hs2 is a collaborative project undertaken by Rodrigo Velasco and Alex McLean in January 2015 in the School of Music, University of Leeds.

Instructions:

- To run s2hs2 first we need to install TidalCycles, here we can follow some easy steps:
http://tidalcycles.org/getting_started.html

- We must be sure we have installed Haskell, Tidal Cycles and the text editor of our choice (Atom, Emacs, etc). Atom recommended for its simplicity to be installed (.

- Now we need to install Processing, the following link is very simple download the proper version for your operating system - https://processing.org/download/?processing

- Already installed the above, we will open Atom, first thing we need in case of not having done it before, is to install the "tidalcycles" package which you can search in Atom Preferences and then in the tab "+ Install" when the package is installed, we need to restart Atom.

- With Atom back on our screen, we will open our 'cruel_laberinto.tidal' file

- Now we need to install and open Processing; uncompress the 's2hs2tidalcycles08.zip' file and double click on the file 's2hs2tidalcycles08.pde', which display a sketch with 3 tabs 's2hs2tidalcycles08', 'Letters' and 'Thing', now must run this file, giving play or pressing 'ctrl or cmd + R'.

- Now we turn back to Atom and boot TidalCycles - 'Packages' - 'Tidal Cycles' - 'Boot TidalCycles'.

- Evaluate the first line of code 'import Sound.Tidal.OscStream' with shift + enter.

- The following lines of code used to establish the OSC interconnection between TidalCycles and Processing, so
they need to be evaluated with 'ctrl + enter' - from 'let poetry = Shape {' - until - 'str = makeI poetry "str"'.

- Now we evaluate separately the following lines of code in our archive.

- And finally we need to evaluate with 'ctrl + enter' our pattern of words (visual forms):

p1 $ word "h e l l o w o r l d" # x "0.1 0.2 0.3 0.4 0.5 0.6 0.7 0.8 0.9" # life "12" # r "0" # g (slow 2 $ scale 0 255 sine) # b "155"

- If all went well, in our Processing window, we begin to visualize what we have evaluated in TidalCycles.

- Now is time to live code and put the funk into functions! ( .
