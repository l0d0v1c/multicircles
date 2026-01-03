# Multicircles - Dessin par Epicycles de Fourier

Visualisation interactive des séries de Fourier pour dessiner des formes SVG à l'aide d'épicycles (cercles emboîtés en rotation).

## Demo

[Voir la démo en ligne](https://l0d0v1c.github.io/multicircles)

<video src="https://l0d0v1c.github.io/multicircles/epi.mp4" autoplay loop muted playsinline width="600"></video>

## Principe

Toute courbe fermée peut être décomposée en une somme de cercles en rotation (épicycles) grâce à la Transformée de Fourier Discrète (DFT). Chaque cercle a :
- Une **amplitude** (rayon)
- Une **fréquence** (vitesse de rotation)
- Une **phase** (angle initial)

En faisant tourner tous les cercles simultanément, le point final trace la forme originale.

## Fonctionnalités

- Chargement de fichiers SVG (path)
- Calcul automatique des coefficients de Fourier
- Animation en temps réel des épicycles
- Contrôle du nombre de cercles (précision du dessin)
- Contrôle de la vitesse d'animation
- Formes incluses : Chat, France

## Utilisation

1. Sélectionner une forme dans le menu déroulant
2. Ajuster le nombre de cercles (plus = plus précis)
3. Cliquer sur "Démarrer" pour lancer l'animation
4. Observer les cercles tracer progressivement la forme

## Lancer localement

```bash
python3 -m http.server 8080
```

Puis ouvrir http://localhost:8080

## Fichiers

- `index.html` - Application principale
- `cat.svg` - Contour d'un chat
- `france.svg` - Carte de France
