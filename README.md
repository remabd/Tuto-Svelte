# Tutoriel svelte

Ce repository couvre les [exercices](https://moodle-sciences-25.sorbonne-universite.fr/mod/resource/view.php?id=41857) demandés par le prof.
(sauf l'exo1 que j'ai perdu apparement oups)
Les exos sont en Typescript mais on peut travailler en JS si on préfère.

## Tester les exos

Tous les codes sont dans src.
Tous sous la forme un code pricipal App.svelte et des composants.
Pour afficher tel ou tel composant sur le server local, on change la ligne `import App from "./exo1/App.svelte";` dans le `Main.ts`

## Build & Run

Après clonage:

```
cd Tuto-Svelte
npm i
npm run dev
```

## Créer un autre projet

On a utilisé Vite pour créer le projet.
Pour ça on peut faire:

```
npm create vite@latest nom-du-projet
```
