## Arquitectura desplegada

Opció simple: Un únic servidor que executa tant el servei web com la base de dades.
Opció avançada: Separació per rols, amb una VM per al servidor web (apache2+php) i una altra per a la BBDD (MySQL), comunicant-se per xarxa privada virtual.


## Repositori i estructura

S’ha creat un repositori a GitHub, que és públic.
El directori inicial conté un README.md descriptiu.
Dins el directori docs hi ha aquesta documentació en Markdown (instal·lacio.md) i un altre README.md indicant el contingut del directori.


## Exemples funcionament i demostració

És imprescindible afegir captures de pantalla on es pugui veure:
La web desplegada correctament.
Com es connecta a la base de dades sense errors.
Resultats visibles d’operacions (ex. inserció o consulta de dades).

## Check-list i bugs corregits

S’han identificat els “bugs” del codi i arreglat via commit al repositori.
S’ha deixat constància dels canvis al registre de Git.
El sistema arrenca correctament sense errors de permisos ni autenticació.


