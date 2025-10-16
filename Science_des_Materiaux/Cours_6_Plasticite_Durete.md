# Science des Matériaux - Cours 6.1 & 6.2
## Résumé pour Exercices

---

## **COURS 6.1 - LIMITE D'ÉLASTICITÉ**

### 📐 Formules Clés

#### Limite d'élasticité théorique
```
σ_LJ = E/27 = 0.037E
```
*En pratique, beaucoup plus faible à cause des défauts*

#### Cisaillement
```
G = E / (2(1 + ν))
τ_xy = G·γ = G·(ΔL_x / L_0y)
```

---

### 🔩 **DURCISSEMENT DES MÉTAUX**

La limite d'élasticité totale est la **SOMME** de tous les mécanismes:

```
σ_Y = σ_C + Δσ_ss + Δσ_pr + Δσ_ec + Δσ_HP
```

#### 1️⃣ **Durcissement par solution solide**
```
Δσ_ss = K_ss · G · ε^(1/2) · X^(1/2)
```
- **ε** = différence de rayons atomiques [m]
- **G** = module de cisaillement [Pa]
- **X** = composition en atomes interstitiels [-]

#### 2️⃣ **Durcissement par précipités**
```
Δσ_pr = K_p · G·b / L
```
- **b** = norme du vecteur de Burgers [m]
- **L** = distance entre obstacles [m]

#### 3️⃣ **Durcissement par écrouissage**
```
Δσ_ec = K_e · G·b · √ρ_d
```
- **ρ_d** = densité de dislocations [m⁻²]

#### 4️⃣ **Durcissement Hall-Petch (taille de grains)**
```
Δσ_HP = K_HP / √φ_g
```
- **φ_g** = diamètre des grains [m]

---

### 🎯 **À RETENIR - Dislocations**

**Dislocation coin (⊥)**:
- b ⊥ t (vecteur de Burgers ⊥ tangente)
- Se déplace parallèlement à b
- Crée compression + tension + cisaillement

**Dislocation vis (∥)**:
- b ∥ t
- Structure hélicoïdale

**Condition de mouvement**:
```
τ_xy > τ_c = t·b / (L_1·L_2)
```
où t ≈ (1/2)·E·b²/l (tension de ligne)

---

## **COURS 6.2 - DURETÉ & USURE**

### 💎 **DURETÉ VICKERS**

```
H_V = 1.854 · F[kgForce] / d²[mm²]
    = 0.189 · F[N] / d²[mm²]
```

**Contrainte Vickers**:
```
σ_V = 1.854 · F[N] / d²[mm²] = 10·H_V
```

**Relation avec σ_y**:
```
σ_y [MPa] ≈ 3·H_V ≈ σ_V / 3
```

où d = (d₁ + d₂)/2

---

### 🔘 **DURETÉ BRINELL**

```
H_B = 0.102 · 2F[N] / (π·D·[D - √(D² - d²)]) [mm²]
```

- **D** = diamètre de la sphère [mm]
- **d** = diamètre de l'empreinte [mm]

---

### ⚙️ **USURE & FRICTION**

#### Coefficients de friction
```
μ_s = F_t / F_n    (statique, v = 0)
μ_d = F_t / F_n    (dynamique, v ≠ 0)
```

#### Taux d'usure
```
W = Volume enlevé / Distance parcourue [m²]
```

#### Taux d'usure spécifique
```
κ = W/A = k_a · p = k_a · F_n/A [-]
```

- **k_a** = coefficient d'Archard [Pa⁻¹]
- **A** = surface de contact [m²]
- **p** = pression appliquée [Pa]

#### Relation avec la dureté
```
A_C/A = p/σ_Y = p/(10·H_V)
```

**Plus H_V est grand → moins d'usure**

---

## 📊 **TABLEAU RÉCAPITULATIF - Propriétés**

| Propriété | Formule | Origine |
|-----------|---------|---------|
| **Rigidité** | σ = E·ε | Liaisons atomiques |
| **Limite élastique** | σ_y (ε=0.2% métaux, 0.5% polymères) | Mouvement dislocations/chaînes |
| **Dureté** | H_V ≈ 3σ_y | Résistance indentation |
| **Écrouissage** | n = dσ/dε | Création de dislocations |
| **Résistance** | σ_m | Contrainte max avant rupture |
| **Ductilité** | ε_R = ε_tot - σ/E | Déformation plastique |

---

## ⚡ **CONSEILS EXERCICES**

### Pour les métaux:
1. **Identifier les mécanismes actifs** (solution solide, précipités, écrouissage, Hall-Petch)
2. **Calculer chaque Δσ** séparément
3. **Sommer** pour obtenir σ_Y total
4. **Attention aux unités**: GPa ↔ MPa, nm ↔ m

### Pour la dureté:
1. **Mesurer d** avec précision (moyenne de d₁ et d₂)
2. **Convertir** H_V ↔ σ_y avec facteur 3
3. **Relier** à l'usure via k_a

### Pour l'usure:
1. **Identifier** le type (adhésive vs abrasive)
2. **Calculer p = F_n/A**
3. **Appliquer** κ = k_a·p
4. **Optimiser**: ↑ H_V ou ↓ F_n pour ↓ usure

---

## 🎓 **DIFFÉRENCES MATÉRIAUX**

| Aspect | Métaux | Polymères | Céramiques |
|--------|--------|-----------|------------|
| Plasticité | Dislocations | Glissement chaînes + crazes | Fragile (pas de plasticité) |
| Ductilité | ~10% | 50-100% | ~0% |
| T dépendance | Faible | Forte (T_g) | Faible |
| Compression vs Traction | Similaire | Similaire | σ_comp >> σ_tract |

**Polymères**: 
- Fragile si T < 0.75·T_g
- Ductile si T > 0.75·T_g

---

## 🔑 **MOTS-CLÉS EXAMEN**

- Vecteur de Burgers (b)
- Plan de glissement {111}, direction <110>
- Facteur de Schmid: τ = σ·cos φ·cos λ
- Précipité (amas nanométrique)
- Joint de grain (bloque dislocations)
- Craze (craquelure polymère)
- Rugosité (cause usure)
- Lubrification (↓ k_a)

---

**Version**: 2025 | **Source**: Cours V. Michaud, EPFL STI