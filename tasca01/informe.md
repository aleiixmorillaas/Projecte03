# Fase 1: Anàlisi i Justificació (Document d'Informe)

## Índex

1. [Introducció i Justificació](#1-introducció-i-justificació)
2. [Comparativa Tècnica: Bitwarden vs KeePassXC](#2-comparativa-tècnica-bitwarden-vs-keepassxc)
3. [Avantatges i Inconvenients](#3-avantatges-i-inconvenients)

   * [Bitwarden (Online / Núvol)](#bitwarden-online--núvol)
   * [KeePassXC (Offline / Escriptori)](#keepassxc-offline--escriptori)
4. [Recomanació Final](#4-recomanació-final)
5. [Conclusió](#conclusió)

---

## 1. Introducció i Justificació

L’incident de seguretat recent sofert per **EverPia** ha posat de manifest una de les vulnerabilitats més habituals dins les organitzacions: **l’ús de contrasenyes febles o reutilitzades**. Aquest tipus de pràctiques facilita diversos vectors d’atac que poden comprometre comptes i informació crítica:

* **Atacs de diccionari:** els atacants proven combinacions freqüents de paraules o patrons senzills per accedir a comptes protegits amb contrasenyes comunes (ex.: `123456`, `password`, `Everpia2024`).
* **Credential stuffing:** quan les credencials d’una fuita anterior són reutilitzades en altres serveis, els atacants poden automatitzar proves massives d’inici de sessió i accedir a múltiples sistemes amb una sola combinació robada.
* **Phishing i keylogging:** fins i tot si una contrasenya és robusta, la manca d’un sistema centralitzat per gestionar-les augmenta la probabilitat d’errors humans (reutilització, emmagatzematge insegur, etc.).

Per acabar amb aquests riscos, la implementació d’un **gestor de contrasenyes corporatiu** és essencial. Aquest tipus d’eines permet:

* Generar contrasenyes úniques, complexes i aleatòries per a cada servei.
* Emmagatzemar-les de manera xifrada (*end-to-end encryption*).
* Sincronitzar-les de forma segura entre dispositius (en el cas dels serveis en núvol).
* Reduir la dependència de la memòria humana i minimitzar l’ús de contrasenyes febles o repetides.


## 2. Comparativa Tècnica: Bitwarden vs KeePassXC

| **Criteri**                        | **Bitwarden (Online / Núvol)**                              | **KeePassXC (Offline / Escriptori)**          |
| ---------------------------------- | ----------------------------------------------------------- | --------------------------------------------- |
| **Model d’emmagatzematge**         | En núvol (servidors propis o auto-allotjats)                | Local, arxiu `.kdbx` xifrat                   |
| **Xifratge**                       | End-to-end amb AES-256, PBKDF2 i Argon2                     | AES-256 amb SHA-256 per a la integritat       |
| **Codi font**                      | 100% open source (clients i servidor)                       | 100% open source                              |
| **Sincronització**                 | Automàtica entre dispositius (navegador, mòbil, escriptori) | Manual (mitjançant serveis externs si es vol) |
| **Accessibilitat**                 | Web, extensions, app mòbil                                  | Escriptori (Windows, macOS, Linux), portable  |
| **Autenticació multifactor (2FA)** | Inclosa (TOTP, U2F, YubiKey)                                | Depèn de *plugins* o eines externes           |
| **Cost / Model freemium**          | Gratuït amb opcions premium (USD 10/any)                    | Gratuït (sense subscripcions)                 |
| **Administració d’equips**         | Gestió d’usuaris i compartició segura                       | Limitat, sense gestió centralitzada           |
| **Dependència d’internet**         | Necessari per sincronitzar (mode offline temporal)          | Totalment independent d’internet              |
| **Còpies de seguretat**            | Automàtiques al núvol                                       | Manual, a càrrec de l’usuari o IT             |
| **Compatibilitat corporativa**     | Integracions amb SSO, Active Directory, API                 | Limitat; orientat a ús individual o tècnic    |


## 3. Avantatges i Inconvenients

### Bitwarden (Online / Núvol)

**Avantatges:**

* Sincronització automàtica entre dispositius.
* Gestió centralitzada d’usuaris i polítiques de seguretat.
* Xifratge *end-to-end* (ni el proveïdor pot accedir a les dades).
* Compatible amb entorns corporatius i treball en equip.
* Interfície intuïtiva i fàcil d’adoptar per personal no tècnic.

**Inconvenients:**

* Dependència parcial del núvol i d’internet.
* Possibilitat (encara que mínima) d’exposició si es compromet el servei remot.
* Cost associat per a funcionalitats avançades.


### KeePassXC (Offline / Escriptori)

**Avantatges:**

* Total control local de les dades (no depèn de tercers).
* Sense costos recurrents ni subscripcions.
* Ideal per a entorns amb requisits d’aïllament o alta confidencialitat.
* Portable i lleuger.

**Inconvenients:**

* No sincronitza automàticament entre dispositius.
* Gestió d’usuaris i còpies de seguretat manual.
* Major risc de pèrdua de dades si no s’estableix un sistema de *backup* adequat.
* Corba d’aprenentatge més pronunciada per a usuaris no tècnics.


## 4. Recomanació Final

Després de valorar els factors de seguretat, usabilitat i continuïtat operativa, **es recomana la implementació de Bitwarden** com a gestor de contrasenyes corporatiu per al personal tècnic d’EverPia.

**Justificació:**

* Ofereix xifratge *end-to-end* amb la possibilitat d’auto-allotjament als servidors de la companyia, eliminant riscos de tercers.
* Facilita la sincronització entre dispositius (essencial en entorns de treball híbrids).
* Inclou gestió d’equips i polítiques de seguretat centralitzades, cosa que simplifica el control per part del departament IT.
* Manté un cost baix i escalable comparat amb altres solucions comercials.
* Redueix la superfície d’error humà i incrementa la maduresa en ciberseguretat dins de l’organització.


## Conclusió

Adoptar **Bitwarden** com a eina corporativa de gestió de contrasenyes representa una mesura tècnica i estratègica clau per **reforçar la seguretat interna d’EverPia**, prevenir incidents similars i establir bones pràctiques en la protecció de credencials.

