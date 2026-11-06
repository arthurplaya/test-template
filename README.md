# Mon projet

Ce dépôt est planifié avec [TaskVibe](https://github.com/arthurplaya/taskvibe-action). Décris le projet dans une issue, et l'IA le découpe en tâches réparties dans l'équipe selon les compétences et les disponibilités de chacun. Elle crée ensuite les sub-issues, et replanifie si vous prenez du retard.

## Mise en route (5 minutes)

- [ ] **1. La clé d'IA.** Crée une clé gratuite sur [Google AI Studio](https://aistudio.google.com/apikey). Ajoute-la dans *Settings → Secrets and variables → Actions → New repository secret*, sous le nom `GEMINI_API_KEY`.
- [ ] **2. Le label.** Dans l'onglet *Actions*, choisis *TaskVibe*, puis *Run workflow*. Cette étape crée le label `vibe-plan`. Elle est nécessaire, car les labels ne sont pas copiés avec le modèle.
- [ ] **3. L'équipe.** Remplis [`.team-skills.yml`](.team-skills.yml) avec les logins GitHub, les rôles, les compétences et les disponibilités. Invite aussi chaque membre comme collaborateur (*Settings → Collaborators*) pour qu'il puisse être assigné.
- [ ] **4. C'est prêt.** *Issues → New issue → Projet* : décris le projet et sa durée, puis valide.

## Commandes

| Quand | Quoi |
|---|---|
| L'issue « Projet » est créée | Le plan proposé s'affiche en commentaire, en 1 à 3 minutes |
| Le plan te convient | Commente `/valider` : les tâches deviennent des sub-issues |
| Retard, nouvelle idée, absence… | Commente `/replan <ta consigne>`, par exemple `/replan on a pris une demi-journée de retard`, puis `/valider` |

Seuls les collaborateurs du dépôt peuvent lancer ces commandes.

Tu peux ensuite remplacer ce README par celui de ton projet.
