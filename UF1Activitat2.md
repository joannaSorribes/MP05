# 
GO d6

Utilitzant la línia de comandes, sense utilitzar un IDE de desenvolupament escriureu el programa en un fitxer de text que sigui el codi font, el codi font l’adjunteu dins el document.

Primer crearem amb un touch a la carpeta quer vulguem l'arxiu "dado.go"
l'extensio és importantíssima, després entrem a l'arxiu i posem el codi.

```
 package main

 import (
     "fmt"
     "math/rand"
     "sync"<img width="601" alt="image" src="https://user-images.githubusercontent.com/113586183/194762918-3c47f503-e30f-4c30-95c5-8a994a1eee18.png">

     "time"
 )

 var onlyOnce sync.Once

 // preparacio del dado   
 var dado = []int{1, 2, 3, 4, 5, 6}

 func rollDice() int {

     onlyOnce.Do(func() {
         rand.Seed(time.Now().UnixNano()) // ejecutar nomes una vegada
     })

     return dado[rand.Intn(len(dado))]
 }

 func main() {
     dado1 := rollDice()
     

     fmt.Println("La teva cara del Dau es: ", dado1)
     
 }
```
Guardem l’arxiu i obrim la terminal i al fer el build o el run em donava error
![](s_1.png)![s_1](https://user-images.githubusercontent.com/113586183/194256428-689c3691-89fe-4ddb-80dc-aa650a7b08c4.png)



El que he fet ha sigut instal·lar el "golang-go" i ara si l'he pogut executar creant l'executable amb build

![](S_2.png)![S_2](https://user-images.githubusercontent.com/113586183/194257635-c84c1ca8-9303-45c6-8a6c-b26f9621575a.png)



Descriviu com passar de codi font a codi objecte.

Per poder passar de codi font a codi objecte el que farem sera la comanda “go build dado.go”
![](s_3.png)![s_3](https://user-images.githubusercontent.com/113586183/194257767-9ea12bb4-2c7d-4b54-a3ec-d044912c5cd3.png)




***Mostreu les extensions dels fitxers de codi font i codi objecte***

![](s_4.png)![s_4](https://user-images.githubusercontent.com/113586183/194257883-9b0832dc-bf10-4e70-990f-a05773701f7b.png)



***Expliqueu els avantatges d’utilitzar un llenguatge compilat i els punts febles***

Unes de les avantatges serien; La pròpia correcció dels errors en la compilació, ja que ens avisa abans de crear l'executable els erros que hi han. L'execució és molt més ràpida pel fet que no passa d'instrucció a instrucció executa tot el bloc una volta compilat.

Els punts febles serien; No podem corregir errors fins que no acabi de compilar, quan es revisa l'error cal tornar a compilar i la dificultat d'aprenentatge.





***Busqueu 3 IDEs de desenvolupament pel llenguatge***
Els IDEs serien:

Visual studio code
https://code.visualstudio.com/
![](ide's.png)<img width="601" alt="ide's" src="https://user-images.githubusercontent.com/113586183/194762860-6c017ec7-e776-4957-86e3-3ad6750d407e.png">



Netbeans
https://netbeans.apache.org/
![](netbeans.png)<img width="599" alt="netbeans" src="https://user-images.githubusercontent.com/113586183/194762982-6ef63740-26aa-4d9e-8d83-88e67af8cd70.png">




Aquest és online

go.dev
https://go.dev/play/
![](go_dev.png)<img width="602" alt="go_dev" src="https://user-images.githubusercontent.com/113586183/194762984-92ffe426-d4ce-4885-8a3b-6256c147f129.png">





# PYTHON d6

```
import random
 
numero1 = random.randint(0,10)

print ('El numero que has obtingut és ',numero1 

```


Obrim un document nou on escrivim el codi font amb la funció per realitzar el programa del dau.

Guardem el document amb extensió del llenguatge codi font que untilitzem, en aquest cas és llenguatge Python.El document serà d6_Python.py.

![](1.png)![1](https://user-images.githubusercontent.com/113586183/194021408-1c5cedc6-8a70-43a8-98d8-7f4b583683ef.png)


Obrim el terminal de la carpeta on està el document amb el codi que volem executar.

Al intentar executar l'arxiu ens dóna error i demana que instal·lem el Python.

Instal·lem l'extensió python

Un cop tenim l'extensió de Python instal·lada introduim el següent comandament : ``` python3 d6_Python.py``` i obtenim el resultat del programa.

![](2.png)![2](https://user-images.githubusercontent.com/113586183/194021919-46bbc921-4ded-47da-a0bb-9fe0cdb62d90.png)



***Descriviu com passar de codi font a codi objecte***

Per passar de codi font a codi objecte introduïm la comanda: ```pyhton3d6_Python.py```

***Mostreu les extensions dels fitxers de codi font i codi objecte***

**Ventatges i desventatges llenguatge interpretat

**Pros**

-És independent de la màquina i del sistema operatiuc, es poden executar en qualsevol plataforma.
-Es pot modificar el codi mentre s'executa.
-Ocupen menys lloc en la memòria
-L'entorn de treball s'encarrega de que el hardware executi les instruccions.
-Molt emprat en desenvolupament web i en electrònica.


**Inconvenients**
-La alta portabilidad afecta a la velocita al executar el codi.
-Difícils de depurar.
-Requereix d'un software per interpretar les instruccions del procesador.
-No todos los software es troben disponibles en totes les plataformes.

# JAVA d6

Utilitzant la línia de comandes, sense utilitzar un IDE de desenvolupament
escriureu el programa en un fitxer de text que sigui el codi font, el codi font
l’adjunteu dins el document.


```
import java.util.ArrayList;
import java.util.List;
import java.util.Random;
import java.util.Scanner;

public class DauSisCares {

    public static void main(String arg[]) {

 List<Integer> numbers = new ArrayList<>(6);
        for (int i = 1; i < 7; i++) {
            numbers.add(i);
        }

// Instanciamos la clase Random
        Random random = new Random();

// Mientras queden cartas en el mazo (en la lista de numbers)
        while (numbers.size() > 1) {
            // Elegimos un índice al azar, entre 0 y el número de cartas que quedan por sacar
            int randomIndex = random.nextInt(numbers.size());

            // Damos la carta al jugador (sacamos el número por pantalla)
            System.out.println("Els resultat de la teva tirada, és " + numbers.get(randomIndex));

            // Y eliminamos la carta del mazo (la borramos de la lista)
            numbers.remove(randomIndex);
        }
    }
}


```
2. **Descriviu com passar de codi font a codi objecte.**

Per executar un programa Java, primer hem de compilar el programa. Llavor necessitem el openjdk-18 (Java Development Kit) per compilar i executar programes Java.

El primer que farem serà instal·lar el openjdk-18 ja que estem programant en la versió 18 sudo apt install openjdk-18-jre-headless
![](java_1.png)<img width="546" alt="java_1" src="https://user-images.githubusercontent.com/113586183/194763271-7f2ac4e8-b264-40b7-a607-fc8e4d8ef703.png">


Molt bé, ara passem al IntelIj i creem l'arxiu amb extensió .jar d'aquesta manera només tenim el Java Development Kit podrem executar el .jar en qualsevol sistema operatiu SO

Anem a file Project Structure
![](java_2.png)<img width="398" alt="java_2" src="https://user-images.githubusercontent.com/113586183/194763311-8059846a-736f-4eee-aafa-79aad7df13e4.png">


Artifacts  i seleccionem el nom del nostre projecte i li donem al ok
![](java_3.png)<img width="542" alt="java_3" src="https://user-images.githubusercontent.com/113586183/194763338-d6b3e730-12ea-4037-a3f6-d89c43af409d.png">

I carregem el projecte al transformador JAR


![](java_4.png)<img width="541" alt="java_4" src="https://user-images.githubusercontent.com/113586183/194763379-81c8fd36-eac5-4ac7-a9ef-6e02ab9c3357.png">![]

Una volta sap on està la ruta de l'arxiu anem a la pestanya Build i Build Artifacs
![](java_5.png)<img width="544" alt="java_5" src="https://user-images.githubusercontent.com/113586183/194763457-2b5bb5f3-46ba-4453-9bad-c1af11e42d96.png">

I seleccionem en Action Build

![](java_6.png)<img width="412" alt="java_6" src="https://user-images.githubusercontent.com/113586183/194763485-e9c17008-f521-4360-9869-41abf4771905.png">


 I ja tenim el nostre programa preparat per a ser executat amb qualsevol SO
![](java_7.png)<img width="285" alt="java_7" src="https://user-images.githubusercontent.com/113586183/194763515-f10488b7-34d2-418e-9a49-1c5bc6def726.png">
 
Finalment executem el programa amb la comanda java -jar PrimerProjecte.jar
![](java_8.png)<img width="538" alt="java_8" src="https://user-images.githubusercontent.com/113586183/194763619-94c86f69-e2fd-41b2-acbe-2dc62698242c.png">




**Mostreu les extensions dels fitxers de codi font i codi objecte**
![](extensions.png)<img width="278" alt="extensions" src="https://user-images.githubusercontent.com/113586183/194763673-f7120502-dce4-45b8-b068-ea8b4a224874.png">

**Expliqueu els avantatges d’utilitzar un llenguatge màquina virtual i els punts febles**

Els avantatges serien la portabilitat entre diferents SO mantenint tot el codi igual que l'encapsulat, ja que tot allò necessari per al seu funcionament dins d'un entorn que és independent, tant del sistema operatiu des de la qual és creada, com amb altres màquines virtuals diferents del mateix servidor, com també un alt nivell de seguretat perquè una màquina virtual s'aïlla del mateix sistema operatiu en què està instal·lada, evitant qualsevol problema de seguretat, com pot ser malware. Evitant afecta el servidor, equip o altres màquines virtuals.

Però no tot són avantatges, també té inconvenients com per exemple la disminució del rendiment, ja que el rendiment serà inferior al del mateix equip o servidor físic on s'instal·la, Complexitat d'ús perquè on hi ha connexions amb xarxes diferents i s'utilitza una gran varietat de maquinari, pot arribar a ser tediós configurar una màquina. Al ser un llenguatge interpretat pot ser una mica més lent en l'execució dels programes.

**Busqueu 3 IDEs de desenvolupament pel llenguatge**

Els IDEs serien:

IntelIj
https://code.visualstudio.com/

![](ide's_2.png)<img width="591" alt="ide's_2" src="https://user-images.githubusercontent.com/113586183/194763789-11001c14-f847-43f6-b22c-d848952e1e84.png">
Netbeans
https://netbeans.apache.org/

![alt text](fotos/Selecció_078.png)

Aquest és online

Eclipse

https://www.eclipse.org/ide/
![](eclipse.png)<img width="600" alt="eclipse" src="https://user-images.githubusercontent.com/113586183/194763865-4911ab26-7f93-4062-94d1-86d3883c2145.png">










