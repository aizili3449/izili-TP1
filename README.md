# TP1  
NOM : IZILI
PRENOM : ABDELJALIL
REPONSE
1. reponse de question 1
Algorithme exercice_1
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
Algorithme exercice_2
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
Algorithme exercice_3
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
   Algorithme exercice_3_F
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
    COMPLEXITE algorithme avec boucle = O(LOG(N))
    COMPLEXITE algorithme avec fonction =O(LOG(N))
   LES DEUX COMPLEXITE SONT EGAUX
4 . exercice 4
   4.1:
Algorithme exercice_4
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
   Algorithme exercice_4_methode_2
var n,i ,R: entier
Début
ecrire("entre un nombre")
lire(n)
R<-sqrt(n)
pour i <- 1 à R pas 1 faire 
    si(R mod i )=0 alors 
            ecrire (i,"   est un deviseur de  ", R )
            ecrireln("    et le père est ", R div i , "  et aussi un diviseur de   ",R)
    finsi
    
finpour
Fin
