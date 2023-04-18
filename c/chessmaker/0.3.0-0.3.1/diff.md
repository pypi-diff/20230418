# Comparing `tmp/chessmaker-0.3.0.tar.gz` & `tmp/chessmaker-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chessmaker-0.3.0.tar", max compression
+gzip compressed data, was "chessmaker-0.3.1.tar", max compression
```

## Comparing `chessmaker-0.3.0.tar` & `chessmaker-0.3.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0      159 2023-04-12 23:23:56.894161 chessmaker-0.3.0/chessmaker/__init__.py
--rw-r--r--   0        0        0      240 2023-04-13 13:53:22.478241 chessmaker-0.3.0/chessmaker/chess/__init__.py
--rw-r--r--   0        0        0      690 2023-04-15 21:57:06.856292 chessmaker-0.3.0/chessmaker/chess/base/__init__.py
--rw-r--r--   0        0        0     6771 2023-04-16 20:54:04.898469 chessmaker-0.3.0/chessmaker/chess/base/board.py
--rw-r--r--   0        0        0     1091 2023-04-16 20:29:32.083728 chessmaker-0.3.0/chessmaker/chess/base/game.py
--rw-r--r--   0        0        0      275 2023-04-13 19:53:48.822414 chessmaker-0.3.0/chessmaker/chess/base/move_option.py
--rw-r--r--   0        0        0     4006 2023-04-16 20:23:48.040602 chessmaker-0.3.0/chessmaker/chess/base/piece.py
--rw-r--r--   0        0        0      583 2023-04-12 22:32:25.286163 chessmaker-0.3.0/chessmaker/chess/base/player.py
--rw-r--r--   0        0        0      241 2023-04-12 22:32:25.006418 chessmaker-0.3.0/chessmaker/chess/base/position.py
--rw-r--r--   0        0        0      708 2023-04-12 22:57:13.193723 chessmaker-0.3.0/chessmaker/chess/base/rule.py
--rw-r--r--   0        0        0     2304 2023-04-16 20:16:29.441811 chessmaker-0.3.0/chessmaker/chess/base/square.py
--rw-r--r--   0        0        0     5299 2023-04-14 16:36:39.857090 chessmaker-0.3.0/chessmaker/chess/game_factory.py
--rw-r--r--   0        0        0     2460 2023-04-15 15:01:42.502293 chessmaker-0.3.0/chessmaker/chess/piece_utils.py
--rw-r--r--   0        0        0      319 2023-04-13 13:47:46.308045 chessmaker-0.3.0/chessmaker/chess/pieces/__init__.py
--rw-r--r--   0        0        0      652 2023-04-13 13:46:31.618457 chessmaker-0.3.0/chessmaker/chess/pieces/bishop.py
--rw-r--r--   0        0        0     6790 2023-04-16 20:01:11.181718 chessmaker-0.3.0/chessmaker/chess/pieces/king.py
--rw-r--r--   0        0        0      880 2023-04-13 13:46:31.589457 chessmaker-0.3.0/chessmaker/chess/pieces/knight.py
--rw-r--r--   0        0        0      191 2023-04-12 23:23:13.134441 chessmaker-0.3.0/chessmaker/chess/pieces/knook/__init__.py
--rw-r--r--   0        0        0      968 2023-04-15 14:44:35.264730 chessmaker-0.3.0/chessmaker/chess/pieces/knook/knook.py
--rw-r--r--   0        0        0       30 2023-04-15 15:13:15.595692 chessmaker-0.3.0/chessmaker/chess/pieces/knook/knookable.py
--rw-r--r--   0        0        0     1184 2023-04-16 21:13:06.169907 chessmaker-0.3.0/chessmaker/chess/pieces/knook/knookable_knight.py
--rw-r--r--   0        0        0     1216 2023-04-15 21:58:00.111375 chessmaker-0.3.0/chessmaker/chess/pieces/knook/knookable_rook.py
--rw-r--r--   0        0        0     1615 2023-04-15 21:58:00.012862 chessmaker-0.3.0/chessmaker/chess/pieces/knook/merge_to_knook.py
--rw-r--r--   0        0        0     5506 2023-04-16 20:01:11.191719 chessmaker-0.3.0/chessmaker/chess/pieces/pawn.py
--rw-r--r--   0        0        0      785 2023-04-13 13:46:31.572457 chessmaker-0.3.0/chessmaker/chess/pieces/queen.py
--rw-r--r--   0        0        0     1057 2023-04-16 21:13:16.019354 chessmaker-0.3.0/chessmaker/chess/pieces/rook.py
--rw-r--r--   0        0        0      332 2023-04-14 13:45:12.352119 chessmaker-0.3.0/chessmaker/chess/results/__init__.py
--rw-r--r--   0        0        0      478 2023-04-14 12:39:03.945677 chessmaker-0.3.0/chessmaker/chess/results/capture_all_pieces_to_win.py
--rw-r--r--   0        0        0      584 2023-04-14 12:32:41.047541 chessmaker-0.3.0/chessmaker/chess/results/checkmate.py
--rw-r--r--   0        0        0      801 2023-04-16 21:29:32.511999 chessmaker-0.3.0/chessmaker/chess/results/double_check_to_win.py
--rw-r--r--   0        0        0     1134 2023-04-15 02:00:39.838687 chessmaker-0.3.0/chessmaker/chess/results/no_captures_or_pawn_moves.py
--rw-r--r--   0        0        0      923 2023-04-14 11:49:56.085457 chessmaker-0.3.0/chessmaker/chess/results/repetition.py
--rw-r--r--   0        0        0      326 2023-04-14 11:49:56.091457 chessmaker-0.3.0/chessmaker/chess/results/stalemate.py
--rw-r--r--   0        0        0      510 2023-04-15 00:31:09.011728 chessmaker-0.3.0/chessmaker/chess/results/standard_result.py
--rw-r--r--   0        0        0      345 2023-04-14 13:02:43.693404 chessmaker-0.3.0/chessmaker/chess/rules/__init__.py
--rw-r--r--   0        0        0     3533 2023-04-13 13:46:31.611456 chessmaker-0.3.0/chessmaker/chess/rules/beta_decay.py
--rw-r--r--   0        0        0     1875 2023-04-14 14:42:06.954160 chessmaker-0.3.0/chessmaker/chess/rules/forced_en_passant.py
--rw-r--r--   0        0        0     3670 2023-04-15 12:04:05.521043 chessmaker-0.3.0/chessmaker/chess/rules/il_vaticano.py
--rw-r--r--   0        0        0      979 2023-04-14 12:49:09.088586 chessmaker-0.3.0/chessmaker/chess/rules/king_cant_move_to_c2.py
--rw-r--r--   0        0        0     2695 2023-04-12 22:57:13.120723 chessmaker-0.3.0/chessmaker/chess/rules/knight_boosting.py
--rw-r--r--   0        0        0     2461 2023-04-14 13:33:54.257799 chessmaker-0.3.0/chessmaker/chess/rules/la_bastarda.py
--rw-r--r--   0        0        0     1871 2023-04-15 12:04:05.540043 chessmaker-0.3.0/chessmaker/chess/rules/omnipotent_f6_pawn.py
--rw-r--r--   0        0        0     1982 2023-04-14 01:23:32.960857 chessmaker-0.3.0/chessmaker/chess/rules/siberian_swipe.py
--rw-r--r--   0        0        0       64 2023-04-14 17:14:53.444902 chessmaker-0.3.0/chessmaker/clients/__init__.py
--rw-r--r--   0        0        0    16008 2023-04-16 21:34:55.732847 chessmaker-0.3.0/chessmaker/clients/pywebio_ui.py
--rw-r--r--   0        0        0      278 2023-04-12 22:32:25.207165 chessmaker-0.3.0/chessmaker/cloneable.py
--rw-r--r--   0        0        0      149 2023-04-15 21:57:06.796292 chessmaker-0.3.0/chessmaker/events/__init__.py
--rw-r--r--   0        0        0      395 2023-04-13 19:53:48.832414 chessmaker-0.3.0/chessmaker/events/event.py
--rw-r--r--   0        0        0      146 2023-04-14 13:26:17.602659 chessmaker-0.3.0/chessmaker/events/event_priority.py
--rw-r--r--   0        0        0     3689 2023-04-16 20:12:32.196037 chessmaker-0.3.0/chessmaker/events/event_publisher.py
--rw-r--r--   0        0        0    35184 2023-04-05 10:50:17.213863 chessmaker-0.3.0/LICENSE
--rw-r--r--   0        0        0     1098 2023-04-16 21:19:33.850028 chessmaker-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1862 2023-04-14 14:15:04.351108 chessmaker-0.3.0/README.md
--rw-r--r--   0        0        0     2960 1970-01-01 00:00:00.000000 chessmaker-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      159 2023-04-12 23:23:56.894161 chessmaker-0.3.1/chessmaker/__init__.py
+-rw-r--r--   0        0        0      240 2023-04-13 13:53:22.478241 chessmaker-0.3.1/chessmaker/chess/__init__.py
+-rw-r--r--   0        0        0      690 2023-04-15 21:57:06.856292 chessmaker-0.3.1/chessmaker/chess/base/__init__.py
+-rw-r--r--   0        0        0     6771 2023-04-16 20:54:04.898469 chessmaker-0.3.1/chessmaker/chess/base/board.py
+-rw-r--r--   0        0        0     1091 2023-04-16 20:29:32.083728 chessmaker-0.3.1/chessmaker/chess/base/game.py
+-rw-r--r--   0        0        0      275 2023-04-13 19:53:48.822414 chessmaker-0.3.1/chessmaker/chess/base/move_option.py
+-rw-r--r--   0        0        0     3553 2023-04-18 19:28:26.768718 chessmaker-0.3.1/chessmaker/chess/base/piece.py
+-rw-r--r--   0        0        0      583 2023-04-12 22:32:25.286163 chessmaker-0.3.1/chessmaker/chess/base/player.py
+-rw-r--r--   0        0        0      241 2023-04-12 22:32:25.006418 chessmaker-0.3.1/chessmaker/chess/base/position.py
+-rw-r--r--   0        0        0      708 2023-04-12 22:57:13.193723 chessmaker-0.3.1/chessmaker/chess/base/rule.py
+-rw-r--r--   0        0        0     2304 2023-04-16 20:16:29.441811 chessmaker-0.3.1/chessmaker/chess/base/square.py
+-rw-r--r--   0        0        0     5299 2023-04-14 16:36:39.857090 chessmaker-0.3.1/chessmaker/chess/game_factory.py
+-rw-r--r--   0        0        0     2460 2023-04-15 15:01:42.502293 chessmaker-0.3.1/chessmaker/chess/piece_utils.py
+-rw-r--r--   0        0        0      319 2023-04-13 13:47:46.308045 chessmaker-0.3.1/chessmaker/chess/pieces/__init__.py
+-rw-r--r--   0        0        0      652 2023-04-13 13:46:31.618457 chessmaker-0.3.1/chessmaker/chess/pieces/bishop.py
+-rw-r--r--   0        0        0     6790 2023-04-16 20:01:11.181718 chessmaker-0.3.1/chessmaker/chess/pieces/king.py
+-rw-r--r--   0        0        0      880 2023-04-13 13:46:31.589457 chessmaker-0.3.1/chessmaker/chess/pieces/knight.py
+-rw-r--r--   0        0        0      191 2023-04-12 23:23:13.134441 chessmaker-0.3.1/chessmaker/chess/pieces/knook/__init__.py
+-rw-r--r--   0        0        0      968 2023-04-15 14:44:35.264730 chessmaker-0.3.1/chessmaker/chess/pieces/knook/knook.py
+-rw-r--r--   0        0        0       30 2023-04-15 15:13:15.595692 chessmaker-0.3.1/chessmaker/chess/pieces/knook/knookable.py
+-rw-r--r--   0        0        0     1184 2023-04-16 21:13:06.169907 chessmaker-0.3.1/chessmaker/chess/pieces/knook/knookable_knight.py
+-rw-r--r--   0        0        0     1216 2023-04-15 21:58:00.111375 chessmaker-0.3.1/chessmaker/chess/pieces/knook/knookable_rook.py
+-rw-r--r--   0        0        0     1615 2023-04-15 21:58:00.012862 chessmaker-0.3.1/chessmaker/chess/pieces/knook/merge_to_knook.py
+-rw-r--r--   0        0        0     5506 2023-04-16 20:01:11.191719 chessmaker-0.3.1/chessmaker/chess/pieces/pawn.py
+-rw-r--r--   0        0        0      785 2023-04-13 13:46:31.572457 chessmaker-0.3.1/chessmaker/chess/pieces/queen.py
+-rw-r--r--   0        0        0     1057 2023-04-16 21:13:16.019354 chessmaker-0.3.1/chessmaker/chess/pieces/rook.py
+-rw-r--r--   0        0        0      332 2023-04-14 13:45:12.352119 chessmaker-0.3.1/chessmaker/chess/results/__init__.py
+-rw-r--r--   0        0        0      478 2023-04-14 12:39:03.945677 chessmaker-0.3.1/chessmaker/chess/results/capture_all_pieces_to_win.py
+-rw-r--r--   0        0        0      584 2023-04-14 12:32:41.047541 chessmaker-0.3.1/chessmaker/chess/results/checkmate.py
+-rw-r--r--   0        0        0      801 2023-04-16 21:29:32.511999 chessmaker-0.3.1/chessmaker/chess/results/double_check_to_win.py
+-rw-r--r--   0        0        0     1134 2023-04-15 02:00:39.838687 chessmaker-0.3.1/chessmaker/chess/results/no_captures_or_pawn_moves.py
+-rw-r--r--   0        0        0      923 2023-04-14 11:49:56.085457 chessmaker-0.3.1/chessmaker/chess/results/repetition.py
+-rw-r--r--   0        0        0      326 2023-04-14 11:49:56.091457 chessmaker-0.3.1/chessmaker/chess/results/stalemate.py
+-rw-r--r--   0        0        0      510 2023-04-15 00:31:09.011728 chessmaker-0.3.1/chessmaker/chess/results/standard_result.py
+-rw-r--r--   0        0        0      345 2023-04-14 13:02:43.693404 chessmaker-0.3.1/chessmaker/chess/rules/__init__.py
+-rw-r--r--   0        0        0     3533 2023-04-13 13:46:31.611456 chessmaker-0.3.1/chessmaker/chess/rules/beta_decay.py
+-rw-r--r--   0        0        0     1875 2023-04-14 14:42:06.954160 chessmaker-0.3.1/chessmaker/chess/rules/forced_en_passant.py
+-rw-r--r--   0        0        0     3670 2023-04-15 12:04:05.521043 chessmaker-0.3.1/chessmaker/chess/rules/il_vaticano.py
+-rw-r--r--   0        0        0      979 2023-04-14 12:49:09.088586 chessmaker-0.3.1/chessmaker/chess/rules/king_cant_move_to_c2.py
+-rw-r--r--   0        0        0     2695 2023-04-12 22:57:13.120723 chessmaker-0.3.1/chessmaker/chess/rules/knight_boosting.py
+-rw-r--r--   0        0        0     2461 2023-04-14 13:33:54.257799 chessmaker-0.3.1/chessmaker/chess/rules/la_bastarda.py
+-rw-r--r--   0        0        0     1871 2023-04-15 12:04:05.540043 chessmaker-0.3.1/chessmaker/chess/rules/omnipotent_f6_pawn.py
+-rw-r--r--   0        0        0     1982 2023-04-14 01:23:32.960857 chessmaker-0.3.1/chessmaker/chess/rules/siberian_swipe.py
+-rw-r--r--   0        0        0       64 2023-04-14 17:14:53.444902 chessmaker-0.3.1/chessmaker/clients/__init__.py
+-rw-r--r--   0        0        0    16031 2023-04-18 19:28:26.764718 chessmaker-0.3.1/chessmaker/clients/pywebio_ui.py
+-rw-r--r--   0        0        0      278 2023-04-12 22:32:25.207165 chessmaker-0.3.1/chessmaker/cloneable.py
+-rw-r--r--   0        0        0      149 2023-04-15 21:57:06.796292 chessmaker-0.3.1/chessmaker/events/__init__.py
+-rw-r--r--   0        0        0      395 2023-04-13 19:53:48.832414 chessmaker-0.3.1/chessmaker/events/event.py
+-rw-r--r--   0        0        0      146 2023-04-14 13:26:17.602659 chessmaker-0.3.1/chessmaker/events/event_priority.py
+-rw-r--r--   0        0        0     3834 2023-04-18 18:39:24.165304 chessmaker-0.3.1/chessmaker/events/event_publisher.py
+-rw-r--r--   0        0        0    35184 2023-04-05 10:50:17.213863 chessmaker-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1098 2023-04-18 19:45:29.028136 chessmaker-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1862 2023-04-14 14:15:04.351108 chessmaker-0.3.1/README.md
+-rw-r--r--   0        0        0     2960 1970-01-01 00:00:00.000000 chessmaker-0.3.1/PKG-INFO
```

### Comparing `chessmaker-0.3.0/chessmaker/chess/base/__init__.py` & `chessmaker-0.3.1/chessmaker/chess/base/__init__.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.0/chessmaker/chess/base/board.py` & `chessmaker-0.3.1/chessmaker/chess/base/board.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.0/chessmaker/chess/base/game.py` & `chessmaker-0.3.1/chessmaker/chess/base/game.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.0/chessmaker/chess/base/piece.py` & `chessmaker-0.3.1/chessmaker/chess/base/piece.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from abc import abstractmethod
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Iterable
 
-from chessmaker.chess.base.square import AfterAddPieceEvent, AfterRemovePieceEvent
 from chessmaker.chess.base.move_option import MoveOption
 from chessmaker.chess.base.player import Player
 from chessmaker.cloneable import Cloneable
 from chessmaker.events import event_publisher, Event, CancellableEvent, EventPublisher
 
 if TYPE_CHECKING:
     from chessmaker.chess.base.board import Board
@@ -49,30 +48,26 @@
 
 @event_publisher(*PIECE_EVENT_TYPES)
 class Piece(Cloneable, EventPublisher):
     def __init__(self, player: Player):
         super().__init__()
         self._player = player
         self._board: Board = None
-        self._move_options = None
 
     def __repr__(self):
         return f"{self.__class__.__name__} ({self.player})"
 
     def get_move_options(self) -> Iterable[MoveOption]:
-        if False:
-            return self._move_options
         move_options = self._get_move_options()
 
         before_get_move_options_event = BeforeGetMoveOptionsEvent(self, move_options)
         self.publish(before_get_move_options_event)
         move_options = before_get_move_options_event.move_options
         self.publish(AfterGetMoveOptionsEvent(self, move_options))
 
-        self._move_options = move_options
         return move_options
 
     def move(self, move_option: MoveOption):
         before_move_event = BeforeMoveEvent(self, move_option)
         self.publish(before_move_event)
         if before_move_event.cancelled:
             return
@@ -91,19 +86,15 @@
             capture_piece.publish(AfterCapturedEvent(capture_piece))
 
         destination.piece = self
 
         self.publish(AfterMoveEvent(self, move_option))
 
     def on_join_board(self):
-        self.board.subscribe(AfterAddPieceEvent, self._on_after_change_piece)
-        self.board.subscribe(AfterRemovePieceEvent, self._on_after_change_piece)
-
-    def _on_after_change_piece(self, _: Event):
-        self._move_options = None
+        pass
 
     @property
     def player(self):
         return self._player
 
     @property
     def position(self):
```

### Comparing `chessmaker-0.3.0/chessmaker/chess/base/player.py` & `chessmaker-0.3.1/chessmaker/chess/base/player.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.0/chessmaker/chess/base/rule.py` & `chessmaker-0.3.1/chessmaker/chess/base/rule.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.0/chessmaker/chess/base/square.py` & `chessmaker-0.3.1/chessmaker/chess/base/square.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.0/chessmaker/chess/game_factory.py` & `chessmaker-0.3.1/chessmaker/chess/game_factory.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.0/chessmaker/chess/piece_utils.py` & `chessmaker-0.3.1/chessmaker/chess/piece_utils.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.0/chessmaker/chess/pieces/bishop.py` & `chessmaker-0.3.1/chessmaker/chess/pieces/bishop.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.0/chessmaker/chess/pieces/king.py` & `chessmaker-0.3.1/chessmaker/chess/pieces/king.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.0/chessmaker/chess/pieces/knight.py` & `chessmaker-0.3.1/chessmaker/chess/pieces/knight.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.0/chessmaker/chess/pieces/knook/knook.py` & `chessmaker-0.3.1/chessmaker/chess/pieces/knook/knook.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.0/chessmaker/chess/pieces/knook/knookable_knight.py` & `chessmaker-0.3.1/chessmaker/chess/pieces/knook/knookable_knight.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.0/chessmaker/chess/pieces/knook/knookable_rook.py` & `chessmaker-0.3.1/chessmaker/chess/pieces/knook/knookable_rook.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.0/chessmaker/chess/pieces/knook/merge_to_knook.py` & `chessmaker-0.3.1/chessmaker/chess/pieces/knook/merge_to_knook.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.0/chessmaker/chess/pieces/pawn.py` & `chessmaker-0.3.1/chessmaker/chess/pieces/pawn.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.0/chessmaker/chess/pieces/queen.py` & `chessmaker-0.3.1/chessmaker/chess/pieces/queen.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.0/chessmaker/chess/pieces/rook.py` & `chessmaker-0.3.1/chessmaker/chess/pieces/rook.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.0/chessmaker/chess/results/checkmate.py` & `chessmaker-0.3.1/chessmaker/chess/results/checkmate.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.0/chessmaker/chess/results/double_check_to_win.py` & `chessmaker-0.3.1/chessmaker/chess/results/double_check_to_win.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.0/chessmaker/chess/results/no_captures_or_pawn_moves.py` & `chessmaker-0.3.1/chessmaker/chess/results/no_captures_or_pawn_moves.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.0/chessmaker/chess/results/repetition.py` & `chessmaker-0.3.1/chessmaker/chess/results/repetition.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.0/chessmaker/chess/rules/beta_decay.py` & `chessmaker-0.3.1/chessmaker/chess/rules/beta_decay.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.0/chessmaker/chess/rules/forced_en_passant.py` & `chessmaker-0.3.1/chessmaker/chess/rules/forced_en_passant.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.0/chessmaker/chess/rules/il_vaticano.py` & `chessmaker-0.3.1/chessmaker/chess/rules/il_vaticano.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.0/chessmaker/chess/rules/king_cant_move_to_c2.py` & `chessmaker-0.3.1/chessmaker/chess/rules/king_cant_move_to_c2.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.0/chessmaker/chess/rules/knight_boosting.py` & `chessmaker-0.3.1/chessmaker/chess/rules/knight_boosting.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.0/chessmaker/chess/rules/la_bastarda.py` & `chessmaker-0.3.1/chessmaker/chess/rules/la_bastarda.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.0/chessmaker/chess/rules/omnipotent_f6_pawn.py` & `chessmaker-0.3.1/chessmaker/chess/rules/omnipotent_f6_pawn.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.0/chessmaker/chess/rules/siberian_swipe.py` & `chessmaker-0.3.1/chessmaker/chess/rules/siberian_swipe.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.0/chessmaker/clients/pywebio_ui.py` & `chessmaker-0.3.1/chessmaker/clients/pywebio_ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import time
 from copy import deepcopy
 from dataclasses import dataclass, field
-from functools import partial
 from itertools import groupby
-from typing import Callable, List, ParamSpec, TypeVar, Optional, Any
+from typing import Callable, List, ParamSpec, TypeVar, Optional
 from uuid import uuid4
 
 from pywebio import start_server, config
 from pywebio.input import input_group, actions, checkbox, radio
 from pywebio.io_ctrl import Output
 from pywebio.output import put_text, put_table, put_markdown, put_button, use_scope, clear, put_scope, popup, \
     close_popup, toast, put_error
@@ -45,28 +44,28 @@
 
 PIECE_URLS: dict[str, tuple[str, ...]] = {}
 for piece, piece_type in PIECE_TYPES.items():
     PIECE_URLS[piece] = (
         PIECE_URL_TEMPLATE.format(piece_color="w", piece_type=piece_type),
         PIECE_URL_TEMPLATE.format(piece_color="b", piece_type=piece_type),
     )
-    
+
+
 @dataclass
 class MultiplayerGame:
     game: Game
     options: list[str]
     sessions: List[ThreadBasedSession] = field(default_factory=list)
     colors: dict[str, str] = field(default_factory=dict)
     piece_urls: dict[str, tuple[str, ...]] = field(default_factory=lambda: PIECE_URLS)
 
 
 public_games: dict[str, tuple[float, MultiplayerGame]] = {}
 multiplayer_games: dict[str, MultiplayerGame] = {}
 
-
 PS = ParamSpec("PS")
 RT = TypeVar("RT")
 
 
 def for_all_game_sessions(func: Callable[PS, RT]) -> Callable[PS, RT]:
     game_id = session_data.game_id
 
@@ -149,23 +148,22 @@
                 else:
                     on_click = lambda _move_options=position_move_options: show_multiple_move_options(piece,
                                                                                                       _move_options)
                     text = "Multiple options"
 
                 content = put_button(text, color="transparent", onclick=on_click)
 
-
                 move_option_position_piece = board[move_option_position].piece
                 if move_option_position_piece is not None:
                     content.style(f"background-image: url({get_piece_url(move_option_position_piece)});")
 
                 content.style("width:80px")
                 content.style("height:80px")
                 content.style("background-size: 100%;")
-                content.style("background-color: #3c93f2") # #4bb543
+                content.style("background-color: #3c93f2")  # #4bb543
                 content.style("box-sizing: content-box")
                 content.style("border: 0.5px solid #aaaaaa")
 
     session_data.shown_move_options = sorted_move_options
     session_data.clicked_position = position
 
 
@@ -187,15 +185,14 @@
             return
 
     show_move_options(position)
 
 
 @use_scope("board")
 def square_content(square: Square):
-
     content = put_text(" ")
     content.style("white-space: nowrap;")
     if square is None:
         content = content.style("background-color: #ffffff")
         content = content.style("width:80px")
         content = content.style("height:80px")
     else:
@@ -204,14 +201,15 @@
             content = put_button("", color="transparent", onclick=lambda: on_piece_click(piece.position))
             content.style("white-space: nowrap;")
             content.style(f"background-image: url({get_piece_url(piece)});")
             content.style("background-size: 100%;")
 
     return content
 
+
 def get_board_strings(board: Board) -> dict[Position, Optional[str]]:
     board_strings = {}
     for y in range(board.size[1]):
         for x in range(board.size[0]):
             square = board[Position(x, y)]
             if square is None:
                 board_strings[Position(x, y)] = None
@@ -290,15 +288,17 @@
 
     session_data.game = game
     session_data.game_id = game_id
     session_data.own_game = False
 
     put_markdown("""# ChessMaker \n """).style("text-align:center")
     initialize_board()
-    put_markdown("[Docs](https://wolfdwyc.github.io/ChessMaker) - [Source](https://github.com/WolfDWyc/ChessMaker)\nMade by WolfDWyc").style("text-align:center")
+    put_markdown(
+        "[Docs](https://wolfdwyc.github.io/ChessMaker) - [Source](https://github.com/WolfDWyc/ChessMaker)\nMade by WolfDWyc").style(
+        "text-align:center")
 
 
 def new_game(game_factory: Callable[..., Game], options: list[str], mode: str, piece_urls: dict[str, tuple[str, ...]]):
     game: Game = game_factory(**{option: True for option in options})
     game_id = str(uuid4())
 
     session_data.game = game
@@ -315,23 +315,25 @@
 
     session_data.own_game = True
     if mode != 'Singleplayer':
         session_data.player = game.board.current_player
     else:
         session_data.player = ""
 
-    game.board.subscribe(AfterMoveEvent, for_all_game_sessions(on_after_move), EventPriority.LOW)
+    game.board.subscribe(AfterMoveEvent, for_all_game_sessions(on_after_move), EventPriority.VERY_LOW + 1)
     game.board.subscribe(AfterTurnChangeEvent, for_all_game_sessions(on_after_turn_change))
     game.subscribe(AfterGameEndEvent, for_all_game_sessions(on_game_end))
 
     put_markdown("""# ChessMaker \n """).style("text-align:center")
     if mode == 'Multiplayer (Private)':
         put_text("Invite URL: " + eval_js("window.location.href.split('?')[0]") + "?game_id=" + session_data.game_id)
     initialize_board()
-    put_markdown("[Docs](https://wolfdwyc.github.io/ChessMaker) - [Source](https://github.com/WolfDWyc/ChessMaker)\nMade by WolfDWyc").style("text-align:center")
+    put_markdown(
+        "[Docs](https://wolfdwyc.github.io/ChessMaker) - [Source](https://github.com/WolfDWyc/ChessMaker)\nMade by WolfDWyc").style(
+        "text-align:center")
 
 
 def start_pywebio_chess_server(
         game_factory: Callable[..., Game],
         supported_options: List[str] = None,
         piece_urls: dict[str, tuple[str, ...]] = PIECE_URLS,
         remote_access: bool = False,
@@ -358,22 +360,23 @@
             if get_query("game_id") not in multiplayer_games:
                 popup("Error", put_error("Game not found"))
             else:
                 join_game(get_query("game_id"))
             return
 
         form_result = input_group('New Game', [
-            radio('Mode', ['Singleplayer', 'Multiplayer (Private)', 'Multiplayer (Public)'], name='mode', value='Singleplayer'),
+            radio('Mode', ['Singleplayer', 'Multiplayer (Private)', 'Multiplayer (Public)'], name='mode',
+                  value='Singleplayer'),
             checkbox('Options',
                      options=supported_options,
                      name='options'),
             actions('Public Games', [
                 {'label': f"Join game: {', '.join(public_game.options) or 'standard'}", 'value': game_id}
                 for game_id, (_, public_game) in public_games.items()
-                ], name='public_games'),
+            ], name='public_games'),
             actions('-', [
                 {'label': 'Create ', 'value': 'create'},
             ], name='action'),
         ])
 
         if form_result['public_games'] is not None:
             public_games.pop(form_result['public_games'])
```

### Comparing `chessmaker-0.3.0/chessmaker/events/event_publisher.py` & `chessmaker-0.3.1/chessmaker/events/event_publisher.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,16 @@
             subscriber.callback(event)
 
     def propagate(self, publisher: 'EventPublisher', event_type: Type[Event]):
         """
         For all events publisher publishes of type event_type, publish them to self
         """
         self._propagating_to[event_type].append(publisher)
+        for subscriber in self._subscribers[event_type]:
+            publisher.subscribe(event_type, subscriber.callback, subscriber.priority)
 
     def propagate_all(self, publisher: 'EventPublisher'):
         """
         For all events publisher publishes, publish them to self
         """
         for event_type in (set(publisher._subscribers.keys()) & set(self._propagating_to.keys())):
             self.propagate(publisher, event_type)
```

### Comparing `chessmaker-0.3.0/LICENSE` & `chessmaker-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.0/pyproject.toml` & `chessmaker-0.3.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chessmaker"
-version = "0.3.0"
+version = "0.3.1"
 description = "An easily extendible chess implementation designed to support any custom rule or feature"
 readme = "README.md"
 authors = ["WolfDWyc <yoavwolfdw@gmail.com>",]
 license = "AGPL-3.0-or-later"
 classifiers = [
 "License :: OSI Approved :: GNU Affero General Public License v3",
 "Programming Language :: Python",
```

### Comparing `chessmaker-0.3.0/README.md` & `chessmaker-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.0/PKG-INFO` & `chessmaker-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chessmaker
-Version: 0.3.0
+Version: 0.3.1
 Summary: An easily extendible chess implementation designed to support any custom rule or feature
 License: AGPL-3.0-or-later
 Keywords: chess
 Author: WolfDWyc
 Author-email: yoavwolfdw@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
```

