# ⚠️ Pièges Courants - Analyse 1

## Suites

### ❌ Piège 1: Somme de suites
```
❌ FAUX: (uₙ + vₙ) converge ⟹ uₙ et vₙ convergent

✅ Contre-exemple:
uₙ = n, vₙ = -n
(uₙ + vₙ) = 0 converge, mais uₙ et vₙ divergent
```

### ❌ Piège 2: Suite bornée
```
❌ FAUX: uₙ bornée ⟹ uₙ converge

✅ Contre-exemple:
uₙ = (-1)ⁿ est bornée mais diverge (oscille)
```

### ❌ Piège 3: Produit de suites
```
❌ FAUX: lim(uₙ·vₙ) = lim(uₙ)·lim(vₙ) toujours

✅ VRAI seulement si les deux limites existent!

Contre-exemple:
uₙ = 0, vₙ = n
lim(uₙ·vₙ) = 0 mais lim(vₙ) n'existe pas
```

### ❌ Piège 4: Inégalités strictes
```
❌ FAUX: Si uₙ < vₙ pour tout n ⟹ lim(uₙ) < lim(vₙ)

✅ On a seulement lim(uₙ) ≤ lim(vₙ)

Contre-exemple:
uₙ = 0, vₙ = 1/n
uₙ < vₙ mais lim(uₙ) = lim(vₙ) = 0
```

---

## Valeur absolue

### ❌ Piège 5: Addition
```
❌ FAUX: |a + b| = |a| + |b|

✅ VRAI: |a + b| ≤ |a| + |b| (inégalité!)

Égalité ssi a et b de même signe
```

### ❌ Piège 6: Carrés
```
❌ FAUX: |a|² = a²

✅ VRAI! |a|² = a² toujours

Mais attention:
√(a²) = |a| ≠ a en général!
```

---

## Logarithmes et exponentielles

### ❌ Piège 7: Logarithme de somme
```
❌ FAUX: ln(a + b) = ln(a) + ln(b)

✅ VRAI: ln(a·b) = ln(a) + ln(b)
```

### ❌ Piège 8: Logarithme de puissance
```
❌ FAUX: ln(aᵇ) = ln(a)ᵇ

✅ VRAI: ln(aᵇ) = b·ln(a)
```

### ❌ Piège 9: Exponentielle de somme
```
❌ FAUX: eˣ⁺ʸ = eˣ + eʸ

✅ VRAI: eˣ⁺ʸ = eˣ·eʸ
```

---

## Nombres complexes

### ❌ Piège 10: Module de somme
```
❌ FAUX: |z₁ + z₂| = |z₁| + |z₂|

✅ VRAI: |z₁ + z₂| ≤ |z₁| + |z₂|

Égalité ssi arg(z₁) = arg(z₂)
```

### ❌ Piège 11: Argument de somme
```
❌ FAUX: arg(z₁ + z₂) = arg(z₁) + arg(z₂)

✅ Faux en général! Pas de formule simple.

VRAI pour produit: arg(z₁·z₂) = arg(z₁) + arg(z₂) [2π]
```

### ❌ Piège 12: Conjugué de somme
```
✅ VRAI: (z₁ + z₂)‾ = z̄₁ + z̄₂
✅ VRAI: (z₁·z₂)‾ = z̄₁·z̄₂

Le conjugué respecte + et ×
```

---

## Fonctions

### ❌ Piège 13: Composition
```
❌ FAUX: (f ∘ g)(x) = (g ∘ f)(x)

✅ En général f ∘ g ≠ g ∘ f

Exemple:
f(x) = x², g(x) = x + 1
(f ∘ g)(x) = (x+1)² ≠ x² + 1 = (g ∘ f)(x)
```

### ❌ Piège 14: Réciproque
```
❌ FAUX: Toute fonction a une réciproque

✅ Seulement les bijections!

❌ FAUX: f⁻¹(x) = 1/f(x)

✅ f⁻¹ est la fonction réciproque, pas l'inverse!
```

### ❌ Piège 15: Injection
```
❌ FAUX: f(x₁) ≠ f(x₂) ⟹ f injective

✅ Il faut: ∀x₁ ≠ x₂, f(x₁) ≠ f(x₂)

Trouver un contre-exemple ne suffit pas!
```

---

## Supremum et infimum

### ❌ Piège 16: Maximum vs supremum
```
❌ FAUX: sup(A) ∈ A toujours

✅ sup(A) ∈ A ssi max(A) existe

Exemple:
A = ]0, 1[
sup(A) = 1 ∉ A
```

### ❌ Piège 17: Ensemble vide
```
❌ sup(∅) et inf(∅) ne sont pas définis

Par convention (en analyse avancée):
sup(∅) = -∞
inf(∅) = +∞
```

---

## Récurrence

### ❌ Piège 18: Oublier la base
```
❌ Faire seulement l'hérédité

✅ Toujours vérifier P(n₀) d'abord!
```

### ❌ Piège 19: Hypothèse de récurrence
```
❌ Ne pas écrire explicitement l'hypothèse

✅ Toujours écrire "Supposons P(n) vraie"
   puis l'utiliser clairement
```

### ❌ Piège 20: Prouver ce qu'on veut montrer
```
❌ Partir de P(n+1) et arriver à P(n)

✅ Partir de P(n) et arriver à P(n+1)
```

---

## Trigonométrie

### ❌ Piège 21: sin² + cos²
```
✅ VRAI: sin²(x) + cos²(x) = 1

❌ FAUX: sin(x)² + cos(x)² = 1
       (notation ambiguë!)

Toujours écrire sin²(x) ou (sin(x))²
```

### ❌ Piège 22: Périodes
```
✅ sin et cos: période 2π
✅ tan: période π (pas 2π!)

❌ FAUX: tan(x + 2π) = tan(x)
✅ VRAI: tan(x + π) = tan(x)
```

---

## Calculs de limites

### ❌ Piège 23: Forme indéterminée
```
Formes indéterminées:
0/0, ∞/∞, 0·∞, ∞-∞, 0⁰, 1^∞, ∞⁰

❌ Ne pas conclure directement!
✅ Il faut transformer l'expression
```

### ❌ Piège 24: ∞ n'est pas un nombre
```
❌ FAUX: ∞ + 1 = ∞ donc 1 = 0

✅ ∞ est un symbole, pas un nombre!
   On ne peut pas faire d'algèbre avec ∞
```

---

[↩️ Retour au wiki](./Home.md)