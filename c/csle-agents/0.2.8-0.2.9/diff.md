# Comparing `tmp/csle_agents-0.2.8.tar.gz` & `tmp/csle_agents-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_agents-0.2.8.tar", last modified: Sun Jun  4 08:49:25 2023, max compression
+gzip compressed data, was "csle_agents-0.2.9.tar", last modified: Sun Jun  4 09:09:45 2023, max compression
```

## Comparing `csle_agents-0.2.8.tar` & `csle_agents-0.2.9.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:49:25.788114 csle_agents-0.2.8/
--rw-rw-r--   0 kim       (1000) kim       (1000)      653 2023-06-04 08:49:25.788114 csle_agents-0.2.8/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)     4154 2023-03-28 14:03:22.000000 csle_agents-0.2.8/README.md
--rw-rw-r--   0 kim       (1000) kim       (1000)      671 2023-03-28 14:03:22.000000 csle_agents-0.2.8/pyproject.toml
--rw-rw-r--   0 kim       (1000) kim       (1000)     1410 2023-06-04 08:49:25.788114 csle_agents-0.2.8/setup.cfg
--rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 csle_agents-0.2.8/setup.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:49:25.780114 csle_agents-0.2.8/src/
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:49:25.780114 csle_agents-0.2.8/src/csle_agents/
--rw-rw-r--   0 kim       (1000) kim       (1000)       37 2023-03-28 14:03:22.000000 csle_agents-0.2.8/src/csle_agents/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-06-04 08:47:59.000000 csle_agents-0.2.8/src/csle_agents/__version__.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:49:25.784114 csle_agents-0.2.8/src/csle_agents/agents/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.8/src/csle_agents/agents/__init__.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:49:25.784114 csle_agents-0.2.8/src/csle_agents/agents/base/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.8/src/csle_agents/agents/base/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1854 2023-03-28 14:03:22.000000 csle_agents-0.2.8/src/csle_agents/agents/base/base_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:49:25.784114 csle_agents-0.2.8/src/csle_agents/agents/bayesian_optimization/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.8/src/csle_agents/agents/bayesian_optimization/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    28162 2023-04-30 06:59:23.000000 csle_agents-0.2.8/src/csle_agents/agents/bayesian_optimization/bayes_opt_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:49:25.784114 csle_agents-0.2.8/src/csle_agents/agents/cross_entropy/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.8/src/csle_agents/agents/cross_entropy/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    26958 2023-05-30 09:03:51.000000 csle_agents-0.2.8/src/csle_agents/agents/cross_entropy/cross_entropy_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:49:25.784114 csle_agents-0.2.8/src/csle_agents/agents/dfsp_local/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-05-03 08:18:28.000000 csle_agents-0.2.8/src/csle_agents/agents/dfsp_local/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    37993 2023-05-22 08:32:58.000000 csle_agents-0.2.8/src/csle_agents/agents/dfsp_local/dfsp_local_agent.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    39891 2023-05-03 13:32:44.000000 csle_agents-0.2.8/src/csle_agents/agents/dfsp_local/dfsp_local_ppo_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:49:25.784114 csle_agents-0.2.8/src/csle_agents/agents/differential_evolution/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.8/src/csle_agents/agents/differential_evolution/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    31471 2023-05-30 09:03:51.000000 csle_agents-0.2.8/src/csle_agents/agents/differential_evolution/differential_evolution_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:49:25.784114 csle_agents-0.2.8/src/csle_agents/agents/dqn/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.8/src/csle_agents/agents/dqn/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    19153 2023-03-28 14:03:22.000000 csle_agents-0.2.8/src/csle_agents/agents/dqn/dqn_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:49:25.784114 csle_agents-0.2.8/src/csle_agents/agents/dynasec/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.8/src/csle_agents/agents/dynasec/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    75392 2023-03-28 14:03:22.000000 csle_agents-0.2.8/src/csle_agents/agents/dynasec/dynasec_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:49:25.784114 csle_agents-0.2.8/src/csle_agents/agents/fp/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.8/src/csle_agents/agents/fp/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    18259 2023-03-28 14:03:22.000000 csle_agents-0.2.8/src/csle_agents/agents/fp/fictitious_play_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:49:25.784114 csle_agents-0.2.8/src/csle_agents/agents/hsvi/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.8/src/csle_agents/agents/hsvi/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    49313 2023-03-28 14:03:22.000000 csle_agents-0.2.8/src/csle_agents/agents/hsvi/hsvi_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:49:25.784114 csle_agents-0.2.8/src/csle_agents/agents/hsvi_os_posg/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.8/src/csle_agents/agents/hsvi_os_posg/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    75255 2023-03-28 14:03:22.000000 csle_agents-0.2.8/src/csle_agents/agents/hsvi_os_posg/hsvi_os_posg_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:49:25.784114 csle_agents-0.2.8/src/csle_agents/agents/kiefer_wolfowitz/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.8/src/csle_agents/agents/kiefer_wolfowitz/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    28849 2023-04-30 06:59:23.000000 csle_agents-0.2.8/src/csle_agents/agents/kiefer_wolfowitz/kiefer_wolfowitz_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:49:25.784114 csle_agents-0.2.8/src/csle_agents/agents/lp_nf/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.8/src/csle_agents/agents/lp_nf/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    18360 2023-03-28 14:03:22.000000 csle_agents-0.2.8/src/csle_agents/agents/lp_nf/linear_programming_normal_form_game_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:49:25.784114 csle_agents-0.2.8/src/csle_agents/agents/pi/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.8/src/csle_agents/agents/pi/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    17642 2023-03-28 14:03:22.000000 csle_agents-0.2.8/src/csle_agents/agents/pi/pi_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:49:25.784114 csle_agents-0.2.8/src/csle_agents/agents/ppo/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.8/src/csle_agents/agents/ppo/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    25589 2023-05-03 08:18:28.000000 csle_agents-0.2.8/src/csle_agents/agents/ppo/ppo_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:49:25.784114 csle_agents-0.2.8/src/csle_agents/agents/q_learning/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.8/src/csle_agents/agents/q_learning/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    17360 2023-03-28 14:03:22.000000 csle_agents-0.2.8/src/csle_agents/agents/q_learning/q_learning_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:49:25.784114 csle_agents-0.2.8/src/csle_agents/agents/random_search/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.8/src/csle_agents/agents/random_search/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    26175 2023-04-30 06:59:23.000000 csle_agents-0.2.8/src/csle_agents/agents/random_search/random_search_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:49:25.784114 csle_agents-0.2.8/src/csle_agents/agents/reinforce/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.8/src/csle_agents/agents/reinforce/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    25109 2023-03-28 14:03:22.000000 csle_agents-0.2.8/src/csle_agents/agents/reinforce/reinforce_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:49:25.784114 csle_agents-0.2.8/src/csle_agents/agents/sarsa/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.8/src/csle_agents/agents/sarsa/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    17456 2023-03-28 14:03:22.000000 csle_agents-0.2.8/src/csle_agents/agents/sarsa/sarsa_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:49:25.784114 csle_agents-0.2.8/src/csle_agents/agents/shapley_iteration/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.8/src/csle_agents/agents/shapley_iteration/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    15788 2023-03-28 14:03:22.000000 csle_agents-0.2.8/src/csle_agents/agents/shapley_iteration/shapley_iteration_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:49:25.788114 csle_agents-0.2.8/src/csle_agents/agents/sondik_vi/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.8/src/csle_agents/agents/sondik_vi/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    22182 2023-03-28 14:03:22.000000 csle_agents-0.2.8/src/csle_agents/agents/sondik_vi/sondik_vi_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:49:25.788114 csle_agents-0.2.8/src/csle_agents/agents/t_fp/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.8/src/csle_agents/agents/t_fp/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    41988 2023-05-03 08:18:28.000000 csle_agents-0.2.8/src/csle_agents/agents/t_fp/t_fp_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:49:25.788114 csle_agents-0.2.8/src/csle_agents/agents/t_spsa/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.8/src/csle_agents/agents/t_spsa/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    32117 2023-05-30 09:03:51.000000 csle_agents-0.2.8/src/csle_agents/agents/t_spsa/t_spsa_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:49:25.788114 csle_agents-0.2.8/src/csle_agents/agents/vi/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.8/src/csle_agents/agents/vi/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    16358 2023-04-30 06:59:23.000000 csle_agents-0.2.8/src/csle_agents/agents/vi/vi_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:49:25.788114 csle_agents-0.2.8/src/csle_agents/common/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.8/src/csle_agents/common/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5759 2023-03-28 14:03:22.000000 csle_agents-0.2.8/src/csle_agents/common/actor_critic_net.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4595 2023-03-28 14:03:22.000000 csle_agents-0.2.8/src/csle_agents/common/fnn_w_gaussian.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3936 2023-03-28 14:03:22.000000 csle_agents-0.2.8/src/csle_agents/common/fnn_w_linear.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3460 2023-03-28 14:03:22.000000 csle_agents-0.2.8/src/csle_agents/common/pruning.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:49:25.788114 csle_agents-0.2.8/src/csle_agents/constants/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.8/src/csle_agents/constants/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    11876 2023-05-03 08:18:28.000000 csle_agents-0.2.8/src/csle_agents/constants/constants.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:49:25.788114 csle_agents-0.2.8/src/csle_agents/job_controllers/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.8/src/csle_agents/job_controllers/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2459 2023-03-28 14:03:22.000000 csle_agents-0.2.8/src/csle_agents/job_controllers/training_job_manager.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 08:49:25.784114 csle_agents-0.2.8/src/csle_agents.egg-info/
--rw-rw-r--   0 kim       (1000) kim       (1000)      653 2023-06-04 08:49:25.000000 csle_agents-0.2.8/src/csle_agents.egg-info/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)     3034 2023-06-04 08:49:25.000000 csle_agents-0.2.8/src/csle_agents.egg-info/SOURCES.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-06-04 08:49:25.000000 csle_agents-0.2.8/src/csle_agents.egg-info/dependency_links.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:51:05.000000 csle_agents-0.2.8/src/csle_agents.egg-info/not-zip-safe
--rw-rw-r--   0 kim       (1000) kim       (1000)      371 2023-06-04 08:49:25.000000 csle_agents-0.2.8/src/csle_agents.egg-info/requires.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)       12 2023-06-04 08:49:25.000000 csle_agents-0.2.8/src/csle_agents.egg-info/top_level.txt
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:09:45.646437 csle_agents-0.2.9/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      653 2023-06-04 09:09:45.646437 csle_agents-0.2.9/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4154 2023-03-28 14:03:22.000000 csle_agents-0.2.9/README.md
+-rw-rw-r--   0 kim       (1000) kim       (1000)      671 2023-03-28 14:03:22.000000 csle_agents-0.2.9/pyproject.toml
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1410 2023-06-04 09:09:45.646437 csle_agents-0.2.9/setup.cfg
+-rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 csle_agents-0.2.9/setup.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:09:45.638437 csle_agents-0.2.9/src/
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:09:45.638437 csle_agents-0.2.9/src/csle_agents/
+-rw-rw-r--   0 kim       (1000) kim       (1000)       37 2023-03-28 14:03:22.000000 csle_agents-0.2.9/src/csle_agents/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-06-04 09:08:20.000000 csle_agents-0.2.9/src/csle_agents/__version__.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:09:45.642437 csle_agents-0.2.9/src/csle_agents/agents/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.9/src/csle_agents/agents/__init__.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:09:45.642437 csle_agents-0.2.9/src/csle_agents/agents/base/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.9/src/csle_agents/agents/base/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1854 2023-03-28 14:03:22.000000 csle_agents-0.2.9/src/csle_agents/agents/base/base_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:09:45.642437 csle_agents-0.2.9/src/csle_agents/agents/bayesian_optimization/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.9/src/csle_agents/agents/bayesian_optimization/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    28162 2023-04-30 06:59:23.000000 csle_agents-0.2.9/src/csle_agents/agents/bayesian_optimization/bayes_opt_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:09:45.642437 csle_agents-0.2.9/src/csle_agents/agents/cross_entropy/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.9/src/csle_agents/agents/cross_entropy/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    26958 2023-05-30 09:03:51.000000 csle_agents-0.2.9/src/csle_agents/agents/cross_entropy/cross_entropy_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:09:45.642437 csle_agents-0.2.9/src/csle_agents/agents/dfsp_local/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-05-03 08:18:28.000000 csle_agents-0.2.9/src/csle_agents/agents/dfsp_local/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    37993 2023-05-22 08:32:58.000000 csle_agents-0.2.9/src/csle_agents/agents/dfsp_local/dfsp_local_agent.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    39891 2023-05-03 13:32:44.000000 csle_agents-0.2.9/src/csle_agents/agents/dfsp_local/dfsp_local_ppo_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:09:45.642437 csle_agents-0.2.9/src/csle_agents/agents/differential_evolution/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.9/src/csle_agents/agents/differential_evolution/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    31471 2023-05-30 09:03:51.000000 csle_agents-0.2.9/src/csle_agents/agents/differential_evolution/differential_evolution_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:09:45.642437 csle_agents-0.2.9/src/csle_agents/agents/dqn/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.9/src/csle_agents/agents/dqn/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    19153 2023-03-28 14:03:22.000000 csle_agents-0.2.9/src/csle_agents/agents/dqn/dqn_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:09:45.642437 csle_agents-0.2.9/src/csle_agents/agents/dynasec/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.9/src/csle_agents/agents/dynasec/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    75392 2023-03-28 14:03:22.000000 csle_agents-0.2.9/src/csle_agents/agents/dynasec/dynasec_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:09:45.642437 csle_agents-0.2.9/src/csle_agents/agents/fp/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.9/src/csle_agents/agents/fp/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    18259 2023-03-28 14:03:22.000000 csle_agents-0.2.9/src/csle_agents/agents/fp/fictitious_play_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:09:45.642437 csle_agents-0.2.9/src/csle_agents/agents/hsvi/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.9/src/csle_agents/agents/hsvi/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    49313 2023-03-28 14:03:22.000000 csle_agents-0.2.9/src/csle_agents/agents/hsvi/hsvi_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:09:45.642437 csle_agents-0.2.9/src/csle_agents/agents/hsvi_os_posg/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.9/src/csle_agents/agents/hsvi_os_posg/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    75255 2023-03-28 14:03:22.000000 csle_agents-0.2.9/src/csle_agents/agents/hsvi_os_posg/hsvi_os_posg_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:09:45.642437 csle_agents-0.2.9/src/csle_agents/agents/kiefer_wolfowitz/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.9/src/csle_agents/agents/kiefer_wolfowitz/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    28849 2023-04-30 06:59:23.000000 csle_agents-0.2.9/src/csle_agents/agents/kiefer_wolfowitz/kiefer_wolfowitz_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:09:45.642437 csle_agents-0.2.9/src/csle_agents/agents/lp_nf/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.9/src/csle_agents/agents/lp_nf/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    18360 2023-03-28 14:03:22.000000 csle_agents-0.2.9/src/csle_agents/agents/lp_nf/linear_programming_normal_form_game_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:09:45.642437 csle_agents-0.2.9/src/csle_agents/agents/pi/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.9/src/csle_agents/agents/pi/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    17642 2023-03-28 14:03:22.000000 csle_agents-0.2.9/src/csle_agents/agents/pi/pi_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:09:45.642437 csle_agents-0.2.9/src/csle_agents/agents/ppo/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.9/src/csle_agents/agents/ppo/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    25589 2023-05-03 08:18:28.000000 csle_agents-0.2.9/src/csle_agents/agents/ppo/ppo_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:09:45.642437 csle_agents-0.2.9/src/csle_agents/agents/q_learning/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.9/src/csle_agents/agents/q_learning/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    17360 2023-03-28 14:03:22.000000 csle_agents-0.2.9/src/csle_agents/agents/q_learning/q_learning_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:09:45.642437 csle_agents-0.2.9/src/csle_agents/agents/random_search/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.9/src/csle_agents/agents/random_search/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    26175 2023-04-30 06:59:23.000000 csle_agents-0.2.9/src/csle_agents/agents/random_search/random_search_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:09:45.642437 csle_agents-0.2.9/src/csle_agents/agents/reinforce/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.9/src/csle_agents/agents/reinforce/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    25109 2023-03-28 14:03:22.000000 csle_agents-0.2.9/src/csle_agents/agents/reinforce/reinforce_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:09:45.642437 csle_agents-0.2.9/src/csle_agents/agents/sarsa/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.9/src/csle_agents/agents/sarsa/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    17456 2023-03-28 14:03:22.000000 csle_agents-0.2.9/src/csle_agents/agents/sarsa/sarsa_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:09:45.642437 csle_agents-0.2.9/src/csle_agents/agents/shapley_iteration/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.9/src/csle_agents/agents/shapley_iteration/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    15788 2023-03-28 14:03:22.000000 csle_agents-0.2.9/src/csle_agents/agents/shapley_iteration/shapley_iteration_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:09:45.642437 csle_agents-0.2.9/src/csle_agents/agents/sondik_vi/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.9/src/csle_agents/agents/sondik_vi/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    22182 2023-03-28 14:03:22.000000 csle_agents-0.2.9/src/csle_agents/agents/sondik_vi/sondik_vi_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:09:45.642437 csle_agents-0.2.9/src/csle_agents/agents/t_fp/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.9/src/csle_agents/agents/t_fp/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    41988 2023-05-03 08:18:28.000000 csle_agents-0.2.9/src/csle_agents/agents/t_fp/t_fp_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:09:45.642437 csle_agents-0.2.9/src/csle_agents/agents/t_spsa/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.9/src/csle_agents/agents/t_spsa/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    32117 2023-05-30 09:03:51.000000 csle_agents-0.2.9/src/csle_agents/agents/t_spsa/t_spsa_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:09:45.642437 csle_agents-0.2.9/src/csle_agents/agents/vi/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.9/src/csle_agents/agents/vi/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    16358 2023-04-30 06:59:23.000000 csle_agents-0.2.9/src/csle_agents/agents/vi/vi_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:09:45.646437 csle_agents-0.2.9/src/csle_agents/common/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.9/src/csle_agents/common/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5759 2023-03-28 14:03:22.000000 csle_agents-0.2.9/src/csle_agents/common/actor_critic_net.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4595 2023-03-28 14:03:22.000000 csle_agents-0.2.9/src/csle_agents/common/fnn_w_gaussian.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3936 2023-03-28 14:03:22.000000 csle_agents-0.2.9/src/csle_agents/common/fnn_w_linear.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3460 2023-03-28 14:03:22.000000 csle_agents-0.2.9/src/csle_agents/common/pruning.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:09:45.646437 csle_agents-0.2.9/src/csle_agents/constants/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.9/src/csle_agents/constants/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    11876 2023-05-03 08:18:28.000000 csle_agents-0.2.9/src/csle_agents/constants/constants.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:09:45.646437 csle_agents-0.2.9/src/csle_agents/job_controllers/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.9/src/csle_agents/job_controllers/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2459 2023-03-28 14:03:22.000000 csle_agents-0.2.9/src/csle_agents/job_controllers/training_job_manager.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-04 09:09:45.642437 csle_agents-0.2.9/src/csle_agents.egg-info/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      653 2023-06-04 09:09:45.000000 csle_agents-0.2.9/src/csle_agents.egg-info/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3034 2023-06-04 09:09:45.000000 csle_agents-0.2.9/src/csle_agents.egg-info/SOURCES.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-06-04 09:09:45.000000 csle_agents-0.2.9/src/csle_agents.egg-info/dependency_links.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:51:05.000000 csle_agents-0.2.9/src/csle_agents.egg-info/not-zip-safe
+-rw-rw-r--   0 kim       (1000) kim       (1000)      371 2023-06-04 09:09:45.000000 csle_agents-0.2.9/src/csle_agents.egg-info/requires.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)       12 2023-06-04 09:09:45.000000 csle_agents-0.2.9/src/csle_agents.egg-info/top_level.txt
```

### Comparing `csle_agents-0.2.8/PKG-INFO` & `csle_agents-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_agents
-Version: 0.2.8
+Version: 0.2.9
 Summary: Reinforcement learning agents for CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_agents-0.2.8/README.md` & `csle_agents-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.8/pyproject.toml` & `csle_agents-0.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.8/setup.cfg` & `csle_agents-0.2.9/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -15,20 +15,20 @@
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
-	csle-common>=0.2.8
-	csle-collector>=0.2.8
-	csle-attacker>=0.2.8
-	csle-defender>=0.2.8
-	csle-system-identification>=0.2.8
-	gym-csle-stopping-game>=0.2.8
+	csle-common>=0.2.9
+	csle-collector>=0.2.9
+	csle-attacker>=0.2.9
+	csle-defender>=0.2.9
+	csle-system-identification>=0.2.9
+	gym-csle-stopping-game>=0.2.9
 	stable-baselines3>=1.8.0
 	pulp>=2.7.0
 	bayesian-optimization>=1.3.1
 python_requires = >=3.8
 package_dir = 
 	=src
 packages = find:
```

### Comparing `csle_agents-0.2.8/src/csle_agents/agents/base/base_agent.py` & `csle_agents-0.2.9/src/csle_agents/agents/base/base_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.8/src/csle_agents/agents/bayesian_optimization/bayes_opt_agent.py` & `csle_agents-0.2.9/src/csle_agents/agents/bayesian_optimization/bayes_opt_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.8/src/csle_agents/agents/cross_entropy/cross_entropy_agent.py` & `csle_agents-0.2.9/src/csle_agents/agents/cross_entropy/cross_entropy_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.8/src/csle_agents/agents/dfsp_local/dfsp_local_agent.py` & `csle_agents-0.2.9/src/csle_agents/agents/dfsp_local/dfsp_local_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.8/src/csle_agents/agents/dfsp_local/dfsp_local_ppo_agent.py` & `csle_agents-0.2.9/src/csle_agents/agents/dfsp_local/dfsp_local_ppo_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.8/src/csle_agents/agents/differential_evolution/differential_evolution_agent.py` & `csle_agents-0.2.9/src/csle_agents/agents/differential_evolution/differential_evolution_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.8/src/csle_agents/agents/dqn/dqn_agent.py` & `csle_agents-0.2.9/src/csle_agents/agents/dqn/dqn_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.8/src/csle_agents/agents/dynasec/dynasec_agent.py` & `csle_agents-0.2.9/src/csle_agents/agents/dynasec/dynasec_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.8/src/csle_agents/agents/fp/fictitious_play_agent.py` & `csle_agents-0.2.9/src/csle_agents/agents/fp/fictitious_play_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.8/src/csle_agents/agents/hsvi/hsvi_agent.py` & `csle_agents-0.2.9/src/csle_agents/agents/hsvi/hsvi_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.8/src/csle_agents/agents/hsvi_os_posg/hsvi_os_posg_agent.py` & `csle_agents-0.2.9/src/csle_agents/agents/hsvi_os_posg/hsvi_os_posg_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.8/src/csle_agents/agents/kiefer_wolfowitz/kiefer_wolfowitz_agent.py` & `csle_agents-0.2.9/src/csle_agents/agents/kiefer_wolfowitz/kiefer_wolfowitz_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.8/src/csle_agents/agents/lp_nf/linear_programming_normal_form_game_agent.py` & `csle_agents-0.2.9/src/csle_agents/agents/lp_nf/linear_programming_normal_form_game_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.8/src/csle_agents/agents/pi/pi_agent.py` & `csle_agents-0.2.9/src/csle_agents/agents/pi/pi_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.8/src/csle_agents/agents/ppo/ppo_agent.py` & `csle_agents-0.2.9/src/csle_agents/agents/ppo/ppo_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.8/src/csle_agents/agents/q_learning/q_learning_agent.py` & `csle_agents-0.2.9/src/csle_agents/agents/q_learning/q_learning_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.8/src/csle_agents/agents/random_search/random_search_agent.py` & `csle_agents-0.2.9/src/csle_agents/agents/random_search/random_search_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.8/src/csle_agents/agents/reinforce/reinforce_agent.py` & `csle_agents-0.2.9/src/csle_agents/agents/reinforce/reinforce_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.8/src/csle_agents/agents/sarsa/sarsa_agent.py` & `csle_agents-0.2.9/src/csle_agents/agents/sarsa/sarsa_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.8/src/csle_agents/agents/shapley_iteration/shapley_iteration_agent.py` & `csle_agents-0.2.9/src/csle_agents/agents/shapley_iteration/shapley_iteration_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.8/src/csle_agents/agents/sondik_vi/sondik_vi_agent.py` & `csle_agents-0.2.9/src/csle_agents/agents/sondik_vi/sondik_vi_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.8/src/csle_agents/agents/t_fp/t_fp_agent.py` & `csle_agents-0.2.9/src/csle_agents/agents/t_fp/t_fp_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.8/src/csle_agents/agents/t_spsa/t_spsa_agent.py` & `csle_agents-0.2.9/src/csle_agents/agents/t_spsa/t_spsa_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.8/src/csle_agents/agents/vi/vi_agent.py` & `csle_agents-0.2.9/src/csle_agents/agents/vi/vi_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.8/src/csle_agents/common/actor_critic_net.py` & `csle_agents-0.2.9/src/csle_agents/common/actor_critic_net.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.8/src/csle_agents/common/fnn_w_gaussian.py` & `csle_agents-0.2.9/src/csle_agents/common/fnn_w_gaussian.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.8/src/csle_agents/common/fnn_w_linear.py` & `csle_agents-0.2.9/src/csle_agents/common/fnn_w_linear.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.8/src/csle_agents/common/pruning.py` & `csle_agents-0.2.9/src/csle_agents/common/pruning.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.8/src/csle_agents/constants/constants.py` & `csle_agents-0.2.9/src/csle_agents/constants/constants.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.8/src/csle_agents/job_controllers/training_job_manager.py` & `csle_agents-0.2.9/src/csle_agents/job_controllers/training_job_manager.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.2.8/src/csle_agents.egg-info/PKG-INFO` & `csle_agents-0.2.9/src/csle_agents.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-agents
-Version: 0.2.8
+Version: 0.2.9
 Summary: Reinforcement learning agents for CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_agents-0.2.8/src/csle_agents.egg-info/SOURCES.txt` & `csle_agents-0.2.9/src/csle_agents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

