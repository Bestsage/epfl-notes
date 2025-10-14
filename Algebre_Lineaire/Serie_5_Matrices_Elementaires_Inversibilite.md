# 📊 Série 5 - Matrices Élémentaires et Inversibilité

**Cours :** MATH-111 Linear Algebra  
**Semestre :** Automne 2025  
**Thème principal :** Matrices inversibles, matrices élémentaires, et méthodes de calcul d'inverse

---

## 📋 Vue d'ensemble

Cette série se concentre sur les **matrices inversibles** et les **opérations élémentaires** sur les lignes, sans utiliser les déterminants. Les méthodes principales sont la réduction de lignes et les propriétés du Théorème de la Matrice Inversible.

---

## 🎯 Exercice 5.1 - Matrices Élémentaires

### Concepts clés
- **Matrices élémentaires** : matrices qui effectuent une seule opération élémentaire sur les lignes
- **Trois types d'opérations élémentaires** :
  1. **Échange de lignes** : Pᵢⱼ (permutation)
  2. **Multiplication d'une ligne par un scalaire non-nul** : Dᵢ(λ) où λ ≠ 0
  3. **Addition d'un multiple d'une ligne à une autre** : Lᵢⱼ(λ)

### Points importants
- Une matrice élémentaire doit être **inversible**
- Test pratique : multiplier la matrice par un vecteur général pour voir l'effet
- Une matrice qui multiplie une ligne par 0 n'est **pas élémentaire** (non inversible)
- Une matrice qui effectue deux opérations simultanément n'est **pas élémentaire**

### Exemples de la série
```
A = [1  0  0]     → Élémentaire (ajoute 2×ligne1 à ligne2)
    [2  1  0]
    [0  0  1]

B = [0  1]        → Élémentaire (échange ligne1 et ligne2)
    [1  0]

C = [1  1  0]     → NON élémentaire (deux opérations à la fois)
    [0  1  0]
    [0  1  1]

D = [1  0  0]     → NON élémentaire (multiplie ligne2 par 0)
    [0  0  0]
    [0  0  1]
```

---

## 🧮 Exercice 5.2 - Méthodes de Calcul d'Inverse (2×2)

### Concepts clés
- **Formule directe pour matrices 2×2** :
  ```
  [a  b]⁻¹ = 1/(ad-bc) × [ d  -b]
  [c  d]                  [-c   a]
  ```
- **Réduction de lignes** : transformer [A | I] en [I | A⁻¹]

### Points importants
- Pour les matrices 2×2, la formule directe est plus rapide
- La réduction de lignes fonctionne pour toutes les tailles
- Les deux méthodes doivent donner le **même résultat**

### Exemple
```
A = [1  2]  →  A⁻¹ = [-2   1 ]
    [3  4]           [3/2  -1/2]
```

---

## 🔢 Exercice 5.3 - Calcul d'Inverses (Matrices Diverses)

### Concepts clés
- **Réduction de lignes augmentée** : [A | I] → [I | A⁻¹]
- Opérations élémentaires systématiques
- Matrices triangulaires sont souvent plus faciles à inverser

### Stratégie de résolution
1. Former la matrice augmentée [A | I]
2. Utiliser les opérations élémentaires pour transformer A en I
3. La partie droite devient A⁻¹
4. **Vérification** : AA⁻¹ = I

### Cas particulier : Matrice triangulaire inférieure
```
[1  0  0  0]⁻¹   [1   0   0  0]
[2  1  0  0]  =  [-2  1   0  0]
[3  2  1  0]     [1  -2   1  0]
[4  3  2  1]     [0   1  -2  1]
```
Les inverses de matrices triangulaires sont aussi triangulaires !

---

## ✅ Exercice 5.4 - Détermination de l'Inversibilité

### Concepts clés
- **Matrices non carrées** : jamais inversibles
- **Test d'inversibilité** : réduction à la forme échelonnée
- Une matrice n×n est inversible ⟺ elle a **n pivots**

### Méthode
1. Réduire la matrice à la forme échelonnée (pas besoin de calculer l'inverse complet)
2. Compter les pivots
3. Si nombre de pivots = nombre de lignes → **inversible**
4. Sinon → **non inversible**

### Exemples
```
Matrice 4×4 avec 4 pivots → INVERSIBLE
Matrice 4×4 avec 3 pivots → NON INVERSIBLE
Matrice 3×4 → NON INVERSIBLE (pas carrée)
```

---

## 🔄 Exercice 5.5 - Inversion de Transformations Linéaires

### Concepts clés
- Une transformation linéaire T: ℝⁿ → ℝⁿ est inversible ⟺ sa matrice est inversible
- Pour trouver T⁻¹ : inverser la matrice correspondante
- **Vérification** : T⁻¹(T(x)) = x pour tout x

### Méthode
1. Écrire la matrice de T
2. Inverser cette matrice par réduction de lignes
3. La matrice inverse donne la formule de T⁻¹

### Exemple de la série
```
T(x) = [x₁ + 2x₂    ]
       [2x₁ - 3x₃   ]
       [x₂ + x₃     ]

Matrice: [1   2   0]
         [2   0  -3]
         [0   1   1]

T⁻¹(y) = [-3y₁ + 2y₂ + 6y₃]
         [2y₁ - y₂ - 3y₃  ]
         [-2y₁ + y₂ + 4y₃ ]
```

---

## ⚠️ Exercice 5.6 - Matrices Non Inversibles avec AB = I

### Concepts clés
- Pour des matrices **non carrées**, on peut avoir AB = Iₙ sans que A soit inversible
- Si A est m×n avec m < n, alors A n'est pas inversible (pas carrée)
- **Attention** : AB = I n'implique pas BA = I si A et B ne sont pas carrées

### Exemple clé
```
A = [1  1  0]    B = [1  0]
    [0  1  1]        [0  0]
                     [0  1]

AB = I₂  MAIS  BA ≠ I₃
```

### Leçon importante
L'inversibilité nécessite que la matrice soit **carrée** !

---

## 🔗 Exercice 5.7 - Inversibilité des Facteurs

### Concepts clés
- **Théorème** : Si AB est inversible, alors A et B sont aussi inversibles
- Utilise le **Théorème de la Matrice Inversible**

### Démonstration
Si AB est inversible, ∃C tel que (AB)C = I
- Donc A(BC) = I → A est inversible
- Donc (CA)B = I → B est inversible

### Point important
Ce théorème ne fonctionne que pour des matrices **carrées** de même taille !

---

## 🔁 Exercice 5.8 - Inverses des Matrices Élémentaires

### Concepts clés et formules
Les matrices élémentaires ont des inverses simples :

1. **Permutation** : Pᵢⱼ⁻¹ = Pᵢⱼ
   - Échanger deux fois = revenir à l'original

2. **Multiplication scalaire** : Dᵢ(λ)⁻¹ = Dᵢ(λ⁻¹)
   - Multiplier par λ puis par λ⁻¹ = identité

3. **Addition de lignes** : Lᵢⱼ(λ)⁻¹ = Lᵢⱼ(-λ)
   - Ajouter λ×ligneᵢ puis soustraire λ×ligneᵢ = identité

### Application pratique
Ces formules permettent de **défaire** rapidement des opérations élémentaires sans calcul complet.

---

## 🎲 Exercice 5.9 - Questions Vrai/Faux et QCM

### Concepts testés

#### A) Calcul efficace d'un élément de A⁻¹
- Pour trouver (A⁻¹)₂₃ (élément ligne 2, colonne 3), il suffit de calculer la **3ème colonne** de A⁻¹
- Méthode : résoudre Ax = e₃ par réduction (pas besoin de calculer toute la matrice inverse)

#### B) Propositions importantes

**VRAI :**
- Si A inversible et AB = AC → B = C (multiplier par A⁻¹ à gauche)
- Si Ax = b a au moins une solution pour tout b ∈ ℝⁿ → solution unique (équivalent à inversibilité)
- Si colonnes de A linéairement indépendantes → elles engendrent ℝⁿ (Théorème de la Matrice Inversible)
- Si colonnes de A engendrent ℝⁿ → elles sont linéairement indépendantes (TMI)
- Si colonnes linéairement indépendantes → lignes aussi (A et Aᵀ ont même inversibilité)
- Si AD = I → ∃C tel que CA = I (Théorème de la Matrice Inversible)

**FAUX :**
- A et B inversibles → A + B inversible (contre-exemple : A = I, B = -I)
- AB = AC → B = C (seulement si A inversible !)
- Toute matrice triangulaire supérieure est échelonnée (faux si zéros sur la diagonale)
- Pour matrice 2×2 : ab - cd ≠ 0 → inversible (FAUX ! il faut ad - bc ≠ 0)
- Opérations réduisant A à I réduisent aussi A⁻¹ à I (FAUX ! il faut les opérations **inverses** dans l'**ordre inverse**)

---

## 📚 Théorème de la Matrice Inversible (TMI)

### Résumé du théorème
Pour une matrice carrée A de taille n×n, les conditions suivantes sont **équivalentes** :

1. A est inversible
2. A est équivalente par lignes à Iₙ
3. A a n positions de pivot
4. Ax = 0 a seulement la solution triviale
5. Les colonnes de A sont linéairement indépendantes
6. La transformation x ↦ Ax est injective
7. Ax = b a au moins une solution pour tout b ∈ ℝⁿ
8. Les colonnes de A engendrent ℝⁿ
9. La transformation x ↦ Ax est surjective
10. Il existe une matrice C telle que CA = Iₙ
11. Il existe une matrice D telle que AD = Iₙ
12. Aᵀ est inversible

---

## 💡 Méthodes et Stratégies Récapitulatives

### Quand utiliser quelle méthode ?

| Situation | Méthode recommandée |
|-----------|---------------------|
| Matrice 2×2 | Formule directe : A⁻¹ = 1/(ad-bc) [d -b; -c a] |
| Matrices 3×3 et plus | Réduction de lignes [A \| I] → [I \| A⁻¹] |
| Vérifier inversibilité | Réduire à la forme échelonnée et compter les pivots |
| Un seul élément de A⁻¹ | Résoudre Ax = eⱼ pour la colonne j uniquement |
| Matrice triangulaire | Réduction (souvent plus simple que la formule) |

### Erreurs courantes à éviter

1. ❌ Confondre ad - bc avec ab - cd dans la formule 2×2
2. ❌ Oublier que les matrices non carrées ne sont jamais inversibles
3. ❌ Penser que AB = AC implique B = C (nécessite A inversible)
4. ❌ Croire que A + B inversible si A et B inversibles (FAUX)
5. ❌ Multiplier une ligne par 0 (pas une opération élémentaire)

### Vérifications importantes

✅ Toujours vérifier : AA⁻¹ = I  
✅ Pour transformations linéaires : vérifier T⁻¹(T(x)) = x  
✅ Compter les pivots pour l'inversibilité  
✅ S'assurer que la matrice est carrée avant de parler d'inverse

---

## 🎯 Points Clés à Retenir

1. **Matrices élémentaires** = une seule opération élémentaire, toujours inversibles
2. **Trois méthodes** pour inverser : formule 2×2, réduction de lignes, équations
3. **Inversibilité** ⟺ n pivots pour matrice n×n
4. **Théorème de la Matrice Inversible** relie 12 propriétés équivalentes
5. **Matrices non carrées** : jamais inversibles, mais peuvent avoir AB = I
6. **Inverses d'élémentaires** : formules simples (Pᵢⱼ⁻¹ = Pᵢⱼ, etc.)

---

## 📖 Ressources Complémentaires

- **Théorème de la Matrice Inversible** : référence centrale pour presque tous les exercices
- **Opérations élémentaires** : base de la réduction de lignes
- **Prochaine série** : déterminants (alternative pour vérifier l'inversibilité)

---

*Série développée par Annina Iseli - Enseignée par Andrei Negut*  
*Automne 2025 - EPFL MATH-111*
