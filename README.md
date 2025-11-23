#izili-TP1  
NOM : IZILI
PRENOM : ABDELJALIL
REPONSE
1. reponse de question 1
Algorithme code_PIN
var
pin,n:entier
Début
n<-0
   tantque(n< 3)  faire 
           ecrire("entre le code pin:")
           lire(pin)
                si pin = 1234 alors
            ecrireln("succes")
            n<-n+4
                 sinon 
            ecrireln("erreur")
             n<-n+1
           finsi
   fintantque
     si n=3 alors 
              ecrireln("blocage")
     finsi      
Fin
2. reponse de question 2
Algorithme echanger_les_valeurs
var
a,b,c:entier 
Début
ecrire("entre le nombre a :")
lire(a)
ecrire("entre le nombre b:")
lire(b)
c<-a
a<-b
b<-c
ecrire("le nombre a =", a , "et le nombre b =", b)
FIN
3. exercice 3
3.1: 
Algorithme PGCD
var 
a,b,pgcd,g :entier
Début
ecrire("entre le nombre a : ")
	lire (a)
	ecrire("entre le nombre b : ")
	lire (b)
	si b=0 alors 
		    ecrire ("le pgcd  de ",a ,"et " , b, "est :" , a)
		    sinon 
		    repeter
		    g<-a 
		    a<-b
		    b<- g mod b 
		    jusqua b =0 
		    ecrire (" le pgcd de de a et b est :", a)
	finsi
Fin
3.2:
   Algorithme PGCD
fonction pgcd (a: entier, b :entier):entier
        debut
                    si b=0 alors 
                                            retourne a
                                            Sinon 
                         retourne pgcd (b ,a mod b )
                    finsi
        fin
        var 
a,b: entier        
Début 
ecrire("entre nombre")
lire (a)
ecrire("entre nombre")
lire (b)
	ecrire(" le pgcd est ", pgcd (a,b ))
Fin
3.3:
    COMPLEXITE algorithme avec boucle = O(LOG(N)) : COPLIXITE LOGARITMIQUE 
    COMPLEXITE algorithme avec fonction =O(LOG(N)) : COPLIXITE LOGARITMIQUE 
   LES DEUX COMPLEXITE SONT EGAUX
4 . exercice 4
   4.1:
Algorithme  diviseurs 
var
i,n : entier
Début
	ecrire("entre un nombre")
	lire (n)
	pour i<-1 à n pas 1 faire 
		si    n mod i =0 alors
				    ecrireln (i," est diviseur de ", n)
				    sinon 
				    ecrireln (i," pas un diveseur de", n)
		finsi
	finpour
fin
4.2:
   Algorithme  diviseurs_methode_2
var n,i ,R: entier
Début
ecrire("entre un nombre")
lire(n)
R<-racineCarree(n)
pour i <- 1 à R pas 1 faire 
    si(R mod i )=0 alors 
            ecrire (i,"   est un deviseur de  ", R )
            ecrireln("    et le père est ", R div i , "  et aussi un diviseur de   ",R)
    finsi
    
finpour
Fin
4.3: complixite de mthode 1 = o(n) : complixite liniere
     complixite de mthode 2 = o(√n) = o(n^1/2) < O(n) ALORS PLUS RAPIDE
5. EXERCICE 5
Algorithme deviner
var
n,k,A :entier
Début
A<- aleatoire(1,100)
k<-0
	tantque k<5 faire		    
		    ecrire("entre un nombre")
		    lire (n)
		    si n=A alors		    		        
		    ecrireln("correct")	
		    k<-k+10
		    sinon
		    si n>A alors 
		        		ecrireln("incorrect , trop grand ") 
		        		sinon 
		        		ecrireln ("incorrect , trop petite")	        		 
		        		k<-k+1      
		    finsi	
		    finsi		    
	fintantque
	si k=5 alors
	ecrireln	  (" le nombre est :",A)
	finsi
	ecrireln("au-revoir")
Fin
6.EXERCICE 6
Algorithme triangle
var
n,k,A :entier
Début
A<- 5
k<-0
	tantque k<5 faire		    
		    ecrire("entre un nombre")
		    lire (n)
		    si n=A alors		    		        
		    ecrireln("correct")	
		    k<-k+10
		    sinon
		    si n>A alors 
		        		ecrireln("incorrect , trop grand ") 
		        		sinon 
		        		ecrireln ("incorrect , trop petite")	        		 
		        		k<-k+1      
		    finsi	
		    finsi		    
	fintantque
	si k=5 alors
	ecrireln	  (" le nombre est :",A)
	finsi
	ecrireln("au-revoir")
Fin
6.2 
complixite = O(n^2) : complixite quqdrqtique
7 . EXERCICE 7
7.1
Algorithme somme
var
n,i,S:entier
Début
	ecrire("entre un nombre :")
	lire (n)
	S<-0
	pour i <-1 à n pas 1 faire 
		    S <-S + i 
	finpour
 ecrire ("la somme des entier de 1 à ", n, " est ", S)
Fin
7.2 
Algorithme somme_F
fonction somme (n:entier): entier
      debut
                si n =0 alors 
                                    retourne n
                                    sinon 
                                    retourne somme (n -1 )+n
                finsi
      fin
      var 
      n: entier
Début
	ecrire ("       entre un nombre : ")
	lire (n)
	ecrire("la somme des entier est :", somme (n))
Fin
7.3
complixite de algorithme 1 = O(n) : COMPLIXITE LINEAIRE
complixite de algorithme 2 = O(n) : COMPLIXITE LINEAIRE

