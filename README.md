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
3. reponse de question 3
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
