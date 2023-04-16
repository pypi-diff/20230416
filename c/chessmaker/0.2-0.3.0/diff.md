# Comparing `tmp/chessmaker-0.2.tar.gz` & `tmp/chessmaker-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chessmaker-0.2.tar", max compression
+gzip compressed data, was "chessmaker-0.3.0.tar", max compression
```

## Comparing `chessmaker-0.2.tar` & `chessmaker-0.3.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0      159 2023-04-12 23:23:56.894161 chessmaker-0.2/chessmaker/__init__.py
--rw-r--r--   0        0        0      240 2023-04-13 13:53:22.478241 chessmaker-0.2/chessmaker/chess/__init__.py
--rw-r--r--   0        0        0      688 2023-04-15 12:04:05.533044 chessmaker-0.2/chessmaker/chess/base/__init__.py
--rw-r--r--   0        0        0     6833 2023-04-13 19:53:48.828413 chessmaker-0.2/chessmaker/chess/base/board.py
--rw-r--r--   0        0        0     1095 2023-04-12 22:57:13.177726 chessmaker-0.2/chessmaker/chess/base/game.py
--rw-r--r--   0        0        0      275 2023-04-13 19:53:48.822414 chessmaker-0.2/chessmaker/chess/base/move_option.py
--rw-r--r--   0        0        0     3515 2023-04-15 12:04:05.524045 chessmaker-0.2/chessmaker/chess/base/piece.py
--rw-r--r--   0        0        0      583 2023-04-12 22:32:25.286163 chessmaker-0.2/chessmaker/chess/base/player.py
--rw-r--r--   0        0        0      241 2023-04-12 22:32:25.006418 chessmaker-0.2/chessmaker/chess/base/position.py
--rw-r--r--   0        0        0      708 2023-04-12 22:57:13.193723 chessmaker-0.2/chessmaker/chess/base/rule.py
--rw-r--r--   0        0        0     2187 2023-04-13 19:53:48.815413 chessmaker-0.2/chessmaker/chess/base/square.py
--rw-r--r--   0        0        0     5299 2023-04-14 16:36:39.857090 chessmaker-0.2/chessmaker/chess/game_factory.py
--rw-r--r--   0        0        0     2460 2023-04-15 15:01:42.502293 chessmaker-0.2/chessmaker/chess/piece_utils.py
--rw-r--r--   0        0        0      319 2023-04-13 13:47:46.308045 chessmaker-0.2/chessmaker/chess/pieces/__init__.py
--rw-r--r--   0        0        0      652 2023-04-13 13:46:31.618457 chessmaker-0.2/chessmaker/chess/pieces/bishop.py
--rw-r--r--   0        0        0     6790 2023-04-14 01:55:25.122905 chessmaker-0.2/chessmaker/chess/pieces/king.py
--rw-r--r--   0        0        0      880 2023-04-13 13:46:31.589457 chessmaker-0.2/chessmaker/chess/pieces/knight.py
--rw-r--r--   0        0        0      191 2023-04-12 23:23:13.134441 chessmaker-0.2/chessmaker/chess/pieces/knook/__init__.py
--rw-r--r--   0        0        0      968 2023-04-15 14:44:35.264730 chessmaker-0.2/chessmaker/chess/pieces/knook/knook.py
--rw-r--r--   0        0        0       30 2023-04-15 15:13:15.595692 chessmaker-0.2/chessmaker/chess/pieces/knook/knookable.py
--rw-r--r--   0        0        0     1177 2023-04-15 15:59:27.992040 chessmaker-0.2/chessmaker/chess/pieces/knook/knookable_knight.py
--rw-r--r--   0        0        0     1209 2023-04-15 15:54:03.824540 chessmaker-0.2/chessmaker/chess/pieces/knook/knookable_rook.py
--rw-r--r--   0        0        0     1607 2023-04-15 15:26:32.334630 chessmaker-0.2/chessmaker/chess/pieces/knook/merge_to_knook.py
--rw-r--r--   0        0        0     5453 2023-04-15 12:04:05.529045 chessmaker-0.2/chessmaker/chess/pieces/pawn.py
--rw-r--r--   0        0        0      785 2023-04-13 13:46:31.572457 chessmaker-0.2/chessmaker/chess/pieces/queen.py
--rw-r--r--   0        0        0     1057 2023-04-13 13:46:31.652457 chessmaker-0.2/chessmaker/chess/pieces/rook.py
--rw-r--r--   0        0        0      332 2023-04-14 13:45:12.352119 chessmaker-0.2/chessmaker/chess/results/__init__.py
--rw-r--r--   0        0        0      478 2023-04-14 12:39:03.945677 chessmaker-0.2/chessmaker/chess/results/capture_all_pieces_to_win.py
--rw-r--r--   0        0        0      584 2023-04-14 12:32:41.047541 chessmaker-0.2/chessmaker/chess/results/checkmate.py
--rw-r--r--   0        0        0      770 2023-04-14 13:40:19.292622 chessmaker-0.2/chessmaker/chess/results/double_check_to_win.py
--rw-r--r--   0        0        0     1134 2023-04-15 02:00:39.838687 chessmaker-0.2/chessmaker/chess/results/no_captures_or_pawn_moves.py
--rw-r--r--   0        0        0      923 2023-04-14 11:49:56.085457 chessmaker-0.2/chessmaker/chess/results/repetition.py
--rw-r--r--   0        0        0      326 2023-04-14 11:49:56.091457 chessmaker-0.2/chessmaker/chess/results/stalemate.py
--rw-r--r--   0        0        0      510 2023-04-15 00:31:09.011728 chessmaker-0.2/chessmaker/chess/results/standard_result.py
--rw-r--r--   0        0        0      345 2023-04-14 13:02:43.693404 chessmaker-0.2/chessmaker/chess/rules/__init__.py
--rw-r--r--   0        0        0     3533 2023-04-13 13:46:31.611456 chessmaker-0.2/chessmaker/chess/rules/beta_decay.py
--rw-r--r--   0        0        0     1875 2023-04-14 14:42:06.954160 chessmaker-0.2/chessmaker/chess/rules/forced_en_passant.py
--rw-r--r--   0        0        0     3670 2023-04-15 12:04:05.521043 chessmaker-0.2/chessmaker/chess/rules/il_vaticano.py
--rw-r--r--   0        0        0      979 2023-04-14 12:49:09.088586 chessmaker-0.2/chessmaker/chess/rules/king_cant_move_to_c2.py
--rw-r--r--   0        0        0     2695 2023-04-12 22:57:13.120723 chessmaker-0.2/chessmaker/chess/rules/knight_boosting.py
--rw-r--r--   0        0        0     2461 2023-04-14 13:33:54.257799 chessmaker-0.2/chessmaker/chess/rules/la_bastarda.py
--rw-r--r--   0        0        0     1871 2023-04-15 12:04:05.540043 chessmaker-0.2/chessmaker/chess/rules/omnipotent_f6_pawn.py
--rw-r--r--   0        0        0     1982 2023-04-14 01:23:32.960857 chessmaker-0.2/chessmaker/chess/rules/siberian_swipe.py
--rw-r--r--   0        0        0       64 2023-04-14 17:14:53.444902 chessmaker-0.2/chessmaker/clients/__init__.py
--rw-r--r--   0        0        0    15728 2023-04-15 15:58:59.834041 chessmaker-0.2/chessmaker/clients/pywebio_ui.py
--rw-r--r--   0        0        0      278 2023-04-12 22:32:25.207165 chessmaker-0.2/chessmaker/cloneable.py
--rw-r--r--   0        0        0      132 2023-04-12 23:20:16.008216 chessmaker-0.2/chessmaker/events/__init__.py
--rw-r--r--   0        0        0      395 2023-04-13 19:53:48.832414 chessmaker-0.2/chessmaker/events/event.py
--rw-r--r--   0        0        0      146 2023-04-14 13:26:17.602659 chessmaker-0.2/chessmaker/events/event_priority.py
--rw-r--r--   0        0        0     3203 2023-04-12 22:57:13.182724 chessmaker-0.2/chessmaker/events/event_publisher.py
--rw-r--r--   0        0        0    35184 2023-04-05 10:50:17.213863 chessmaker-0.2/LICENSE
--rw-r--r--   0        0        0     1096 2023-04-15 16:07:51.887204 chessmaker-0.2/pyproject.toml
--rw-r--r--   0        0        0     1862 2023-04-14 14:15:04.351108 chessmaker-0.2/README.md
--rw-r--r--   0        0        0     2958 1970-01-01 00:00:00.000000 chessmaker-0.2/PKG-INFO
+-rw-r--r--   0        0        0      159 2023-04-12 23:23:56.894161 chessmaker-0.3.0/chessmaker/__init__.py
+-rw-r--r--   0        0        0      240 2023-04-13 13:53:22.478241 chessmaker-0.3.0/chessmaker/chess/__init__.py
+-rw-r--r--   0        0        0      690 2023-04-15 21:57:06.856292 chessmaker-0.3.0/chessmaker/chess/base/__init__.py
+-rw-r--r--   0        0        0     6771 2023-04-16 20:54:04.898469 chessmaker-0.3.0/chessmaker/chess/base/board.py
+-rw-r--r--   0        0        0     1091 2023-04-16 20:29:32.083728 chessmaker-0.3.0/chessmaker/chess/base/game.py
+-rw-r--r--   0        0        0      275 2023-04-13 19:53:48.822414 chessmaker-0.3.0/chessmaker/chess/base/move_option.py
+-rw-r--r--   0        0        0     4006 2023-04-16 20:23:48.040602 chessmaker-0.3.0/chessmaker/chess/base/piece.py
+-rw-r--r--   0        0        0      583 2023-04-12 22:32:25.286163 chessmaker-0.3.0/chessmaker/chess/base/player.py
+-rw-r--r--   0        0        0      241 2023-04-12 22:32:25.006418 chessmaker-0.3.0/chessmaker/chess/base/position.py
+-rw-r--r--   0        0        0      708 2023-04-12 22:57:13.193723 chessmaker-0.3.0/chessmaker/chess/base/rule.py
+-rw-r--r--   0        0        0     2304 2023-04-16 20:16:29.441811 chessmaker-0.3.0/chessmaker/chess/base/square.py
+-rw-r--r--   0        0        0     5299 2023-04-14 16:36:39.857090 chessmaker-0.3.0/chessmaker/chess/game_factory.py
+-rw-r--r--   0        0        0     2460 2023-04-15 15:01:42.502293 chessmaker-0.3.0/chessmaker/chess/piece_utils.py
+-rw-r--r--   0        0        0      319 2023-04-13 13:47:46.308045 chessmaker-0.3.0/chessmaker/chess/pieces/__init__.py
+-rw-r--r--   0        0        0      652 2023-04-13 13:46:31.618457 chessmaker-0.3.0/chessmaker/chess/pieces/bishop.py
+-rw-r--r--   0        0        0     6790 2023-04-16 20:01:11.181718 chessmaker-0.3.0/chessmaker/chess/pieces/king.py
+-rw-r--r--   0        0        0      880 2023-04-13 13:46:31.589457 chessmaker-0.3.0/chessmaker/chess/pieces/knight.py
+-rw-r--r--   0        0        0      191 2023-04-12 23:23:13.134441 chessmaker-0.3.0/chessmaker/chess/pieces/knook/__init__.py
+-rw-r--r--   0        0        0      968 2023-04-15 14:44:35.264730 chessmaker-0.3.0/chessmaker/chess/pieces/knook/knook.py
+-rw-r--r--   0        0        0       30 2023-04-15 15:13:15.595692 chessmaker-0.3.0/chessmaker/chess/pieces/knook/knookable.py
+-rw-r--r--   0        0        0     1184 2023-04-16 21:13:06.169907 chessmaker-0.3.0/chessmaker/chess/pieces/knook/knookable_knight.py
+-rw-r--r--   0        0        0     1216 2023-04-15 21:58:00.111375 chessmaker-0.3.0/chessmaker/chess/pieces/knook/knookable_rook.py
+-rw-r--r--   0        0        0     1615 2023-04-15 21:58:00.012862 chessmaker-0.3.0/chessmaker/chess/pieces/knook/merge_to_knook.py
+-rw-r--r--   0        0        0     5506 2023-04-16 20:01:11.191719 chessmaker-0.3.0/chessmaker/chess/pieces/pawn.py
+-rw-r--r--   0        0        0      785 2023-04-13 13:46:31.572457 chessmaker-0.3.0/chessmaker/chess/pieces/queen.py
+-rw-r--r--   0        0        0     1057 2023-04-16 21:13:16.019354 chessmaker-0.3.0/chessmaker/chess/pieces/rook.py
+-rw-r--r--   0        0        0      332 2023-04-14 13:45:12.352119 chessmaker-0.3.0/chessmaker/chess/results/__init__.py
+-rw-r--r--   0        0        0      478 2023-04-14 12:39:03.945677 chessmaker-0.3.0/chessmaker/chess/results/capture_all_pieces_to_win.py
+-rw-r--r--   0        0        0      584 2023-04-14 12:32:41.047541 chessmaker-0.3.0/chessmaker/chess/results/checkmate.py
+-rw-r--r--   0        0        0      801 2023-04-16 21:29:32.511999 chessmaker-0.3.0/chessmaker/chess/results/double_check_to_win.py
+-rw-r--r--   0        0        0     1134 2023-04-15 02:00:39.838687 chessmaker-0.3.0/chessmaker/chess/results/no_captures_or_pawn_moves.py
+-rw-r--r--   0        0        0      923 2023-04-14 11:49:56.085457 chessmaker-0.3.0/chessmaker/chess/results/repetition.py
+-rw-r--r--   0        0        0      326 2023-04-14 11:49:56.091457 chessmaker-0.3.0/chessmaker/chess/results/stalemate.py
+-rw-r--r--   0        0        0      510 2023-04-15 00:31:09.011728 chessmaker-0.3.0/chessmaker/chess/results/standard_result.py
+-rw-r--r--   0        0        0      345 2023-04-14 13:02:43.693404 chessmaker-0.3.0/chessmaker/chess/rules/__init__.py
+-rw-r--r--   0        0        0     3533 2023-04-13 13:46:31.611456 chessmaker-0.3.0/chessmaker/chess/rules/beta_decay.py
+-rw-r--r--   0        0        0     1875 2023-04-14 14:42:06.954160 chessmaker-0.3.0/chessmaker/chess/rules/forced_en_passant.py
+-rw-r--r--   0        0        0     3670 2023-04-15 12:04:05.521043 chessmaker-0.3.0/chessmaker/chess/rules/il_vaticano.py
+-rw-r--r--   0        0        0      979 2023-04-14 12:49:09.088586 chessmaker-0.3.0/chessmaker/chess/rules/king_cant_move_to_c2.py
+-rw-r--r--   0        0        0     2695 2023-04-12 22:57:13.120723 chessmaker-0.3.0/chessmaker/chess/rules/knight_boosting.py
+-rw-r--r--   0        0        0     2461 2023-04-14 13:33:54.257799 chessmaker-0.3.0/chessmaker/chess/rules/la_bastarda.py
+-rw-r--r--   0        0        0     1871 2023-04-15 12:04:05.540043 chessmaker-0.3.0/chessmaker/chess/rules/omnipotent_f6_pawn.py
+-rw-r--r--   0        0        0     1982 2023-04-14 01:23:32.960857 chessmaker-0.3.0/chessmaker/chess/rules/siberian_swipe.py
+-rw-r--r--   0        0        0       64 2023-04-14 17:14:53.444902 chessmaker-0.3.0/chessmaker/clients/__init__.py
+-rw-r--r--   0        0        0    16008 2023-04-16 21:34:55.732847 chessmaker-0.3.0/chessmaker/clients/pywebio_ui.py
+-rw-r--r--   0        0        0      278 2023-04-12 22:32:25.207165 chessmaker-0.3.0/chessmaker/cloneable.py
+-rw-r--r--   0        0        0      149 2023-04-15 21:57:06.796292 chessmaker-0.3.0/chessmaker/events/__init__.py
+-rw-r--r--   0        0        0      395 2023-04-13 19:53:48.832414 chessmaker-0.3.0/chessmaker/events/event.py
+-rw-r--r--   0        0        0      146 2023-04-14 13:26:17.602659 chessmaker-0.3.0/chessmaker/events/event_priority.py
+-rw-r--r--   0        0        0     3689 2023-04-16 20:12:32.196037 chessmaker-0.3.0/chessmaker/events/event_publisher.py
+-rw-r--r--   0        0        0    35184 2023-04-05 10:50:17.213863 chessmaker-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1098 2023-04-16 21:19:33.850028 chessmaker-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1862 2023-04-14 14:15:04.351108 chessmaker-0.3.0/README.md
+-rw-r--r--   0        0        0     2960 1970-01-01 00:00:00.000000 chessmaker-0.3.0/PKG-INFO
```

### Comparing `chessmaker-0.2/chessmaker/chess/base/board.py` & `chessmaker-0.3.0/chessmaker/chess/base/board.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,74 +1,81 @@
 import itertools
 import warnings
 from dataclasses import dataclass
 from typing import Iterable, Iterator
 
-from chessmaker.chess.base.piece import Piece, PieceEventTypes, AfterMoveEvent
+from chessmaker.cloneable import Cloneable
+from chessmaker.chess.base.piece import Piece, PIECE_EVENT_TYPES, AfterMoveEvent
 from chessmaker.chess.base.player import Player
 from chessmaker.chess.base.position import Position
 from chessmaker.chess.base.rule import Rule
-from chessmaker.chess.base.square import Square, BeforeAddPieceEvent, AfterRemovePieceEvent, AfterAddPieceEvent, \
-    BeforeRemovePieceEvent
-from chessmaker.cloneable import Cloneable
-from chessmaker.events import EventPublisher, Event, CancellableEvent
+from chessmaker.chess.base.square import Square, SQUARE_EVENT_TYPES, AfterAddPieceEvent
+from chessmaker.events import event_publisher, Event, CancellableEvent, EventPublisher, EventPriority
 
 
 @dataclass(frozen=True)
 class AfterNewPieceEvent(Event):
     piece: Piece
 
+
 @dataclass(frozen=True)
 class AfterRemoveSquareEvent(Event):
     position: Position
     square: Square
 
+
 @dataclass(frozen=True)
 class BeforeRemoveSquareEvent(AfterRemoveSquareEvent):
     pass
 
+
 @dataclass(frozen=True)
 class AfterAddSquareEvent(Event):
     position: Position
     square: Square
 
+
 @dataclass(frozen=True)
 class BeforeAddSquareEvent(AfterAddSquareEvent):
     def set_square(self, square: Square):
         self._set("square", square)
 
+
 @dataclass(frozen=True)
 class BeforeTurnChangeEvent(CancellableEvent):
     board: "Board"
     next_player: Player
 
     def set_next_player(self, next_player: Player):
         self._set("next_player", next_player)
 
+
 @dataclass(frozen=True)
 class AfterTurnChangeEvent(Event):
     board: "Board"
     player: Player
 
-class Board(EventPublisher[BeforeAddPieceEvent | AfterAddPieceEvent | BeforeRemovePieceEvent | AfterRemovePieceEvent
-                           | PieceEventTypes | AfterNewPieceEvent | BeforeAddSquareEvent | AfterAddSquareEvent
-                           | BeforeRemoveSquareEvent | AfterRemoveSquareEvent | BeforeTurnChangeEvent
-                           | AfterTurnChangeEvent], Cloneable):
+
+@event_publisher(*SQUARE_EVENT_TYPES, *PIECE_EVENT_TYPES, BeforeAddSquareEvent, AfterAddSquareEvent,
+                 BeforeRemoveSquareEvent, AfterRemoveSquareEvent, BeforeTurnChangeEvent, AfterTurnChangeEvent,
+                 AfterNewPieceEvent)
+class Board(Cloneable, EventPublisher):
     def __init__(
             self,
             squares: list[list[Square | None]],
             players: list[Player],
             turn_iterator: Iterator[Player],
             rules: list[Rule] = None
-         ):
+    ):
         super().__init__()
         # Use the max length for each dimension to determine the size of the board
         self.size = (max(len(row) for row in squares), len(squares))
         self._squares = squares
-        self._squares_to_positions = {square: Position(x, y) for y, row in enumerate(squares) for x, square in enumerate(row) if square is not None}
+        self._squares_to_positions = {square: Position(x, y) for y, row in enumerate(squares) for x, square in
+                                      enumerate(row) if square is not None}
         self.players = players
         self.turn_iterator = turn_iterator
         self.current_player = next(self.turn_iterator)
         self.rules = rules or []
 
         # Subscribe to the events of each square
         for row in self._squares:
@@ -77,20 +84,19 @@
                     # TODO: Subscribe to new squares
                     self.propagate_all(square)
                     square._board = self
                     if square.piece is not None:
                         self._on_after_add_piece(AfterAddPieceEvent(square, square.piece))
 
         self.subscribe(AfterAddPieceEvent, self._on_after_add_piece)
-        self.subscribe(AfterMoveEvent, self._on_after_move)
+        self.subscribe(AfterMoveEvent, self._on_after_move, EventPriority.VERY_LOW)
 
         for rule in self.rules:
             rule.on_join_board(self)
 
-
     # TODO: Implement this in a way that detects actual new pieces and not moved pieces
     def _on_after_add_piece(self, event: AfterAddPieceEvent):
         piece: Piece = event.piece
         if piece._board is None:
             piece._board = self
             piece.on_join_board()
             self.publish(AfterNewPieceEvent(piece))
@@ -107,15 +113,15 @@
 
     def __getitem__(self, position: Position) -> Square | None:
         return self._squares[position.y][position.x]
 
     def __setitem__(self, position: Position, square: Square | None):
         if square == self._squares[position.y][position.x]:
             warnings.warn("Setting a square to the same square doesn't have any effect, did you mean to to change "
-                              "the piece on the square?", RuntimeWarning)
+                          "the piece on the square?", RuntimeWarning)
             return
 
         old_square = self._squares[position.y][position.x]
         if old_square is not None:
             self.publish(BeforeRemoveSquareEvent(position, old_square))
 
         if square is None:
@@ -165,8 +171,7 @@
         self.turn_iterator = turn_iterators[0]
         return Board(
             [[square.clone() if square is not None else None for square in row] for row in self._squares],
             self.players,
             turn_iterators[1],
             [rule.clone() for rule in self.rules]
         )
-
```

### Comparing `chessmaker-0.2/chessmaker/chess/base/game.py` & `chessmaker-0.3.0/chessmaker/chess/base/game.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from dataclasses import dataclass
-from dataclasses import dataclass
 from typing import Callable
 
 from chessmaker.chess.base.board import Board, AfterTurnChangeEvent
-from chessmaker.events import Event, EventPublisher
+from chessmaker.events import Event, event_publisher, EventPublisher
 
 
 @dataclass(frozen=True)
 class AfterGameEndEvent(Event):
     game: "Game"
     result: str
 
-class Game(EventPublisher[AfterGameEndEvent]):
+
+@event_publisher(AfterGameEndEvent)
+class Game(EventPublisher):
     def __init__(
             self,
             board: Board,
             get_result: Callable[[Board], str | None],
-        ):
+    ):
         super().__init__()
         self.board: Board = board
         self._get_result = get_result
         self.result = None
 
         self.board.subscribe(AfterTurnChangeEvent, self._on_after_turn_change)
 
-
     def _on_after_turn_change(self, _: AfterTurnChangeEvent):
         self.result = self._get_result(self.board)
         if self.result is not None:
             self.turn_iterator = []
             self.current_player = None
             self.publish(AfterGameEndEvent(self, self.result))
```

### Comparing `chessmaker-0.2/chessmaker/chess/base/piece.py` & `chessmaker-0.3.0/chessmaker/chess/base/piece.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from abc import abstractmethod
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Iterable
 
+from chessmaker.chess.base.square import AfterAddPieceEvent, AfterRemovePieceEvent
 from chessmaker.chess.base.move_option import MoveOption
 from chessmaker.chess.base.player import Player
 from chessmaker.cloneable import Cloneable
-from chessmaker.events import EventPublisher, Event, CancellableEvent
+from chessmaker.events import event_publisher, Event, CancellableEvent, EventPublisher
 
 if TYPE_CHECKING:
     from chessmaker.chess.base.board import Board
 
 
 @dataclass(frozen=True)
 class AfterGetMoveOptionsEvent(Event):
@@ -38,35 +39,40 @@
     captured_piece: "Piece"
 
 
 class BeforeCapturedEvent(AfterCapturedEvent):
     pass
 
 
-PieceEventTypes = AfterGetMoveOptionsEvent | BeforeGetMoveOptionsEvent | AfterMoveEvent | BeforeMoveEvent | \
-                  AfterCapturedEvent | BeforeCapturedEvent
+PIECE_EVENT_TYPES = (BeforeGetMoveOptionsEvent, AfterGetMoveOptionsEvent, BeforeMoveEvent, AfterMoveEvent,
+                     BeforeCapturedEvent, AfterCapturedEvent)
 
 
-class Piece(EventPublisher[PieceEventTypes], Cloneable):
+@event_publisher(*PIECE_EVENT_TYPES)
+class Piece(Cloneable, EventPublisher):
     def __init__(self, player: Player):
         super().__init__()
         self._player = player
         self._board: Board = None
+        self._move_options = None
 
     def __repr__(self):
         return f"{self.__class__.__name__} ({self.player})"
 
     def get_move_options(self) -> Iterable[MoveOption]:
+        if False:
+            return self._move_options
         move_options = self._get_move_options()
 
         before_get_move_options_event = BeforeGetMoveOptionsEvent(self, move_options)
         self.publish(before_get_move_options_event)
         move_options = before_get_move_options_event.move_options
         self.publish(AfterGetMoveOptionsEvent(self, move_options))
 
+        self._move_options = move_options
         return move_options
 
     def move(self, move_option: MoveOption):
         before_move_event = BeforeMoveEvent(self, move_option)
         self.publish(before_move_event)
         if before_move_event.cancelled:
             return
@@ -85,15 +91,19 @@
             capture_piece.publish(AfterCapturedEvent(capture_piece))
 
         destination.piece = self
 
         self.publish(AfterMoveEvent(self, move_option))
 
     def on_join_board(self):
-        pass
+        self.board.subscribe(AfterAddPieceEvent, self._on_after_change_piece)
+        self.board.subscribe(AfterRemovePieceEvent, self._on_after_change_piece)
+
+    def _on_after_change_piece(self, _: Event):
+        self._move_options = None
 
     @property
     def player(self):
         return self._player
 
     @property
     def position(self):
```

### Comparing `chessmaker-0.2/chessmaker/chess/base/player.py` & `chessmaker-0.3.0/chessmaker/chess/base/player.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.2/chessmaker/chess/base/rule.py` & `chessmaker-0.3.0/chessmaker/chess/base/rule.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.2/chessmaker/chess/base/square.py` & `chessmaker-0.3.0/chessmaker/chess/base/square.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,58 +1,66 @@
 import warnings
 from dataclasses import dataclass
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Optional
 
-from chessmaker.chess.base.piece import Piece
 from chessmaker.cloneable import Cloneable
-from chessmaker.events import Event, EventPublisher
+from chessmaker.events import Event, event_publisher, EventPublisher
 
 if TYPE_CHECKING:
+    from chessmaker.chess.base.piece import Piece
     from chessmaker.chess.base.board import Board
 
+
 @dataclass(frozen=True)
 class AfterAddPieceEvent(Event):
     square: "Square"
-    piece: Piece
+    piece: "Piece"
+
 
 class BeforeAddPieceEvent(AfterAddPieceEvent):
-    def set_piece(self, piece: Piece):
+    def set_piece(self, piece: "Piece"):
         self._set("piece", piece)
 
+
 @dataclass(frozen=True)
 class BeforeRemovePieceEvent(Event):
     square: "Square"
-    piece: Piece
+    piece: "Piece"
+
 
 class AfterRemovePieceEvent(BeforeRemovePieceEvent):
     pass
 
 
-class Square(EventPublisher[BeforeAddPieceEvent | AfterAddPieceEvent | BeforeRemovePieceEvent | AfterRemovePieceEvent], Cloneable):
-    def __init__(self, piece: Piece | None = None):
+SQUARE_EVENT_TYPES = (BeforeAddPieceEvent, AfterAddPieceEvent, BeforeRemovePieceEvent, AfterRemovePieceEvent)
+
+
+@event_publisher(*SQUARE_EVENT_TYPES)
+class Square(Cloneable, EventPublisher):
+    def __init__(self, piece: Optional["Piece"] = None):
         super().__init__()
         self._piece = piece
         self._board: Board = None
 
     @property
-    def piece(self) -> Piece:
+    def piece(self) -> "Piece":
         return self._piece
 
     @property
     def position(self):
         return self.board._get_square_position(self)
 
     @property
     def board(self):
         if self._board is None:
             raise Exception("Square is not on the board yet")
         return self._board
 
     @piece.setter
-    def piece(self, piece: Piece):
+    def piece(self, piece: "Piece"):
         old_piece = self._piece
 
         if piece is old_piece:
             warnings.warn("Setting the same piece on the square has no effect", RuntimeWarning)
             return
 
         if old_piece is not None:
```

### Comparing `chessmaker-0.2/chessmaker/chess/game_factory.py` & `chessmaker-0.3.0/chessmaker/chess/game_factory.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.2/chessmaker/chess/piece_utils.py` & `chessmaker-0.3.0/chessmaker/chess/piece_utils.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.2/chessmaker/chess/pieces/bishop.py` & `chessmaker-0.3.0/chessmaker/chess/pieces/bishop.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.2/chessmaker/chess/pieces/king.py` & `chessmaker-0.3.0/chessmaker/chess/pieces/king.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,61 +1,63 @@
 from dataclasses import dataclass
 from functools import partial
 from typing import Iterable
 
 from chessmaker.chess.base.board import AfterNewPieceEvent
 from chessmaker.chess.base.move_option import MoveOption
-from chessmaker.chess.base.piece import Piece, PieceEventTypes, BeforeMoveEvent, BeforeGetMoveOptionsEvent
+from chessmaker.chess.base.piece import Piece, BeforeMoveEvent, BeforeGetMoveOptionsEvent
 from chessmaker.chess.base.player import Player
 from chessmaker.chess.base.position import Position
 from chessmaker.chess.base.square import Square
 from chessmaker.chess.piece_utils import filter_uncapturable_positions, is_in_board, iterate_until_blocked, \
     positions_to_move_options
 from chessmaker.chess.pieces.rook import Rook
-from chessmaker.events import Event, EventPublisher, EventPriority
+from chessmaker.events import Event, event_publisher, EventPriority
 
 
 @dataclass(frozen=True)
 class AfterCastleEvent(Event):
     king: "King"
     rook: Rook
 
+
 @dataclass(frozen=True)
 class BeforeCastleEvent(AfterCastleEvent):
     king_destination: Square
     rook_destination: Square
 
     def set_king_destination(self, king_destination: Square):
         self._set("king_destination", king_destination)
 
     def set_rook_destination(self, rook_destination: Square):
         self._set("rook_destination", rook_destination)
 
-class King(Piece, EventPublisher[PieceEventTypes | AfterCastleEvent | BeforeCastleEvent]):
+
+@event_publisher(AfterCastleEvent, BeforeCastleEvent)
+class King(Piece):
     def __init__(
             self,
             player: Player,
             moved: bool = False,
             attackable: bool = False,
             castling_directions: tuple[tuple[int, int], ...] = ((1, 0), (-1, 0))
     ):
         super().__init__(player)
         self._moved = moved
         self._attackable = attackable
         self._castling_directions = castling_directions
         self.subscribe(BeforeMoveEvent, self._on_before_move, EventPriority.VERY_HIGH)
 
-
-
     @classmethod
     @property
     def name(cls):
         return "King"
 
     def on_join_board(self):
+        super().on_join_board()
         if not self._attackable:
             for piece in self.board.get_pieces():
                 if piece.player == self.player:
                     piece.subscribe(BeforeGetMoveOptionsEvent, self._on_before_get_move_options)
             self.board.subscribe(AfterNewPieceEvent, self._on_after_new_piece)
 
     def _on_after_new_piece(self, event: AfterNewPieceEvent):
@@ -70,15 +72,14 @@
             move_options = piece.get_move_options()
 
             for move_option in move_options:
                 if self.position in move_option.captures:
                     return True
         return False
 
-
     def _is_attacked_after_move(self, piece: Piece, move_option: MoveOption) -> bool:
         board_clone = self.board.clone()
         self_clone = board_clone[self.position].piece
         piece_clone = board_clone[piece.position].piece
         piece_clone.move(move_option)
         return self_clone.is_attacked()
 
@@ -130,14 +131,15 @@
                         last_piece.player == self.player and
                         isinstance(last_piece, Rook) and
                         not last_piece.moved and
                         not self._moved):
                     move_options.append(MoveOption(line[1], extra=dict(castle=line[-1])))
 
         return move_options
+
     def _on_before_move(self, event: BeforeMoveEvent):
         if "castle" in event.move_option.extra:
             move_option = event.move_option
             destination = self.board[move_option.position]
 
             rook_source = self.board[Position(*move_option.extra["castle"])]
             rook_destination = self.board[Position(
```

### Comparing `chessmaker-0.2/chessmaker/chess/pieces/knight.py` & `chessmaker-0.3.0/chessmaker/chess/pieces/knight.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.2/chessmaker/chess/pieces/knook/knook.py` & `chessmaker-0.3.0/chessmaker/chess/pieces/knook/knook.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.2/chessmaker/chess/pieces/knook/knookable_knight.py` & `chessmaker-0.3.0/chessmaker/chess/pieces/knook/knookable_knight.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from functools import partial
 from itertools import chain
 
-from chessmaker.chess.base.piece import AfterMoveEvent, PieceEventTypes
+from chessmaker.chess.base.piece import AfterMoveEvent
 from chessmaker.chess.pieces import knight
 from chessmaker.chess.pieces.knight import Knight
-from chessmaker.chess.pieces.knook import merge_to_knook
 from chessmaker.chess.pieces.knook.knookable import Knookable
 from chessmaker.chess.piece_utils import is_in_board
-from chessmaker.events import EventPriority, EventPublisher
+from chessmaker.chess.pieces.knook.merge_to_knook import get_merge_move_options, merge_after_move, \
+    MERGE_TO_KNOOK_EVENT_TYPES
+from chessmaker.events import EventPriority, event_publisher
 
 
-class KnookableKnight(Knight, EventPublisher[PieceEventTypes | merge_to_knook.MergeToKnookEventTypes], Knookable):
+@event_publisher(*MERGE_TO_KNOOK_EVENT_TYPES)
+class KnookableKnight(Knight, Knookable):
     def __init__(self, player):
         super().__init__(player)
-        self.subscribe(AfterMoveEvent, merge_to_knook.on_after_move, EventPriority.VERY_HIGH)
+        self.subscribe(AfterMoveEvent, merge_after_move, EventPriority.VERY_HIGH)
 
     def _get_move_options(self):
         positions = [self.position.offset(*offset) for offset in knight.MOVE_OFFSETS]
         positions = list(filter(partial(is_in_board, self.board), positions))
-        merge_move_options = merge_to_knook.get_merge_move_options(self, positions)
+        merge_move_options = get_merge_move_options(self, positions)
 
         return chain(super()._get_move_options(), merge_move_options)
 
     def clone(self):
         return KnookableKnight(self.player)
```

### Comparing `chessmaker-0.2/chessmaker/chess/pieces/knook/knookable_rook.py` & `chessmaker-0.3.0/chessmaker/chess/pieces/knook/knookable_rook.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from itertools import chain
 from typing import Iterable
 
 from chessmaker.chess.base.move_option import MoveOption
-from chessmaker.chess.base.piece import AfterMoveEvent, PieceEventTypes
+from chessmaker.chess.base.piece import AfterMoveEvent
 from chessmaker.chess.base.player import Player
-from chessmaker.chess.pieces.knook import merge_to_knook
 from chessmaker.chess.pieces.knook.knookable import Knookable
 from chessmaker.chess.piece_utils import get_straight_until_blocked
+from chessmaker.chess.pieces.knook.merge_to_knook import get_merge_move_options, MERGE_TO_KNOOK_EVENT_TYPES, \
+    merge_after_move
 from chessmaker.chess.pieces.rook import Rook
-from chessmaker.events import EventPriority, EventPublisher
+from chessmaker.events import EventPriority, event_publisher
 
 
-class KnookableRook(Rook, EventPublisher[PieceEventTypes | merge_to_knook.MergeToKnookEventTypes], Knookable):
+@event_publisher(*MERGE_TO_KNOOK_EVENT_TYPES)
+class KnookableRook(Rook, Knookable):
     def __init__(self, player: Player, moved: bool = False):
         super().__init__(player, moved)
-        self.subscribe(AfterMoveEvent, merge_to_knook.on_after_move, EventPriority.VERY_HIGH)
+        self.subscribe(AfterMoveEvent, merge_after_move, EventPriority.VERY_HIGH)
 
     def _get_move_options(self) -> Iterable[MoveOption]:
         positions = list(get_straight_until_blocked(self))
-        merge_move_options = merge_to_knook.get_merge_move_options(self, positions)
+        merge_move_options = get_merge_move_options(self, positions)
 
         return chain(super()._get_move_options(), merge_move_options)
 
     def clone(self):
         return KnookableRook(self.player, self.moved)
```

### Comparing `chessmaker-0.2/chessmaker/chess/pieces/knook/merge_to_knook.py` & `chessmaker-0.3.0/chessmaker/chess/pieces/knook/merge_to_knook.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,27 +16,27 @@
 
 
 class BeforeMergeToKnookEvent(AfterMergeToKnookEvent):
     def set_knook(self, knook: Knook):
         self._set("knook", knook)
 
 
-MergeToKnookEventTypes = AfterMergeToKnookEvent | BeforeMergeToKnookEvent
+MERGE_TO_KNOOK_EVENT_TYPES = (BeforeMergeToKnookEvent, AfterMergeToKnookEvent)
 
 
 def get_merge_move_options(piece: Piece, positions: Iterable[Position]) -> Iterable[MoveOption]:
     for position in positions:
         position_piece = piece.board[position].piece
 
         if position_piece is not None and position_piece.player == piece.player:
             if isinstance(position_piece, Knookable) and not isinstance(position_piece, type(piece)):
                 yield MoveOption(position, extra=dict(knook=True))
 
 
-def on_after_move(event: AfterMoveEvent):
+def merge_after_move(event: AfterMoveEvent):
     if event.move_option.extra.get("knook"):
         piece = event.piece
         before_merge_to_knook_event = BeforeMergeToKnookEvent(piece, Knook(event.piece.player))
         event.piece.publish(before_merge_to_knook_event)
         knook = before_merge_to_knook_event.knook
         piece.board[event.move_option.position].piece = knook
         piece.publish(AfterMergeToKnookEvent(piece, knook))
```

### Comparing `chessmaker-0.2/chessmaker/chess/pieces/pawn.py` & `chessmaker-0.3.0/chessmaker/chess/pieces/pawn.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 import dataclasses
 from dataclasses import dataclass
 from enum import Enum
 from typing import Iterable, Type
 
-from chessmaker.chess.base.board import AfterNewPieceEvent
 from chessmaker.chess.base.game import AfterTurnChangeEvent
 from chessmaker.chess.base.move_option import MoveOption
 from chessmaker.chess.base.piece import Piece, BeforeMoveEvent, AfterMoveEvent, BeforeCapturedEvent, AfterCapturedEvent
 from chessmaker.chess.base.player import Player
 from chessmaker.chess.base.position import Position
 from chessmaker.chess.piece_utils import iterate_until_blocked, is_in_board
-from chessmaker.events import EventPriority, Event
+from chessmaker.events import EventPriority, Event, event_publisher
 
 @dataclass(frozen=True)
 class AfterPromotionEvent(Event):
     pawn: "Pawn"
     promotion: Piece
 
 @dataclass(frozen=True)
 class BeforePromotionEvent(AfterPromotionEvent):
     def set_promotion(self, promotion: Piece):
         self._set("promotion", promotion)
 
+
+@event_publisher(BeforePromotionEvent, AfterPromotionEvent)
 class Pawn(Piece):
     class Direction(Enum):
         UP = -1
         DOWN = 1
 
     @classmethod
     @property
@@ -48,14 +49,15 @@
         self._moved_turns_ago = moved_turns_ago
         self._last_position = last_position
 
         self.subscribe(BeforeMoveEvent, self._on_before_move, EventPriority.VERY_HIGH)
         self.subscribe(AfterMoveEvent, self._on_after_move, EventPriority.VERY_HIGH)
 
     def on_join_board(self):
+        super().on_join_board()
         self.board.subscribe(AfterTurnChangeEvent, self._on_turn_change)
 
     def _on_turn_change(self, _: AfterTurnChangeEvent):
         if self._moved_turns_ago != -1:
             self._moved_turns_ago += 1
 
     def _get_move_options(self) -> Iterable[MoveOption]:
```

### Comparing `chessmaker-0.2/chessmaker/chess/pieces/queen.py` & `chessmaker-0.3.0/chessmaker/chess/pieces/queen.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.2/chessmaker/chess/pieces/rook.py` & `chessmaker-0.3.0/chessmaker/chess/pieces/rook.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.2/chessmaker/chess/results/checkmate.py` & `chessmaker-0.3.0/chessmaker/chess/results/checkmate.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.2/chessmaker/chess/results/double_check_to_win.py` & `chessmaker-0.3.0/chessmaker/chess/results/double_check_to_win.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,10 +11,11 @@
         attacker_count = 0
         position = king.position
         for piece in board.get_pieces():
             if piece.player != current_player:
                 for move_option in piece.get_move_options():
                     if position in move_option.captures:
                         attacker_count += 1
+                        break
 
         if attacker_count >= 2:
             return f"Double check - {current_player.name} loses"
```

### Comparing `chessmaker-0.2/chessmaker/chess/results/no_captures_or_pawn_moves.py` & `chessmaker-0.3.0/chessmaker/chess/results/no_captures_or_pawn_moves.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.2/chessmaker/chess/results/repetition.py` & `chessmaker-0.3.0/chessmaker/chess/results/repetition.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.2/chessmaker/chess/rules/beta_decay.py` & `chessmaker-0.3.0/chessmaker/chess/rules/beta_decay.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.2/chessmaker/chess/rules/forced_en_passant.py` & `chessmaker-0.3.0/chessmaker/chess/rules/forced_en_passant.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.2/chessmaker/chess/rules/il_vaticano.py` & `chessmaker-0.3.0/chessmaker/chess/rules/il_vaticano.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.2/chessmaker/chess/rules/king_cant_move_to_c2.py` & `chessmaker-0.3.0/chessmaker/chess/rules/king_cant_move_to_c2.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.2/chessmaker/chess/rules/knight_boosting.py` & `chessmaker-0.3.0/chessmaker/chess/rules/knight_boosting.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.2/chessmaker/chess/rules/la_bastarda.py` & `chessmaker-0.3.0/chessmaker/chess/rules/la_bastarda.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.2/chessmaker/chess/rules/omnipotent_f6_pawn.py` & `chessmaker-0.3.0/chessmaker/chess/rules/omnipotent_f6_pawn.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.2/chessmaker/chess/rules/siberian_swipe.py` & `chessmaker-0.3.0/chessmaker/chess/rules/siberian_swipe.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.2/chessmaker/clients/pywebio_ui.py` & `chessmaker-0.3.0/chessmaker/clients/pywebio_ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import time
 from copy import deepcopy
 from dataclasses import dataclass, field
 from functools import partial
 from itertools import groupby
 from typing import Callable, List, ParamSpec, TypeVar, Optional, Any
 from uuid import uuid4
 
@@ -17,14 +18,15 @@
 from chessmaker.chess.base.game import Game, AfterTurnChangeEvent, AfterGameEndEvent
 from chessmaker.chess.base.move_option import MoveOption
 from chessmaker.chess.base.piece import Piece, AfterMoveEvent
 from chessmaker.chess.base.player import Player
 from chessmaker.chess.base.position import Position
 from chessmaker.chess.base.square import Square
 from chessmaker.chess.game_factory import create_game
+from chessmaker.events import EventPriority
 
 CSS = """
 .pywebio {padding-top: 0} .markdown-body table {display:table; width:250px; margin:10px auto;}
 .markdown-body table th {padding:0;}
 .markdown-body p {margin:0;}
 .markdown-body table td {font-weight:bold; padding:0; line-height:80px; border: 0}
 .markdown-body table tr {border: 0}
@@ -53,15 +55,15 @@
     game: Game
     options: list[str]
     sessions: List[ThreadBasedSession] = field(default_factory=list)
     colors: dict[str, str] = field(default_factory=dict)
     piece_urls: dict[str, tuple[str, ...]] = field(default_factory=lambda: PIECE_URLS)
 
 
-public_games: dict[str, MultiplayerGame] = {}
+public_games: dict[str, tuple[float, MultiplayerGame]] = {}
 multiplayer_games: dict[str, MultiplayerGame] = {}
 
 
 PS = ParamSpec("PS")
 RT = TypeVar("RT")
 
 
@@ -277,24 +279,24 @@
             grid[index].insert(0, put_text(str(number)))
         grid.insert(0, [put_text()] + [put_text(chr(index + 65)) for index in range(board.size[0])])
 
         put_table(grid).style("text-align: center")
 
     session_data.last_board_pieces = get_board_strings(board)
 
+
 def join_game(game_id: str):
     multiplayer_games[game_id].sessions.append(ThreadBasedSession.get_current_session())
     game = multiplayer_games[game_id].game
 
     session_data.game = game
     session_data.game_id = game_id
     session_data.own_game = False
 
     put_markdown("""# ChessMaker \n """).style("text-align:center")
-    put_text("Invite URL: " + eval_js("window.location.href.split('?')[0]") + "?game_id=" + session_data.game_id)
     initialize_board()
     put_markdown("[Docs](https://wolfdwyc.github.io/ChessMaker) - [Source](https://github.com/WolfDWyc/ChessMaker)\nMade by WolfDWyc").style("text-align:center")
 
 
 def new_game(game_factory: Callable[..., Game], options: list[str], mode: str, piece_urls: dict[str, tuple[str, ...]]):
     game: Game = game_factory(**{option: True for option in options})
     game_id = str(uuid4())
@@ -305,23 +307,23 @@
     multiplayer_game = MultiplayerGame(game, options, [ThreadBasedSession.get_current_session()], {}, piece_urls)
     colors = ['w', 'b']
     for player in game.board.players:
         multiplayer_game.colors[player.name] = colors.pop(0)
 
     multiplayer_games[game_id] = multiplayer_game
     if mode == 'Multiplayer (Public)':
-        public_games[game_id] = multiplayer_game
+        public_games[game_id] = (time.time(), multiplayer_game)
 
     session_data.own_game = True
     if mode != 'Singleplayer':
         session_data.player = game.board.current_player
     else:
         session_data.player = ""
 
-    game.board.subscribe(AfterMoveEvent, for_all_game_sessions(on_after_move))
+    game.board.subscribe(AfterMoveEvent, for_all_game_sessions(on_after_move), EventPriority.LOW)
     game.board.subscribe(AfterTurnChangeEvent, for_all_game_sessions(on_after_turn_change))
     game.subscribe(AfterGameEndEvent, for_all_game_sessions(on_game_end))
 
     put_markdown("""# ChessMaker \n """).style("text-align:center")
     if mode == 'Multiplayer (Private)':
         put_text("Invite URL: " + eval_js("window.location.href.split('?')[0]") + "?game_id=" + session_data.game_id)
     initialize_board()
@@ -341,29 +343,36 @@
 
     @config(
         title="ChessMaker",
         description="An easily extendible chess implementation designed to support any custom rule or feature.",
         css_style=CSS
     )
     def main():
+        games_to_remove = []
+        for game_id, (time_created, game) in public_games.items():
+            if time.time() - time_created > 5 * 60:
+                games_to_remove.append(game_id)
+        for game_id in games_to_remove:
+            public_games.pop(game_id)
+
         if get_query("game_id"):
             if get_query("game_id") not in multiplayer_games:
                 popup("Error", put_error("Game not found"))
             else:
                 join_game(get_query("game_id"))
             return
 
         form_result = input_group('New Game', [
             radio('Mode', ['Singleplayer', 'Multiplayer (Private)', 'Multiplayer (Public)'], name='mode', value='Singleplayer'),
             checkbox('Options',
                      options=supported_options,
                      name='options'),
             actions('Public Games', [
                 {'label': f"Join game: {', '.join(public_game.options) or 'standard'}", 'value': game_id}
-                for game_id, public_game in public_games.items()
+                for game_id, (_, public_game) in public_games.items()
                 ], name='public_games'),
             actions('-', [
                 {'label': 'Create ', 'value': 'create'},
             ], name='action'),
         ])
 
         if form_result['public_games'] is not None:
```

### Comparing `chessmaker-0.2/chessmaker/events/event_publisher.py` & `chessmaker-0.3.0/chessmaker/events/event_publisher.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,72 +1,90 @@
 import bisect
-from collections import defaultdict
 from dataclasses import dataclass, field
-from typing import TypeVar, Callable, Generic, Type
+from typing import TypeVar, Callable, Type, cast
 
 from chessmaker.events.event import Event
 from chessmaker.events.event_priority import EventPriority
 
 
 @dataclass(frozen=True)
 class _Subscriber:
     callback: Callable[[Event], None]
     priority: int = field(default=EventPriority.NORMAL, compare=False, hash=False)
-TEvent = TypeVar('TEvent', bound=Event)
 
-class EventPublisher(Generic[TEvent]):
-    def __init__(self,
-                 subscribers: dict[Type[TEvent], list[_Subscriber]] = None,
-                subscribers_to_all: list[_Subscriber] = None
-         ):
-        if subscribers is None:
-            subscribers = defaultdict(list)
-        if subscribers_to_all is None:
-            subscribers_to_all = defaultdict(list)
-        self._subscribers: dict[Type[TEvent], list[_Subscriber]] = subscribers
-        self._subscribers_to_all: dict[_Subscriber, list[Type[TEvent]]] = subscribers_to_all
 
-    def subscribe(self, event_type: Type[TEvent], callback: Callable[[TEvent], None], priority: int = EventPriority.NORMAL):
-        bisect.insort(self._subscribers[event_type], _Subscriber(callback, priority), key=lambda subscriber: -subscriber.priority)
+TEvent = TypeVar("TEvent", bound=Event)
 
 
+class EventPublisher:
+    def __init__(self, event_types: tuple[Type[Event], ...] = None):
+        if event_types is not None:
+            self._subscribers: dict[Type[Event], list[_Subscriber]] = {}
+            self._propagating_to: dict[Type[Event], list[EventPublisher]] = {}
+            for event_type in event_types:
+                self._subscribers[event_type] = []
+                self._propagating_to[event_type] = []
+
+    def subscribe(self, event_type: Type[TEvent], callback: Callable[[TEvent], None],
+                  priority: int = EventPriority.NORMAL):
+        bisect.insort(self._subscribers[event_type], _Subscriber(callback, priority),
+                      key=lambda subscriber: -subscriber.priority)
+        for publisher in self._propagating_to[event_type]:
+            publisher.subscribe(event_type, callback, priority)
+
     def unsubscribe(self, event_type: Type[TEvent], callback: Callable[[TEvent], None]):
         while callback in self._subscribers[event_type]:
             self._subscribers[event_type].remove(_Subscriber(callback))
 
-    def subscribe_to_all(self, callback: Callable[[TEvent], None], priority: int = EventPriority.NORMAL):
-        for event_type in self._subscribers:
+    def subscribe_to_all(self, callback: Callable[[Event], None], priority: int = EventPriority.NORMAL):
+        for event_type in self._subscribers.keys():
             self.subscribe(event_type, callback, priority)
-        self._subscribers_to_all[_Subscriber(callback, priority)] = list(self._subscribers.keys())
 
-    def unsubscribe_from_all(self, callback: Callable[[TEvent], None]):
-        for event_type in self._subscribers:
+    def unsubscribe_from_all(self, callback: Callable[[Event], None]):
+        for event_type in self._subscribers.keys():
             self.unsubscribe(event_type, callback)
-        self._subscribers_to_all.pop(_Subscriber(callback))
 
-    def publish(self, event: TEvent):
-        event_type = type(event)
-        for subscriber, event_types in self._subscribers_to_all.items():
-            if event_type not in event_types:
-                self.subscribe(event_type, subscriber.callback, subscriber.priority)
-                self._subscribers_to_all[subscriber].append(event_type)
+    def publish(self, event: Event):
         for subscriber in self._subscribers[type(event)]:
             subscriber.callback(event)
 
-
-    def propagate(self, publisher: 'EventPublisher', event_type: Type[TEvent], priority: int = EventPriority.NORMAL):
+    def propagate(self, publisher: 'EventPublisher', event_type: Type[Event]):
         """
         For all events publisher publishes of type event_type, publish them to self
         """
-        def callback(event: TEvent):
-            self.publish(event)
-
-        publisher.subscribe(event_type, callback, priority)
+        self._propagating_to[event_type].append(publisher)
 
-    def propagate_all(self, publisher: 'EventPublisher', priority: int = EventPriority.NORMAL):
+    def propagate_all(self, publisher: 'EventPublisher'):
         """
         For all events publisher publishes, publish them to self
         """
-        def callback(event: TEvent):
-            self.publish(event)
+        for event_type in (set(publisher._subscribers.keys()) & set(self._propagating_to.keys())):
+            self.propagate(publisher, event_type)
+
+
+T = TypeVar('T')
+
+
+def event_publisher(*event_types: Type[Event]) -> Callable[[Type[T]], Type[T] | Type[EventPublisher]]:
+    def _class(cls: Type[T]) -> Type[T] | Type[EventPublisher]:
+        original_init = cls.__init__
+
+        def __init__(self, *args, **kwargs):
+            if hasattr(self, "_subscribers") and self._subscribers:
+                EventPublisher.__init__(self, tuple(self._subscribers.keys()) + event_types)
+            else:
+                EventPublisher.__init__(self, event_types)
+
+            original_init(self, *args, **kwargs)
+
+        cls.__init__ = __init__
+        cls.subscribe = EventPublisher.subscribe
+        cls.unsubscribe = EventPublisher.unsubscribe
+        cls.subscribe_to_all = EventPublisher.subscribe_to_all
+        cls.unsubscribe_from_all = EventPublisher.unsubscribe_from_all
+        cls.publish = EventPublisher.publish
+        cls.propagate = EventPublisher.propagate
+        cls.propagate_all = EventPublisher.propagate_all
+
+        return cast(Type[EventPublisher], cls)
 
-        publisher.subscribe_to_all(callback, priority)
+    return _class
```

### Comparing `chessmaker-0.2/LICENSE` & `chessmaker-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chessmaker-0.2/pyproject.toml` & `chessmaker-0.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chessmaker"
-version = "0.2"
+version = "0.3.0"
 description = "An easily extendible chess implementation designed to support any custom rule or feature"
 readme = "README.md"
 authors = ["WolfDWyc <yoavwolfdw@gmail.com>",]
 license = "AGPL-3.0-or-later"
 classifiers = [
 "License :: OSI Approved :: GNU Affero General Public License v3",
 "Programming Language :: Python",
```

### Comparing `chessmaker-0.2/README.md` & `chessmaker-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `chessmaker-0.2/PKG-INFO` & `chessmaker-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chessmaker
-Version: 0.2
+Version: 0.3.0
 Summary: An easily extendible chess implementation designed to support any custom rule or feature
 License: AGPL-3.0-or-later
 Keywords: chess
 Author: WolfDWyc
 Author-email: yoavwolfdw@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
```

