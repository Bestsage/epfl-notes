# 🎯 Théorèmes Importants - Analyse 1

## Nombres Réels

### Propriété de la borne supérieure
```
Toute partie non vide et majorée de ℝ admet un supremum dans ℝ
```

**Importance**: C'est ce qui distingue ℝ de ℚ et rend ℝ "complet".

### Propriété d'Archimède
```
∀x ∈ ℝ, ∃n ∈ ℕ : n > x
```

**Conséquence**: ℕ n'est pas majoré dans ℝ.

### Densité de ℚ dans ℝ
```
∀a, b ∈ ℝ, a < b ⟹ ∃r ∈ ℚ : a < r < b
```

**Interprétation**: Entre deux réels, on peut toujours trouver un rationnel.

---

## Suites

### Théorème de convergence monotone
```
Si (uₙ) est monotone et bornée ⟹ (uₙ) converge
```

### Théorème des gendarmes
```
Si aₙ ≤ bₙ ≤ cₙ et lim(aₙ) = lim(cₙ) = L
⟹ lim(bₙ) = L
```

### Théorème de Bolzano-Weierstrass
```
Toute suite bornée admet au moins une sous-suite convergente
```

### Critère de Cauchy
```
Dans ℝ:
(uₙ) converge ⟺ (uₙ) est de Cauchy

Définition de Cauchy:
∀ε > 0, ∃N₀ : ∀n,m ≥ N₀, |uₙ - uₘ| < ε
```

---

## Inégalités

### Inégalité de Bernoulli
```
∀x ≥ -1, ∀n ∈ ℕ: (1 + x)ⁿ ≥ 1 + nx

Égalité ssi n = 1 ou x = 0
```

### Inégalité triangulaire
```
|a + b| ≤ |a| + |b|

||a| - |b|| ≤ |a - b|
```

### Inégalité arithmético-géométrique (AM-GM)
```
Pour a, b ≥ 0:
√(ab) ≤ (a + b)/2

Égalité ssi a = b
```

### Inégalité de Cauchy-Schwarz
```
|a₁b₁ + a₂b₂ + ... + aₙbₙ| ≤ √(a₁² + ... + aₙ²)·√(b₁² + ... + bₙ²)
```

---

## Fonctions

### Théorème: Fonction strictement monotone
```
Si f: A → B est continue et strictement monotone
⟹ f est bijective de A sur Im(f)
⟹ f⁻¹ existe et est continue
```

### Théorème: Composition
```
Si f: A → B et g: B → C:

- f, g injectives ⟹ g ∘ f injective
- f, g surjectives ⟹ g ∘ f surjective
- f, g bijectives ⟹ g ∘ f bijective
  et (g ∘ f)⁻¹ = f⁻¹ ∘ g⁻¹
```

---

## Nombres Complexes

### Formule d'Euler
```
e^(iθ) = cos(θ) + i·sin(θ)
```

### Formule de De Moivre
```
(cos(θ) + i·sin(θ))ⁿ = cos(nθ) + i·sin(nθ)

Ou: (e^(iθ))ⁿ = e^(inθ)
```

### Théorème fondamental de l'algèbre
```
Tout polynôme de degré n ≥ 1 à coefficients complexes
admet exactement n racines dans ℂ (comptées avec multiplicité)
```

---

[↩️ Retour au wiki](./Home.md)