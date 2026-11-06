# équipe-dev : une équipe d'agents pour Claude Code

Tu décris ce que tu veux construire. Claude devient **manager** : il pose quelques questions, découpe le travail, puis le confie à des agents spécialisés.

| Agent | Rôle |
|---|---|
| Développeur | écrit le code et ses tests |
| Cybersécurité | cherche les failles, chacune prouvée par un test qui échoue |
| Chasseur de bugs | cherche les cas limites et les régressions |
| Rédacteur | met le README à jour une fois la fonctionnalité finie et sécurisée |
| Git / CI | rejoue la CI en local, commit sur une branche, ne pousse qu'avec ton accord |

## Économe en tokens

- Trois niveaux : **éco** (2 agents), **standard**, **renforcé** (argent, mots de passe, données perso, prod).
- Mémoire partagée dans `EQUIPE.md` : chaque agent y écrit son rapport, le manager ne relit que la section utile.
- Les relecteurs lisent le diff, pas tout le projet. Un budget de tokens peut être imposé.

## Installation

Dans Claude Code :

```
/plugin marketplace add YanisseIsmaili/equipe-dev
/plugin install equipe-dev@equipe-dev
```

Ensuite, demande simplement « lance l'équipe pour ajouter … » ou tape `/equipe-dev`.

À voir en direct avec l'extension VS Code [Agent-Verse](https://github.com/YanisseIsmaili/agent-verse).

## Licence

MIT, par Yanisse Ismaili.
