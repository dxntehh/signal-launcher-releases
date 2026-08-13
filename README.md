# Signal Launcher — téléchargements

**Ce dépôt ne contient aucun code source.** Il sert uniquement à héberger les
fichiers téléchargeables de Signal Launcher : l'installateur et le manifeste que
le launcher consulte pour se mettre à jour.

Le code du launcher n'est pas public.

## Télécharger

La dernière version se trouve dans les [Releases](../../releases/latest).
Téléchargez `Signal-Launcher-Setup.exe` — ce nom ne change jamais, quelle que soit la version.

Windows affichera « Windows a protégé votre ordinateur » : le launcher n'est pas
encore signé électroniquement. Cliquez sur **Informations complémentaires**, puis
sur **Exécuter quand même**.

Chaque Release publie l'empreinte SHA-256 de son installateur. Pour vérifier que
votre fichier est bien celui-là, intact :

```powershell
Get-FileHash "$env:USERPROFILE\Downloads\Signal.Launcher_1.0.1_x64-setup.exe" -Algorithm SHA256
```

## Mises à jour

Une fois installé, le launcher se met à jour tout seul : il propose la nouvelle
version au démarrage et l'installe si vous acceptez. Il n'y a jamais besoin de
revenir télécharger ici.

Il n'installe que ce qui est signé par la clé du projet, et refuse tout le reste.

## À propos des archives « Source code »

GitHub joint automatiquement une archive du dépôt à chaque Release. Celle-ci ne
contient que ce fichier : il n'y a rien d'autre ici.

---

Signal Launcher — Created by @Unstable Project Team
