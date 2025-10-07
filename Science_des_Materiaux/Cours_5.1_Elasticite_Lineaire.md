# Cours 5.1 - Élasticité Linéaire

**Matière :** Introduction à la Science des Matériaux  
**Faculté :** STI - Génie Mécanique  
**Professeur :** V. Michaud  
**Institution :** EPFL

---

## 🎯 Objectifs du Cours

- Comprendre les propriétés d'élasticité linéaire des matériaux
- Découvrir l'origine physique de l'élasticité
- Maîtriser les cas de chargement en traction/compression
- Analyser un test de traction

---

## 📊 Test de Traction d'un Métal

### Étapes de Déformation

1. **Déformation élastique** : réversible
2. **Déformation plastique uniforme**
3. **Début de la striction**
4. **Rupture**

### Paramètres Clés

| Paramètre | Symbole | Description |
|-----------|---------|-------------|
| **Module d'élasticité** | E | Rigidité du matériau (pente initiale) |
| **Limite d'élasticité** | σ_Y = σ_{0.2} | Contrainte au seuil plastique (0.2% déformation) |
| **Résistance à la rupture** | σ_R | Contrainte maximale supportée |
| **Ductilité** | ε_R | Déformation plastique à la rupture |

---

## 🔧 Définitions Fondamentales

### Contrainte (σ)

**Contrainte en traction :**
```
σ_xx = F_x / S_x   [Pa]
```

**Contrainte en cisaillement :**
```
τ_xy = F_x / S_y   [Pa]
```

### Déformation (ε)

**Déformation en traction :**
```
ε_xx = ΔL_x / L_{0x}   [sans dimension]
```

**Déformation en cisaillement :**
```
γ = ΔL_x / L_{0y}   [sans dimension]
ε_xy = γ/2   (par convention)
```

---

## 📐 Propriétés Élastiques Linéaires

### 1. Traction/Compression Uniaxiale

**Loi de Hooke (1660) :**
```
σ_xx = E · ε_xx
```

- **E** = Module d'élasticité (module de Young) [Pa]
- La déformation est réversible dans le domaine élastique

**Coefficient de Poisson (ν) :**
```
ν = -ε_yy / ε_xx = -ε_zz / ε_xx
```

Mesure la contraction latérale lors d'une déformation uniaxiale
- **ν ≤ 0.5** (limite théorique)
- Caoutchouc : ν ≈ 0.5 (déformation sans changement de volume)

**Variation de volume :**
```
ΔV/V = (1 - 2ν) · ε_xx
```

### 2. Compression Hydrostatique

Contrainte normale constante sur toute la surface :
```
-σ_xx = -σ_yy = -σ_zz = Δp
```

**Module de compressibilité (K) :**
```
K = -Δp / (ΔV/V)
```

**Relation avec E et ν :**
```
K = E / [3(1 - 2ν)]
```

### 3. Cisaillement Simple

**Module de cisaillement (G) :**
```
σ_xy = G · 2ε_xy = G · γ
```

**Relation entre E, ν et G :**

Pour un solide isotrope, ces trois paramètres ne sont pas indépendants :
```
G = E / [2(1 + ν)]
```

---

## 🔬 Origine Physique de l'Élasticité

### Liaisons Interatomiques

| Type de liaison | Énergie (kJ/mole) |
|----------------|-------------------|
| Ionique | > 40 |
| Covalente | 300-400 |
| Métallique | > 40 |
| Faible (Van der Waals) | 1-40 (400 pour H) |

### Potentiel de Lennard-Jones

La rigidité E dépend de :
- **ε₀** : profondeur du puits de potentiel (plus grand → plus rigide)
- **r₀** : distance d'équilibre (plus petit → plus rigide)

```
E ∝ ε₀ / r₀
```

**Principe :**
- La force F = -dV/dr
- La rigidité est la pente de F près de r₀
- Plus les liaisons sont fortes et courtes, plus E est élevé

---

## 📏 Exemples de Propriétés Élastiques

| Matériau | E [GPa] | ν |
|----------|---------|---|
| Diamant | 1000 | 0.2 |
| Carbure de tungstène (WC) | 450-650 | 0.22 |
| Acier | 200 | 0.3 |
| Aluminium | 70 | 0.33 |
| Verre | 70 | 0.25 |
| Bois | 10-20 | 0.4-0.5 |
| Béton | 45 | 0.2 |
| Polyéthylène (PE) | 0.2-1.3 | 0.4 |
| Caoutchouc naturel | 0.001-0.1 | 0.5 |
| Polystyrène (PS) | 3 | 0.33 |
| Nylon | 2-4 | 0.4 |
| Titane | 116 | 0.34 |

---

## 🧪 Méthodes de Mesure

### 1. Test de Traction Quasi-Statique

- Éprouvette normalisée
- Capteurs de force et d'allongement
- Mesure directe de E et ν
- Identification de σ_Y (limite élastique)

### 2. Méthodes Dynamiques (Ondes)

**Vitesse de propagation des ondes :**

Ondes longitudinales (traction-compression) :
```
v_L = √(E/ρ)
```

Ondes transverses (cisaillement) :
```
v_T = √(G/ρ)
```

**Applications :** échographie, diapason, contrôle non destructif

---

## 🔄 Anisotropie

- **Monocristal** : E dépend de l'orientation cristalline
  - E[100] ≠ E[110]
  - Exemple : aubes de turbine monocristallines

- **Polycristal** : propriétés isotropes (moyenne de toutes les orientations)

---

## 🎈 Cas Particulier : Élastomères

- Déformation élastique grâce aux ponts moléculaires (structure en treillis)
- Déformation élastique peut atteindre **1000%**
- Au-delà : durcissement (tous les ligaments étirés)

---

## ✅ Points Clés à Retenir

1. **Module d'élasticité (E)** et **module de cisaillement (G)** définissent la rigidité
2. Les déformations engendrent une **variation de volume** (dépend de ν)
3. Ces propriétés dépendent des **liaisons inter-atomiques/moléculaires**
4. Tests **quasi-statiques** ou **dynamiques** pour mesurer E, ν, G
5. Un matériau doit être utilisé dans son **domaine élastique** pour retrouver sa forme initiale
6. Pour un solide isotrope : **E, ν et G sont liés** par des relations mathématiques

---

## 📚 Formules Essentielles à Maîtriser

```
σ_xx = E · ε_xx
ν = -ε_yy / ε_xx
ΔV/V = (1 - 2ν) · ε_xx
K = E / [3(1 - 2ν)]
G = E / [2(1 + ν)]
σ_xy = G · γ
```

---

*Résumé basé sur le Cours 5.1 - Élasticité Linéaire, Prof. V. Michaud, EPFL*