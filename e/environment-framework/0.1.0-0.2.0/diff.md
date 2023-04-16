# Comparing `tmp/environment_framework-0.1.0.tar.gz` & `tmp/environment_framework-0.2.0.tar.gz`

## Comparing `environment_framework-0.1.0.tar` & `environment_framework-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0     4520 2020-02-02 00:00:00.000000 environment_framework-0.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 environment_framework-0.1.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 environment_framework-0.1.0/makefile
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 environment_framework-0.1.0/mypy.ini
--rw-r--r--   0        0        0    18086 2020-02-02 00:00:00.000000 environment_framework-0.1.0/pylintrc
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 environment_framework-0.1.0/pytest.ini
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 environment_framework-0.1.0/version.py
--rw-r--r--   0        0        0    12834 2020-02-02 00:00:00.000000 environment_framework-0.1.0/example/grid_world.ipynb
--rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 environment_framework-0.1.0/example/grid_world.py
--rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 environment_framework-0.1.0/requirements/dev.txt
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 environment_framework-0.1.0/requirements/main.txt
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 environment_framework-0.1.0/src/environment_framework/__init__.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 environment_framework-0.1.0/src/environment_framework/estimator.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 environment_framework-0.1.0/src/environment_framework/game.py
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 environment_framework-0.1.0/src/environment_framework/gym.py
--rw-r--r--   0        0        0     5540 2020-02-02 00:00:00.000000 environment_framework-0.1.0/src/environment_framework/level.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 environment_framework-0.1.0/src/environment_framework/observer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 environment_framework-0.1.0/src/environment_framework/py.typed
--rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 environment_framework-0.1.0/src/environment_framework/simulator.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 environment_framework-0.1.0/src/environment_framework/visualizer.py
--rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 environment_framework-0.1.0/tests/test_gym.py
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 environment_framework-0.1.0/tests/test_level.py
--rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 environment_framework-0.1.0/tests/test_simulator.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 environment_framework-0.1.0/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 environment_framework-0.1.0/LICENSE
--rw-r--r--   0        0        0     6579 2020-02-02 00:00:00.000000 environment_framework-0.1.0/README.md
--rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 environment_framework-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     8219 2020-02-02 00:00:00.000000 environment_framework-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     4520 2020-02-02 00:00:00.000000 environment_framework-0.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 environment_framework-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 environment_framework-0.2.0/makefile
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 environment_framework-0.2.0/mypy.ini
+-rw-r--r--   0        0        0    18086 2020-02-02 00:00:00.000000 environment_framework-0.2.0/pylintrc
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 environment_framework-0.2.0/pytest.ini
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 environment_framework-0.2.0/version.py
+-rw-r--r--   0        0        0    10847 2020-02-02 00:00:00.000000 environment_framework-0.2.0/example/grid_world.ipynb
+-rw-r--r--   0        0        0     6267 2020-02-02 00:00:00.000000 environment_framework-0.2.0/example/grid_world.py
+-rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 environment_framework-0.2.0/requirements/dev.txt
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 environment_framework-0.2.0/requirements/main.txt
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 environment_framework-0.2.0/src/environment_framework/__init__.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 environment_framework-0.2.0/src/environment_framework/estimator.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 environment_framework-0.2.0/src/environment_framework/game.py
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 environment_framework-0.2.0/src/environment_framework/gym.py
+-rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 environment_framework-0.2.0/src/environment_framework/ilevel.py
+-rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 environment_framework-0.2.0/src/environment_framework/level.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 environment_framework-0.2.0/src/environment_framework/observer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 environment_framework-0.2.0/src/environment_framework/py.typed
+-rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 environment_framework-0.2.0/src/environment_framework/simulator.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 environment_framework-0.2.0/src/environment_framework/visualizer.py
+-rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 environment_framework-0.2.0/tests/test_gym.py
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 environment_framework-0.2.0/tests/test_level.py
+-rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 environment_framework-0.2.0/tests/test_simulator.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 environment_framework-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 environment_framework-0.2.0/LICENSE
+-rw-r--r--   0        0        0     6304 2020-02-02 00:00:00.000000 environment_framework-0.2.0/README.md
+-rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 environment_framework-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7944 2020-02-02 00:00:00.000000 environment_framework-0.2.0/PKG-INFO
```

### Comparing `environment_framework-0.1.0/CODE_OF_CONDUCT.md` & `environment_framework-0.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `environment_framework-0.1.0/CONTRIBUTING.md` & `environment_framework-0.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `environment_framework-0.1.0/makefile` & `environment_framework-0.2.0/makefile`

 * *Files identical despite different names*

### Comparing `environment_framework-0.1.0/pylintrc` & `environment_framework-0.2.0/pylintrc`

 * *Files identical despite different names*

### Comparing `environment_framework-0.1.0/example/grid_world.ipynb` & `environment_framework-0.2.0/example/grid_world.ipynb`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9847494948717774%*

 * *Differences: {"'cells'": "{1: {'execution_count': None, 'source': {insert: [(7, 'from numpy.typing import "*

 * *            "NDArray\\n'), (8, 'from gymnasium.spaces import Space, Discrete\\n'), (13, 'from "*

 * *            "gymnasium.spaces import Space, Box\\n'), (14, 'import math\\n'), (15, 'import numpy "*

 * *            "as np\\n'), (16, '\\n'), (17, 'from environment_framework import Level\\n'), (18, "*

 * *            "'from environment_framework import EnvironmentFrameworkGym\\n'), (19, 'from "*

 * *            "environment_framework […]*

```diff
@@ -8,51 +8,57 @@
                 "# Grid World example\n",
                 "\n",
                 "In this notebook we implement the GridWorld game with the `environment-framework` and use stable-baseliens3 to train a `DQN`-agent on it."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": null,
             "id": "34ec77d0-740e-4fda-b709-1a237ff49e43",
             "metadata": {
                 "lines_to_next_cell": 2,
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "from enum import Enum\n",
                 "from random import randint\n",
                 "from typing import Any, List, Tuple\n",
                 "\n",
                 "from stable_baselines3.common.evaluation import evaluate_policy\n",
                 "from stable_baselines3.dqn import DQN\n",
                 "\n",
+                "from numpy.typing import NDArray\n",
+                "from gymnasium.spaces import Space, Discrete\n",
                 "\n",
                 "import cv2\n",
                 "import numpy as np\n",
                 "\n",
-                "from environment_framework.level import ActionSpace, Level, ObservationSpace\n",
-                "from environment_framework.gym import SimulatorFrameworkGym\n",
-                "from environment_framework.simulator import Simulator"
+                "from gymnasium.spaces import Space, Box\n",
+                "import math\n",
+                "import numpy as np\n",
+                "\n",
+                "from environment_framework import Level\n",
+                "from environment_framework import EnvironmentFrameworkGym\n",
+                "from environment_framework import Simulator"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "206b9f02-7f3c-4861-bf6d-81dd4652381e",
             "metadata": {
                 "lines_to_next_cell": 2
             },
             "source": [
                 "## Implement the `Game`"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": null,
             "id": "42cf31a4-d776-41e9-adbb-44fe9056d083",
             "metadata": {
                 "lines_to_next_cell": 2,
                 "tags": []
             },
             "outputs": [],
             "source": [
@@ -69,14 +75,19 @@
                 "        self.player_position = (0, 0)\n",
                 "        self.target_position = (0, 0)\n",
                 "        self.reset()\n",
                 "\n",
                 "    @property\n",
                 "    def done(self) -> bool:\n",
                 "        return self.player_position == self.target_position\n",
+                "    \n",
+                "    @property\n",
+                "    def space(self) -> Space:\n",
+                "        return Discrete(4)\n",
+                "        \n",
                 "\n",
                 "    def act(self, action: Action, **_: Any) -> None:\n",
                 "        if action == Action.UP:\n",
                 "            self.player_position = (self.player_position[0], self.player_position[1] - 1)\n",
                 "        if action == Action.DOWN:\n",
                 "            self.player_position = (self.player_position[0], self.player_position[1] + 1)\n",
                 "        if action == Action.RIGHT:\n",
@@ -105,32 +116,32 @@
             },
             "source": [
                 "## Implement the `Observer` and the `Estimator`"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": null,
             "id": "e4109d2c-3202-4499-8e2e-0c58e4456f30",
             "metadata": {
                 "lines_to_next_cell": 2,
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "class GridWorldObserver:\n",
                 "    def __init__(self, game: GridWorldGame) -> None:\n",
                 "        self.game = game\n",
                 "\n",
                 "    @property\n",
-                "    def shape(self) -> Tuple[int, ...]:\n",
-                "        return (4,)\n",
+                "    def space(self) -> Space:\n",
+                "        return Box(shape=(4,), low=-math.inf, high=math.inf)\n",
                 "\n",
-                "    def observe(self, _: Any) -> List[float]:\n",
-                "        return [*self.game.player_position, *self.game.target_position]\n",
+                "    def observe(self, _: Any) -> NDArray:\n",
+                "        return np.array([*self.game.player_position, *self.game.target_position])\n",
                 "\n",
                 "\n",
                 "class GridWorldEstimator:\n",
                 "    def __init__(self, game: GridWorldGame) -> None:\n",
                 "        self.game = game\n",
                 "\n",
                 "    def estimate(self, _: Any) -> float:\n",
@@ -146,15 +157,15 @@
             },
             "source": [
                 "## Add a nice little `Visualizer`"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": null,
             "id": "b8855c93-3335-4475-80aa-3e3a64ae5300",
             "metadata": {
                 "lines_to_next_cell": 2,
                 "tags": []
             },
             "outputs": [],
             "source": [
@@ -181,15 +192,15 @@
             },
             "source": [
                 "## Connect all together with a `Level`"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": null,
             "id": "18451c66-de76-411a-adff-51a2b23c5c30",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "class GridWorldLevel(Level):\n",
@@ -209,52 +220,38 @@
                 "\n",
                 "    def reset(self) -> None:\n",
                 "        self._game.reset()\n",
                 "\n",
                 "    def step(self, action: Action) -> Any:\n",
                 "        if isinstance(action, np.int64):  # handle integer inputs\n",
                 "            action = Action(action)\n",
-                "        self._game.act(action)\n",
-                "\n",
-                "    @property\n",
-                "    def action_space(self) -> ActionSpace:\n",
-                "        return ActionSpace(\"discrete\", 4)\n",
-                "\n",
-                "    @property\n",
-                "    def observation_space(self) -> ObservationSpace:\n",
-                "        return ObservationSpace(\"discrete\", (4,))\n",
-                "\n",
-                "\n",
-                "class GridWorldSimulation:\n",
-                "    def __init__(self, level: GridWorldLevel) -> None:\n",
-                "        self.level = level\n",
-                "        self.level_settings = None"
+                "        self._game.act(action)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "370e3268-a7b6-4e51-9f03-ece9dec0acc3",
             "metadata": {},
             "source": [
                 "## Look at a random selecting agent"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": null,
             "id": "89f7c5dc-de16-4dd1-bb63-8b30a349ca02",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "game = GridWorldGame(7)\n",
-                "scale_factor = 10\n",
+                "scale_factor = 50\n",
                 "level = GridWorldLevel(game, GridWorldObserver(game), GridWorldEstimator(game), GridWorldVisualizer(game))\n",
-                "simulator = Simulator(GridWorldSimulation(level))\n",
+                "simulator = Simulator(level)\n",
                 "while not simulator.done:\n",
                 "    action = Action(randint(0, 3))\n",
                 "    simulator.step(action)\n",
                 "    frame = np.array(simulator.render(), dtype=np.uint8)\n",
                 "    frame = cv2.resize(frame, (scale_factor * game.size, scale_factor * game.size), interpolation=cv2.INTER_AREA)\n",
                 "    cv2.imshow(\"GridWorld\", frame)\n",
                 "    cv2.waitKey(33)\n",
@@ -268,134 +265,65 @@
             "metadata": {},
             "source": [
                 "## Use stable-baselines3 to train an DQN-agent in the environment"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": null,
             "id": "3392de7b-d58b-47ae-94e6-5bad09bdfc39",
             "metadata": {
                 "tags": []
             },
-            "outputs": [
-                {
-                    "data": {
-                        "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "596fccf4fae34c518d6c6381dfcf0ffe",
-                            "version_major": 2,
-                            "version_minor": 0
-                        },
-                        "text/plain": [
-                            "Output()"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
-                },
-                {
-                    "data": {
-                        "text/html": [
-                            "<pre style=\"white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,'DejaVu Sans Mono',consolas,'Courier New',monospace\"></pre>\n"
-                        ],
-                        "text/plain": []
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
-                },
-                {
-                    "data": {
-                        "text/html": [
-                            "<pre style=\"white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,'DejaVu Sans Mono',consolas,'Courier New',monospace\">\n",
-                            "</pre>\n"
-                        ],
-                        "text/plain": [
-                            "\n"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
-                },
-                {
-                    "data": {
-                        "text/plain": [
-                            "<stable_baselines3.dqn.dqn.DQN at 0x7fe8852df430>"
-                        ]
-                    },
-                    "execution_count": 7,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
+            "outputs": [],
             "source": [
                 "game = GridWorldGame(7)\n",
                 "level = GridWorldLevel(game, GridWorldObserver(game), GridWorldEstimator(game), GridWorldVisualizer(game))\n",
-                "simulator = Simulator(GridWorldSimulation(level))\n",
-                "env = SimulatorFrameworkGym(GridWorldSimulation(level), render_mode=\"rgb_array\")\n",
+                "env = EnvironmentFrameworkGym(level, render_mode=\"rgb_array\")\n",
                 "\n",
                 "model = DQN(\"MlpPolicy\", env)\n",
                 "model.learn(\n",
-                "    total_timesteps=int(2.5e5),\n",
+                "    total_timesteps=int(5e5),\n",
                 "    progress_bar=True,\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": null,
             "id": "bd172f4e-7492-4860-9a42-ada5056eb064",
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "/home/rb/git/simulator-framework/venv/lib/python3.10/site-packages/stable_baselines3/common/evaluation.py:67: UserWarning: Evaluation environment is not wrapped with a ``Monitor`` wrapper. This may result in reporting modified episode lengths and rewards, if other wrappers happen to modify these. Consider wrapping environment first with ``Monitor`` wrapper.\n",
-                        "  warnings.warn(\n"
-                    ]
-                },
-                {
-                    "data": {
-                        "text/plain": [
-                            "(-3.9, 2.6248809496813372)"
-                        ]
-                    },
-                    "execution_count": 8,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
+            "outputs": [],
             "source": [
                 "evaluate_policy(model, env, n_eval_episodes=10)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": null,
             "id": "34db8e65-7046-49f0-b6c4-cdf3b18d2289",
             "metadata": {},
             "outputs": [],
             "source": [
                 "model.save(\"gridworld-dqn.zip\")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": null,
             "id": "ca143958-07db-4562-a43a-72f442a5d2b2",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "game = GridWorldGame(7)\n",
-                "scale_factor = 20\n",
+                "scale_factor = 50\n",
                 "level = GridWorldLevel(game, GridWorldObserver(game), GridWorldEstimator(game), GridWorldVisualizer(game))\n",
-                "simulator = Simulator(GridWorldSimulation(level))\n",
-                "env = SimulatorFrameworkGym(GridWorldSimulation(level), render_mode=\"rgb_array\")\n",
+                "env = EnvironmentFrameworkGym(level, render_mode=\"rgb_array\")\n",
                 "\n",
                 "model = DQN.load(\"gridworld-dqn.zip\", env=env)\n",
                 "vec_env = model.get_env()\n",
                 "obs = vec_env.reset()\n",
                 "for _ in range(50):\n",
                 "    obs = np.array(obs)\n",
                 "    action, _states = model.predict(obs)  # type: ignore\n",
@@ -403,14 +331,22 @@
                 "    frame = np.array(vec_env.render(), dtype=np.uint8)\n",
                 "    frame = cv2.resize(frame, (scale_factor * game.size, scale_factor * game.size), interpolation=cv2.INTER_AREA)\n",
                 "    cv2.imshow(\"GridWorld\", frame)\n",
                 "    cv2.waitKey(250)\n",
                 "cv2.waitKey(500)\n",
                 "cv2.destroyAllWindows()"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "07e4cc1f-cc51-4eb2-9872-aa116814209d",
+            "metadata": {},
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "jupytext": {
             "formats": "ipynb,py:hydrogen"
         },
         "kernelspec": {
```

### Comparing `environment_framework-0.1.0/example/grid_world.py` & `environment_framework-0.2.0/example/grid_world.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,21 +22,27 @@
 from enum import Enum
 from random import randint
 from typing import Any, List, Tuple
 
 from stable_baselines3.common.evaluation import evaluate_policy
 from stable_baselines3.dqn import DQN
 
+from numpy.typing import NDArray
+from gymnasium.spaces import Space, Discrete
 
 import cv2
 import numpy as np
 
-from environment_framework.level import ActionSpace, Level, ObservationSpace
-from environment_framework.gym import SimulatorFrameworkGym
-from environment_framework.simulator import Simulator
+from gymnasium.spaces import Space, Box
+import math
+import numpy as np
+
+from environment_framework import Level
+from environment_framework import EnvironmentFrameworkGym
+from environment_framework import Simulator
 
 
 # %% [markdown]
 # ## Implement the `Game`
 
 
 # %%
@@ -53,14 +59,19 @@
         self.player_position = (0, 0)
         self.target_position = (0, 0)
         self.reset()
 
     @property
     def done(self) -> bool:
         return self.player_position == self.target_position
+    
+    @property
+    def space(self) -> Space:
+        return Discrete(4)
+        
 
     def act(self, action: Action, **_: Any) -> None:
         if action == Action.UP:
             self.player_position = (self.player_position[0], self.player_position[1] - 1)
         if action == Action.DOWN:
             self.player_position = (self.player_position[0], self.player_position[1] + 1)
         if action == Action.RIGHT:
@@ -87,19 +98,19 @@
 
 # %%
 class GridWorldObserver:
     def __init__(self, game: GridWorldGame) -> None:
         self.game = game
 
     @property
-    def shape(self) -> Tuple[int, ...]:
-        return (4,)
+    def space(self) -> Space:
+        return Box(shape=(4,), low=-math.inf, high=math.inf)
 
-    def observe(self, _: Any) -> List[float]:
-        return [*self.game.player_position, *self.game.target_position]
+    def observe(self, _: Any) -> NDArray:
+        return np.array([*self.game.player_position, *self.game.target_position])
 
 
 class GridWorldEstimator:
     def __init__(self, game: GridWorldGame) -> None:
         self.game = game
 
     def estimate(self, _: Any) -> float:
@@ -150,37 +161,23 @@
         self._game.reset()
 
     def step(self, action: Action) -> Any:
         if isinstance(action, np.int64):  # handle integer inputs
             action = Action(action)
         self._game.act(action)
 
-    @property
-    def action_space(self) -> ActionSpace:
-        return ActionSpace("discrete", 4)
-
-    @property
-    def observation_space(self) -> ObservationSpace:
-        return ObservationSpace("discrete", (4,))
-
-
-class GridWorldSimulation:
-    def __init__(self, level: GridWorldLevel) -> None:
-        self.level = level
-        self.level_settings = None
-
 
 # %% [markdown]
 # ## Look at a random selecting agent
 
 # %%
 game = GridWorldGame(7)
-scale_factor = 10
+scale_factor = 50
 level = GridWorldLevel(game, GridWorldObserver(game), GridWorldEstimator(game), GridWorldVisualizer(game))
-simulator = Simulator(GridWorldSimulation(level))
+simulator = Simulator(level)
 while not simulator.done:
     action = Action(randint(0, 3))
     simulator.step(action)
     frame = np.array(simulator.render(), dtype=np.uint8)
     frame = cv2.resize(frame, (scale_factor * game.size, scale_factor * game.size), interpolation=cv2.INTER_AREA)
     cv2.imshow("GridWorld", frame)
     cv2.waitKey(33)
@@ -189,42 +186,42 @@
 
 # %% [markdown]
 # ## Use stable-baselines3 to train an DQN-agent in the environment
 
 # %%
 game = GridWorldGame(7)
 level = GridWorldLevel(game, GridWorldObserver(game), GridWorldEstimator(game), GridWorldVisualizer(game))
-simulator = Simulator(GridWorldSimulation(level))
-env = SimulatorFrameworkGym(GridWorldSimulation(level), render_mode="rgb_array")
+env = EnvironmentFrameworkGym(level, render_mode="rgb_array")
 
 model = DQN("MlpPolicy", env)
 model.learn(
-    total_timesteps=int(2.5e5),
+    total_timesteps=int(5e5),
     progress_bar=True,
 )
 
 # %%
 evaluate_policy(model, env, n_eval_episodes=10)
 
 # %%
 model.save("gridworld-dqn.zip")
 
 # %%
 game = GridWorldGame(7)
-scale_factor = 20
+scale_factor = 50
 level = GridWorldLevel(game, GridWorldObserver(game), GridWorldEstimator(game), GridWorldVisualizer(game))
-simulator = Simulator(GridWorldSimulation(level))
-env = SimulatorFrameworkGym(GridWorldSimulation(level), render_mode="rgb_array")
+env = EnvironmentFrameworkGym(level, render_mode="rgb_array")
 
 model = DQN.load("gridworld-dqn.zip", env=env)
 vec_env = model.get_env()
 obs = vec_env.reset()
 for _ in range(50):
     obs = np.array(obs)
     action, _states = model.predict(obs)  # type: ignore
     obs, _, _, _ = vec_env.step(action)
     frame = np.array(vec_env.render(), dtype=np.uint8)
     frame = cv2.resize(frame, (scale_factor * game.size, scale_factor * game.size), interpolation=cv2.INTER_AREA)
     cv2.imshow("GridWorld", frame)
     cv2.waitKey(250)
 cv2.waitKey(500)
 cv2.destroyAllWindows()
+
+# %%
```

### Comparing `environment_framework-0.1.0/requirements/dev.txt` & `environment_framework-0.2.0/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `environment_framework-0.1.0/requirements/main.txt` & `environment_framework-0.2.0/requirements/main.txt`

 * *Files identical despite different names*

### Comparing `environment_framework-0.1.0/src/environment_framework/game.py` & `environment_framework-0.2.0/src/environment_framework/game.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 from typing import Any, Protocol
 
+from gymnasium.spaces import Space
+
 
 class Game(Protocol):
     @property
     def done(self) -> bool:
         """
         Indicates if the game has is done/finished.
         Sould be set if the end state is reached.
 
         Returns
         -------
         done : bool
             Game has reached its end state.
         """
 
+    @property
+    def space(self) -> Space:
+        pass
+
     def act(self, action: Any, **kwargs: Any) -> None:
         """
         Implements the logic for a step in the game.
 
         Parameters
         ----------
         action : Any
```

### Comparing `environment_framework-0.1.0/src/environment_framework/gym.py` & `environment_framework-0.2.0/src/environment_framework/gym.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,31 @@
-import math
 from typing import Any, Dict, List, Optional, Tuple
 
 import gymnasium as gym
 
-from environment_framework.simulator import Simulation, Simulator
+from environment_framework.ilevel import ILevel
+from environment_framework.simulator import Simulator
 
 
-class SimulatorFrameworkGym(gym.Env):
+class EnvironmentFrameworkGym(gym.Env):
     metadata = {"render_modes": ["rgb_array"], "render_fps": 4}
 
     def __init__(
         self,
-        simulation: Simulation,
+        level: ILevel,
         render_mode: Any = Optional[None],
     ) -> None:
         super().__init__()
 
-        self.simulator = Simulator(simulation)
+        self.simulator = Simulator(level)
 
-        self.observation_space = gym.spaces.Box(
-            low=-math.inf, high=math.inf, shape=self.simulator.observation_space.shape
-        )
-        if self.simulator.action_space.type_ == "discrete":
-            self.action_space = gym.spaces.Discrete(self.simulator.action_space.shape)
-        else:
-            raise NotImplementedError(f"Action space type: {self.simulator.action_space.type_} not implemented")
+        self.observation_space = self.simulator.observation_space
+        self.action_space = self.simulator.action_space
 
-        supported_render_modes: List[str] = SimulatorFrameworkGym.metadata["render_modes"]
+        supported_render_modes: List[str] = EnvironmentFrameworkGym.metadata["render_modes"]
         if render_mode and render_mode not in supported_render_modes:
             raise Exception("Specified unsupported render mode")
         self.render_mode = render_mode
 
         # We may take steps during the init of the game
         self.simulator.clear_counter()
```

### Comparing `environment_framework-0.1.0/src/environment_framework/level.py` & `environment_framework-0.2.0/src/environment_framework/level.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,122 +1,32 @@
 from abc import ABC, abstractmethod
-from dataclasses import dataclass
-from typing import Any, List, Protocol, Tuple
+from typing import Any
+
+from gymnasium.spaces import Space
+from numpy.typing import NDArray
 
 from environment_framework.estimator import Estimator
 from environment_framework.game import Game
 from environment_framework.observer import Observer
 from environment_framework.visualizer import Visualizer
 
 
-@dataclass
-class ObservationSpace:
-    # TODO: Add doc
-    type_: str
-    shape: Tuple[int, ...]
-
-
-@dataclass
-class ActionSpace:
-    # TODO: Add doc
-    type_: str
-    shape: int
-
-
-class ILevel(Protocol):
-    @property
-    def done(self) -> bool:
-        """
-        Returns if the game in the level has reached the end state.
-
-        Returns
-        -------
-            done: bool
-                Game has reached its end state.
-        """
-
-    @property
-    def observation_space(self) -> ObservationSpace:
-        """
-        Return the desciribtion of the observation space.
-
-        Returns
-        -------
-            observation_space: ObservationSpace
-                The observation space describtion.
-        """
-
-    @property
-    def action_space(self) -> ActionSpace:
-        """
-        Return the desciribtion of the action space.
-
-        Returns
-        -------
-            observation_space: ActionSpace
-                The action space describtion.
-        """
-
-    def reset(self) -> None:
-        """
-        Reset the level.
-        """
-
-    def step(self, action: Any) -> Any:
-        """
-        Take a step in the level with a given action.
-
-        Parameters
-        ----------
-            action: Any
-                Object which describes the action.
-        Returns
-        -------
-            state: Any
-                The step in which is the level after the action.
-        """
-
-    def observe(self) -> List[float]:
-        """
-        Observes the level and returns an observation.
-
-        Returns
-        -------
-            observation: List[float]
-                Observation of the current level state.
-        """
-
-    def estimate(self, estimated: Any) -> float:
-        """
-        Estimates the level state and returns a estimation value.
-
-        Returns
-        -------
-            estimation: float
-                Estimated reward of the current level state.
-        """
-
-    def render(self) -> Any:
-        """
-        Renders the current level state into a visualisation.
-
-        Returns
-        -------
-            visualisation: Any
-                Rendered visualisation of the current level state.
-        """
-
-
 class Level(ABC):  # pylint: disable=too-many-instance-attributes
     """
     Manages the lifecycle of a game and its observer and estimator.
     Is used within the Simulator to step through a Simulation.
     """
 
-    def __init__(self, game: Game, observer: Observer, estimator: Estimator, visualizer: Visualizer) -> None:
+    def __init__(
+        self,
+        game: Game,
+        observer: Observer,
+        estimator: Estimator,
+        visualizer: Visualizer,
+    ) -> None:
         """
         Parameters
         ----------
             game: Game
                 The game in which the level takes place.
             observer: Observer
                 The observer of the game.
@@ -139,36 +49,36 @@
         -------
             done: bool
                 Game has reached its end state.
         """
         return self._game.done
 
     @property
-    @abstractmethod
-    def observation_space(self) -> ObservationSpace:
+    def observation_space(self) -> Space:
         """
         Return the desciribtion of the observation space.
 
         Returns
         -------
             observation_space: ObservationSpace
                 The observation space describtion.
         """
+        return self._observer.space
 
     @property
-    @abstractmethod
-    def action_space(self) -> ActionSpace:
+    def action_space(self) -> Space:
         """
         Return the desciribtion of the action space.
 
         Returns
         -------
             observation_space: ActionSpace
                 The action space describtion.
         """
+        return self._game.space
 
     @abstractmethod
     def reset(self) -> None:
         """
         Reset the level.
         """
 
@@ -183,15 +93,15 @@
                 Object which describes the action.
         Returns
         -------
             state: Any
                 The step in which is the level after the action.
         """
 
-    def observe(self) -> List[float]:
+    def observe(self) -> NDArray:
         """
         Observes the level and returns an observation.
 
         Returns
         -------
             observation: List[float]
                 Observation of the current level state.
```

### Comparing `environment_framework-0.1.0/src/environment_framework/observer.py` & `environment_framework-0.2.0/src/environment_framework/observer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,27 @@
-from typing import Any, List, Protocol, Tuple
+from typing import Any, Protocol
+
+from gymnasium.spaces import Space
+from numpy.typing import NDArray
 
 
 class Observer(Protocol):
     # TODO: Add low and high poperties for the observation space
     @property
-    def shape(self) -> Tuple[int, ...]:
+    def space(self) -> Space:
         """
         The shape of the observation which is returned by observe().
 
         Returns
         -------
         shape: Tuple[int, ...]:
             The shape of the observation list.
         """
 
-    def observe(self, observed: Any) -> List[float]:
+    def observe(self, observed: Any) -> NDArray:
         """
         Returns an observation of the an observed object.
 
         Parameters
         ----------
         observed: Any
             The object which is observed.
```

### Comparing `environment_framework-0.1.0/src/environment_framework/simulator.py` & `environment_framework-0.2.0/src/environment_framework/simulator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,35 @@
-from typing import Any, List, Protocol
+from typing import Any
 
-from environment_framework.level import ActionSpace, ILevel, ObservationSpace
+from gymnasium.spaces import Space
+from numpy.typing import NDArray
 
-
-class Simulation(Protocol):
-    """
-    Describes the simulation of a Level.
-    """
-
-    level: ILevel
-    level_settings: Any
+from environment_framework.ilevel import ILevel
 
 
 class Simulator:  # pylint: disable = too-many-instance-attributes
     """
     Runs simulations on a Level.
     """
 
     # TODO: Add a proper state which is passed to the observe,estimate and render method.
     # TODO: Rename episodes to simulation.
-    def __init__(self, simulation: Simulation, max_episode_steps: int = 100000) -> None:
-        self.level = simulation.level
+    def __init__(self, level: ILevel, max_episode_steps: int = 100000) -> None:
+        self.level = level
         self._max_episode_steps = max_episode_steps
         self.current_episodes_steps_done = 0
         self.episodes_done = 0
         self.steps_done = 0
 
     @property
-    def action_space(self) -> ActionSpace:
+    def action_space(self) -> Space:
         return self.level.action_space
 
     @property
-    def observation_space(self) -> ObservationSpace:
+    def observation_space(self) -> Space:
         return self.level.observation_space
 
     @property
     def done(self) -> bool:
         """
         If the current simulation is finished.
 
@@ -76,15 +70,15 @@
             taken_action: Any
                 Returns the action taken in the Level.
         """
         self.current_episodes_steps_done += 1
         self.steps_done += 1
         return self.level.step(action)
 
-    def observe(self) -> List[float]:
+    def observe(self) -> NDArray:
         """
         Observes the level and returns an observation.
 
         Returns
         -------
             observation: List[float]
                 Observation of the current level state.
```

### Comparing `environment_framework-0.1.0/tests/test_gym.py` & `environment_framework-0.2.0/tests/test_gym.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,75 +1,80 @@
 from typing import List, Tuple
 from unittest.mock import MagicMock
 from typing import Any
 
 import numpy as np
+from numpy.typing import NDArray
 import pytest
 
+from gymnasium.spaces import Discrete, Space
+
 from environment_framework.estimator import Estimator
 from environment_framework.game import Game
-from environment_framework.gym import SimulatorFrameworkGym
-from environment_framework.level import ActionSpace, ILevel, Level, ObservationSpace
+from environment_framework.gym import EnvironmentFrameworkGym
+from environment_framework.level import Level
+from environment_framework.ilevel import ILevel
 from environment_framework.observer import Observer
-from environment_framework.simulator import Simulation, Simulator
+from environment_framework.simulator import Simulator
 from environment_framework.visualizer import Visualizer
 
 
 class TestLevel(Level):
     __test__ = False
 
     @property
     def done(self) -> bool:
         return True
 
     @property
-    def observation_space(self) -> ObservationSpace:
-        return ObservationSpace("discrete", (10,))
+    def observation_space(self) -> Space:
+        return Discrete(
+            10,
+        )
 
     @property
-    def action_space(self) -> ActionSpace:
-        return ActionSpace("discrete", 10)
+    def action_space(self) -> Space:
+        return Discrete(10)
 
     def reset(self) -> None:
         ...
 
     def step(self, action: int) -> bool:
         return True
 
-    def observe(self) -> List[float]:
+    def observe(self) -> NDArray:
         return np.zeros((10,))
 
 
 class TestSimulation:
     __test__ = False
 
     def __init__(self, level: Level, settings: int) -> None:
         self.level = level
         self.level_settings = settings
 
 
-SetupT = Tuple[SimulatorFrameworkGym, MagicMock]
+SetupT = Tuple[EnvironmentFrameworkGym, MagicMock]
 
 
 @pytest.fixture
 def setup() -> SetupT:
     game_mock = MagicMock(spec_set=Game)
     observer_mock = MagicMock(spec_set=Observer)
     estimator_mock = MagicMock(spec_set=Estimator)
     visualizer_mock = MagicMock(spec_set=Visualizer)
 
     level: ILevel = TestLevel(game_mock, observer_mock, estimator_mock, visualizer_mock)
-    simulation: Simulation = TestSimulation(level, 10)
     simulator_mock = MagicMock(spec_set=Simulator)
-    gym = SimulatorFrameworkGym(simulation, "rgb_array")
+    gym = EnvironmentFrameworkGym(level, "rgb_array")
     gym.simulator = simulator_mock
     return gym, simulator_mock
 
 
-def test_step(setup: SimulatorFrameworkGym) -> None:
+def test_step(setup: EnvironmentFrameworkGym) -> None:
     gym, simulator_mock = setup
 
     simulator_mock.estimate.return_value = 42
     simulator_mock.observe.return_value = np.array([42])
     simulator_mock.done = True
 
     observation, reward, done, truncated, extra = gym.step([10])
@@ -77,24 +82,24 @@
     assert observation == np.array([42])
     assert reward == 42
     assert truncated == False
     assert done
     assert extra == {}
 
 
-def test_reset(setup: SimulatorFrameworkGym) -> None:
+def test_reset(setup: EnvironmentFrameworkGym) -> None:
     gym, simulator_mock = setup
 
     simulator_mock.observe.return_value = [42]
     observation = gym.reset()
 
     simulator_mock.reset.assert_called_once()
     assert observation == ([42], {})
 
 
-def test_render(setup: SimulatorFrameworkGym) -> None:
+def test_render(setup: EnvironmentFrameworkGym) -> None:
     gym, simulator_mock = setup
     simulator_mock.render.return_value = "frame"
     frame = gym.render()
 
     simulator_mock.render.assert_called_once()
     assert frame == "frame"
```

### Comparing `environment_framework-0.1.0/tests/test_level.py` & `environment_framework-0.2.0/tests/test_level.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from unittest.mock import MagicMock
 
 import pytest
+from gymnasium.spaces import Discrete, Space
 
 from environment_framework.estimator import Estimator
 from environment_framework.game import Game
-from environment_framework.level import ActionSpace, Level, ObservationSpace
+from environment_framework.level import Level
 from environment_framework.observer import Observer
 from environment_framework.visualizer import Visualizer
 
 
 @pytest.fixture
 def setup() -> Level:
     class LevelImpl(Level):
         @property
-        def observation_space(self) -> ObservationSpace:
-            return ObservationSpace("discrete", (1,))
+        def observation_space(self) -> Space:
+            return Discrete(1)
 
         @property
-        def action_space(self) -> ActionSpace:
-            return ActionSpace("discrete", 10)
+        def action_space(self) -> Space:
+            return Discrete(10)
 
         def step(self, action: int) -> None:
             assert True
 
         def reset(self) -> None:
             assert True
```

### Comparing `environment_framework-0.1.0/tests/test_simulator.py` & `environment_framework-0.2.0/tests/test_simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from unittest.mock import MagicMock, PropertyMock
 
 import pytest
 
 from environment_framework.level import Level
-from environment_framework.simulator import Simulation, Simulator
+from environment_framework.simulator import Simulator
 
 
 @pytest.fixture
 def setup() -> Simulator:
     simulation_mock = MagicMock()
     level_mock = MagicMock(spec_set=Level)
-    simulation_mock.level = level_mock
 
-    return Simulator(simulation_mock, 10000)
+    return Simulator(level_mock, 10000)
 
 
 def test_action_space(setup: Simulator) -> None:
     simulator = setup
     simulator.level.action_space = "Testee"
 
     assert simulator.action_space == "Testee"
```

### Comparing `environment_framework-0.1.0/.gitignore` & `environment_framework-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `environment_framework-0.1.0/LICENSE` & `environment_framework-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `environment_framework-0.1.0/README.md` & `environment_framework-0.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ![License](https://img.shields.io/github/license/crzdg/environment-framework)
-![Last Commit](https://img.shields.io/github/last-commit/crzdg/environmnet-framework)
+![Last Commit](https://img.shields.io/github/last-commit/crzdg/environment-framework)
 ![Coverage](https://raw.githubusercontent.com/gist/crzdg/e60a9d0af9c141f6d2a3e0bd09366f5f/raw/coverage-badge.svg)
 ![Tests](https://raw.githubusercontent.com/gist/crzdg/79f221f23ccd460bba50b81f0df78ae1/raw/tests-badge.svg)
 ![PyPI](https://img.shields.io/pypi/pyversions/environment-framework)
 ![PyPI](https://img.shields.io/pypi/status/environment-framework)
 ![PyPI](https://img.shields.io/pypi/v/environment-framework)
 
 
@@ -50,14 +50,19 @@
         self.target_position = (0, 0)
         self.reset()
 
     @property
     def done(self) -> bool:
         return self.player_position == self.target_position
 
+    @property
+    def space(self) -> Space:
+        return Discrete(4)
+
+
     def act(self, action: Action, **_: Any) -> None:
         if action == Action.UP:
             self.player_position = (self.player_position[0], self.player_position[1] - 1)
         if action == Action.DOWN:
             self.player_position = (self.player_position[0], self.player_position[1] + 1)
         if action == Action.RIGHT:
             self.player_position = (self.player_position[0] + 1, self.player_position[1])
@@ -76,20 +81,19 @@
             self.reset()
 
 class GridWorldObserver:
     def __init__(self, game: GridWorldGame) -> None:
         self.game = game
 
     @property
-    def shape(self) -> Tuple[int, ...]:
-        return (4,)
-
-    def observe(self, _: Any) -> List[float]:
-        return [*self.game.player_position, *self.game.target_position]
+    def space(self) -> Space:
+        return Box(shape=(4,), low=-math.inf, high=math.inf)
 
+    def observe(self, _: Any) -> NDArray:
+        return np.array([*self.game.player_position, *self.game.target_position])
 
 class GridWorldEstimator:
     def __init__(self, game: GridWorldGame) -> None:
         self.game = game
 
     def estimate(self, _: Any) -> float:
         return -1 + float(self.game.done)
@@ -123,35 +127,21 @@
     ) -> None:
         super().__init__(game, observer, estimator, visualizer)
 
     def reset(self) -> None:
         self._game.reset()
 
     def step(self, action: Action) -> Any:
-        if isinstance(action, np.int64): # handle integer inputs
+        if isinstance(action, np.int64):  # handle integer inputs
             action = Action(action)
         self._game.act(action)
 
-    @property
-    def action_space(self) -> ActionSpace:
-        return ActionSpace("discrete", 4)
-
-    @property
-    def observation_space(self) -> ObservationSpace:
-        return ObservationSpace("discrete", (4,))
-
-
-class GridWorldSimulation:
-    def __init__(self, level: GridWorldLevel) -> None:
-        self.level = level
-        self.level_settings = None
-
 game = GridWorldGame(7)
 level = GridWorldLevel(game, GridWorldObserver(game), GridWorldEstimator(game), GridWorldVisualizer(game))
-simulator = Simulator(GridWorldSimulation(level))
+simulator = Simulator(level)
 while not simulator.done:
     action = Action(randint(0, 3))
     simulator.step(action)
 ```
 
 ### 📃 Documentation
```

### Comparing `environment_framework-0.1.0/pyproject.toml` & `environment_framework-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `environment_framework-0.1.0/PKG-INFO` & `environment_framework-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: environment-framework
-Version: 0.1.0
+Version: 0.2.0
 Summary: Loose building blocks to create agent-environment loops.
 Project-URL: Source, https://github.com/crzdg/environment-framework
 Author: Reto Barmettler
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
@@ -40,15 +40,15 @@
 Requires-Dist: pytest-mock; extra == 'test'
 Provides-Extra: type
 Requires-Dist: mypy; extra == 'type'
 Requires-Dist: types-pyyaml; extra == 'type'
 Description-Content-Type: text/markdown
 
 ![License](https://img.shields.io/github/license/crzdg/environment-framework)
-![Last Commit](https://img.shields.io/github/last-commit/crzdg/environmnet-framework)
+![Last Commit](https://img.shields.io/github/last-commit/crzdg/environment-framework)
 ![Coverage](https://raw.githubusercontent.com/gist/crzdg/e60a9d0af9c141f6d2a3e0bd09366f5f/raw/coverage-badge.svg)
 ![Tests](https://raw.githubusercontent.com/gist/crzdg/79f221f23ccd460bba50b81f0df78ae1/raw/tests-badge.svg)
 ![PyPI](https://img.shields.io/pypi/pyversions/environment-framework)
 ![PyPI](https://img.shields.io/pypi/status/environment-framework)
 ![PyPI](https://img.shields.io/pypi/v/environment-framework)
 
 
@@ -95,14 +95,19 @@
         self.target_position = (0, 0)
         self.reset()
 
     @property
     def done(self) -> bool:
         return self.player_position == self.target_position
 
+    @property
+    def space(self) -> Space:
+        return Discrete(4)
+
+
     def act(self, action: Action, **_: Any) -> None:
         if action == Action.UP:
             self.player_position = (self.player_position[0], self.player_position[1] - 1)
         if action == Action.DOWN:
             self.player_position = (self.player_position[0], self.player_position[1] + 1)
         if action == Action.RIGHT:
             self.player_position = (self.player_position[0] + 1, self.player_position[1])
@@ -121,20 +126,19 @@
             self.reset()
 
 class GridWorldObserver:
     def __init__(self, game: GridWorldGame) -> None:
         self.game = game
 
     @property
-    def shape(self) -> Tuple[int, ...]:
-        return (4,)
-
-    def observe(self, _: Any) -> List[float]:
-        return [*self.game.player_position, *self.game.target_position]
+    def space(self) -> Space:
+        return Box(shape=(4,), low=-math.inf, high=math.inf)
 
+    def observe(self, _: Any) -> NDArray:
+        return np.array([*self.game.player_position, *self.game.target_position])
 
 class GridWorldEstimator:
     def __init__(self, game: GridWorldGame) -> None:
         self.game = game
 
     def estimate(self, _: Any) -> float:
         return -1 + float(self.game.done)
@@ -168,35 +172,21 @@
     ) -> None:
         super().__init__(game, observer, estimator, visualizer)
 
     def reset(self) -> None:
         self._game.reset()
 
     def step(self, action: Action) -> Any:
-        if isinstance(action, np.int64): # handle integer inputs
+        if isinstance(action, np.int64):  # handle integer inputs
             action = Action(action)
         self._game.act(action)
 
-    @property
-    def action_space(self) -> ActionSpace:
-        return ActionSpace("discrete", 4)
-
-    @property
-    def observation_space(self) -> ObservationSpace:
-        return ObservationSpace("discrete", (4,))
-
-
-class GridWorldSimulation:
-    def __init__(self, level: GridWorldLevel) -> None:
-        self.level = level
-        self.level_settings = None
-
 game = GridWorldGame(7)
 level = GridWorldLevel(game, GridWorldObserver(game), GridWorldEstimator(game), GridWorldVisualizer(game))
-simulator = Simulator(GridWorldSimulation(level))
+simulator = Simulator(level)
 while not simulator.done:
     action = Action(randint(0, 3))
     simulator.step(action)
 ```
 
 ### 📃 Documentation
```

