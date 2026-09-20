# Hyperliquid Scanner V3.3 — GitHub Pages V25

## V25
- Suppression du glitch iPhone pendant le défilement : `visualViewport.resize` ne déclenche plus de `render()` lorsque seule la hauteur du viewport change à cause de la barre d'adresse Safari.
- Le re-render responsive est conservé lorsque la largeur réelle de mise en page change, notamment lors du passage portrait/paysage.
- Le bouton flottant Journal fonctionne maintenant comme un vrai bouton aller/retour : depuis n'importe quelle position il va au journal, puis depuis le journal il revient en haut de la page.
- L'état et le libellé du bouton sont recalculés à partir de la position réelle du panneau Journal, et non plus uniquement à partir du bas de la page.
- Version centralisée : `V25`.
