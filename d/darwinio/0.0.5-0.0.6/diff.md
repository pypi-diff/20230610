# Comparing `tmp/darwinio-0.0.5.tar.gz` & `tmp/darwinio-0.0.6.tar.gz`

## Comparing `darwinio-0.0.5.tar` & `darwinio-0.0.6.tar`

### file list

```diff
@@ -1,43 +1,45 @@
--rwxr-xr-x   0        0        0     1873 2020-02-02 00:00:00.000000 darwinio-0.0.5/CONTRIBUTING.md
--rwxr-xr-x   0        0        0       65 2020-02-02 00:00:00.000000 darwinio-0.0.5/requirements.txt
--rwxr-xr-x   0        0        0     5915 2020-02-02 00:00:00.000000 darwinio-0.0.5/documentation/characteristics.ods
--rwxr-xr-x   0        0        0      814 2020-02-02 00:00:00.000000 darwinio-0.0.5/documentation/earlystages.md
--rwxr-xr-x   0        0        0     2057 2020-02-02 00:00:00.000000 darwinio-0.0.5/documentation/implementation.md
--rwxr-xr-x   0        0        0     3062 2020-02-02 00:00:00.000000 darwinio-0.0.5/documentation/graphical_interface/empty_window.png
--rwxr-xr-x   0        0        0    11317 2020-02-02 00:00:00.000000 darwinio-0.0.5/documentation/graphical_interface/main_game.png
--rwxr-xr-x   0        0        0     7816 2020-02-02 00:00:00.000000 darwinio-0.0.5/documentation/graphical_interface/starting_window.png
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 darwinio-0.0.5/src/darwinio/__init__.py
--rwxr-xr-x   0        0        0     3415 2020-02-02 00:00:00.000000 darwinio-0.0.5/src/darwinio/__main__.py
--rwxr-xr-x   0        0        0     5467 2020-02-02 00:00:00.000000 darwinio-0.0.5/src/darwinio/brain.py
--rwxr-xr-x   0        0        0     2313 2020-02-02 00:00:00.000000 darwinio-0.0.5/src/darwinio/constants.py
--rwxr-xr-x   0        0        0    16148 2020-02-02 00:00:00.000000 darwinio-0.0.5/src/darwinio/distribution.py
--rwxr-xr-x   0        0        0     2697 2020-02-02 00:00:00.000000 darwinio-0.0.5/src/darwinio/genome.py
--rwxr-xr-x   0        0        0    20899 2020-02-02 00:00:00.000000 darwinio-0.0.5/src/darwinio/graphical_sim.py
--rwxr-xr-x   0        0        0     4012 2020-02-02 00:00:00.000000 darwinio-0.0.5/src/darwinio/organism.py
--rwxr-xr-x   0        0        0     1483 2020-02-02 00:00:00.000000 darwinio-0.0.5/src/darwinio/text_sim.py
--rwxr-xr-x   0        0        0     3767 2020-02-02 00:00:00.000000 darwinio-0.0.5/src/darwinio/assets/art/archaebacteria_halophile.png
--rwxr-xr-x   0        0        0     3805 2020-02-02 00:00:00.000000 darwinio-0.0.5/src/darwinio/assets/art/archaebacteria_methanogen.png
--rwxr-xr-x   0        0        0     3712 2020-02-02 00:00:00.000000 darwinio-0.0.5/src/darwinio/assets/art/archaebacteria_thermoacidophile.png
--rwxr-xr-x   0        0        0     5075 2020-02-02 00:00:00.000000 darwinio-0.0.5/src/darwinio/assets/art/eubacteria_BGA.png
--rwxr-xr-x   0        0        0     4533 2020-02-02 00:00:00.000000 darwinio-0.0.5/src/darwinio/assets/art/eubacteria_mycoplasma.png
--rwxr-xr-x   0        0        0     5241 2020-02-02 00:00:00.000000 darwinio-0.0.5/src/darwinio/assets/art/eubacteroa_chemosynthetic.png
--rwxr-xr-x   0        0        0     4269 2020-02-02 00:00:00.000000 darwinio-0.0.5/src/darwinio/assets/art/fungi-ascomycetes.png
--rwxr-xr-x   0        0        0     4427 2020-02-02 00:00:00.000000 darwinio-0.0.5/src/darwinio/assets/art/fungi-basidiomycetes.png
--rwxr-xr-x   0        0        0     3117 2020-02-02 00:00:00.000000 darwinio-0.0.5/src/darwinio/assets/art/fungi-deuteromycetes.png
--rwxr-xr-x   0        0        0    11139 2020-02-02 00:00:00.000000 darwinio-0.0.5/src/darwinio/assets/art/fungi-phycomycetes.png
--rwxr-xr-x   0        0        0     4609 2020-02-02 00:00:00.000000 darwinio-0.0.5/src/darwinio/assets/art/metaphyta-algae.png
--rwxr-xr-x   0        0        0     6760 2020-02-02 00:00:00.000000 darwinio-0.0.5/src/darwinio/assets/art/metaphyta-angiospermae.png
--rwxr-xr-x   0        0        0     4285 2020-02-02 00:00:00.000000 darwinio-0.0.5/src/darwinio/assets/art/metaphyta-bryophyta.png
--rwxr-xr-x   0        0        0     6598 2020-02-02 00:00:00.000000 darwinio-0.0.5/src/darwinio/assets/art/metaphyta-gymnospermae.png
--rwxr-xr-x   0        0        0     3474 2020-02-02 00:00:00.000000 darwinio-0.0.5/src/darwinio/assets/art/metaphyta-pterdiophyta.png
--rwxr-xr-x   0        0        0     4270 2020-02-02 00:00:00.000000 darwinio-0.0.5/src/darwinio/assets/art/protista_dinoflagellate.png
--rwxr-xr-x   0        0        0     2858 2020-02-02 00:00:00.000000 darwinio-0.0.5/src/darwinio/assets/art/protista_euglena.png
--rwxr-xr-x   0        0        0     3734 2020-02-02 00:00:00.000000 darwinio-0.0.5/src/darwinio/assets/art/protista_protozoan.png
--rwxr-xr-x   0        0        0     6104 2020-02-02 00:00:00.000000 darwinio-0.0.5/src/darwinio/assets/art/protista_slimemould.png
--rwxr-xr-x   0        0        0      859 2020-02-02 00:00:00.000000 darwinio-0.0.5/src/darwinio/assets/art/theme.json
--rwxr-xr-x   0        0        0  4128852 2020-02-02 00:00:00.000000 darwinio-0.0.5/src/darwinio/assets/audio/Darwinio.mp3
--rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 darwinio-0.0.5/.gitignore
--rwxr-xr-x   0        0        0    34915 2020-02-02 00:00:00.000000 darwinio-0.0.5/LICENSE.md
--rwxr-xr-x   0        0        0     1479 2020-02-02 00:00:00.000000 darwinio-0.0.5/README.md
--rwxr-xr-x   0        0        0      804 2020-02-02 00:00:00.000000 darwinio-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 darwinio-0.0.5/PKG-INFO
+-rwxr-xr-x   0        0        0     1873 2020-02-02 00:00:00.000000 darwinio-0.0.6/CONTRIBUTING.md
+-rwxr-xr-x   0        0        0       65 2020-02-02 00:00:00.000000 darwinio-0.0.6/requirements.txt
+-rwxr-xr-x   0        0        0     5915 2020-02-02 00:00:00.000000 darwinio-0.0.6/documentation/characteristics.ods
+-rwxr-xr-x   0        0        0      814 2020-02-02 00:00:00.000000 darwinio-0.0.6/documentation/earlystages.md
+-rwxr-xr-x   0        0        0     2057 2020-02-02 00:00:00.000000 darwinio-0.0.6/documentation/implementation.md
+-rwxr-xr-x   0        0        0     3062 2020-02-02 00:00:00.000000 darwinio-0.0.6/documentation/graphical_interface/empty_window.png
+-rwxr-xr-x   0        0        0    11317 2020-02-02 00:00:00.000000 darwinio-0.0.6/documentation/graphical_interface/main_game.png
+-rwxr-xr-x   0        0        0     7816 2020-02-02 00:00:00.000000 darwinio-0.0.6/documentation/graphical_interface/starting_window.png
+-rwxr-xr-x   0        0        0    71751 2020-02-02 00:00:00.000000 darwinio-0.0.6/documentation/screenshot/main_game_play.png
+-rwxr-xr-x   0        0        0    23470 2020-02-02 00:00:00.000000 darwinio-0.0.6/documentation/screenshot/titlescreen.png
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 darwinio-0.0.6/src/darwinio/__init__.py
+-rwxr-xr-x   0        0        0     3415 2020-02-02 00:00:00.000000 darwinio-0.0.6/src/darwinio/__main__.py
+-rwxr-xr-x   0        0        0     5467 2020-02-02 00:00:00.000000 darwinio-0.0.6/src/darwinio/brain.py
+-rwxr-xr-x   0        0        0     2313 2020-02-02 00:00:00.000000 darwinio-0.0.6/src/darwinio/constants.py
+-rwxr-xr-x   0        0        0    16148 2020-02-02 00:00:00.000000 darwinio-0.0.6/src/darwinio/distribution.py
+-rwxr-xr-x   0        0        0     2697 2020-02-02 00:00:00.000000 darwinio-0.0.6/src/darwinio/genome.py
+-rwxr-xr-x   0        0        0    20899 2020-02-02 00:00:00.000000 darwinio-0.0.6/src/darwinio/graphical_sim.py
+-rwxr-xr-x   0        0        0     4012 2020-02-02 00:00:00.000000 darwinio-0.0.6/src/darwinio/organism.py
+-rwxr-xr-x   0        0        0     1483 2020-02-02 00:00:00.000000 darwinio-0.0.6/src/darwinio/text_sim.py
+-rwxr-xr-x   0        0        0     3767 2020-02-02 00:00:00.000000 darwinio-0.0.6/src/darwinio/assets/art/archaebacteria_halophile.png
+-rwxr-xr-x   0        0        0     3805 2020-02-02 00:00:00.000000 darwinio-0.0.6/src/darwinio/assets/art/archaebacteria_methanogen.png
+-rwxr-xr-x   0        0        0     3712 2020-02-02 00:00:00.000000 darwinio-0.0.6/src/darwinio/assets/art/archaebacteria_thermoacidophile.png
+-rwxr-xr-x   0        0        0     5075 2020-02-02 00:00:00.000000 darwinio-0.0.6/src/darwinio/assets/art/eubacteria_BGA.png
+-rwxr-xr-x   0        0        0     4533 2020-02-02 00:00:00.000000 darwinio-0.0.6/src/darwinio/assets/art/eubacteria_mycoplasma.png
+-rwxr-xr-x   0        0        0     5241 2020-02-02 00:00:00.000000 darwinio-0.0.6/src/darwinio/assets/art/eubacteroa_chemosynthetic.png
+-rwxr-xr-x   0        0        0     4269 2020-02-02 00:00:00.000000 darwinio-0.0.6/src/darwinio/assets/art/fungi-ascomycetes.png
+-rwxr-xr-x   0        0        0     4427 2020-02-02 00:00:00.000000 darwinio-0.0.6/src/darwinio/assets/art/fungi-basidiomycetes.png
+-rwxr-xr-x   0        0        0     3117 2020-02-02 00:00:00.000000 darwinio-0.0.6/src/darwinio/assets/art/fungi-deuteromycetes.png
+-rwxr-xr-x   0        0        0    11139 2020-02-02 00:00:00.000000 darwinio-0.0.6/src/darwinio/assets/art/fungi-phycomycetes.png
+-rwxr-xr-x   0        0        0     4609 2020-02-02 00:00:00.000000 darwinio-0.0.6/src/darwinio/assets/art/metaphyta-algae.png
+-rwxr-xr-x   0        0        0     6760 2020-02-02 00:00:00.000000 darwinio-0.0.6/src/darwinio/assets/art/metaphyta-angiospermae.png
+-rwxr-xr-x   0        0        0     4285 2020-02-02 00:00:00.000000 darwinio-0.0.6/src/darwinio/assets/art/metaphyta-bryophyta.png
+-rwxr-xr-x   0        0        0     6598 2020-02-02 00:00:00.000000 darwinio-0.0.6/src/darwinio/assets/art/metaphyta-gymnospermae.png
+-rwxr-xr-x   0        0        0     3474 2020-02-02 00:00:00.000000 darwinio-0.0.6/src/darwinio/assets/art/metaphyta-pterdiophyta.png
+-rwxr-xr-x   0        0        0     4270 2020-02-02 00:00:00.000000 darwinio-0.0.6/src/darwinio/assets/art/protista_dinoflagellate.png
+-rwxr-xr-x   0        0        0     2858 2020-02-02 00:00:00.000000 darwinio-0.0.6/src/darwinio/assets/art/protista_euglena.png
+-rwxr-xr-x   0        0        0     3734 2020-02-02 00:00:00.000000 darwinio-0.0.6/src/darwinio/assets/art/protista_protozoan.png
+-rwxr-xr-x   0        0        0     6104 2020-02-02 00:00:00.000000 darwinio-0.0.6/src/darwinio/assets/art/protista_slimemould.png
+-rwxr-xr-x   0        0        0      859 2020-02-02 00:00:00.000000 darwinio-0.0.6/src/darwinio/assets/art/theme.json
+-rwxr-xr-x   0        0        0  4128852 2020-02-02 00:00:00.000000 darwinio-0.0.6/src/darwinio/assets/audio/Darwinio.mp3
+-rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 darwinio-0.0.6/.gitignore
+-rwxr-xr-x   0        0        0    34915 2020-02-02 00:00:00.000000 darwinio-0.0.6/LICENSE.md
+-rwxr-xr-x   0        0        0     1965 2020-02-02 00:00:00.000000 darwinio-0.0.6/README.md
+-rwxr-xr-x   0        0        0      804 2020-02-02 00:00:00.000000 darwinio-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 darwinio-0.0.6/PKG-INFO
```

### Comparing `darwinio-0.0.5/CONTRIBUTING.md` & `darwinio-0.0.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.5/documentation/characteristics.ods` & `darwinio-0.0.6/documentation/characteristics.ods`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.5/documentation/earlystages.md` & `darwinio-0.0.6/documentation/earlystages.md`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.5/documentation/implementation.md` & `darwinio-0.0.6/documentation/implementation.md`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.5/documentation/graphical_interface/empty_window.png` & `darwinio-0.0.6/documentation/graphical_interface/empty_window.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.5/documentation/graphical_interface/main_game.png` & `darwinio-0.0.6/documentation/graphical_interface/main_game.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.5/documentation/graphical_interface/starting_window.png` & `darwinio-0.0.6/documentation/graphical_interface/starting_window.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.5/src/darwinio/__main__.py` & `darwinio-0.0.6/src/darwinio/__main__.py`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.5/src/darwinio/brain.py` & `darwinio-0.0.6/src/darwinio/brain.py`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.5/src/darwinio/constants.py` & `darwinio-0.0.6/src/darwinio/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-TITLE_ACSII_ART = """
+TITLE_ASCII_ART = """
  ______   _______  _______          _________ _       _________ _______ 
 (  __  \ (  ___  )(  ____ )|\     /|\__   __/( (    /|\__   __/(  ___  )
 | (  \  )| (   ) || (    )|| )   ( |   ) (   |  \  ( |   ) (   | (   ) |
 | |   ) || (___) || (____)|| | _ | |   | |   |   \ | |   | |   | |   | |
 | |   | ||  ___  ||     __)| |( )| |   | |   | (\ \) |   | |   | |   | |
 | |   ) || (   ) || (\ (   | || || |   | |   | | \   |   | |   | |   | |
 | (__/  )| )   ( || ) \ \__| () () |___) (___| )  \  |___) (___| (___) |
```

### Comparing `darwinio-0.0.5/src/darwinio/distribution.py` & `darwinio-0.0.6/src/darwinio/distribution.py`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.5/src/darwinio/genome.py` & `darwinio-0.0.6/src/darwinio/genome.py`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.5/src/darwinio/graphical_sim.py` & `darwinio-0.0.6/src/darwinio/graphical_sim.py`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.5/src/darwinio/organism.py` & `darwinio-0.0.6/src/darwinio/organism.py`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.5/src/darwinio/text_sim.py` & `darwinio-0.0.6/src/darwinio/text_sim.py`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.5/src/darwinio/assets/art/archaebacteria_halophile.png` & `darwinio-0.0.6/src/darwinio/assets/art/archaebacteria_halophile.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.5/src/darwinio/assets/art/archaebacteria_methanogen.png` & `darwinio-0.0.6/src/darwinio/assets/art/archaebacteria_methanogen.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.5/src/darwinio/assets/art/archaebacteria_thermoacidophile.png` & `darwinio-0.0.6/src/darwinio/assets/art/archaebacteria_thermoacidophile.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.5/src/darwinio/assets/art/eubacteria_BGA.png` & `darwinio-0.0.6/src/darwinio/assets/art/eubacteria_BGA.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.5/src/darwinio/assets/art/eubacteria_mycoplasma.png` & `darwinio-0.0.6/src/darwinio/assets/art/eubacteria_mycoplasma.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.5/src/darwinio/assets/art/eubacteroa_chemosynthetic.png` & `darwinio-0.0.6/src/darwinio/assets/art/eubacteroa_chemosynthetic.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.5/src/darwinio/assets/art/fungi-ascomycetes.png` & `darwinio-0.0.6/src/darwinio/assets/art/fungi-ascomycetes.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.5/src/darwinio/assets/art/fungi-basidiomycetes.png` & `darwinio-0.0.6/src/darwinio/assets/art/fungi-basidiomycetes.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.5/src/darwinio/assets/art/fungi-deuteromycetes.png` & `darwinio-0.0.6/src/darwinio/assets/art/fungi-deuteromycetes.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.5/src/darwinio/assets/art/fungi-phycomycetes.png` & `darwinio-0.0.6/src/darwinio/assets/art/fungi-phycomycetes.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.5/src/darwinio/assets/art/metaphyta-algae.png` & `darwinio-0.0.6/src/darwinio/assets/art/metaphyta-algae.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.5/src/darwinio/assets/art/metaphyta-angiospermae.png` & `darwinio-0.0.6/src/darwinio/assets/art/metaphyta-angiospermae.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.5/src/darwinio/assets/art/metaphyta-bryophyta.png` & `darwinio-0.0.6/src/darwinio/assets/art/metaphyta-bryophyta.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.5/src/darwinio/assets/art/metaphyta-gymnospermae.png` & `darwinio-0.0.6/src/darwinio/assets/art/metaphyta-gymnospermae.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.5/src/darwinio/assets/art/metaphyta-pterdiophyta.png` & `darwinio-0.0.6/src/darwinio/assets/art/metaphyta-pterdiophyta.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.5/src/darwinio/assets/art/protista_dinoflagellate.png` & `darwinio-0.0.6/src/darwinio/assets/art/protista_dinoflagellate.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.5/src/darwinio/assets/art/protista_euglena.png` & `darwinio-0.0.6/src/darwinio/assets/art/protista_euglena.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.5/src/darwinio/assets/art/protista_protozoan.png` & `darwinio-0.0.6/src/darwinio/assets/art/protista_protozoan.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.5/src/darwinio/assets/art/protista_slimemould.png` & `darwinio-0.0.6/src/darwinio/assets/art/protista_slimemould.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.5/src/darwinio/assets/art/theme.json` & `darwinio-0.0.6/src/darwinio/assets/art/theme.json`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.5/src/darwinio/assets/audio/Darwinio.mp3` & `darwinio-0.0.6/src/darwinio/assets/audio/Darwinio.mp3`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.5/LICENSE.md` & `darwinio-0.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.5/pyproject.toml` & `darwinio-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [tool.hatch.build]
 exclude = [
   "*.wav",
 ]
 
 [project]
 name = "darwinio"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Tushar Maharana", email="tusharhero@sdf.org" },
   { name="Mihir Nallagonda", email="adhikshithamihir@gmail.com" },
 ]
 description = "An evolution simulator"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `darwinio-0.0.5/PKG-INFO` & `darwinio-0.0.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: darwinio
-Version: 0.0.5
+Version: 0.0.6
 Summary: An evolution simulator
 Project-URL: Homepage, https://github.com/tusharhero/darwinio
 Project-URL: Bug Tracker, https://github.com/tusharhero/darwinio/issues
 Author-email: Tushar Maharana <tusharhero@sdf.org>, Mihir Nallagonda <adhikshithamihir@gmail.com>
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
@@ -15,48 +15,66 @@
 Requires-Dist: pygame-ce>=2.2.1
 Requires-Dist: pygame-gui>=0.6.9
 Description-Content-Type: text/markdown
 
 # Darwinio
 
  ```ascii
- ______   _______  _______          _________ _       _________ _______ 
+ ______   _______  _______          _________ _       _________ _______
 (  __  \ (  ___  )(  ____ )|\     /|\__   __/( (    /|\__   __/(  ___  )
 | (  \  )| (   ) || (    )|| )   ( |   ) (   |  \  ( |   ) (   | (   ) |
 | |   ) || (___) || (____)|| | _ | |   | |   |   \ | |   | |   | |   | |
 | |   | ||  ___  ||     __)| |( )| |   | |   | (\ \) |   | |   | |   | |
 | |   ) || (   ) || (\ (   | || || |   | |   | | \   |   | |   | |   | |
 | (__/  )| )   ( || ) \ \__| () () |___) (___| )  \  |___) (___| (___) |
 (______/ |/     \||/   \__/(_______)\_______/|/    )_)\_______/(_______)
  ```
 
 This is a Python program that simulates the process of evolution, complete with
-organisms, genetic codes, and neural networks. The program is intended to explore
-the intricacies of the natural world and replicate the processes of evolution
-through a simulation.
+organisms, genetic codes, and neural networks.
+
+## Features
+
+- You get to randomly generate organisms, and see how they evolve.
+- Change the conditions while the simulation is running.
+- You can control - Food and Temperature
+
+## Screenshot
+
+![title screen screenshot](./documentation/screenshot/titlescreen.png)
+![main game play screenshot](./documentation/screenshot/main_game_play.png)
 
 ## Setup
 
 ### *Nix(Gnu-Linux, *BSD, MacOS)
 
-+ Make sure you have Python installed using whichever package manager you use.
-+ Create a Python-venv.
-```bash
-python -m venv .venv
-source .venv/bin/activate
-```
-+ Install the dependencies
-```
-python -m pip install -r requirements.txt
-```
-+ finally, run it,
-```
-cd src
-python main.py
-```
+1. Make sure your python is up-to date
+2. Open your terminal, and install darwinio by running
+   ```bash
+   pip install darwinio
+   ```
+3. To run the program,
+   ```bash
+   python -m darwinio
+   ```
+
+### Microsoft Windows
+
+1. Make sure you python is up-to date, if you don't have python installed
+   install a recent version from [python's official website.](https://python.org/).
+2. Open your terminal/Powershell, and install darwinio by running
+   ```powershell
+   py -m pip install darwinio
+   ```
+3. To run the program,
+   ```powershell
+   py -m darwinio
+   ```
+
+
 ## License
 
 This program is copyright © 2023 Tushar Maharana <tusharhero@sdf.org>,
 and Mihir Nallagonda <adhikshithamihir@gmail.com>.
 
 This program is licensed under the terms of the
 [GNU GENERAL PUBLIC LICENSE VERSION 3](./LICENSE.md) which means this is Free Software.
```

