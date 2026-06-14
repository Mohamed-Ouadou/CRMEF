# Guide de Révision : Domaine de Spécialité (Physique-Chimie)
*Préparation à l'examen de sortie des Centres Régionaux des Métiers de l'Éducation et de la Formation (CRMEF) - Session 2026*

Ce guide rassemble les concepts clés, les lois fondamentales et les formules incontournables pour les épreuves de spécialité en Physique (60%) et en Chimie (40%) selon le cadre de référence.

---

## PARTIE 1 : PHYSIQUE (60% de l'épreuve | 36 points)

### FICHE 1 : Mécanique (25% | 15 points)
*   **Cinématique & Dynamique Newtonienne** :
    *   **Vecteurs position, vitesse et accélération** : $\vec{r}(t)$, $\vec{v} = \frac{d\vec{r}}{dt}$, $\vec{a} = \frac{d\vec{v}}{dt}$. En coordonnées cartésiennes et dans la base de Frenet : $\vec{a} = a_t \vec{u} + a_n \vec{n} = \frac{dv}{dt} \vec{u} + \frac{v^2}{R} \vec{n}$.
    *   **2ème Loi de Newton (Principe Fondamental de la Dynamique)** : Dans un référentiel galiléen, $\sum \vec{F}_{ext} = m \vec{a}$.
    *   **Relation Fondamentale de la Dynamique en rotation (RFD)** : Pour un solide en rotation autour d'un axe fixe $(\Delta)$ : $\sum M_{\Delta}(\vec{F}_{ext}) = J_{\Delta} \ddot{\theta}$, où $J_{\Delta}$ est le moment d'inertie et $\ddot{\theta}$ l'accélération angulaire.
*   **Énergétique** :
    *   **Énergie cinétique** : Translation : $E_c = \frac{1}{2} m v^2$. Rotation : $E_c = \frac{1}{2} J_{\Delta} \dot{\theta}^2$.
    *   **Théorème de l'énergie cinétique (TEC)** : $\Delta E_c = E_{c2} - E_{c1} = \sum W_{1\to2}(\vec{F}_{ext})$.
    *   **Énergie potentielle de pesanteur** : $E_{pp} = m g z + Cte$.
    *   **Énergie mécanique** : $E_m = E_c + E_p$. Si les forces non-conservatives (ex: frottements) ne travaillent pas, $E_m$ se conserve ($\Delta E_m = 0$).
*   **Oscillateurs Mécaniques** :
    *   *Pendule élastique (système solide-ressort)* : Équation différentielle sans frottement : $\ddot{x} + \frac{k}{m} x = 0$. Période propre : $T_0 = 2\pi \sqrt{\frac{m}{k}}$.
    *   *Pendule de torsion* : Équation différentielle : $\ddot{\theta} + \frac{C}{J_{\Delta}} \theta = 0$. Période propre : $T_0 = 2\pi \sqrt{\frac{J_{\Delta}}{C}}$.
    *   *Phénomène de Résonance* : Se produit sous l'action d'un excitateur périodique de fréquence proche de la fréquence propre de l'oscillateur (résonateur). Amplitude maximale de l'oscillation à la résonance.

### FICHE 2 : Électricité & Électronique (25% | 15 points)
*   **Régimes Transitoires (RC, RL, RLC série)** :
    *   **Circuit RC (Échelon de tension $E$)** :
        *   Charge du condensateur : $u_c(t) + RC \frac{du_c}{dt} = E \Rightarrow u_c(t) = E(1 - e^{-t/\tau})$ avec $\tau = RC$.
    *   **Circuit RL (Échelon de tension $E$)** :
        *   Établissement du courant : $u_L(t) + R i(t) = E \Rightarrow L\frac{di}{dt} + (R+r)i = E$. Constante de temps : $\tau = \frac{L}{R_{tot}}$.
    *   **Circuit RLC série (Oscillations libres)** :
        *   Équation différentielle : $\frac{d^2u_c}{dt^2} + \frac{R_{tot}}{L} \frac{du_c}{dt} + \frac{1}{LC} u_c = 0$.
        *   Régimes d'amortissement : Pseudo-périodique (faible résistance), Critique, Aperiodique (forte résistance).
*   **Électrostatique et Magnétostatique** :
    *   *Loi de Coulomb* : $\vec{F}_{1\to2} = \frac{1}{4\pi\epsilon_0} \frac{q_1 q_2}{r^2} \vec{u}_{1\to2}$.
    *   *Champ et potentiel électrostatiques* : $\vec{E} = -\vec{grad}(V)$. Pour une charge ponctuelle $q$ : $E = \frac{1}{4\pi\epsilon_0} \frac{q}{r^2}$ et $V = \frac{1}{4\pi\epsilon_0} \frac{q}{r}$.
    *   *Champ magnétique* : Crée par un courant (Loi de Biot et Savart). Pour un solénoïde infini : $B = \mu_0 n I$ (où $n = N/L$).

### FICHE 3 : Optique Géométrique (10% | 6 points)
*   **Lois de Snell-Descartes** :
    *   Réflexion : $i_1 = i'_1$.
    *   Réfraction : $n_1 \sin(i_1) = n_2 \sin(i_2)$.
*   **Lentilles Minces** :
    *   Formule de conjugaison de Descartes (origine au centre optique $O$) : $\frac{1}{\overline{OA'}} - \frac{1}{\overline{OA}} = \frac{1}{f'} = C$ (Vergence).
    *   Grandissement transversal : $\gamma = \frac{\overline{A'B'}}{\overline{AB}} = \frac{\overline{OA'}}{\overline{OA}}$.
*   **Instruments d'Optique** :
    *   *Loupe* : Instrument convergent de courte distance focale permettant de grossir un objet placé entre le foyer objet $F$ et le centre optique $O$.
    *   *Microscope* : Association d'un objectif (très convergent, donne une image intermédiaire réelle très agrandie) et d'un oculaire (joue le rôle de loupe pour observer l'image intermédiaire).
    *   *Lunette astronomique afocale* : L'image intermédiaire d'un objet situé à l'infini se forme dans le plan focal image de l'objectif et le plan focal objet de l'oculaire ($F'_1 = F_2$). Grossissement : $G = \frac{\theta'}{\theta} = \frac{f'_1}{f'_2}$.

---

## PARTIE 2 : CHIMIE (40% de l'épreuve | 24 points)

### FICHE 4 : Chimie des Solutions et Cinétique Chimique (20% | 12 points)
*   **Chimie des Solutions Aqueuses** :
    *   *Réactions Acido-basiques* : $\text{pH} = \text{p}K_a + \log\frac{[\text{A}^-]}{[\text{AH}]}$. Produit ionique de l'eau : $K_e = [\text{H}_3\text{O}^+][\text{OH}^-] = 10^{-14}$ à 25 °C.
    *   *Titrage* : À l'équivalence, les réactifs ont été introduits dans les proportions stœchiométriques : $n_i(\text{titré}) = n_E(\text{titrant}) \Rightarrow C_A V_A = C_B V_E$.
    *   *Précipitation et dissolution* : Produit de solubilité $K_s$. Un précipité apparaît si le quotient de réaction $Q_{r,i} > K_s$. Solubilité $S$ (en mol/L).
    *   *Oxydoréduction* : Équation de Nernst : $E = E^0 + \frac{0,059}{n} \log\frac{[\text{Ox}]^a}{[\text{Red}]^b}$ à 25 °C.
*   **Cinétique Chimique** :
    *   *Vitesse volumique de réaction* : $v(t) = \frac{1}{V} \frac{dx}{dt}$ (où $x$ est l'avancement).
    *   *Facteurs cinétiques* : Température, concentration initiale des réactifs, catalyseur.
    *   *Temps de demi-réaction $t_{1/2}$* : Durée au bout de laquelle l'avancement atteint la moitié de sa valeur finale ($x(t_{1/2}) = x_f / 2$).

### FICHE 5 : Chimie Organique (20% | 12 points)
*   **Structure de la Matière** :
    *   Configuration électronique des atomes (règles de Klechkowski, Pauli, Hund) : Ex: Carbone ($Z=6$) : $1s^2 2s^2 2p^2$ (4 électrons de valence).
    *   Représentations moléculaires : Formules développées, semi-développées, topologiques. Représentation de Cram, projection de Newman, représentation de Fischer.
    *   Stéréochimie : Carbone asymétrique ($C^*$), énantiomérie (images spéculaires non superposables), diastéréomérie, configurations absolues $R / S$ et géométriques $Z / E$.
*   **Méthodes d'Extraction et Identification** :
    *   Hydrodistillation, extraction par solvant (ampoule à décanter, choix du solvant basé sur la solubilité et la densité).
    *   Identification : Chromatographie sur Couche Mince (CCM) avec calcul du rapport frontal $R_f = h / H$, température de fusion (banc Kofler), spectroscopie IR (groupes caractéristiques).
*   **Réactivité Organique** :
    *   Grandes familles : Alcanes, alcènes, alcools, acides carboxyliques, esters, amines, amides.
    *   Réactions caractéristiques : Substitution (ex: nucléophile), Addition, Élimination, Estérification et Hydrolyse (réactions réversibles et limitées).
