# Comparing `tmp/pokerkit-0.4.9.tar.gz` & `tmp/pokerkit-0.5.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokerkit-0.4.9.tar", last modified: Sun Jan 28 07:40:22 2024, max compression
+gzip compressed data, was "pokerkit-0.5.0a0.tar", last modified: Tue Apr 23 17:56:31 2024, max compression
```

## Comparing `pokerkit-0.4.9.tar` & `pokerkit-0.5.0a0.tar`

### file list

```diff
@@ -1,29 +1,34 @@
-drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2024-01-28 07:40:22.247020 pokerkit-0.4.9/
--rw-rw-r--   0 juho      (1000) juho      (1000)     1108 2024-01-19 00:50:06.000000 pokerkit-0.4.9/LICENSE
--rw-r--r--   0 juho      (1000) juho      (1000)    13777 2024-01-28 07:40:22.247020 pokerkit-0.4.9/PKG-INFO
--rw-rw-r--   0 juho      (1000) juho      (1000)    12141 2024-01-28 07:31:06.000000 pokerkit-0.4.9/README.rst
-drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2024-01-28 07:40:22.247020 pokerkit-0.4.9/pokerkit/
--rw-rw-r--   0 juho      (1000) juho      (1000)     4030 2024-01-20 20:38:54.000000 pokerkit-0.4.9/pokerkit/__init__.py
--rw-rw-r--   0 juho      (1000) juho      (1000)    55107 2024-01-20 21:50:46.000000 pokerkit-0.4.9/pokerkit/games.py
--rw-rw-r--   0 juho      (1000) juho      (1000)    19496 2024-01-19 00:50:06.000000 pokerkit-0.4.9/pokerkit/hands.py
--rw-rw-r--   0 juho      (1000) juho      (1000)    13677 2024-01-19 00:50:06.000000 pokerkit-0.4.9/pokerkit/lookups.py
--rw-rw-r--   0 juho      (1000) juho      (1000)    17624 2024-01-28 07:03:04.000000 pokerkit-0.4.9/pokerkit/notation.py
--rw-rw-r--   0 juho      (1000) juho      (1000)        0 2024-01-19 00:50:06.000000 pokerkit-0.4.9/pokerkit/py.typed
--rw-rw-r--   0 juho      (1000) juho      (1000)   146217 2024-01-20 20:53:53.000000 pokerkit-0.4.9/pokerkit/state.py
-drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2024-01-28 07:40:22.247020 pokerkit-0.4.9/pokerkit/tests/
--rw-rw-r--   0 juho      (1000) juho      (1000)       88 2024-01-19 00:50:06.000000 pokerkit-0.4.9/pokerkit/tests/__init__.py
--rw-rw-r--   0 juho      (1000) juho      (1000)     4368 2024-01-19 00:50:06.000000 pokerkit-0.4.9/pokerkit/tests/test_lookups.py
--rw-rw-r--   0 juho      (1000) juho      (1000)    30011 2024-01-22 17:43:18.000000 pokerkit-0.4.9/pokerkit/tests/test_papers.py
--rw-rw-r--   0 juho      (1000) juho      (1000)    26921 2024-01-20 21:00:02.000000 pokerkit-0.4.9/pokerkit/tests/test_state.py
--rw-rw-r--   0 juho      (1000) juho      (1000)     2062 2024-01-19 00:50:06.000000 pokerkit-0.4.9/pokerkit/tests/test_utilities.py
-drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2024-01-28 07:40:22.247020 pokerkit-0.4.9/pokerkit/tests/test_wsop/
--rw-rw-r--   0 juho      (1000) juho      (1000)      141 2024-01-19 00:50:06.000000 pokerkit-0.4.9/pokerkit/tests/test_wsop/__init__.py
--rw-rw-r--   0 juho      (1000) juho      (1000)   193280 2024-01-19 00:50:06.000000 pokerkit-0.4.9/pokerkit/tests/test_wsop/test_2023_43.py
--rw-rw-r--   0 juho      (1000) juho      (1000)    18245 2024-01-20 20:48:35.000000 pokerkit-0.4.9/pokerkit/utilities.py
-drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2024-01-28 07:40:22.247020 pokerkit-0.4.9/pokerkit.egg-info/
--rw-r--r--   0 juho      (1000) juho      (1000)    13777 2024-01-28 07:40:22.000000 pokerkit-0.4.9/pokerkit.egg-info/PKG-INFO
--rw-rw-r--   0 juho      (1000) juho      (1000)      539 2024-01-28 07:40:22.000000 pokerkit-0.4.9/pokerkit.egg-info/SOURCES.txt
--rw-rw-r--   0 juho      (1000) juho      (1000)        1 2024-01-28 07:40:22.000000 pokerkit-0.4.9/pokerkit.egg-info/dependency_links.txt
--rw-rw-r--   0 juho      (1000) juho      (1000)        9 2024-01-28 07:40:22.000000 pokerkit-0.4.9/pokerkit.egg-info/top_level.txt
--rw-rw-r--   0 juho      (1000) juho      (1000)       38 2024-01-28 07:40:22.247020 pokerkit-0.4.9/setup.cfg
--rw-rw-r--   0 juho      (1000) juho      (1000)     2105 2024-01-28 07:29:41.000000 pokerkit-0.4.9/setup.py
+drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2024-04-23 17:56:31.690392 pokerkit-0.5.0a0/
+-rw-rw-r--   0 juho      (1000) juho      (1000)     1116 2024-04-11 09:02:36.000000 pokerkit-0.5.0a0/LICENSE
+-rw-r--r--   0 juho      (1000) juho      (1000)    17204 2024-04-23 17:56:31.690392 pokerkit-0.5.0a0/PKG-INFO
+-rw-rw-r--   0 juho      (1000) juho      (1000)    15530 2024-04-23 17:49:32.000000 pokerkit-0.5.0a0/README.rst
+drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2024-04-23 17:56:31.686392 pokerkit-0.5.0a0/pokerkit/
+-rw-rw-r--   0 juho      (1000) juho      (1000)     4460 2024-04-20 15:21:12.000000 pokerkit-0.5.0a0/pokerkit/__init__.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)    15073 2024-04-09 08:26:29.000000 pokerkit-0.5.0a0/pokerkit/analysis.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)    74102 2024-04-23 17:26:14.000000 pokerkit-0.5.0a0/pokerkit/games.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)    21443 2024-04-09 09:11:40.000000 pokerkit-0.5.0a0/pokerkit/hands.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)    15305 2024-04-09 09:11:43.000000 pokerkit-0.5.0a0/pokerkit/lookups.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)    28717 2024-04-09 08:58:34.000000 pokerkit-0.5.0a0/pokerkit/notation.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)        0 2024-03-03 02:45:25.000000 pokerkit-0.5.0a0/pokerkit/py.typed
+-rw-rw-r--   0 juho      (1000) juho      (1000)   194299 2024-04-23 17:00:45.000000 pokerkit-0.5.0a0/pokerkit/state.py
+drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2024-04-23 17:56:31.690392 pokerkit-0.5.0a0/pokerkit/tests/
+-rw-rw-r--   0 juho      (1000) juho      (1000)       88 2024-03-03 02:45:25.000000 pokerkit-0.5.0a0/pokerkit/tests/__init__.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)    17128 2024-03-25 16:57:08.000000 pokerkit-0.5.0a0/pokerkit/tests/test_analysis.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)     6485 2024-04-23 17:51:34.000000 pokerkit-0.5.0a0/pokerkit/tests/test_games.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)     5331 2024-03-15 11:23:34.000000 pokerkit-0.5.0a0/pokerkit/tests/test_lookups.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)    28167 2024-03-29 06:34:10.000000 pokerkit-0.5.0a0/pokerkit/tests/test_notation.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)    35725 2024-04-23 17:51:05.000000 pokerkit-0.5.0a0/pokerkit/tests/test_papers.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)    37676 2024-04-23 14:37:55.000000 pokerkit-0.5.0a0/pokerkit/tests/test_state.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)     2062 2024-04-23 17:51:13.000000 pokerkit-0.5.0a0/pokerkit/tests/test_utilities.py
+drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2024-04-23 17:56:31.690392 pokerkit-0.5.0a0/pokerkit/tests/test_wsop/
+-rw-rw-r--   0 juho      (1000) juho      (1000)      141 2024-03-03 02:45:25.000000 pokerkit-0.5.0a0/pokerkit/tests/test_wsop/__init__.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)   193298 2024-04-16 23:01:37.000000 pokerkit-0.5.0a0/pokerkit/tests/test_wsop/test_2023_43_5.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)    32968 2024-04-23 17:38:59.000000 pokerkit-0.5.0a0/pokerkit/tests/test_wsop/test_2023_54_4.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)    18574 2024-04-10 07:51:29.000000 pokerkit-0.5.0a0/pokerkit/utilities.py
+drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2024-04-23 17:56:31.690392 pokerkit-0.5.0a0/pokerkit.egg-info/
+-rw-r--r--   0 juho      (1000) juho      (1000)    17204 2024-04-23 17:56:31.000000 pokerkit-0.5.0a0/pokerkit.egg-info/PKG-INFO
+-rw-rw-r--   0 juho      (1000) juho      (1000)      698 2024-04-23 17:56:31.000000 pokerkit-0.5.0a0/pokerkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 juho      (1000) juho      (1000)        1 2024-04-23 17:56:31.000000 pokerkit-0.5.0a0/pokerkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 juho      (1000) juho      (1000)        9 2024-04-23 17:56:31.000000 pokerkit-0.5.0a0/pokerkit.egg-info/top_level.txt
+-rw-rw-r--   0 juho      (1000) juho      (1000)       38 2024-04-23 17:56:31.690392 pokerkit-0.5.0a0/setup.cfg
+-rw-rw-r--   0 juho      (1000) juho      (1000)     2143 2024-04-23 17:55:18.000000 pokerkit-0.5.0a0/setup.py
```

### Comparing `pokerkit-0.4.9/LICENSE` & `pokerkit-0.5.0a0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 University of Toronto Computer Poker Research Group
+Copyright (c) 2023 University of Toronto Computer Poker Student Research Group
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pokerkit-0.4.9/PKG-INFO` & `pokerkit-0.5.0a0/README.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,71 +1,156 @@
-Metadata-Version: 2.1
-Name: pokerkit
-Version: 0.4.9
-Summary: An open-source Python library for poker simulations and hand evaluations
-Home-page: https://github.com/uoftcprg/pokerkit
-Author: University of Toronto Computer Poker Research Group
-Author-email: uoftcprg@studentorg.utoronto.ca
-License: MIT
-Project-URL: Documentation, https://pokerkit.readthedocs.io/en/latest/
-Project-URL: Source, https://github.com/uoftcprg/pokerkit
-Project-URL: Tracker, https://github.com/uoftcprg/pokerkit/issues
-Keywords: artificial-intelligence,deep-learning,game,game-development,game-theory,holdem-poker,imperfect-information-game,libratus,pluribus,poker,poker-engine,poker-evaluator,poker-game,poker-hands,poker-library,poker-strategies,python,reinforcement-learning,texas-holdem
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Topic :: Education
-Classifier: Topic :: Games/Entertainment
-Classifier: Topic :: Games/Entertainment :: Board Games
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3.13
-Requires-Python: >=3.11
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
 ========
 PokerKit
 ========
 
-PokerKit is an open-source Python library for simulating poker games and evaluating poker hands, developed by the University of Toronto Computer Poker Research Group. PokerKit supports an extensive array of poker variants and it provides a flexible architecture for users to define their custom games. These facilities are exposed via an intuitive unified high-level programmatic API. The library can be used in a variety of use cases, from poker AI development, and tool creation, to online poker casino implementation. PokerKit's reliability has been established through static type checking, extensive doctests, and unit tests, achieving 99% code coverage.
+PokerKit is an open-source software library, written in pure Python, for simulating games, evaluating hands, and facilitating statistical analysis, developed by the University of Toronto Computer Poker Student Research Group. PokerKit supports an extensive array of poker variants and it provides a flexible architecture for users to define their custom games. These facilities are exposed via an intuitive unified high-level programmatic API. The library can be used in a variety of use cases, from poker AI development, and tool creation, to online poker casino implementation. PokerKit's reliability has been established through static type checking, extensive doctests, and unit tests, achieving 99% code coverage.
 
 Features
 --------
 
 * Extensive poker game logic for major and minor poker variants.
 * High-speed hand evaluations.
 * Customizable game states and parameters.
 * Robust implementation with static type checking and extensive unit tests and doctests.
-* Dataset of over 10,000 hand histories.
 
 Installation
 ------------
 
 The PokerKit library can be installed using pip:
 
 .. code-block:: bash
 
    pip install pokerkit
 
 Usages
 ------
 
-**The first televised million-dollar pot between Tom Dwan and Phil Ivey.**
+Example usages of PokerKit is shown below.
 
-Link: https://youtu.be/GnxFohpljqM
+Multi-Runout in an All-In Situation
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+Below shows the 4-runout hand between Phil Hellmuth and the Loose Cannon Ernest Wiggins.
+
+Link: https://youtu.be/cnjJv7x0HMY?si=4l05Ez7lQVczt8DI&t=638
+
+.. code-block:: python
+
+   from pokerkit import Automation, Mode, NoLimitTexasHoldem
+
+   state = NoLimitTexasHoldem.create_state(
+       # Automations
+       (
+           Automation.ANTE_POSTING,
+           Automation.BET_COLLECTION,
+           Automation.BLIND_OR_STRADDLE_POSTING,
+           Automation.HOLE_CARDS_SHOWING_OR_MUCKING,
+           Automation.HAND_KILLING,
+           Automation.CHIPS_PUSHING,
+           Automation.CHIPS_PULLING,
+       ),
+       False,  # Uniform antes?
+       {-1: 600},  # Antes
+       (200, 400, 800),  # Blinds or straddles
+       400,  # Min-bet
+       (999999, 116400, 86900, 999999, 50000, 999999),  # Starting stacks
+       6,  # Number of players
+       mode=Mode.CASH_GAME,
+   )
+
+Below are the pre-flop dealings and actions.
+
+.. code-block:: python
+
+   state.deal_hole('JsTh')  # Tony G
+   state.deal_hole('Ah9d')  # Hellmuth
+   state.deal_hole('KsKc')  # Wiggins
+   state.deal_hole('5c2h')  # Negreanu
+   state.deal_hole('6h5h')  # Brunson
+   state.deal_hole('6s3s')  # Laak
+
+   state.fold()  # Negreanu
+   state.complete_bet_or_raise_to(2800)  # Brunson
+   state.fold()  # Laak
+   state.check_or_call()  # Tony G
+   state.complete_bet_or_raise_to(12600)  # Hellmuth
+   state.check_or_call()  # Wiggins
+   state.check_or_call()  # Brunson
+   state.check_or_call()  # Tony G
+
+Below are the flop dealing and actions.
+
+.. code-block:: python
+
+   state.burn_card('??')
+   state.deal_board('9hTs9s')
+
+   state.check_or_call()  # Tony G
+   state.complete_bet_or_raise_to(17000)  # Hellmuth
+   state.complete_bet_or_raise_to(36000)  # Wiggins
+   state.fold()  # Brunson
+   state.fold()  # Tony G
+   state.complete_bet_or_raise_to(103800)  # Hellmuth
+   state.check_or_call()  # Wiggins
+
+Below is selecting the number of runouts.
+
+.. code-block:: python
+
+   state.select_runout_count(4)  # Hellmuth
+   state.select_runout_count(None)  # Wiggins
 
-Set up the game.
+Below is the first runout.
+
+.. code-block:: python
+
+   state.burn_card('??')
+   state.deal_board('Jh')  # Turn
+   state.burn_card('??')
+   state.deal_board('Ad')  # River
+
+Below is the second runout.
+
+.. code-block:: python
+
+   state.burn_card('??')
+   state.deal_board('Kh')  # Turn
+   state.burn_card('??')
+   state.deal_board('3c')  # River
+
+Below is the third runout.
+
+.. code-block:: python
+
+   state.burn_card('??')
+   state.deal_board('7s')  # Turn
+   state.burn_card('??')
+   state.deal_board('8s')  # River
+
+Below is the fourth runout.
+
+.. code-block:: python
+
+   state.burn_card('??')
+   state.deal_board('Qc')  # Turn
+   state.burn_card('??')
+   state.deal_board('Kd')  # River
+
+Below are the final stacks.
+
+.. code-block:: python
+
+   print(state.stacks)  # [987399, 79400, 149700, 999999, 37400, 999399]
+
+A Sample No-Limit Texas Hold'em Hand
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+Below shows the first televised million-dollar pot between Tom Dwan and Phil Ivey.
+
+Link: https://youtu.be/GnxFohpljqM
 
 .. code-block:: python
 
    from pokerkit import Automation, NoLimitTexasHoldem
 
    state = NoLimitTexasHoldem.create_state(
        # Automations
@@ -130,15 +215,18 @@
 
 Below are the final stacks.
 
 .. code-block:: python
 
    print(state.stacks)  # [572100, 1997500, 1109500]
 
-**An all-in hand between Xuan and Phua.**
+A Sample Short-Deck Hold'em Hand
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+Below shows an all-in hand between Xuan and Phua.
 
 Link: https://youtu.be/QlgCcphLjaQ
 
 .. code-block:: python
 
    from pokerkit import Automation, NoLimitShortDeckHoldem
 
@@ -205,16 +293,18 @@
 
 Below are the final stacks.
 
 .. code-block:: python
 
    print(state.stacks)  # [489000, 226000, 684000, 400000, 0, 198000]
 
-**The largest online poker pot ever played between Patrik Antonius and Viktor
-Blom.**
+A Sample Pot-Limit Omaha Hold'em Hand
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+Below shows the largest online poker pot ever played between Patrik Antonius and Viktor Blom.
 
 Link: https://youtu.be/UMBm66Id2AA
 
 .. code-block:: python
 
    from pokerkit import Automation, PotLimitOmahaHoldem
 
@@ -278,15 +368,18 @@
 
 Below are the final stacks.
 
 .. code-block:: python
 
    print(state.stacks)  # [1937923.75, 0.0]
 
-**A bad beat between Yockey and Arieh.**
+A Sample Fixed-Limit Deuce-To-Seven Lowball Triple Draw Hand
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+Below shows a bad beat between Yockey and Arieh.
 
 Link: https://youtu.be/pChCqb2FNxY
 
 .. code-block:: python
 
    from pokerkit import Automation, FixedLimitDeuceToSevenLowballTripleDraw
 
@@ -363,15 +456,18 @@
 
 Below are the final stacks.
 
 .. code-block:: python
 
    print(state.stacks)  # [0, 4190000, 5910000, 12095000]
 
-**An example badugi hand from Wikipedia.**
+A Sample Badugi Hand
+^^^^^^^^^^^^^^^^^^^^
+
+Below shows an example badugi hand from Wikipedia.
 
 Link: https://en.wikipedia.org/wiki/Badugi
 
 .. code-block:: python
 
    from pokerkit import Automation, FixedLimitBadugi
 
@@ -467,15 +563,15 @@
 .. code-block:: python
 
    print(state.stacks)  # [196, 220, 200, 184]
 
 Testing and Validation
 ----------------------
 
-PokerKit has extensive test coverage, passes mypy static type checking with strict parameter, and has been validated through extensive use in real-life scenarios.
+PokerKit has extensive test coverage, passes mypy static type checking with strict mode, and has been validated through extensive use in real-life scenarios.
 
 Contributing
 ------------
 
 Contributions are welcome! Please read our Contributing Guide for more information.
 
 License
```

### Comparing `pokerkit-0.4.9/README.rst` & `pokerkit-0.5.0a0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,188 @@
+Metadata-Version: 2.1
+Name: pokerkit
+Version: 0.5.0a0
+Summary: An open-source Python library for poker game simulations, hand evaluations, and statistical analysis
+Home-page: https://github.com/uoftcprg/pokerkit
+Author: University of Toronto Computer Poker Student Research Group
+Author-email: uoftcprg@studentorg.utoronto.ca
+License: MIT
+Project-URL: Documentation, https://pokerkit.readthedocs.io/en/latest/
+Project-URL: Source, https://github.com/uoftcprg/pokerkit
+Project-URL: Tracker, https://github.com/uoftcprg/pokerkit/issues
+Keywords: artificial-intelligence,deep-learning,game,game-development,game-theory,holdem-poker,imperfect-information-game,libratus,pluribus,poker,poker-engine,poker-evaluator,poker-game,poker-hands,poker-library,poker-strategies,python,reinforcement-learning,texas-holdem
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Topic :: Education
+Classifier: Topic :: Games/Entertainment
+Classifier: Topic :: Games/Entertainment :: Board Games
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
+Requires-Python: >=3.11
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
 ========
 PokerKit
 ========
 
-PokerKit is an open-source Python library for simulating poker games and evaluating poker hands, developed by the University of Toronto Computer Poker Research Group. PokerKit supports an extensive array of poker variants and it provides a flexible architecture for users to define their custom games. These facilities are exposed via an intuitive unified high-level programmatic API. The library can be used in a variety of use cases, from poker AI development, and tool creation, to online poker casino implementation. PokerKit's reliability has been established through static type checking, extensive doctests, and unit tests, achieving 99% code coverage.
+PokerKit is an open-source software library, written in pure Python, for simulating games, evaluating hands, and facilitating statistical analysis, developed by the University of Toronto Computer Poker Student Research Group. PokerKit supports an extensive array of poker variants and it provides a flexible architecture for users to define their custom games. These facilities are exposed via an intuitive unified high-level programmatic API. The library can be used in a variety of use cases, from poker AI development, and tool creation, to online poker casino implementation. PokerKit's reliability has been established through static type checking, extensive doctests, and unit tests, achieving 99% code coverage.
 
 Features
 --------
 
 * Extensive poker game logic for major and minor poker variants.
 * High-speed hand evaluations.
 * Customizable game states and parameters.
 * Robust implementation with static type checking and extensive unit tests and doctests.
-* Dataset of over 10,000 hand histories.
 
 Installation
 ------------
 
 The PokerKit library can be installed using pip:
 
 .. code-block:: bash
 
    pip install pokerkit
 
 Usages
 ------
 
-**The first televised million-dollar pot between Tom Dwan and Phil Ivey.**
+Example usages of PokerKit is shown below.
 
-Link: https://youtu.be/GnxFohpljqM
+Multi-Runout in an All-In Situation
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+Below shows the 4-runout hand between Phil Hellmuth and the Loose Cannon Ernest Wiggins.
+
+Link: https://youtu.be/cnjJv7x0HMY?si=4l05Ez7lQVczt8DI&t=638
+
+.. code-block:: python
+
+   from pokerkit import Automation, Mode, NoLimitTexasHoldem
+
+   state = NoLimitTexasHoldem.create_state(
+       # Automations
+       (
+           Automation.ANTE_POSTING,
+           Automation.BET_COLLECTION,
+           Automation.BLIND_OR_STRADDLE_POSTING,
+           Automation.HOLE_CARDS_SHOWING_OR_MUCKING,
+           Automation.HAND_KILLING,
+           Automation.CHIPS_PUSHING,
+           Automation.CHIPS_PULLING,
+       ),
+       False,  # Uniform antes?
+       {-1: 600},  # Antes
+       (200, 400, 800),  # Blinds or straddles
+       400,  # Min-bet
+       (999999, 116400, 86900, 999999, 50000, 999999),  # Starting stacks
+       6,  # Number of players
+       mode=Mode.CASH_GAME,
+   )
+
+Below are the pre-flop dealings and actions.
+
+.. code-block:: python
+
+   state.deal_hole('JsTh')  # Tony G
+   state.deal_hole('Ah9d')  # Hellmuth
+   state.deal_hole('KsKc')  # Wiggins
+   state.deal_hole('5c2h')  # Negreanu
+   state.deal_hole('6h5h')  # Brunson
+   state.deal_hole('6s3s')  # Laak
+
+   state.fold()  # Negreanu
+   state.complete_bet_or_raise_to(2800)  # Brunson
+   state.fold()  # Laak
+   state.check_or_call()  # Tony G
+   state.complete_bet_or_raise_to(12600)  # Hellmuth
+   state.check_or_call()  # Wiggins
+   state.check_or_call()  # Brunson
+   state.check_or_call()  # Tony G
+
+Below are the flop dealing and actions.
+
+.. code-block:: python
+
+   state.burn_card('??')
+   state.deal_board('9hTs9s')
+
+   state.check_or_call()  # Tony G
+   state.complete_bet_or_raise_to(17000)  # Hellmuth
+   state.complete_bet_or_raise_to(36000)  # Wiggins
+   state.fold()  # Brunson
+   state.fold()  # Tony G
+   state.complete_bet_or_raise_to(103800)  # Hellmuth
+   state.check_or_call()  # Wiggins
+
+Below is selecting the number of runouts.
+
+.. code-block:: python
+
+   state.select_runout_count(4)  # Hellmuth
+   state.select_runout_count(None)  # Wiggins
 
-Set up the game.
+Below is the first runout.
+
+.. code-block:: python
+
+   state.burn_card('??')
+   state.deal_board('Jh')  # Turn
+   state.burn_card('??')
+   state.deal_board('Ad')  # River
+
+Below is the second runout.
+
+.. code-block:: python
+
+   state.burn_card('??')
+   state.deal_board('Kh')  # Turn
+   state.burn_card('??')
+   state.deal_board('3c')  # River
+
+Below is the third runout.
+
+.. code-block:: python
+
+   state.burn_card('??')
+   state.deal_board('7s')  # Turn
+   state.burn_card('??')
+   state.deal_board('8s')  # River
+
+Below is the fourth runout.
+
+.. code-block:: python
+
+   state.burn_card('??')
+   state.deal_board('Qc')  # Turn
+   state.burn_card('??')
+   state.deal_board('Kd')  # River
+
+Below are the final stacks.
+
+.. code-block:: python
+
+   print(state.stacks)  # [987399, 79400, 149700, 999999, 37400, 999399]
+
+A Sample No-Limit Texas Hold'em Hand
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+Below shows the first televised million-dollar pot between Tom Dwan and Phil Ivey.
+
+Link: https://youtu.be/GnxFohpljqM
 
 .. code-block:: python
 
    from pokerkit import Automation, NoLimitTexasHoldem
 
    state = NoLimitTexasHoldem.create_state(
        # Automations
@@ -98,15 +247,18 @@
 
 Below are the final stacks.
 
 .. code-block:: python
 
    print(state.stacks)  # [572100, 1997500, 1109500]
 
-**An all-in hand between Xuan and Phua.**
+A Sample Short-Deck Hold'em Hand
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+Below shows an all-in hand between Xuan and Phua.
 
 Link: https://youtu.be/QlgCcphLjaQ
 
 .. code-block:: python
 
    from pokerkit import Automation, NoLimitShortDeckHoldem
 
@@ -173,16 +325,18 @@
 
 Below are the final stacks.
 
 .. code-block:: python
 
    print(state.stacks)  # [489000, 226000, 684000, 400000, 0, 198000]
 
-**The largest online poker pot ever played between Patrik Antonius and Viktor
-Blom.**
+A Sample Pot-Limit Omaha Hold'em Hand
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+Below shows the largest online poker pot ever played between Patrik Antonius and Viktor Blom.
 
 Link: https://youtu.be/UMBm66Id2AA
 
 .. code-block:: python
 
    from pokerkit import Automation, PotLimitOmahaHoldem
 
@@ -246,15 +400,18 @@
 
 Below are the final stacks.
 
 .. code-block:: python
 
    print(state.stacks)  # [1937923.75, 0.0]
 
-**A bad beat between Yockey and Arieh.**
+A Sample Fixed-Limit Deuce-To-Seven Lowball Triple Draw Hand
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+Below shows a bad beat between Yockey and Arieh.
 
 Link: https://youtu.be/pChCqb2FNxY
 
 .. code-block:: python
 
    from pokerkit import Automation, FixedLimitDeuceToSevenLowballTripleDraw
 
@@ -331,15 +488,18 @@
 
 Below are the final stacks.
 
 .. code-block:: python
 
    print(state.stacks)  # [0, 4190000, 5910000, 12095000]
 
-**An example badugi hand from Wikipedia.**
+A Sample Badugi Hand
+^^^^^^^^^^^^^^^^^^^^
+
+Below shows an example badugi hand from Wikipedia.
 
 Link: https://en.wikipedia.org/wiki/Badugi
 
 .. code-block:: python
 
    from pokerkit import Automation, FixedLimitBadugi
 
@@ -435,15 +595,15 @@
 .. code-block:: python
 
    print(state.stacks)  # [196, 220, 200, 184]
 
 Testing and Validation
 ----------------------
 
-PokerKit has extensive test coverage, passes mypy static type checking with strict parameter, and has been validated through extensive use in real-life scenarios.
+PokerKit has extensive test coverage, passes mypy static type checking with strict mode, and has been validated through extensive use in real-life scenarios.
 
 Contributing
 ------------
 
 Contributions are welcome! Please read our Contributing Guide for more information.
 
 License
```

### Comparing `pokerkit-0.4.9/pokerkit/__init__.py` & `pokerkit-0.5.0a0/pokerkit/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,16 @@
     'BadugiLookup',
     'BetCollection',
     'BettingStructure',
     'BlindOrStraddlePosting',
     'BoardCombinationHand',
     'BoardDealing',
     'BringInPosting',
+    'calculate_equities',
+    'calculate_hand_strength',
     'Card',
     'CardBurning',
     'CardsLike',
     'CheckingOrCalling',
     'ChipsPulling',
     'ChipsPushing',
     'clean_values',
@@ -50,53 +52,66 @@
     'HoleDealing',
     'KuhnPokerHand',
     'KuhnPokerLookup',
     'Label',
     'Lookup',
     'max_or_none',
     'min_or_none',
+    'Mode',
     'NoLimitDeuceToSevenLowballSingleDraw',
     'NoLimitPokerMixin',
     'NoLimitShortDeckHoldem',
     'NoLimitTexasHoldem',
+    'NoOperation',
     'OmahaEightOrBetterLowHand',
     'OmahaHoldemHand',
     'OmahaHoldemMixin',
     'Opening',
     'Operation',
     'parse_action',
+    'parse_range',
     'parse_value',
     'Poker',
     'Pot',
     'PotLimitOmahaHoldem',
     'PotLimitPokerMixin',
     'rake',
     'Rank',
     'RankOrder',
     'RegularLookup',
     'RegularLowHand',
+    'RunoutCountSelection',
     'SevenCardStud',
     'ShortDeckHoldemHand',
     'ShortDeckHoldemLookup',
     'shuffled',
     'SingleDraw',
+    'StandardBadugiHand',
+    'StandardBadugiLookup',
     'StandardHand',
     'StandardHighHand',
     'StandardLookup',
     'StandardLowHand',
     'StandingPatOrDiscarding',
     'State',
+    'Statistics',
     'Street',
     'Suit',
     'TexasHoldemMixin',
     'TripleDraw',
     'UnfixedLimitHoldem',
     'ValuesLike',
 )
 
+from pokerkit.analysis import (
+    calculate_equities,
+    calculate_hand_strength,
+    parse_range,
+    Statistics,
+)
 from pokerkit.games import (
     DeuceToSevenLowballMixin,
     Draw,
     FixedLimitBadugi,
     FixedLimitDeuceToSevenLowballTripleDraw,
     FixedLimitOmahaHoldemHighLowSplitEightOrBetter,
     FixedLimitPokerMixin,
@@ -128,27 +143,29 @@
     Hand,
     HoleBoardCombinationHand,
     KuhnPokerHand,
     OmahaEightOrBetterLowHand,
     OmahaHoldemHand,
     RegularLowHand,
     ShortDeckHoldemHand,
+    StandardBadugiHand,
     StandardHand,
     StandardHighHand,
     StandardLowHand,
 )
 from pokerkit.lookups import (
     BadugiLookup,
     EightOrBetterLookup,
     Entry,
     KuhnPokerLookup,
     Label,
     Lookup,
     RegularLookup,
     ShortDeckHoldemLookup,
+    StandardBadugiLookup,
     StandardLookup,
 )
 from pokerkit.notation import HandHistory, parse_action
 from pokerkit.state import (
     AntePosting,
     Automation,
     BetCollection,
@@ -161,17 +178,20 @@
     ChipsPulling,
     ChipsPushing,
     CompletionBettingOrRaisingTo,
     Folding,
     HandKilling,
     HoleCardsShowingOrMucking,
     HoleDealing,
+    Mode,
+    NoOperation,
     Opening,
     Operation,
     Pot,
+    RunoutCountSelection,
     StandingPatOrDiscarding,
     State,
     Street,
 )
 from pokerkit.utilities import (
     Card,
     CardsLike,
```

### Comparing `pokerkit-0.4.9/pokerkit/lookups.py` & `pokerkit-0.5.0a0/pokerkit/lookups.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """:mod:`pokerkit.lookups` implements classes related to poker hand
 lookups.
 """
 
-from abc import ABC
+from abc import ABC, abstractmethod
 from collections.abc import Iterable, Reversible, Sequence
 from collections import Counter
-from dataclasses import dataclass, field
+from dataclasses import dataclass, field, replace
 from enum import StrEnum, unique
 from functools import partial
 from itertools import combinations, filterfalse
 from math import prod
 from operator import contains
 from typing import ClassVar
 
@@ -48,16 +48,17 @@
 
 @dataclass(order=True, frozen=True)
 class Entry:
     """The class for hand lookup entries.
 
     The :attr:`index` represents the strength of the corresponding
     hand. In this library, a stronger hand is considered greater. In
-    other words, stronger hands have a greater index with which
-    different entries and hands are compared.
+    other words, stronger hands have either a greater or less (depending
+    on whether using a high/low hand) index with which different entries
+    and hands are compared.
 
     The attributes are read-only.
 
     Note that the entries in the example below are meaningless. They
     are only meant to show how entries are used by other poker
     utilities.
 
@@ -142,14 +143,37 @@
             ):
                 hashes.append(hash_ * partial_hash)
 
         counter[multiplicity] = count
 
         return hashes
 
+    def __post_init__(self) -> None:
+        self._add_entries()
+        self.__reset_ranks()
+
+    @abstractmethod
+    def _add_entries(self) -> None:
+        pass  # pragma: no cover
+
+    def __reset_ranks(self) -> None:
+        indices = set()
+
+        for entry in self.__entries.values():
+            indices.add(entry.index)
+
+        sorted_indices = sorted(indices)
+        reset_indices = dict(zip(sorted_indices, range(len(indices))))
+
+        for key, value in self.__entries.items():
+            self.__entries[key] = replace(
+                value,
+                index=reset_indices[value.index],
+            )
+
     def has_entry(self, cards: CardsLike) -> bool:
         """Return whether the cards can be looked up.
 
         The cards can be looked up if the lookup contains an entry with
         the given cards.
 
         >>> lookup = ShortDeckHoldemLookup()
@@ -158,60 +182,65 @@
         >>> lookup.has_entry('Ah6h7s8c2s')
         False
 
         :param cards: The cards to look up.
         :return: ``True`` if the cards can looked up, otherwise
                  ``False``.
         """
-        return self.__get_key(cards) in self.__entries
+        try:
+            key = self._get_key(cards)
+        except ValueError:
+            key = None
+
+        return key in self.__entries
 
     def get_entry(self, cards: CardsLike) -> Entry:
         """Return the corresponding lookup entry of the hand that the
         cards form.
 
         >>> lookup = ShortDeckHoldemLookup()
         >>> entry = lookup.get_entry('Ah6h7s8c9s')
         >>> entry.index
-        1134
+        1128
         >>> entry.label
         <Label.STRAIGHT: 'Straight'>
         >>> entry = lookup.get_entry('Ah6h7s8c2s')
         Traceback (most recent call last):
             ...
-        ValueError: cards form an invalid hand
+        ValueError: The cards 'Ah6h7s8c2s' form an invalid hand.
 
         :param cards: The cards to look up.
         :return: The corresponding lookup entry.
         :raises ValueError: If cards do not form a valid hand.
         """
-        key = self.__get_key(cards)
+        key = self._get_key(cards)
 
         if key not in self.__entries:
-            raise ValueError('cards form an invalid hand')
+            raise ValueError(f'The cards {repr(cards)} form an invalid hand.')
 
         return self.__entries[key]
 
     def get_entry_or_none(self, cards: CardsLike) -> Entry | None:
         """Return the corresponding lookup entry of the hand that the
         cards form if it exists. Otherwise, return ``None``.
 
         >>> lookup = ShortDeckHoldemLookup()
         >>> lookup.get_entry('Ah6h7s8c2s')
         Traceback (most recent call last):
             ...
-        ValueError: cards form an invalid hand
+        ValueError: The cards 'Ah6h7s8c2s' form an invalid hand.
         >>> lookup.get_entry_or_none('Ah6h7s8c2s') is None
         True
 
         :param cards: The cards to look up.
         :return: The optional corresponding lookup entry.
         """
-        return self.__entries.get(self.__get_key(cards))
+        return self.__entries.get(self._get_key(cards))
 
-    def __get_key(self, cards: CardsLike) -> tuple[int, bool]:
+    def _get_key(self, cards: CardsLike) -> tuple[int, bool]:
         cards = Card.clean(cards)
         hash_ = self.__hash(Card.get_ranks(cards))
         suitedness = Card.are_suited(cards)
 
         return hash_, suitedness
 
     def _add_multisets(
@@ -219,36 +248,36 @@
             counter: Counter[int],
             suitednesses: tuple[bool, ...],
             label: Label,
     ) -> None:
         hashes = self.__hash_multisets(self.rank_order, counter)
 
         for hash_ in reversed(hashes):
-            self.__add(hash_, suitednesses, label)
+            self.__add_entry(hash_, suitednesses, label)
 
     def _add_straights(
             self,
             count: int,
             suitednesses: tuple[bool, ...],
             label: Label,
     ) -> None:
-        self.__add(
+        self.__add_entry(
             self.__hash(self.rank_order[-1:] + self.rank_order[: count - 1]),
             suitednesses,
             label,
         )
 
         for i in range(len(self.rank_order) - count + 1):
-            self.__add(
+            self.__add_entry(
                 self.__hash(self.rank_order[i:i + count]),
                 suitednesses,
                 label,
             )
 
-    def __add(
+    def __add_entry(
             self,
             hash_: int,
             suitednesses: Iterable[bool],
             label: Label,
     ) -> None:
         entry = Entry(self.__entry_count, label)
         self.__entry_count += 1
@@ -267,26 +296,26 @@
 
     >>> lookup = StandardLookup()
     >>> e0 = lookup.get_entry('Ah6h7s8c9s')
     >>> e1 = lookup.get_entry('AhAc6s6hTd')
     >>> e2 = lookup.get_entry('AcAdAhAsAc')
     Traceback (most recent call last):
         ...
-    ValueError: cards form an invalid hand
+    ValueError: The cards 'AcAdAhAsAc' form an invalid hand.
     >>> e0 < e1
     True
     >>> e0.label
     <Label.HIGH_CARD: 'High card'>
     >>> e1.label
     <Label.TWO_PAIR: 'Two pair'>
     """
 
     rank_order = RankOrder.STANDARD
 
-    def __post_init__(self) -> None:
+    def _add_entries(self) -> None:
         self._add_multisets(Counter({1: 5}), (False,), Label.HIGH_CARD)
         self._add_multisets(Counter({2: 1, 1: 3}), (False,), Label.ONE_PAIR)
         self._add_multisets(Counter({2: 2, 1: 1}), (False,), Label.TWO_PAIR)
         self._add_multisets(
             Counter({3: 1, 1: 2}),
             (False,),
             Label.THREE_OF_A_KIND,
@@ -313,26 +342,26 @@
 
     >>> lookup = ShortDeckHoldemLookup()
     >>> e0 = lookup.get_entry('AhAc6s6hTd')
     >>> e1 = lookup.get_entry('Ah6h7s8c9s')
     >>> e2 = lookup.get_entry('Ah2h3s4c5s')
     Traceback (most recent call last):
         ...
-    ValueError: cards form an invalid hand
+    ValueError: The cards 'Ah2h3s4c5s' form an invalid hand.
     >>> e0 < e1
     True
     >>> e0.label
     <Label.TWO_PAIR: 'Two pair'>
     >>> e1.label
     <Label.STRAIGHT: 'Straight'>
     """
 
     rank_order = RankOrder.SHORT_DECK_HOLDEM
 
-    def __post_init__(self) -> None:
+    def _add_entries(self) -> None:
         self._add_multisets(Counter({1: 5}), (False,), Label.HIGH_CARD)
         self._add_multisets(Counter({2: 1, 1: 3}), (False,), Label.ONE_PAIR)
         self._add_multisets(Counter({2: 2, 1: 1}), (False,), Label.TWO_PAIR)
         self._add_multisets(
             Counter({3: 1, 1: 2}),
             (False,),
             Label.THREE_OF_A_KIND,
@@ -354,15 +383,15 @@
 
     Lookups are used by evaluators. If you want to evaluate poker hands,
     please use :class:`pokerkit.hands.EightOrBetterLowHand`.
     """
 
     rank_order = RankOrder.EIGHT_OR_BETTER_LOW
 
-    def __post_init__(self) -> None:
+    def _add_entries(self) -> None:
         self._add_multisets(Counter({1: 5}), (False, True), Label.HIGH_CARD)
 
 
 @dataclass
 class RegularLookup(Lookup):
     """The class for regular hand lookups.
 
@@ -373,26 +402,26 @@
 
     >>> lookup = RegularLookup()
     >>> e0 = lookup.get_entry('Ah6h7s8c9s')
     >>> e1 = lookup.get_entry('AhAc6s6hTd')
     >>> e2 = lookup.get_entry('3s4sQhTc')
     Traceback (most recent call last):
         ...
-    ValueError: cards form an invalid hand
+    ValueError: The cards '3s4sQhTc' form an invalid hand.
     >>> e0 < e1
     True
     >>> e0.label
     <Label.HIGH_CARD: 'High card'>
     >>> e1.label
     <Label.TWO_PAIR: 'Two pair'>
     """
 
     rank_order = RankOrder.REGULAR
 
-    def __post_init__(self) -> None:
+    def _add_entries(self) -> None:
         self._add_multisets(Counter({1: 5}), (False, True), Label.HIGH_CARD)
         self._add_multisets(Counter({2: 1, 1: 3}), (False,), Label.ONE_PAIR)
         self._add_multisets(Counter({2: 2, 1: 1}), (False,), Label.TWO_PAIR)
         self._add_multisets(
             Counter({3: 1, 1: 2}),
             (False,),
             Label.THREE_OF_A_KIND,
@@ -414,49 +443,73 @@
 
     >>> lookup = BadugiLookup()
     >>> e0 = lookup.get_entry('2s')
     >>> e1 = lookup.get_entry('KhQc')
     >>> e2 = lookup.get_entry('AcAdAhAs')
     Traceback (most recent call last):
         ...
-    ValueError: cards form an invalid hand
+    ValueError: The cards 'AcAdAhAs' form an invalid hand.
     >>> e0 > e1
     True
     >>> e0.label
     <Label.HIGH_CARD: 'High card'>
     >>> e1.label
     <Label.HIGH_CARD: 'High card'>
     """
 
     rank_order = RankOrder.REGULAR
 
-    def __post_init__(self) -> None:
+    def _add_entries(self) -> None:
         for i in range(4, 0, -1):
             self._add_multisets(Counter({1: i}), (i == 1,), Label.HIGH_CARD)
 
+    def _get_key(self, cards: CardsLike) -> tuple[int, bool]:
+        cards = Card.clean(cards)
+
+        if not Card.are_rainbow(cards):
+            raise ValueError(
+                (
+                    'Badugi hands must be rainbow (i.e. of distinct suits) but'
+                    f' the cards {repr(cards)} are not.'
+                ),
+            )
+
+        return super()._get_key(cards)
+
+
+@dataclass
+class StandardBadugiLookup(BadugiLookup):
+    """The class for standard badugi hand lookups.
+
+    Lookups are used by evaluators. If you want to evaluate poker hands,
+    please use :class:`pokerkit.hands.StandardBadugiHand`.
+    """
+
+    rank_order = RankOrder.STANDARD
+
 
 @dataclass
 class KuhnPokerLookup(Lookup):
     """The class for Kuhn poker hand lookups.
 
     Lookups are used by evaluators. If you want to evaluate poker hands,
     please use :class:`pokerkit.hands.KuhnPokerHand`.
 
     >>> lookup = KuhnPokerLookup()
     >>> e0 = lookup.get_entry('J?')
     >>> e1 = lookup.get_entry('Q?')
     >>> e2 = lookup.get_entry('2?')
     Traceback (most recent call last):
         ...
-    ValueError: cards form an invalid hand
+    ValueError: The cards '2?' form an invalid hand.
     >>> e0 < e1
     True
     >>> e0.label
     <Label.HIGH_CARD: 'High card'>
     >>> e1.label
     <Label.HIGH_CARD: 'High card'>
     """
 
     rank_order = RankOrder.KUHN_POKER
 
-    def __post_init__(self) -> None:
+    def _add_entries(self) -> None:
         self._add_multisets(Counter({1: 1}), (True,), Label.HIGH_CARD)
```

### Comparing `pokerkit-0.4.9/pokerkit/notation.py` & `pokerkit-0.5.0a0/pokerkit/notation.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 notations.
 """
 
 from __future__ import annotations
 
 from collections.abc import Callable, Iterable, Iterator
 from collections import defaultdict, deque
-from dataclasses import asdict, dataclass, fields, KW_ONLY
+from dataclasses import asdict, dataclass, field, fields, KW_ONLY
 from functools import partial
 from operator import itemgetter
 from tomllib import loads as loads_toml
 from typing import Any, ClassVar, BinaryIO
 from warnings import warn
 import datetime
 
@@ -184,14 +184,18 @@
         'finishing_stacks',
         'currency',
         'ante_trimming_status',
         'time_limit',
         'time_banks',
     )
     """The optional field names."""
+    ACPC_PROTOCOL_VARIANTS = {'FT', 'NT'}
+    """The variant codes supported by the ACPC protocol."""
+    PLURIBUS_PROTOCOL_VARIANTS = {'NT'}
+    """The variant codes supported by the Pluribus protocol."""
     _: KW_ONLY
     variant: str
     """The variant name."""
     ante_trimming_status: bool = False
     """The ante trimming status."""
     antes: list[int]
     """The antes."""
@@ -251,14 +255,16 @@
     """The finishing stacks."""
     currency: str | None = None
     """The currency."""
     time_limit: int | None = None
     """The time limit."""
     time_banks: list[int] | None = None
     """The time banks."""
+    user_defined_fields: dict[str, Any] = field(default_factory=dict)
+    """The user-defined fields."""
     automations: tuple[Automation, ...] = (
         Automation.ANTE_POSTING,
         Automation.BET_COLLECTION,
         Automation.BLIND_OR_STRADDLE_POSTING,
         Automation.CARD_BURNING,
         Automation.HAND_KILLING,
         Automation.CHIPS_PUSHING,
@@ -271,21 +277,39 @@
     """The rake function."""
     parse_value: Callable[[str], int] = parse_value
     """The value parsing function."""
 
     @classmethod
     def _filter_non_fields(cls, **kwargs: Any) -> dict[str, Any]:
         field_names = {field.name for field in fields(cls)}
+        filtered_fields = {}
 
-        for key in tuple(kwargs.keys()):
-            if key not in field_names and not key.startswith('_'):
-                warn(f'unexpected field \'{key}\'')
-                kwargs.pop(key)
+        if 'user_defined_fields' in kwargs:
+            filtered_fields['user_defined_fields'] = kwargs.pop(
+                'user_defined_fields',
+            )
+        else:
+            filtered_fields['user_defined_fields'] = {}
+
+        for key, value in kwargs.items():
+            if key in field_names:
+                filtered_fields[key] = value
+            else:
+                if not key.startswith('_'):
+                    warn(
+                        (
+                            f'The field {repr(key)} is an unexpected field and'
+                            ' should probably be prefixed with an underscore'
+                            ' character \'_\'.'
+                        ),
+                    )
+
+                filtered_fields['user_defined_fields'][key] = value
 
-        return kwargs
+        return filtered_fields
 
     @classmethod
     def loads(
             cls,
             s: str,
             *,
             parse_value: Callable[[str], int] = parse_value,
@@ -326,39 +350,53 @@
 
         :param game: The game.
         :param state: The state.
         :param compression_status: The compression status.
         :param kwargs: The metadata.
         :return: The hand history.
         """
+
+        action: str | None
+
+        def append_dealing_actions() -> None:
+            nonlocal action
+
+            for player_index in hole_cards:
+                if hole_cards[player_index]:
+                    action = (
+                        f'd dh p{player_index + 1} '
+                        + ''.join(map(repr, hole_cards[player_index]))
+                    )
+
+                    actions.append(action.strip())
+                    hole_cards[player_index].clear()
+
+            if board_cards:
+                action = 'd db ' + ''.join(map(repr, board_cards))
+
+                actions.append(action.strip())
+                board_cards.clear()
+
         variant = cls.variants[type(game)]
         actions = []
-        cards = defaultdict[int, list[Card]](list)
+        hole_cards = defaultdict[int, list[Card]](list)
+        board_cards = list[Card]()
 
         for operation in state.operations:
-            action: str | None
-
             if (
                     not compression_status
-                    or not isinstance(operation, HoleDealing)
+                    or not isinstance(operation, HoleDealing | BoardDealing)
             ):
-                for player_index in cards:
-                    if cards[player_index]:
-                        action = (
-                            f'd dh p{player_index + 1} '
-                            + ''.join(map(repr, cards[player_index]))
-                        )
-
-                        actions.append(action.strip())
-                        cards[player_index].clear()
-
+                append_dealing_actions()
             if isinstance(operation, BoardDealing):
-                action = 'd db ' + ''.join(map(repr, operation.cards))
+                board_cards.extend(operation.cards)
+
+                action = None
             elif isinstance(operation, HoleDealing):
-                cards[operation.player_index].extend(operation.cards)
+                hole_cards[operation.player_index].extend(operation.cards)
 
                 action = None
             elif isinstance(operation, StandingPatOrDiscarding):
                 action = (
                     f'p{operation.player_index + 1} sd '
                     + ''.join(map(repr, operation.cards))
                 )
@@ -376,19 +414,24 @@
                 action = (
                     f'p{operation.player_index + 1} sm '
                     + ''.join(map(repr, operation.hole_cards))
                 )
             else:
                 action = None
 
+            if operation.commentary is not None:
+                if action is None:
+                    action = f'# {operation.commentary}'
+                else:
+                    action = action.strip() + f' # {operation.commentary}'
+
             if action is not None:
                 actions.append(action.strip())
 
-        assert not any(cards.values())
-
+        append_dealing_actions()
         kwargs.setdefault('variant', variant)
         kwargs.setdefault('actions', actions)
         kwargs.setdefault('starting_stacks', list(state.starting_stacks))
 
         field_names = {field.name for field in fields(cls)}
 
         for name in cls.required_field_names[variant]:
@@ -440,14 +483,17 @@
             elif state.can_kill_hand():
                 state.kill_hand()
             elif state.can_push_chips():
                 state.push_chips()
             elif state.can_pull_chips():
                 state.pull_chips()
             else:
+                if not actions:
+                    break
+
                 action = actions.popleft()
 
                 parse_action(state, action, self.parse_value)
 
             yield state, action
 
     @property
@@ -524,24 +570,267 @@
                         key in self.required_field_names[self.variant]
                         or key in self.optional_field_names
                     )
                     and value is not None
             ):
                 lines.append(f'{key} = {clean(value)}')
 
+        for key, value in self.user_defined_fields.items():
+            lines.append(f'{key} = {clean(value)}')
+
         return '\n'.join(lines)
 
     def dump(self, fp: BinaryIO) -> None:
         """Dump PHH to a file pointer.
 
         :param fp: The file pointer.
         :return: ``None``.
         """
         fp.write(self.dumps().encode())
 
+    def to_acpc_protocol(
+            self,
+            position: int,
+            hand_number: int | None = None,
+    ) -> Iterator[tuple[str, str]]:
+        """Convert to the ACPC protocol.
+
+        Only the fixed-limit/no-limit Texas hold'em variants are
+        supported.
+
+        :param position: The client position.
+        :param hand_number: The optional hand number. If ``None``, it is
+                            inferred from the field.
+        :return: The hand histories in the ACPC protocol.
+        :raises ValueError: If the game is not supported or the hand
+                            number cannot be determined.
+        """
+        if self.variant not in self.ACPC_PROTOCOL_VARIANTS:
+            raise ValueError(
+                (
+                    f'The variant {repr(self.variant)} is not among the'
+                    ' supported ACPC variants'
+                    f' {repr(self.ACPC_PROTOCOL_VARIANTS)}.'
+                ),
+            )
+
+        if hand_number is None:
+            if self.hand is None:
+                raise ValueError(
+                    (
+                        'Since the hand number is not defined in the hand'
+                        ' history object, it must be passed as an argument.'
+                    ),
+                )
+
+            hand_number = self.hand
+
+        index = 0
+        actions = ''
+        raw_hole_cards = [['', ''] for _ in self.starting_stacks]
+        hole_cards = ''
+        board_cards = ''
+        match_state = ''
+        action = ''
+
+        def egress() -> tuple[str, str]:
+            if not all(raw_hole_cards[position]):
+                raise ValueError(
+                    'The hole cards at the desired position must be known.',
+                )
+
+            return 'S->', f'{match_state}\r\n'
+
+        def ingress() -> tuple[str, str]:
+            return '<-C', f'{match_state}:{action}\r\n'
+
+        for state in self:
+            while index < len(state.operations):
+                operation = state.operations[index]
+                index += 1
+
+                if (
+                        isinstance(
+                            operation,
+                            (
+                                Folding
+                                | CheckingOrCalling
+                                | CompletionBettingOrRaisingTo
+                            ),
+                        )
+                ):
+                    yield egress()
+
+                if isinstance(operation, Folding):
+                    action = 'f'
+                    actions += action
+                elif isinstance(operation, CheckingOrCalling):
+                    action = 'c'
+                    actions += action
+                elif isinstance(operation, CompletionBettingOrRaisingTo):
+                    match self.variant:
+                        case 'FT':
+                            action = 'r'
+                        case 'NT':
+                            amount = (
+                                state.starting_stacks[operation.player_index]
+                                - state.stacks[operation.player_index]
+                            )
+                            action = f'r{amount}'
+                        case _:
+                            raise AssertionError
+
+                    actions += action
+
+                if (
+                        isinstance(
+                            operation,
+                            (
+                                Folding
+                                | CheckingOrCalling
+                                | CompletionBettingOrRaisingTo
+                            ),
+                        )
+                        and operation.player_index == position
+                ):
+                    yield ingress()
+
+                if isinstance(operation, HoleDealing):
+                    if operation.player_index == position:
+                        for i, card in enumerate(operation.cards):
+                            if not card.unknown_status:
+                                raw_hole_cards[position][i] = repr(card)
+                elif isinstance(operation, HoleCardsShowingOrMucking):
+                    for i, card in enumerate(operation.hole_cards):
+                        if not card.unknown_status:
+                            raw_hole_cards[operation.player_index][i] = (
+                                repr(card)
+                            )
+
+                if isinstance(operation, BoardDealing):
+                    actions += '/'
+                    board_cards += '/' + ''.join(map(repr, operation.cards))
+
+                hole_cards = '|'.join(map(''.join, raw_hole_cards))
+                match_state = (
+                    f'MATCHSTATE'
+                    f':{position}'
+                    f':{hand_number}'
+                    f':{actions}'
+                    f':{hole_cards}{board_cards}'
+                )
+
+        if not state.status or state.actor_index is not None:
+            yield egress()
+
+    def to_pluribus_protocol(
+            self,
+            hand_number: int | None = None,
+    ) -> str:
+        """Convert to the Pluribus protocol.
+
+        Only the no-limit Texas hold'em variant is supported.
+
+        :param hand_number: The optional hand number. If ``None``, it is
+                            inferred from the field.
+        :return: The hand histories in the Pluribus protocol.
+        :raises ValueError: If the game is not supported or the hand
+                            number cannot be determined.
+        """
+        if self.variant not in self.PLURIBUS_PROTOCOL_VARIANTS:
+            raise ValueError(
+                (
+                    f'The variant {repr(self.variant)} is not among the'
+                    ' supported variants for pluribus notation'
+                    f' {repr(self.PLURIBUS_PROTOCOL_VARIANTS)}.'
+                ),
+            )
+
+        if hand_number is None:
+            if self.hand is None:
+                raise ValueError(
+                    (
+                        'Since the hand number is not defined in the hand'
+                        ' history object, it must be passed as an argument.'
+                    ),
+                )
+
+            hand_number = self.hand
+
+        index = 0
+        actions = ''
+        raw_hole_cards = [['', ''] for _ in self.starting_stacks]
+        board_cards = ''
+
+        for state in self:
+            while index < len(state.operations):
+                operation = state.operations[index]
+                index += 1
+
+                if isinstance(operation, Folding):
+                    actions += 'f'
+                elif isinstance(operation, CheckingOrCalling):
+                    actions += 'c'
+                elif isinstance(operation, CompletionBettingOrRaisingTo):
+                    amount = (
+                        state.starting_stacks[operation.player_index]
+                        - state.stacks[operation.player_index]
+                    )
+                    actions += f'r{amount}'
+                elif isinstance(operation, HoleDealing):
+                    for i, card in enumerate(operation.cards):
+                        if not card.unknown_status:
+                            raw_hole_cards[operation.player_index][i] = repr(
+                                card,
+                            )
+                elif isinstance(operation, HoleCardsShowingOrMucking):
+                    for i, card in enumerate(operation.hole_cards):
+                        if not card.unknown_status:
+                            raw_hole_cards[operation.player_index][i] = (
+                                repr(card)
+                            )
+                elif isinstance(operation, BoardDealing):
+                    actions += '/'
+                    board_cards += '/' + ''.join(map(repr, operation.cards))
+
+        hole_cards = '|'.join(map(''.join, raw_hole_cards))
+        raw_payoffs = []
+
+        if self.finishing_stacks is None:
+            finishing_stacks = tuple(self)[-1].stacks
+        else:
+            finishing_stacks = self.finishing_stacks
+
+        for starting_stack, finishing_stack in zip(
+                self.starting_stacks,
+                finishing_stacks,
+        ):
+            raw_payoffs.append(finishing_stack - starting_stack)
+
+        payoffs = '|'.join(map(str, raw_payoffs))
+
+        if self.players is None:
+            raw_players = [
+                f'p{i + 1}' for i in range(len(self.starting_stacks))
+            ]
+        else:
+            raw_players = self.players
+
+        players = '|'.join(raw_players)
+        match_state = (
+            f'STATE'
+            f':{hand_number}'
+            f':{actions}'
+            f':{hole_cards}{board_cards}'
+            f':{payoffs}'
+            f':{players}'
+        )
+
+        return match_state
+
 
 def parse_action(
         state: State,
         action: str,
         parse_value: Callable[[str], int] = parse_value,
 ) -> None:
     """Parse the action.
@@ -551,51 +840,62 @@
     :param parse_value: The value parsing function.
     :return: ``None``.
     """
     def verify_player(index: int | None) -> None:
         label, parsed_index = player[:1], int(player[1:]) - 1
 
         if label != 'p' or parsed_index != index:
-            raise ValueError(f'invalid Player \'{player}\'')
+            raise ValueError(
+                (
+                    f'The player {repr(player)} is not a valid player for the'
+                    f' action {repr(action)}.'
+                ),
+            )
 
+    commentary = action[action.index('#') + 2:] if '#' in action else None
     words = action.split()
 
     if '#' in words:
         words = words[:words.index('#')]
 
     match words:
         case 'd', 'db', cards:
             state.deal_board(cards)
         case 'd', 'dh', player, cards:
             verify_player(state.hole_dealee_index)
-            state.deal_hole(cards)
+            state.deal_hole(cards, commentary=commentary)
         case player, 'sd':
             verify_player(state.stander_pat_or_discarder_index)
-            state.stand_pat_or_discard()
+            state.stand_pat_or_discard(commentary=commentary)
         case player, 'sd', cards:
             verify_player(state.stander_pat_or_discarder_index)
-            state.stand_pat_or_discard(cards)
+            state.stand_pat_or_discard(cards, commentary=commentary)
         case player, 'pb':
             verify_player(state.actor_index)
-            state.post_bring_in()
+            state.post_bring_in(commentary=commentary)
         case player, 'f':
             verify_player(state.actor_index)
-            state.fold()
+            state.fold(commentary=commentary)
         case player, 'cc':
             verify_player(state.actor_index)
-            state.check_or_call()
+            state.check_or_call(commentary=commentary)
         case player, 'cbr', amount:
             verify_player(state.actor_index)
-            state.complete_bet_or_raise_to(parse_value(amount))
+            state.complete_bet_or_raise_to(
+                parse_value(amount),
+                commentary=commentary,
+            )
         case player, 'sm':
             verify_player(state.showdown_index)
-            state.show_or_muck_hole_cards(False)
+            state.show_or_muck_hole_cards(False, commentary=commentary)
         case player, 'sm', '-':
             verify_player(state.showdown_index)
-            state.show_or_muck_hole_cards(True)
+            state.show_or_muck_hole_cards(True, commentary=commentary)
         case player, 'sm', cards:
             verify_player(state.showdown_index)
-            state.show_or_muck_hole_cards(cards)
+            state.show_or_muck_hole_cards(cards, commentary=commentary)
         case ():
-            pass
+            state.no_operate(commentary=commentary)
         case _:
-            raise ValueError(f'invalid action \'{action}\'')
+            raise ValueError(
+                f'The action {repr(action)} is an invalid action.',
+            )
```

### Comparing `pokerkit-0.4.9/pokerkit/tests/test_lookups.py` & `pokerkit-0.5.0a0/pokerkit/tests/test_lookups.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 from pokerkit.lookups import (
     BadugiLookup,
     EightOrBetterLookup,
     KuhnPokerLookup,
     RegularLookup,
     ShortDeckHoldemLookup,
+    StandardBadugiLookup,
     StandardLookup,
 )
 from pokerkit.utilities import Card, Deck
 
 
 class LookupTestCaseMixin:
     @classmethod
@@ -65,50 +66,77 @@
         )
 
 
 class EightOrBetterLookupTestCase(LookupTestCaseMixin, TestCase):
     def test_get_entry(self) -> None:
         lookup = EightOrBetterLookup()
         combinations_ = sorted(
-            filter(lookup.has_entry, combinations(Deck.STANDARD, 5)),
+            filter(lookup.has_entry, combinations(Deck.REGULAR, 5)),
             key=lookup.get_entry,
         )
         string = self.serialize_combinations(combinations_)
         algorithm = md5()
         algorithm.update(string.encode())
 
         self.assertEqual(
             algorithm.hexdigest(),
-            'd765d50ed799d03a8f062a3d5a31ad5c',
+            'ecf2b6b16031562a6761932b1ce1de91',
         )
 
 
 class RegularLookupTestCase(LookupTestCaseMixin, TestCase):
     def test_get_entry(self) -> None:
         lookup = RegularLookup()
         combinations_ = sorted(
-            combinations(Deck.STANDARD, 5),
+            combinations(Deck.REGULAR, 5),
             key=lookup.get_entry,
         )
         string = self.serialize_combinations(combinations_)
         algorithm = md5()
         algorithm.update(string.encode())
 
         self.assertEqual(
             algorithm.hexdigest(),
-            'edd288a3022b2763475a533ad2a102e9',
+            '28925b97b06a1e674eaabf241a441e15',
         )
 
 
 class BadugiLookupTestCase(LookupTestCaseMixin, TestCase):
     def test_get_entry(self) -> None:
         lookup = BadugiLookup()
         combinations_ = []
 
         for n in range(1, 5):
+            for cards in combinations(Deck.REGULAR, n):
+                pairedness = Card.are_paired(cards)
+                suitedness = Card.are_suited(cards)
+                rainbowness = Card.are_rainbow(cards)
+
+                if not pairedness and rainbowness:
+                    combinations_.append(cards)
+                elif pairedness or suitedness:
+                    self.assertRaises(ValueError, lookup.get_entry, cards)
+
+        combinations_.sort(key=lookup.get_entry)
+        string = self.serialize_combinations(combinations_)
+        algorithm = md5()
+        algorithm.update(string.encode())
+
+        self.assertEqual(
+            algorithm.hexdigest(),
+            '9d29ddbc3f76d815e166c6faa2af9021',
+        )
+
+
+class StandardBadugiLookupTestCase(LookupTestCaseMixin, TestCase):
+    def test_get_entry(self) -> None:
+        lookup = StandardBadugiLookup()
+        combinations_ = []
+
+        for n in range(1, 5):
             for cards in combinations(Deck.STANDARD, n):
                 pairedness = Card.are_paired(cards)
                 suitedness = Card.are_suited(cards)
                 rainbowness = Card.are_rainbow(cards)
 
                 if not pairedness and rainbowness:
                     combinations_.append(cards)
@@ -118,15 +146,15 @@
         combinations_.sort(key=lookup.get_entry)
         string = self.serialize_combinations(combinations_)
         algorithm = md5()
         algorithm.update(string.encode())
 
         self.assertEqual(
             algorithm.hexdigest(),
-            'c284d3bf45c87707f62cd7fc6699c31a',
+            '06886dd57a4c7b780953f5090c63bcfe',
         )
 
 
 class KuhnPokerLookupTestCase(LookupTestCaseMixin, TestCase):
     def test_get_entry(self) -> None:
         lookup = KuhnPokerLookup()
         combinations_ = sorted(
```

### Comparing `pokerkit-0.4.9/pokerkit/tests/test_papers.py` & `pokerkit-0.5.0a0/pokerkit/tests/test_papers.py`

 * *Files 10% similar despite different names*

```diff
@@ -433,122 +433,179 @@
             hh.actions,
         )
         self.assertEqual(new_state.stacks, [1937923.75, 0.0])
         self.assertEqual(new_state.operations, state.operations)
         self.assertEqual(s, hh.dumps())
 
     def test_arieh_yockey_2019(self) -> None:
-        s = dedent(
-            '''\
-            # A bad beat between Yockey and Arieh.
-            # Link: https://youtu.be/pChCqb2FNxY
-
-            variant = "F2L3D"
-            ante_trimming_status = true
-            antes = [0, 0, 0, 0]
-            blinds_or_straddles = [75000, 150000, 0, 0]
-            small_bet = 150000
-            big_bet = 300000
-            starting_stacks = [1180000, 4340000, 5910000, 10765000]
-            actions = [
-              # Pre-draw
-
-              "d dh p1 7h6c4c3d2c",  # Yockey
-              "d dh p2 ??????????",  # Hui
-              "d dh p3 ??????????",  # Esposito
-              "d dh p4 AsQs6s5c3c",  # Arieh
-
-              "p3 f",  # Esposito
-              "p4 cbr 300000",  # Arieh
-              "p1 cbr 450000",  # Yockey
-              "p2 f",  # Hui
-              "p4 cc",  # Arieh
-
-              # First draw
-
-              "p1 sd",  # Yockey
-              "p4 sd AsQs",  # Arieh
-              "d dh p4 2hQh",  # Arieh
-
-              "p1 cbr 150000",  # Yockey
-              "p4 cc",  # Arieh
-
-              # Second draw
-
-              "p1 sd",  # Yockey
-              "p4 sd Qh",  # Arieh
-              "d dh p4 4d",  # Arieh
-
-              "p1 cbr 300000",  # Yockey
-              "p4 cc",  # Arieh
-
-              # Third draw
-
-              "p1 sd",  # Yockey
-              "p4 sd 6s",  # Arieh
-              "d dh p4 7c",  # Arieh
-
-              "p1 cbr 280000",  # Yockey
-              "p4 cc",  # Arieh
-
-              # Showdown
-
-              "p1 sm 7h6c4c3d2c",  # Yockey
-              "p4 sm 2h4d7c5c3c",  # Arieh
-            ]
-            author = "Juho Kim"
-            event = """2019 World Series of Poker Event #58: $50,000 Poker \\
-            Players Championship | Day 5"""
-            city = "Las Vegas"
-            region = "Nevada"
-            country = "United States of America"
-            day = 28
-            month = 6
-            year = 2019
-            players = [
-              "Bryce Yockey",
-              "Phil Hui",
-              "John Esposito",
-              "Josh Arieh",
-            ]
-            '''
-        )
-        hh = HandHistory.loads(s)
-        it = iter(hh)
-        state = next(it)
-
-        while state.status:
+        for s in map(
+            dedent,
+            (
+                '''\
+                # A bad beat between Yockey and Arieh.
+                # Link: https://youtu.be/pChCqb2FNxY
+
+                variant = "F2L3D"
+                ante_trimming_status = true
+                antes = [0, 0, 0, 0]
+                blinds_or_straddles = [75000, 150000, 0, 0]
+                small_bet = 150000
+                big_bet = 300000
+                starting_stacks = [1180000, 4340000, 5910000, 10765000]
+                actions = [
+                  # Pre-draw
+
+                  "d dh p1 7h6c4c3d2c",  # Yockey
+                  "d dh p2 ??????????",  # Hui
+                  "d dh p3 ??????????",  # Esposito
+                  "d dh p4 AsQs6s5c3c",  # Arieh
+
+                  "p3 f",  # Esposito
+                  "p4 cbr 300000",  # Arieh
+                  "p1 cbr 450000",  # Yockey
+                  "p2 f",  # Hui
+                  "p4 cc",  # Arieh
+
+                  # First draw
+
+                  "p1 sd",  # Yockey
+                  "p4 sd AsQs",  # Arieh
+                  "d dh p4 2hQh",  # Arieh
+
+                  "p1 cbr 150000",  # Yockey
+                  "p4 cc",  # Arieh
+
+                  # Second draw
+
+                  "p1 sd",  # Yockey
+                  "p4 sd Qh",  # Arieh
+                  "d dh p4 4d",  # Arieh
+
+                  "p1 cbr 300000",  # Yockey
+                  "p4 cc",  # Arieh
+
+                  # Third draw
+
+                  "p1 sd",  # Yockey
+                  "p4 sd 6s",  # Arieh
+                  "d dh p4 7c",  # Arieh
+
+                  "p1 cbr 280000",  # Yockey
+                  "p4 cc",  # Arieh
+
+                  # Showdown
+
+                  "p1 sm 7h6c4c3d2c",  # Yockey
+                  "p4 sm 2h4d7c5c3c",  # Arieh
+                ]
+                author = "Juho Kim"
+                event = """2019 World Series of Poker Event #58: $50,000 \\
+                Poker Players Championship | Day 5"""
+                city = "Las Vegas"
+                region = "Nevada"
+                country = "United States of America"
+                day = 28
+                month = 6
+                year = 2019
+                players = [
+                  "Bryce Yockey",
+                  "Phil Hui",
+                  "John Esposito",
+                  "Josh Arieh",
+                ]
+                ''',
+                '''
+                # A bad beat between Yockey and Arieh.
+                variant = "F2L3D"
+                antes = [0, 0, 0, 0]
+                blinds_or_straddles = [
+                75000, 150000, 0, 0,
+                ]
+                small_bet = 150000
+                big_bet = 300000
+                starting_stacks = [
+                  1180000, 4340000, 5910000, 10765000,
+                ]
+                actions = [
+                  "d dh p1 7h6c4c3d2c", # Yockey
+                  "d dh p2 ??????????", # Hui
+                  "d dh p3 ??????????", # Esposito
+                  "d dh p4 AsQs6s5c3c", # Arieh
+                  "p3 f", # Esposito
+                  "p4 cbr 300000", # Arieh
+                  "p1 cbr 450000", # Yockey
+                  "p2 f", # Hui
+                  "p4 cc", # Arieh
+                  "p1 sd", # First draw; Yockey
+                  "p4 sd AsQs", # Arieh
+                  "d dh p4 2hQh", # Arieh
+                  "p1 cbr 150000", # Yockey
+                  "p4 cc", # Arieh
+                  "p1 sd", # Second draw; Yockey
+                  "p4 sd Qh", # Arieh
+                  "d dh p4 4d", # Arieh
+                  "p1 cbr 300000", # Yockey
+                  "p4 cc", # Arieh
+                  "p1 sd", # Third draw; Yockey
+                  "p4 sd 6s", # Arieh
+                  "d dh p4 7c", # Arieh
+                  "p1 cbr 280000", # Yockey
+                  "p4 cc", # Arieh
+                  "p1 sm 7h6c4c3d2c", # Showdown; Yockey
+                  "p4 sm 2h4d7c5c3c", # Arieh
+                ]
+                event = "2019 WSOP Event #58"
+                city = "Las Vegas"
+                region = "Nevada"
+                country = "United States of America"
+                day = 28
+                month = 6
+                year = 2019
+                players = [
+                  "Bryce Yockey", "Phil Hui",
+                  "John Esposito", "Josh Arieh",
+                ]
+                ''',
+            ),
+        ):
+            hh = HandHistory.loads(s)
+            it = iter(hh)
             state = next(it)
 
-        self.assertRaises(StopIteration, next, it)
-        self.assertEqual(state.stacks, [0, 4190000, 5910000, 12095000])
-
-        s = hh.dumps()
-        hh = HandHistory.loads(s)
-        new_state = tuple(hh)[-1]
+            while state.status:
+                state = next(it)
 
-        self.assertEqual(
-            list(map(itemgetter(1), hh.iter_state_actions())),
-            [None] + hh.actions,
-        )
-        self.assertEqual(new_state.stacks, [0, 4190000, 5910000, 12095000])
-        self.assertEqual(new_state.operations, state.operations)
-        self.assertEqual(s, hh.dumps())
+            self.assertRaises(StopIteration, next, it)
+            self.assertEqual(state.stacks, [0, 4190000, 5910000, 12095000])
 
-        hh = HandHistory.loads(s, automations=())
-        new_state = tuple(hh)[-1]
-
-        self.assertEqual(len(tuple(hh)), len(new_state.operations) + 1)
-        self.assertEqual(
-            list(filter(None, map(itemgetter(1), hh.iter_state_actions()))),
-            hh.actions,
-        )
-        self.assertEqual(new_state.stacks, [0, 4190000, 5910000, 12095000])
-        self.assertEqual(new_state.operations, state.operations)
-        self.assertEqual(s, hh.dumps())
+            s = hh.dumps()
+            hh = HandHistory.loads(s)
+            new_state = tuple(hh)[-1]
+
+            self.assertEqual(
+                list(map(itemgetter(1), hh.iter_state_actions())),
+                [None] + hh.actions,
+            )
+            self.assertEqual(new_state.stacks, [0, 4190000, 5910000, 12095000])
+            self.assertEqual(new_state.operations, state.operations)
+            self.assertEqual(s, hh.dumps())
+
+            hh = HandHistory.loads(s, automations=())
+            new_state = tuple(hh)[-1]
+
+            self.assertEqual(len(tuple(hh)), len(new_state.operations) + 1)
+            self.assertEqual(
+                list(
+                    filter(None, map(itemgetter(1), hh.iter_state_actions())),
+                ),
+                hh.actions,
+            )
+            self.assertEqual(new_state.stacks, [0, 4190000, 5910000, 12095000])
+            self.assertEqual(new_state.operations, state.operations)
+            self.assertEqual(s, hh.dumps())
 
     def test_alice_carol_wikipedia(self) -> None:
         s = dedent(
             '''\
             # An example badugi hand from Wikipedia.
             # Link: https://en.wikipedia.org/wiki/Badugi
 
@@ -651,17 +708,120 @@
         )
         self.assertEqual(new_state.stacks, [196, 220, 200, 184])
         self.assertEqual(new_state.operations, state.operations)
         self.assertEqual(s, hh.dumps())
 
 
 class READMETestCase(TestCase):
+    def test_hellmuth_wiggins(self) -> None:
+        # The 4-runout hand between Phil Hellmuth and the Loose Cannon Ernest
+        # Wiggins.
+        # Link: https://youtu.be/cnjJv7x0HMY?si=4l05Ez7lQVczt8DI&t=638
+
+        from pokerkit import Automation, Mode, NoLimitTexasHoldem
+
+        # Set up the game.
+
+        state = NoLimitTexasHoldem.create_state(
+            # Automations
+            (
+                Automation.ANTE_POSTING,
+                Automation.BET_COLLECTION,
+                Automation.BLIND_OR_STRADDLE_POSTING,
+                Automation.HOLE_CARDS_SHOWING_OR_MUCKING,
+                Automation.HAND_KILLING,
+                Automation.CHIPS_PUSHING,
+                Automation.CHIPS_PULLING,
+            ),
+            False,  # Uniform antes?
+            {-1: 600},  # Antes
+            (200, 400, 800),  # Blinds or straddles
+            400,  # Min-bet
+            (999999, 116400, 86900, 999999, 50000, 999999),  # Starting stacks
+            6,  # Number of players
+            mode=Mode.CASH_GAME,
+        )
+
+        # Below are the pre-flop dealings and actions.
+
+        state.deal_hole('JsTh')  # Tony G
+        state.deal_hole('Ah9d')  # Hellmuth
+        state.deal_hole('KsKc')  # Wiggins
+        state.deal_hole('5c2h')  # Negreanu
+        state.deal_hole('6h5h')  # Brunson
+        state.deal_hole('6s3s')  # Laak
+
+        state.fold()  # Negreanu
+        state.complete_bet_or_raise_to(2800)  # Brunson
+        state.fold()  # Laak
+        state.check_or_call()  # Tony G
+        state.complete_bet_or_raise_to(12600)  # Hellmuth
+        state.check_or_call()  # Wiggins
+        state.check_or_call()  # Brunson
+        state.check_or_call()  # Tony G
+
+        # Below are the flop dealing and actions.
+
+        state.burn_card('??')
+        state.deal_board('9hTs9s')
+
+        state.check_or_call()  # Tony G
+        state.complete_bet_or_raise_to(17000)  # Hellmuth
+        state.complete_bet_or_raise_to(36000)  # Wiggins
+        state.fold()  # Brunson
+        state.fold()  # Tony G
+        state.complete_bet_or_raise_to(103800)  # Hellmuth
+        state.check_or_call()  # Wiggins
+
+        # Below is selecting the number of runouts.
+
+        state.select_runout_count(4)  # Hellmuth
+        state.select_runout_count(None)  # Wiggins
+
+        # Below is the first runout.
+
+        state.burn_card('??')
+        state.deal_board('Jh')  # Turn
+        state.burn_card('??')
+        state.deal_board('Ad')  # River
+
+        # Below is the second runout.
+
+        state.burn_card('??')
+        state.deal_board('Kh')  # Turn
+        state.burn_card('??')
+        state.deal_board('3c')  # River
+
+        # Below is the third runout.
+
+        state.burn_card('??')
+        state.deal_board('7s')  # Turn
+        state.burn_card('??')
+        state.deal_board('8s')  # River
+
+        # Below is the fourth runout.
+
+        state.burn_card('??')
+        state.deal_board('Qc')  # Turn
+        state.burn_card('??')
+        state.deal_board('Kd')  # River
+
+        # Below are the final stacks.
+
+        # print(state.stacks)  # [987399, 79400, 149700, 999999, 37400, 999399]
+
+        self.assertEqual(
+            state.stacks,
+            [987399, 79400, 149700, 999999, 37400, 999399],
+        )
+
     def test_dwan_ivey(self) -> None:
-        # The first televised million dollar pot between Tom Dwan and Phil
-        # Ivey.
+        # Below shows the first televised million-dollar pot between Tom Dwan
+        # and Phil Ivey.
+        #
         # Link: https://youtu.be/GnxFohpljqM
 
         from pokerkit import Automation, NoLimitTexasHoldem
 
         state = NoLimitTexasHoldem.create_state(
             (
                 Automation.ANTE_POSTING,
@@ -676,56 +836,57 @@
             500,
             (1000, 2000),
             2000,
             (1125600, 2000000, 553500),
             3,
         )
 
-        # Below shows the pre-flop dealings and actions.
+        # Below are the pre-flop dealings and actions.
 
         state.deal_hole('Ac2d')  # Ivey
         state.deal_hole('????')  # Antonius
         state.deal_hole('7h6h')  # Dwan
 
         state.complete_bet_or_raise_to(7000)  # Dwan
         state.complete_bet_or_raise_to(23000)  # Ivey
         state.fold()  # Antonius
         state.check_or_call()  # Dwan
 
-        # Below shows the flop dealing and actions.
+        # Below are the flop dealing and actions.
 
         state.burn_card('??')
         state.deal_board('Jc3d5c')
 
         state.complete_bet_or_raise_to(35000)  # Ivey
         state.check_or_call()  # Dwan
 
-        # Below shows the turn dealing and actions.
+        # Below are the turn dealing and actions.
 
         state.burn_card('??')
         state.deal_board('4h')
 
         state.complete_bet_or_raise_to(90000)  # Ivey
         state.complete_bet_or_raise_to(232600)  # Dwan
         state.complete_bet_or_raise_to(1067100)  # Ivey
         state.check_or_call()  # Dwan
 
-        # Below shows the river dealing.
+        # Below is the river dealing.
 
         state.burn_card('??')
         state.deal_board('Jh')
 
-        # Below show the final stacks.
+        # Below are the final stacks.
 
         # print(state.stacks)  # [572100, 1997500, 1109500]
 
         self.assertEqual(state.stacks, [572100, 1997500, 1109500])
 
     def test_phua_xuan(self) -> None:
-        # An all-in hand between Xuan and Phua.
+        # Below shows an all-in hand between Xuan and Phua.
+        #
         # Link: https://youtu.be/QlgCcphLjaQ
 
         from pokerkit import Automation, NoLimitShortDeckHoldem
 
         state = NoLimitShortDeckHoldem.create_state(
             (
                 Automation.ANTE_POSTING,
@@ -740,15 +901,15 @@
             3000,
             {-1: 3000},
             3000,
             (495000, 232000, 362000, 403000, 301000, 204000),
             6,
         )
 
-        # Below shows the pre-flop dealings and actions.
+        # Below are the pre-flop dealings and actions.
 
         state.deal_hole('Th8h')  # Badziakouski
         state.deal_hole('QsJd')  # Zhong
         state.deal_hole('QhQd')  # Xuan
         state.deal_hole('8d7c')  # Jun
         state.deal_hole('KhKs')  # Phua
         state.deal_hole('8c7h')  # Koon
@@ -759,41 +920,42 @@
         state.fold()  # Jun
         state.complete_bet_or_raise_to(298000)  # Phua
         state.fold()  # Koon
         state.fold()  # Badziakouski
         state.fold()  # Zhong
         state.check_or_call()  # Xuan
 
-        # Below shows the flop dealing.
+        # Below is the flop dealing.
 
         state.burn_card('??')
         state.deal_board('9h6cKc')
 
-        # Below shows the turn dealing.
+        # Below is the turn dealing.
 
         state.burn_card('??')
         state.deal_board('Jh')
 
-        # Below shows the river dealing.
+        # Below is the river dealing.
 
         state.burn_card('??')
         state.deal_board('Ts')
 
-        # Below show the final stacks.
+        # Below are the final stacks.
 
         # print(state.stacks)  # [489000, 226000, 684000, 400000, 0, 198000]
 
         self.assertEqual(
             state.stacks,
             [489000, 226000, 684000, 400000, 0, 198000],
         )
 
     def test_antonius_blom(self) -> None:
-        # The largest online poker pot every played between Patrik Antonius and
-        # Viktor Blom.
+        # Below shows the largest online poker pot ever played between Patrik
+        # Antonius and Viktor Blom.
+        #
         # Link: https://youtu.be/UMBm66Id2AA
 
         from pokerkit import Automation, PotLimitOmahaHoldem
 
         state = PotLimitOmahaHoldem.create_state(
             (
                 Automation.ANTE_POSTING,
@@ -808,53 +970,54 @@
             0,
             (500, 1000),
             2000,
             (1259450.25, 678473.5),  # type: ignore[arg-type]
             2,
         )
 
-        # Below shows the pre-flop dealings and actions.
+        # Below are the pre-flop dealings and actions.
 
         state.deal_hole('Ah3sKsKh')  # Antonius
         state.deal_hole('6d9s7d8h')  # Blom
 
         state.complete_bet_or_raise_to(3000)  # Blom
         state.complete_bet_or_raise_to(9000)  # Antonius
         state.complete_bet_or_raise_to(27000)  # Blom
         state.complete_bet_or_raise_to(81000)  # Antonius
         state.check_or_call()  # Blom
 
-        # Below shows the flop dealing and actions.
+        # Below are the flop dealing and actions.
 
         state.burn_card('??')
         state.deal_board('4s5c2h')
 
         state.complete_bet_or_raise_to(91000)  # Antonius
         state.complete_bet_or_raise_to(435000)  # Blom
         state.complete_bet_or_raise_to(779000)  # Antonius
         state.check_or_call()  # Blom
 
-        # Below shows the turn dealing.
+        # Below is the turn dealing.
 
         state.burn_card('??')
         state.deal_board('5h')
 
-        # Below shows the river dealing.
+        # Below is the river dealing.
 
         state.burn_card('??')
         state.deal_board('9c')
 
-        # Below show the final stacks.
+        # Below are the final stacks.
 
         # print(state.stacks)  # [1937923.75, 0.0]
 
         self.assertEqual(state.stacks, [1937923.75, 0.0])
 
     def test_yockey_arieh(self) -> None:
-        # A bad beat between Yockey and Arieh.
+        # Below shows a bad beat between Yockey and Arieh.
+        #
         # Link: https://youtu.be/pChCqb2FNxY
 
         from pokerkit import (
             Automation,
             FixedLimitDeuceToSevenLowballTripleDraw,
         )
 
@@ -873,65 +1036,66 @@
             (75000, 150000),
             150000,
             300000,
             (1180000, 4340000, 5910000, 10765000),
             4,
         )
 
-        # Below shows the pre-flop dealings and actions.
+        # Below are the pre-flop dealings and actions.
 
         state.deal_hole('7h6c4c3d2c')  # Yockey
         state.deal_hole('??????????')  # Hui
         state.deal_hole('??????????')  # Esposito
         state.deal_hole('AsQs6s5c3c')  # Arieh
 
         state.fold()  # Esposito
         state.complete_bet_or_raise_to()  # Arieh
         state.complete_bet_or_raise_to()  # Yockey
         state.fold()  # Hui
         state.check_or_call()  # Arieh
 
-        # Below shows the first draw and actions.
+        # Below are the first draw and actions.
 
         state.stand_pat_or_discard()  # Yockey
         state.stand_pat_or_discard('AsQs')  # Arieh
         state.burn_card('??')
         state.deal_hole('2hQh')  # Arieh
 
         state.complete_bet_or_raise_to()  # Yockey
         state.check_or_call()  # Arieh
 
-        # Below shows the second draw and actions.
+        # Below are the second draw and actions.
 
         state.stand_pat_or_discard()  # Yockey
         state.stand_pat_or_discard('Qh')  # Arieh
         state.burn_card('??')
         state.deal_hole('4d')  # Arieh
 
         state.complete_bet_or_raise_to()  # Yockey
         state.check_or_call()  # Arieh
 
-        # Below shows the third draw and actions.
+        # Below are the third draw and actions.
 
         state.stand_pat_or_discard()  # Yockey
         state.stand_pat_or_discard('6s')  # Arieh
         state.burn_card('??')
         state.deal_hole('7c')  # Arieh
 
         state.complete_bet_or_raise_to()  # Yockey
         state.check_or_call()  # Arieh
 
-        # Below show the final stacks.
+        # Below are the final stacks.
 
         # print(state.stacks)  # [0, 4190000, 5910000, 12095000]
 
         self.assertEqual(state.stacks, [0, 4190000, 5910000, 12095000])
 
     def test_alice_carol(self) -> None:
-        # An example badugi hand from Wikipedia.
+        # Below shows an example badugi hand from Wikipedia.
+        #
         # Link: https://en.wikipedia.org/wiki/Badugi
 
         from pokerkit import Automation, FixedLimitBadugi
 
         state = FixedLimitBadugi.create_state(
             (
                 Automation.ANTE_POSTING,
@@ -946,73 +1110,73 @@
             (1, 2),
             2,
             4,
             200,
             4,
         )
 
-        # Below shows the pre-flop dealings and actions.
+        # Below are the pre-flop dealings and actions.
 
         state.deal_hole('????????')  # Bob
         state.deal_hole('????????')  # Carol
         state.deal_hole('????????')  # Ted
         state.deal_hole('????????')  # Alice
 
         state.fold()  # Ted
         state.check_or_call()  # Alice
         state.check_or_call()  # Bob
         state.check_or_call()  # Carol
 
-        # Below shows the first draw and actions.
+        # Below are the first draw and actions.
 
         state.stand_pat_or_discard('????')  # Bob
         state.stand_pat_or_discard('????')  # Carol
         state.stand_pat_or_discard('??')  # Alice
         state.burn_card('??')
         state.deal_hole('????')  # Bob
         state.deal_hole('????')  # Carol
         state.deal_hole('??')  # Alice
 
         state.check_or_call()  # Bob
         state.complete_bet_or_raise_to()  # Carol
         state.check_or_call()  # Alice
         state.check_or_call()  # Bob
 
-        # Below shows the second draw and actions.
+        # Below are the second draw and actions.
 
         state.stand_pat_or_discard('??')  # Bob
         state.stand_pat_or_discard()  # Carol
         state.stand_pat_or_discard('??')  # Alice
         state.burn_card('??')
         state.deal_hole('??')  # Bob
         state.deal_hole('??')  # Alice
 
         state.check_or_call()  # Bob
         state.complete_bet_or_raise_to()  # Carol
         state.complete_bet_or_raise_to()  # Alice
         state.fold()  # Bob
         state.check_or_call()  # Carol
 
-        # Below shows the third draw and actions.
+        # Below are the third draw and actions.
 
         state.stand_pat_or_discard('??')  # Carol
         state.stand_pat_or_discard()  # Alice
         state.burn_card('??')
         state.deal_hole('??')  # Carol
 
         state.check_or_call()  # Carol
         state.complete_bet_or_raise_to()  # Alice
         state.check_or_call()  # Carol
 
-        # Below show the showdown.
+        # Below is the showdown.
 
         state.show_or_muck_hole_cards('2s4c6d9h')  # Alice
         state.show_or_muck_hole_cards('3s5d7c8h')  # Carol
 
-        # Below show the final stacks.
+        # Below are the final stacks.
 
         # print(state.stacks)  # [196, 220, 200, 184]
 
         self.assertEqual(state.stacks, [196, 220, 200, 184])
 
 
 if __name__ == '__main__':
```

### Comparing `pokerkit-0.4.9/pokerkit/tests/test_utilities.py` & `pokerkit-0.5.0a0/pokerkit/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `pokerkit-0.4.9/pokerkit/tests/test_wsop/test_2023_43.py` & `pokerkit-0.5.0a0/pokerkit/tests/test_wsop/test_2023_43_5.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """:mod:`pokerkit.tests.test_wsop.test_2023_43` implements unit tests
-for :mod:`pokerkit.state` with hands played on 2023 World Series of
-Poker Event #43: $50000 Poker Players Championship.
+for :mod:`pokerkit.state` with hands played on the Day 5 of the 2023
+World Series of Poker Event #43: $50,000 Poker Players Championship.
 
 https://www.pokergo.com/videos/6e5e4f34-9857-458c-b61e-d478ad29dbd6
 
 Game order (in WSOP notations):
 - No-limit hold'em
 - Seven card stud
 - Omaha 8-or-better
```

### Comparing `pokerkit-0.4.9/pokerkit/utilities.py` & `pokerkit-0.5.0a0/pokerkit/utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from enum import Enum, StrEnum, unique
 from functools import partial
 from itertools import product, starmap
 from numbers import Integral
 from operator import is_not
 from random import shuffle
 from typing import Any, cast, TypeVar
+import builtins
 
 _T = TypeVar('_T')
 
 
 @unique
 class Rank(StrEnum):
     """The enum class for ranks.
@@ -339,46 +340,46 @@
         >>> Card.clean('AsKs')
         (As, Ks)
         >>> Card.clean(Card(Rank.ACE, Suit.SPADE))
         (As,)
         >>> Card.clean(None)
         Traceback (most recent call last):
             ...
-        ValueError: invalid values
+        ValueError: The card values None are invalid.
 
         :param values: The cards.
         :return: The cleaned cards.
         """
         if isinstance(values, Card):
             values = (values,)
         elif isinstance(values, str):
             values = tuple(Card.parse(values))
         elif isinstance(values, Iterable):
             assert not isinstance(values, str)
 
             values = tuple(values)
         else:
-            raise ValueError('invalid values')
+            raise ValueError(f'The card values {repr(values)} are invalid.')
 
         return values
 
     @classmethod
     def parse(cls, *raw_cards: str) -> Iterator[Card]:
         """Parse the string of the card representations.
 
         >>> Card.parse('AsKsQsJsTs')  # doctest: +ELLIPSIS
         <generator object Card.parse at 0x...>
         >>> list(Card.parse('2c8d5sKh'))
         [2c, 8d, 5s, Kh]
         >>> next(Card.parse('AcAh'))
         Ac
-        >>> next(Card.parse('AcA'))
+        >>> next(Card.parse('AcA'))  # doctest: +ELLIPSIS
         Traceback (most recent call last):
             ...
-        ValueError: content length not a multiple of 2
+        ValueError: The lengths of valid card representations must be multip...
         >>> next(Card.parse('1d'))
         Traceback (most recent call last):
             ...
         ValueError: '1' is not a valid Rank
         >>> next(Card.parse('Ax'))
         Traceback (most recent call last):
             ...
@@ -387,15 +388,20 @@
         :param raw_cards: The string of the card representations.
         :return: The generator yielding the parsed cards.
         :raises ValueError: If any card representation is invalid.
         """
         for contents in raw_cards:
             for content in contents.split():
                 if len(content) % 2 != 0:
-                    raise ValueError('content length not a multiple of 2')
+                    raise ValueError(
+                        (
+                            'The lengths of valid card representations must be'
+                            f' multiples of 2, unlike {repr(content)}'
+                        ),
+                    )
 
                 for i in range(0, len(content), 2):
                     rank = Rank(content[i])
                     suit = Suit(content[i + 1])
 
                     yield cls(rank, suit)
 
@@ -578,15 +584,15 @@
     >>> clean_values(4, 4)
     (4, 4, 4, 4)
     >>> clean_values((1, 2, 3), 2)
     (1, 2)
     >>> clean_values(None, 2)
     Traceback (most recent call last):
         ...
-    ValueError: invalid values
+    ValueError: The values None are invalid.
 
     :param values: The values.
     :param count: The number of values.
     :return: The cleaned integers.
     """
     if isinstance(values, int | float):
         values = (values,) * count
@@ -601,15 +607,15 @@
         parsed_values = list(values)[:count]
 
         while len(parsed_values) < count:
             parsed_values.append(0)
 
         values = tuple(parsed_values)
     else:
-        raise ValueError('invalid values')
+        raise ValueError(f'The values {repr(values)} are invalid.')
 
     return values
 
 
 def shuffled(values: Iterable[_T]) -> list[_T]:
     """Return the shuffled values.
 
@@ -625,31 +631,28 @@
     values = list(values)
 
     shuffle(values)
 
     return values
 
 
-_divmod = divmod
-
-
 def divmod(dividend: int, divisor: int) -> tuple[int, int]:
     """Divide the amount.
 
     >>> divmod(11, 3)
     (3, 2)
     >>> divmod(11.0, 3)  # doctest: +ELLIPSIS
     (3.666666666666666..., 0.0)
 
     :param dividend: The pot amount.
     :param divisor: The number of players.
     :return: The quotient and the remainder.
     """
     if isinstance(dividend, Integral):
-        return _divmod(dividend, divisor)
+        return builtins.divmod(dividend, divisor)
 
     quotient = dividend / divisor
     remainder = dividend - quotient * divisor
 
     return cast(tuple[int, int], (quotient, remainder))
```

### Comparing `pokerkit-0.4.9/pokerkit.egg-info/PKG-INFO` & `pokerkit-0.5.0a0/pokerkit.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pokerkit
-Version: 0.4.9
-Summary: An open-source Python library for poker simulations and hand evaluations
+Version: 0.5.0a0
+Summary: An open-source Python library for poker game simulations, hand evaluations, and statistical analysis
 Home-page: https://github.com/uoftcprg/pokerkit
-Author: University of Toronto Computer Poker Research Group
+Author: University of Toronto Computer Poker Student Research Group
 Author-email: uoftcprg@studentorg.utoronto.ca
 License: MIT
 Project-URL: Documentation, https://pokerkit.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/uoftcprg/pokerkit
 Project-URL: Tracker, https://github.com/uoftcprg/pokerkit/issues
 Keywords: artificial-intelligence,deep-learning,game,game-development,game-theory,holdem-poker,imperfect-information-game,libratus,pluribus,poker,poker-engine,poker-evaluator,poker-game,poker-hands,poker-library,poker-strategies,python,reinforcement-learning,texas-holdem
 Classifier: Development Status :: 5 - Production/Stable
@@ -30,42 +30,159 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ========
 PokerKit
 ========
 
-PokerKit is an open-source Python library for simulating poker games and evaluating poker hands, developed by the University of Toronto Computer Poker Research Group. PokerKit supports an extensive array of poker variants and it provides a flexible architecture for users to define their custom games. These facilities are exposed via an intuitive unified high-level programmatic API. The library can be used in a variety of use cases, from poker AI development, and tool creation, to online poker casino implementation. PokerKit's reliability has been established through static type checking, extensive doctests, and unit tests, achieving 99% code coverage.
+PokerKit is an open-source software library, written in pure Python, for simulating games, evaluating hands, and facilitating statistical analysis, developed by the University of Toronto Computer Poker Student Research Group. PokerKit supports an extensive array of poker variants and it provides a flexible architecture for users to define their custom games. These facilities are exposed via an intuitive unified high-level programmatic API. The library can be used in a variety of use cases, from poker AI development, and tool creation, to online poker casino implementation. PokerKit's reliability has been established through static type checking, extensive doctests, and unit tests, achieving 99% code coverage.
 
 Features
 --------
 
 * Extensive poker game logic for major and minor poker variants.
 * High-speed hand evaluations.
 * Customizable game states and parameters.
 * Robust implementation with static type checking and extensive unit tests and doctests.
-* Dataset of over 10,000 hand histories.
 
 Installation
 ------------
 
 The PokerKit library can be installed using pip:
 
 .. code-block:: bash
 
    pip install pokerkit
 
 Usages
 ------
 
-**The first televised million-dollar pot between Tom Dwan and Phil Ivey.**
+Example usages of PokerKit is shown below.
 
-Link: https://youtu.be/GnxFohpljqM
+Multi-Runout in an All-In Situation
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+Below shows the 4-runout hand between Phil Hellmuth and the Loose Cannon Ernest Wiggins.
+
+Link: https://youtu.be/cnjJv7x0HMY?si=4l05Ez7lQVczt8DI&t=638
+
+.. code-block:: python
+
+   from pokerkit import Automation, Mode, NoLimitTexasHoldem
+
+   state = NoLimitTexasHoldem.create_state(
+       # Automations
+       (
+           Automation.ANTE_POSTING,
+           Automation.BET_COLLECTION,
+           Automation.BLIND_OR_STRADDLE_POSTING,
+           Automation.HOLE_CARDS_SHOWING_OR_MUCKING,
+           Automation.HAND_KILLING,
+           Automation.CHIPS_PUSHING,
+           Automation.CHIPS_PULLING,
+       ),
+       False,  # Uniform antes?
+       {-1: 600},  # Antes
+       (200, 400, 800),  # Blinds or straddles
+       400,  # Min-bet
+       (999999, 116400, 86900, 999999, 50000, 999999),  # Starting stacks
+       6,  # Number of players
+       mode=Mode.CASH_GAME,
+   )
+
+Below are the pre-flop dealings and actions.
+
+.. code-block:: python
+
+   state.deal_hole('JsTh')  # Tony G
+   state.deal_hole('Ah9d')  # Hellmuth
+   state.deal_hole('KsKc')  # Wiggins
+   state.deal_hole('5c2h')  # Negreanu
+   state.deal_hole('6h5h')  # Brunson
+   state.deal_hole('6s3s')  # Laak
+
+   state.fold()  # Negreanu
+   state.complete_bet_or_raise_to(2800)  # Brunson
+   state.fold()  # Laak
+   state.check_or_call()  # Tony G
+   state.complete_bet_or_raise_to(12600)  # Hellmuth
+   state.check_or_call()  # Wiggins
+   state.check_or_call()  # Brunson
+   state.check_or_call()  # Tony G
+
+Below are the flop dealing and actions.
+
+.. code-block:: python
+
+   state.burn_card('??')
+   state.deal_board('9hTs9s')
+
+   state.check_or_call()  # Tony G
+   state.complete_bet_or_raise_to(17000)  # Hellmuth
+   state.complete_bet_or_raise_to(36000)  # Wiggins
+   state.fold()  # Brunson
+   state.fold()  # Tony G
+   state.complete_bet_or_raise_to(103800)  # Hellmuth
+   state.check_or_call()  # Wiggins
+
+Below is selecting the number of runouts.
+
+.. code-block:: python
+
+   state.select_runout_count(4)  # Hellmuth
+   state.select_runout_count(None)  # Wiggins
 
-Set up the game.
+Below is the first runout.
+
+.. code-block:: python
+
+   state.burn_card('??')
+   state.deal_board('Jh')  # Turn
+   state.burn_card('??')
+   state.deal_board('Ad')  # River
+
+Below is the second runout.
+
+.. code-block:: python
+
+   state.burn_card('??')
+   state.deal_board('Kh')  # Turn
+   state.burn_card('??')
+   state.deal_board('3c')  # River
+
+Below is the third runout.
+
+.. code-block:: python
+
+   state.burn_card('??')
+   state.deal_board('7s')  # Turn
+   state.burn_card('??')
+   state.deal_board('8s')  # River
+
+Below is the fourth runout.
+
+.. code-block:: python
+
+   state.burn_card('??')
+   state.deal_board('Qc')  # Turn
+   state.burn_card('??')
+   state.deal_board('Kd')  # River
+
+Below are the final stacks.
+
+.. code-block:: python
+
+   print(state.stacks)  # [987399, 79400, 149700, 999999, 37400, 999399]
+
+A Sample No-Limit Texas Hold'em Hand
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+Below shows the first televised million-dollar pot between Tom Dwan and Phil Ivey.
+
+Link: https://youtu.be/GnxFohpljqM
 
 .. code-block:: python
 
    from pokerkit import Automation, NoLimitTexasHoldem
 
    state = NoLimitTexasHoldem.create_state(
        # Automations
@@ -130,15 +247,18 @@
 
 Below are the final stacks.
 
 .. code-block:: python
 
    print(state.stacks)  # [572100, 1997500, 1109500]
 
-**An all-in hand between Xuan and Phua.**
+A Sample Short-Deck Hold'em Hand
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+Below shows an all-in hand between Xuan and Phua.
 
 Link: https://youtu.be/QlgCcphLjaQ
 
 .. code-block:: python
 
    from pokerkit import Automation, NoLimitShortDeckHoldem
 
@@ -205,16 +325,18 @@
 
 Below are the final stacks.
 
 .. code-block:: python
 
    print(state.stacks)  # [489000, 226000, 684000, 400000, 0, 198000]
 
-**The largest online poker pot ever played between Patrik Antonius and Viktor
-Blom.**
+A Sample Pot-Limit Omaha Hold'em Hand
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+Below shows the largest online poker pot ever played between Patrik Antonius and Viktor Blom.
 
 Link: https://youtu.be/UMBm66Id2AA
 
 .. code-block:: python
 
    from pokerkit import Automation, PotLimitOmahaHoldem
 
@@ -278,15 +400,18 @@
 
 Below are the final stacks.
 
 .. code-block:: python
 
    print(state.stacks)  # [1937923.75, 0.0]
 
-**A bad beat between Yockey and Arieh.**
+A Sample Fixed-Limit Deuce-To-Seven Lowball Triple Draw Hand
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+Below shows a bad beat between Yockey and Arieh.
 
 Link: https://youtu.be/pChCqb2FNxY
 
 .. code-block:: python
 
    from pokerkit import Automation, FixedLimitDeuceToSevenLowballTripleDraw
 
@@ -363,15 +488,18 @@
 
 Below are the final stacks.
 
 .. code-block:: python
 
    print(state.stacks)  # [0, 4190000, 5910000, 12095000]
 
-**An example badugi hand from Wikipedia.**
+A Sample Badugi Hand
+^^^^^^^^^^^^^^^^^^^^
+
+Below shows an example badugi hand from Wikipedia.
 
 Link: https://en.wikipedia.org/wiki/Badugi
 
 .. code-block:: python
 
    from pokerkit import Automation, FixedLimitBadugi
 
@@ -467,15 +595,15 @@
 .. code-block:: python
 
    print(state.stacks)  # [196, 220, 200, 184]
 
 Testing and Validation
 ----------------------
 
-PokerKit has extensive test coverage, passes mypy static type checking with strict parameter, and has been validated through extensive use in real-life scenarios.
+PokerKit has extensive test coverage, passes mypy static type checking with strict mode, and has been validated through extensive use in real-life scenarios.
 
 Contributing
 ------------
 
 Contributions are welcome! Please read our Contributing Guide for more information.
 
 License
```

### Comparing `pokerkit-0.4.9/pokerkit.egg-info/SOURCES.txt` & `pokerkit-0.5.0a0/pokerkit.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 LICENSE
 README.rst
 setup.py
 pokerkit/__init__.py
+pokerkit/analysis.py
 pokerkit/games.py
 pokerkit/hands.py
 pokerkit/lookups.py
 pokerkit/notation.py
 pokerkit/py.typed
 pokerkit/state.py
 pokerkit/utilities.py
 pokerkit.egg-info/PKG-INFO
 pokerkit.egg-info/SOURCES.txt
 pokerkit.egg-info/dependency_links.txt
 pokerkit.egg-info/top_level.txt
 pokerkit/tests/__init__.py
+pokerkit/tests/test_analysis.py
+pokerkit/tests/test_games.py
 pokerkit/tests/test_lookups.py
+pokerkit/tests/test_notation.py
 pokerkit/tests/test_papers.py
 pokerkit/tests/test_state.py
 pokerkit/tests/test_utilities.py
 pokerkit/tests/test_wsop/__init__.py
-pokerkit/tests/test_wsop/test_2023_43.py
+pokerkit/tests/test_wsop/test_2023_43_5.py
+pokerkit/tests/test_wsop/test_2023_54_4.py
```

### Comparing `pokerkit-0.4.9/setup.py` & `pokerkit-0.5.0a0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!/usr/bin/env python3
 
 from setuptools import find_packages, setup
 
 setup(
     name='pokerkit',
-    version='0.4.9',
-    description='An open-source Python library for poker simulations and hand evaluations',
+    version='0.5.0a0',
+    description='An open-source Python library for poker game simulations, hand evaluations, and statistical analysis',
     long_description=open('README.rst').read(),
     long_description_content_type='text/x-rst',
     url='https://github.com/uoftcprg/pokerkit',
-    author='University of Toronto Computer Poker Research Group',
+    author='University of Toronto Computer Poker Student Research Group',
     author_email='uoftcprg@studentorg.utoronto.ca',
     license='MIT',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: Education',
         'Topic :: Education',
```

