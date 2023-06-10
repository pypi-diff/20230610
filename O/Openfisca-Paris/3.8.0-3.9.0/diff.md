# Comparing `tmp/Openfisca-Paris-3.8.0.tar.gz` & `tmp/Openfisca-Paris-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/openfisca-paris/openfisca-paris/dist/.tmp-g70uv0rm/Openfisca-Paris-3.8.0.tar", last modified: Tue Apr 25 14:39:16 2023, max compression
+gzip compressed data, was "/home/runner/work/openfisca-paris/openfisca-paris/dist/.tmp-c7yrql_i/Openfisca-Paris-3.9.0.tar", last modified: Sat Jun 10 09:54:06 2023, max compression
```

## Comparing `Openfisca-Paris-3.8.0.tar` & `Openfisca-Paris-3.9.0.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:16.000000 Openfisca-Paris-3.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    34519 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/LICENSE.AGPL.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:16.000000 Openfisca-Paris-3.8.0/Openfisca_Paris.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-25 14:39:15.000000 Openfisca-Paris-3.8.0/Openfisca_Paris.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-04-25 14:39:15.000000 Openfisca-Paris-3.8.0/Openfisca_Paris.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 14:39:15.000000 Openfisca-Paris-3.8.0/Openfisca_Paris.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-25 14:39:15.000000 Openfisca-Paris-3.8.0/Openfisca_Paris.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-25 14:39:15.000000 Openfisca-Paris-3.8.0/Openfisca_Paris.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-25 14:39:16.000000 Openfisca-Paris-3.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:16.000000 Openfisca-Paris-3.8.0/openfisca_paris/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:16.000000 Openfisca-Paris-3.8.0/openfisca_paris/familles/
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/familles/aspeh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/familles/paris_energie_familles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/familles/paris_forfait_familles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:16.000000 Openfisca-Paris-3.8.0/openfisca_paris/parameters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:16.000000 Openfisca-Paris-3.8.0/openfisca_paris/parameters/paris/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:16.000000 Openfisca-Paris-3.8.0/openfisca_paris/parameters/paris/familles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:16.000000 Openfisca-Paris-3.8.0/openfisca_paris/parameters/paris/familles/aspeh/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/parameters/paris/familles/aspeh/aide_aspeh.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/parameters/paris/familles/aspeh/plafond_aspeh.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/parameters/paris/familles/paris_energie_familles.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/parameters/paris/familles/paris_forfait_familles.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:16.000000 Openfisca-Paris-3.8.0/openfisca_paris/parameters/paris/paris_logement/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/parameters/paris/paris_logement/aide_couple_avec_enf.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/parameters/paris/paris_logement/aide_couple_ss_enf.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/parameters/paris/paris_logement/aide_pers_isol.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/parameters/paris/paris_logement/aide_pl_apd_couple.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/parameters/paris/paris_logement/aide_pl_apd_pers_isol.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/parameters/paris/paris_logement/aide_pl_fam.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/parameters/paris/paris_logement/plafond_pl.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/parameters/paris/paris_logement/plafond_pl_apd.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/parameters/paris/paris_logement/plafond_pl_avec_enf.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/parameters/paris/paris_logement/plafond_pl_fam.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/parameters/paris/paris_logement/taux_effort_min.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:16.000000 Openfisca-Paris-3.8.0/openfisca_paris/parameters/paris/paris_logement_familles/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/parameters/paris/paris_logement_familles/montant_2enf.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/parameters/paris/paris_logement_familles/montant_bas_3enf.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/parameters/paris/paris_logement_familles/montant_bas_enf_sup.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/parameters/paris/paris_logement_familles/montant_haut_3enf.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/parameters/paris/paris_logement_familles/montant_haut_enf_sup.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/parameters/paris/paris_logement_familles/plafond_2enf.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/parameters/paris/paris_logement_familles/plafond_bas_3enf.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/parameters/paris/paris_logement_familles/plafond_haut_3enf.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/parameters/paris/paris_pass.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:16.000000 Openfisca-Paris-3.8.0/openfisca_paris/parameters/paris/personnes_agees/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/parameters/paris/personnes_agees/paris_complement_sante.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/parameters/paris/personnes_agees/paris_logement.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/parameters/paris/personnes_agees/personnes_agees.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/parameters/paris/personnes_agees/psol.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:16.000000 Openfisca-Paris-3.8.0/openfisca_paris/parameters/paris/personnes_handicapees/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/parameters/paris/personnes_handicapees/paris_complement_sante.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/parameters/paris/personnes_handicapees/psol.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:16.000000 Openfisca-Paris-3.8.0/openfisca_paris/parameters/paris/plfm/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/parameters/paris/plfm/aide_1er_plafond_plfm.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/parameters/paris/plfm/aide_2eme_plafond_plfm.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/parameters/paris/plfm/deuxieme_plafond_plfm.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/parameters/paris/plfm/premier_plafond_plfm.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/parameters/paris/smic_net_mensuel.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10499 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/paris.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/paris_complement_sante.py
--rw-r--r--   0 runner    (1001) docker     (123)     9335 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/paris_logement.py
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/paris_logement_fam.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/paris_logement_fam_mono.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/paris_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/paris_solidarite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:16.000000 Openfisca-Paris-3.8.0/openfisca_paris/personnes_agees/
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/personnes_agees/paris_complement_sante.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/personnes_agees/paris_logement.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/personnes_agees/paris_pass_seniors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/personnes_agees/personnes_agees.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/personnes_agees/psol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:16.000000 Openfisca-Paris-3.8.0/openfisca_paris/personnes_handicapees/
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/personnes_handicapees/paris_complement_sante.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/personnes_handicapees/paris_pass_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/personnes_handicapees/personne_handicapee.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/openfisca_paris/personnes_handicapees/psol.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 14:39:16.000000 Openfisca-Paris-3.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-25 14:38:38.000000 Openfisca-Paris-3.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:54:06.000000 Openfisca-Paris-3.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34519 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/LICENSE.AGPL.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:54:06.000000 Openfisca-Paris-3.9.0/Openfisca_Paris.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-10 09:54:06.000000 Openfisca-Paris-3.9.0/Openfisca_Paris.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-06-10 09:54:06.000000 Openfisca-Paris-3.9.0/Openfisca_Paris.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 09:54:06.000000 Openfisca-Paris-3.9.0/Openfisca_Paris.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-10 09:54:06.000000 Openfisca-Paris-3.9.0/Openfisca_Paris.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-10 09:54:06.000000 Openfisca-Paris-3.9.0/Openfisca_Paris.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-10 09:54:06.000000 Openfisca-Paris-3.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:54:06.000000 Openfisca-Paris-3.9.0/openfisca_paris/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:54:06.000000 Openfisca-Paris-3.9.0/openfisca_paris/familles/
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/familles/aspeh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/familles/paris_energie_familles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/familles/paris_forfait_familles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:54:06.000000 Openfisca-Paris-3.9.0/openfisca_paris/parameters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:54:06.000000 Openfisca-Paris-3.9.0/openfisca_paris/parameters/paris/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:54:06.000000 Openfisca-Paris-3.9.0/openfisca_paris/parameters/paris/familles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:54:06.000000 Openfisca-Paris-3.9.0/openfisca_paris/parameters/paris/familles/aspeh/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/parameters/paris/familles/aspeh/aide_aspeh.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/parameters/paris/familles/aspeh/plafond_aspeh.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/parameters/paris/familles/paris_energie_familles.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/parameters/paris/familles/paris_forfait_familles.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:54:06.000000 Openfisca-Paris-3.9.0/openfisca_paris/parameters/paris/paris_logement/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/parameters/paris/paris_logement/aide_couple_avec_enf.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/parameters/paris/paris_logement/aide_couple_ss_enf.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/parameters/paris/paris_logement/aide_pers_isol.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/parameters/paris/paris_logement/aide_pl_apd_couple.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/parameters/paris/paris_logement/aide_pl_apd_pers_isol.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/parameters/paris/paris_logement/aide_pl_fam.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/parameters/paris/paris_logement/plafond_pl.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/parameters/paris/paris_logement/plafond_pl_apd.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/parameters/paris/paris_logement/plafond_pl_avec_enf.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/parameters/paris/paris_logement/plafond_pl_fam.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/parameters/paris/paris_logement/taux_effort_min.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:54:06.000000 Openfisca-Paris-3.9.0/openfisca_paris/parameters/paris/paris_logement_familles/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/parameters/paris/paris_logement_familles/montant_2enf.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/parameters/paris/paris_logement_familles/montant_bas_3enf.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/parameters/paris/paris_logement_familles/montant_bas_enf_sup.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/parameters/paris/paris_logement_familles/montant_haut_3enf.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/parameters/paris/paris_logement_familles/montant_haut_enf_sup.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/parameters/paris/paris_logement_familles/plafond_2enf.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/parameters/paris/paris_logement_familles/plafond_bas_3enf.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/parameters/paris/paris_logement_familles/plafond_haut_3enf.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/parameters/paris/paris_pass.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:54:06.000000 Openfisca-Paris-3.9.0/openfisca_paris/parameters/paris/personnes_agees/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/parameters/paris/personnes_agees/paris_complement_sante.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/parameters/paris/personnes_agees/paris_logement.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/parameters/paris/personnes_agees/personnes_agees.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/parameters/paris/personnes_agees/psol.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:54:06.000000 Openfisca-Paris-3.9.0/openfisca_paris/parameters/paris/personnes_handicapees/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/parameters/paris/personnes_handicapees/paris_complement_sante.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/parameters/paris/personnes_handicapees/psol.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:54:06.000000 Openfisca-Paris-3.9.0/openfisca_paris/parameters/paris/plfm/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/parameters/paris/plfm/aide_1er_plafond_plfm.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/parameters/paris/plfm/aide_2eme_plafond_plfm.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/parameters/paris/plfm/deuxieme_plafond_plfm.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/parameters/paris/plfm/premier_plafond_plfm.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/parameters/paris/smic_net_mensuel.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10499 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/paris.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/paris_complement_sante.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9335 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/paris_logement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/paris_logement_fam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/paris_logement_fam_mono.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/paris_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/paris_solidarite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:54:06.000000 Openfisca-Paris-3.9.0/openfisca_paris/personnes_agees/
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/personnes_agees/paris_complement_sante.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/personnes_agees/paris_logement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/personnes_agees/paris_pass_seniors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/personnes_agees/personnes_agees.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/personnes_agees/psol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:54:06.000000 Openfisca-Paris-3.9.0/openfisca_paris/personnes_handicapees/
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/personnes_handicapees/paris_complement_sante.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/personnes_handicapees/paris_pass_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/personnes_handicapees/personne_handicapee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/openfisca_paris/personnes_handicapees/psol.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 09:54:06.000000 Openfisca-Paris-3.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-10 09:53:35.000000 Openfisca-Paris-3.9.0/setup.py
```

### Comparing `Openfisca-Paris-3.8.0/LICENSE.AGPL.txt` & `Openfisca-Paris-3.9.0/LICENSE.AGPL.txt`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-3.8.0/Openfisca_Paris.egg-info/PKG-INFO` & `Openfisca-Paris-3.9.0/Openfisca_Paris.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Openfisca-Paris
-Version: 3.8.0
+Version: 3.9.0
 Summary: Plugin OpenFisca pour les aides sociales de la mairie de Paris
 Author: OpenFisca Team
 Author-email: contact@openfisca.fr
 License: http://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: benefit france paris microsimulation social tax
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `Openfisca-Paris-3.8.0/Openfisca_Paris.egg-info/SOURCES.txt` & `Openfisca-Paris-3.9.0/Openfisca_Paris.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-3.8.0/PKG-INFO` & `Openfisca-Paris-3.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Openfisca-Paris
-Version: 3.8.0
+Version: 3.9.0
 Summary: Plugin OpenFisca pour les aides sociales de la mairie de Paris
 Author: OpenFisca Team
 Author-email: contact@openfisca.fr
 License: http://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: benefit france paris microsimulation social tax
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `Openfisca-Paris-3.8.0/README.md` & `Openfisca-Paris-3.9.0/README.md`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-3.8.0/openfisca_paris/familles/aspeh.py` & `Openfisca-Paris-3.9.0/openfisca_paris/familles/aspeh.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-3.8.0/openfisca_paris/familles/paris_energie_familles.py` & `Openfisca-Paris-3.9.0/openfisca_paris/familles/paris_energie_familles.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-3.8.0/openfisca_paris/familles/paris_forfait_familles.py` & `Openfisca-Paris-3.9.0/openfisca_paris/familles/paris_forfait_familles.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-3.8.0/openfisca_paris/parameters/paris/familles/paris_energie_familles.yaml` & `Openfisca-Paris-3.9.0/openfisca_paris/parameters/paris/familles/paris_energie_familles.yaml`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-3.8.0/openfisca_paris/parameters/paris/familles/paris_forfait_familles.yaml` & `Openfisca-Paris-3.9.0/openfisca_paris/parameters/paris/familles/paris_forfait_familles.yaml`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-3.8.0/openfisca_paris/parameters/paris/personnes_agees/paris_complement_sante.yaml` & `Openfisca-Paris-3.9.0/openfisca_paris/parameters/paris/personnes_agees/paris_complement_sante.yaml`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-3.8.0/openfisca_paris/parameters/paris/personnes_agees/paris_logement.yaml` & `Openfisca-Paris-3.9.0/openfisca_paris/parameters/paris/personnes_agees/paris_logement.yaml`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-3.8.0/openfisca_paris/paris.py` & `Openfisca-Paris-3.9.0/openfisca_paris/paris.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-3.8.0/openfisca_paris/paris_complement_sante.py` & `Openfisca-Paris-3.9.0/openfisca_paris/paris_complement_sante.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-3.8.0/openfisca_paris/paris_logement.py` & `Openfisca-Paris-3.9.0/openfisca_paris/paris_logement.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-3.8.0/openfisca_paris/paris_logement_fam.py` & `Openfisca-Paris-3.9.0/openfisca_paris/paris_logement_fam.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-3.8.0/openfisca_paris/paris_logement_fam_mono.py` & `Openfisca-Paris-3.9.0/openfisca_paris/paris_logement_fam_mono.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-3.8.0/openfisca_paris/paris_pass.py` & `Openfisca-Paris-3.9.0/openfisca_paris/paris_pass.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-3.8.0/openfisca_paris/paris_solidarite.py` & `Openfisca-Paris-3.9.0/openfisca_paris/paris_solidarite.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-3.8.0/openfisca_paris/personnes_agees/paris_complement_sante.py` & `Openfisca-Paris-3.9.0/openfisca_paris/personnes_agees/paris_complement_sante.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-3.8.0/openfisca_paris/personnes_agees/paris_logement.py` & `Openfisca-Paris-3.9.0/openfisca_paris/personnes_agees/paris_logement.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-3.8.0/openfisca_paris/personnes_agees/paris_pass_seniors.py` & `Openfisca-Paris-3.9.0/openfisca_paris/personnes_agees/paris_pass_seniors.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-3.8.0/openfisca_paris/personnes_agees/personnes_agees.py` & `Openfisca-Paris-3.9.0/openfisca_paris/personnes_agees/personnes_agees.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-3.8.0/openfisca_paris/personnes_agees/psol.py` & `Openfisca-Paris-3.9.0/openfisca_paris/personnes_agees/psol.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-3.8.0/openfisca_paris/personnes_handicapees/paris_complement_sante.py` & `Openfisca-Paris-3.9.0/openfisca_paris/personnes_handicapees/paris_complement_sante.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-3.8.0/openfisca_paris/personnes_handicapees/paris_pass_access.py` & `Openfisca-Paris-3.9.0/openfisca_paris/personnes_handicapees/paris_pass_access.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-3.8.0/openfisca_paris/personnes_handicapees/personne_handicapee.py` & `Openfisca-Paris-3.9.0/openfisca_paris/personnes_handicapees/personne_handicapee.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-3.8.0/openfisca_paris/personnes_handicapees/psol.py` & `Openfisca-Paris-3.9.0/openfisca_paris/personnes_handicapees/psol.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-3.8.0/setup.py` & `Openfisca-Paris-3.9.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup, find_packages
 
 setup(
     name="Openfisca-Paris",
-    version="3.8.0",
+    version="3.9.0",
     author="OpenFisca Team",
     author_email="contact@openfisca.fr",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Operating System :: POSIX",
         "Programming Language :: Python",
@@ -19,15 +19,15 @@
     keywords="benefit france paris microsimulation social tax",
     license="http://www.fsf.org/licensing/licenses/agpl-3.0.html",
 
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'OpenFisca-Core >= 35.2.0, < 36',
-        'OpenFisca-France >= 102, < 147',
+        'OpenFisca-France >= 102, < 148',
     ],
     extras_require={
         'test': [
             'nose',
             'pytest >= 5.4.2'
         ]
     },
```

