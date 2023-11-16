# Human code
## ES.8  CONTARE I POSTI A TAVOLA DI 2 IN 2
<h4>Variabili:</h4> 
n = quante volte conto di due in due. Quindi se n=1 ho contato 2 coperti, se n=4 ho contato 8 coperti.<br>
N = numero di coperti necessari per il pranzo
<h4>Soluzione:</h4>

    SE  n <= N/2  ALLORA    aggiungo a tavola [N – (n*2)] coperti<br>
    ALTRIMENTI (cioè se n > N/2)     tolgo [(n*2) – N] coperti


## Es.11  GIOCO DEL BLACKJACK

<h4>Variabili:</h4>
c1, c2 =  le carte del giocatore<br>
b1, b2 = le carte del banco<br>
C = somma di c1+c2+cn<br>
B = somma di b1+b2+bn
<h4>Soluzione:</h4>

	SE   c1 + c2 <= 20    ALLORA     show-cards
		SE      b1+b2<17     ALLORA    (loop)banco gira n-carte UNTIL  b1+b2+bn >= 17
			SE   17<B<21    AND    c1 + c2 >= B     ALLORA    win    
			ALTRIMENTI    (loop)giocatore  gira n-carte  UNTIL c1+c2+cn >= B
				SE   C > 21   lost
				ALTRIMENTI    win 
		ALTRIMENTI  
			SE   C >= B    ALLORA   win
			ALTRIMENTI   (loop)giocatore  gira n-carte  UNTIL c1+c2+cn >= B
				SE   C > 21   lost
				ALTRIMENTI    win 
	ALTRIMENTI (cioè se c1 + c2 >20, quindi solo 10+11 è possibile) win



