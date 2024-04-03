# Comparing `tmp/pyved-engine-23.9a5.tar.gz` & `tmp/pyved-engine-24.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyved-engine-23.9a5.tar", last modified: Fri Sep 22 21:39:41 2023, max compression
+gzip compressed data, was "pyved-engine-24.3a1.tar", last modified: Wed Apr  3 12:42:18 2024, max compression
```

## Comparing `pyved-engine-23.9a5.tar` & `pyved-engine-24.3a1.tar`

### file list

```diff
@@ -1,203 +1,212 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 21:39:41.046912 pyved-engine-23.9a5/
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      300 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9203 2023-09-22 21:39:41.046912 pyved-engine-23.9a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8769 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-22 21:39:41.046912 pyved-engine-23.9a5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 21:39:41.022911 pyved-engine-23.9a5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 21:39:41.026911 pyved-engine-23.9a5/src/pyvcmdline/
--rw-r--r--   0 runner    (1001) docker     (127)      371 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38298 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 21:39:41.026911 pyved-engine-23.9a5/src/pyvcmdline/emb_demos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/emb_demos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/emb_demos/my_demo1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/json_prec.py
--rw-r--r--   0 runner    (1001) docker     (127)     4308 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/launch_game.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 21:39:41.022911 pyved-engine-23.9a5/src/pyvcmdline/template_0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 21:39:41.026911 pyved-engine-23.9a5/src/pyvcmdline/template_0/cartridge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_0/cartridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_0/cartridge/gamedef.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_0/cartridge/pimodules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 21:39:41.022911 pyved-engine-23.9a5/src/pyvcmdline/template_1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 21:39:41.026911 pyved-engine-23.9a5/src/pyvcmdline/template_1/cartridge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_1/cartridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_1/cartridge/gamedef.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_1/cartridge/pimodules.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_1/cartridge/shared.py
--rw-r--r--   0 runner    (1001) docker     (127)     3403 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_1/cartridge/systems.py
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_1/cartridge/world.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 21:39:41.022911 pyved-engine-23.9a5/src/pyvcmdline/template_2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 21:39:41.026911 pyved-engine-23.9a5/src/pyvcmdline/template_2/cartridge/
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_2/cartridge/World.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_2/cartridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3283 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_2/cartridge/classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_2/cartridge/gamedef.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_2/cartridge/my_map.ncsv
--rw-r--r--   0 runner    (1001) docker     (127)       98 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_2/cartridge/pimodules.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_2/cartridge/shared.py
--rw-r--r--   0 runner    (1001) docker     (127)     7057 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_2/cartridge/systems.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 21:39:41.022911 pyved-engine-23.9a5/src/pyvcmdline/template_3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 21:39:41.030912 pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/ChessGUI_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/ChessGameParams.py
--rw-r--r--   0 runner    (1001) docker     (127)     3391 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/ChessmatchMod.py
--rw-r--r--   0 runner    (1001) docker     (127)     8573 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/PythonChessAIStats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4402 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/ScrollingTextBox.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14676 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/ai_players.py
--rw-r--r--   0 runner    (1001) docker     (127)    43714 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/black_bishop.png
--rw-r--r--   0 runner    (1001) docker     (127)    62348 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/black_king.png
--rw-r--r--   0 runner    (1001) docker     (127)    56206 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/black_knight.png
--rw-r--r--   0 runner    (1001) docker     (127)    49193 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/black_pawn.png
--rw-r--r--   0 runner    (1001) docker     (127)    44736 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/black_queen.png
--rw-r--r--   0 runner    (1001) docker     (127)    46630 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/black_rook.png
--rw-r--r--   0 runner    (1001) docker     (127)      196 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/brown_square.png
--rw-r--r--   0 runner    (1001) docker     (127)      734 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/chdefs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15696 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/chess_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     4075 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/chessintro.py
--rw-r--r--   0 runner    (1001) docker     (127)    15158 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/chessmatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/cyan_square.png
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/gamedef.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/info-assets.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4531 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/main_gui_view.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    19833 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/pimodules.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/run_chess.py
--rw-r--r--   0 runner    (1001) docker     (127)    48191 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/white_bishop.png
--rw-r--r--   0 runner    (1001) docker     (127)    70224 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/white_king.png
--rw-r--r--   0 runner    (1001) docker     (127)    63997 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/white_knight.png
--rw-r--r--   0 runner    (1001) docker     (127)    54315 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/white_pawn.png
--rw-r--r--   0 runner    (1001) docker     (127)    49247 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/white_queen.png
--rw-r--r--   0 runner    (1001) docker     (127)    51431 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/white_rook.png
--rw-r--r--   0 runner    (1001) docker     (127)      200 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/white_square.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 21:39:41.022911 pyved-engine-23.9a5/src/pyvcmdline/template_4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 21:39:41.034911 pyved-engine-23.9a5/src/pyvcmdline/template_4/cartridge/
--rw-r--r--   0 runner    (1001) docker     (127)     6555 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_4/cartridge/CC0 License.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_4/cartridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5222 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_4/cartridge/avatar1.png
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_4/cartridge/gamedef.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_4/cartridge/info.txt
--rw-r--r--   0 runner    (1001) docker     (127)      876 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_4/cartridge/monster.png
--rw-r--r--   0 runner    (1001) docker     (127)     6333 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_4/cartridge/mvc_parts.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_4/cartridge/pimodules.py
--rw-r--r--   0 runner    (1001) docker     (127)    88026 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyvcmdline/template_4/cartridge/tileset.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 21:39:41.034911 pyved-engine-23.9a5/src/pyved_engine/
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/Singleton.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8976 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/_ecs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6140 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/_ecs_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     3642 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/_hub.py
--rw-r--r--   0 runner    (1001) docker     (127)     7761 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/_pyv_implem.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/_utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 21:39:41.022911 pyved-engine-23.9a5/src/pyved_engine/add_ons/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 21:39:41.038912 pyved-engine-23.9a5/src/pyved_engine/add_ons/gui/
--rw-r--r--   0 runner    (1001) docker     (127)     6362 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/add_ons/gui/BaseGuiElement.py
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/add_ons/gui/Button.py
--rw-r--r--   0 runner    (1001) docker     (127)     6388 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/add_ons/gui/Button2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/add_ons/gui/DispCenteredPopup.py
--rw-r--r--   0 runner    (1001) docker     (127)    10310 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/add_ons/gui/DispPopup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3768 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/add_ons/gui/Label.py
--rw-r--r--   0 runner    (1001) docker     (127)     3476 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/add_ons/gui/TextBlock.py
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/add_ons/gui/Trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3872 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/add_ons/gui/WidgetBo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/add_ons/gui/WidgetContainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6813 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/add_ons/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7654 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/add_ons/gui/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7034 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/add_ons/gui/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 21:39:41.038912 pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24970 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     6546 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 21:39:41.038912 pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/
--rw-r--r--   0 runner    (1001) docker     (127)      836 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/common_types.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     7189 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 21:39:41.038912 pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 21:39:41.038912 pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/json/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12154 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/json/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/json/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     8784 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/json/tiled_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    10066 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/json/tiled_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    10750 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/json/tileset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/json/wang_set.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 21:39:41.042912 pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/tmx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/tmx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11770 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/tmx/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/tmx/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     6619 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/tmx/tiled_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     9363 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/tmx/tiled_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     7392 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/tmx/tileset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/tmx/wang_set.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     3316 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/tiled_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     5087 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/tiled_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    10641 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/tileset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/util.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3085 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/wang_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     4941 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/world.py
--rw-r--r--   0 runner    (1001) docker     (127)     5382 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/ztilemap.py
--rw-r--r--   0 runner    (1001) docker     (127)    13290 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4704 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/classes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 21:39:41.042912 pyved-engine-23.9a5/src/pyved_engine/compo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/compo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11201 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/compo/gfx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/compo/modes.py
--rw-r--r--   0 runner    (1001) docker     (127)    40142 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/compo/packed_capello_ft.py
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/compo/vscreen.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 21:39:41.042912 pyved-engine-23.9a5/src/pyved_engine/core/
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/core/Injector.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9611 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/core/events.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/core_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11780 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/custom_struct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 21:39:41.042912 pyved-engine-23.9a5/src/pyved_engine/foundation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/foundation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6681 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/foundation/defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/foundation/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     8045 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/foundation/pbackends.py
--rw-r--r--   0 runner    (1001) docker     (127)    17075 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/legacy_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/legacy_init.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/legacy_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 21:39:41.042912 pyved-engine-23.9a5/src/pyved_engine/looparts/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/looparts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 21:39:41.046912 pyved-engine-23.9a5/src/pyved_engine/looparts/ai/
--rw-r--r--   0 runner    (1001) docker     (127)     3934 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/looparts/ai/FSA_classes_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/looparts/ai/NorrecBrain.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/looparts/ai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/looparts/ai/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     5018 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/looparts/anim.py
--rw-r--r--   0 runner    (1001) docker     (127)    35467 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/looparts/ascii.py
--rw-r--r--   0 runner    (1001) docker     (127)    17900 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/looparts/console.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 21:39:41.046912 pyved-engine-23.9a5/src/pyved_engine/looparts/demolib/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/looparts/demolib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4192 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/looparts/demolib/animobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8178 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/looparts/demolib/dialogue.py
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/looparts/demolib/pathfinding.py
--rw-r--r--   0 runner    (1001) docker     (127)    15785 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/looparts/demolib/rpgmenu.py
--rw-r--r--   0 runner    (1001) docker     (127)    21241 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/looparts/rogue.py
--rw-r--r--   0 runner    (1001) docker     (127)    11888 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/looparts/rpg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/looparts/sysconsole.py
--rw-r--r--   0 runner    (1001) docker     (127)    15881 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/looparts/tabletop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/looparts/terrain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3862 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/pal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/state_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     4766 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/tankui.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/src/pyved_engine/vars.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 21:39:41.034911 pyved-engine-23.9a5/src/pyved_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9203 2023-09-22 21:39:41.000000 pyved-engine-23.9a5/src/pyved_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7619 2023-09-22 21:39:41.000000 pyved-engine-23.9a5/src/pyved_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-22 21:39:41.000000 pyved-engine-23.9a5/src/pyved_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2023-09-22 21:39:41.000000 pyved-engine-23.9a5/src/pyved_engine.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2023-09-22 21:39:41.000000 pyved-engine-23.9a5/src/pyved_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-09-22 21:39:41.000000 pyved-engine-23.9a5/src/pyved_engine.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 21:39:41.046912 pyved-engine-23.9a5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      723 2023-09-22 21:39:32.000000 pyved-engine-23.9a5/tests/test_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:42:18.884230 pyved-engine-24.3a1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9208 2024-04-03 12:42:18.884230 pyved-engine-24.3a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8774 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 12:42:18.884230 pyved-engine-24.3a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:42:18.852230 pyved-engine-24.3a1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:42:18.856230 pyved-engine-24.3a1/src/pyvcmdline/
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43876 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:42:18.856230 pyved-engine-24.3a1/src/pyvcmdline/emb_demos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/emb_demos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/emb_demos/my_demo1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/json_prec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/pyvcli_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:42:18.852230 pyved-engine-24.3a1/src/pyvcmdline/template_0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:42:18.856230 pyved-engine-24.3a1/src/pyvcmdline/template_0/cartridge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_0/cartridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_0/cartridge/gamedef.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_0/cartridge/pimodules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:42:18.852230 pyved-engine-24.3a1/src/pyvcmdline/template_1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:42:18.856230 pyved-engine-24.3a1/src/pyvcmdline/template_1/cartridge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_1/cartridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_1/cartridge/gamedef.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_1/cartridge/pimodules.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_1/cartridge/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_1/cartridge/systems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_1/cartridge/world.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:42:18.852230 pyved-engine-24.3a1/src/pyvcmdline/template_2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:42:18.860230 pyved-engine-24.3a1/src/pyvcmdline/template_2/cartridge/
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_2/cartridge/World.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_2/cartridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_2/cartridge/classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_2/cartridge/gamedef.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_2/cartridge/my_map.ncsv
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_2/cartridge/pimodules.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_2/cartridge/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7057 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_2/cartridge/systems.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10384 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_2/cartridge/thumb_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12766 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_2/cartridge/thumb_2.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:42:18.852230 pyved-engine-24.3a1/src/pyvcmdline/template_3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:42:18.864230 pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/ChessGUI_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/ChessGameParams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/ChessmatchMod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8573 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/PythonChessAIStats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/ScrollingTextBox.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14676 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/ai_players.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43714 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/black_bishop.png
+-rw-r--r--   0 runner    (1001) docker     (127)    62348 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/black_king.png
+-rw-r--r--   0 runner    (1001) docker     (127)    56206 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/black_knight.png
+-rw-r--r--   0 runner    (1001) docker     (127)    49193 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/black_pawn.png
+-rw-r--r--   0 runner    (1001) docker     (127)    44736 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/black_queen.png
+-rw-r--r--   0 runner    (1001) docker     (127)    46630 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/black_rook.png
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/brown_square.png
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/chdefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15696 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/chess_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4075 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/chessintro.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15158 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/chessmatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/cyan_square.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/gamedef.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/info-assets.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4531 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/main_gui_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19833 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/pimodules.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/run_chess.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10384 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/thumb_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12766 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/thumb_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    48191 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/white_bishop.png
+-rw-r--r--   0 runner    (1001) docker     (127)    70224 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/white_king.png
+-rw-r--r--   0 runner    (1001) docker     (127)    63997 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/white_knight.png
+-rw-r--r--   0 runner    (1001) docker     (127)    54315 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/white_pawn.png
+-rw-r--r--   0 runner    (1001) docker     (127)    49247 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/white_queen.png
+-rw-r--r--   0 runner    (1001) docker     (127)    51431 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/white_rook.png
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/white_square.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:42:18.852230 pyved-engine-24.3a1/src/pyvcmdline/template_4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:42:18.868230 pyved-engine-24.3a1/src/pyvcmdline/template_4/cartridge/
+-rw-r--r--   0 runner    (1001) docker     (127)     6555 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_4/cartridge/CC0 License.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_4/cartridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_4/cartridge/avatar1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_4/cartridge/gamedef.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_4/cartridge/glvars.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_4/cartridge/info.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_4/cartridge/monster.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7151 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_4/cartridge/mvc_parts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_4/cartridge/pimodules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9278 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_4/cartridge/smallninja_sprites.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10384 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_4/cartridge/thumb_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12766 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_4/cartridge/thumb_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    88026 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyvcmdline/template_4/cartridge/tileset.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:42:18.872230 pyved-engine-24.3a1/src/pyved_engine/
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/Singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8976 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/_ecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/_ecs_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/_hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7761 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/_pyv_implem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/_utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:42:18.852230 pyved-engine-24.3a1/src/pyved_engine/add_ons/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:42:18.872230 pyved-engine-24.3a1/src/pyved_engine/add_ons/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)     6362 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/add_ons/gui/BaseGuiElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/add_ons/gui/Button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/add_ons/gui/Button2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/add_ons/gui/DispCenteredPopup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10310 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/add_ons/gui/DispPopup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/add_ons/gui/Label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/add_ons/gui/TextBlock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/add_ons/gui/Trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/add_ons/gui/WidgetBo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/add_ons/gui/WidgetContainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6813 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/add_ons/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7654 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/add_ons/gui/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7034 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/add_ons/gui/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:42:18.876230 pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24970 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:42:18.876230 pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7189 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:42:18.876230 pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:42:18.876230 pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/json/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12154 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/json/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/json/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8784 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/json/tiled_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10066 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/json/tiled_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10750 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/json/tileset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/json/wang_set.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:42:18.880230 pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/tmx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/tmx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11770 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/tmx/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/tmx/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/tmx/tiled_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9363 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/tmx/tiled_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7392 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/tmx/tileset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/tmx/wang_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/tiled_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/tiled_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10641 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/tileset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/wang_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4941 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/world.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/ztilemap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13762 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/classes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:42:18.880230 pyved-engine-24.3a1/src/pyved_engine/compo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/compo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11201 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/compo/gfx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/compo/modes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40142 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/compo/packed_capello_ft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/compo/vscreen.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:42:18.880230 pyved-engine-24.3a1/src/pyved_engine/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/core/Injector.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9611 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/core/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/core_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11780 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/custom_struct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:42:18.880230 pyved-engine-24.3a1/src/pyved_engine/foundation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/foundation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/foundation/defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/foundation/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8045 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/foundation/pbackends.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17075 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/legacy_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/legacy_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/legacy_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:42:18.884230 pyved-engine-24.3a1/src/pyved_engine/looparts/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/looparts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:42:18.884230 pyved-engine-24.3a1/src/pyved_engine/looparts/ai/
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/looparts/ai/FSA_classes_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/looparts/ai/NorrecBrain.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/looparts/ai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/looparts/ai/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/looparts/anim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35467 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/looparts/ascii.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17900 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/looparts/console.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:42:18.884230 pyved-engine-24.3a1/src/pyved_engine/looparts/demolib/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/looparts/demolib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/looparts/demolib/animobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8178 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/looparts/demolib/dialogue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/looparts/demolib/pathfinding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15785 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/looparts/demolib/rpgmenu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21616 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/looparts/rogue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11888 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/looparts/rpg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/looparts/sysconsole.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15881 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/looparts/tabletop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/looparts/terrain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/pal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/state_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4766 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/tankui.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/src/pyved_engine/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:42:18.884230 pyved-engine-24.3a1/src/pyved_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9208 2024-04-03 12:42:18.000000 pyved-engine-24.3a1/src/pyved_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8038 2024-04-03 12:42:18.000000 pyved-engine-24.3a1/src/pyved_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 12:42:18.000000 pyved-engine-24.3a1/src/pyved_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-03 12:42:18.000000 pyved-engine-24.3a1/src/pyved_engine.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-03 12:42:18.000000 pyved-engine-24.3a1/src/pyved_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 12:42:18.000000 pyved-engine-24.3a1/src/pyved_engine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:42:18.884230 pyved-engine-24.3a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-03 12:42:15.000000 pyved-engine-24.3a1/tests/test_engine.py
```

### Comparing `pyved-engine-23.9a5/LICENSE` & `pyved-engine-24.3a1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/PKG-INFO` & `pyved-engine-24.3a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pyved-engine
-Version: 23.9a5
+Version: 24.3a1
 Summary: Custom game engine built upon python/pygame
 Home-page: https://github.com/gaudiatech/pyved-engine
 Author: moonb3ndr et al.
 Author-email: thomas.iw@kata.games
 License: LGPL3
 Keywords: Python,Pygame,Game Engine
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pygame-ce>=2.2.1
 Requires-Dist: pyperclip>=1.8.2
 Requires-Dist: requests>=2.28.1
 
 <p align="center">
-  <img src="https://gaudia-tech.com/shared/pyv-logo.jpg" alt="pyv logo" />
+  <img src="https://www.gaudia-tech.com/mirror/pyv-logo.jpg" alt="pyv logo" />
 </p>
 
 Introducing `pyved-engine`, a Python package that provides you with
 the versatile, efficient 2D game engine named PYV!
 Designed to streamline game development, PYV offers a set of
 tools for smooth and rapid game prototyping.
 
@@ -31,15 +31,15 @@
 </a>
 </p>
 
 
 
 ## 1. Introduction
 
-### Cpabilities of a game engine
+### Capabilities of a game engine
 
 A game engine provides invaluable time-saving benefits by storing a collection
 of useful and reusable code snippets within its framework.
 Instead of reinventing the wheel and wasting your precious time by re-writing
 generic code for video games, you can leverage the power of the engine.
 
 By referring to the
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: pyved-engine Version: 23.9a5 Summary: Custom game
+Metadata-Version: 2.1 Name: pyved-engine Version: 24.3a1 Summary: Custom game
 engine built upon python/pygame Home-page: https://github.com/gaudiatech/pyved-
 engine Author: moonb3ndr et al. Author-email: thomas.iw@kata.games License:
 LGPL3 Keywords: Python,Pygame,Game Engine Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: pygame-ce>=2.2.1 Requires-Dist:
 pyperclip>=1.8.2 Requires-Dist: requests>=2.28.1
                                   [pyv logo]
 Introducing `pyved-engine`, a Python package that provides you with the
 versatile, efficient 2D game engine named PYV! Designed to streamline game
 development, PYV offers a set of tools for smooth and rapid game prototyping.
 Unlock the full potential of your game development thanks to __pyv__!
                         _T_o_ _j_o_i_n_ _o_u_r_ _D_i_s_c_o_r_d_ _c_o_m_m_u_n_i_t_y_:
                              _[_j_o_i_n_ _u_s_ _o_n_ _D_i_s_c_o_r_d_]
-## 1. Introduction ### Cpabilities of a game engine A game engine provides
+## 1. Introduction ### Capabilities of a game engine A game engine provides
 invaluable time-saving benefits by storing a collection of useful and reusable
 code snippets within its framework. Instead of reinventing the wheel and
 wasting your precious time by re-writing generic code for video games, you can
 leverage the power of the engine. By referring to the [work-in-progress
 documentation](https://gaudiatech.github.io/pyved-engine/), you could quickly
 learn how to implement various functionalities such as pathfinding or loading
 spritesheets. With simple function or method calls, you can seamlessly
```

### Comparing `pyved-engine-23.9a5/README.md` & `pyved-engine-24.3a1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <p align="center">
-  <img src="https://gaudia-tech.com/shared/pyv-logo.jpg" alt="pyv logo" />
+  <img src="https://www.gaudia-tech.com/mirror/pyv-logo.jpg" alt="pyv logo" />
 </p>
 
 Introducing `pyved-engine`, a Python package that provides you with
 the versatile, efficient 2D game engine named PYV!
 Designed to streamline game development, PYV offers a set of
 tools for smooth and rapid game prototyping.
 
@@ -16,15 +16,15 @@
 </a>
 </p>
 
 
 
 ## 1. Introduction
 
-### Cpabilities of a game engine
+### Capabilities of a game engine
 
 A game engine provides invaluable time-saving benefits by storing a collection
 of useful and reusable code snippets within its framework.
 Instead of reinventing the wheel and wasting your precious time by re-writing
 generic code for video games, you can leverage the power of the engine.
 
 By referring to the
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
                                   [pyv logo]
 Introducing `pyved-engine`, a Python package that provides you with the
 versatile, efficient 2D game engine named PYV! Designed to streamline game
 development, PYV offers a set of tools for smooth and rapid game prototyping.
 Unlock the full potential of your game development thanks to __pyv__!
                         _T_o_ _j_o_i_n_ _o_u_r_ _D_i_s_c_o_r_d_ _c_o_m_m_u_n_i_t_y_:
                              _[_j_o_i_n_ _u_s_ _o_n_ _D_i_s_c_o_r_d_]
-## 1. Introduction ### Cpabilities of a game engine A game engine provides
+## 1. Introduction ### Capabilities of a game engine A game engine provides
 invaluable time-saving benefits by storing a collection of useful and reusable
 code snippets within its framework. Instead of reinventing the wheel and
 wasting your precious time by re-writing generic code for video games, you can
 leverage the power of the engine. By referring to the [work-in-progress
 documentation](https://gaudiatech.github.io/pyved-engine/), you could quickly
 learn how to implement various functionalities such as pathfinding or loading
 spritesheets. With simple function or method calls, you can seamlessly
```

### Comparing `pyved-engine-23.9a5/setup.py` & `pyved-engine-24.3a1/setup.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyvcmdline/__main__.py` & `pyved-engine-24.3a1/src/pyvcmdline/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,40 @@
 """
-    pyved_engine.cmdline
-    ~~~~~~~~~~~~~~~~
+    pyved_engine/__main__
 
-    Command line interface.
-
-    :copyright: Copyright 2018-2023 by the Kata.Games team, see AUTHORS.
-    :license: MIT, see LICENSE for details.
+    Here, we define the command line interface
+    :copyright: Copyright 2018-2024 by the Kata.Games team.
+    :license: LGPL-3.0, see LICENSE for details.
 """
 import argparse
 import importlib
 import json
 import os
 import re
-import requests
 import shutil
 import sys
 import tempfile
 import time
-from .json_prec import TEMPL_ID_TO_JSON_STR
 import zipfile
+from pprint import pprint
 
-# will be used later on, where `pyv-cli share` becomes a thing
-# import requests
-
+import pyperclip
+import requests  # used to implement the `pyv-cli share` feature
+from .pyvcli_cogs import *
 from pyved_engine import vars
+from .const import *
+from .json_prec import TEMPL_ID_TO_JSON_STR
+from .pyvcli_config import API_HOST_PLAY_DEV, API_ENDPOINT_DEV, \
+    FRUIT_URL_TEMPLATE_DEV
+from .pyvcli_config import BETA_VM_API_HOST, API_ENDPOINT_BETA, FRUIT_URL_TEMPLATE_BETA
+from .pyvcli_config import VMSTORAGE_URL
 
 __version__ = vars.ENGINE_VERSION_STR
 
 
-PLAY_SCRIPT_NAME = 'launch_game'
-VALID_SUBCOMMANDS = (
-    'init',
-    'play',
-    'share',
-    'pub'
-)
-
-
 # -----------------------------------
 #  kept only to have some 'template' for arg parsing, not using anything below
 # -----------------------------------
 # from pygments import __version__, highlight
 # from pygments.util import ClassNotFound, OptionError, docstring_headline, \
 #     guess_decode, guess_decode_from_terminal, terminal_encoding, \
 #     UnclosingTextIOWrapper
@@ -202,128 +196,100 @@
 #                 'doc': docstring_headline(cls)
 #             }
 #         result['styles'] = info
 #
 #     json.dump(result, sys.stdout)
 
 
-def play_command(x):
+def play_subcommand(x):
+    if '.' != x and os.path.isdir('cartridge'):
+        raise ValueError('launching with a "cartridge" in the current folder, but no parameter "." is forbidden')
     metadata = None
     try:
-        fptr = open(fpath_join(x, 'cartridge', 'metadat.json'), 'r')
+        fptr = open(os.path.join(x, 'cartridge', 'metadat.json'), 'r')
         metadata = json.load(fptr)
         fptr.close()
         print(f"game bundle {x} found. Loading...")
         print('Metadata:\n', metadata)
     except FileNotFoundError:
         print(f'Error: cannot find the game bundle you specified: {x}')
         print('  Are you sure it exists in the current folder? Alternatively you can try to')
         print('  change directory (cd) and simply type `pyv-cli play`')
         print('  once you are inside the bundle')
 
     if metadata is not None:
         sys.path.append(os.getcwd())
         if x == '.':
-            vmsl = importlib.import_module(PLAY_SCRIPT_NAME, None)
+            vmsl = importlib.import_module(LAUNCH_GAME_SCRIPT_BASENAME, None)
         else:
-            vmsl = importlib.import_module('.'+PLAY_SCRIPT_NAME, x)
+            vmsl = importlib.import_module('.' + LAUNCH_GAME_SCRIPT_BASENAME, x)
         vmsl.bootgame(metadata)
 
 
-# alias!
-fpath_join = os.path.join
-
-
-def recursive_copy(source_folder, destination_folder):
-    if not os.path.exists(destination_folder):
-        os.makedirs(destination_folder)
-
-    for item in os.listdir(source_folder):
-        source_item = fpath_join(source_folder, item)
-        destination_item = fpath_join(destination_folder, item)
-
-        if os.path.isdir(source_item):
-            recursive_copy(source_item, destination_item)
-        else:
-            shutil.copy2(source_item, destination_item)
+def _is_valid_identifier(test_identifier):
+    ok_pattern = '^[a-zA-Z0-9_]+$'
+    return bool(re.match(ok_pattern, test_identifier))
 
 
-def create_folder_and_serialize_dict(folder0_name, data_dict):
-    # Check if the folder exists, create it if not
-    folder1_name = fpath_join(folder0_name, 'cartridge')
-    if not os.path.exists(folder1_name):
-        os.makedirs(folder1_name)
-
-    # Serialize the dictionary using JSON and create a JSON file
-    json_file_path = fpath_join(folder1_name, 'metadat.json')
-    with open(json_file_path, 'w') as json_file:
-        json.dump(data_dict, json_file, indent=4)
-
-
-def init_command(cartridge_name) -> None:
+def init_command(game_identifier) -> None:
     """
     this is the pyv-cli INIT command, it should create a new game bundle, fully operational
-    :param cartridge_name: name for your new bundle...
+    :param game_identifier: name for your new bundle...
     """
-    possib_templates = {
-        0: 'Empty',
-        1: 'Breakout',
-        2: 'Platformer',
-        3: 'Chess',
-        4: 'Roguelike'
-    }
-    bsup_template_id = 4
+    print(f" Calling sub-command INIT: with game identifier(slug)={game_identifier}")
+    print()
 
-    print(f" Using sub-command INIT: your new cartridge name is [{cartridge_name}]")
-    print('-' * 60)
     print('  Game templates:')
-    for code, name in possib_templates.items():
+    for code, name in POSSIB_TEMPLATES.items():
         print(f'    {code}:  {name}')
     template_id = input('select a template: ')
-    while not (template_id.isnumeric() and 0 <= int(template_id) <= bsup_template_id):
+    while not (template_id.isnumeric() and 0 <= int(template_id) <= MAX_TEMPLATE_ID):
         print('invalid input!')
         template_id = input('select a template: ')
     template_id = int(template_id)
     print('-' * 60)
 
     adhoc_json_prec = TEMPL_ID_TO_JSON_STR[template_id]
     metadata = json.loads(adhoc_json_prec)
-    # TODO perform this important check:
-    #  assets need to be already available in cartridge/
 
-    pattern = '^[a-zA-Z0-9]+$'
-    is_validname = bool(re.match(pattern, cartridge_name))
-    while not is_validname:
-        print('*** WARNING: bundle name needs to contains only alphanumeric that is A-Z and a-z and 0-9 characters')
-        cartridge_name = input('please select another valid name for your game bundle: ')
-        is_validname = bool(re.match(pattern, cartridge_name))
-    x = cartridge_name
+    # TODO: shall we use HERE
+    #  the network to test if the name is remotely available?
+    #  that feature is already implemented by the 'test' subcommand
+
+    while not _is_valid_identifier(game_identifier):
+        print('*** WARNING: the selected game identifier is rejected. Expected format:')
+        print(' solely alphanumeric that is A-Z and a-z, plus 0-9 numbers and the underscore _ special character')
+        game_identifier = input('enter another game identifier(slug): ')
 
-    metadata['cartridge'] = x
-    tmp = input('whats the name of your game? [Default: Same as the bundle]')
+    x = game_identifier
+
+    metadata['slug'] = x
+    tmp = input('whats the name of the game? [Default: Equal to the bundle name]')
     metadata['game_title'] = tmp if len(tmp) > 0 else x
 
     tmp = input('whos the author? [Default: Unknown]')
     metadata['author'] = tmp if len(tmp) > 0 else 'Unknown'
     metadata['vmlib_ver'] = __version__.replace('.', '_')
 
     metadata['build_date'] = time.ctime(time.time())
 
     # Get the absolute path of the current script
     script_directory = os.path.dirname(os.path.abspath(__file__))
-    lg_script_blueprint_filename = fpath_join(script_directory, PLAY_SCRIPT_NAME+'.py')
-    template_blueprint_folder = fpath_join(script_directory, f'template_{template_id}')
-    target_bundle_folder = fpath_join(os.getcwd(), x)
-
-    recursive_copy(template_blueprint_folder, target_bundle_folder)
-    shutil.copy2(lg_script_blueprint_filename, target_bundle_folder)
-    create_folder_and_serialize_dict(target_bundle_folder, data_dict=metadata)
+    template_blueprint_folder = os.path.join(script_directory, f'template_{template_id}')
+    target_folder = os.path.join(os.getcwd(), x)
+    recursive_copy(template_blueprint_folder, target_folder)
+
+    copy_launcher_script(x)
+    create_folder_and_serialize_dict(target_folder, data_dict=metadata)
     for _ in range(3):
         print()
+
     print('GAME BUNDLE=', x)
+    print('Important remark: do not rename the name of the folder! (Game bundle)')
+
     print(f'--->Succesfully created! Now you can type `pyv-cli play {x}`')
     print('Go ahead and have fun ;)')
 
 
 def create_zip_from_folder(bundle_name, source_folder):
     # origin_no_sep = source_folder.rstrip('/\\')
     tmp_output_zip_filename = 'output.zip'
@@ -354,77 +320,165 @@
 #     def __init__(self, *args, **keyws):
 #         file.__init__(self, *args, **keyws)
 #
 #     def __len__(self):
 #         return int(os.fstat(self.fileno())[6])
 
 
-def trigger_publish(chosenslug, remote_cart_id) -> bool:
+def trigger_publish(slug):
     """
-    once the game is available server-side as a stored cartridge (therefore it has a cartridge_id ...)
+    once the game is available server-side, as a stored cartridge,
+    (therefore your game has a slug/Server-side game identifier)
+
     we trigger the "PUBLISH" op server-side.
     This means the game will spawn/pop within the gaming CMS (cloudarcade)
 
-    :param chosenslug:
-    :param remote_cart_id: str that was provided by the server to uniquely identify a game cartridge
+    :param slug: str that the server uses to uniquely identify a cartridge
     stored server-side
     :return: True/False
     """
     dummy_json_str = """
 {
-"title": "This is the game title",
-"slug": "essaiFlappy",
+"game_title": "This is the game title",
+"slug": "flappy",
 "description": "This is a test game",
 "instructions": "Click any object to move",
 "width": 960,
 "height": 720,
 "thumb_1": "https://img.gamemonetize.com/ulol31p2l8xogmlxh1yqfa64dxzkyrix/512x384.jpg",
 "thumb_2": "https://img.gamemonetize.com/ulol31p2l8xogmlxh1yqfa64dxzkyrix/512x384.jpg",
 "category": "Puzzle,Arcade,Action",
 "source": "API",
-"cartridge":"flappy"
 }
 """
-    TARG_TRIGGER_PUBLISH = 'https://kata.games/api/uploads.php'
-
     # check that can be deserialized...
     jsondata = json.loads(dummy_json_str)
-    jsondata['slug'] = x = chosenslug
-    jsondata['cartridge'] = y = remote_cart_id
+    jsondata['slug'] = x = slug
+    # jsondata['cartridge'] = y = slug
     # print(jsondata)
     # print(type(jsondata))
 
     reply = requests.post(
         url=TARG_TRIGGER_PUBLISH,
         data=json.dumps(jsondata)
     )
-    print(f'trigger_publish CALLED (arg:x,y=={x},{y})--- result is...')
+    print(f'trigger_publish CALLED (arg:x=={x})--- result is...')
     print(reply.text)
 
 
-def upload_my_zip_file(zip_file_path, server_host):
-    # new and shiny (ver2 . september23)
-    # TODO: this works only on the local VM, how to port it to work in production mode?
-    import pyperclip
+# TODO will be useful for implementing a future "repair" bundle subcommand
+# def _bundle_renaming(path_to_bundle):
+#     # ensure that OUR NORM is respected:
+#     # what norm? We need to enforce the rule that states:
+#     # the directory name == the slug
+#     pass
+
+
+def _query_slug_availability(x):
+    # ---------------------------------------
+    #  test for slug availability!
+    # ---------------------------------------
+    CAN_UPLOAD_SCRIPT = 'can_upload.php'
+    slug_avail_serv_truth = requests.get(
+        VMSTORAGE_URL + '/' + CAN_UPLOAD_SCRIPT,
+        {'slug': x}
+    )
+    # error handling after ping the VMstorage remote service
+    if slug_avail_serv_truth.status_code != 200:
+        raise Exception('[netw error] cannot reach the VMstorage service! Contact developers to report that bug please')
+    obj_serv_truth = slug_avail_serv_truth.json()
+    if ('success' not in obj_serv_truth) or not obj_serv_truth['success']:
+        raise Exception('[protocol error] unexpected result after communication with VMstorage service. Contact devs')
+    return obj_serv_truth
+
+
+def ensure_correct_slug(givenslug):
+    """
+    goal=
+    renaming bundle if and only if it is required
+    """
+    server_truth = _query_slug_availability(givenslug)
+    assert (server_truth['success'])
+
+    print('availability?', server_truth['available'])
+    if not (server_truth['available']):
+        print('SUGGESTIONS:')
+        for elt in server_truth['suggestions']:
+            print('   *', elt)
+    print()
+    print('-' * 60)
+
+
+def test_subcommand(bundle_name):
+    print(f"***TESTING bundle {bundle_name}***")
+
+    metadat = read_metadata(bundle_name)
+    pprint(metadat)
+    print()
+    btest = verify_metadata(metadat)
+    print('valid metadata?', btest is None)
+    if btest is not None:
+        raise ValueError('Invalid metadata file! Missing key= {}'.format(btest))
+
+    # ensure that thumbnails & assets described do exist:
+    print('ensuring if assets exist')
+    files_exp_li = [  # all expected files need to be known
+        metadat['thumbnail512x384'],
+        metadat['thumbnail512x512']
+    ]
+    files_exp_li.extend(metadat['assets'])
+    for elt in files_exp_li:
+        print('____testing file:', elt)
+        if not test_isfile_in_cartridge(elt, bundle_name):
+            raise FileNotFoundError('cannot find asset:', elt)
+    print('assets --->OK')
+    print()
+
+    print('COHESION test:', bundle_name == metadat['slug'])
+    print()
+
+    print('~ Serv-side Slug Availability? ~')
+    obj = _query_slug_availability(metadat['slug'])
+    if not obj['success']:
+        raise ValueError('cannot read info from server!')
+    print(' ->', 'yes' if obj['available'] else 'no')
+    if not obj['available']:
+        print('suggestions:')
+        pprint(obj['suggestions'])
+
+
+def upload_my_zip_file(zip_file_path: str, gslug, debugmode: bool) -> None:
+    """
+    :zip_file_path: as param name indicates
+    :param: dev_mode is a flag to say if we target the dev server or prod server...
+
+    Side effect: puts something important in the paperclip!
+    """
     file_to_send = zip_file_path  # dont forget the extension!
+    api_endpoint = API_ENDPOINT_DEV if debugmode else API_ENDPOINT_BETA
+    # serv_host = DEV_SERVER_HOST if dev_mode else PROD_SERVER_HOST
+
     files = {
         'uploadedFile': (file_to_send,
                          open(file_to_send, 'rb'),
                          'application/zip',
                          {'Expires': '0'})
     }
     reply = requests.post(
-        url=server_host + 'webapp_backend/do_upload.php',
+        url=api_endpoint,
         files=files,
-        data={'pyv-cli-flag': True, 'uploadBtn': 'Upload'}
+        data={'pyv-cli-flag': True, 'chosen-slug': gslug, 'uploadBtn': 'Upload'}
     )
     print('upload_my_zip_file called! Resp. is:')
     print(reply.text)
     rep_obj = json.loads(reply.text)
-    fruit_url = server_host + 'play/' + rep_obj[1]
+    if debugmode:
+        fruit_url = FRUIT_URL_TEMPLATE_DEV.format(API_HOST_PLAY_DEV, rep_obj[1])
+    else:
+        fruit_url = FRUIT_URL_TEMPLATE_BETA.format(BETA_VM_API_HOST, rep_obj[1])
 
     pyperclip.copy(fruit_url)
     print(f'URL:{fruit_url} has been copied to the paperclip!')
 
     # new and shiny (ver1 . august23):
     # theFile = EnhancedFile('a.xml', 'r')
     # theUrl = "http://example.com/abcde"
@@ -449,63 +503,112 @@
     # zip_file_path = "path/to/your/file.zip"
     # server_url = "http://example.com/upload.php"
     # response = upload_zip_file(zip_file_path, server_url)
     # print("Response status code:", response.status_code)
     # print("Response content:", response.text)
 
 
-def subcmd_share(bundle_name):
-    # Check if the folder exists, otherwise we'll throw an error
-    wrapper_bundle = fpath_join(os.getcwd(), bundle_name)
-    if not os.path.exists(wrapper_bundle):
-        raise FileNotFoundError('ERR! Cannot find the specified bundle, named:', bundle_name)
-
-    zip_precise_target = fpath_join(wrapper_bundle, 'cartridge')
-    if not os.path.exists(zip_precise_target):
-        raise ValueError('ERR! Seems like you have passed smth that is not a game bundle...')
+def share_subcommand(bundle_name, dev_flag_on):
+    # FIRST, need to answer the question: whats the slug name?
+    metadata = read_metadata(bundle_name)
+    slug = metadata['slug']
+    print('slug found:', slug)
 
     # pre-made func usage
-    source_folder = zip_precise_target
+    wrapper_bundle = os.path.join(os.getcwd(), bundle_name)
+    zip_precise_target = os.path.join(wrapper_bundle, 'cartridge')
 
-    fn = create_zip_from_folder(bundle_name, source_folder)
+    fn = create_zip_from_folder(bundle_name, zip_precise_target)
     # print("ZIP file created:", output_zip_filename)
     # create_zip_from_folder(, os.getcwd())
     # print('tmpfile created ok')
-    upload_my_zip_file(
-        fn,
-        'http://127.0.0.1:8001/'
-    )
+    upload_my_zip_file(fn, slug, dev_flag_on)
+
+
+def upgrade_subcmd(bundlename):
+    """
+    ordre dans lequel l'algo procèdera, idéalement:
+    [1] rebuild le py_connecteur L (local ctx) à la volée, à partir du fichier de SPEC trouvé
+    [2] update des metadata
+    [3] constitution d'un module network avec ledit connecteur renommé en __init__.py,
+    [4] insertion code network vers le chemin bundle/network
+    [5] écrasement launch_game.py par la version moddée
+    """
+    # prép. etapes 2 & 3
+    obj = read_metadata(bundlename)
+    if obj['ktg_services']:
+        print('***WARNING*** ktg_services is already set to True.\n'
+              + 'In order to avoid unexpected behavior, the bundle isnt upgraded')
+        return
+    # tests anticipés pr gérer erreurs:
+    bundle_location = os.path.join(os.getcwd(), bundlename)
+    new_dir = os.path.join(bundle_location, 'network')
+    if os.path.isdir(new_dir):
+        raise Exception('folder "network" exists in bundle, but non-consistent metadata found')
+
+    # étape 2 stricto sensu
+    obj['ktg_services'] = True
+    rewrite_metadata(bundlename, obj)
+
+    # TODO améliorations, avec autogen
+    # etape 3, quasi-ok. Pas implem comme il faudrait (là on récupère un network.py statique)
+    bundle_location = os.path.join(os.getcwd(), bundlename)
+    new_dir = os.path.join(bundle_location, 'network')
+    if os.path.isdir(new_dir):
+        raise Exception('folder "network" exists in bundle, but non-consistent metadata found')
+    os.makedirs(new_dir)
+
+    # etape 4: transfert network component
+    root_pyvcli = os.path.dirname(os.path.abspath(__file__))
+    read_from_netw = os.path.join(root_pyvcli, 'spare_parts', 'network.py')
+    target_file = os.path.join(bundle_location, 'network', '__init__.py')
+    shutil.copy(read_from_netw, target_file)
+
+    # etape 5: impacter launch_game.py
+    copy_launcher_script(bundlename, False)
 
 
 def main_inner(parser, argns):
-    if (not argns.version) and argns.subcommand not in VALID_SUBCOMMANDS:
-        parser.print_help()
-        return 1
+    # definitions
+    subcommand_mapping = {
+        'init': init_command,
+        'test': test_subcommand,
+        'upgrade': upgrade_subcmd,
+        'play': play_subcommand,
+        'share': share_subcommand,
+        'pub': None,
+        'autogen': proc_autogen_localctx
+    }
+    no_arg_subcommands = {'autogen'}
+    extra_flags_subcommands = {'share'}  # mark all subcommands that use the 'dev' mode flag
 
-    if argns.help:
-        parser.print_help()
-        return 0
+    # the algorithm
+    ope_name = argns.subcommand
 
     if argns.version:
-        print('Pyved-engine version %s (c) 2018-2023 the Kata.Games Team: Thomas Iwaszko '
-              'and contributors.' % __version__)
+        print(VERSION_PRINT_MESSAGE % __version__)
         return 0
+    if argns.help:
+        parser.print_help()
+        return 0
+    if ope_name not in subcommand_mapping:
+        parser.print_help()
+        return 1
+    if subcommand_mapping[ope_name] is None:
+        raise NotImplementedError(f"subcommand \"{ope_name}\" is valid, but isnt implemented yet!")
 
-    # handle ``init GameBundleName``
-    if argns.subcommand == "pub":
-        y = trigger_publish(argns.slug, argns.cart_id)
-        return 1 if y else 0
-
-    bundname = argns.bundle_name
-    if argns.subcommand == "init":
-        init_command(bundname)
-    elif argns.subcommand == "play":
-        play_command(bundname)
-    elif argns.subcommand == "share":
-        subcmd_share(bundname)
+    adhoc_subcommand_func = subcommand_mapping[ope_name]
+    if ope_name in no_arg_subcommands:
+        # a few subcommands do not take an argument
+        adhoc_subcommand_func()
+    elif ope_name not in extra_flags_subcommands:
+        adhoc_subcommand_func(argns.bundle_name)
+    else:
+        # a few subcommands require the the dev mode flag!
+        adhoc_subcommand_func(argns.bundle_name, argns.dev)
     return 0
 
     # handle ``pygmentize -L``
     # if argns.L is not None:
     #     arg_set = set()
     #     for k, v in vars(argns).items():
     #         if v:
@@ -859,54 +962,83 @@
     either_one_option = special_modes_group.add_mutually_exclusive_group()
     either_one_option.add_argument(
         '-v', '--version', action='store_true',
         help='Print the current pyved engine version.')
     either_one_option.add_argument(
         '-h', '--help', action='store_true',
         help='Print this help.')
+    either_one_option.add_argument(
+        '-d', '--dev', action='store_true',
+        help='Use the developer server (tool debug etc)'
+    )
 
-    # ----------------
-    #  subcommands
-    # ----------------
+    # Declare all subcommands
     subparsers = parser.add_subparsers(title="Subcommands", dest="subcommand", required=False)
 
+    # ——————————————————————————————————
     # +++ INIT subcommand
     init_parser = subparsers.add_parser("init", help="Initialize something")
     init_parser.add_argument("bundle_name", type=str, help="Name of the bundle")
-    # ——————————————————————————————————
 
+    # ——————————————————————————————————
     # +++ PLAY subcommand
     play_parser = subparsers.add_parser(
         "play", help="Play a given game bundle now!"
     )
     play_parser.add_argument(
         "bundle_name", type=str, nargs="?", default=".", help="Specified bundle (default: current folder)"
     )
+
+    # ——————————————————————————————————
+    # +++ AUTOGEN subcommand
+    autogen = subparsers.add_parser(
+        "autogen", help="Command to be used only by admins ->tool for py connector autogen"
+    )
+
+    # ——————————————————————————————————
+    # +++ UPGRADE subcommand:
+    # the goal here is to enable katagames API calls from inside a game
+    play_parser = subparsers.add_parser(
+        "upgrade", help="Upgrade a given game, to enable katagames API calls"
+    )
+    play_parser.add_argument(
+        "bundle_name", type=str, help="Specified bundle"
+    )
+
     # ——————————————————————————————————
+    # +++ TEST subcommand
+    play_parser = subparsers.add_parser(
+        "test", help="only for debug"
+    )
+    play_parser.add_argument(
+        "bundle_name", type=str
+    )
 
+    # ——————————————————————————————————
     # +++ SHARE subcommand {
     share_parser = subparsers.add_parser(
         "share", help="Share a given game bundle with the world"
     )
     share_parser.add_argument(
         "bundle_name", type=str, nargs="?", default=".", help="Specified bundle (default: current folder)"
     )
+
     # ——————————————————————————————————
+    # +++ PUB subcommand {
     pubpp = subparsers.add_parser(
-        "pub", help="Publish a game based on its cartridge id"
+        "pub", help="Publish a game based on its slug"
     )
     pubpp.add_argument(
-        "slug", type=str, help="Chosen slug (slug means: identifier in the CM system.)"
+        "slug", type=str, help="Chosen slug (slug = cartridge identifier in the cloud-based game warehouse)"
     )
-    pubpp.add_argument(
-        "cart_id", type=str, help="Cartridge id required, as provided by the server"
-    )
-    # +++ PUB subcommand {
 
     ret_args = parser.parse_args()
+    # print('debug:')
+    # print(ret_args)
+    # print()
     main_inner(parser, ret_args)
 
     # flags_only = parser.add_argument_group('Flags')
     # flags_only.add_argument(
     #     '-v', action='store_true',
     #     help='Print out engine version information'
     # )
```

### Comparing `pyved-engine-23.9a5/src/pyvcmdline/template_1/cartridge/gamedef.py` & `pyved-engine-24.3a1/src/pyvcmdline/template_1/cartridge/gamedef.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyvcmdline/template_1/cartridge/systems.py` & `pyved-engine-24.3a1/src/pyvcmdline/template_1/cartridge/systems.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyvcmdline/template_1/cartridge/world.py` & `pyved-engine-24.3a1/src/pyvcmdline/template_1/cartridge/world.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyvcmdline/template_2/cartridge/World.py` & `pyved-engine-24.3a1/src/pyvcmdline/template_2/cartridge/World.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyvcmdline/template_2/cartridge/classes.py` & `pyved-engine-24.3a1/src/pyvcmdline/template_2/cartridge/classes.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyvcmdline/template_2/cartridge/gamedef.py` & `pyved-engine-24.3a1/src/pyvcmdline/template_2/cartridge/gamedef.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyvcmdline/template_2/cartridge/systems.py` & `pyved-engine-24.3a1/src/pyvcmdline/template_2/cartridge/systems.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/ChessGUI_text.py` & `pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/ChessGUI_text.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/ChessGameParams.py` & `pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/ChessGameParams.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/ChessmatchMod.py` & `pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/ChessmatchMod.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/PythonChessAIStats.py` & `pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/PythonChessAIStats.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/ScrollingTextBox.py` & `pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/ScrollingTextBox.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/ai_players.py` & `pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/ai_players.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/black_bishop.png` & `pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/black_bishop.png`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/black_king.png` & `pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/black_king.png`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/black_knight.png` & `pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/black_knight.png`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/black_pawn.png` & `pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/black_pawn.png`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/black_queen.png` & `pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/black_queen.png`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/black_rook.png` & `pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/black_rook.png`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/chdefs.py` & `pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/chdefs.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/chess_rules.py` & `pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/chess_rules.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/chessintro.py` & `pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/chessintro.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/chessmatch.py` & `pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/chessmatch.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/cyan_square.png` & `pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/cyan_square.png`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/gamedef.py` & `pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/gamedef.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/main_gui_view.py` & `pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/main_gui_view.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/misc.py` & `pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/misc.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/model.py` & `pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/model.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/white_bishop.png` & `pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/white_bishop.png`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/white_king.png` & `pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/white_king.png`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/white_knight.png` & `pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/white_knight.png`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/white_pawn.png` & `pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/white_pawn.png`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/white_queen.png` & `pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/white_queen.png`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyvcmdline/template_3/cartridge/white_rook.png` & `pyved-engine-24.3a1/src/pyvcmdline/template_3/cartridge/white_rook.png`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyvcmdline/template_4/cartridge/CC0 License.txt` & `pyved-engine-24.3a1/src/pyvcmdline/template_4/cartridge/CC0 License.txt`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyvcmdline/template_4/cartridge/avatar1.png` & `pyved-engine-24.3a1/src/pyvcmdline/template_4/cartridge/avatar1.png`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyvcmdline/template_4/cartridge/gamedef.py` & `pyved-engine-24.3a1/src/pyvcmdline/template_4/cartridge/gamedef.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from . import pimodules
 from .mvc_parts import NinjamazeMod, NinjamazeView, NinjamazeCtrl, SpecificEvTypes
+from . import glvars
 
 
 pyv = pimodules.pyved_engine
 EngineEvTypes = pyv.EngineEvTypes
 
 
 def print_help():
@@ -18,23 +19,41 @@
 @pyv.Singleton
 class MiniStorage:
     def __init__(self):
         self.ev_manager = pyv.get_ev_manager()
         self.ev_manager.setup(SpecificEvTypes)
         self.screen = pyv.get_surface()
 
+class DummyDisp(pyv.EvListener):
+    def __init__(self,color):
+        super().__init__()
+        self.col = color
+    
+    def on_paint(self, ev):
+        ev.screen.fill(self.col)
+
 
 @pyv.declare_begin
 def rogue_begin(vms=None):
     pyv.init(wcaption='roguelike template')
+    # bind obj to glvars
+    glvars.avatar_sprite_sheet = pyv.vars.spritesheets['smallninja_sprites']
+
     MiniStorage.instance()  # by doing this, we also init the ev_manager
     m = NinjamazeMod()
-    # be careful: you wont be able to instantiate the View if the ev_manager isnt ready
-    NinjamazeView(m).turn_on()
+ 
+    # Careful:
+    # you wont be able to instantiate the View if the ev_manager isnt ready
+    v = NinjamazeView(m)
+    # *debugging
+    # v = DummyDisp('pink')
+    v.turn_on()
+
     NinjamazeCtrl(m).turn_on()
+
     print_help()  # so the player knows how to "play"
 
 
 @pyv.declare_update
 def rogue_update(info_t=None):
     gvars = MiniStorage.instance()
     gvars.ev_manager.post(EngineEvTypes.Update, curr_t=info_t)
```

### Comparing `pyved-engine-23.9a5/src/pyvcmdline/template_4/cartridge/mvc_parts.py` & `pyved-engine-24.3a1/src/pyvcmdline/template_4/cartridge/mvc_parts.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 this file contains 3 basic mvc COMPOnents
 that can implement a rogue-like
 """
 from . import pimodules
-
+from . import glvars
 pyv = pimodules.pyved_engine
 pyv.bootstrap_e()
 
 
 pygame = pyv.pygame
 EngineEvTypes = pyv.EngineEvTypes
 CogObject = pyv.Emitter
@@ -119,46 +119,58 @@
     THE VIEW
     """
     CELL_SIDE = 32  # px
     WALL_COLOR = (8, 8, 24)
     HIDDEN_CELL_COLOR = (24, 24, 24)
 
     def __init__(self, ref_mod):
+        print('------------------------ dans NinjamazeView !! --------------------------------')
+        print()
         super().__init__()
         self.assoc_r_col = dict()
         grid_rez = (32, 32)
 
         img = pyv.vars.images['tileset']
+        print('etape 0')
         self.tileset = Sprsheet(img, 2)  # use upscaling x2
+        print('etape 1')
         self.tileset.set_infos(grid_rez)
+        print('etape 2')
 
-        img = pyv.vars.images['avatar1']
-        self.planche_avatar = Sprsheet(img, 2)  # upscaling x2
-        self.planche_avatar.set_infos(grid_rez)
-        self.planche_avatar.colorkey = (255, 0, 255)
-
+        # img = pyv.vars.images['avatar1']
+        # self.planche_avatar = Sprsheet(img, 2)  # upscaling x2
+        # self.planche_avatar.set_infos(grid_rez)
+        # self.planche_avatar.colorkey = (255, 0, 255)
+        flashy_pink = (255, 0, 255)
         self.monster_img = pyv.vars.images['monster']
-        self.monster_img = pygame.transform.scale(self.monster_img, (32, 32))
-        self.monster_img.set_colorkey((255, 0, 255))
+        # self.monster_img = pygame.transform.scale(self.monster_img, (32, 32))
+        # self.monster_img.set_colorkey(flashy_pink)
 
         self.mod = ref_mod
-        self.avatar_apparence = self.planche_avatar.image_by_rank(0)
+        print('*** avant planche_avatar.image_by_rank !!! ')
+        print()
+        self.avatar_apparence = glvars.avatar_sprite_sheet['av0.png']
+        # self.avatar_apparence.set_colorkey(flashy_pink)
+        # self.avatar_apparence = self.planche_avatar.image_by_rank(0)
+        print('*** ok c bon')
+
         self.pos_avatar = ref_mod.get_av_pos()
 
     def on_player_moves(self, ev):  # custom event hook
         self.pos_avatar = ev.new_pos
 
     def on_paint(self, ev):  # engine ev type hook
         scr = ev.screen
         scr.fill(self.WALL_COLOR)
 
         nw_corner = (0, 0)
         tmp_r4 = [None, None, None, None]
 
-        tuile = self.tileset.image_by_rank(912)
+        # TODO recup image depuis le tilesheet et l'upscale x 2 à la mano
+        # tuile = self.tileset.image_by_rank(912)
 
         dim = self.mod.get_terrain().get_size()
         for i in range(dim[0]):
             for j in range(dim[1]):
                 # ignoring walls
                 tmp = self.mod.get_terrain().get_val(i, j)
                 if tmp is None:
@@ -167,28 +179,34 @@
                 tmp_r4[0], tmp_r4[1] = nw_corner
                 tmp_r4[0] += i * self.CELL_SIDE
                 tmp_r4[1] += j * self.CELL_SIDE
                 tmp_r4[2] = tmp_r4[3] = self.CELL_SIDE
                 if not self.mod.can_see((i, j)):  # hidden cell
                     pygame.draw.rect(scr, self.HIDDEN_CELL_COLOR, tmp_r4)
                 else:  # visible tile
-                    scr.blit(tuile, tmp_r4)
+                    pygame.draw.rect(scr, pyv.pal.punk['green'], tmp_r4)
 
-        # draw avatar process
-        av_i, av_j = self.pos_avatar[0] * self.CELL_SIDE, self.pos_avatar[1] * self.CELL_SIDE
-        scr.blit(self.avatar_apparence, (av_i, av_j, 32, 32))
+                    # scr.blit(tuile, tmp_r4)
+                    # scr.blit(tuile, (tmp_r4[0], tmp_r4[1]))#, tmp_r4)
+                    # pass
 
         # draw enemies
         for enemy_info in self.mod.enemies_pos2type.items():
             pos, t = enemy_info
             if not self.mod.visibility_m.get_val(*pos):
                 continue
             en_i, en_j = pos[0] * self.CELL_SIDE, pos[1] * self.CELL_SIDE
+            # pass
             scr.blit(self.monster_img, (en_i, en_j, 32, 32))
 
+        # draw avatar process
+        av_x, av_y = self.pos_avatar[0] * self.CELL_SIDE, self.pos_avatar[1] * self.CELL_SIDE
+        # scr.blit(self.avatar_apparence, (av_i, av_j, 32, 32))
+        scr.blit(self.avatar_apparence, (av_x, av_y))
+
 
 class NinjamazeCtrl(ReceiverObj):
     """
     THE CONTROLLER
     """
     def __init__(self, ref_mod):
         super().__init__()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyved-engine-23.9a5/src/pyvcmdline/template_4/cartridge/tileset.png` & `pyved-engine-24.3a1/src/pyvcmdline/template_4/cartridge/tileset.png`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/Singleton.py` & `pyved-engine-24.3a1/src/pyved_engine/Singleton.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/__init__.py` & `pyved-engine-24.3a1/src/pyved_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/_classes.py` & `pyved-engine-24.3a1/src/pyved_engine/_classes.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/_ecs.py` & `pyved-engine-24.3a1/src/pyved_engine/_ecs.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/_ecs_pattern.py` & `pyved-engine-24.3a1/src/pyved_engine/_ecs_pattern.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/_hub.py` & `pyved-engine-24.3a1/src/pyved_engine/_hub.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/_pyv_implem.py` & `pyved-engine-24.3a1/src/pyved_engine/_pyv_implem.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/_utility.py` & `pyved-engine-24.3a1/src/pyved_engine/_utility.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/add_ons/gui/BaseGuiElement.py` & `pyved-engine-24.3a1/src/pyved_engine/add_ons/gui/BaseGuiElement.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/add_ons/gui/Button.py` & `pyved-engine-24.3a1/src/pyved_engine/add_ons/gui/Button.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/add_ons/gui/Button2.py` & `pyved-engine-24.3a1/src/pyved_engine/add_ons/gui/Button2.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/add_ons/gui/DispCenteredPopup.py` & `pyved-engine-24.3a1/src/pyved_engine/add_ons/gui/DispCenteredPopup.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/add_ons/gui/DispPopup.py` & `pyved-engine-24.3a1/src/pyved_engine/add_ons/gui/DispPopup.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/add_ons/gui/Label.py` & `pyved-engine-24.3a1/src/pyved_engine/add_ons/gui/Label.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/add_ons/gui/TextBlock.py` & `pyved-engine-24.3a1/src/pyved_engine/add_ons/gui/TextBlock.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/add_ons/gui/Trigger.py` & `pyved-engine-24.3a1/src/pyved_engine/add_ons/gui/Trigger.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/add_ons/gui/WidgetBo.py` & `pyved-engine-24.3a1/src/pyved_engine/add_ons/gui/WidgetBo.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/add_ons/gui/WidgetContainer.py` & `pyved-engine-24.3a1/src/pyved_engine/add_ons/gui/WidgetContainer.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/add_ons/gui/__init__.py` & `pyved-engine-24.3a1/src/pyved_engine/add_ons/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/add_ons/gui/base.py` & `pyved-engine-24.3a1/src/pyved_engine/add_ons/gui/base.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/add_ons/gui/text.py` & `pyved-engine-24.3a1/src/pyved_engine/add_ons/gui/text.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/data.py` & `pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/data.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/misc.py` & `pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/misc.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/__init__.py` & `pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/common_types.py` & `pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/common_types.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/layer.py` & `pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/layer.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/parser.py` & `pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/parser.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/json/layer.py` & `pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/json/layer.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/json/properties.py` & `pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/json/properties.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/json/tiled_map.py` & `pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/json/tiled_map.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/json/tiled_object.py` & `pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/json/tiled_object.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/json/tileset.py` & `pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/json/tileset.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/json/wang_set.py` & `pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/json/wang_set.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/tmx/layer.py` & `pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/tmx/layer.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/tmx/properties.py` & `pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/tmx/properties.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/tmx/tiled_map.py` & `pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/tmx/tiled_map.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/tmx/tiled_object.py` & `pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/tmx/tiled_object.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/tmx/tileset.py` & `pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/tmx/tileset.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/tmx/wang_set.py` & `pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/parsers/tmx/wang_set.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/tiled_map.py` & `pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/tiled_map.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/tiled_object.py` & `pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/tiled_object.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/tileset.py` & `pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/tileset.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/util.py` & `pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/util.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/wang_set.py` & `pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/wang_set.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/pytiled_parser/world.py` & `pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/pytiled_parser/world.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/add_ons/tmx/ztilemap.py` & `pyved-engine-24.3a1/src/pyved_engine/add_ons/tmx/ztilemap.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/api.py` & `pyved-engine-24.3a1/src/pyved_engine/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,20 +168,32 @@
 
 def declare_end(gfunc):  # decorator!
     vars.endfunc_ref = gfunc
     return gfunc
 
 
 def run_game():
-    vars.beginfunc_ref(None)
-    while not vars.gameover:
-        vars.updatefunc_ref(time.time())
-        flip()  # commit gfx mem to screen, already contains the .tick
-    vars.endfunc_ref(None)
+    if __import__('sys').platform in ('emscripten','wasi'):
+        import asyncio
+        async def async_run_game():
+            vars.beginfunc_ref(None)
+            while not vars.gameover:
+                vars.updatefunc_ref(time.time())
+                flip()  # commit gfx mem to screen, already contains the .tick
+                await asyncio.sleep(0)
+            vars.endfunc_ref(None)
 
+        asyncio.run( async_run_game() )
+    else:
+        vars.beginfunc_ref(None)
+        while not vars.gameover:
+            vars.updatefunc_ref(time.time())
+            flip()  # commit gfx mem to screen, already contains the .tick
+        vars.endfunc_ref(None)
+      
 
 # --- rest of functions ---
 def preload_assets(adhoc_dict: dict, prefix_asset_folder=None, webhack=None):
     """
     expected to find the (mandatory) key 'images',
     also we may find the (optionnal) key 'sounds'
     :param prefix_asset_folder:
```

### Comparing `pyved-engine-23.9a5/src/pyved_engine/classes.py` & `pyved-engine-24.3a1/src/pyved_engine/classes.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/compo/gfx.py` & `pyved-engine-24.3a1/src/pyved_engine/compo/gfx.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/compo/modes.py` & `pyved-engine-24.3a1/src/pyved_engine/compo/modes.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/compo/packed_capello_ft.py` & `pyved-engine-24.3a1/src/pyved_engine/compo/packed_capello_ft.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/compo/vscreen.py` & `pyved-engine-24.3a1/src/pyved_engine/compo/vscreen.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/core/Injector.py` & `pyved-engine-24.3a1/src/pyved_engine/core/Injector.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/core/events.py` & `pyved-engine-24.3a1/src/pyved_engine/core/events.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/core_classes.py` & `pyved-engine-24.3a1/src/pyved_engine/core_classes.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/custom_struct.py` & `pyved-engine-24.3a1/src/pyved_engine/custom_struct.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/foundation/defs.py` & `pyved-engine-24.3a1/src/pyved_engine/foundation/defs.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/foundation/interfaces.py` & `pyved-engine-24.3a1/src/pyved_engine/foundation/interfaces.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
-code (c) 2018-2022, by Thomas Iwaszko
-contact - tom@kata.games
+Licensed code LGPL 3
+(c) 2018-2024, to the Kata.Games company
 
-TL;DR - KENGI does not use 100% of pygame capabilities. How much of pygame do we use?
+TL;DR - Pyved is not using 100% of pygame functions.
+So how much of pygame do we use?
 
 More precisely: this file is here so I can:
 (A) specify (for this I propose an informal interface) a SUBSET of pygame
 
 (B) offer a formal interface for the so-called "PRIMAL backend". Such a backend can
 be implemented in various ways. Interestingly, one possible way is to use a SUBSET of pygame.
 Since I consider that it wouldn't be great to use a subset of pygame without "exposing" it
```

### Comparing `pyved-engine-23.9a5/src/pyved_engine/foundation/pbackends.py` & `pyved-engine-24.3a1/src/pyved_engine/foundation/pbackends.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/legacy_event.py` & `pyved-engine-24.3a1/src/pyved_engine/legacy_event.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/legacy_init.py` & `pyved-engine-24.3a1/src/pyved_engine/legacy_init.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/legacy_version.py` & `pyved-engine-24.3a1/src/pyved_engine/legacy_version.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/looparts/ai/FSA_classes_base.py` & `pyved-engine-24.3a1/src/pyved_engine/looparts/ai/FSA_classes_base.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/looparts/ai/NorrecBrain.py` & `pyved-engine-24.3a1/src/pyved_engine/looparts/ai/NorrecBrain.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/looparts/ai/tests.py` & `pyved-engine-24.3a1/src/pyved_engine/looparts/ai/tests.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/looparts/anim.py` & `pyved-engine-24.3a1/src/pyved_engine/looparts/anim.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/looparts/ascii.py` & `pyved-engine-24.3a1/src/pyved_engine/looparts/ascii.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/looparts/console.py` & `pyved-engine-24.3a1/src/pyved_engine/looparts/console.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/looparts/demolib/animobs.py` & `pyved-engine-24.3a1/src/pyved_engine/looparts/demolib/animobs.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/looparts/demolib/dialogue.py` & `pyved-engine-24.3a1/src/pyved_engine/looparts/demolib/dialogue.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/looparts/demolib/pathfinding.py` & `pyved-engine-24.3a1/src/pyved_engine/looparts/demolib/pathfinding.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/looparts/demolib/rpgmenu.py` & `pyved-engine-24.3a1/src/pyved_engine/looparts/demolib/rpgmenu.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/looparts/rogue.py` & `pyved-engine-24.3a1/src/pyved_engine/looparts/rogue.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-import random
 import math
+import random
+
 from .. import e_struct as struct
 
 
 # ----------------------------
 #  random map generation tool
 # ----------------------------
 SYM_UP, SYM_DOWN, SYM_LEFT, SYM_RIGHT = range(4)
@@ -55,14 +56,16 @@
     Elle permet de récupérer une matrice (objet type IntegerMatrix) constante et adéquate
     pour le but recherché (disposer dun labyrinthe différent à chaque fois)
     via la méthode RandomMaze.getMatrix
     """
     def __init__(self, w, h, min_room_size, max_room_size, density_factor=140):
         self.int_matrix = struct.IntegerMatrix((w, h))
         self.int_matrix.set_all(None)  # super important! Otherwise the algorithm wont work
+        self.blocking_map = struct.BoolMatrix((w, h))
+        self.blocking_map.set_all(True)  # by default, all is blocking
 
         self.room_possib_size = list()
 
         for i in range(min_room_size, max_room_size + 1):
             if i % 2 == 0:  # choix dune taille impaire nécessairement
                 continue
             self.room_possib_size.append(i)
@@ -99,14 +102,20 @@
         while self.canMerge():
             self.stepMerge()
 
         # (4) suppr. cul-de-sac
         self.tested_pos = set()
         self.recUncarve((1, 1))
 
+        # --- post-processing step: sync the data in self.blocking_map
+        for i in range(dim[0]):
+            for j in range(dim[1]):
+                if self.int_matrix.get_val(i, j):
+                    self.blocking_map.set_val(i, j, False)
+
     def pick_walkable_cell(self):
         # helps choosing a valid initial position for the avatar
         floor = self.int_matrix
         w, h = floor.get_size()
         chosen_pos = [
             random.randint(0, w-1),
             random.randint(0, h-1)
```

### Comparing `pyved-engine-23.9a5/src/pyved_engine/looparts/rpg.py` & `pyved-engine-24.3a1/src/pyved_engine/looparts/rpg.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/looparts/sysconsole.py` & `pyved-engine-24.3a1/src/pyved_engine/looparts/sysconsole.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/looparts/tabletop.py` & `pyved-engine-24.3a1/src/pyved_engine/looparts/tabletop.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/looparts/terrain.py` & `pyved-engine-24.3a1/src/pyved_engine/looparts/terrain.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/pal.py` & `pyved-engine-24.3a1/src/pyved_engine/pal.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/state_management.py` & `pyved-engine-24.3a1/src/pyved_engine/state_management.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/tankui.py` & `pyved-engine-24.3a1/src/pyved_engine/tankui.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/util.py` & `pyved-engine-24.3a1/src/pyved_engine/util.py`

 * *Files identical despite different names*

### Comparing `pyved-engine-23.9a5/src/pyved_engine/vars.py` & `pyved-engine-24.3a1/src/pyved_engine/vars.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 WARNING: Although these variables can be accesed directly, it is NOT recommended
 to tweak these values manually.
 Unexpected outcomes/side-effects could be produced by doing so.
 Instead use functions like pyv.preload_assets(...) or init(max_fps=..., ...) etc.
 """
 
 
-ENGINE_VERSION_STR = '23.9a5'  # a read-only value, can this val. from outside via a func. call on pyv.get_version()
+ENGINE_VERSION_STR = '24.3a1'  # a read-only value, can this val. from outside via a func. call on pyv.get_version()
 
 # deprecated but mandatory for web ctx
 STD_SCR_SIZE = [960, 720]
 
 # - engine related
 disp_size = [960, 720]
```

### Comparing `pyved-engine-23.9a5/src/pyved_engine.egg-info/PKG-INFO` & `pyved-engine-24.3a1/src/pyved_engine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pyved-engine
-Version: 23.9a5
+Version: 24.3a1
 Summary: Custom game engine built upon python/pygame
 Home-page: https://github.com/gaudiatech/pyved-engine
 Author: moonb3ndr et al.
 Author-email: thomas.iw@kata.games
 License: LGPL3
 Keywords: Python,Pygame,Game Engine
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pygame-ce>=2.2.1
 Requires-Dist: pyperclip>=1.8.2
 Requires-Dist: requests>=2.28.1
 
 <p align="center">
-  <img src="https://gaudia-tech.com/shared/pyv-logo.jpg" alt="pyv logo" />
+  <img src="https://www.gaudia-tech.com/mirror/pyv-logo.jpg" alt="pyv logo" />
 </p>
 
 Introducing `pyved-engine`, a Python package that provides you with
 the versatile, efficient 2D game engine named PYV!
 Designed to streamline game development, PYV offers a set of
 tools for smooth and rapid game prototyping.
 
@@ -31,15 +31,15 @@
 </a>
 </p>
 
 
 
 ## 1. Introduction
 
-### Cpabilities of a game engine
+### Capabilities of a game engine
 
 A game engine provides invaluable time-saving benefits by storing a collection
 of useful and reusable code snippets within its framework.
 Instead of reinventing the wheel and wasting your precious time by re-writing
 generic code for video games, you can leverage the power of the engine.
 
 By referring to the
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: pyved-engine Version: 23.9a5 Summary: Custom game
+Metadata-Version: 2.1 Name: pyved-engine Version: 24.3a1 Summary: Custom game
 engine built upon python/pygame Home-page: https://github.com/gaudiatech/pyved-
 engine Author: moonb3ndr et al. Author-email: thomas.iw@kata.games License:
 LGPL3 Keywords: Python,Pygame,Game Engine Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: pygame-ce>=2.2.1 Requires-Dist:
 pyperclip>=1.8.2 Requires-Dist: requests>=2.28.1
                                   [pyv logo]
 Introducing `pyved-engine`, a Python package that provides you with the
 versatile, efficient 2D game engine named PYV! Designed to streamline game
 development, PYV offers a set of tools for smooth and rapid game prototyping.
 Unlock the full potential of your game development thanks to __pyv__!
                         _T_o_ _j_o_i_n_ _o_u_r_ _D_i_s_c_o_r_d_ _c_o_m_m_u_n_i_t_y_:
                              _[_j_o_i_n_ _u_s_ _o_n_ _D_i_s_c_o_r_d_]
-## 1. Introduction ### Cpabilities of a game engine A game engine provides
+## 1. Introduction ### Capabilities of a game engine A game engine provides
 invaluable time-saving benefits by storing a collection of useful and reusable
 code snippets within its framework. Instead of reinventing the wheel and
 wasting your precious time by re-writing generic code for video games, you can
 leverage the power of the engine. By referring to the [work-in-progress
 documentation](https://gaudiatech.github.io/pyved-engine/), you could quickly
 learn how to implement various functionalities such as pathfinding or loading
 spritesheets. With simple function or method calls, you can seamlessly
```

### Comparing `pyved-engine-23.9a5/src/pyved_engine.egg-info/SOURCES.txt` & `pyved-engine-24.3a1/src/pyved_engine.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 src/pyvcmdline/__init__.py
 src/pyvcmdline/__main__.py
+src/pyvcmdline/const.py
 src/pyvcmdline/json_prec.py
-src/pyvcmdline/launch_game.py
+src/pyvcmdline/pyvcli_config.py
 src/pyvcmdline/emb_demos/__init__.py
 src/pyvcmdline/emb_demos/my_demo1.py
 src/pyvcmdline/template_0/cartridge/__init__.py
 src/pyvcmdline/template_0/cartridge/gamedef.py
 src/pyvcmdline/template_0/cartridge/pimodules.py
 src/pyvcmdline/template_1/cartridge/__init__.py
 src/pyvcmdline/template_1/cartridge/gamedef.py
@@ -21,14 +22,16 @@
 src/pyvcmdline/template_2/cartridge/__init__.py
 src/pyvcmdline/template_2/cartridge/classes.py
 src/pyvcmdline/template_2/cartridge/gamedef.py
 src/pyvcmdline/template_2/cartridge/my_map.ncsv
 src/pyvcmdline/template_2/cartridge/pimodules.py
 src/pyvcmdline/template_2/cartridge/shared.py
 src/pyvcmdline/template_2/cartridge/systems.py
+src/pyvcmdline/template_2/cartridge/thumb_1.png
+src/pyvcmdline/template_2/cartridge/thumb_2.png
 src/pyvcmdline/template_3/cartridge/ChessGUI_text.py
 src/pyvcmdline/template_3/cartridge/ChessGameParams.py
 src/pyvcmdline/template_3/cartridge/ChessmatchMod.py
 src/pyvcmdline/template_3/cartridge/PythonChessAIStats.py
 src/pyvcmdline/template_3/cartridge/ScrollingTextBox.py
 src/pyvcmdline/template_3/cartridge/__init__.py
 src/pyvcmdline/template_3/cartridge/ai_players.py
@@ -47,29 +50,35 @@
 src/pyvcmdline/template_3/cartridge/gamedef.py
 src/pyvcmdline/template_3/cartridge/info-assets.txt
 src/pyvcmdline/template_3/cartridge/main_gui_view.py
 src/pyvcmdline/template_3/cartridge/misc.py
 src/pyvcmdline/template_3/cartridge/model.py
 src/pyvcmdline/template_3/cartridge/pimodules.py
 src/pyvcmdline/template_3/cartridge/run_chess.py
+src/pyvcmdline/template_3/cartridge/thumb_1.png
+src/pyvcmdline/template_3/cartridge/thumb_2.png
 src/pyvcmdline/template_3/cartridge/white_bishop.png
 src/pyvcmdline/template_3/cartridge/white_king.png
 src/pyvcmdline/template_3/cartridge/white_knight.png
 src/pyvcmdline/template_3/cartridge/white_pawn.png
 src/pyvcmdline/template_3/cartridge/white_queen.png
 src/pyvcmdline/template_3/cartridge/white_rook.png
 src/pyvcmdline/template_3/cartridge/white_square.png
 src/pyvcmdline/template_4/cartridge/CC0 License.txt
 src/pyvcmdline/template_4/cartridge/__init__.py
 src/pyvcmdline/template_4/cartridge/avatar1.png
 src/pyvcmdline/template_4/cartridge/gamedef.py
+src/pyvcmdline/template_4/cartridge/glvars.py
 src/pyvcmdline/template_4/cartridge/info.txt
 src/pyvcmdline/template_4/cartridge/monster.png
 src/pyvcmdline/template_4/cartridge/mvc_parts.py
 src/pyvcmdline/template_4/cartridge/pimodules.py
+src/pyvcmdline/template_4/cartridge/smallninja_sprites.png
+src/pyvcmdline/template_4/cartridge/thumb_1.png
+src/pyvcmdline/template_4/cartridge/thumb_2.png
 src/pyvcmdline/template_4/cartridge/tileset.png
 src/pyved_engine/Singleton.py
 src/pyved_engine/__init__.py
 src/pyved_engine/_classes.py
 src/pyved_engine/_ecs.py
 src/pyved_engine/_ecs_pattern.py
 src/pyved_engine/_hub.py
```

### Comparing `pyved-engine-23.9a5/tests/test_engine.py` & `pyved-engine-24.3a1/tests/test_engine.py`

 * *Files identical despite different names*

