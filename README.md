El joc del Tic Tac Toe, també conegut com a tres en ratlla, és un joc per a dos jugadors que juguen sobre un tauler quadrat de 3x3 caselles. 
Els jugadors van col·locant una fitxa cada cop i l'objectiu és aconseguir una línia de tres fitxes, tant en horitzontal, vertical o diagonal.

Aquest és un programa Java que implementa el joc del Tic Tac Toe perquè el jugador jugui contra una màquina aleatòria.

Descarga/Instalació

Per a poder jugar aquest joc, necesitem JDK. Descarguem el programa i l'únic que necesitem per a que funcioni és obrir la terminal, localitzar el .java del programa, 
i finalment escriure a la terminal "java ticTacToe.java".

Funcionament

A l'iniciar el programa, es crea una matriu de 3x3 per representar el tauler del joc. El tauler es mostra per pantalla i les cel·les estan marcades com a buides (-3).

Després, es crida el mètode iniciJoc que inicialitza totes les cel·les del tauler amb el valor -3 per indicar que estan buides.

A continuació, s'entra en un bucle infinit que fa que el jugador i la màquina vagin col·locant les seves fitxes alternativament, fins que algú guanya o hi ha empat.

Per cada iteració del bucle, es crida el mètode tirJugador perquè el jugador entri la seva jugada per teclat, després es mostra el tauler per pantalla 
i després es crida el mètode tirContrincant que simula la jugada de la màquina.

El mètode tirContrincant genera coordenades aleatòries fins que troba una cel·la buida i hi col·loca una fitxa.

El programa es continua executant fins que es produeix un guanyador o hi ha empat, en quin cas es mostra el missatge corresponent i es tanca el programa.

Funcions

iniciJoc(int[][] taulerJoc)
Aquesta funció inicialitza totes les cel·les del tauler amb el valor -3 per indicar que estan buides.

imprimirTauler(int[][] taulerJoc)
Aquesta funció mostra el tauler del joc per pantalla amb les fitxes del jugador i la màquina.

crossOrCircle(int i)
Aquesta funció retorna la fitxa que correspon a cada casella del tauler (-3, 0 o 1).

tirContrincant(int[][] taulerJoc)
Aquesta funció simula la jugada de la màquina. Genera coordenades aleatòries fins que troba una cel·la buida i hi col·loca una fitxa.

tirJugador(int[][] taulerJoc)
Aquesta funció demana al jugador que entri la seva jugada per teclat i hi col·loca la fitxa corresponent.

main(String[] args)
La funció principal que executa el joc. Inicialitza el tauler, mostra el tauler inicial per pantalla i entra en el bucle infinit que fa que el jugador 
i la màquina juguin alternativament fins que es produeix un guanyador o hi ha empat.

