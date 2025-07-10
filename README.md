# 🎯 Android Quiz App – Projet Tutoré ESGI

Une application Android simple de quiz à choix multiple, développée en Java avec IntelliJ IDEA (plugin Android).

## 📱 Fonctionnalités principales

- Interface d'accueil avec saisie du prénom
- Lancement du quiz via un bouton
- Affichage des questions à choix multiples (1 bonne réponse par question)
- Enregistrement des réponses de l'utilisateur
- Calcul automatique du score
- Affichage visuel des bonnes/mauvaises réponses
- Utilisation des `SharedPreferences` pour mémoriser le prénom et le score

## 🧠 Logique du quiz

- Chaque question comporte 4 choix, dont **1 seul est correct**
- L'utilisateur sélectionne ses réponses via des `CheckBox`
- Lors de la validation, chaque question est évaluée :
  - ✅ Bonne réponse cochée : +1 point
  - ❌ Mauvaise ou multiple réponses : 0 point

## 🧱 Architecture

Le projet suit une architecture **MVC simplifiée** :

```

com.monapp.quiz
├── MainActivity.java           // Écran d'accueil
├── QuizActivity.java           // Écran du quiz
├── ResultActivity.java         // Écran des résultats
├── model/
│   └── Question.java           // Représente une question et ses réponses
├── controller/
│   └── QuizManager.java        // Gère les questions, les réponses, le score
└── utils/
└── PreferencesHelper.java  // Gère les SharedPreferences

````

## 📸 Écrans (prévu)

- **Accueil** : champ prénom + bouton "Lancer le quiz"
- **Quiz** : liste scrollable de 10 questions à choix multiples
- **Résultat** : résumé du score + bonnes/mauvaises réponses colorées

## 🛠️ Technologies utilisées

- Java
- Android SDK
- XML (UI)
- ViewBinding
- SharedPreferences

## ✅ Fonctionnalités terminées

- [x] Arborescence du projet
- [x] `.gitignore` propre (IntelliJ + Android)
- [x] Configuration initiale IntelliJ avec plugin Android
- [ ] Écran d'accueil fonctionnel
- [ ] Modèle de question (`Question.java`)
- [ ] Logique de quiz (`QuizManager.java`)
- [ ] Écran de quiz avec layout dynamique
- [ ] Système de score et de feedback
- [ ] Écran de résultat avec affichage visuel

## 📂 Lancement du projet

1. Cloner le repo :
   ```bash
   git clone https://github.com/libaclibac/Quizz.git
````

2. Ouvrir dans **IntelliJ IDEA avec le plugin Android**
3. Vérifier que le SDK Android est bien configuré
4. Lancer l’émulateur ou connecter un téléphone Android
5. Lancer l’app avec ▶️

## ✍️ Auteurs

* Lili BACHELIER
* Stadiane 
