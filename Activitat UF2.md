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
  -![image](https://user-images.githubusercontent.com/113586183/204746399-5012c044-0310-42cd-a80e-d6885346cc33.png)

  - **Resultat CC:**

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
  - **Diagrama:**
  - **Resultat CC:**
  - **Resultat proves camins:**

5. Investiga sobre les proves de caixa negra:

  - Què són?
  - Quina diferència principal tenen sobre les de caixa blanca?
