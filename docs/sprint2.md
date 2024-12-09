# Sprint 2

## Gestió de processos

## Gestió d’usuaris i grups

### Fitxers de configuració

Aquest fitxers són importants a tindrels en compte ja que les seues funcions son essencials.

**/etc/passwd**

El fitxer **/etc/passwd** conté informació bàsica sobre els usuaris del sistema, com els noms dels usuaris, identificadors i altres opcions que fan que el sistema funcioni perfectament.
![Comanda](./imatges/imagen.png)
Aquí podem veure els usuaris i les seves informacions basiques.
![Comanda](./imatges/imatge2.png)

Si volem modificar el fitxer utilitzem aquesta comanda:
![Comanda](./imatges/imatge3.png)
Llavors ens apereixeria aquest fitxer:
![Comanda](./imatges/imatge4.png)

**/etc/group**

Es un fitxer de comfiguració essencial que defineix els grups i la seva relació amb els usuaris.S’utilitza per controlar els permisos dels usuaris i l’accés als recursos.Aquí es podria visualitzar els diferents grups amb el seu GID particular.
![Comanda](./imatges/imatge5.png)
![Comanda](./imatges/imatge6.png)
Per modificar aquest fitxer utilitzem aquesta comanda.
![Comanda](./imatges/imatge7.png)
![Comanda](./imatges/imatge8.png)

**/etc/shadow**

Aquest fitxer conté informació encriptada de les contrasenyes dels usuaris i configuracions de seguretat. nomes es pot accedir pel usuari root ja que es protegeixen les contrasenyes. 
![Comanda](./imatges/imatge9.png)
![Comanda](./imatges/imatge10.png)
Per modificar el fitxer s'utilitza aquesta comanda.
![Comanda](./imatges/imatge11.png)
![Comanda](./imatges/imatge12.png)

**/etc/gshadow**

Aquest fitxer és similar al anterior però en aquest cas està fet per a la gestió de grups.
![Comanda](./imatges/imatge13.png)
![Comanda](./imatges/imatge14.png)
Per modificar aquest fitxer:
![Comanda](./imatges/imatge15.png)
![Comanda](./imatges/imatge16.png)

**/etc/login.defs**

Aquest fitxer proporciona valors predeterminats  a les comandes “useradd” “passwd” i “login” facilitant la configuració per als usuaris.
![Comanda](./imatges/imatge17.png)
![Comanda](./imatges/imatge18.png)
Per modificar el fitxer:
![Comanda](./imatges/imatge19.png)
![Comanda](./imatges/imatge20.png)

**/etc/default/useradd**

Aquest fitxer conté configuracions predeterminades per a quan es crea un nou usuari amb la comanda useradd.
![Comanda](./imatges/imatge21.png)
![Comanda](./imatges/imatge22.png)
Per accedir al document es en aquesta comanda.
![Comanda](./imatges/imatge23.png)
![Comanda](./imatges/imatge24.png)

**/etc/adduser.conf i /etc/deluser.conf**

Són fitxers que controlen el comportament de les eines adduser i deluser. Son molt mes completes que useradd i userdel.
![Comanda](./imatges/imatge25.png)
![Comanda](./imatges/imatge26.png)

**/etc/Skel**

Aquest fitxer conté una plantilla i directoris predeterminats que se copien directament al directori de **home** dels nous usuaris quan es creen amb la comanda **Useradd**.

Per poder accedir al directori es en aquesta comanda i ja podem observar que estem dins.
![Comanda](./imatges/imatge35.png)

Ara que ja estem dins del directori fem un ls -la i observem els arxius que tenim.
![Comanda](./imatges/imatge36.png) 

Poedem observar que tenim 3 documents amb permisos root.

**.Bash_logout**: Aquest fitxer s'executa quan el usuari tanca la sessió. Coné ordres per netejar recursos o finalitzar processos. 

**.bashrc**:Es carrega a cada sessió, en aquest arxiu es poden definir funcions i varbiales de l'entorn personalitzades.

**.profile**: Aquest fitxer s'executa quan el usuari inicia la sessió.S'utilitza principalment per establir configuracions.

Ara que ja hem aprés que realitzen cada un d'aquests arxius podem fer una prova del seu funcionament.

![Comanda](./imatges/imatge37.png) 
![Comanda](./imatges/imatge38.png) 
En el arxiu .profile hem modificat que la carpeta home de l'usuari en vex de crearse en el /home s'ha de crear en el /var.

![Comanda](./imatges/imatge39.png)
![Comanda](./imatges/imatge40.png)
La modificació que hem realitzat ha segut sobre una comanda, es a dir, que aun fem escribem "connexió" es farà un ls -la.

![Comanda](./imatges/imatge41.png)
![Comanda](./imatges/imatge42.png)
En aquest fitxer he agregat la comanada que he subratllat en la imatge. Aquesta comanada ens vol que elimina tots els arxius dins del directori "Baixades" del usuri actual. S'executa quan la sessió se tanca.  





**UserAdd**

Per crear usuaris s'utilitza aquesta comanada.
Aquesta comanda es la més bàsica, principalment fes de les herramentes de gestío d'usuaris.

![Comanda](./imatges/imatge27.png)
Per verificar que si hem creat el usuari utilitzem el fitxers que he expplicat abans.
![Comanda](./imatges/imatge28.png)
![Comanda](./imatges/imatge43.png)

**adduser** 

Aqeusta comanda realitza varies configuracions, ja que es molt mes cmpleta que la comanada anterior.


**Deluser**

Per eliminar un usuari es en aquesta comanda.
![Comanda](./imatges/imatge27.png)
Comprovem que s’ha borrat, podem observar que ja no es veu el l'usuari.
![Comanda](./imatges/imatge28.png)



**Groupadd**

Creem el grup classe i verifiquem que esta en el fitxer /etc/group.
![Comanda](./imatges/imatge31.png)
![Comanda](./imatges/imatge32.png)

**Delgroup**

Ara eliminem el grup i verifiquem si esta borrat.
![Comanda](./imatges/imatge29.png)
![Comanda](./imatges/imatge30.png)



## Gestió de permisos

## Sistemes de fitxers i particions

## Còpies de seguretat i automatització de tasques

## Quotes de disc
