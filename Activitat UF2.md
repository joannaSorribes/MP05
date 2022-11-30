# Activitats: 

Per dibuixar els diagrames de flux podeu fer servir [draw.io](https://draw.io) o qualsevol altra eina online.

1. Calcula el CC de les següents figures:
  - ![image](https://user-images.githubusercontent.com/110727546/204613022-4ab64342-2e06-438d-a7e8-570685b3c406.png)
  - ![image](https://user-images.githubusercontent.com/110727546/204613180-6d55bf09-28b8-417e-96f4-f71a762ac44c.png)
  - ![image](https://user-images.githubusercontent.com/110727546/204655229-8c3f28d7-3d8b-4746-a55d-331f89da39d2.png)

  - **Resultat 1:**   16 - 14 + 2 = 4
  - **Resultat 2:**   16 - 14 + 2 = 4
  - **Resultat 3:**    8 - 6  + 2 = 4


2. Dibuixa el diagrama de flux representat per aquest codi i després calcula la seva CC:
  - ![image](https://user-images.githubusercontent.com/110727546/204615125-363e5e6c-173b-4ec0-8c0b-cb97985ade06.png)
  - **Diagrama:** 
![Captura de pantalla de 2022-11-30 09-15-16](https://user-images.githubusercontent.com/113586183/204743032-f3e9c96a-a9ec-488d-9aa2-531ab976ed35.png)
  - **Resultat CC:**  5 - 4 + 2 = 3 



3. Dibuixa el diagrama de flux representat per aquest codi i després calcula la seva CC:

```
public class proves {
    public static  String queEmPoso(int temperatura) {
        String roba = "res";
        if(temperatura<0){
           roba = "roba d'esquiar";
        }
        else if(temperatura<10){
           roba = "roba de muntanya";
        }
        else if(temperatura<20){
           roba = "roba d'hivern";
        }
        else if(temperatura<30){
           roba = "roba d'estiu";
        }
        return roba;
    }    
}
```

  - **Diagrama:**
![imatge](https://user-images.githubusercontent.com/113586183/204762562-9d51bffa-0e63-4d4b-bbf5-e36a49439567.png)
-**Complexitat ciclomàtica = nombre de sentencies condicionals + 1
  - **Resultat CC:** 4 + 1 =5
  - **Resultat proves camins:**  
  - SI T ÉS < 0 (DE -1 A ?)= ROBA ESQUI
  - SI T ÉS < 10 (0 A 9) = ROBA MUNTANYA
  - SI T ÉS < 20 (10 A 19) = ROBA HIVERN
  - SI T ÉS < 30 (20 A 29)= ROBA ESTIU
  - SI ÉS MAJOR DE 30 QUEDA'T A CASA

4. Dibuixa el diagrama de flux representat per aquest codi, calcula la seva CC i crea una prova per a cada camí posible:

```
    public static Boolean llumsEncesos(int hora) {
        Boolean llums = false;
        if(hora <= 8 || hora >= 20){
            llums = true;
        }
        return llums;
    }
```
  - **Diagrama:**![image](https://user-images.githubusercontent.com/113586183/204750401-ac88562a-0caf-4f7c-8475-a489339aee8c.png)

  - **Resultat CC:**  4 + 1 = 5
  - **Resultat proves camins:**
  - SI L'HORA ÉS <= 8 LLUMS ON
  - SI L'HORA ÉS >= 20 LLUMS ON
  - SI L'HORA ÉS > 8 LLUMS OFF
  - SI L'HORA < 20 = LLUMS OFF

5. Investiga sobre les proves de caixa negra:

  **Què són?**
  - Normalment són les proves que fan els usuaris, proves alfa i beta. Els usuaris no saben com funciona internament l'objeste o element. Ex un televisor o un cotxe. L'usuari comprova que un tv sintonitze els canals, puje el volum... una persona que vol comprar un cotxe comprovarà que s'enjagui lo motor, funcionen les llums, etc.
   
  **Quina diferència principal tenen sobre les de caixa blanca?**
  - La principal diferència és que en la caixa blanca es sap i es veu el seu funcionament de manera interna, com ho faria un mecànic o tècnic d'aparells electrónics, i en la caixa negra no se sap com funciona però es porba que funcioni de la manera en que s'espera que ho faci.
