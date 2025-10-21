🛡️ Projecte 3 — Gestió Segura de Contrasenyes
Tasca 01 — Fase 1 i Fase 2
📢 Context de la Situació

Alerta!!
EverPia ha estat atacada per ciberdelinqüents.
La consultora on esteu de becaris ha patit una fuita d’informació (data breach), i informació confidencial sobre un projecte en desenvolupament està ara en mans de delinqüents que amenacen amb publicar-la si no es paga un rescat.

Aquesta situació ha causat una gran alarma dins la companyia, i s’ha creat un comitè de crisi per gestionar-la.

La investigació interna ha revelat que un dels comptes tècnics va ser compromès a causa de l’ús d’una contrasenya feble o reutilitzada.

⚙️ Resposta de la Direcció Tècnica

Com a resposta a aquesta crisi, la Direcció Tècnica ha emès una directriu:

Tot el personal tècnic ha de començar a utilitzar un gestor de contrasenyes validat per garantir l'ús de credencials úniques i robustes.

Se us encarrega la tasca d’avaluar les opcions i crear la documentació necessària per a la formació del personal.

🧩 Fase 1: Anàlisi i Justificació (Document d'Informe)

Heu de redactar un informe tècnic que justifiqui la decisió de la Direcció i compari les opcions disponibles.

📘 Contingut obligatori de l’informe
1. Introducció i Justificació

Explicació de per què les contrasenyes febles o reutilitzades són un risc crític per a l'empresa (atac de diccionari, credential stuffing, phishing, etc.).

La funció crucial d’un gestor de contrasenyes per mitigar aquests riscos.

2. Comparativa Tècnica

Realitzeu una taula comparativa detallada entre:

Eina	Tipus	Aspectes a Analitzar
Bitwarden	Alternativa Online / Núvol	Sincronització, model de seguretat (xifratge end-to-end), facilitat d’accés multi-dispositiu, cost/model freemium.
KeePassX / KeePassXC	Alternativa Offline / Escriptori	Emmagatzematge local de l’arxiu .kdbx, independència del núvol, model open source, portabilitat.
3. Avantatges i Inconvenients

Resumiu els principals pros i contres de cada model (online vs offline) des del punt de vista de:

Seguretat

Usabilitat

Continuïtat del negoci

4. Recomanació Final

Concloeu l’informe:

Escollint l’eina més adequada per al personal tècnic.

Justificant tècnicament la vostra elecció.

🧭 Fase 2: Guia d’Ús Tècnica (Manual Operatiu)

Utilitzant l’eina seleccionada a la Fase 1 (Bitwarden, KeePassX, o similar), creeu una Guia d’Ús per a l’equip tècnic.

Aquesta guia ha de ser visual, clara i pas a pas, incloent captures de pantalla i explicacions pràctiques.

📋 Contingut obligatori de la guia
1. Instal·lació i Configuració Inicial

Descàrrega i instal·lació del programa.

Creació del compte mestre o de la base de dades principal (.kdbx en KeePass o compte en Bitwarden).

2. Generació de Contrasenyes Segures

Com utilitzar el generador de contrasenyes de l’eina.

Paràmetres: longitud, caràcters especials, aleatorietat, etc.

3. Exemples d’Ús i Emplenament Automàtic

Desar una credencial d’un compte de correu electrònic.

Desar una credencial d’una aplicació o servei web.

Ús de l’extensió del navegador per emplenar automàticament les dades d’inici de sessió.

4. Gestió de Còpies de Seguretat (Backup)

Explicació detallada de com fer una còpia de seguretat:

Arxiu .kdbx (KeePass)

Exportació (Bitwarden)

Recomanacions sobre bones pràctiques d’emmagatzematge segur:

Clau USB xifrada

Emmagatzematge xifrat al núvol

📂 Estructura de Lliurament

Dins el vostre repositori del projecte-3, heu de crear la següent estructura de carpetes:

projecte-3/
└── tasca01/
    ├── README.md        # Descripció general de la tasca
    ├── informe.md       # Document de la Fase 1 (Anàlisi i Justificació)
    ├── guia.md          # Document de la Fase 2 (Guia d’Ús Tècnica)
    └── img/             # Carpeta amb les imatges i captures de pantalla


📝 Important:
Les imatges incloses a la guia han d’estar dins la carpeta img o pics, i s’han de referenciar correctament dins del fitxer guia.md.

🔗 Materials i Links de Suport

INCIBE: Gestión de contraseñas seguras

Pàgina oficial de Bitwarden

Pàgina oficial de KeePassXC

INCIBE: Gestores de contraseñas: qué son y cómo pueden mejorar la seguridad de las empresas
