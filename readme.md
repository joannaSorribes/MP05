# LLenguatges de Programació
//**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ 

#OBJECTIVE C

El llenguatge de programació **Objective-C** es va crear al 1980 de la mà de **Brad Cox** i la corporació StepStone.

Es tracta d’un llenguatge orientat als objectes i que es basa en el llenguatge C estandar.
Permet generar objectes que tenen una similitud amb **SmallTalk**.
L’any *1988* va ser afiliada al llenguatge de programació Nextstep i en 1992 va ser alliberar mitjançant la llicència GPL para els software de compilació GCC.
Actualment **Objective-C** és el principal llenguatge utilitzat per al desenvolupament d app en **iOS**. 
És un llenguatge més antic que java(95), python(91), php (95) etc i és nota en algunes de les seves característiques que després veurem.
Apple té la intenció de substituir **Objective-C** per **Swift** en un futur pròxim.

**Característiques:**
### Avantatges

1. És un llenguatge d’alt nivell compilat compatible amb molts softwares i contextos de programació.
2. Les sentències de control de flux com while, for, do, while estan immersos.
3. Orientat a objectes que poden rebre i enviar missatges
4. És dinàmic i comparat amb altres com java dona més llibertat
5. Àmbits variables, tals com globals, estàtiques i locals.
6. Conversions explicites i implicites entre dos tipus.
7. Les classes es guarden en dos fitxers .h i .m.
8. Com a llenguatge antic no té recolector de basura però a implementat ARC un recurs per eliminar objectes i no tampoc es poden usar excepcions.
9. Tots els seus mètodes són públics
10. Permet enviar missatges a Nill(null) per el qual si es crida un mètode d’una variable no inicialitzada no es veuran els errors, arrancarà però no farà res. ( aixó pot ser un avantatge o desventatge, segons com es mire).

### Inconvenients

1. No fa comprovacions en la compilació, es fan al temps d’execució. Els errors no es detecten fins al final però té recursos per limitar aquests inconvenients.
2. Maneig del punter un poc complicat.
3. És un programa vell i és més susceptible als problemes de seguretat.
4. Té una sintaxi enrevessada que pot resultar difícil per a no iniciats.
5. Cada cop és menys utilitzat i Apple vol substituir-lo definitivament per Swift.
6. No està tant actualitzat com els més nous i fàcils d’utilitzar.
7. Funcionalitats limitades.

### Exemple Codi

`#import <Foundation/Foundation.h>
int main (int argc, const char * argv[])

{
NSAutoreleasePool *pool = [[NSAutoreleasePool alloc] init];
 NSLog (@"Hello, World!");
   [pool drain];
        return 0;
}`

*2022-09-28 14:53:52.048 a.out[2101:2101] Hello, World!*

`#import <Foundation/Foundation.h>
int main (int argc, const char * argv[])
{NSLog (@"Indica el teu usuari");
 char user=0;
 scanf("%s, &user");
 printf("user=", user);
 
        return 0;
}`

d <NSThread: 0x5654b54be190>{name = (null), num = 1279}
2022-09-28 15:56:40.899 a.out[1279:1279] Indica el teu usuari
Joanna
user=

...Program finished with exit code 0
Press ENTER to exit console.


//**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ 

#PYTHON

Llenguatge de programació interpretat creat per **Guido Van Rossum** a principis dels anys **90’**( al 91 es publica la 1r versió). Deu el seu nom a l’afició que tenia el seu creador al grup humorista britànic dels Monty Python. Originalment desenvolupat per sistema operatiu AMOEBA, que es basava en una arquitectura de micronúclis. 

**Característiques:**
### Avantatges

1. És un llenguatge interpretat simple i fàcil per a la iniciació en programació.
2. Portable. Permet la seva utilització en diverses plataformes al ser de naturaleza Open Source.(Linux, MacOs, Unix i WIndows)
3. Llenguatge d'alt nivell orientat a objectes.
4. Permet la seva implementació dins d’un programa **C/C++**.
5. Disposa de extenses llibreries i frameworks.
6. Sintaxis clara i de fàcil enteniment.
7. “Tipado” dinàmic pel qual no és necessari indicar el tipus de dades. S'adapta al contingut que se li escriu (tot i que pot suposar inconvenients d’optimització de memoria o errors al escriure entre d’altres)
8. Disposa de suport i informació per múltiple varietats de base de dades i compta amb una gran comunitat.
9. Molt emprat per al **Big Data**, amb mòduls com **NumPy**, **Pandas** o **Matplotlib**…
10. Compatible amb una amplia gama de **GUI** ( interfície gràfica d'usuari) que es poden importar fàcilment i que facilita la visualització de les dades.

### Inconvenients
1. Degut a la seva gran versatilitat i a que no té un ús específic i compilat pot arribar a tenir un processament lent. Python ofereix algunes opcions per tal de solucionar  aquest inconvenient però pot arribar a ser una tasca molesta.
2. En algunes aplicacions i camps no és l'opció més adient, com ara app mòbils. Hi han llenguatges més especialitzats per aquestos camps.
3. Al ser un llenguatge que opera amb moltes dades pot tenir un consum de la memòria molt elevat. No és el més adient per projectes molt grans.
4. El seu dinamisme pot arribar a sorgir errors durant l'execució.
5. La majoria dels servidors amb servei de hosting no tenen soport per Python.

### Entorns on s'utilitza

1. Videojocs. Permet la creació i manipulació de gràfics i entorns 3D interactius.
2. Analitzar Big Data. Permet analitzar gran quantitats de dades en temps real i disposa de tot tipus de biblioteques de processament.
3. IA. Llenguatge molt conegut per la programació i desenvolupament de intel·ligència artificial de gran eficàcia.
4. Data Science. Utilitzat per molts científics per estudiar les grans quantitats de dades que d'un altra manera no seria possible. Es beneficien del seu us en el BigData.
5. Desenvolupament Web. Moltes aplicacions i llocs webs utilitzen aquest llenguatge ja que és un sistema estable i eficient.
6. Machine Learning. Com a llenguatge molt utilitzat per desenvolupar IA també els pot facilitar la capacitat d’aprendre mitjançant l’experiència i realitzar noves tasques amb el temps.

### Exemple Codi
`print('Hola, món!')`

Hola, món!

** Process exited - Return Code: 0 **
Press Enter to exit terminal


`nombre = input("Indica el teu nom d'usuari ")
print(nombre)`

Indica el teu nom d'usuari 
Joanna
Joanna

** Process exited - Return Code: 0 **
Press Enter to exit terminal


//**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ 

#JAVA

La companyuia de Sun Microsystems va crear de la mà del Green Team (James Gosling) aquest llenguatge per a dispositius digitals de consum. En un principi es va anomenar **OAK** que vol dir *Roble* en inglès perquè hi havia un a fora de la seva oficina.
Van fer una demostració de com funcionava el llenguatge mitjançant una televisió interactiva però era massa avançat per la televisió interactiva digital per cable d'aquell moment.

El lleguatge va passar a dir-se **GREEN* i finalment es va dir **JAVA** en referència al cafè del mateix nom i d'aquí també la icona de la tassa.
Degut a la popularitat de **C/C++**, James Gosling va dissenyar aquest llenguatge emprant un estil de sintaxi de **C/C++** i la seua filosofia "*escriu un cop, executa en qualsevol lloc*".


Creat i comercialitzat per **Sun Microsystems**en *1995*.
Oracle Corp va adquirir Sun Microsystems juntament amb Java al *2010*.
Con el compilador se convierte el código fuente que reside en archivos cuya extensión es .java, a un conjunto de instrucciones que recibe el nombre de bytecodes que se guardan en un archivo cuya extensión es .class. E

**Característiques:**
### Avantatges

1.És un llenguatge híbrid d’alt nivell que deriva del **C** i del **C++** però més simple potent.
2.Llenguatge orientat a objectes i que s’executen en qualsevol dispositiu.
3.Disposa d’una gran biblioteca estàndard i d'eines per a poder distribuir els programes.
4.Portable. Pot executarse en qualsevol tipus de plataforma/hardware.
5.Recolector de brossa. Quan no hi han referències localitzades a un objecte, el recolecto borra aquest objecte alliberant espai a la memoria ocupada.
6.Segur i sòlid per desenvolupar i executar aplicacions, administra automàticament la memòria, ofereix canals de comunicació segura per protegir la privacitat de les dades.
7.Sintaxi rigurosa que permet evitar que es trenque el codi i que es corrompi.
8.Multifil. Permet dur a terme diverses tasques simultàniament dins del mateix programa que permet millorar el rendiment i la velocitat d’execució.
9.Adaptabilitat a diferents tipus de dispositius (tablets, telèfons intel·ligents, portàtils, ordinadors…)
10.Avui en dia**JAVA** és un dels llenguatges de programació més usats a tot el món. Moltes aplicacions i llocs web no funcionaran o tindra elements que no s’executaran si no tenen **JAVA** instal·lat.

### Inconvenients

1. Al ser un llenguatge que també interpreta el rendiment a l'hora d'executar els programes pot disminuir, ja que es poden presentar variables no desitjades en donar una ordre inicial.
2. Per a iniciar-se en la programació no és el llenguatge mé recomanable, ja que la pogromació orientada a objectes és una evolució de altres composicions informatiques.
3. La sintaxi que utilitza és un poc complicada i te una evolució algo més lenta que altres llenguatges com **Python**.
4. Necessita de la màquina virtual de Java per accedir alguns contingut i pot supossar incompatibilitats amb alguns dispositius. Necessita d'aquesta maquina per executar els programes escrits.
5. Es necessiten dispositius i equips que soportin la potència dels programes que s'executen amb la tecnologia provocant la lentitud en les aplicacions

6. Opcions 3D limitades.
7. No compta amb una funció de copia de seguretat.

Java trabaja principalmente en el almacenamiento y no se enfoca en la copia de seguridad de los datos. Esta es una de las desventajas del lenguaje de programación Java que hace que se pierda el interés y las valoraciones entre los usuarios.


## Entorns on més s'utilitza JAVA

1. Video Jocs. Java pot ser una gran opció per al desenvolupament de videojocs. Disposa de un gran número de frameworks i llibreries disponibles com **OpenGL**.
2. Big Data. La majoria de programadors escollixen Java a l'hora de treballar en Big Data. Una de les raons d'aquesta preferència és que una de les eïnes més famoses del Big data utilitza Java. A més, té una gran comunitat per donar soport i ajuda en Big Data.
3. Construir aplicacions webs. Disposa d'alguns dels més populars frameworks com **Spring**, **Hibernate**, entre d'altres, per construir aplicacions web.
4. Contruir interficies gràfiques per aplicacions d'escritori.
5. Aplicacions d'Android. Idioma oficial per desenvolupar en Androir.

## Exemple Codi
`public class HolaMon {
    public static void main(String[] args) {
        System.out.println("Hola, món!");
    }
}` 

Hola, món!

Process finished with exit code 0


`import java.util.Scanner;
public class UserName {
    public static void main (String args[]){
         Scanner sc = new Scanner(System.in);
        // demanar introduir una tecla 
        String user;
        System.out.println("Indica el teu nom d'usuari:");
        
       
        user = sc.nextLine();
        System.out.println(user);

    }

}`
jousomi27@iMac-de-Joanna Mp5 %  /usr/bin/env /Library/Java/JavaVirtualMachines/jdk-17.jdk/Contents/Home/bin/java -agentlib:jdwp=transport=dt_socket,server=
n,suspend=y,address=localhost:51241 -XX:+ShowCodeDetailsInExceptionMessages -cp /Users/jousomi27/Desktop/Mp5/bin App 
Indica el teu nom d'usuari:
Joanna
Joanna
jousomi27@iMac-de-Joanna Mp5 % 




//**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ //**\\ 

#SWIFT

Es un llenguatge de programació especialitzat para el desenvolupament d'aplicacions en **OS (iOS,tvOS, OS X i watch OS)**.
Va ser creat per **Chris Lattner, Doug Gregor, John McCall, Ted Kremenek i Joe Groff juntament amb Apple Inc** al *2014*. Va substituir el llenguatge de programació **iOS SALLETTE**i en breu es preveu que reemplace completament **Objective C**.
  Al *2015* va passar a ser de *codi obert* amb Llicència Apache 2.0.
  
**Característiques:**
### Avantatges
 
1.Llenguatge de programació compilat d’alt nivell molt potent.
2.Eina intuitiva i amigable amb el programador, fàcil de llegir i escriure. Molt recomendable per iniciar-se a la programació.
3.Llenguatge orientat a objectes.
4.Proporciona seguretat al programador gràcies al sistema per detectar errors fàcilment permeten corregir els errors de l’app abans que surti al mercat.
5.Destinat a substituir els llenguatges C **(C, C++ i Objective C)** pel que fa a apps**Apple**.
6.Sintaxis fàcil d’utilitzar i de característiques que la majoria de desenvolupadors esperen.
7.Compta amb una gran comunitat activa que ofereix suport, ajuda i nous recursos per poder aprendre i dominar aquest llenguatge.
8.Multiparadigma. Pot treballar amb diferents estils de programació, permeten decidir al profesional com treballar amb ell d’acord amb el tipus de projecte 9.que es vagi a desenvolupar i la plataforma a la qual es vulgui enfocar.
10.Múltiples valors de retorn.
11.Iteració concisa i ràpida.
12.Admet extensions, mètodes i protocols en les seues estructures.

### Inconvenients

1.	AL ser un programa relativament jove que no gaudeix de una gran confiança entre les empreses.
2.	No disposa de una gran comunitat com poden fer-ho Java o Python.
3.	La formació en aquest llenguatge segueix sent difícil i de forma autodidacta.
4.	Hi ha pocs programadors  amb experiència en aquest llenguatge, pocs en tenen un bon domini. Aquest inconvenient pot ser un avantatge a l’hora de trobar feina.
5.	Les empreses tenen dificultats per trobar empleats especialitzats.


## Entorns on més s'utilitza SWFT

Com hem explicat anteriorment és un llenguatge de programació que s’utilitza per al desenvolupament Apps de entorn iOS i macOS.



webgrafia 
https://javadesdecero.es/fundamentos/breve-historia-caracteristicas-y-aplicaciones/
http://www.sc.ehu.es/sbweb/fisica/cursoJava/fundamentos/introduccion/virtual.htm
https://www.crehana.com/blog/desarrollo-web/ventajas-desventajas-java/
https://lenguajedeprogramacionblog.wordpress.com/c/
https://lenguajesdeprogramacion.net/python/
https://www.startechup.com/es/blog/objective-c-vs-swift-which-programming-language-is-better-for-your-ios-application-development/
https://www.tokioschool.com/noticias/lenguaje-programacion-swift/


