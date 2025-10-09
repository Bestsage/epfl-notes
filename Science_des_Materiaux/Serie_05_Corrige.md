# Corrigé Série 5 - Matériaux: de la chimie aux propriétés

**Propédeutique - Automne 2025**  
**Professeur:** V. Michaud - IMX  
**Sujet:** Structure des matériaux, élasticité

---

## Exercice 1: Vrai ou Faux?

### a) Un atome interstitiel est un atome qui peut venir se mettre à la place d'un atome existant dans la structure cristalline.
**FAUX** ❌

**Explication:** Un atome interstitiel ne remplace pas un atome existant. Il s'insère dans les espaces vides (sites interstitiels) entre les atomes du réseau cristallin, comme les sites octaédriques ou tétraédriques. Un atome qui remplace un atome existant s'appelle un atome de substitution.

### b) Dans l'acier, le carbone forme le solvant et le fer forme le soluté.
**FAUX** ❌

**Explication:** C'est l'inverse ! Dans l'acier :
- **Fer (Fe)** = solvant (élément majoritaire, matrice)
- **Carbone (C)** = soluté (élément minoritaire, dissous dans la matrice)

### c) La masse molaire d'un polymère dépend du type d'atomes qui le forment, mais aussi du degré de polymérisation.
**VRAI** ✅

**Explication:** La masse molaire d'un polymère est donnée par :
M = n × M_monomère
où n est le degré de polymérisation et M_monomère dépend des atomes constitutifs.

### d) La déformation est le rapport de deux longueurs et est donc sans dimension. La contrainte quant à elle est le rapport de deux forces, et est aussi sans dimension.
**FAUX** ❌

**Explication:** 
- **Déformation ε = ΔL/L₀** → sans dimension ✅
- **Contrainte σ = F/A** (force/surface) → dimension = Pa = N/m² ❌

### e) Si le module d'Young d'un matériau est grand, cela signifie qu'il est très résistant à la rupture.
**FAUX** ❌

**Explication:** Le module d'Young (E) mesure la **rigidité** (résistance à la déformation élastique), pas la résistance à la rupture. Un matériau peut être très rigide mais fragile.

### f) Lors d'une déformation élastique linéaire, la variation de volume du matériau dépend de la valeur de la déformation et du coefficient de Poisson.
**VRAI** ✅

**Explication:** La variation relative de volume est :
ΔV/V₀ = ε(1 - 2ν)
où ε est la déformation et ν le coefficient de Poisson.

### g) Le module d'Young d'un polymère est en général très inférieur à celui d'une céramique.
**VRAI** ✅

**Explication:** Ordre de grandeur typique :
- Polymères : E ≈ 0.1 - 10 GPa
- Céramiques : E ≈ 100 - 500 GPa

### h) Un fakir de 60 kg peut tranquillement s'endormir s'il est allongé sur un lit de 1000 clous...
**Calculons :**

Force totale : F = mg = 60 × 10 = 600 N
Surface totale de contact : A = 1000 × 0.3 mm² = 1000 × 0.3 × 10⁻⁶ m² = 3 × 10⁻⁴ m²
Contrainte : σ = F/A = 600/(3 × 10⁻⁴) = 2 × 10⁶ Pa = 2 MPa

**Résistance de la peau : 2.5 MPa**
**Contrainte calculée : 2 MPa < 2.5 MPa**

**VRAI** ✅ - Le fakir peut dormir tranquillement !

---

## Exercice 2: Atomes interstitiels

**Données:**
- Structure CFC du Fe
- Rayon Fe : r_Fe = 0.127 nm
- Rayon C : r_C = 0.077 nm

### Calcul du rayon maximal dans un site octaédrique CFC

Dans une structure CFC, les sites octaédriques sont situés :
- Au centre des faces : (1/2, 0, 0), (0, 1/2, 0), (0, 0, 1/2)
- Au centre des arêtes : (1/2, 1/2, 0), etc.

**Pour un site octaédrique au centre d'une face (1/2, 0, 0) :**

La distance entre le centre du site et un atome de Fe adjacent est :
d = a/2

Où a est le paramètre de maille.

Dans la structure CFC : a = 2√2 × r_Fe = 2√2 × 0.127 = 0.359 nm

Pour que l'atome interstitiel ne déforme pas le réseau :
r_interstitiel + r_Fe ≤ a/2

**r_i,max = a/2 - r_Fe = 0.359/2 - 0.127 = 0.180 - 0.127 = 0.053 nm**

### Vérification pour le carbone :
r_C = 0.077 nm > r_i,max = 0.053 nm

**Conclusion :** Le carbone va déformer la maille cristalline du fer CFC.

### Calcul facultatif pour la structure CC :
Dans la structure CC, les sites tétraédriques sont en position (1/4, 1/4, 1/4).

**r_i,CC = 0.036 nm** (résultat donné)

---

## Exercice 3: Structure des céramiques (BaTiO₃)

### a) Réseau cristallographique :
**Cubique simple** (structure pérovskite)

### b) Motif :
Le motif contient : 1 Ba + 1 Ti + 3 O

### c) Plans cristallographiques :
- **(100)** : Plans perpendiculaires à l'axe x
- **(200)** : Plans parallèles au (100) mais avec d = a/2
- **(110)** : Plans diagonaux
- **(111)** : Plans diagonaux passant par les coins du cube

### d) Calcul du paramètre de maille :

**Données :**
- ρ = 6000 kg/m³
- M_Ti = 48 g/mol
- M_Ba = 137 g/mol  
- M_O = 16 g/mol (attention : O₂⁻, pas O₂)

**Masse molaire de BaTiO₃ :**
M = 137 + 48 + 3×16 = 233 g/mol = 0.233 kg/mol

**Nombre d'atomes par maille :**
Dans la structure pérovskite : Z = 1 (1 motif BaTiO₃ par maille)

**Formule de la densité :**
ρ = (Z × M)/(N_A × a³)

**Résolution :**
a³ = (Z × M)/(N_A × ρ) = (1 × 0.233)/(6.022 × 10²³ × 6000)
a³ = 6.45 × 10⁻²⁹ m³
**a = 4.0 × 10⁻¹⁰ m = 4 Å**

---

## Exercice 4: Le polyéthylène

**Données :**
- Masse molaire du PE : M = 150000 g/mol
- M_C = 12 g/mol, M_H = 1 g/mol
- Longueur liaison C-C : l = 0.154 nm
- Angle de liaison : θ = 109°

### a) Degré de polymérisation :

**Masse molaire du monomère éthylène (C₂H₄) :**
M_monomère = 2 × 12 + 4 × 1 = 28 g/mol

**Degré de polymérisation :**
n = M_PE / M_monomère = 150000 / 28 = **5357**

### b) Longueur de la chaîne :

**Configuration zigzag plane :**
- Nombre de liaisons C-C : n - 1 = 5356
- Projection de chaque liaison sur l'axe de la chaîne : l × cos(θ/2)

**Avec θ = 109° (angle tétraédrique) :**
θ/2 = 54.5°
cos(54.5°) ≈ 0.577

**Longueur totale :**
L = (n-1) × l × cos(θ/2) = 5356 × 0.154 × 0.577 = **1.34 μm**

---

## Exercice 5: Corde pour une poulie

**Données :**
- Diamètre : d = 4 mm → rayon r = 2 mm
- Longueur : L = 40 m
- Limite élastique : σ_max = 60 MPa
- Module d'élasticité : E = 3 GPa
- Coefficient de Poisson : ν = 0.35
- Charge : m = 100 kg → F = 1000 N
- Hauteur d'un étage : h = 3.5 m

### a) Vérification de la capacité :

**Hauteur totale (4 étages) :**
H = 4 × 3.5 = 14 m

**Longueur nécessaire (aller-retour) :**
L_nécessaire = 2 × H = 28 m < 40 m ✅

**Section de la corde :**
A = π × r² = π × (2×10⁻³)² = 1.26 × 10⁻⁵ m²

**Contrainte avec 100 kg :**
σ = F/A = 1000/(1.26 × 10⁻⁵) = 79.6 × 10⁶ Pa = **79.6 MPa**

**Comparaison :** σ = 79.6 MPa > σ_max = 60 MPa ❌

**Conclusion :** La corde ne peut PAS supporter 100 kg en sécurité !

### b) Test avec 50 kg :

**Force :** F = 50 × 10 = 500 N
**Contrainte :** σ = 500/(1.26 × 10⁻⁵) = **39.8 MPa < 60 MPa** ✅

**Déformation :**
ε = σ/E = 39.8 × 10⁶ / (3 × 10⁹) = 0.0133 = **1.33%**

**Allongement sur 35 m :**
ΔL = ε × L = 0.0133 × 35 = **0.46 m = 46 cm**

### c) Variation de diamètre (section carrée b = 3.5 mm) :

**Déformation transversale :**
ε_transverse = -ν × ε = -0.35 × 0.0133 = -0.00465

**Variation de côté :**
Δb = ε_transverse × b = -0.00465 × 3.5 = **-0.0163 mm**

### d) Variation de volume :

**Volume initial (35 m de corde) :**
V₀ = L × b² = 35 × (3.5×10⁻³)² = 4.29 × 10⁻⁴ m³

**Variation relative de volume :**
ΔV/V₀ = ε(1 - 2ν) = 0.0133 × (1 - 2×0.35) = 0.0133 × 0.3 = 0.004

**Variation de volume :**
ΔV = 0.004 × V₀ = 0.004 × 4.29 × 10⁻⁴ = **6.84 × 10⁻⁷ m³ = 684 mm³**

**Pourquoi non nulle ?** Car ν ≠ 0.5. Pour les matériaux incompressibles (ν = 0.5), la variation de volume serait nulle.

---

## Exercice 6: Calcul théorique du module d'élasticité

**Potentiel de Lennard-Jones :**
V(r) = ε₀[(r₀/r)¹² - 2(r₀/r)⁶]

**Données :**
- Réseau cubique simple : a = 2 Å
- ε₀ = 1 eV = 1.6 × 10⁻¹⁹ J
- r₀ = a (distance d'équilibre)

### a) Force entre atomes :
F(r) = -dV/dr = (12ε₀/r₀) × [(r₀/r)¹³ - (r₀/r)⁷]

### b) Contrainte :
À l'équilibre (r = r₀) :
F(r₀) = 0

La contrainte pour une petite déformation dr :
σ = F(r₀ + dr)/a² 

### c) Module d'élasticité :
E = dσ/dε|_{r₀} = (1/a) × dF/dr|_{r₀}

**Calcul de dF/dr à r₀ :**
dF/dr|_{r₀} = (12ε₀/r₀²) × [13 - 7] = 72ε₀/r₀²

### d) Résultat numérique :
E = (72ε₀)/(a³) = (72 × 1.6 × 10⁻¹⁹)/((2 × 10⁻¹⁰)³)
E = (1.15 × 10⁻¹⁷)/(8 × 10⁻³⁰) = **144 GPa**

**Comparaison avec le diagramme d'Ashby :** Cette valeur est dans l'ordre de grandeur des métaux et céramiques simples, ce qui est cohérent pour un modèle théorique basé sur les liaisons atomiques.

---

## Résumé des solutions numériques

| Exercice | Paramètre | Valeur calculée |
|----------|-----------|-----------------|
| 2 | r_i,CFC | 0.053 nm |
| 2 | r_i,CC | 0.036 nm |
| 3 | a (BaTiO₃) | 4 Å |
| 4a | n_PE | 5357 |
| 4b | L_PE | 1.34 μm |
| 5b | Allongement | 46 cm |
| 5c | Δb | -0.0159 mm |
| 5d | ΔV | 684 mm³ |
| 6 | E théorique | 144 GPa |

---

## Points clés à retenir

1. **Atomes interstitiels** : S'insèrent dans les sites vides, ne remplacent pas
2. **Solvant/soluté** : L'élément majoritaire est toujours le solvant  
3. **Module d'Young** : Mesure la rigidité, pas la résistance à rupture
4. **Coefficient de Poisson** : Détermine la variation de volume sous contrainte
5. **Structures cristallines** : Connaître les sites interstitiels caractéristiques
6. **Élasticité** : Relations contrainte-déformation fondamentales

Ce corrigé détaillé devrait vous aider à maîtriser les concepts fondamentaux de la science des matériaux !