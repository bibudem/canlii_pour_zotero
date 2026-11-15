# CanLII pour Zotero

## Introduction

Ce répertoire diffuse une version corrigée du convertisseur CanLII de Zotero. Un convertisseur (translator) remplit la notice Zotero à l'enregistrement d'une page Web avec le connecteur Zotero. Le convertisseur officiel ne remplit plus correctement les notices des pages de [CanLII](https://www.canlii.org).

Cette version est temporaire. Elle sert aux essais pendant l'examen des corrections par Zotero. Après la publication d'une version officielle plus récente, la mise à jour automatique de Zotero remplace ce fichier.

## Contenu du répertoire

- `CanLII.js` : le convertisseur corrigé;
- `LICENSE` : le texte de la licence GNU AGPL 3.0.

## Changements

Cette version reprend la [demande de fusion (pull request) #3678](https://github.com/zotero/translators/pull/3678) du répertoire GitHub `zotero/translators`, au commit `850ef6b`. Cette demande remplit à nouveau les champs **Tribunal**, **Date de décision** et **N° de requête** des décisions. Elle inscrit aussi le numéro de la référence neutre dans le champ **Première page**.

Changements apportés à cette base :

- 2026-11-11 — décisions sans référence neutre : référence CanLII inscrite dans le champ **Tribunal** (ex. « CanLII 17741 (QC CS) »);
- 2026-11-15 — documents de doctrine : PDF du texte intégral joint à la notice, à la place de la capture de la page.

## Installation sous Windows

Prérequis : Zotero et le connecteur Zotero, déjà installés.

1. Sur la page de ce répertoire, cliquer sur **Code**, puis sur **Download ZIP**.
2. Dans Zotero, ouvrir **Édition** › **Paramètres** › **Avancé**. Dans la section **Fichiers et dossiers**, cliquer sur **Ouvrir le répertoire de données**.
3. Fermer Zotero.
4. Ouvrir l'archive téléchargée. Copier `CanLII.js` dans le dossier `translators` du répertoire de données, en remplaçant le fichier existant.
5. Rouvrir Zotero.
6. Dans le navigateur, cliquer avec le bouton droit sur le bouton du connecteur Zotero, puis sur **Preferences**. Dans l'onglet **Advanced**, cliquer sur **Reset Translators**.

Les libellés de l'étape 6 sont ceux de la version anglaise du connecteur.

## Vérification

- Enregistrer avec le connecteur la décision [2000 CanLII 17741 (QC CS)](https://canlii.ca/t/1kg5g). Le champ **Tribunal** de la notice affiche « CanLII 17741 (QC CS) ».
- Enregistrer avec le connecteur le document de doctrine [2025 CanLIIDocs 1985](https://www.canlii.org/fr/doctrine/doc/2025CanLIIDocs1985). La notice a une seule pièce jointe : le PDF « CanLII Full Text PDF ».

## Retrait

1. Dans Zotero, ouvrir **Édition** › **Paramètres** › **Avancé**.
2. Dans la section **Fichiers et dossiers**, sous **Maintenance de la base de données**, cliquer sur **Réinitialiser les convertisseurs…**.
3. Dans le connecteur, refaire l'étape 6 de l'installation.

Zotero reprend alors la version officielle du convertisseur.

## Licence

`CanLII.js` fait partie de Zotero. Le fichier est distribué sous la licence GNU Affero General Public License, version 3 ou ultérieure. Le texte de la licence est dans le fichier `LICENSE`.
