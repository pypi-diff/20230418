# Comparing `tmp/arlq-1.2.0.tar.gz` & `tmp/arlq-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arlq-1.2.0.tar", last modified: Mon Apr 17 12:40:05 2023, max compression
+gzip compressed data, was "arlq-1.2.1.tar", last modified: Tue Apr 18 12:12:29 2023, max compression
```

## Comparing `arlq-1.2.0.tar` & `arlq-1.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2023-04-17 12:40:05.617907 arlq-1.2.0/
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     1305 2023-04-14 17:26:18.000000 arlq-1.2.0/LICENSE
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     1046 2023-04-17 12:40:05.617907 arlq-1.2.0/PKG-INFO
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     4375 2023-04-17 11:28:51.000000 arlq-1.2.0/README.md
-drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2023-04-17 12:40:05.617907 arlq-1.2.0/arlq/
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       57 2023-04-14 17:26:18.000000 arlq-1.2.0/arlq/__init__.py
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       22 2023-04-16 12:23:10.000000 arlq-1.2.0/arlq/_version.py
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)    21720 2023-04-17 11:56:08.000000 arlq-1.2.0/arlq/arlq.py
-drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2023-04-17 12:40:05.617907 arlq-1.2.0/arlq.egg-info/
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     1046 2023-04-17 12:40:05.000000 arlq-1.2.0/arlq.egg-info/PKG-INFO
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)      253 2023-04-17 12:40:05.000000 arlq-1.2.0/arlq.egg-info/SOURCES.txt
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)        1 2023-04-17 12:40:05.000000 arlq-1.2.0/arlq.egg-info/dependency_links.txt
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       36 2023-04-17 12:40:05.000000 arlq-1.2.0/arlq.egg-info/entry_points.txt
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       43 2023-04-17 12:40:05.000000 arlq-1.2.0/arlq.egg-info/requires.txt
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)        5 2023-04-17 12:40:05.000000 arlq-1.2.0/arlq.egg-info/top_level.txt
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)      836 2023-04-17 12:40:05.617907 arlq-1.2.0/setup.cfg
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       38 2023-04-14 17:26:18.000000 arlq-1.2.0/setup.py
+drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2023-04-18 12:12:29.971434 arlq-1.2.1/
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     1305 2023-04-14 17:26:18.000000 arlq-1.2.1/LICENSE
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     1046 2023-04-18 12:12:29.971434 arlq-1.2.1/PKG-INFO
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     4375 2023-04-17 16:10:09.000000 arlq-1.2.1/README.md
+drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2023-04-18 12:12:29.971434 arlq-1.2.1/arlq/
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       57 2023-04-14 17:26:18.000000 arlq-1.2.1/arlq/__init__.py
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       22 2023-04-18 04:07:02.000000 arlq-1.2.1/arlq/_version.py
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)    22524 2023-04-18 12:12:02.000000 arlq-1.2.1/arlq/arlq.py
+drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2023-04-18 12:12:29.971434 arlq-1.2.1/arlq.egg-info/
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     1046 2023-04-18 12:12:29.000000 arlq-1.2.1/arlq.egg-info/PKG-INFO
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)      253 2023-04-18 12:12:29.000000 arlq-1.2.1/arlq.egg-info/SOURCES.txt
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)        1 2023-04-18 12:12:29.000000 arlq-1.2.1/arlq.egg-info/dependency_links.txt
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       36 2023-04-18 12:12:29.000000 arlq-1.2.1/arlq.egg-info/entry_points.txt
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       43 2023-04-18 12:12:29.000000 arlq-1.2.1/arlq.egg-info/requires.txt
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)        5 2023-04-18 12:12:29.000000 arlq-1.2.1/arlq.egg-info/top_level.txt
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)      836 2023-04-18 12:12:29.971434 arlq-1.2.1/setup.cfg
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       38 2023-04-14 17:26:18.000000 arlq-1.2.1/setup.py
```

### Comparing `arlq-1.2.0/LICENSE` & `arlq-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arlq-1.2.0/PKG-INFO` & `arlq-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arlq
-Version: 1.2.0
+Version: 1.2.1
 Summary: ARQL, another rogue-like quest game.
 Home-page: https://github.com/tos-kamiya/arlq
 Author: Toshihiro Kamiya
 Author-email: kamiya@mbj.nifty.com
 License: BSD 2-Clause License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `arlq-1.2.0/README.md` & `arlq-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `arlq-1.2.0/arlq/arlq.py` & `arlq-1.2.1/arlq/arlq.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,49 +7,51 @@
 import time
 
 try:
     from ._version import __version__
 except:
     __version__ = "(unknown)"
 
-ROOM_WIDTH = 5
-ROOM_HEIGHT = 4
-ROOM_NUM_X = 12
-ROOM_NUM_Y = 4
-FIELD_WIDTH = (ROOM_WIDTH + 1) * ROOM_NUM_X + 1
-FIELD_HEIGHT = (ROOM_HEIGHT + 1) * ROOM_NUM_Y + 1
+
+TILE_WIDTH = 5
+TILE_HEIGHT = 4
+TILE_NUM_X = 12
+TILE_NUM_Y = 4
+FIELD_WIDTH = (TILE_WIDTH + 1) * TILE_NUM_X + 1
+FIELD_HEIGHT = (TILE_HEIGHT + 1) * TILE_NUM_Y + 1
 CORRIDOR_V_WIDTH = 3
 CORRIDOR_H_WIDTH = 2
 WALL_CHARS = "###"  # cross, horizontal, vertical
 
-FOOD_MAX = 120
+FOOD_MAX = 100
 FOOD_INIT = 90
 FOOD_STARVATION = 30
 
-FOOD_BISON = 40
-FOOD_SPECIAL_BISON = 80
-FOOD_AMOEBA = 8
-FOOD_CHIMERA = 8
-FOOD_COMODO_DRAGON = 30
-FOOD_DRAGON = 10
-FOOD_ELEMENTAL = 0
-FOOD_GORGON = -48
+FEED_BISON = 30
+FEED_RARE_BISON = 60
+FEED_AMOEBA = 5
+FEED_CHIMERA = 8
+FEED_COMODO_DRAGON = 30
+FEED_DRAGON = 10
+FEED_ELEMENTAL = 0
+FEED_GORGON = -48
 
-ITEM_BISON_MEAT = "Bison Meat"
 ITEM_SWORD = "Sword"
 ITEM_POISONED = "Poisoned"
-ITEM_RANDOM_TRANSPORT = "Random Trans."
-ITEM_SPECIAL_EXP = "Special Exp."
-ITEM_SPECIAL_BISON_MEAT = "Bison Meat++"
-ITEM_SWORD_AND_CLAIRVOYANCE = "Sword & Eye"
-ITEM_TREASURE_POINTER = "Treasure Ptr."
-ITEM_STONED = "Stoned"
 ITEM_TREASURE = "Treasure"
 
+EFFECT_SPECIAL_EXP = "Special Exp."
+EFFECT_FEED_MUCH = "Bison Meat"
+EFFECT_RANDOM_TRANSPORT = "Random Trans."
+EFFECT_CLAIRVOYANCE = "Sword & Eye"
+EFFECT_TREASURE_POINTER = "Treasure Ptr."
+EFFECT_STONED = "Stoned"
+
 COMPANION_FAIRY = "Fairy"
+FAIRY_TORCH_EXTENSION = 2
 
 CHAR_DRAGON = "D"
 CHAR_TREASURE = "T"
 
 
 Point = Tuple[int, int]
 Edge = Tuple[Point, Point]
@@ -84,15 +86,15 @@
     # Initialize the maze generation process
     unconnected_point_set = set((x, y) for y in range(height) for x in range(width))
     connecting_points = []
     done_points = []
     edges = []
 
     # Choose a random starting point
-    cur_p = rand.choice(list(unconnected_point_set))
+    first_point = cur_p = rand.choice(list(unconnected_point_set))
     unconnected_point_set.remove(cur_p)
     connecting_points.append(cur_p)
 
     # Keep generating until all points have been connected
     while len(done_points) < width * height:
         # Choose a random connecting point
         i = rand.randrange(len(connecting_points))
@@ -105,23 +107,23 @@
         # If there are no unconnected neighboring points, remove this point from the connecting points list
         if not unconnected_nps:
             done_points.append(cur_p)
             del connecting_points[i]
             continue
 
         # Choose a random unconnected neighboring point and connect it
-        selected_np = rand.choice(unconnected_nps)
+        last_point = selected_np = rand.choice(unconnected_nps)
         unconnected_point_set.remove(selected_np)
         connecting_points.append(selected_np)
 
         # Add the edge between the current point and the selected neighboring point to the list of edges
         edges.append((cur_p, selected_np))
 
     # Return the list of edges that connect all points in the maze
-    return edges
+    return edges, first_point, last_point
 
 
 # The following visualization function has been generated by ChatGPT 3.5, Mar23 Version. Thanks.
 #
 # def visualize_maze(width, height, edges):
 #     maze = [['#' for _ in range(2 * width + 1)] for _ in range(2 * height + 1)]
 #
@@ -163,52 +165,74 @@
 class Monster(Entity):
     def __init__(self, x, y, kind):
         super().__init__(x, y)
         self.kind = kind
 
 
 class MonsterKind:
-    def __init__(self, char, level, feed, item="", companion=""):
+    def __init__(self, char, level, feed, item="", effect="", companion=""):
         self.char = char
         self.level = level
         self.item = item
+        self.effect = effect
         self.feed = feed
         self.companion = companion
 
 
 # Combine monster_data and item_data into a single dict
 MONSTER_KINDS: List[MonsterKind] = [
-    MonsterKind("a", 1, FOOD_AMOEBA),  # Amoeba
-    MonsterKind("b", 3, FOOD_BISON, item=ITEM_BISON_MEAT),  # Bison
-    MonsterKind("c", 6, FOOD_CHIMERA, item=ITEM_SWORD),  # Chimera
-    MonsterKind("d", 15, FOOD_COMODO_DRAGON, item=ITEM_POISONED),  # Comodo Dragon
-    MonsterKind(CHAR_DRAGON, 15, FOOD_DRAGON, item=ITEM_TREASURE_POINTER),  # Dragon
-    MonsterKind("E", 20, FOOD_ELEMENTAL, item=ITEM_RANDOM_TRANSPORT),  # Elemental
+    MonsterKind("a", 1, FEED_AMOEBA),  # Amoeba
+    MonsterKind("b", 3, FEED_BISON, effect=EFFECT_FEED_MUCH),  # Bison
+    MonsterKind("c", 6, FEED_CHIMERA, item=ITEM_SWORD),  # Chimera
+    MonsterKind("d", 18, FEED_COMODO_DRAGON, item=ITEM_POISONED),  # Comodo Dragon
+    MonsterKind(CHAR_DRAGON, 15, FEED_DRAGON, effect=EFFECT_TREASURE_POINTER),  # Dragon
+    MonsterKind("E", 24, FEED_ELEMENTAL, effect=EFFECT_RANDOM_TRANSPORT),  # Elemental
     MonsterKind("f", 0, 0, companion=COMPANION_FAIRY),  # Fairy
 ]
 
 RARE_MONSTER_KINDS: List[MonsterKind] = [
-    MonsterKind("A", 1, FOOD_AMOEBA, item=ITEM_SPECIAL_EXP),  # Amoeba rare
-    MonsterKind("B", 3, FOOD_SPECIAL_BISON, item=ITEM_SPECIAL_BISON_MEAT),  # Bison rare
-    MonsterKind("C", 6, FOOD_CHIMERA, item=ITEM_SWORD_AND_CLAIRVOYANCE),  # Chimera rare
-    MonsterKind("G", 0, FOOD_GORGON, item=ITEM_STONED),  # Gorgon
+    MonsterKind("A", 1, FEED_AMOEBA, effect=EFFECT_SPECIAL_EXP),  # Amoeba rare
+    MonsterKind("B", 3, FEED_RARE_BISON, effect=EFFECT_FEED_MUCH),  # Bison rare
+    MonsterKind("C", 6, FEED_CHIMERA, item=ITEM_SWORD, effect=EFFECT_CLAIRVOYANCE),  # Chimera rare
+    MonsterKind("G", 0, FEED_GORGON, effect=EFFECT_STONED),  # Gorgon
 ]
 
 MONSTER_KIND_POPULATION: Dict[str, int] = {
-    "a": 20,
-    "b": 4,
+    "a": 22,
+    "b": 5,
     "c": 4,
     "d": 4,
     "D": 1,
-    "E": 2,
+    "E": 1,
     "f": 1,
 }
 
 
-def find_random_place(objects: List[Entity], field: List[List[str]], distance: int) -> Point:
+def place_to_tile(x: int, y: int) -> Point:
+    return (x - 1) // (TILE_WIDTH + 1), (y - 1) // (TILE_HEIGHT)
+
+
+def tile_to_place_range(x: int, y: int) -> Tuple[Point, Point]:
+    lt = (x * (TILE_WIDTH + 1) + 1, y * (TILE_HEIGHT + 1) + 1)
+    rb = (lt[0] + TILE_WIDTH, lt[1] + TILE_HEIGHT)
+    return lt, rb
+
+
+def find_random_place_in_range(field: List[List[str]], left_top: Point, right_bottom: Point) -> Point:
+    assert left_top[0] < right_bottom[0]
+    assert left_top[1] < right_bottom[1]
+
+    x = rand.randrange(right_bottom[0] - left_top[0]) + left_top[0]
+    y = rand.randrange(right_bottom[1] - left_top[1]) + left_top[1]
+    assert field[y][x] == " "
+
+    return x, y
+
+
+def find_random_place(objects: List[Entity], field: List[List[str]], distance: int = 2, place_range: Optional[Tuple[Point, Point]] = None) -> Point:
     places = [(o.x, o.y) for o in objects]
     while True:
         x = rand.randrange(FIELD_WIDTH - 2) + 1
         y = rand.randrange(FIELD_HEIGHT - 2) + 1
         if (
             field[y][x] == " "
             and field[y][x + 1] == " "
@@ -226,59 +250,63 @@
     - field: the game field
 
     This function modifies the objects list by adding newly spawned monsters.
     """
 
     for kind in MONSTER_KINDS:
         for _ in range(MONSTER_KIND_POPULATION[kind.char]):
-            x, y = find_random_place(objects, field, 3)
+            x, y = find_random_place(objects, field, distance=3)
             m = Monster(x, y, kind)
             objects.append(m)
     kind = rand.choice(RARE_MONSTER_KINDS)
-    x, y = find_random_place(objects, field, 3)
+    x, y = find_random_place(objects, field, distance=3)
     m = Monster(x, y, kind)
     objects.append(m)
 
 
-def create_field(corridor_h_width: int, corridor_v_width: int, wall_chars: str) -> List[List[str]]:
+def create_field(corridor_h_width: int, corridor_v_width: int, wall_chars: str) -> Tuple[List[List[str]], Point, Point]:
     # Create field filled with spaces
     field = [[" " for _ in range(FIELD_WIDTH)] for _ in range(FIELD_HEIGHT)]
 
     # Create walls
-    for ry in range(ROOM_NUM_Y + 1):
-        y = ry * (ROOM_HEIGHT + 1)
+    for ty in range(TILE_NUM_Y + 1):
+        y = ty * (TILE_HEIGHT + 1)
         for x in range(0, FIELD_WIDTH):
             field[y][x] = wall_chars[1]
-    for rx in range(ROOM_NUM_X + 1):
-        x = rx * (ROOM_WIDTH + 1)
+    for tx in range(TILE_NUM_X + 1):
+        x = tx * (TILE_WIDTH + 1)
         for y in range(0, FIELD_HEIGHT):
             field[y][x] = wall_chars[2]
-    for ry in range(ROOM_NUM_Y + 1):
-        y = ry * (ROOM_HEIGHT + 1)
-        for rx in range(ROOM_NUM_X + 1):
-            x = rx * (ROOM_WIDTH + 1)
+    for ty in range(TILE_NUM_Y + 1):
+        y = ty * (TILE_HEIGHT + 1)
+        for tx in range(TILE_NUM_X + 1):
+            x = tx * (TILE_WIDTH + 1)
             field[y][x] = wall_chars[0]
 
     # Create corridors
-    edges = gen_maze(ROOM_NUM_X, ROOM_NUM_Y)
+    edges, first_p, last_p = gen_maze(TILE_NUM_X, TILE_NUM_Y)
     for edge in edges:
         (x1, y1), (x2, y2) = sorted(edge)
         assert x1 <= x2
         assert y1 <= y2
         if y1 == y2:
-            d = rand.randrange(ROOM_HEIGHT + 1 - corridor_h_width) + 1
+            d = rand.randrange(TILE_HEIGHT + 1 - corridor_h_width) + 1
             for y in range(corridor_h_width):
-                field[y1 * (ROOM_HEIGHT + 1) + d + y][x2 * (ROOM_WIDTH + 1)] = " "
+                field[y1 * (TILE_HEIGHT + 1) + d + y][x2 * (TILE_WIDTH + 1)] = " "
         else:
             assert x1 == x2
-            d = rand.randrange(ROOM_WIDTH + 1 - corridor_v_width) + 1
+            d = rand.randrange(TILE_WIDTH + 1 - corridor_v_width) + 1
             for x in range(corridor_v_width):
-                field[y2 * (ROOM_HEIGHT + 1)][x1 * (ROOM_WIDTH + 1) + d + x] = " "
+                field[y2 * (TILE_HEIGHT + 1)][x1 * (TILE_WIDTH + 1) + d + x] = " "
 
-    return field
+    r = tile_to_place_range(*first_p)
+    first_p = find_random_place_in_range(field, r[0], r[1])
+    r = tile_to_place_range(*last_p)
+    last_p = find_random_place_in_range(field, r[0], r[1])
+    return field, first_p, last_p
 
 
 def draw_stage(
     stdscr: curses.window,
     objects: List[Entity],
     field: List[List[str]],
     torched: List[List[int]],
@@ -348,21 +376,21 @@
     else:
         return player.level
 
 
 def draw_status_bar(stdscr: curses.window, player: Player, hours: int, message: Optional[str] = None) -> None:
     if player.item == ITEM_SWORD:
         level_str = "LVL: %d x3" % player.level
-        item_str = "ITEM: %s(%s)" % (player.item, player.item_taken_from)
+        item_str = "+%s(%s)" % (player.item, player.item_taken_from)
     elif player.item == ITEM_POISONED:
         level_str = "LVL: %d /3" % player.level
-        item_str = "ITEM: %s(%s)" % (player.item, player.item_taken_from)
+        item_str = "+%s(%s)" % (player.item, player.item_taken_from)
     else:
         level_str = "LVL: %d" % player.level
-        item_str = "ITEM: -"
+        item_str = ""
 
     beatable = None
     atk = player_attack_by_level(player)
     for mk in MONSTER_KINDS:
         if mk.level == 0:
             continue
         if mk.level > atk:
@@ -373,15 +401,15 @@
     buf = []
     buf.append("HRS: %d" % hours)
     buf.append(level_str)
     if beatable is not None:
         buf.append("> %s" % beatable.char)
     buf.append("FOOD: %d" % player.food)
     buf.append(item_str)
-    buf.append("/ [Q] to exit")
+    buf.append("/ [Q]uit [R]estart")
     stdscr.addstr(FIELD_HEIGHT, 0, "  ".join(buf))
 
     if player.item == ITEM_TREASURE or player.food <= 0:
         if not message:
             message = ''
         message += "  SEED: %d" % rand.seed
 
@@ -402,112 +430,93 @@
     else:
         return None
     return dx, dy
 
 
 def update_torched(torched: List[List[int]], player: Player, torch_radius: int) -> None:
     if player.companion == COMPANION_FAIRY:
-        torch_radius += 1
+        torch_radius += FAIRY_TORCH_EXTENSION
 
     for dy in range(-torch_radius, torch_radius + 1):
         y = player.y + dy
         if 0 <= y < FIELD_HEIGHT:
-            w = int(math.sqrt((torch_radius * 1.2) ** 2 - dy**2) + 0.5)
+            w = int(math.sqrt((torch_radius * 1.1) ** 2 - dy**2) + 0.5)
             for dx in range(-w, w + 1):
                 x = player.x + dx
                 if 0 <= x < FIELD_WIDTH:
                     torched[y][x] = 1
 
 
 args_box: List[argparse.Namespace] = []
 
 
 class TerminalSizeSmall(ValueError):
     pass
 
 
-def curses_main(stdscr: curses.window) -> None:
+def curses_main(stdscr: curses.window) -> bool:
     sh, sw = stdscr.getmaxyx()
     if sh < FIELD_HEIGHT + 2 or sw < FIELD_WIDTH:
         raise TerminalSizeSmall()
 
     assert args_box
     args = args_box[0]
 
     # Set up the game
     corridor_h_width, corridor_v_width = (1, 2) if args.narrower_corridors else (CORRIDOR_H_WIDTH, CORRIDOR_V_WIDTH)
-    field: List[List[str]] = create_field(corridor_h_width, corridor_v_width, WALL_CHARS)
+    field, first_p, last_p = create_field(corridor_h_width, corridor_v_width, WALL_CHARS)
     torched: List[List[int]] = [[0 for _ in range(FIELD_WIDTH)] for _ in range(FIELD_HEIGHT)]
-    x, y = find_random_place([], field, 2)
-    player: Player = Player(x, y, 1, FOOD_INIT)
+    player: Player = Player(first_p[0], first_p[1], 1, FOOD_INIT)
     objects: List[Entity] = [player]
-    treasure: Treasure = Treasure(*find_random_place(objects, field, 2))
+    treasure: Treasure = Treasure(last_p[0], last_p[1])
     objects.append(treasure)
     spawn_monsters(objects, field)
     encountered_types: Set[str] = set()
 
     torch_radius: int = 4
     if args.large_torch:
         torch_radius = 5
     elif args.small_torch:
         torch_radius = 3
 
-    def consume_player_item(player: Player) -> str:
-        item = player.item
-        message = ""
-        if item in [ITEM_BISON_MEAT, ITEM_SPECIAL_BISON_MEAT]:
-            message = "-- Stuffed."
-            player.item = ""
-        elif item == ITEM_TREASURE_POINTER:
-            message = "-- Sparkle."
-            player.item = ""
-        elif item == ITEM_SPECIAL_EXP:
-            message = "-- Special Exp."
-            player.item = ""
-        elif item == ITEM_SWORD_AND_CLAIRVOYANCE:
-            message = "-- Clairvoyance."
-            player.item = ITEM_SWORD
-        elif item == ITEM_STONED:
-            message = "-- Stoned."
-            player.item = ""
-        return message
-
     stdscr.keypad(True)
 
+    flash_message: Optional[str] = None
     message: Optional[str] = None
     hours: int = -1
     game_ends = False
     while not game_ends:
         hours += 1
 
         # Starvation check
         player.food -= 1
         if args.eating_frugal and player.food < FOOD_STARVATION and hours % 2 == 0:
             player.food += 1
-        elif args.eating_excessive and player.food > FOOD_INIT and hours % 4 == 0:
-            player.food -= 1
         if player.food <= 0:
             message = ">> Starved to Death. <<"
             game_ends = True
             break
 
         # Show the field
         update_torched(torched, player, torch_radius)
-        temp_message = consume_player_item(player)
         stdscr.clear()
         draw_stage(stdscr, objects, field, torched, encountered_types, show_entities=args.debug_show_entities)
-        draw_status_bar(stdscr, player, hours, message=message or temp_message)
+        draw_status_bar(stdscr, player, hours, message=message or flash_message)
         stdscr.refresh()
+        if flash_message:
+            flash_message = None
 
         # Move player
         while True:
             key = stdscr.getch()
+            if key == ord('r'):
+                return True  # restart
             d = key_to_dir(key)
             if d is None:
-                return
+                return False  # quit
 
             dx, dy = d
             new_x, new_y = player.x + dx, player.y + dy
             if field[new_y][new_x] == " ":  # if the cell is not a wall
                 player.x, player.y = new_x, new_y
                 break
 
@@ -534,80 +543,86 @@
                     player.item_taken_from = ''
                     break
             elif isinstance(enc_obj, Monster):
                 m = enc_obj
                 encountered_types.add(m.kind.char)
                 player_attack = player_attack_by_level(player)
 
+                effect = m.kind.effect
                 if player_attack < m.kind.level:
-                    if m.kind.item == ITEM_RANDOM_TRANSPORT:
-                        player.x, player.y = find_random_place(objects, field, 2)
+                    if effect == EFFECT_RANDOM_TRANSPORT:
+                        player.x, player.y = find_random_place(objects, field, distance=2)
                     else:
                         # respawn
-                        player.x, player.y = find_random_place(objects, field, 2)
+                        player.x, player.y = find_random_place(objects, field, distance=2)
                         player.item = ""
                         player.item_taken_from = ""
                         player.food = min(player.food, FOOD_INIT)
+                        # flash_message = "-- Respawn."
                 else:
-                    if m.kind.item == ITEM_RANDOM_TRANSPORT:
+                    if effect == EFFECT_RANDOM_TRANSPORT:
                         pass  # do not change player level
-                    elif m.kind.item == ITEM_SPECIAL_EXP:
+                    elif effect == EFFECT_SPECIAL_EXP:
                         player.level += 7
                     else:
                         player.level += 1
 
-                    if m.kind.item == ITEM_SWORD_AND_CLAIRVOYANCE:
-                        update_torched(torched, player, torch_radius * 4)
-
-                    if m.kind.item == ITEM_TREASURE_POINTER:
-                        encountered_types.add(CHAR_TREASURE)
-
-                    if m.kind.item == ITEM_STONED:
-                        if player.companion == COMPANION_FAIRY:
-                            player.companion = ''
-                        else:
-                            hours += -m.kind.feed
-                            player.food += m.kind.feed
-                            if player.food < 1:
-                                player.food = 1
-                    else:
-                        player.food = min(FOOD_MAX, player.food + m.kind.feed)
+                    if m.kind.feed < 0:
+                        hours += -m.kind.feed
+                    player.food += m.kind.feed
+                    player.food = max(1, min(FOOD_MAX, player.food + m.kind.feed))
 
                     if m.kind.companion:
                         player.companion = m.kind.companion
 
-                    if m.kind.item == ITEM_RANDOM_TRANSPORT:
-                        player.x, player.y = find_random_place(objects, field, 2)
+                    if effect == EFFECT_RANDOM_TRANSPORT:
+                        player.x, player.y = find_random_place(objects, field, distance=2)
                         m.x, m.y = player.x + 1, player.y
                     else:
                         del objects[enc_obj_i]
                         player.item = m.kind.item
                         player.item_taken_from = m.kind.char
 
+                        if effect == EFFECT_CLAIRVOYANCE:
+                            update_torched(torched, player, torch_radius * 4)
+                            flash_message = "-- Clairvoyance."
+                        elif effect == EFFECT_TREASURE_POINTER:
+                            encountered_types.add(CHAR_TREASURE)
+                            flash_message = "-- Sparkle."
+                        elif effect == EFFECT_FEED_MUCH:
+                            flash_message = "-- Stuffed."
+                        elif effect == EFFECT_SPECIAL_EXP:
+                            flash_message = "-- Special Exp."
+                        elif effect == EFFECT_STONED:
+                            flash_message = "-- Stoned."
+                            if player.companion == COMPANION_FAIRY:
+                                player.companion = ''
+
         for sur_obj_i, sur_obj in sur_obj_infos:
             if isinstance(sur_obj, Treasure):
                 if CHAR_DRAGON in encountered_types:
                     encountered_types.add(CHAR_TREASURE)
 
     update_torched(torched, player, torch_radius)
 
-    temp_message = consume_player_item(player)
     stdscr.clear()
     draw_stage(stdscr, objects, field, torched, encountered_types, show_entities=args.debug_show_entities)
-    draw_status_bar(stdscr, player, hours, message=message or temp_message)
+    draw_status_bar(stdscr, player, hours, message=message or flash_message)
     stdscr.refresh()
 
     while True:
         key = stdscr.getch()
         if key == ord("q"):
-            break
+            return False  # quit
         elif key == ord("r"):
+            return True  # restart
+        elif key == ord("m"):
             stdscr.clear()
             draw_stage(stdscr, objects, field, torched, encountered_types, show_entities=True)
-            draw_status_bar(stdscr, player, hours, message=message or temp_message)
+            draw_status_bar(stdscr, player, hours, message=message or flash_message)
             stdscr.refresh()
 
 
 def main():
     global rand
 
     parser = argparse.ArgumentParser(
@@ -619,39 +634,42 @@
     g = parser.add_mutually_exclusive_group()
     g.add_argument("-T", "--large-torch", action="store_true", help="Large torch.")
     g.add_argument("-t", "--small-torch", action="store_true", help="Small torch.")
 
     parser.add_argument("--debug-show-entities", action="store_true", help="Debug option.")
     parser.add_argument("-n", "--narrower-corridors", action="store_true", help="Narrower corridors.")
     parser.add_argument("-E", '--eating-frugal', action='store_true', help='Decrease rate of consuming food')
-    parser.add_argument("-e", '--eating-excessive', action='store_true', help='Increase rate of consuming food')
     parser.add_argument("--seed", action='store', type=int, help='Seed value')
 
     args = parser.parse_args()
     args_box.append(args)
 
-    if args.seed is not None:
-        rand = MyRandom(args.seed)
-    else:
-        rand = MyRandom(int(time.time()) % 100000)
+    seed = args.seed
+    if seed is None:
+        seed = int(time.time()) % 100000
 
     curses.initscr()
     curses.noecho()
     curses.cbreak()
     curses.curs_set(0)
 
     curses.start_color()
     curses.use_default_colors()
     curses.init_pair(1, curses.COLOR_GREEN, -1)  # wall
     curses.init_pair(2, curses.COLOR_BLUE, -1)  # player
     curses.init_pair(3, curses.COLOR_WHITE, -1)  # monster
     curses.init_pair(4, curses.COLOR_YELLOW, -1)  # treasure
 
     try:
-        curses.wrapper(curses_main)
+        while True:
+            rand = MyRandom(seed)
+
+            retry = curses.wrapper(curses_main)
+            if not retry:
+                break
     except TerminalSizeSmall as e:
         sys.exit("Error: Terminal size too small. Minimum size is: %d x %d" % (FIELD_WIDTH, FIELD_HEIGHT + 2))
     finally:
         curses.endwin()
 
 
 if __name__ == "__main__":
```

### Comparing `arlq-1.2.0/arlq.egg-info/PKG-INFO` & `arlq-1.2.1/arlq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arlq
-Version: 1.2.0
+Version: 1.2.1
 Summary: ARQL, another rogue-like quest game.
 Home-page: https://github.com/tos-kamiya/arlq
 Author: Toshihiro Kamiya
 Author-email: kamiya@mbj.nifty.com
 License: BSD 2-Clause License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `arlq-1.2.0/setup.cfg` & `arlq-1.2.1/setup.cfg`

 * *Files identical despite different names*

