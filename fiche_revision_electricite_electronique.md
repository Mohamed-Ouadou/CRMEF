# Fiche de Révision : Électricité et Électronique
*Basée sur le Cadre Référentiel du Concours/Examen de Sortie CRMEF (Physique-Chimie)*

Cette fiche récapitule de manière structurée et rigoureuse l'ensemble des connaissances théoriques, relations mathématiques, phénomènes physiques et montages pratiques à maîtriser pour le sous-domaine **Électricité et Électronique** (qui représente **25%** de l'épreuve de spécialité de Physique, soit environ **15 points sur 60**).

---

## 📌 Sommaire
1. [Approximation des Régimes Quasi-Stationnaires (ARQS)](#1-approximation-des-régimes-quasi-stationnaires-arqs)
2. [Électrostatique et Magnétostatique](#2-électrostatique-et-magnétostatique)
3. [Propriétés Physiques et Caractérisation des Dipôles Passifs (R, L, C)](#3-propriétés-physiques-et-caractérisation-des-dipôles-passifs-r-l-c)
4. [Régimes Transitoires (RC, RL, RLC Libre)](#4-régimes-transitoires-rc-rl-rlc-libre)
5. [Régime Sinusoïdal Forcé et Résonance dans le RLC Série](#5-régime-sinusoïdal-forcé-et-résonance-dans-le-rlc-série)
6. [Électronique Analogique : L'Amplificateur Opérationnel (AOP / ALI)](#6-électronique-analogique--lamplificateur-opérationnel-aop--ali)
7. [Électronique des Télécommunications : Modulation et Démodulation d'Amplitude](#7-électronique-des-télécommunications--modulation-et-démodulation-damplitude)

---

## 1. Approximation des Régimes Quasi-Stationnaires (ARQS)

### 💡 Définition et Condition de Validité
Dans un circuit électrique de dimension spatiale caractéristique $D$, les variations temporelles des sources se propagent le long des conducteurs à la vitesse de la lumière $c$ ($c \approx 3 \times 10^8 \text{ m/s}$). Le temps de propagation est donné par $\tau_{\text{prop}} \approx \frac{D}{c}$.

L'**ARQS** est valable si le temps caractéristique de variation des signaux (la période $T$ pour un signal périodique) est très grand devant ce temps de propagation :
$$\tau_{\text{prop}} \ll T \iff \frac{D}{c} \ll T \iff D \ll \lambda$$
Où $\lambda = c \cdot T$ est la longueur d'onde associée au signal.

> [!NOTE]
> *   **À l'échelle d'un laboratoire ($D \approx 1\text{ m}$) :** L'ARQS est vérifiée pour des fréquences $f \ll 300\text{ MHz}$, ce qui englobe largement les domaines des basses et moyennes fréquences (BF et MF).
> *   **À l'échelle des lignes de transmission haute fréquence :** L'ARQS n'est plus valable. On utilise alors le modèle des lignes de transmission et les équations de propagation (ondes guidées).

### ⚡ Conséquences Physiques
1.  **Conservation instantanée de la charge :** Le courant électrique $i(t)$ possède la même valeur en tout point d'une branche non ramifiée à un instant $t$ donné. On néglige l'accumulation locale de charge dans les fils de connexion.
2.  **Lois de Kirchhoff applicables :**
    *   **Loi des nœuds :** $\sum_{k} i_k(t) = 0$
    *   **Loi des mailles :** $\sum_{k} u_k(t) = 0$
3.  **Potentiel électrique défini :** Le champ électrique reste à circulation conservative ($\vec{\nabla} \wedge \vec{E} \approx \vec{0} \implies \vec{E} = -\vec{\nabla}V$).

---

## 2. Électrostatique et Magnétostatique

### 🌌 Électrostatique
L'électrostatique étudie les champs et potentiels créés par des charges électriques immobiles.

*   **Loi de Coulomb :** Force exercée par une charge ponctuelle $q_1$ sur $q_2$ à distance $r$ :
    $$\vec{F}_{1\to 2} = \frac{q_1 q_2}{4\pi\epsilon_0 r^2} \vec{u}_{1\to 2}$$
    (Avec $\epsilon_0 \approx 8.85 \times 10^{-12} \text{ F/m}$ la permittivité du vide, et $\frac{1}{4\pi\epsilon_0} \approx 9 \times 10^9 \text{ N}\cdot\text{m}^2\cdot\text{C}^{-2}$).
*   **Champ Électrostatique $\vec{E}$ et Potentiel $V$ (charge ponctuelle $q$ en $O$) :**
    $$\vec{E}(M) = \frac{q}{4\pi\epsilon_0 r^2} \vec{u} \quad \text{et} \quad V(M) = \frac{q}{4\pi\epsilon_0 r} \quad (\text{avec } V(\infty) = 0)$$
    La relation fondamentale est : $\vec{E} = -\vec{\nabla}V$. Pour une dimension : $E = -\frac{\mathrm{d}V}{\mathrm{d}x}$.
*   **Énergie Potentielle Électrostatique $E_p$ :**
    Pour une charge d'essai $q$ placée dans un potentiel externe $V$ :
    $$E_p = qV$$
*   **Principe de Superposition :**
    Pour un système de $N$ charges ponctuelles $q_i$ situées aux distances $r_i$ du point $M$ :
    $$\vec{E}(M) = \sum_{i=1}^{N} \frac{q_i}{4\pi\epsilon_0 r_i^2}\vec{u}_i \quad \text{et} \quad V(M) = \sum_{i=1}^{N} \frac{q_i}{4\pi\epsilon_0 r_i}$$

### 🧲 Magnétostatique
La magnétostatique étudie les champs magnétiques créés par des courants stationnaires (courant continu).

*   **Loi de Biot-Savart :** Champ élémentaire $\mathrm{d}\vec{B}$ créé en $M$ par un élément de courant $I\mathrm{d}\vec{l}$ situé en $P$ :
    $$\mathrm{d}\vec{B}(M) = \frac{\mu_0}{4\pi} \frac{I\mathrm{d}\vec{l} \wedge \vec{u}_{PM}}{r^2}$$
    (Avec $\mu_0 = 4\pi \times 10^{-7} \text{ H/m}$ la perméabilité magnétique du vide).
*   **Champs magnétiques classiques (dans le vide) :**
    1.  **Fil rectiligne infini** parcouru par $I$, à distance $d$ :
        $$B = \frac{\mu_0 I}{2\pi d}$$
    2.  **Au centre d'une spire circulaire** de rayon $R$ parcourue par $I$ :
        $$B = \frac{\mu_0 I}{2R}$$
    3.  **À l'intérieur d'un solénoïde infini** comportant $n = \frac{N}{l}$ spires par unité de longueur :
        $$B = \mu_0 n I = \mu_0 \frac{N}{l} I$$

---

## 3. Propriétés Physiques et Caractérisation des Dipôles Passifs (R, L, C)

### 🧱 Résistance (Conducteur Ohmique)
Le conducteur ohmique dissipe l'énergie électrique sous forme de chaleur par effet Joule.
*   **Loi d'Ohm :** $u_R(t) = R \cdot i(t)$
*   **Puissance dissipée :** $P_J(t) = R \cdot i(2)^2 = \frac{u_R(t)^2}{R}$
*   **Expression géométrique d'une résistance cylindrique :** $R = \rho \frac{l}{S}$ (où $\rho$ est la résistivité du matériau, $l$ sa longueur et $S$ sa section).

---

### 🔋 Condensateur
Le condensateur accumule des charges électriques opposées sur ses armatures, stockant de l'énergie sous forme électrostatique.

```
       +q   | |  -q
   i  ----->| |----->
            | |
            u_C
```

*   **Relation charge-tension :** $q(t) = C \cdot u_C(t)$
*   **Relation courant-tension :** $i(t) = \frac{\mathrm{d}q}{\mathrm{d}t} = C \frac{\mathrm{d}u_C}{\mathrm{d}t}$
*   **Énergie électrostatique stockée :**
    $$E_e = \frac{1}{2} C u_C^2 = \frac{q^2}{2C}$$

#### 📐 Caractéristiques Physiques (Condensateur Plan)
Pour un condensateur constitué de deux armatures parallèles de surface en regard $S$ séparées par une distance $d$ contenant un diélectrique de permittivité relative $\epsilon_r$ :
$$C = \epsilon_r \epsilon_0 \frac{S}{d}$$
> [!TIP]
> *   La capacité $C$ augmente si $S$ augmente ou si $d$ diminue.
> *   L'introduction d'un milieu diélectrique (ex: Titanate de Baryum $\text{BaTiO}_3$ à forte permittivité relative $\epsilon_r \approx 10^3 \sim 10^4$) permet d'obtenir une forte capacité sous un très faible volume.

#### ⚠️ Phénomène de Claquage et Rigidité Diélectrique
*   Le champ électrique interne s'exprime par : $E = \frac{u_C}{d}$.
*   Chaque matériau diélectrique possède un **champ disruptif** maximum $E_{\text{dis}}$ (rigidité diélectrique) au-delà duquel le milieu devient conducteur par ionisation (arc électrique destructeur).
*   **Dangers des bulles d'air (impuretés) :** Si des bulles d'air se forment dans le diélectrique, comme $\epsilon_{r,\text{air}} = 1 \ll \epsilon_{r,\text{diélectrique}}$, le champ électrique au sein de la bulle d'air sera fortement amplifié :
    $$E_{\text{bulle}} \approx \epsilon_r E_{\text{externe}}$$
    Cela engendre des **décharges partielles** à l'intérieur de la bulle d'air bien avant que le champ global n'atteigne le seuil de rupture du matériau. Cela consume lentement le diélectrique et provoque un claquage à basse tension.

---

### 🌀 Bobine d'Inductance
La bobine s'oppose aux variations du courant qui la traverse et stocke l'énergie sous forme magnétique.

```
          L, r
   i  ----((((----->
            u_L
```

*   **Relation courant-tension :** $u_L(t) = L \frac{\mathrm{d}i}{\mathrm{d}t} + r \cdot i(t)$ (où $r$ est la résistance interne du fil).
*   **Énergie magnétique stockée :**
    $$E_m = \frac{1}{2} L i^2$$

#### 📐 Caractéristiques Physiques (Solénoïde avec Noyau)
Pour un solénoïde de longueur $l$, comportant $N$ spires de section $S = \pi R^2$, contenant un noyau ferromagnétique de perméabilité relative $\mu_r$ :
$$L = \mu_r \mu_0 \frac{N^2 S}{l}$$
*   Le champ magnétique axial à l'intérieur vaut : $B = \mu_r \mu_0 \frac{N}{l} I$.
*   **Rôle du noyau ferromagnétique ($\mu_r \gg 1$) :** Il canalise, concentre et amplifie les lignes de flux magnétique (multipliées par $\mu_r$, pouvant aller de 100 à plusieurs milliers). Cela permet de concevoir des bobines à forte inductance $L$ compactes (moins de spires et taille réduite).

---

## 4. Régimes Transitoires (RC, RL, RLC Libre)

### 📈 Circuits du Premier Ordre (RC et RL) sous Échelon de Tension
Lorsqu'un circuit contenant un seul élément stockeur d'énergie ($C$ ou $L$) subit une transition brusque de tension (échelon $E$) :

| Paramètre / Dipôle | Circuit RC | Circuit RL |
| :--- | :--- | :--- |
| **Schéma de principe** | Résistance $R$ en série avec Condensateur $C$ | Résistance $R$ en série avec Bobine $L$ |
| **Équation Différentielle** | $$RC \frac{\mathrm{d}u_C}{\mathrm{d}t} + u_C = E$$ | $$\frac{L}{R} \frac{\mathrm{d}i}{\mathrm{d}t} + i = \frac{E}{R}$$ |
| **Constante de Temps $\tau$** | $$\tau = RC$$ | $$\tau = \frac{L}{R}$$ |
| **Solution (Charge / Établissement)** | $$u_C(t) = E \left(1 - e^{-t/\tau}\right)$$ | $$i(t) = \frac{E}{R} \left(1 - e^{-t/\tau}\right)$$ |
| **Solution (Décharge / Rupture)** | $$u_C(t) = E e^{-t/\tau}$$ | $$i(t) = \frac{E}{R} e^{-t/\tau}$$ |
| **Continuité Physique** | Continuité de la tension : $u_C(0^+) = u_C(0^-)$ | Continuité du courant : $i(0^+) = i(0^-)$ |

> [!NOTE]
> Au bout de $t = 3\tau$, la réponse atteint **95%** de sa valeur finale. Au bout de $t = 5\tau$, elle atteint **99%** (considéré comme le régime permanent).

---

### 📉 Circuit RLC Série Libre
On considère un circuit fermé constitué d'un condensateur initialement chargé sous $U_0$, d'une bobine idéale $L$ et d'une résistance totale $R$.

```
       +--- C ---+
       |         |
       R         L
       |         |
       +---------+
```

#### ⚖️ Équation Différentielle
D'après la loi des mailles, la décharge obéit à :
$$u_L + u_R + u_C = 0 \implies L \frac{\mathrm{d}i}{\mathrm{d}t} + R i + u_C = 0$$
En exprimant le système en fonction du courant $i(t) = C \frac{\mathrm{d}u_C}{\mathrm{d}t}$ (en dérivant l'équation ci-dessus) :
$$\frac{\mathrm{d}^2i}{\mathrm{d}t^2} + \frac{R}{L} \frac{\mathrm{d}i}{\mathrm{d}t} + \frac{1}{LC} i = 0$$
Sous forme canonique :
$$\frac{\mathrm{d}^2i}{\mathrm{d}t^2} + 2\alpha \frac{\mathrm{d}i}{\mathrm{d}t} + \omega_0^2 i = 0$$
*   **Pulsation propre :** $\omega_0 = \frac{1}{\sqrt{LC}}$ (période propre $T_0 = \frac{2\pi}{\omega_0} = 2\pi\sqrt{LC}$)
*   **Facteur d'amortissement :** $\alpha = \frac{R}{2L}$ (constante de temps d'amortissement $\tau = \frac{1}{\alpha} = \frac{2L}{R}$)

#### 🔄 Résistance Critique $R_c$ et Types de Régimes
L'équation caractéristique associée $r^2 + 2\alpha r + \omega_0^2 = 0$ possède un discriminant réduit $\Delta' = \alpha^2 - \omega_0^2$. La limite entre les régimes oscillant et non-oscillant définit la **résistance critique** $R_c$ :
$$\alpha = \omega_0 \implies \frac{R_c}{2L} = \frac{1}{\sqrt{LC}} \implies R_c = 2 \sqrt{\frac{L}{C}}$$

On distingue trois régimes physiques selon la valeur de la résistance $R$ :

```
Régime pseudo-périodique (R < Rc)      Régime critique (R = Rc)         Régime apériodique (R > Rc)
        u_C(t)                                u_C(t)                            u_C(t)
         |                                     |                                 |
     U0 -+\                                U0 -+\                            U0 -+\
         | \   _                               |  \                              |   \
         |  \ / \                              |   \                             |    \______
---------+---X---+------> t           ---------+----+---------> t       ---------+-----------+------> t
         |  /   \_/                            |     \___                        |
         | /                                   |                                 |
```

1.  **Régime Pseudo-périodique ($R < R_c$) :**
    *   $\Delta' < 0$. Oscillations électriques sinusoïdales amorties de pseudo-pulsation $\omega = \sqrt{\omega_0^2 - \alpha^2}$.
    *   Solution : $u_C(t) = A e^{-\alpha t} \cos(\omega t + \phi)$.
    *   Pseudo-période : $T = \frac{2\pi}{\omega} = \frac{2\pi}{\sqrt{\omega_0^2 - \alpha^2}}$. Si l'amortissement est faible ($\alpha \ll \omega_0$), alors $T \approx T_0$.
2.  **Régime Critique ($R = R_c$) :**
    *   $\Delta' = 0$. Retour à l'équilibre le plus rapide possible sans aucune oscillation ni dépassement.
    *   Solution : $u_C(t) = (A \cdot t + B) e^{-\alpha t}$.
3.  **Régime Apériodique ($R > R_c$) :**
    *   $\Delta' > 0$. L'amortissement est trop fort pour permettre des oscillations. Le retour à l'équilibre est lent.
    *   Solution : $u_C(t) = A e^{r_1 t} + B e^{r_2 t}$ (avec $r_1, r_2 < 0$ les racines réelles de l'équation caractéristique).
    *   La vitesse de décharge finale est imposée par la racine la plus lente (la plus proche de 0) : $r_{\text{lent}} = -\alpha + \sqrt{\alpha^2 - \omega_0^2}$. La constante de temps globale est $\tau_{\text{lent}} = -1/r_{\text{lent}}$.

#### 🩺 Application Pratique : Le Défibrillateur Cardiaque
*   **Objectif médical :** Envoyer une impulsion brève de courant intense à travers le cœur pour resynchroniser les cellules cardiaques (fibrillation).
*   **Impératif de sécurité :** Éviter toute oscillation du courant (ce qui correspondrait à un régime pseudo-périodique). Un courant inverse (négatif) endommagerait gravement les tissus cardiaques et pourrait provoquer une nouvelle fibrillation.
*   **Solution technique :** Le circuit de décharge (condensateur du défibrillateur + inductance de l'appareil + résistance du thorax du patient) doit impérativement fonctionner en **régime apériodique** ($R_{\text{patient}} > R_c$). On choisit la capacité $C$ et l'inductance $L$ pour que le choc soit très bref (décharge à 99% en moins de $15\text{ ms}$) tout en maintenant $R_c = 2\sqrt{L/C} < R_{\text{patient}}$.

---

## 5. Régime Sinusoïdal Forcé et Résonance dans le RLC Série

Le circuit RLC série est alimenté par une tension sinusoïdale de pulsation $\omega$ : $e(t) = E_m \cos(\omega t)$.
En régime permanent établi, toutes les tensions et intensités sont sinusoïdales de même pulsation $\omega$. On utilise le formalisme complexe.

```
       --- R --- L --- C ---
      |                     |
     e(t)                  i(t)
```

### 🧮 Impédances Complexes
*   Résistance : $\underline{Z}_R = R$
*   Inductance : $\underline{Z}_L = j L \omega$
*   Condensateur : $\underline{Z}_C = \frac{1}{j C \omega} = -j \frac{1}{C \omega}$
*   Impédance équivalente du circuit RLC série :
    $$\underline{Z} = R + j\left(L\omega - \frac{1}{C\omega}\right)$$
*   Module de l'impédance :
    $$Z = |\underline{Z}| = \sqrt{R^2 + \left(L\omega - \frac{1}{C\omega}\right)^2}$$
*   Déphasage $\phi = \arg(\underline{Z})$ du courant $i(t)$ par rapport à la tension $e(t)$ ($i(t) = I_m \cos(\omega t - \phi)$) :
    $$\tan\phi = \frac{L\omega - \frac{1}{C\omega}}{R}$$

---

### 🔊 Résonance en Intensité
La résonance en intensité correspond à la valeur de pulsation pour laquelle l'amplitude $I_m$ (ou la valeur efficace $I$) du courant est maximale.

*   Comme $I_m(\omega) = \frac{E_m}{Z(\omega)}$, $I_m$ est maximal lorsque $Z(\omega)$ est minimal.
*   Le minimum de $Z$ a lieu lorsque la partie imaginaire s'annule :
    $$L\omega_0 - \frac{1}{C\omega_0} = 0 \implies \omega_0 = \frac{1}{\sqrt{LC}}$$
*   **À la résonance ($\omega = \omega_0$) :**
    *   L'impédance est purement réelle et minimale : $Z(\omega_0) = R$.
    *   Le courant efficace est maximal : $I_0 = \frac{E}{R}$.
    *   Le déphasage s'annule : $\phi = 0$ (le courant et la tension sont en phase).

#### 🎚️ Facteur de Qualité $Q$
Le facteur de qualité mesure la sélectivité du circuit à la résonance (la finesse de la courbe de résonance) :
$$Q = \frac{L\omega_0}{R} = \frac{1}{R}\sqrt{\frac{L}{C}} = \frac{1}{C\omega_0 R}$$

#### 📉 Bande Passante et Sélectivité
La bande passante à $-3\text{ dB}$ est l'intervalle de pulsations $[\omega_1, \omega_2]$ pour lequel le courant efficace vérifie $I(\omega) \ge \frac{I_0}{\sqrt{2}}$.
*   **Largeur de la bande passante :**
    $$\Delta\omega = \omega_2 - \omega_1 = \frac{\omega_0}{Q} = \frac{R}{L}$$
*   **Sélectivité :** Plus la résistance $R$ est faible, plus le facteur de qualité $Q$ est élevé et plus la bande passante $\Delta\omega$ est étroite (le circuit est très sélectif).

---

## 6. Électronique Analogique : L'Amplificateur Opérationnel (AOP / ALI)

L'AOP est un composant actif tripôle possédant deux entrées (inverseuse $E^-$ et non-inverseuse $E^+$) et une sortie $S$.

```
           +Vcc
          +---\
  v_+ --->| \  \
          |  \  \---> v_s
  v_- --->| /  /
          +---/
           -Vcc
```

### 🎯 Modèle de l'AOP Idéal
Un AOP idéal est caractérisé par :
1.  **Courants d'entrée nuls :** $i_+ = i_- = 0$ (impédance d'entrée infinie).
2.  **Gain différentiel en boucle ouverte infini :** $A_d \to \infty$.
3.  **Résistance de sortie nulle :** $R_s = 0$.

### ⚖️ Régimes de Fonctionnement

*   **Tension différentielle d'entrée :** $\epsilon = v_+ - v_-$
*   **Tension de sortie :** $v_s$ limitée par les tensions d'alimentation : $-V_{\text{sat}} \le v_s \le +V_{\text{sat}}$ (typiquement $\pm 15\text{ V}$).

```
                             v_s
                              |  +Vsat
                              |________
                             /|
                            / |
  -------------------------+--+----------> epsilon
                         / |  |
               _________/  |  |
                 -Vsat     |  |
```

1.  **Régime Linéaire (avec rétroaction négative) :**
    *   *Condition :* Présence d'un chemin de retour reliant la sortie $S$ à l'entrée inverseuse $E^-$ (directement ou via un composant).
    *   *Propriété :* Comme $A_d \to \infty$ et $v_s$ est finie, $\epsilon = \frac{v_s}{A_d} \to 0 \implies v_+ = v_-$.
2.  **Régime de Saturation (avec rétroaction positive ou en boucle ouverte) :**
    *   *Condition :* Rétroaction sur la borne non-inverseuse $E^+$, ou absence de rétroaction.
    *   *Propriété :* La sortie ne peut prendre que deux valeurs stables :
        *   Si $\epsilon > 0 \implies v_s = +V_{\text{sat}}$
        *   Si $\epsilon < 0 \implies v_s = -V_{\text{sat}}$

---

### 🎛️ Montages Fondamentaux en Régime Linéaire ($v_+ = v_-$)

#### 1. Amplificateur Inverseur
```
           R2
      +--R_2--+
      |       |
  Ve -R1- E-  +-- Vs
         E+
          |
         GND
```
*   $v_+ = 0$
*   Loi des nœuds en $E^-$ (Théorème de Millman) :
    $$\frac{v_e}{R_1} + \frac{v_s}{R_2} = 0 \implies v_s = -\frac{R_2}{R_1} v_e$$
*   Le gain en tension est négatif : le signal est amplifié et déphasé de $180^\circ$.

#### 2. Amplificateur Non-Inverseur
```
         R2
      +-R_2-+
      |     |
  E- -R1-   +-- Vs
      |
     GND  E+ <-- Ve
```
*   $v_+ = v_e$
*   Pont diviseur de tension sur l'entrée inverseuse $E^-$ :
    $$v_- = v_s \frac{R_1}{R_1 + R_2}$$
*   Comme $v_+ = v_-$ :
    $$v_s = \left(1 + \frac{R_2}{R_1}\right) v_e$$
*   Le gain en tension est toujours supérieur ou égal à 1 et le signal n'est pas déphasé.

#### 3. Suiveur de Tension
*   Cas particulier du non-inverseur avec $R_2 = 0$ (fil direct) et $R_1 \to \infty$.
    $$v_s = v_e$$
*   **Intérêt :** Il possède une impédance d'entrée infinie et une impédance de sortie quasi nulle. Il sert d'**adaptateur d'impédances** (isolateur) pour connecter une source de faible puissance à une charge sans perturber la tension de la source.

#### 4. Intégrateur Pur
```
           C
      +---C---+
      |       |
  Ve -R-- E-  +-- Vs
         E+
          |
         GND
```
*   Le courant d'entrée vaut $i = \frac{v_e}{R}$. Ce courant traverse le condensateur :
    $$i = -C \frac{\mathrm{d}v_s}{\mathrm{d}t} \implies \frac{\mathrm{d}v_s}{\mathrm{d}t} = -\frac{v_e}{RC}$$
*   En intégrant par rapport au temps :
    $$v_s(t) = -\frac{1}{RC} \int_{0}^{t} v_e(t') \mathrm{d}t' + v_s(0)$$

---

## 7. Électronique des Télécommunications : Modulation et Démodulation d'Amplitude

### 📡 Pourquoi Moduler ?
Le signal informatif basse fréquence (BF) (ex: voix, musique, $f_s \approx 20\text{ Hz} \sim 20\text{ kHz}$) ne peut pas être transmis directement par onde radio car :
1.  **Taille de l'antenne prohibitive :** Pour une bonne réception, l'antenne doit avoir une taille comparable à la demi-longueur d'onde $\lambda/2$. Pour $f = 100\text{ Hz} \implies \lambda = 3000\text{ km} \implies L_{\text{antenne}} = 1500\text{ km}$ ! En HF ($f = 100\text{ MHz}$), $L_{\text{antenne}} \approx 1.5\text{ m}$.
2.  **Multiplexage impossible :** Si toutes les stations transmettaient directement en BF, tous les signaux se mélangeraient dans la même bande de fréquences, rendant la réception inaudible.

---

### 🌊 Modulation d'Amplitude (AM)
Elle consiste à faire varier l'amplitude d'une onde porteuse haute fréquence $p(t) = P_m \cos(2\pi F_p t)$ en fonction du signal informatif basse fréquence $s(t) = S_m \cos(2\pi f_s t)$ (avec $F_p \gg f_s$).

#### 🛠️ Réalisation Pratique (Le Multiplieur)
On utilise un composant multiplieur analogique (de constante multiplicatrice $k$) alimenté par :
*   L'onde porteuse : $p(t)$
*   Le signal informatif décalé d'une tension continue (offset) $U_0$ : $s(t) + U_0$.

```
   s(t) + U_0 ----> \¯¯¯/
                    | X | ----> u(t)  (Signal Modulé)
      p(t)   ----> /___/
```

L'expression du signal modulé en amplitude est :
$$u(t) = k \cdot [U_0 + s(t)] \cdot p(t) = k \cdot P_m \cdot U_0 \left[1 + \frac{s(t)}{U_0}\right] \cos(2\pi F_p t)$$
En posant $A = k \cdot P_m \cdot U_0$ et $m = \frac{S_m}{U_0}$ (le **taux de modulation**) :
$$u(t) = A [1 + m \cos(2\pi f_s t)] \cos(2\pi F_p t)$$

#### 📈 Qualité de la Modulation (Éviter la Surmodulation)
Le taux de modulation s'exprime également à partir de l'enveloppe du signal visualisé à l'oscilloscope :
$$m = \frac{U_{\text{max}} - U_{\text{min}}}{U_{\text{max}} + U_{\text{min}}}$$

```
   Bonne modulation (m < 1)                  Surmodulation (m > 1)
         u(t)                                      u(t)
          |    _ _                                  |    _ _
        +-+\  /   \  /+-+                         +-+\  /   \  /+-+
        | \ \/     \/ / |                         | \ \/     \/ / |
--------+--X-------X--+----> t            --------+-/-\-------/-\-+----> t
        | / /\     /\ \ |                         |/   \_____/   \|  <-- Phase inversée
        +-+/  \___/  \+-+                         +-+\  /   \  /+-+
```

*   **Si $m < 1 \iff U_0 > S_m$ :** L'enveloppe supérieure du signal modulé ne franchit jamais l'axe des abscisses. Elle reproduit fidèlement le signal informatif $s(t)$. C'est une **bonne modulation**.
*   **Si $m > 1 \iff U_0 < S_m$ :** Il y a franchissement de l'axe (inversion de phase). L'enveloppe ne correspond plus au signal d'origine. On assiste au phénomène de **surmodulation** (le signal démodulé sera distordu et inaudible).

---

### 🔓 Démodulation d'Amplitude
La démodulation consiste à extraire le signal informatif $s(t)$ du signal modulé $u(t)$ reçu. Elle se déroule en deux étapes clés :

```
             Étape 1 : Détecteur d'enveloppe            Étape 2 : Filtre Passe-Haut
                  (Diode + Circuit RC //)                   (Circuit RC Série)
                 ___________|___________                     _______|_______
                |                       |                   |               |
   u(t) ------>|D|----+-------R--------+-----[ C_l ]--------+------ Vs(t)
   (Modulé)     ¯     |       |         |                   |
                     [C]     [Ru]      Vs1                 [R_l]
                      |       |         |                   |
   -------------------+-------+---------+-------------------+--------------- (GND)
```

#### 1️⃣ Étape 1 : Détection d'enveloppe (Redressement + Filtrage Passe-bas)
*   **La diode** redresse le signal en éliminant les alternances négatives.
*   **Le filtre RC parallèle** se charge rapidement durant les pics de tension et se décharge lentement à travers la résistance $R$ quand la diode est bloquée.
*   **Condition cruciale sur la constante de temps $\tau = RC$ :**
    $$\frac{1}{F_p} \ll RC \ll \frac{1}{f_s} \iff T_p \ll \tau \ll T_s$$
    *   *Si $\tau$ est trop petit ($\tau \approx T_p$) :* Le condensateur se décharge trop vite entre deux oscillations de la porteuse. Le signal de sortie oscille fortement à la fréquence de la porteuse (mauvais filtrage).
    *   *Si $\tau$ est trop grand ($\tau \ge T_s$) :* Le condensateur se décharge trop lentement. La tension ne peut pas suivre les variations descendantes de l'enveloppe du signal informatif (phénomène de "biseautage").

#### 2️⃣ Étape 2 : Élimination de la composante continue
Le signal obtenu après le détecteur d'enveloppe contient encore la composante de décalage continu $U_0$ ($v_{s1}(t) \approx k' [U_0 + s(t)]$).
*   On utilise un **filtre passe-haut passif RC série** (composé d'un condensateur de liaison $C_l$ en série et d'une résistance $R_l$ en parallèle).
*   Ce filtre bloque le courant continu ($f = 0$) et laisse passer les composantes basse fréquence du signal utile $s(t)$.
*   On récupère ainsi le signal informatif purifié en sortie : $v_s(t) \propto s(t)$.
