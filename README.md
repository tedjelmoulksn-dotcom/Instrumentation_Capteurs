# Capteurs et mesures — exploitation MATLAB

## Vue d'ensemble
Scripts MATLAB de tracé et d'exploitation de mesures relevées en TP de capteurs (formation 2023–2026) : sonde Pt100, thermistance CTN (seule, en pont diviseur, avec conditionnement) et capteur de déplacement LVDT.

## Objectifs
- Tracer la caractéristique de différents capteurs à partir de mesures réelles.
- Comparer réponse brute et réponse après conditionnement.
- Approcher une caractéristique par une droite (LVDT).

## Architecture
| Script | Mesures |
|---|---|
| `pt100_resistance_temperature.m` | R de la Pt100 de 107,8 Ω à 142 Ω pour 16 → 110 °C |
| `ctn_resistance_temperature.m` | R et Rd de la CTN de 15 à 85 °C |
| `ctn_pont_diviseur.m` | Tension Um du pont diviseur, 20 → 85 °C |
| `ctn_conditionnement.m` | Tensions Ur / Urd après conditionnement, 20 → 86 °C |
| `lvdt_caracteristique.m` | 6 séries Um en fonction de la position p (0 → 1), droite Um = 11,2·p − 0,8 |

## Matériel
Bancs de TP (Pt100, CTN, LVDT, multimètres). Références exactes : À documenter.

## Logiciel
MATLAB (fonctions de base `plot`).

## Implémentation
Les valeurs mesurées sont saisies en vecteurs dans chaque script puis tracées.

## Principes d'ingénierie
- Linéarité de la Pt100 vs non-linéarité exponentielle de la CTN.
- Linéarisation d'un capteur résistif par pont diviseur.
- Sensibilité et approximation linéaire d'un LVDT.

## Résultats
Courbes générées par les scripts ; figures non incluses : À documenter.

## Difficultés / limites
Un script de tracé CTN du dossier d'origine n'a pas été repris car sa syntaxe était incomplète.

## Structure
```
Capteurs_Mesures_MATLAB/
├── README.md
├── .gitignore
└── src/
```

## Exécution
Lancer chaque script dans MATLAB depuis `src/`.

## Médias
À documenter.

## Compétences
Instrumentation, capteurs de température et de déplacement, conditionnement, exploitation de mesures sous MATLAB.
