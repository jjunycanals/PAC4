Explica què fa cadascuna de les opcions següents d'Angular CLI:

1. ng new : aquesta opció és utilitzada per a crear un nou projecte en angular. Quan l'usuari executa el comandament 'ng new nom-del-projecte" pots crear un projecte basat en angular mitjançant un assistent que et fa 3 preguntes. Aquest comandament crea l'estructura del projecte, configura les dependències i estableix un entorn de desenvolupament bàsic per a començar a treballar.

2. ng generate : s'utilitza per generar codi automàticament i té varies possibles aplicacions.
>component : ng generate component nom-del-component serveix per a generar un nou componenet d'angular. És a dir, es generen els arxius per un component especific incloent el typescript, plantilla HTML, estils CSS i altres arxius que hi pugui haver relacionats.
>directive : ng generate directive genera una nova directiva Angular. 
>enum : ng generate enum nom-del-enumerat genera un nou enumerat. En especific genera un arxiu Typescript amb el seu enumerat.
>guard : ng generate guard nom-del-guard genera un nou guard.
>interface : ng generate interface nom-interface genera una nova interfície.
>pipe  : ng generate pipe nom-pipe genera un nou filtre.
>service : ng generate service nom-service genera un nou servei.

3. ng serve : aquest comandament inicia el servidor de desenvolupament d'Angular i alhora fa recarges automàtiques. Això ens permet iniciar de manera local la nostra aplicació d'Angular en el navegador. Els canvis de codi es decten a temps real en l'entorn de desenvolupmanet i l'aplicació es recarrega auotmàticament perquè veiem de manera local els canvis reflexats en el navegador.

4. ng test : ng test executa proves unitaries de tests unitaris de l'aplicació d'Angular. Aquesta ordre inicia l'execució de les proves i retorna els resultats d'aquestes. Així se sap si l'aplicació passa els tests unitaris o no.

5. ng version : aquesta ordre retorna la versió d'Angular i de totes les seves dependències. És útil per saber la versió actual de Angular CLI que s'està utilitzant en el projecte. També per les dependències com per exemple, Angular Core, TypeScript i altres paquets importants.

