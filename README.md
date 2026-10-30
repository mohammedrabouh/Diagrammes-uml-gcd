# Diagrammes d'activité UML - Plateforme GCD (USMBA)

Atelier O&M Développement Logiciel - IL

Ce dépôt contient 4 diagrammes d'activité UML qui décrivent l'**inscription** et la **réinscription** des doctorants sur la plateforme **GCD** (Gestion du Cycle Doctoral) de l'USMBA.

- Les 2 diagrammes **simples** présentent le fonctionnement général de la plateforme.
- Les 2 diagrammes **améliorés** sont plus précis et proposent un processus simplifié.

L'inscription a lieu au moment où le candidat **postule** à un sujet de thèse.

## Contenu du dépôt

| Fichier | Description |
|---|---|
| `uml_inscription_simple.png` | Inscription, vue générale |
| `uml_reinscription_simple.png` | Réinscription, vue générale |
| `uml_inscription_amelioree.png` | Inscription, version améliorée |
| `uml_reinscription_amelioree.png` | Réinscription, version améliorée |

---

## 1. Inscription simple

Le candidat crée un compte et postule à un sujet. L'encadrant examine la candidature. Si elle est retenue, le candidat dépose son dossier et l'administration remet le reçu.

## 2. Réinscription simple

Le doctorant remplit le rapport d'activités. Le directeur de thèse donne l'avis du comité de thèse, puis le doctorant charge les documents signés. Le directeur de thèse, puis la structure et le CED confirment la réinscription. Le doctorant dépose enfin son dossier.

## 3. Inscription améliorée

Après la candidature, le système notifie l'encadrant. Si la candidature est retenue, le système génère le dossier pré-rempli, le candidat le signe en ligne, puis le système vérifie que la période de dépôt est ouverte. Le candidat dépose alors son dossier, l'administration remet le reçu cacheté et délivre la carte du doctorant.

## 4. Réinscription améliorée

Le système notifie chaque acteur à chaque étape. Les signatures se font en ligne. Le directeur de structure et le directeur du CED confirment **en parallèle** (barre fork/join). Le système génère la fiche signée et le doctorant dépose un dossier en une seule copie.

---

## Notation UML utilisée

| Élément | Signification |
|---|---|
| Disque plein | Nœud initial |
| Cercle avec disque plein | Nœud final |
| Rectangle arrondi | Action |
| Losange | Décision, avec des gardes entre crochets (`[Oui]`, `[Non]`) |
| Barre noire épaisse | Fork (début du parallélisme) et join (fin du parallélisme) |
| Colonnes | Partitions (couloirs) : qui fait l'action |
| Flèche ouverte | Flux de contrôle |

Dans les diagrammes améliorés, les actions en vert sont des actions humaines et celles en violet sont automatiques (réalisées par GCD).

## Sources

Guides d'utilisation de la plateforme GCD (étudiants et professeurs), procédure d'inscription 2026-2027 et guide de réinscription 2026-2027.
