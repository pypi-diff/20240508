# Comparing `tmp/blackjax-1.2.0.tar.gz` & `tmp/blackjax-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackjax-1.2.0.tar", last modified: Mon May  6 16:18:53 2024, max compression
+gzip compressed data, was "blackjax-1.2.1.tar", last modified: Wed May  8 15:35:03 2024, max compression
```

## Comparing `blackjax-1.2.0.tar` & `blackjax-1.2.1.tar`

### file list

```diff
@@ -1,177 +1,177 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:53.177889 blackjax-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-06 16:18:44.000000 blackjax-1.2.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:53.149889 blackjax-1.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:53.149889 blackjax-1.2.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-05-06 16:18:44.000000 blackjax-1.2.0/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-06 16:18:44.000000 blackjax-1.2.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-06 16:18:44.000000 blackjax-1.2.0/.github/ISSUE_TEMPLATE/enhancement.md
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-06 16:18:44.000000 blackjax-1.2.0/.github/ISSUE_TEMPLATE/meeting.md
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-06 16:18:44.000000 blackjax-1.2.0/.github/ISSUE_TEMPLATE/sampler_proposal.md
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-06 16:18:44.000000 blackjax-1.2.0/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:53.153889 blackjax-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-06 16:18:44.000000 blackjax-1.2.0/.github/workflows/benchmark.yml
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-06 16:18:44.000000 blackjax-1.2.0/.github/workflows/build_documentation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-06 16:18:44.000000 blackjax-1.2.0/.github/workflows/nightly.yml
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-06 16:18:44.000000 blackjax-1.2.0/.github/workflows/publish_documentation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-06 16:18:44.000000 blackjax-1.2.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-06 16:18:44.000000 blackjax-1.2.0/.github/workflows/schedule-meeting.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-06 16:18:44.000000 blackjax-1.2.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-06 16:18:44.000000 blackjax-1.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-06 16:18:44.000000 blackjax-1.2.0/.gitlint
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-06 16:18:44.000000 blackjax-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-06 16:18:44.000000 blackjax-1.2.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-05-06 16:18:44.000000 blackjax-1.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-05-06 16:18:44.000000 blackjax-1.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-05-06 16:18:44.000000 blackjax-1.2.0/GOVERNANCE.md
--rw-r--r--   0 runner    (1001) docker     (127)    11354 2024-05-06 16:18:44.000000 blackjax-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-06 16:18:44.000000 blackjax-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-06 16:18:44.000000 blackjax-1.2.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-05-06 16:18:53.177889 blackjax-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-05-06 16:18:44.000000 blackjax-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:53.153889 blackjax-1.2.0/blackjax/
--rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-06 16:18:53.000000 blackjax-1.2.0/blackjax/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:53.157889 blackjax-1.2.0/blackjax/adaptation/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/adaptation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/adaptation/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    17121 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/adaptation/chees_adaptation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7640 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/adaptation/mass_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)    10236 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/adaptation/mclmc_adaptation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10582 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/adaptation/meads_adaptation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7576 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/adaptation/pathfinder_adaptation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9557 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/adaptation/step_size.py
--rw-r--r--   0 runner    (1001) docker     (127)    16440 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/adaptation/window_adaptation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7915 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/diagnostics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:53.157889 blackjax-1.2.0/blackjax/mcmc/
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/mcmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8885 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/mcmc/barker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/mcmc/diffusions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6891 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/mcmc/dynamic_hmc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9133 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/mcmc/elliptical_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)    10649 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/mcmc/ghmc.py
--rw-r--r--   0 runner    (1001) docker     (127)    11017 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/mcmc/hmc.py
--rw-r--r--   0 runner    (1001) docker     (127)    16461 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/mcmc/integrators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/mcmc/mala.py
--rw-r--r--   0 runner    (1001) docker     (127)     8430 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/mcmc/marginal_latent_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/mcmc/mclmc.py
--rw-r--r--   0 runner    (1001) docker     (127)    11000 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/mcmc/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    11050 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/mcmc/nuts.py
--rw-r--r--   0 runner    (1001) docker     (127)    11963 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/mcmc/periodic_orbital.py
--rw-r--r--   0 runner    (1001) docker     (127)     8602 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/mcmc/proposal.py
--rw-r--r--   0 runner    (1001) docker     (127)    15645 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/mcmc/random_walk.py
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/mcmc/rmhmc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/mcmc/termination.py
--rw-r--r--   0 runner    (1001) docker     (127)    22915 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/mcmc/trajectory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:53.161889 blackjax-1.2.0/blackjax/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/optimizers/dual_averaging.py
--rw-r--r--   0 runner    (1001) docker     (127)    11581 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/optimizers/lbfgs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/progress_bar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:53.161889 blackjax-1.2.0/blackjax/sgmcmc/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/sgmcmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8691 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/sgmcmc/csgld.py
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/sgmcmc/diffusions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/sgmcmc/gradients.py
--rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/sgmcmc/sghmc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/sgmcmc/sgld.py
--rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/sgmcmc/sgnht.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:53.161889 blackjax-1.2.0/blackjax/smc/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/smc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5311 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/smc/adaptive_tempered.py
--rw-r--r--   0 runner    (1001) docker     (127)     5535 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/smc/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/smc/ess.py
--rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/smc/inner_kernel_tuning.py
--rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/smc/resampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/smc/solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/smc/tempered.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:53.161889 blackjax-1.2.0/blackjax/smc/tuning/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/smc/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/smc/tuning/from_kernel_info.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1368 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/smc/tuning/from_particles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     7311 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:53.161889 blackjax-1.2.0/blackjax/vi/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/vi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5386 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/vi/meanfield_vi.py
--rw-r--r--   0 runner    (1001) docker     (127)     8871 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/vi/pathfinder.py
--rw-r--r--   0 runner    (1001) docker     (127)     7101 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/vi/schrodinger_follmer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5494 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/vi/svgd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:53.177889 blackjax-1.2.0/blackjax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-05-06 16:18:53.000000 blackjax-1.2.0/blackjax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4227 2024-05-06 16:18:53.000000 blackjax-1.2.0/blackjax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 16:18:53.000000 blackjax-1.2.0/blackjax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-06 16:18:53.000000 blackjax-1.2.0/blackjax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-06 16:18:53.000000 blackjax-1.2.0/blackjax.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-06 16:18:44.000000 blackjax-1.2.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:53.165889 blackjax-1.2.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:53.165889 blackjax-1.2.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)   161829 2024-05-06 16:18:44.000000 blackjax-1.2.0/docs/_static/blackjax.png
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 16:18:44.000000 blackjax-1.2.0/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-06 16:18:44.000000 blackjax-1.2.0/docs/bib.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-05-06 16:18:44.000000 blackjax-1.2.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:53.165889 blackjax-1.2.0/docs/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:53.173889 blackjax-1.2.0/docs/examples/data/
--rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-05-06 16:18:44.000000 blackjax-1.2.0/docs/examples/data/blackjax.png
--rw-r--r--   0 runner    (1001) docker     (127)    63251 2024-05-06 16:18:44.000000 blackjax-1.2.0/docs/examples/data/google.csv
--rw-r--r--   0 runner    (1001) docker     (127)     6030 2024-05-06 16:18:44.000000 blackjax-1.2.0/docs/examples/howto_custom_gradients.md
--rw-r--r--   0 runner    (1001) docker     (127)    12029 2024-05-06 16:18:44.000000 blackjax-1.2.0/docs/examples/howto_metropolis_within_gibbs.md
--rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-05-06 16:18:44.000000 blackjax-1.2.0/docs/examples/howto_other_frameworks.md
--rw-r--r--   0 runner    (1001) docker     (127)     5494 2024-05-06 16:18:44.000000 blackjax-1.2.0/docs/examples/howto_reproduce_the_blackjax_image.md
--rw-r--r--   0 runner    (1001) docker     (127)     9833 2024-05-06 16:18:44.000000 blackjax-1.2.0/docs/examples/howto_sample_multiple_chains.md
--rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-05-06 16:18:44.000000 blackjax-1.2.0/docs/examples/howto_use_aesara.md
--rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-05-06 16:18:44.000000 blackjax-1.2.0/docs/examples/howto_use_numpyro.md
--rw-r--r--   0 runner    (1001) docker     (127)     6122 2024-05-06 16:18:44.000000 blackjax-1.2.0/docs/examples/howto_use_oryx.md
--rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-05-06 16:18:44.000000 blackjax-1.2.0/docs/examples/howto_use_pymc.md
--rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-05-06 16:18:44.000000 blackjax-1.2.0/docs/examples/howto_use_tfp.md
--rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-05-06 16:18:44.000000 blackjax-1.2.0/docs/examples/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (127)  4461357 2024-05-06 16:18:44.000000 blackjax-1.2.0/docs/examples/scatter.gif
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-05-06 16:18:44.000000 blackjax-1.2.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)    13273 2024-05-06 16:18:44.000000 blackjax-1.2.0/docs/refs.bib
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-06 16:18:44.000000 blackjax-1.2.0/jupytex.toml
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-06 16:18:44.000000 blackjax-1.2.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-06 16:18:44.000000 blackjax-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-06 16:18:44.000000 blackjax-1.2.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-06 16:18:44.000000 blackjax-1.2.0/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-06 16:18:44.000000 blackjax-1.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-06 16:18:53.177889 blackjax-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:53.173889 blackjax-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:53.173889 blackjax-1.2.0/tests/adaptation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/adaptation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/adaptation/test_adaptation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/adaptation/test_mass_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/adaptation/test_step_size.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:53.177889 blackjax-1.2.0/tests/mcmc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/mcmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/mcmc/test_barker.py
--rw-r--r--   0 runner    (1001) docker     (127)    13030 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/mcmc/test_integrators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/mcmc/test_latent_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/mcmc/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/mcmc/test_proposal.py
--rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/mcmc/test_random_walk_without_chex.py
--rw-r--r--   0 runner    (1001) docker     (127)    29756 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/mcmc/test_sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)    10911 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/mcmc/test_trajectory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/mcmc/test_uturn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:53.177889 blackjax-1.2.0/tests/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/optimizers/test_optimizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/optimizers/test_pathfinder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:53.177889 blackjax-1.2.0/tests/smc/
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/smc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13930 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/smc/test_inner_kernel_tuning.py
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/smc/test_kernel_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/smc/test_resampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/smc/test_smc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/smc/test_smc_ess.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/smc/test_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     6852 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/smc/test_tempered_smc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/test_benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/test_compilation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/test_diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:53.177889 blackjax-1.2.0/tests/vi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/vi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/vi/test_meanfield_vi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/vi/test_schrodinger_follmer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/vi/test_svgd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:35:03.245586 blackjax-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-08 15:34:58.000000 blackjax-1.2.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:35:03.217586 blackjax-1.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:35:03.217586 blackjax-1.2.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-05-08 15:34:58.000000 blackjax-1.2.1/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-08 15:34:58.000000 blackjax-1.2.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-08 15:34:58.000000 blackjax-1.2.1/.github/ISSUE_TEMPLATE/enhancement.md
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-08 15:34:58.000000 blackjax-1.2.1/.github/ISSUE_TEMPLATE/meeting.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-08 15:34:58.000000 blackjax-1.2.1/.github/ISSUE_TEMPLATE/sampler_proposal.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-08 15:34:58.000000 blackjax-1.2.1/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:35:03.217586 blackjax-1.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-08 15:34:58.000000 blackjax-1.2.1/.github/workflows/benchmark.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-08 15:34:58.000000 blackjax-1.2.1/.github/workflows/build_documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-08 15:34:58.000000 blackjax-1.2.1/.github/workflows/nightly.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-08 15:34:58.000000 blackjax-1.2.1/.github/workflows/publish_documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-08 15:34:58.000000 blackjax-1.2.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-08 15:34:58.000000 blackjax-1.2.1/.github/workflows/schedule-meeting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-08 15:34:58.000000 blackjax-1.2.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-08 15:34:58.000000 blackjax-1.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-08 15:34:58.000000 blackjax-1.2.1/.gitlint
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-08 15:34:58.000000 blackjax-1.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-08 15:34:58.000000 blackjax-1.2.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-05-08 15:34:58.000000 blackjax-1.2.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-05-08 15:34:58.000000 blackjax-1.2.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-05-08 15:34:58.000000 blackjax-1.2.1/GOVERNANCE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11354 2024-05-08 15:34:58.000000 blackjax-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-08 15:34:58.000000 blackjax-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-08 15:34:58.000000 blackjax-1.2.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-05-08 15:35:03.245586 blackjax-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-05-08 15:34:58.000000 blackjax-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:35:03.217586 blackjax-1.2.1/blackjax/
+-rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-08 15:35:03.000000 blackjax-1.2.1/blackjax/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:35:03.221586 blackjax-1.2.1/blackjax/adaptation/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/adaptation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/adaptation/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17121 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/adaptation/chees_adaptation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7640 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/adaptation/mass_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10236 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/adaptation/mclmc_adaptation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10582 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/adaptation/meads_adaptation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7576 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/adaptation/pathfinder_adaptation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9557 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/adaptation/step_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16440 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/adaptation/window_adaptation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7915 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/diagnostics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:35:03.225586 blackjax-1.2.1/blackjax/mcmc/
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/mcmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8885 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/mcmc/barker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/mcmc/diffusions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6891 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/mcmc/dynamic_hmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9133 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/mcmc/elliptical_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10649 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/mcmc/ghmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11017 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/mcmc/hmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16461 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/mcmc/integrators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/mcmc/mala.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8430 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/mcmc/marginal_latent_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/mcmc/mclmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11000 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/mcmc/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11050 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/mcmc/nuts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11963 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/mcmc/periodic_orbital.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8596 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/mcmc/proposal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15645 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/mcmc/random_walk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/mcmc/rmhmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/mcmc/termination.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22915 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/mcmc/trajectory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:35:03.225586 blackjax-1.2.1/blackjax/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/optimizers/dual_averaging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11581 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/optimizers/lbfgs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/progress_bar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:35:03.225586 blackjax-1.2.1/blackjax/sgmcmc/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/sgmcmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8691 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/sgmcmc/csgld.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/sgmcmc/diffusions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/sgmcmc/gradients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/sgmcmc/sghmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/sgmcmc/sgld.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/sgmcmc/sgnht.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:35:03.229586 blackjax-1.2.1/blackjax/smc/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/smc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5311 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/smc/adaptive_tempered.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5535 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/smc/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/smc/ess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/smc/inner_kernel_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/smc/resampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/smc/solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/smc/tempered.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:35:03.229586 blackjax-1.2.1/blackjax/smc/tuning/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/smc/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/smc/tuning/from_kernel_info.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1368 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/smc/tuning/from_particles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7311 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:35:03.229586 blackjax-1.2.1/blackjax/vi/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/vi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5386 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/vi/meanfield_vi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8871 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/vi/pathfinder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7101 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/vi/schrodinger_follmer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5494 2024-05-08 15:34:58.000000 blackjax-1.2.1/blackjax/vi/svgd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:35:03.245586 blackjax-1.2.1/blackjax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-05-08 15:35:03.000000 blackjax-1.2.1/blackjax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4227 2024-05-08 15:35:03.000000 blackjax-1.2.1/blackjax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:35:03.000000 blackjax-1.2.1/blackjax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-08 15:35:03.000000 blackjax-1.2.1/blackjax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-08 15:35:03.000000 blackjax-1.2.1/blackjax.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-08 15:34:58.000000 blackjax-1.2.1/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:35:03.229586 blackjax-1.2.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:35:03.229586 blackjax-1.2.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)   161829 2024-05-08 15:34:58.000000 blackjax-1.2.1/docs/_static/blackjax.png
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-08 15:34:58.000000 blackjax-1.2.1/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-08 15:34:58.000000 blackjax-1.2.1/docs/bib.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-05-08 15:34:58.000000 blackjax-1.2.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:35:03.233586 blackjax-1.2.1/docs/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:35:03.237586 blackjax-1.2.1/docs/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-05-08 15:34:58.000000 blackjax-1.2.1/docs/examples/data/blackjax.png
+-rw-r--r--   0 runner    (1001) docker     (127)    63251 2024-05-08 15:34:58.000000 blackjax-1.2.1/docs/examples/data/google.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     6030 2024-05-08 15:34:58.000000 blackjax-1.2.1/docs/examples/howto_custom_gradients.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12029 2024-05-08 15:34:58.000000 blackjax-1.2.1/docs/examples/howto_metropolis_within_gibbs.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-05-08 15:34:58.000000 blackjax-1.2.1/docs/examples/howto_other_frameworks.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5494 2024-05-08 15:34:58.000000 blackjax-1.2.1/docs/examples/howto_reproduce_the_blackjax_image.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9833 2024-05-08 15:34:58.000000 blackjax-1.2.1/docs/examples/howto_sample_multiple_chains.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-05-08 15:34:58.000000 blackjax-1.2.1/docs/examples/howto_use_aesara.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-05-08 15:34:58.000000 blackjax-1.2.1/docs/examples/howto_use_numpyro.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6122 2024-05-08 15:34:58.000000 blackjax-1.2.1/docs/examples/howto_use_oryx.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-05-08 15:34:58.000000 blackjax-1.2.1/docs/examples/howto_use_pymc.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-05-08 15:34:58.000000 blackjax-1.2.1/docs/examples/howto_use_tfp.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-05-08 15:34:58.000000 blackjax-1.2.1/docs/examples/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (127)  4461357 2024-05-08 15:34:58.000000 blackjax-1.2.1/docs/examples/scatter.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-05-08 15:34:58.000000 blackjax-1.2.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13273 2024-05-08 15:34:58.000000 blackjax-1.2.1/docs/refs.bib
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-08 15:34:58.000000 blackjax-1.2.1/jupytex.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-08 15:34:58.000000 blackjax-1.2.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-08 15:34:58.000000 blackjax-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-08 15:34:58.000000 blackjax-1.2.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-08 15:34:58.000000 blackjax-1.2.1/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-08 15:34:58.000000 blackjax-1.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-08 15:35:03.245586 blackjax-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:35:03.237586 blackjax-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:34:58.000000 blackjax-1.2.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:35:03.237586 blackjax-1.2.1/tests/adaptation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:34:58.000000 blackjax-1.2.1/tests/adaptation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-08 15:34:58.000000 blackjax-1.2.1/tests/adaptation/test_adaptation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-08 15:34:58.000000 blackjax-1.2.1/tests/adaptation/test_mass_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-08 15:34:58.000000 blackjax-1.2.1/tests/adaptation/test_step_size.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:35:03.241586 blackjax-1.2.1/tests/mcmc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:34:58.000000 blackjax-1.2.1/tests/mcmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-08 15:34:58.000000 blackjax-1.2.1/tests/mcmc/test_barker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13030 2024-05-08 15:34:58.000000 blackjax-1.2.1/tests/mcmc/test_integrators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-05-08 15:34:58.000000 blackjax-1.2.1/tests/mcmc/test_latent_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-05-08 15:34:58.000000 blackjax-1.2.1/tests/mcmc/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-08 15:34:58.000000 blackjax-1.2.1/tests/mcmc/test_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-05-08 15:34:58.000000 blackjax-1.2.1/tests/mcmc/test_random_walk_without_chex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29756 2024-05-08 15:34:58.000000 blackjax-1.2.1/tests/mcmc/test_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10911 2024-05-08 15:34:58.000000 blackjax-1.2.1/tests/mcmc/test_trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-08 15:34:58.000000 blackjax-1.2.1/tests/mcmc/test_uturn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:35:03.241586 blackjax-1.2.1/tests/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:34:58.000000 blackjax-1.2.1/tests/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-05-08 15:34:58.000000 blackjax-1.2.1/tests/optimizers/test_optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-08 15:34:58.000000 blackjax-1.2.1/tests/optimizers/test_pathfinder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:35:03.241586 blackjax-1.2.1/tests/smc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-08 15:34:58.000000 blackjax-1.2.1/tests/smc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13930 2024-05-08 15:34:58.000000 blackjax-1.2.1/tests/smc/test_inner_kernel_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-08 15:34:58.000000 blackjax-1.2.1/tests/smc/test_kernel_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-08 15:34:58.000000 blackjax-1.2.1/tests/smc/test_resampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-05-08 15:34:58.000000 blackjax-1.2.1/tests/smc/test_smc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-05-08 15:34:58.000000 blackjax-1.2.1/tests/smc/test_smc_ess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-08 15:34:58.000000 blackjax-1.2.1/tests/smc/test_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6852 2024-05-08 15:34:58.000000 blackjax-1.2.1/tests/smc/test_tempered_smc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-05-08 15:34:58.000000 blackjax-1.2.1/tests/test_benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-05-08 15:34:58.000000 blackjax-1.2.1/tests/test_compilation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-08 15:34:58.000000 blackjax-1.2.1/tests/test_diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-08 15:34:58.000000 blackjax-1.2.1/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:35:03.241586 blackjax-1.2.1/tests/vi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:34:58.000000 blackjax-1.2.1/tests/vi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-08 15:34:58.000000 blackjax-1.2.1/tests/vi/test_meanfield_vi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-05-08 15:34:58.000000 blackjax-1.2.1/tests/vi/test_schrodinger_follmer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-05-08 15:34:58.000000 blackjax-1.2.1/tests/vi/test_svgd.py
```

### Comparing `blackjax-1.2.0/.github/ISSUE_TEMPLATE/bug_report.yml` & `blackjax-1.2.1/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/.github/ISSUE_TEMPLATE/enhancement.md` & `blackjax-1.2.1/.github/ISSUE_TEMPLATE/enhancement.md`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/.github/ISSUE_TEMPLATE/meeting.md` & `blackjax-1.2.1/.github/ISSUE_TEMPLATE/meeting.md`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/.github/ISSUE_TEMPLATE/sampler_proposal.md` & `blackjax-1.2.1/.github/ISSUE_TEMPLATE/sampler_proposal.md`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/.github/PULL_REQUEST_TEMPLATE.md` & `blackjax-1.2.1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/.github/workflows/benchmark.yml` & `blackjax-1.2.1/.github/workflows/benchmark.yml`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/.github/workflows/build_documentation.yml` & `blackjax-1.2.1/.github/workflows/build_documentation.yml`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/.github/workflows/nightly.yml` & `blackjax-1.2.1/.github/workflows/nightly.yml`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/.github/workflows/publish_documentation.yml` & `blackjax-1.2.1/.github/workflows/publish_documentation.yml`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/.github/workflows/release.yml` & `blackjax-1.2.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/.github/workflows/test.yml` & `blackjax-1.2.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/.gitignore` & `blackjax-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/.gitlint` & `blackjax-1.2.1/.gitlint`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/.pre-commit-config.yaml` & `blackjax-1.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/CODE_OF_CONDUCT.md` & `blackjax-1.2.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/CONTRIBUTING.md` & `blackjax-1.2.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/GOVERNANCE.md` & `blackjax-1.2.1/GOVERNANCE.md`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/LICENSE` & `blackjax-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/Makefile` & `blackjax-1.2.1/Makefile`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/PKG-INFO` & `blackjax-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackjax
-Version: 1.2.0
+Version: 1.2.1
 Summary: Flexible and fast sampling in Python
 Author-email: The Blackjax team <remi@thetypicalset.com>
 License: Apache License 2.0
 Project-URL: homepage, https://github.com/blackjax-devs/blackjax
 Project-URL: documentation, https://blackjax-devs.github.io/blackjax/
 Project-URL: repository, https://github.com/blackjax-devs/blackjax
 Keywords: probability,machine learning,statistics,mcmc,sampling
```

### Comparing `blackjax-1.2.0/README.md` & `blackjax-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax/__init__.py` & `blackjax-1.2.1/blackjax/__init__.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax/adaptation/base.py` & `blackjax-1.2.1/blackjax/adaptation/base.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax/adaptation/chees_adaptation.py` & `blackjax-1.2.1/blackjax/adaptation/chees_adaptation.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax/adaptation/mass_matrix.py` & `blackjax-1.2.1/blackjax/adaptation/mass_matrix.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax/adaptation/mclmc_adaptation.py` & `blackjax-1.2.1/blackjax/adaptation/mclmc_adaptation.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax/adaptation/meads_adaptation.py` & `blackjax-1.2.1/blackjax/adaptation/meads_adaptation.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax/adaptation/pathfinder_adaptation.py` & `blackjax-1.2.1/blackjax/adaptation/pathfinder_adaptation.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax/adaptation/step_size.py` & `blackjax-1.2.1/blackjax/adaptation/step_size.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax/adaptation/window_adaptation.py` & `blackjax-1.2.1/blackjax/adaptation/window_adaptation.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax/base.py` & `blackjax-1.2.1/blackjax/base.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax/diagnostics.py` & `blackjax-1.2.1/blackjax/diagnostics.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax/mcmc/barker.py` & `blackjax-1.2.1/blackjax/mcmc/barker.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax/mcmc/diffusions.py` & `blackjax-1.2.1/blackjax/mcmc/diffusions.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax/mcmc/dynamic_hmc.py` & `blackjax-1.2.1/blackjax/mcmc/dynamic_hmc.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax/mcmc/elliptical_slice.py` & `blackjax-1.2.1/blackjax/mcmc/elliptical_slice.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax/mcmc/ghmc.py` & `blackjax-1.2.1/blackjax/mcmc/ghmc.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax/mcmc/hmc.py` & `blackjax-1.2.1/blackjax/mcmc/hmc.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax/mcmc/integrators.py` & `blackjax-1.2.1/blackjax/mcmc/integrators.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax/mcmc/mala.py` & `blackjax-1.2.1/blackjax/mcmc/mala.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax/mcmc/marginal_latent_gaussian.py` & `blackjax-1.2.1/blackjax/mcmc/marginal_latent_gaussian.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax/mcmc/mclmc.py` & `blackjax-1.2.1/blackjax/mcmc/mclmc.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax/mcmc/metrics.py` & `blackjax-1.2.1/blackjax/mcmc/metrics.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax/mcmc/nuts.py` & `blackjax-1.2.1/blackjax/mcmc/nuts.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax/mcmc/periodic_orbital.py` & `blackjax-1.2.1/blackjax/mcmc/periodic_orbital.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax/mcmc/proposal.py` & `blackjax-1.2.1/blackjax/mcmc/proposal.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,15 +149,15 @@
 ) -> Proposal:
     """Baised proposal sampling :cite:p:`betancourt2017conceptual`.
 
     Unlike uniform sampling, biased sampling favors new proposals. It thus
     biases the transition away from the trajectory's initial state.
 
     """
-    p_accept = jnp.clip(jnp.exp(new_proposal.weight - proposal.weight), a_max=1)
+    p_accept = jnp.clip(jnp.exp(new_proposal.weight - proposal.weight), max=1)
     do_accept = jax.random.bernoulli(rng_key, p_accept)
     new_weight = jnp.logaddexp(proposal.weight, new_proposal.weight)
     new_sum_log_p_accept = jnp.logaddexp(
         proposal.sum_log_p_accept, new_proposal.sum_log_p_accept
     )
 
     return jax.lax.cond(
@@ -220,15 +220,15 @@
 
     In the static setting, the probability with which the new proposal is
     accepted is a function of the difference in energy between the previous and
     the current states. If the current energy is lower than the previous one
     then the new proposal is accepted with probability 1.
 
     """
-    p_accept = jnp.clip(jnp.exp(log_p_accept), a_max=1)
+    p_accept = jnp.clip(jnp.exp(log_p_accept), max=1)
     do_accept = jax.random.bernoulli(rng_key, p_accept)
     info = do_accept, p_accept, None
     return (
         jax.lax.cond(
             do_accept,
             lambda _: new_proposal,
             lambda _: proposal,
@@ -249,15 +249,15 @@
     """Slice sampling for non-reversible Metropolis-Hasting update.
 
     Performs a non-reversible update of a uniform [0, 1] value
     for Metropolis-Hastings accept/reject decisions :cite:p:`neal2020non`, in addition
     to the accept/reject step of a current state and new proposal.
 
     """
-    p_accept = jnp.clip(jnp.exp(delta_energy), a_max=1)
+    p_accept = jnp.clip(jnp.exp(delta_energy), max=1)
     do_accept = jnp.log(jnp.abs(slice)) <= delta_energy
     slice_next = slice * (jnp.exp(-delta_energy) * do_accept + (1 - do_accept))
     info = do_accept, p_accept, slice_next
     return (
         jax.lax.cond(
             do_accept,
             lambda _: new_proposal,
```

### Comparing `blackjax-1.2.0/blackjax/mcmc/random_walk.py` & `blackjax-1.2.1/blackjax/mcmc/random_walk.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax/mcmc/rmhmc.py` & `blackjax-1.2.1/blackjax/mcmc/rmhmc.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax/mcmc/termination.py` & `blackjax-1.2.1/blackjax/mcmc/termination.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax/mcmc/trajectory.py` & `blackjax-1.2.1/blackjax/mcmc/trajectory.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax/optimizers/dual_averaging.py` & `blackjax-1.2.1/blackjax/optimizers/dual_averaging.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax/optimizers/lbfgs.py` & `blackjax-1.2.1/blackjax/optimizers/lbfgs.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax/progress_bar.py` & `blackjax-1.2.1/blackjax/progress_bar.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax/sgmcmc/csgld.py` & `blackjax-1.2.1/blackjax/sgmcmc/csgld.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax/sgmcmc/diffusions.py` & `blackjax-1.2.1/blackjax/sgmcmc/diffusions.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax/sgmcmc/gradients.py` & `blackjax-1.2.1/blackjax/sgmcmc/gradients.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax/sgmcmc/sghmc.py` & `blackjax-1.2.1/blackjax/sgmcmc/sghmc.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax/sgmcmc/sgld.py` & `blackjax-1.2.1/blackjax/sgmcmc/sgld.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax/sgmcmc/sgnht.py` & `blackjax-1.2.1/blackjax/sgmcmc/sgnht.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax/smc/adaptive_tempered.py` & `blackjax-1.2.1/blackjax/smc/adaptive_tempered.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax/smc/base.py` & `blackjax-1.2.1/blackjax/smc/base.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax/smc/ess.py` & `blackjax-1.2.1/blackjax/smc/ess.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax/smc/inner_kernel_tuning.py` & `blackjax-1.2.1/blackjax/smc/inner_kernel_tuning.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax/smc/resampling.py` & `blackjax-1.2.1/blackjax/smc/resampling.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax/smc/solver.py` & `blackjax-1.2.1/blackjax/smc/solver.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax/smc/tempered.py` & `blackjax-1.2.1/blackjax/smc/tempered.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax/smc/tuning/from_kernel_info.py` & `blackjax-1.2.1/blackjax/smc/tuning/from_kernel_info.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax/smc/tuning/from_particles.py` & `blackjax-1.2.1/blackjax/smc/tuning/from_particles.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax/types.py` & `blackjax-1.2.1/blackjax/types.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax/util.py` & `blackjax-1.2.1/blackjax/util.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax/vi/meanfield_vi.py` & `blackjax-1.2.1/blackjax/vi/meanfield_vi.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax/vi/pathfinder.py` & `blackjax-1.2.1/blackjax/vi/pathfinder.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax/vi/schrodinger_follmer.py` & `blackjax-1.2.1/blackjax/vi/schrodinger_follmer.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax/vi/svgd.py` & `blackjax-1.2.1/blackjax/vi/svgd.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/blackjax.egg-info/PKG-INFO` & `blackjax-1.2.1/blackjax.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackjax
-Version: 1.2.0
+Version: 1.2.1
 Summary: Flexible and fast sampling in Python
 Author-email: The Blackjax team <remi@thetypicalset.com>
 License: Apache License 2.0
 Project-URL: homepage, https://github.com/blackjax-devs/blackjax
 Project-URL: documentation, https://blackjax-devs.github.io/blackjax/
 Project-URL: repository, https://github.com/blackjax-devs/blackjax
 Keywords: probability,machine learning,statistics,mcmc,sampling
```

### Comparing `blackjax-1.2.0/blackjax.egg-info/SOURCES.txt` & `blackjax-1.2.1/blackjax.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/docs/_static/blackjax.png` & `blackjax-1.2.1/docs/_static/blackjax.png`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/docs/conf.py` & `blackjax-1.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/docs/examples/data/blackjax.png` & `blackjax-1.2.1/docs/examples/data/blackjax.png`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/docs/examples/data/google.csv` & `blackjax-1.2.1/docs/examples/data/google.csv`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/docs/examples/howto_custom_gradients.md` & `blackjax-1.2.1/docs/examples/howto_custom_gradients.md`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/docs/examples/howto_metropolis_within_gibbs.md` & `blackjax-1.2.1/docs/examples/howto_metropolis_within_gibbs.md`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/docs/examples/howto_other_frameworks.md` & `blackjax-1.2.1/docs/examples/howto_other_frameworks.md`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/docs/examples/howto_reproduce_the_blackjax_image.md` & `blackjax-1.2.1/docs/examples/howto_reproduce_the_blackjax_image.md`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/docs/examples/howto_sample_multiple_chains.md` & `blackjax-1.2.1/docs/examples/howto_sample_multiple_chains.md`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/docs/examples/howto_use_aesara.md` & `blackjax-1.2.1/docs/examples/howto_use_aesara.md`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/docs/examples/howto_use_numpyro.md` & `blackjax-1.2.1/docs/examples/howto_use_numpyro.md`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/docs/examples/howto_use_oryx.md` & `blackjax-1.2.1/docs/examples/howto_use_oryx.md`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/docs/examples/howto_use_pymc.md` & `blackjax-1.2.1/docs/examples/howto_use_pymc.md`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/docs/examples/howto_use_tfp.md` & `blackjax-1.2.1/docs/examples/howto_use_tfp.md`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/docs/examples/quickstart.md` & `blackjax-1.2.1/docs/examples/quickstart.md`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/docs/examples/scatter.gif` & `blackjax-1.2.1/docs/examples/scatter.gif`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/docs/index.md` & `blackjax-1.2.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/docs/refs.bib` & `blackjax-1.2.1/docs/refs.bib`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/pyproject.toml` & `blackjax-1.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/tests/adaptation/test_adaptation.py` & `blackjax-1.2.1/tests/adaptation/test_adaptation.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/tests/adaptation/test_mass_matrix.py` & `blackjax-1.2.1/tests/adaptation/test_mass_matrix.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/tests/adaptation/test_step_size.py` & `blackjax-1.2.1/tests/adaptation/test_step_size.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/tests/mcmc/test_barker.py` & `blackjax-1.2.1/tests/mcmc/test_barker.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/tests/mcmc/test_integrators.py` & `blackjax-1.2.1/tests/mcmc/test_integrators.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/tests/mcmc/test_latent_gaussian.py` & `blackjax-1.2.1/tests/mcmc/test_latent_gaussian.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/tests/mcmc/test_metrics.py` & `blackjax-1.2.1/tests/mcmc/test_metrics.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/tests/mcmc/test_proposal.py` & `blackjax-1.2.1/tests/mcmc/test_proposal.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/tests/mcmc/test_random_walk_without_chex.py` & `blackjax-1.2.1/tests/mcmc/test_random_walk_without_chex.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/tests/mcmc/test_sampling.py` & `blackjax-1.2.1/tests/mcmc/test_sampling.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/tests/mcmc/test_trajectory.py` & `blackjax-1.2.1/tests/mcmc/test_trajectory.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/tests/mcmc/test_uturn.py` & `blackjax-1.2.1/tests/mcmc/test_uturn.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/tests/optimizers/test_optimizers.py` & `blackjax-1.2.1/tests/optimizers/test_optimizers.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/tests/optimizers/test_pathfinder.py` & `blackjax-1.2.1/tests/optimizers/test_pathfinder.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/tests/smc/__init__.py` & `blackjax-1.2.1/tests/smc/__init__.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/tests/smc/test_inner_kernel_tuning.py` & `blackjax-1.2.1/tests/smc/test_inner_kernel_tuning.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/tests/smc/test_kernel_compatibility.py` & `blackjax-1.2.1/tests/smc/test_kernel_compatibility.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/tests/smc/test_resampling.py` & `blackjax-1.2.1/tests/smc/test_resampling.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/tests/smc/test_smc.py` & `blackjax-1.2.1/tests/smc/test_smc.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/tests/smc/test_smc_ess.py` & `blackjax-1.2.1/tests/smc/test_smc_ess.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/tests/smc/test_solver.py` & `blackjax-1.2.1/tests/smc/test_solver.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/tests/smc/test_tempered_smc.py` & `blackjax-1.2.1/tests/smc/test_tempered_smc.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/tests/test_benchmarks.py` & `blackjax-1.2.1/tests/test_benchmarks.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/tests/test_compilation.py` & `blackjax-1.2.1/tests/test_compilation.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/tests/test_diagnostics.py` & `blackjax-1.2.1/tests/test_diagnostics.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/tests/test_util.py` & `blackjax-1.2.1/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/tests/vi/test_meanfield_vi.py` & `blackjax-1.2.1/tests/vi/test_meanfield_vi.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/tests/vi/test_schrodinger_follmer.py` & `blackjax-1.2.1/tests/vi/test_schrodinger_follmer.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.2.0/tests/vi/test_svgd.py` & `blackjax-1.2.1/tests/vi/test_svgd.py`

 * *Files identical despite different names*

