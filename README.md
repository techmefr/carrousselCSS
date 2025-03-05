# Carrousel d'Images CSS

Un carrousel d'images élégant créé uniquement avec HTML et CSS, sans dépendance JavaScript.

## 📋 À propos du projet

Ce projet démontre la création d'un carrousel d'images automatique et interactif en utilisant uniquement des technologies web fondamentales. Le carrousel alterne entre les images à intervalle régulier tout en permettant la navigation manuelle via les boutons de pagination.

## 🎯 Caractéristiques

- **Rotation automatique** des images à intervalle régulier
- **Navigation par points** permettant de sauter à une image spécifique
- **Animations fluides** utilisant les transitions CSS
- **Design responsive** s'adaptant à différentes tailles d'écran
- **Léger et performant** - sans JavaScript ni bibliothèques externes
- **Accessibilité** avec attributs alt sur les images

## 💻 Technologies utilisées

- **HTML5** - Structure sémantique
- **CSS3** - Mise en page et animations
- **Keyframes CSS** - Animation de défilement fluide
- **Sélecteurs CSS avancés** - Pour la navigation et les interactions

## 🔍 Détails techniques

### Animation automatique
Les images défilent automatiquement grâce à une animation CSS keyframes configurée pour une durée de 15 secondes et une répétition infinie. Chaque image reste visible pendant 4 secondes avant de passer à la suivante.

```css
@keyframes carouselAnimation {
  0% { transform: translateX(0%); }
  20% { transform: translateX(0%); }
  25% { transform: translateX(-100%); }
  /* et ainsi de suite */
}
```

### Navigation interactive
Les points de navigation en bas du carrousel permettent aux utilisateurs de sauter directement à une image spécifique en utilisant des liens d'ancrage HTML et le défilement CSS.

### Structure de base

```html
<div class="carousel">
  <ul class="carousel-slide">
    <li id="1" class="carousel-cell"><!-- Image 1 --></li>
    <!-- Autres images -->
  </ul>
</div>
<div class="carousel-links">
  <a href="#1">1</a>
  <!-- Autres liens -->
</div>
```

## 🚀 Comment utiliser ce carrousel

1. Clonez ce dépôt :
```bash
git clone https://github.com/techmefr/carrousselCSS.git
cd carrousselCSS
```

2. Ouvrez le fichier `index.html` dans votre navigateur

3. Pour intégrer ce carrousel dans votre propre projet :
   - Copiez les fichiers HTML et CSS
   - Ajustez les chemins des images dans le HTML
   - Personnalisez les styles selon vos besoins

## 💡 Personnalisation

Vous pouvez facilement personnaliser ce carrousel en modifiant :
- La durée de l'animation (actuellement 15s) dans `.carousel-slide`
- Le nombre d'images en ajoutant ou supprimant des éléments `<li>` dans le HTML
- Les couleurs, dimensions et autres propriétés CSS
- La vitesse de transition entre les images en ajustant les pourcentages dans `@keyframes`

## 📱 Compatibilité

Ce carrousel fonctionne sur tous les navigateurs modernes qui supportent les animations CSS :
- Chrome
- Firefox
- Safari
- Edge

## 🔮 Améliorations possibles

- Ajout de boutons "précédent" et "suivant" (déjà préparés dans le code commenté)
- Intégration d'indicateurs d'image active
- Ajout d'une option pause/lecture
- Mise en œuvre d'un design responsive plus avancé

---

✨ **Développé par [TechmeFR](https://github.com/techmefr)** - Un exemple de développement front-end créatif sans dépendances.
