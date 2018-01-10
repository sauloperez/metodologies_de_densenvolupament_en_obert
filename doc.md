# Metodologies de desenvolupament en obert

## Client/Servidor

És un model d'aplicacions distribuides que particiona una tasca entre dues parts
en el que la comunicació entre ambdos parts succeix a través de la xarxa.

Aquest model és la base fonamental de moltes tecnologies que fem servir durant
el nostre dia a dia.

Funciona de la manera següent:

  * El servidor arrenca un procés de vida indefinida escoltant peticions en un port de xarxa determinat.
  * El client envia una petició a aquest mateix port i espera una resposta.
  * El servidor processa la petició i retorna una resposta al client.

## Frontend

En el cas d'aplicacions web el client rep habitualment el nom de frontend perquè
és a la banda del client on s'executa la part visual amb la que interactua
l'usuari.

El codi frontend s'executa al navegador i és el que implementa el
comportament de la pàgina així com els botons, diàlegs, camps de text,
animacions, etc. aquest conjunt d'elements d'interacció conformen el que
s'anomena interfícia d'usuari. És senzillament el mitjà es produeix la
comunicació entre usuari i màquina.

## Backend

Backend per contra és el nom que rep el servidor en el context d'aplicacions
web. Rep aquest nom pel fet que executa la part que no és visual, com en el cas
del frontend.

El codi backend s'executa a màquines dedicades exclusivament per aquesta
finalitat, molt sovint contractades a tercers, i és el que implementa la lògica
de negoci. Tot i que aquest fet no és exclusiu del backend en segons quines
arquitectures d'aplicació, sí que és el cas de la web clàssica.

Una altra responsabilitat del backend és executar la base de dades.

## Base de dades

Les dades són la peça fonamental de qualsevol aplicació web. Sense les dades no
hi pot haver aplicació. En la gran majoria dels casos l'app haurà de persistir
dades. És per això que tant la gestió eficaç de les dades com un disseny adeqüat
de la seva estructura són crítics pel bon funcionament de l'aplicació.

Les aplicacions web clàssiques fan servir bases de dades relacionals. Un tipus
de bases de dades que fa servir el llenguatge estàndard SQL per mantenir la base de dades
i obtenir-ne informació. Així doncs, SQL permet comunicar l'usuari amb la base de dades a través de
quatre tipus d'operacions: SELECT, INSERT, UPDATE, DELETE.

Les bases de dades en general es basen també en el model client/servidor. El
sistema gestor de la base de dades s'executa de manera indefinida al servidor
esperant peticions en un port especificat. L'usuari utilitza un client
compatible amb aquest sistema gestor de base de dades per enviar-hi peticions
usant les operacions anteriorment esmentades. És llavors quan el sistema gestor
respon a la petició del client amb el resultat de l'operació, i aquest per la
seva banda les mostra visualment a l'usuari en forma de taula.

## App Nativa

En el context de les aplicacions mòbils 
Concepte natiu fa referència a tecnologia del fabricant: Android, iPhone, etc.

Tecnologies multiplataforma fan ús de tecnologies web d'ampli ús i que no
depenen dels fabricants

## API

Application Programming Interface. Comparar amb interfície d'usuari. Implementa
la mateixa lògica de negoci.

Dades per a que les processi el frontend-client. Elements d'una llista.

Ensenyar exemple a https://jsonplaceholder.typicode.com/posts

## Com es fa tot això?

Preguntar a l'audiència

## No reinventis la roda

Quelcom ja inventat, que no té errors coneguts de funcionament, i un intent de
reinvent-ho no tindria sentit no hi afegiria valor. Malgastar el temps mentre et
podries centrar en coses que aportin més valor.

Moltes vegades no és conscient.

## Reusant codi

Metàfora que ens porta a les nostres cebes. Per això incideix-ho tant en les
cebes perquè vull que reuseu.

A quina capa de la ceba desenvolupem.

Llibreria: implementa funcionalitats espcífiques. Nivell de granularitat
variable. Lligat a un domini o una utilitat. Exemple de llibreries de xarxa.
Ensenyar Gemfile.

Framework: conjunt de llibreries per construir quelcom. Molts components. No
lligat a un domini.  Implementa algun disseny de sofware. Has d'inserir el teu
codi, lligat a un domini, per veure'l funcionar. Parlar de Rails.

## Git

Per poder reusar codi i fer codi de manera col·laborativa cal emmagatzemar-lo
fora del nostre ordinador i fer-lo accessible.

Gestió de canvis en arxius i directoris en el temps.

Commit: foto
Branca: Línia de temps indepent de la central. Conjunt de commits. Sempre hi ha
una principal.
Repositori: Estructura de les metadades del projecte usades per git. `.git/`

## Github

Social coding: Vell moto de github. Fer codi amb altres té una gran dimensió
social que s'amplia en el cas de l'open source. Com més open source faig, més
descobreixo aquest dimensió.

## Anatomia

Pull Request. Demanar ajuntar la branca que t'havies fet per
implementar/arreglar un error.

Merge: ajuntar aquestes dues branques.

## Metodologies àgils

Como ya se ha introducido en modulos anteriores, platform cooperativism se
refiere a proyectos que tienen un fuerte enlace con las comunidades en las que
se generan. A la hora de disenyar un proyecto tecnologico se recomienda implicar
todos los actores afectados: usuarias, personas con perfiles tecnicos y toda la
comunidad. Los procesos de co-disenyo suelen utilizar las metodologias agiles
para incluir las necesidades de una comunidad en los procesos de desarrollo
y traducirlos en iteraciones compuestas de tareas concretas y formulas para
medir los resultados. En cada iteracion se implementa un pequenyo grupo de
cambios, que aporte valor a la comunidad y que sea facil de evaluar. La fase de
evaluacion de cada iteracion alimenta las siguientes iteraciones para incorporar
las correcciones y adaptaciones que hayan emergido. De esta forma es mas facil
integrar la comunidad en el co-disenyo ya solo hay que evaluar pequenyos cambios
y compararlos con la vision global del proyecto. Abordar grandes cambios
intentando aportar cuanto mas valor posible en una unica iteracion muy larga
puede en cambio resultar muy dificil de llevar a cabo y de evaluar por un grupo
de personas numeroso.

## Àgil i obert

Les metodologies àgils ja aporten un enorme valor per si soles, motiu pel qual
han tingut un gran èxit en el món tecnològic empresarial no limitat a les
petites i mitjanes empreses.

La combinació entre aquestes metodologies i el desenvolupament en obert aporten
un potencial molt més gran en el món del cooperativisme de plataforma.

Dividir el desenvolupament del producte en tasques d'abast molt reduït
i definit, com part d'iteracions englobades en el full de ruta de la plataforma
permet tant desenvolupar el producte entre varies persones fins i tot en les
mateixes àres del software, com un desenvolupament veloç amb molts canvis
incrementals i freqüents.

Les tasques petites tenen a més el benefici afegit de no requerir un esforç
cognitiu excessiu per a cap de les parts implicades. El desenvolupador entén
perfectament quins són els requeriments de la tasca i compleix amb les
expectatives sense haver de preguntar a la persona que ha creat la tasca. Per
altra banda, la persona que s'encarrega de provar la implementació entén
ràpidament quines són les parts afectades i quines funcionalitats s'han de
provar.

No menys important és l'impacte positiu que té a l'estat d'ànim dels membres de
l'equip de desenvolupament i la comunitat en general veure com el producte
evoluciona positivament i s'avança en els objectius marcats, i com el treball en
equip és efectiu i àgil.

Per últim, tasques d'abast reduït i ben definit són imprescindibles per tal
d'obrir la porta a contribucions per part de membres de la comunitat com també
de contribucions esporàdiques per part de gent fora de la comunitat.

Un cop fot el triatge de tasques fàcils per nous contribuïdors cal encoratjar
a la gent a fer el pas de participar del desenvolupament, no només en codi.
Participar de manera activa requereix reconèixer les pròpies mancances,
deslligar-se de les pròpies vergonyes i centrar-se en les potencialitats que es
poden aportar al projecte.

Quan això va seguit d'un acompanyament augmenten molt les probabilitats que de
ser un contribuidor esporàdic es passi a ser un membre més de la comunitat. Cal
tenir en compte però, l'esforç i dedicació que tot això requereix dels membres
més actius i de l'equip de desenvolupament.

## Operacions i administració de sistemes

Un dels aspectes menys evidents en tot el procés de producció de software està
relacionat amb "posar a producció" el mateix sofwate. És a dir, posar-lo
a disposició dels usuaris. En funció de l'arquitectura de xarxa i de l'aplicació
que s'hagi escollit hi ha diverses maneres de portar a terme aquest procés.

En el de client/servidor, l'equip responsable d'entregar el producte als seus
usuaris necessita traslldar el software a servidors accessibles des de internet.
Els processos necessaris per fer-ho estan estrament relacionats amb el conjunt
de tecnologies escollides per donar suport al software produït.

Tot i aquesta espcificitat, hi ha una sèria de patrons recurrents en aquests
processos. És important però, adoptar unes pràctiques que permetin a tot l'equip
conèixer aquests processos de manera que no depenguin de persones concretes.

Els processos bàsics necessaris per posar un software a producció es poden
resumir en:

  * Gestió de servidors
  * Provisionament
  * Desplegament
  * Monitorització

### Gestió de servidors

L'elecció dels servidors en els que s'executarà el software requereix
coneixement del mercat i dels factors relacionats amb el posicionament geogràfic
dels usuaris del software. Entre tants proveïdors de serveis d'allotjament es
necessari entendre també el nivell de confiança que podem esperar segons el
model de governança, la mida de l'empresa, etc.

### Provisioning

Una vez conseguido acceso a los servidores, necesitamos preparar las maquinas
para que puedan recibir y ejecutar nuestro software. El proceso de provisioning
se encarga basicamente de instalar en los servidores todo aquel software que no
hemos desarrollado nosotros directamente pero del que necesitamos para ejecutar
el nuestro. Un ejemplo puede ser el software que gestiona las bases de datos,
etc. Este software se suele llamar "dependencias".

### Desplegament

A partir del momento en que los servidores esten equipados con todas las
dependencias necesarias podemos empezar el proceso de traslado del software
producido por nuestro equipo. Este proceso es responsable de fisicamente poner
en produccion el software y tambien esta muy vinculado a las tecnologias
elegidas. Un aspecto importante de este proceso es que tiene que facilitar el
acceso a la version del software que ha sido desplegada y a procesos de
emergencia para volver a activar versiones anteriores.

### Monitorització

Deberia ser ya bastante evidente que todo el conjunto de software y procesos
necesarios para mantener accessible nuestro software puede resultar dificil de
mantener y sobretodo dificil de gestionar en casos de emergencias. Para
balancear esta amenaza se suelen poner en marcha unos mecanismos y procesos de
monitorizacion. Basicamente se trata de instrumentar y monitorar cuantos mas
aspectos posible, a partir del correcto funcionamiento del servidor (memoria,
CPU, etc) hasta cada pieza de nuestro puzzle de software que resulta ser vital
para nuestro proyecto. Colectando toda esta cantidad de datos se puede poner en
marcha un sistema de alertas que avisaria al equipo cada vez algunos valores
medidos se alejan de los valores esperados. Estos datos e informaciones tambien
son importantes a la hora de analizar un problema ocurrido y para actuar para
que no se vuelva a repetir.

## Processos compartits

Acabamos de entender lo complejo y a la vez crucial que son los procesos de
"puesta en produccion" de un software, un fallo en ese conjunto puede poner en
riesgo todo el trabajo invertido en el desarrollo de nuestro proyecto. Para esta
razon se recomienda adoptar buenas practicas y compartir el conocimiento entre
proyectos que usan tecnologias parecidas.

### Documentar-ho tot

Centralizar el conocimiento y el know-how puede poner en peligro un proyecto
tecnologico de este tipo. Hay que contrastar cualquier tipo de resistencia al
compartir la informacion aunque pueda resultar en una perdida de poder para
algunas personas. Es importante documentar cada decision y cada cambio en cada
uno de los procesos mencionados. Si por alguna razon hay partes de esos procesos
que se implementaron sin generar documentacion hay que aprovechar la ocasion
para pedir a una persona que nunca ha tenido acceso a esos proces de
documentarlos. La mejor persona para documentar un proceso es la que nunca los
haya puesto en marcha, es una buena ocasion para transferir conocimiento y a la
vez generar documentacion clara y entendible.

### Reusar processos entre projectes

En los casos en los cuales esta cultura de compartir conocimiento todavia no
haya sido "embraced" por todo el equipo, nos podemos encontrar con procesos que
solucionan problemas parecidos pero de forma distinta. Generalmente es debido
a personas que desconocian o ignoraban la existencia de procesos parecidos y la
falta de comunicacion. Es importante reutilizar los procesos entre los proyectos
y encontrar la forma de implicar todas las personas interesadas cuando se
trabaja en la implementacion de nuevos procesos.

### Fàcil replicació

Desde una perspectiva del pro-comun digital todo este trabajo y esfuerzo
dedicado a documentar y compartir los procesos de produccion es necesario que se
haga visible tambien fuera de la propria organizacion publicando todo lo que se
pueda con licencias abiertas (Creative Commons, etc). De esta forma se podra'
potenciar el efecto de replicacion de los proyectos ya que, como hemos visto, no
solo el software en si es importante y estrategico sino que tambien todo el
conjunto de procesos para la puesta en produccion y el mantenimiento del
proyecto lo es.

Ejemplo Loomio https://github.com/loomio/loomio-coop-handbook
