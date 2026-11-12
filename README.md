# Kit du Bastion

Un kit pour sécuriser une borne Wi-Fi OpenWrt contre 9 attaques.

## Démarrer

```bash
cd ~/bastion
chmod +x menu.sh scripts/*.sh boss/*.sh
./menu.sh
```

Choix 5 : installer la borne
Choix 6 : allumer la borne
Choix 8 : voir ce qui va pas

## Le test final (Glitch)

```bash
sudo ./boss/glitch.sh
```

Teste 9 attaques : mots de passe faibles, SSH ouvert, Wi-Fi sans chiffrement, réseau guest pas isolé, etc.

Objectif : 9/9 repoussées et score 100/100 au bilan.

## À faire

- Mot de passe root fort
- SSH par clé (pas de mots de passe)
- Wi-Fi principal : WPA3 + clé de 12 caractères
- Wi-Fi guest complètement isolé
- HTTPS sur l'interface
- Firewall bien configuré

Chaque problème du bilan te dit exactement quoi faire.

## Besoin d'aide

Si tu casses la borne : choix 10 tu la remets en usine.
Les mots de passe sont dans `sauvegardes/` (ne pas commit).

Rôles attribués : 
- Elias Chef de guilde
- Jhamal le Rempart
- Eden le Gardien
- Noham le Passeur
