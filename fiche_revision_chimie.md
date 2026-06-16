# Fiche de Révision : Chimie
*Basée sur le Cadre Référentiel du Concours/Examen de Sortie CRMEF (Physique-Chimie)*

Cette fiche récapitule de manière structurée et rigoureuse l'ensemble des connaissances théoriques, relations mathématiques, règles de nomenclature, représentations géométriques et mécanismes réactionnels à maîtriser pour la partie **Chimie** (qui représente **40%** de l'épreuve de spécialité de Physique-Chimie, soit **24 points sur 60**).

---

## 📌 Sommaire
1. [Chimie des Solutions Aqueuses](#1-chimie-des-solutions-aqueuses)
2. [Cinétique Chimique](#2-cinétique-chimique)
3. [Structure de la Matière et Liaisons Chimiques](#3-structure-de-la-matière-et-liaisons-chimiques)
4. [Géométrie et Stéréochimie des Molécules](#4-géométrie-et-stéréochimie-des-molécules)
5. [Techniques Expérimentales d'Extraction, Purification et Analyse](#5-techniques-expérimentales-dextraction-purification-et-analyse)
6. [Réactivité Organique et Mécanismes Réactionnels](#6-réactivité-organique-et-mécanismes-réactionnels)

---

## 1. Chimie des Solutions Aqueuses

### 🧪 Grandeurs Physiques en Solution
*   **Concentration molaire :** $C = \frac{n}{V} = \frac{m}{M \cdot V} = \frac{t}{M}$ (en $\text{mol/L}$)
*   **Concentration massique (titre) :** $t = \frac{m}{V} = C \cdot M$ (en $\text{g/L}$)
*   **Fraction molaire du constituant $i$ :** $x_i = \frac{n_i}{n_{\text{total}}}$ (sans unité, $\sum x_i = 1$)
*   **Relation avec la densité $d$ et le pourcentage massique $P\%$ :**
    $$C = \frac{d \cdot \rho_{\text{eau}} \cdot P\%}{M}$$
    *(Avec $\rho_{\text{eau}} = 1000\text{ g/L}$ ; si la densité $d$ est donnée, la masse volumique de la solution est $\rho_{\text{sol}} = d \cdot \rho_{\text{eau}}$).*

---

### ⚖️ Réactions Acido-Basiques (Selon Brønsted)
*   **Définition :** Un acide libère un proton $\text{H}^+$ ; une base capte un proton $\text{H}^+$.
*   **pH d'une solution aqueuse :** $pH = -\log [H_3O^+]$ (valable en solution diluée, activité $a(H_3O^+) \approx [H_3O^+]/C^\circ$).
*   **Autoprotolyse de l'eau :** $2 H_2O \rightleftharpoons H_3O^+ + OH^-$. Produit ionique : $K_e = [H_3O^+][OH^-] = 10^{-14}$ à $25^\circ\text{C}$ ($pK_e = 14$).
*   **Constante d'acidité $K_a$ (pour le couple $AH / A^-$) :**
    $$AH + H_2O \rightleftharpoons A^- + H_3O^+ \implies K_a = \frac{[A^-][H_3O^+]}{[AH]} \implies pK_a = -\log K_a$$
*   **Relation de Henderson-Hasselbalch :**
    $$pH = pK_a + \log \frac{[A^-]}{[AH]}$$
*   **Diagramme de prédominance :**
    *   Si $pH < pK_a \implies [AH] > [A^-]$ : la forme acide $AH$ prédomine.
    *   Si $pH > pK_a \implies [AH] < [A^-]$ : la forme basique $A^-$ prédomine.
    *   Si $pH = pK_a \implies [AH] = [A^-]$ (demi-équivalence dans un dosage).

```
                  AH prédomine             A- prédomine
             -----------------------|-----------------------> pH
                                   pKa
```

*   **Calculs de pH de solutions simples (approximations usuelles) :**
    *   **Acide fort** de concentration $C$ : $pH = -\log C$ (si $C \ge 10^{-6}\text{ M}$)
    *   **Base forte** de concentration $C$ : $pH = pK_e + \log C$
    *   **Acide faible** de concentration $C$ : $pH = \frac{1}{2}(pK_a - \log C)$ (valable si l'acide est peu dissocié, soit $pH \le pK_a - 1$)
    *   **Base faible** de concentration $C$ : $pH = \frac{1}{2}(pK_e + pK_a + \log C)$ (valable si la base est peu protonée, soit $pH \ge pK_a + 1$)
    *   **Solution tampon** (mélange équimolaire d'acide faible et de sa base conjuguée) : $pH \approx pK_a$. Le pH d'une solution tampon varie très peu lors de l'ajout d'une petite quantité d'acide ou de base forte, ou lors d'une dilution modérée.

---

### ❄️ Réactions de Précipitation et Solubilité
*   **Équilibre de dissolution :** $A_m B_n(s) \rightleftharpoons m A^{n+}(aq) + n B^{m-}(aq)$.
*   **Produit de solubilité $K_s$ :**
    $$K_s = [A^{n+}]_{\text{éq}}^m \cdot [B^{m-}]_{\text{éq}}^n$$
*   **Solubilité $s$ (en $\text{mol/L}$) :** Quantité maximale de solide qu'on peut dissoudre dans $1\text{ L}$ de solution.
    *   *Exemple pour $AgCl(s) \rightleftharpoons Ag^+ + Cl^-$ :* $K_s = s \cdot s = s^2 \implies s = \sqrt{K_s}$.
    *   *Exemple pour $Al(OH)_3(s) \rightleftharpoons Al^{3+} + 3 OH^-$ :* $K_s = (s) \cdot (3s)^3 = 27 s^4 \implies s = \left(\frac{K_s}{27}\right)^{1/4}$.
*   **Condition de précipitation (comparaison entre $Q_r$ et $K_s$) :**
    *   Si $Q_r < K_s$ : La solution est insaturée (pas de précipité).
    *   Si $Q_r = K_s$ : La solution est saturée (apparition du premier grain de précipité).
    *   Si $Q_r > K_s$ : Il y a précipitation immédiate jusqu'à ce que $Q_r = K_s$ à l'équilibre.
*   **Effet d'ion commun :** La solubilité d'un sel diminue fortement si l'on dissout ce sel dans une solution contenant déjà l'un de ses ions constitutifs.
*   **Influence du pH :** La solubilité d'un précipité contenant une base conjuguée d'acide faible (ex : hydroxydes $M(OH)_n$, carbonates $MCO_3$) augmente lorsque le pH diminue (milieu acide), car les protons $\text{H}^+$ consomment la base, ce qui déplace l'équilibre de dissolution dans le sens direct (principe de Le Chatelier).

---

### ⚡ Réactions d'Oxydo-Réduction
*   **Oxydant (Ox) :** Espèce capable de capter des électrons.
*   **Réducteur (Red) :** Espèce capable de céder des électrons.
*   **Nombre d'oxydation (n.o.) :** Charge fictive affectée à un atome au sein d'une structure pour quantifier son état d'oxydation.
    *   *Règles d'attribution :* corps simple neutre (n.o. = 0) ; hydrogène combiné (n.o. = +I, sauf hydrures -I) ; oxygène combiné (n.o. = -II, sauf peroxydes -I et avec F) ; somme des n.o. = charge globale de l'espèce.
    *   *Oxydation :* Augmentation du n.o. (perte d'électrons).
    *   *Réduction :* Diminution du n.o. (gain d'électrons).
*   **Équation de Nernst :** Électrode caractérisée par le couple $Ox + n e^- \rightleftharpoons Red$ :
    $$E = E^\circ + \frac{R T}{n F} \ln \left(\frac{a_{Ox}}{a_{Red}}\right)$$
    À $T = 298\text{ K}$ ($25^\circ\text{C}$), en remplaçant les activités par les concentrations (en $\text{mol/L}$) :
    $$E = E^\circ + \frac{0,059}{n} \log \left(\frac{[Ox]}{[Red]}\right)$$
    *(Où $E^\circ$ est le potentiel standard du couple, $n$ le nombre d'électrons échangés, $F = 96485\text{ C/mol}$ le Faraday).*
*   **Force électromotrice d'une pile (f.e.m. $e$) :**
    $$e = E^+ - E^- = E_{\text{cathode}} - E_{\text{anode}} > 0$$
    *   *Rappel électrode :* **A**node = **A**ttaque = **O**xydation (borne $-$). **C**athode = **C**onsommation = **R**éduction (borne $+$).
*   **Loi de Faraday (Électrolyse) :** La quantité de matière de substance produite ou consommée à une électrode est liée à la quantité d'électricité $Q$ injectée :
    $$Q = I \cdot \Delta t = n(e^-) \cdot F \implies m = \frac{I \cdot \Delta t \cdot M}{n \cdot F}$$

---

## 2. Cinétique Chimique

### ⏱️ Vitesse de Réaction
Pour une réaction générale $a A + b B \longrightarrow p P + q Q$ :
*   **Vitesse volumique de réaction $v$ :**
    $$v(t) = \frac{1}{V} \frac{\mathrm{d}\xi}{\mathrm{d}t} = -\frac{1}{a} \frac{\mathrm{d}[A]}{\mathrm{d}t} = \frac{1}{p} \frac{\mathrm{d}[P]}{\mathrm{d}t}$$
    *(Où $\xi$ est l'avancement de la réaction en moles et $V$ le volume de la solution).*
*   **Loi de vitesse avec ordre :** La réaction admet un ordre si la vitesse s'exprime sous la forme :
    $$v = k [A]^p [B]^q$$
    (Où $k$ est la constante de vitesse, et $p, q$ sont les ordres partiels par rapport aux réactifs $A$ et $B$. L'ordre global est $n = p + q$).

---

### 📉 Lois de Vitesse Intégrées (Pour un réactif unique $A \longrightarrow Produits$)

| Ordre de réaction | Équation différentielle | Loi de vitesse intégrée | Temps de demi-réaction $t_{1/2}$ | Unité de $k$ |
| :---: | :--- | :--- | :---: | :---: |
| **Ordre 0** | $$-\frac{\mathrm{d}[A]}{\mathrm{d}t} = k$$ | $$[A](t) = [A]_0 - k \cdot t$$ | $$t_{1/2} = \frac{[A]_0}{2k}$$ | $$\text{mol}\cdot\text{L}^{-1}\cdot\text{s}^{-1}$$ |
| **Ordre 1** | $$-\frac{\mathrm{d}[A]}{\mathrm{d}t} = k[A]$$ | $$[A](t) = [A]_0 e^{-k \cdot t}$$ | $$t_{1/2} = \frac{\ln 2}{k}$$ | $$\text{s}^{-1}$$ |
| **Ordre 2** | $$-\frac{\mathrm{d}[A]}{\mathrm{d}t} = k[A]^2$$ | $$\frac{1}{[A](t)} = \frac{1}{[A]_0} + k \cdot t$$ | $$t_{1/2} = \frac{1}{k [A]_0}$$ | $$\text{L}\cdot\text{mol}^{-1}\cdot\text{s}^{-1}$$ |

> [!NOTE]
> *   **Temps de demi-réaction $t_{1/2}$ :** Durée nécessaire pour que la moitié du réactif limitant soit consommée : $[A](t_{1/2}) = \frac{[A]_0}{2}$.
> *   Pour l'ordre 1, le temps de demi-réaction est **indépendant** de la concentration initiale $[A]_0$.

---

### 🔥 Facteurs Cinétiques et Loi d'Arrhenius
Les facteurs cinétiques (température, concentration des réactifs, catalyseurs) modifient la vitesse d'évolution d'un système.
*   **Loi d'Arrhenius :** Modélise l'influence de la température $T$ (en Kelvin) sur la constante de vitesse $k$ :
    $$k(T) = A \cdot e^{-\frac{E_a}{R T}} \implies \ln k = \ln A - \frac{E_a}{R T}$$
    *(Où $E_a$ est l'énergie d'activation en $\text{J/mol}$, $R \approx 8.314\text{ J}\cdot\text{K}^{-1}\cdot\text{mol}^{-1}$ la constante des gaz parfaits, et $A$ le facteur pré-exponentiel).*
*   **Catalyse :** Un catalyseur accélère une réaction en proposant un nouveau chemin réactionnel de plus faible énergie d'activation ($E_a' < E_a$), sans modifier l'état d'équilibre thermodynamique du système. Il est régénéré en fin de réaction.
    *   *Catalyse homogène :* réactifs et catalyseur forment une seule phase (ex: ions en solution).
    *   *Catalyse hétérogène :* phases distinctes (ex: gaz réactifs sur métal solide).
    *   *Catalyse enzymatique :* catalysée par des macromolécules biologiques (spécificité très élevée).

---

## 3. Structure de la Matière et Liaisons Chimiques

### ⚛️ Configuration Électronique des Atomes
L'état d'un électron dans un atome est défini par 4 nombres quantiques :
*   $n$ (principal, couche) : $n \ge 1$.
*   $l$ (azimutal, sous-couche) : $0 \le l \le n-1$ (notations : $l=0\to s$, $l=1\to p$, $l=2\to d$, $l=3\to f$).
*   $m_l$ (magnétique, orbitale) : $-l \le m_l \le +l$.
*   $m_s$ (de spin) : $\pm 1/2$.

#### 📜 Règles de remplissage
1.  **Règle de Klechkowski :** Le remplissage des sous-couches se fait par ordre de somme $(n+l)$ croissant. En cas d'égalité, la sous-couche ayant le plus petit $n$ est remplie en premier.
    *   *Ordre :* $1s \to 2s \to 2p \to 3s \to 3p \to 4s \to 3d \to 4p \to 5s \dots$
2.  **Principe d'exclusion de Pauli :** Deux électrons d'un même atome ne peuvent pas avoir leurs 4 nombres quantiques identiques (au maximum 2 électrons par case quantique, de spins opposés $\uparrow\downarrow$).
3.  **Règle de Hund :** Pour une sous-couche dégénérée (ex : les trois orbitales $2p$), les électrons occupent un maximum d'orbitales avec des spins parallèles avant de s'apparier.

> [!WARNING]
> **Exceptions notables de la ligne 3d :**
> *   **Chrome ($Z=24$) :** configuration $[Ar] 4s^1 3d^5$ (et non $4s^2 3d^4$).
> *   **Cuivre ($Z=29$) :** configuration $[Ar] 4s^1 3d^{10}$ (et non $4s^2 3d^9$).
> *   *Raison :* Les configurations à sous-couche $d$ demi-remplie ($3d^5$) ou complètement remplie ($3d^{10}$) possèdent une stabilité énergétique accrue.

---

### 🤝 Liaisons Chimiques

#### 1. Liaisons Fortes (Intramoléculaires, de forte énergie $\sim 100-800\text{ kJ/mol}$)
*   **Liaison covalente :** Mise en commun de doublets d'électrons entre deux atomes non-métaux ayant des électronégativités proches. Si la différence d'électronégativité $\Delta\chi$ augmente ($0,4 \le \Delta\chi < 1,7$), la liaison est **covalente polarisée**.
*   **Liaison ionique :** Transfert complet d'électrons d'un atome peu électronégatif (métal) vers un atome très électronégatif (non-métal) ($\Delta\chi \ge 1,7$). Cohésion assurée par des forces électrostatiques omnidirectionnelles (ex: $NaCl$).
*   **Liaison métallique :** Partage d'électrons de valence délocalisés ("gaz d'électrons") entre un réseau d'ions métalliques positifs.

#### 2. Liaisons Faibles (Intermoléculaires, de faible énergie $\sim 1-40\text{ kJ/mol}$)
*   **Forces de Van der Waals :** Forces d'interactions électrostatiques de trois natures :
    *   *Keesom :* entre dipôles permanents (molécules polaires).
    *   *Debye :* entre un dipôle permanent et un dipôle induit.
    *   *London :* entre dipôles instantanés (présentes dans toutes les molécules, y compris apolaires).
*   **Liaison Hydrogène :** Liaison très directive établie lorsqu'un atome d'hydrogène (lié de manière covalente à un atome très électronégatif $F, O, N$) interagit avec le doublet non liant d'un autre atome très électronégatif voisin.
    *   *Conséquence physique :* Les liaisons hydrogène augmentent considérablement les températures de fusion et d'ébullition (ex: $H_2O$ bout à $100^\circ\text{C}$ alors que $H_2S$ bout à $-60^\circ\text{C}$).

---

## 4. Géométrie et Stéréochimie des Molécules

### 📐 Théorie VSEPR (Valence Shell Electron Pair Repulsion)
La géométrie autour d'un atome central $A$ entouré de $n$ atomes $X$ et possédant $m$ doublets non liants $E$ (noté $AX_nE_m$) est régie par la répulsion maximale des doublets (liants et non liants).

| Formule | Nombre de directions $(n+m)$ | Géométrie des doublets | Géométrie de la molécule | Angles théoriques | Exemples |
| :---: | :---: | :---: | :---: | :---: | :---: |
| **$AX_2E_0$** | 2 | Linéaire | **Linéaire** | $180^\circ$ | $CO_2, BeCl_2$ |
| **$AX_3E_0$** | 3 | Trigone plan | **Trigonal plan** | $120^\circ$ | $BF_3, HCHO$ |
| **$AX_2E_1$** | 3 | Trigone plan | **Coudée** | $< 120^\circ$ | $SO_2, O_3$ |
| **$AX_4E_0$** | 4 | Tétraédrique | **Tétraédrique** | $109,5^\circ$ | $CH_4, SiCl_4$ |
| **$AX_3E_1$** | 4 | Tétraédrique | **Pyramide trigonale** | $107^\circ$ | $NH_3, H_3O^+$ |
| **$AX_2E_2$** | 4 | Tétraédrique | **Coudée** | $104,5^\circ$ | $H_2O$ |

---

### 🧬 Stéréochimie et Représentations
1.  **Représentation de Cram :** Représentation tridimensionnelle standard. Les liaisons dans le plan sont dessinées par des traits simples, les liaisons vers l'avant par des triangles pleins ($\blacktriangle$), et les liaisons vers l'arrière par des pointillés/hachures ($\text{---}$).
2.  **Projection de Newman :** Regard le long de l'axe d'une liaison simple carbone-carbone $C-C$. Le carbone avant est représenté par un point d'intersection de trois liaisons, et le carbone arrière par un grand cercle.
    *   Permet d'analyser les stéréoisomères de **conformation** (décalée, éclipsée). La conformation la plus stable pour l'éthane ou le butane est la **conformation décalée anti** car elle minimise la gêne stérique.
3.  **Projection de Fischer :** La chaîne carbonée principale est verticale, le carbone au n.o. le plus élevé étant situé en haut. Les liaisons verticales partent vers l'arrière, les horizontales vers l'avant.

```
       CRAM                      NEWMAN (butane décalé anti)           FISCHER
        H                                  CH3                            CHO
        |                               H      H                          |
    H-- C* --OH                          \    /                      H -- C -- OH
       / \                                C--C                            |
     H3C  COOH                          /    \                       H -- C -- OH
                                       H      H                           |
                                          CH3                            CH2OH
```

---

### 🔀 Stéréoisomérie (Isomérie Géométrique)

#### 1. Règles de Cahn-Ingold-Prelog (CIP) pour l'ordre de priorité des substituants
*   **Règle 1 :** Un atome de numéro atomique $Z$ plus élevé est prioritaire sur un atome de $Z$ plus faible : $-\text{OH} (Z=8) > -\text{CH}_3 (Z=6) > -\text{H} (Z=1)$.
*   **Règle 2 :** En cas d'égalité sur le premier atome lié, on compare les atomes de la liste suivante (au rang 2). Le carbone de $-\text{CH}_2-\text{OH}$ est prioritaire sur le carbone de $-\text{CH}_2-\text{CH}_3$ car le premier est lié à $(O, H, H)$ alors que le second est lié à $(C, H, H)$.
*   **Règle 3 :** Les liaisons multiples sont traitées comme des liaisons simples dupliquées (ex : le carbonyle $-\text{CH}=\text{O}$ équivaut à un carbone lié à deux oxygènes et un hydrogène : $(O, O, H)$).

#### 2. Configuration Absolue $R / S$ (Carbone Asymétrique $C^*$)
Après avoir classé les 4 substituants par priorité CIP décroissante ($1 > 2 > 3 > 4$) :
*   On regarde la molécule selon l'axe $C^* \to 4$ (le substituant 4 étant placé à l'arrière).
*   **Configuration $R$ (Rectus) :** Le sens de rotation $1 \to 2 \to 3$ est le sens horaire.
*   **Configuration $S$ (Sinister) :** Le sens de rotation $1 \to 2 \to 3$ est le sens anti-horaire.

#### 3. Configuration Géométrique $E / Z$ (Liaisons Doubles)
Pour chaque carbone d'une double liaison $C=C$, on détermine le substituant prioritaire CIP (notés $P_1$ et $P_2$) :
*   **Configuration $Z$ (Zusammen) :** Les deux groupes prioritaires sont du même côté du plan perpendiculaire à la double liaison.
*   **Configuration $E$ (Entgegen) :** Les deux groupes prioritaires sont de part et d'autre (opposés).

#### 4. Relations entre Stéréoisomères
*   **Chiralité :** Propriété d'un objet de ne pas être superposable à son image dans un miroir plat (présence d'un carbone asymétrique sans plan ni centre de symétrie).
*   **Énantiomères :** Deux stéréoisomères de configuration qui sont images l'un de l'autre dans un miroir, mais non superposables. Ils ont les mêmes propriétés physiques (sauf le pouvoir rotatoire optique).
*   **Diastéréoisomères :** Stéréoisomères de configuration qui ne sont pas énantiomères (ex : isomères $Z/E$, ou molécules à plusieurs carbones asymétriques qui diffèrent sur la configuration de certains carbones mais pas sur tous). Ils ont des propriétés physiques et chimiques différentes.

---

## 5. Techniques Expérimentales d'Extraction, Purification et Analyse

### 🧪 Techniques d'Extraction et de Séparation
*   **Extraction par solvant (liquide-liquide) :** Permet de transférer un soluté d'un solvant initial à un solvant d'extraction non miscible.
    *   *Choix du solvant d'extraction :* Le soluté doit y être très soluble ; le solvant d'extraction doit être non miscible avec le solvant de départ ; sa température d'ébullition doit être faible pour pouvoir l'évaporer facilement.
*   **Hydrodistillation (ou entraînement à la vapeur) :** Extraction d'espèces organiques peu volatiles et insolubles dans l'eau à partir de matières végétales. Le mélange d'eau et d'huile essentielle s'évapore sous forme de mélange azéotropique à une température inférieure à $100^\circ\text{C}$, évitant la dégradation thermique des composés organiques.

### 🧼 Techniques de Purification
*   **Recristallisation (pour les solides) :** Basée sur la différence de solubilité à chaud et à froid du solide à purifier dans un solvant bien choisi. À chaud, le solide et ses impuretés sont solubles. Par refroidissement lent, le composé d'intérêt recristallise sous forme pure tandis que les impuretés restent en solution.
*   **Distillation fractionnée (pour les liquides) :** Séparation des constituants d'un mélange de liquides miscibles ayant des températures d'ébullition différentes grâce à une colonne de Vigreux. Le constituant le plus volatil s'échappe en tête de colonne en premier.

---

### 📊 Techniques d'Identification et Caractérisation

#### 1. Spectroscopie Infrarouge (IR)
Permet d'identifier les groupes fonctionnels d'une molécule par absorption des vibrations moléculaires (les bandes d'absorption pointent vers le bas).
*   **Bande $-\text{OH}$ (Alcool) :**
    *   *Libre (phase gaz) :* bande fine et intense vers $3600\text{ cm}^{-1}$.
    *   *Lié (liaisons hydrogène en phase condensée) :* bande très large et intense vers $3200-3400\text{ cm}^{-1}$.
*   **Bande $\text{C}=\text{O}$ (Carbonyle) :** bande très intense et relativement fine vers $1700-1750\text{ cm}^{-1}$ (caractéristique des cétones, aldéhydes, esters et acides carboxyliques).
*   **Bande $-\text{OH}$ (Acide carboxylique) :** bande extrêmement large s'étendant de $2500$ à $3200\text{ cm}^{-1}$ superposée aux bandes d'absorption $\text{C}-\text{H}$.

#### 2. Spectroscopie RMN du Proton ($^1\text{H}$)
Fournit des informations détaillées sur l'environnement chimique des atomes d'hydrogène.
*   **Déplacement chimique $\delta$ (en ppm) :** Indique le degré de blindage des protons. Un groupe électroattracteur voisin (ex: halogène, oxygène) déblinde les protons voisins et augmente leur $\delta$.
*   **Courbe d'intégration :** Les paliers d'intégration sont proportionnels au nombre de protons équivalents responsables du signal.
*   **Multiplicité (Couplage spin-spin) :** Un proton ayant $n$ protons équivalents sur les carbones voisins ($\text{H}$ vicinaux, couplage $^3J$) apparaît sous forme de multiplet comportant **$n+1$ pics** (règle du n+1 multiplet).
    *   0 voisin $\to$ Singulet
    *   1 voisin $\to$ Doublet
    *   2 voisins $\to$ Triplet
    *   3 voisins $\to$ Quadruplet

---

## 6. Réactivité Organique et Mécanismes Réactionnels

### 🔄 Les Substitutions Nucléophiles ($\text{S}_{\text{N}}1$ et $\text{S}_{\text{N}}2$) sur les Dérivés Halogénés ($R-X$)
La réaction globale consiste à remplacer un groupe partant $X$ (halogénure) par un nucléophile $Nu^-$.

$$\text{R-X} + \text{Nu}^- \longrightarrow \text{R-Nu} + \text{X}^-$$

#### Mechanism Comparison $\text{S}_{\text{N}}1$ vs $\text{S}_{\text{N}}2$

| Caractéristique | Substitution Nucléophile Monomoléculaire ($\text{S}_{\text{N}}1$) | Substitution Nucléophile Bimoléculaire ($\text{S}_{\text{N}}2$) |
| :--- | :--- | :--- |
| **Mécanisme** | **En 2 étapes distinctes** :<br>1. Départ lent de $X^-$ pour former un carbocation plan $R^+$.<br>2. Attaque rapide du nucléophile $Nu^-$ sur l'une ou l'autre des deux faces du carbocation. | **En 1 seule étape concertée** :<br>Attaque dorsale simultanée du nucléophile $Nu^-$ à $180^\circ$ du groupe partant $X$, passant par un état de transition pentacoordonné. |
| **Loi de Vitesse** | Vitesse d'ordre global 1 : $v = k [R-X]$ | Vitesse d'ordre global 2 : $v = k [R-X][Nu^-]$ |
| **Stéréochimie** | Perte d'information stéréochimique. Attaque équiprobable sur le carbocation plan $\implies$ **Racémisation** (mélange $50/50$ d'énantiomères). | Réaction stéréospécifique avec **inversion de configuration absolue** (Inversion de Walden). |
| **Substrat favorisé** | Carbocation stable exigé : **Substrats tertiaires** ($3^\circ$) et secondaires stabilisés par mésomérie. | Faible encombrement stérique exigé : **Substrats primaires** ($1^\circ$) et méthyliques. |
| **Solvant** | Polaire et protique (stabilise le carbocation et le groupe partant). | Polaire et aprotique (exalte le caractère nucléophile de $Nu^-$). |

---

### 💥 Les Éliminations ($\text{E}1$ et $\text{E}2$)
La réaction consiste en l'arrachage d'un proton acide $\text{H}^+$ en $\beta$ du groupe partant $X$ pour former une liaison double (alcène).

#### 1. Mécanisme $\text{E}1$ (Monomoléculaire)
*   Se produit en deux étapes en parallèle de la $\text{S}_{\text{N}}1$ avec passage par un carbocation.
*   **Régiosélectivité :** Elle suit la **règle de Zaytsev** : l'élimination conduit majoritairement à l'alcène le plus substitué (qui est le plus stable thermodynamiquement).

#### 2. Mécanisme $\text{E}2$ (Bimoléculaire)
*   Se produit en une seule étape concertée.
*   **Stéréochimie :** Nécessite une conformation géométrique stricte du substrat où le proton $\text{H}$ éliminé et le groupe partant $X$ sont en position **anti-périplanaire** (angle dièdre de $180^\circ$).

---

### ⚡ Additions Électrophiles sur les Alcènes
La double liaison $C=C$, riche en électrons $\pi$, se comporte comme un site nucléophile et subit des attaques par des réactifs électrophiles.

#### 1. Addition d'halogénures d'hydrogène ($\text{H}-\text{X}$)
*   L'addition commence par la protonation de l'alcène pour former le carbocation le plus stable.
*   **Régiosélectivité (Règle de Markovnikov) :** L'hydrogène se fixe sur le carbone de la double liaison portant le plus grand nombre d'hydrogènes, de sorte à former le carbocation intermédiaire le plus stable (tertiaire > secondaire > primaire).

#### 2. Hydratation des alcènes (Addition de $H_2O$ en milieu acide)
*   Catalysée par $\text{H}_2\text{SO}_4$.
*   Suit également la régiochimie de Markovnikov pour former majoritairement l'alcool le plus substitué.

---

### 🍯 Estérification de Fischer et Hydrolyse/Saponification

#### 1. Estérification de Fischer
Réaction entre un acide carboxylique et un alcool conduisant à un ester et de l'eau.
$$\text{R-COOH} + \text{R'-OH} \rightleftharpoons \text{R-COOR'} + \text{H}_2\text{O}$$
*   **Caractéristiques :** Réaction réversible (limitée par l'hydrolyse inverse de l'ester), lente et athermique.
*   *Optimisation du rendement :* On peut déplacer l'équilibre vers la formation de l'ester soit en introduisant l'un des réactifs en grand excès (généralement l'alcool bon marché), soit en éliminant l'eau formée au fur et à mesure de sa synthèse (utilisation d'un appareil de Dean-Stark ou distillation de l'ester s'il est le plus volatil).
*   *Optimisation de la cinétique :* Augmentation de la température (chauffage à reflux) ou ajout d'un catalyseur acide ($\text{H}^+$).

#### 2. Saponification (Hydrolyse basique d'un ester)
Réaction entre un ester et un ion hydroxyde ($\text{OH}^-$).
$$\text{R-COOR'} + \text{OH}^- \longrightarrow \text{R-COO}^- + \text{R'-OH}$$
*   **Caractéristiques :** Réaction **totale** et rapide.
*   *Intérêt :* L'ion carboxylate obtenu ($\text{R-COO}^-$) à longue chaîne carbonée hydrophobe est un tensioactif (savon).

#### 3. Synthèse totale et rapide d'un ester
Pour obtenir un ester de manière rapide et totale sans libérer d'eau, on fait réagir un alcool avec un dérivé d'acide plus réactif :
*   Un **chlorure d'acyle** : $\text{R-COCl} + \text{R'-OH} \longrightarrow \text{R-COOR'} + \text{HCl}$
*   Un **anhydride d'acide** : $(\text{R-CO})_2\text{O} + \text{R'-OH} \longrightarrow \text{R-COOR'} + \text{R-COOH}$
