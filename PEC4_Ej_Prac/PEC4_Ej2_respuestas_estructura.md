# Respon a cadascun dels punts següents:
1.  (0.75 punts) Quina ordre has d'utilitzar per crear un nou projecte Angular utilitzant Angular CLI anomenat ecommerce? (A les preguntes que us faci Angular CLI pots contestar utilitzant les opcions per defecte).

R/ L'ordre a utilitzar per crear un nou projecte Angular anomenat ecommarce és 'ng new ecommerce'. 

Amb Angular Cli crea el projecte angular ecommerce i explica breument l'estructura i els fitxers que ha generat Angular CLI:
## Estructura:
Executant l'ordre 'ng new ecommerce' s'ha creat la següent estructura (omitin els fitxer de configuració):
    Una carpeta 'src' que és el directori principal on es desenvolupa l'aplicació. 
    Dins de src hi ha:
        'index.html': Fitxer HTML principal que s'envia al navegador.
        'main.ts': Punt d'entrada per a la compilació de TypeScript.
        'styles.css': Fitxer de full d'estils global per a l'aplicació.
        'app': Directori on es desenvolupa el codi de l'aplicació. 
        Dins d'aquest directori hi ha:
            app.component.*: Fitxers del component principal (tipuscript, html, css).
            app.module.ts: Fitxer que defineix el mòdul principal de l'aplicació.

## Fitxers de configuració a l'arrel del projecte:

    o .editorconfig > Es un fitxer de configuració per a l'editor de codi. Defineix les preferències d'estil de codi per al desenvolupament.
    o .gitignore > Es un fitxer que especifica els arxius i directoris que s'han d'ignorar quan es fa servir el control de versions Git.
    o angular.json > Es un fitxer de configuració principal per al projecte Angular. Conté configuracions per a la construcció, les proves, els entorns, etc.
    o package-lock.json >   Es un fitxer generat pel gestor de paquets npm per fixar les versions exactes de les dependències del projecte.
    o package.json  > Es un fitxer de configuració de paquets per a npm. Conté informació sobre el projecte i les dependències.
    o server.ts > és un fitxer typescript on hi ha un petit servidor d'express per al projecte d'Angular en el que ens trobem. S'utilitza principalment per a les proves locals.
    o tsconfing.app.json > Es un fitxer de configuració TypeScript específic per a l'aplicació. Conté opcions de compilació per a la part client de l'aplicació.
    o tsconfig.json > Es un fitxer de configuració TypeScript global per al projecte. Conté configuracions de TypeScript per a tot el projecte.
    o tsconfig.spec.json > Es un fitxer de configuració TypeScript per a les proves. Conté opcions de compilació específiques per a les proves.

• Directori node_modules > Aquest directori conté les dependències del projecte

• Directori src: > Directori de l'entorn de desenvolupament.
    o index.html > Fitxer principal de l'aplicació. És el HTML principal.
    o main.ts > Punt d'entrada de l'aplicació.
    o styles.css > Arxiu d'estils global de l'aplicació
    o Directori assets > Conté els recursos de l'aplicació com ara imatges i possibles arxius de configuració.
    o Directori app
        ▪ Fitxers app.component.* > els 3 fitxers .ts .html i .css és on tenim el codi del component principal, la plantilla del component principal i els estils d'aquest component respectivament. Son 3 arxius indispensables per tenir un component creat dins un projecte basat en Angular.
        ▪ Fitxers app.module.ts > Aquest fitxer 'app.module.ts' no ha estat generat. Buscant informació sobre ell, diuen que és el fitxer que declara el mòdul principal de l'aplicació.


2. (0.25 punts) Explica cadascun dels següents decoradors generats per Angular CLI, detallant cadascuna de les propietats que es defineixen a:
• app.module.ts - @NgModule (declarations, imports, providers, bootstrap).
  R/ 'declarations' es l'array que conté els components, directives i pipes que pertanyen a aquest mòdul. 'imports' altres mòduls que s'han d'importar. 'providers' indica els serveis proporcionats pel mòdul. Per últim 'bootstrap' és el component principal a ser carregat en el llençament de l'aplicació.

• app.component.ts - @Component (selector, templateUrl, styleUrls).
  R/ 'selector' és l'etiqueta HTML utilitzada per referenciar el component en altres fitxers HTML. 'templateUrl' és la ruta al fitxer HTML que defneix la plantilla del component. Per últim, 'styleUrls' és l'array de rutes als fitxers de fulls d'estil CSS que s'apliquen al component.

3. (0.25 punts) És possible poder injectar el template i els estils en línia d'un component sense necessitat d'especificar-los a templateUrl, styleUrls? És recomanable fer-ho?

R/ Sí és possible. Es pot injectar el template i els estils directament en línia en el component sense utilitzar 'templateUrl' o 'styleUrls'. Es podria fer utilitzant les propietats 'template' i 'styles' dins del decorador '@component'. Per exemple:

@Component ({
  selector: 'app-component-x',
  template: '<h1>Hola Mon, aquest és el meu template en línia. </h1>',
  styles: ['h1{ color: red; }']
})
export class ComponentX{}

De totes maneres crec que no es recomanable fer-ho ja que de normal si el 'template' o 'styles' és quelcom extens serà díficil fer el manteniment o si ho volem reutilitzar en altres parts de l'aplicació, si ho fem així, no es podrà fer.
