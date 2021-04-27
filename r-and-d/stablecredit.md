---
Status: En cours de Développement
---

# StableCredit

StableCredit est un nouveau produit en cours de développement qui combine trois piliers de l'infrastructure DeFi existante :

- Création de dette synthétique (DAI, Synthetix).
- Plateforme de prêt décentralisées (Compound, AAVE).
- Fonctionnalités des Automated Market Makers, AMM (Uniswap, Sushiswap). 

## Mécanismes

StableCredit permettra aux utilisateurs de dépôser des actifs comme collatéral et d'obtention une ligne de crédit (exprimée en StableCredit USD) basée sur la valeur en dollar de l'actif déposé. Par exemple, un utilisateur peut déposer 100 LINK et obtiendra 1100$ de StableCredit USD (pour une valeur du LINK de ~11$ au moment de la rédaction de cet article). Le StableCredit USD peut être échangé contre d'autres actifs disponibles sur le protocole. 

Les cours de change entre le StableCredit USD et les actifs du protocol sont déterminés par les prix fournis par des oracles (Chainlink), ainsi que l'actuel ratio d'utilisation des actifs au sein de la plateforme. Par exemple, si les fournisseurs de liquidité (LP) ont prêté 100 DAI à la pool et que 90 DAI sont empruntés, le ration d'utilisation est de 90%. Comme les systèmes utilisant des courbes de liaison (Bonding Curves), il y aura un prime importante pour tout emprunt additionnel de DAI (le coût d'emprunt du DAI sera > \$1). Les utilisateurs pourront emprunter jusqu'à 75% de la valeur de leur collatéral (eg; ration d'utilisation de 75%).

L'AMM permettra aussi de fournir de la liquidité de façon unilaterale. Actuellement, les modèles populaires d'AMM, comme  Uniswap ou SushiSwap, requièrent des LPs qu'ils déposent les 2 actifs dans la pool. Par exemple, dans une pool de liquidité ETH-USDC, les fournisseurs de liquidités doivent déposer de l'ETH et de l'USDC avec un ration de 50/50. Cela augmente la barrière d'entrée ainsi que le capital nécessaire. L'approvisionnement unilatéral en liquidités permettra aux LP de ne déposer qu'un seul actif dans la pool de liquidités. (dans cet exemple, soit de l'ETH soit de l'USDC). La barrière à l'entrée pour devenir LP est donc grandement réduite et cela contribuera à une augmenter efficacité du capital déposée. 

## Résumé

Les utilisateurs peuvent:

- Déposer du collatéral et obtenir une ligne de crédit (StableCredit USD).
- Emprunter d'aurtes actifs avec cette ligne de crédit (similaire à Aave ou Compound).
- Échanger l'actif emprunté pour un autre actif de la pool (fonctionnalité des AMM existantes).

## Ressources pédagogiques supplémentaires et contexte (en anglais)

- [Post Medium original : Introducing StableCredit](https://medium.com/iearn/introducing-stablecredit-a-new-protocol-for-decentralized-lending-stablecoins-and-amms-7252a43ee56)
- [Animation illustrant les mécanismes du StableCredit](https://twitter.com/finematics/status/1305188626008100865)
- [Vidéo de Bankless à propos du StableCredit, avec Andre Cronje](https://www.youtube.com/watch?v=SkTuMVBLBNQ)
- [Vidéo CODEUP 38 à propos du StableCredit, avec Andre Cronje](https://www.youtube.com/watch?v=bdC3rNDChbw&feature=youtu.be&t=2002)
