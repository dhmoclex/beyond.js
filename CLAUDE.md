# beyond.js

Fork de reveal.js (Vite, TypeScript) ; la documentation de reveal.js s'applique.
Remotes : `origin` (`dhmoclex/beyond.js`) et `hakimel` (amont).

- Les ajouts du fork se listent avec `git log --no-merges hakimel/master..HEAD` : thème `dist/theme/beamer.css`,
  `plugin/highlight/monokai-{light,dark}.css`, `plugin/simplemenu/` (copié, non construit par Vite), footer,
  `beyond.html` (gabarit de départ).
- Chaque talk l'embarque en sous-module git : une modification ici n'est pas répercutée dans les talks
  sans mise à jour du sous-module par l'utilisateur.
- Les plugins reveal.js s'initialisent séquentiellement dans l'ordre du tableau `plugins`.
