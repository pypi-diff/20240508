# Comparing `tmp/preliz-0.6.0.tar.gz` & `tmp/preliz-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "preliz-0.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "preliz-0.6.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `preliz-0.6.0.tar` & `preliz-0.6.1.tar`

### file list

```diff
@@ -1,102 +1,102 @@
--rw-r--r--   0        0        0     4324 2024-04-26 20:09:30.590731 preliz-0.6.0/README.md
--rw-r--r--   0        0        0      649 2024-04-26 20:09:30.646732 preliz-0.6.0/preliz/__init__.py
--rw-r--r--   0        0        0     2772 2024-04-26 20:09:30.646732 preliz-0.6.0/preliz/distributions/__init__.py
--rw-r--r--   0        0        0     6930 2024-04-26 20:09:30.646732 preliz-0.6.0/preliz/distributions/asymmetric_laplace.py
--rw-r--r--   0        0        0     5012 2024-04-26 20:09:30.646732 preliz-0.6.0/preliz/distributions/bernoulli.py
--rw-r--r--   0        0        0     7701 2024-04-26 20:09:30.646732 preliz-0.6.0/preliz/distributions/beta.py
--rw-r--r--   0        0        0     6721 2024-04-26 20:09:30.646732 preliz-0.6.0/preliz/distributions/betabinomial.py
--rw-r--r--   0        0        0     7062 2024-04-26 20:09:30.646732 preliz-0.6.0/preliz/distributions/betascaled.py
--rw-r--r--   0        0        0     5242 2024-04-26 20:09:30.646732 preliz-0.6.0/preliz/distributions/binomial.py
--rw-r--r--   0        0        0     4723 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/categorical.py
--rw-r--r--   0        0        0     4302 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/cauchy.py
--rw-r--r--   0        0        0     7488 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/censored.py
--rw-r--r--   0        0        0     4233 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/chi_squared.py
--rw-r--r--   0        0        0    21635 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/continuous_multivariate.py
--rw-r--r--   0        0        0     5071 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/discrete_uniform.py
--rw-r--r--   0        0        0     4942 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/discrete_weibull.py
--rw-r--r--   0        0        0    25352 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/distributions.py
--rw-r--r--   0        0        0     6516 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/distributions_multivariate.py
--rw-r--r--   0        0        0     5946 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/exgaussian.py
--rw-r--r--   0        0        0     4391 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/exponential.py
--rw-r--r--   0        0        0     5866 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/gamma.py
--rw-r--r--   0        0        0     3885 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/geometric.py
--rw-r--r--   0        0        0     4489 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/gumbel.py
--rw-r--r--   0        0        0     3920 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/halfcauchy.py
--rw-r--r--   0        0        0     4920 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/halfnormal.py
--rw-r--r--   0        0        0     7938 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/halfstudentt.py
--rw-r--r--   0        0        0     5386 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/hurdle.py
--rw-r--r--   0        0        0     6141 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/hypergeometric.py
--rw-r--r--   0        0        0     6452 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/inversegamma.py
--rw-r--r--   0        0        0     4798 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/kumaraswamy.py
--rw-r--r--   0        0        0     4061 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/laplace.py
--rw-r--r--   0        0        0     3862 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/logistic.py
--rw-r--r--   0        0        0     5742 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/logitnormal.py
--rw-r--r--   0        0        0     5013 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/lognormal.py
--rw-r--r--   0        0        0     4710 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/moyal.py
--rw-r--r--   0        0        0     6033 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/negativebinomial.py
--rw-r--r--   0        0        0     5017 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/normal.py
--rw-r--r--   0        0        0     5067 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/pareto.py
--rw-r--r--   0        0        0     4194 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/poisson.py
--rw-r--r--   0        0        0     5851 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/rice.py
--rw-r--r--   0        0        0     6212 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/skewnormal.py
--rw-r--r--   0        0        0     7610 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/studentt.py
--rw-r--r--   0        0        0     6875 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/triangular.py
--rw-r--r--   0        0        0     5680 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/truncated.py
--rw-r--r--   0        0        0    14611 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/truncatednormal.py
--rw-r--r--   0        0        0     4692 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/uniform.py
--rw-r--r--   0        0        0     4987 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/vonmises.py
--rw-r--r--   0        0        0     5665 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/wald.py
--rw-r--r--   0        0        0     5068 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/weibull.py
--rw-r--r--   0        0        0     5560 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/zi_binomial.py
--rw-r--r--   0        0        0     7223 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/zi_negativebinomial.py
--rw-r--r--   0        0        0     5667 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/zi_poisson.py
--rw-r--r--   0        0        0       64 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/internal/__init__.py
--rw-r--r--   0        0        0     4540 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/internal/distribution_helper.py
--rw-r--r--   0        0        0    13819 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/internal/optimization.py
--rw-r--r--   0        0        0     5596 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/internal/parser.py
--rw-r--r--   0        0        0    19087 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/internal/plot_helper.py
--rw-r--r--   0        0        0     9785 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/internal/plot_helper_multivariate.py
--rw-r--r--   0        0        0     2028 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/internal/predictive_helper.py
--rw-r--r--   0        0        0    11863 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/internal/special.py
--rw-r--r--   0        0        0     6465 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/ppls/pymc_io.py
--rw-r--r--   0        0        0      145 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/predictive/__init__.py
--rw-r--r--   0        0        0    14606 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/predictive/ppa.py
--rw-r--r--   0        0        0     2251 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/predictive/ppe.py
--rw-r--r--   0        0        0     2160 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/predictive/predictive_explorer.py
--rw-r--r--   0        0        0     1946 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/tests/check_inside_notebook.ipynb
--rw-r--r--   0        0        0     1787 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/tests/plot_interactive.ipynb
--rw-r--r--   0        0        0   477854 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/tests/ppa.ipynb
--rw-r--r--   0        0        0     2787 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/tests/predictive_explorer.ipynb
--rw-r--r--   0        0        0     1439 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/tests/quartile_int.ipynb
--rw-r--r--   0        0        0     1472 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/tests/roulette.ipynb
--rw-r--r--   0        0        0      661 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/tests/test_beta_mode.py
--rw-r--r--   0        0        0     1967 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/tests/test_censored.py
--rw-r--r--   0        0        0      757 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/tests/test_dirichlet_mode.py
--rw-r--r--   0        0        0     1144 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/tests/test_discrete_weibull.py
--rw-r--r--   0        0        0     7265 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/tests/test_distributions.py
--rw-r--r--   0        0        0      346 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/tests/test_distributions_helper.py
--rw-r--r--   0        0        0      626 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/tests/test_helper.py
--rw-r--r--   0        0        0     2292 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/tests/test_hurdle.py
--rw-r--r--   0        0        0      338 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/tests/test_internals.py
--rw-r--r--   0        0        0     6654 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/tests/test_maxent.py
--rw-r--r--   0        0        0     2919 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/tests/test_mle.py
--rw-r--r--   0        0        0      987 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/tests/test_optimization.py
--rw-r--r--   0        0        0     6153 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/tests/test_plots.py
--rw-r--r--   0        0        0       85 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/tests/test_ppa.py
--rw-r--r--   0        0        0      117 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/tests/test_predictive_explorer.py
--rw-r--r--   0        0        0     3475 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/tests/test_quartile.py
--rw-r--r--   0        0        0      103 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/tests/test_quartile_int.py
--rw-r--r--   0        0        0      910 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/tests/test_roulette.py
--rw-r--r--   0        0        0    10795 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/tests/test_scipy.py
--rw-r--r--   0        0        0     1851 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/tests/test_special.py
--rw-r--r--   0        0        0     2568 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/tests/test_truncated.py
--rw-r--r--   0        0        0      325 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/unidimensional/__init__.py
--rw-r--r--   0        0        0     2244 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/unidimensional/beta_mode.py
--rw-r--r--   0        0        0     2341 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/unidimensional/dirichlet_mode.py
--rw-r--r--   0        0        0     4125 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/unidimensional/maxent.py
--rw-r--r--   0        0        0     1654 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/unidimensional/mle.py
--rw-r--r--   0        0        0     3259 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/unidimensional/quartile.py
--rw-r--r--   0        0        0     6136 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/unidimensional/quartile_int.py
--rw-r--r--   0        0        0    12994 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/unidimensional/roulette.py
--rw-r--r--   0        0        0     1410 2024-04-26 20:09:30.654732 preliz-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     5568 1970-01-01 00:00:00.000000 preliz-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     4324 2024-05-08 20:00:08.639523 preliz-0.6.1/README.md
+-rw-r--r--   0        0        0      649 2024-05-08 20:00:08.695523 preliz-0.6.1/preliz/__init__.py
+-rw-r--r--   0        0        0     2772 2024-05-08 20:00:08.695523 preliz-0.6.1/preliz/distributions/__init__.py
+-rw-r--r--   0        0        0     6930 2024-05-08 20:00:08.695523 preliz-0.6.1/preliz/distributions/asymmetric_laplace.py
+-rw-r--r--   0        0        0     4977 2024-05-08 20:00:08.695523 preliz-0.6.1/preliz/distributions/bernoulli.py
+-rw-r--r--   0        0        0     7804 2024-05-08 20:00:08.695523 preliz-0.6.1/preliz/distributions/beta.py
+-rw-r--r--   0        0        0     6721 2024-05-08 20:00:08.695523 preliz-0.6.1/preliz/distributions/betabinomial.py
+-rw-r--r--   0        0        0     7169 2024-05-08 20:00:08.695523 preliz-0.6.1/preliz/distributions/betascaled.py
+-rw-r--r--   0        0        0     5368 2024-05-08 20:00:08.695523 preliz-0.6.1/preliz/distributions/binomial.py
+-rw-r--r--   0        0        0     4730 2024-05-08 20:00:08.695523 preliz-0.6.1/preliz/distributions/categorical.py
+-rw-r--r--   0        0        0     4302 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/cauchy.py
+-rw-r--r--   0        0        0     7488 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/censored.py
+-rw-r--r--   0        0        0     4135 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/chi_squared.py
+-rw-r--r--   0        0        0    21635 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/continuous_multivariate.py
+-rw-r--r--   0        0        0     5071 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/discrete_uniform.py
+-rw-r--r--   0        0        0     4942 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/discrete_weibull.py
+-rw-r--r--   0        0        0    25870 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/distributions.py
+-rw-r--r--   0        0        0     6516 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/distributions_multivariate.py
+-rw-r--r--   0        0        0     5946 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/exgaussian.py
+-rw-r--r--   0        0        0     4397 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/exponential.py
+-rw-r--r--   0        0        0     5941 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/gamma.py
+-rw-r--r--   0        0        0     3987 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/geometric.py
+-rw-r--r--   0        0        0     4489 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/gumbel.py
+-rw-r--r--   0        0        0     3991 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/halfcauchy.py
+-rw-r--r--   0        0        0     4920 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/halfnormal.py
+-rw-r--r--   0        0        0     8033 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/halfstudentt.py
+-rw-r--r--   0        0        0     5386 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/hurdle.py
+-rw-r--r--   0        0        0     6141 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/hypergeometric.py
+-rw-r--r--   0        0        0     6527 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/inversegamma.py
+-rw-r--r--   0        0        0     4899 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/kumaraswamy.py
+-rw-r--r--   0        0        0     4061 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/laplace.py
+-rw-r--r--   0        0        0     3938 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/logistic.py
+-rw-r--r--   0        0        0     5742 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/logitnormal.py
+-rw-r--r--   0        0        0     5093 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/lognormal.py
+-rw-r--r--   0        0        0     4710 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/moyal.py
+-rw-r--r--   0        0        0     6104 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/negativebinomial.py
+-rw-r--r--   0        0        0     5017 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/normal.py
+-rw-r--r--   0        0        0     5070 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/pareto.py
+-rw-r--r--   0        0        0     4265 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/poisson.py
+-rw-r--r--   0        0        0     5851 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/rice.py
+-rw-r--r--   0        0        0     6212 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/skewnormal.py
+-rw-r--r--   0        0        0     7610 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/studentt.py
+-rw-r--r--   0        0        0     6875 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/triangular.py
+-rw-r--r--   0        0        0     5680 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/truncated.py
+-rw-r--r--   0        0        0    14719 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/truncatednormal.py
+-rw-r--r--   0        0        0     4692 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/uniform.py
+-rw-r--r--   0        0        0     4987 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/vonmises.py
+-rw-r--r--   0        0        0     5712 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/wald.py
+-rw-r--r--   0        0        0     5152 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/weibull.py
+-rw-r--r--   0        0        0     5601 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/zi_binomial.py
+-rw-r--r--   0        0        0     7262 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/zi_negativebinomial.py
+-rw-r--r--   0        0        0     5707 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/zi_poisson.py
+-rw-r--r--   0        0        0       64 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/internal/__init__.py
+-rw-r--r--   0        0        0     4602 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/internal/distribution_helper.py
+-rw-r--r--   0        0        0    13819 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/internal/optimization.py
+-rw-r--r--   0        0        0     5596 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/internal/parser.py
+-rw-r--r--   0        0        0    19087 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/internal/plot_helper.py
+-rw-r--r--   0        0        0     9785 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/internal/plot_helper_multivariate.py
+-rw-r--r--   0        0        0     2028 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/internal/predictive_helper.py
+-rw-r--r--   0        0        0    12000 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/internal/special.py
+-rw-r--r--   0        0        0     6565 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/ppls/pymc_io.py
+-rw-r--r--   0        0        0      145 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/predictive/__init__.py
+-rw-r--r--   0        0        0    14606 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/predictive/ppa.py
+-rw-r--r--   0        0        0     2251 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/predictive/ppe.py
+-rw-r--r--   0        0        0     2160 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/predictive/predictive_explorer.py
+-rw-r--r--   0        0        0     1946 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/tests/check_inside_notebook.ipynb
+-rw-r--r--   0        0        0     1787 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/tests/plot_interactive.ipynb
+-rw-r--r--   0        0        0   477854 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/tests/ppa.ipynb
+-rw-r--r--   0        0        0     2787 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/tests/predictive_explorer.ipynb
+-rw-r--r--   0        0        0     1439 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/tests/quartile_int.ipynb
+-rw-r--r--   0        0        0     1472 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/tests/roulette.ipynb
+-rw-r--r--   0        0        0      661 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/tests/test_beta_mode.py
+-rw-r--r--   0        0        0     1967 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/tests/test_censored.py
+-rw-r--r--   0        0        0      757 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/tests/test_dirichlet_mode.py
+-rw-r--r--   0        0        0     1144 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/tests/test_discrete_weibull.py
+-rw-r--r--   0        0        0     7265 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/tests/test_distributions.py
+-rw-r--r--   0        0        0      346 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/tests/test_distributions_helper.py
+-rw-r--r--   0        0        0      626 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/tests/test_helper.py
+-rw-r--r--   0        0        0     2292 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/tests/test_hurdle.py
+-rw-r--r--   0        0        0      338 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/tests/test_internals.py
+-rw-r--r--   0        0        0     6654 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/tests/test_maxent.py
+-rw-r--r--   0        0        0     2919 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/tests/test_mle.py
+-rw-r--r--   0        0        0      987 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/tests/test_optimization.py
+-rw-r--r--   0        0        0     6153 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/tests/test_plots.py
+-rw-r--r--   0        0        0       85 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/tests/test_ppa.py
+-rw-r--r--   0        0        0      117 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/tests/test_predictive_explorer.py
+-rw-r--r--   0        0        0     3475 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/tests/test_quartile.py
+-rw-r--r--   0        0        0      103 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/tests/test_quartile_int.py
+-rw-r--r--   0        0        0      910 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/tests/test_roulette.py
+-rw-r--r--   0        0        0    11083 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/tests/test_scipy.py
+-rw-r--r--   0        0        0     2287 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/tests/test_special.py
+-rw-r--r--   0        0        0     2568 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/tests/test_truncated.py
+-rw-r--r--   0        0        0      325 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/unidimensional/__init__.py
+-rw-r--r--   0        0        0     2244 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/unidimensional/beta_mode.py
+-rw-r--r--   0        0        0     2341 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/unidimensional/dirichlet_mode.py
+-rw-r--r--   0        0        0     4125 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/unidimensional/maxent.py
+-rw-r--r--   0        0        0     1654 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/unidimensional/mle.py
+-rw-r--r--   0        0        0     3259 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/unidimensional/quartile.py
+-rw-r--r--   0        0        0     6136 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/unidimensional/quartile_int.py
+-rw-r--r--   0        0        0    12994 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/unidimensional/roulette.py
+-rw-r--r--   0        0        0     1410 2024-05-08 20:00:08.703523 preliz-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     5568 1970-01-01 00:00:00.000000 preliz-0.6.1/PKG-INFO
```

### Comparing `preliz-0.6.0/README.md` & `preliz-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/__init__.py` & `preliz-0.6.1/preliz/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from .distributions import *
 from .predictive import *
 from .unidimensional import *
 
 
 __all__ = ["maxent", "mle", "ppa", "roulette", "quartile"]
 
-__version__ = "0.6.0"
+__version__ = "0.6.1"
 
 _log = logging.getLogger("preliz")
 
 if not logging.root.handlers:
     _log.setLevel(logging.INFO)
     if len(_log.handlers) == 0:
         handler = logging.StreamHandler()
```

### Comparing `preliz-0.6.0/preliz/distributions/__init__.py` & `preliz-0.6.1/preliz/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/distributions/asymmetric_laplace.py` & `preliz-0.6.1/preliz/distributions/asymmetric_laplace.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/distributions/bernoulli.py` & `preliz-0.6.1/preliz/distributions/bernoulli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # pylint: disable=attribute-defined-outside-init
 # pylint: disable=arguments-differ
 import numba as nb
 import numpy as np
-from scipy.special import logit, expit  # pylint: disable=no-name-in-module
 
 from .distributions import Discrete
 from ..internal.optimization import optimize_ml
 from ..internal.distribution_helper import eps, all_not_none
+from ..internal.special import xlogx, logit, expit
 
 
 class Bernoulli(Discrete):
     R"""Bernoulli distribution
 
     The Bernoulli distribution describes the probability of successes (x=1) and failures (x=0).
     The pmf of this distribution is
@@ -187,15 +187,15 @@
     else:
         return 0.0
 
 
 @nb.njit(cache=True)
 def nb_entropy(p):
     q = 1 - p
-    return -q * np.log(q) - p * np.log(p)
+    return -xlogx(q) - xlogx(p)
 
 
 @nb.vectorize(nopython=True, cache=True)
 def nb_logpdf(x, p):
     if x == 1:
         return np.log(p)
     elif x == 0:
```

### Comparing `preliz-0.6.0/preliz/distributions/beta.py` & `preliz-0.6.1/preliz/distributions/beta.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,16 @@
     betainc,
     betaincinv,
     digamma,
     gammaln,
     cdf_bounds,
     ppf_bounds_cont,
     mean_and_std,
+    xlogy,
+    xlog1py,
 )
 
 
 class Beta(Continuous):
     r"""
     Beta distribution.
 
@@ -244,16 +246,19 @@
         betaln(alpha, beta)
         - (alpha - 1) * digamma(alpha)
         - (beta - 1) * digamma(beta)
         + (psc - 2) * digamma(psc)
     )
 
 
-@nb.njit(cache=True)
+@nb.vectorize(nopython=True, cache=True)
 def nb_logpdf(x, alpha, beta):
-    beta_ = gammaln(alpha) + gammaln(beta) - gammaln(alpha + beta)
-    return (alpha - 1) * np.log(x) + (beta - 1) * np.log(1 - x) - beta_
+    if x < 0 or x > 1:
+        return -np.inf
+    else:
+        beta_ = gammaln(alpha) + gammaln(beta) - gammaln(alpha + beta)
+        return xlogy((alpha - 1), x) + xlog1py((beta - 1), -x) - beta_
 
 
 @nb.njit(cache=True)
 def nb_neg_logpdf(x, alpha, beta):
     return -(nb_logpdf(x, alpha, beta)).sum()
```

### Comparing `preliz-0.6.0/preliz/distributions/betabinomial.py` & `preliz-0.6.1/preliz/distributions/betabinomial.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/distributions/betascaled.py` & `preliz-0.6.1/preliz/distributions/betascaled.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from ..internal.special import (
     betaln,
     betainc,
     betaincinv,
     digamma,
     cdf_bounds,
     ppf_bounds_cont,
+    xlogy,
 )
 
 
 class BetaScaled(Continuous):
     r"""
     Scaled Beta distribution.
 
@@ -212,17 +213,20 @@
         - (alpha - 1) * digamma(alpha)
         - (beta - 1) * digamma(beta)
         + (psc - 2) * digamma(psc)
         + np.log(upper - lower)
     )
 
 
-@nb.njit(cache=True)
+@nb.vectorize(nopython=True, cache=True)
 def nb_logpdf(x, alpha, beta, lower, upper):
-    return ((alpha - 1) * np.log(x - lower) + (beta - 1) * np.log(upper - x)) - (
-        (alpha + beta - 1) * np.log(upper - lower) + betaln(alpha, beta)
-    )
+    if x < lower or x > upper:
+        return -np.inf
+    else:
+        return (xlogy((alpha - 1), (x - lower)) + xlogy((beta - 1), (upper - x))) - (
+            xlogy((alpha + beta - 1), (upper - lower)) + betaln(alpha, beta)
+        )
 
 
 @nb.njit(cache=True)
 def nb_neg_logpdf(x, alpha, beta, lower, upper):
     return -(nb_logpdf(x, alpha, beta, lower, upper)).sum()
```

### Comparing `preliz-0.6.0/preliz/distributions/binomial.py` & `preliz-0.6.1/preliz/distributions/binomial.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import numba as nb
 import numpy as np
 from scipy.special import bdtr, bdtrik  # pylint: disable=no-name-in-module
 
 from .distributions import Discrete
 from ..internal.optimization import optimize_moments
 from ..internal.distribution_helper import eps, all_not_none
-from ..internal.special import cdf_bounds, ppf_bounds_disc, gammaln, mean_and_std
+from ..internal.special import cdf_bounds, ppf_bounds_disc, gammaln, mean_and_std, xlogy, xlog1py
 
 
 class Binomial(Discrete):
     R"""
     Binomial distribution.
 
     The discrete probability distribution of the number of successes
@@ -80,15 +80,15 @@
         self._update(*nb_fit_mle(sample))
 
     def pdf(self, x):
         """
         Compute the probability density function (PDF) at a given point x.
         """
         x = np.asarray(x)
-        return np.exp(nb_logpdf(self.n, x, self.p))
+        return np.exp(self.logpdf(x))
 
     def cdf(self, x):
         """
         Compute the cumulative distribution function (CDF) at a given point x.
         """
         return nb_cdf(x, self.n, self.p, self.support[0], self.support[1])
 
@@ -98,21 +98,21 @@
         """
         return nb_ppf(q, self.n, self.p, self.support[0], self.support[1])
 
     def logpdf(self, x):
         """
         Compute the log probability density function (log PDF) at a given point x.
         """
-        return nb_logpdf(self.n, x, self.p)
+        return nb_logpdf(x, self.n, self.p)
 
     def _neg_logpdf(self, x):
         """
         Compute the neg log_pdf sum for the array x.
         """
-        return nb_neg_logpdf(self.n, x, self.p)
+        return nb_neg_logpdf(x, self.n, self.p)
 
     def entropy(self):
         return nb_entropy(self.n, self.p)
 
     def mean(self):
         return self.n * self.p
 
@@ -172,20 +172,25 @@
     x_bar, x_std = mean_and_std(sample)
     x_max = np.max(sample)
     n = np.ceil(x_max ** (1.5) * x_std / (x_bar**0.5 * (x_max - x_bar) ** 0.5))
     p = x_bar / n
     return n, p
 
 
-@nb.njit(cache=True)
-def nb_logpdf(n, y, p):
-    return (
-        gammaln(n + 1)
-        - (gammaln(y + 1) + gammaln(n - y + 1))
-        + y * np.log(p)
-        + (n - y) * np.log1p(-p)
-    )
+@nb.vectorize(nopython=True, cache=True)
+def nb_logpdf(x, n, p):
+    if x < 0:
+        return -np.inf
+    elif x > n:
+        return -np.inf
+    else:
+        return (
+            gammaln(n + 1)
+            - (gammaln(x + 1) + gammaln(n - x + 1))
+            + xlogy(x, p)
+            + xlog1py(n - x, -p)
+        )
 
 
 @nb.njit(cache=True)
-def nb_neg_logpdf(n, y, p):
-    return -(nb_logpdf(n, y, p)).sum()
+def nb_neg_logpdf(x, n, p):
+    return -(nb_logpdf(x, n, p)).sum()
```

### Comparing `preliz-0.6.0/preliz/distributions/categorical.py` & `preliz-0.6.1/preliz/distributions/categorical.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # pylint: disable=attribute-defined-outside-init
 # pylint: disable=arguments-differ
 import numba as nb
 import numpy as np
-from scipy.special import expit, logit
 
 from .distributions import Discrete
 from ..internal.distribution_helper import all_not_none, eps
 from ..internal.optimization import optimize_ml
+from ..internal.special import xlogx, expit, logit
 
 
 class Categorical(Discrete):
     R"""
     Categorical distribution.
 
     The most general discrete distribution. The pmf of this distribution is
@@ -166,15 +166,15 @@
 def nb_ppf(q, p):
     cumsum = np.cumsum(p)
     return np.searchsorted(cumsum, q)
 
 
 @nb.njit(cache=True)
 def nb_entropy(p):
-    return -np.sum(p * np.log(p))
+    return -np.sum(xlogx(p))
 
 
 def nb_logpdf(x, p):
     log_pmf = np.full_like(x, -np.inf, dtype=float)
     valid_categories = np.where((x >= 0) & (x < len(p)))[0]
     log_pmf[valid_categories] = np.log(p[x[valid_categories]])
     return log_pmf
```

### Comparing `preliz-0.6.0/preliz/distributions/cauchy.py` & `preliz-0.6.1/preliz/distributions/cauchy.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/distributions/censored.py` & `preliz-0.6.1/preliz/distributions/censored.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/distributions/chi_squared.py` & `preliz-0.6.1/preliz/distributions/chi_squared.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import numpy as np
 import numba as nb
 
 from scipy.special import gammainc, gammaincinv  # pylint: disable=no-name-in-module
 
 from .distributions import Continuous
 from ..internal.distribution_helper import eps, all_not_none
-from ..internal.special import cdf_bounds, ppf_bounds_cont, gammaln, digamma
+from ..internal.special import cdf_bounds, ppf_bounds_cont, gammaln, digamma, xlogy
 from ..internal.optimization import optimize_ml
 
 
 class ChiSquared(Continuous):
     r"""
     Chi squared  distribution.
 
@@ -146,21 +146,16 @@
     return ppf_bounds_cont(vals, q, 0, np.inf)
 
 
 @nb.vectorize(nopython=True, cache=True)
 def nb_logpdf(x, nu):
     if x < 0:
         return -np.inf
-    elif x == 0:
-        if nu < 2:
-            return np.inf
-        else:
-            return -np.inf
     else:
-        return (nu / 2 - 1) * np.log(x) - x / 2 - nu / 2 * np.log(2) - gammaln(nu / 2)
+        return xlogy(nu / 2 - 1, x) - x / 2 - gammaln(nu / 2) - (nu * np.log(2)) / 2
 
 
 @nb.njit(cache=True)
 def nb_neg_logpdf(x, lam):
     return (-nb_logpdf(x, lam)).sum()
```

### Comparing `preliz-0.6.0/preliz/distributions/continuous_multivariate.py` & `preliz-0.6.1/preliz/distributions/continuous_multivariate.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/distributions/discrete_uniform.py` & `preliz-0.6.1/preliz/distributions/discrete_uniform.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/distributions/discrete_weibull.py` & `preliz-0.6.1/preliz/distributions/discrete_weibull.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/distributions/distributions.py` & `preliz-0.6.1/preliz/distributions/distributions.py`

 * *Files 1% similar despite different names*

```diff
@@ -597,16 +597,29 @@
         support : str
             Available options are `full` or `restricted`. If `full` the values will cover the entire
             support of the distribution, if finite, or the quantiles 0.0001 or 0.9999, if infinite.
             If `restricted` the values will cover the quantile 0.0001 to 0.9999.
         n_points : int
             Number of values to return.
         """
-        lower_ep, upper_ep = self._finite_endpoints(support)
-        return continuous_xvals(lower_ep, upper_ep, n_points)
+        if isinstance(support, tuple):
+            return self.ppf(np.linspace(*self.cdf(support), n_points))
+        else:
+            lower_ep, upper_ep = self.support
+
+            if not np.isfinite(lower_ep) or support == "restricted":
+                lower_ep = 0.0001
+            if not np.isfinite(upper_ep) or support == "restricted":
+                upper_ep = 0.9999
+
+            half_n_points = int(n_points / 2)
+            even = np.linspace(*self.ppf([lower_ep, upper_ep]), half_n_points)
+            uneven = self.ppf(np.linspace(lower_ep, upper_ep, half_n_points))
+
+            return np.sort(np.concatenate([even, uneven]))
 
     def _fit_mle(self, sample, **kwargs):
         """
         Estimate the parameters of the distribution from a sample by maximizing the likelihood.
 
         Parameters
         ----------
```

### Comparing `preliz-0.6.0/preliz/distributions/distributions_multivariate.py` & `preliz-0.6.1/preliz/distributions/distributions_multivariate.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/distributions/exgaussian.py` & `preliz-0.6.1/preliz/distributions/exgaussian.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/distributions/exponential.py` & `preliz-0.6.1/preliz/distributions/exponential.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # pylint: disable=attribute-defined-outside-init
 # pylint: disable=arguments-differ
 import numpy as np
 import numba as nb
 
 from .distributions import Continuous
 from ..internal.distribution_helper import eps, all_not_none
-from ..internal.special import cdf_bounds, ppf_bounds_cont, mean_sample
+from ..internal.special import cdf_bounds, ppf_bounds_cont, mean_sample, xlog1py
 
 
 class Exponential(Continuous):
     r"""
     Exponential Distribution
 
     The pdf of this distribution is
@@ -154,15 +154,15 @@
 def nb_cdf(x, lam):
     x_lam = lam * x
     return cdf_bounds(1 - np.exp(-x_lam), x, 0, np.inf)
 
 
 @nb.njit(cache=True)
 def nb_ppf(q, beta):
-    return ppf_bounds_cont(-beta * np.log(1 - q), q, 0, np.inf)
+    return ppf_bounds_cont(-xlog1py(beta, -q), q, 0, np.inf)
 
 
 @nb.vectorize(nopython=True, cache=True)
 def nb_logpdf(x, lam):
     if x < 0:
         return -np.inf
     else:
```

### Comparing `preliz-0.6.0/preliz/distributions/gamma.py` & `preliz-0.6.1/preliz/distributions/gamma.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,18 +185,21 @@
 
 
 def nb_ppf(q, alpha, beta, lower, upper):
     x_val = gammaincinv(alpha, q) * (1 / beta)
     return ppf_bounds_cont(x_val, q, lower, upper)
 
 
-@nb.njit(cache=True)
+@nb.vectorize(nopython=True, cache=True)
 def nb_logpdf(x, alpha, beta):
-    x = x / (1 / beta)
-    return xlogy(alpha - 1.0, x) - x - gammaln(alpha) - np.log(1 / beta)
+    if x < 0:
+        return -np.inf
+    else:
+        x = x / (1 / beta)
+        return xlogy(alpha - 1.0, x) - x - gammaln(alpha) - np.log(1 / beta)
 
 
 @nb.njit(cache=True)
 def nb_neg_logpdf(x, alpha, beta):
     return -(nb_logpdf(x, alpha, beta)).sum()
```

### Comparing `preliz-0.6.0/preliz/distributions/geometric.py` & `preliz-0.6.1/preliz/distributions/geometric.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # pylint: disable=arguments-differ
 import numba as nb
 import numpy as np
 
 from .distributions import Discrete
 from ..internal.distribution_helper import eps
 from ..internal.special import mean_sample, cdf_bounds, ppf_bounds_disc
+from ..internal.special import xlog1py, xlogx
 
 
 class Geometric(Discrete):
     R"""
     Geometric distribution.
 
     The probability that the first success in a sequence of Bernoulli trials
@@ -135,18 +136,21 @@
 def nb_ppf(q, p, lower, upper):
     x_vals = np.ceil(np.log(1 - q) / np.log(1 - p))
     return ppf_bounds_disc(x_vals, q, lower, upper)
 
 
 @nb.njit(cache=True)
 def nb_entropy(p):
-    return (-(1 - p) * np.log(1 - p) - p * np.log(p)) / p
+    return (xlog1py((-1 + p), -p) - xlogx(p)) / p
 
 
-@nb.njit(cache=True)
+@nb.vectorize(nopython=True, cache=True)
 def nb_logpdf(x, p):
-    return (x - 1) * np.log((1 - p)) + np.log(p)
+    if x < 1:
+        return -np.inf
+    else:
+        return xlog1py(x - 1, -p) + np.log(p)
 
 
 @nb.njit(cache=True)
 def nb_neg_logpdf(x, p):
     return -(nb_logpdf(x, p)).sum()
```

### Comparing `preliz-0.6.0/preliz/distributions/gumbel.py` & `preliz-0.6.1/preliz/distributions/gumbel.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/distributions/halfcauchy.py` & `preliz-0.6.1/preliz/distributions/halfcauchy.py`

 * *Files 3% similar despite different names*

```diff
@@ -138,17 +138,20 @@
 
 
 @nb.njit(cache=True)
 def nb_entropy(beta):
     return np.log(2 * beta * np.pi)
 
 
-@nb.njit(cache=True)
+@nb.vectorize(nopython=True, cache=True)
 def nb_logpdf(x, beta):
-    return np.log(2) - np.log(np.pi * beta) - np.log(1 + (x / beta) ** 2)
+    if x < 0:
+        return -np.inf
+    else:
+        return np.log(2) - np.log(np.pi * beta) - np.log(1 + (x / beta) ** 2)
 
 
 @nb.njit(cache=True)
 def nb_neg_logpdf(x, beta):
     return (-nb_logpdf(x, beta)).sum()
```

### Comparing `preliz-0.6.0/preliz/distributions/halfnormal.py` & `preliz-0.6.1/preliz/distributions/halfnormal.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/distributions/halfstudentt.py` & `preliz-0.6.1/preliz/distributions/halfstudentt.py`

 * *Files 2% similar despite different names*

```diff
@@ -238,21 +238,24 @@
         np.log(sigma)
         + 0.5 * (nu + 1) * (digamma(0.5 * (nu + 1)) - digamma(0.5 * nu))
         + np.log(np.sqrt(nu) * beta(0.5 * nu, 0.5))
         - np.log(2)
     )
 
 
-@nb.njit(cache=True)
+@nb.vectorize(nopython=True, cache=True)
 def nb_logpdf(x, nu, sigma):
-    return (
-        gammaln((nu + 1) / 2)
-        - gammaln(nu / 2)
-        - 0.5 * np.log(nu * np.pi * sigma**2)
-        - 0.5 * (nu + 1) * np.log(1 + (x / sigma) ** 2 / nu)
-        + np.log(2)
-    )
+    if x < 0:
+        return -np.inf
+    else:
+        return (
+            gammaln((nu + 1) / 2)
+            - gammaln(nu / 2)
+            - 0.5 * np.log(nu * np.pi * sigma**2)
+            - 0.5 * (nu + 1) * np.log(1 + (x / sigma) ** 2 / nu)
+            + np.log(2)
+        )
 
 
 @nb.njit(cache=True)
 def nb_neg_logpdf(x, nu, sigma):
     return -(nb_logpdf(x, nu, sigma)).sum()
```

### Comparing `preliz-0.6.0/preliz/distributions/hurdle.py` & `preliz-0.6.1/preliz/distributions/hurdle.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/distributions/hypergeometric.py` & `preliz-0.6.1/preliz/distributions/hypergeometric.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/distributions/inversegamma.py` & `preliz-0.6.1/preliz/distributions/inversegamma.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # pylint: disable=arguments-differ
 import numpy as np
 import numba as nb
 
 from scipy.special import gammaincc, gammainccinv  # pylint: disable=no-name-in-module
 
 from ..internal.distribution_helper import all_not_none, any_not_none, eps
-from ..internal.special import gammaln, digamma, cdf_bounds, ppf_bounds_cont
+from ..internal.special import gammaln, digamma, cdf_bounds, ppf_bounds_cont, xlogy
 from ..internal.optimization import optimize_ml
 from .distributions import Continuous
 
 
 class InverseGamma(Continuous):
     r"""
     Inverse gamma distribution, the reciprocal of the gamma distribution.
@@ -184,17 +184,20 @@
 
 
 @nb.njit(cache=True)
 def nb_entropy(alpha, beta):
     return alpha + gammaln(alpha) - (1 + alpha) * digamma(alpha) + np.log(beta)
 
 
-@nb.njit(cache=True)
+@nb.vectorize(nopython=True, cache=True)
 def nb_logpdf(x, alpha, beta):
-    return alpha * np.log(beta) - gammaln(alpha) - (alpha + 1) * np.log(x) - beta / x
+    if x <= 0:
+        return -np.inf
+    else:
+        return xlogy(alpha, beta) - gammaln(alpha) - xlogy((alpha + 1), x) - beta / x
 
 
 @nb.njit(cache=True)
 def nb_neg_logpdf(x, alpha, beta):
     return -(nb_logpdf(x, alpha, beta)).sum()
```

### Comparing `preliz-0.6.0/preliz/distributions/kumaraswamy.py` & `preliz-0.6.1/preliz/distributions/kumaraswamy.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from ..internal.distribution_helper import eps, all_not_none
 from ..internal.optimization import optimize_ml, optimize_moments
 from ..internal.special import (
     beta,
     digamma,
     cdf_bounds,
     ppf_bounds_cont,
+    xlogy,
+    xlog1py,
 )
 
 
 class Kumaraswamy(Continuous):
     r"""
     Kumaraswamy distribution.
 
@@ -165,17 +167,20 @@
 
 @nb.njit(cache=True)
 def nb_entropy(a, b):
     h_b = digamma(b + 1) + np.euler_gamma
     return (1 - 1 / b) + (1 - 1 / a) * h_b - np.log(a) - np.log(b)
 
 
-@nb.njit(cache=True)
+@nb.vectorize(nopython=True, cache=True)
 def nb_logpdf(x, a, b):
-    return np.log(a * b) + (a - 1) * np.log(x) + (b - 1) * np.log(1 - x**a)
+    if x < 0 or x > 1:
+        return -np.inf
+    else:
+        return np.log(a * b) + xlogy((a - 1), x) + xlog1py((b - 1), -(x**a))
 
 
 @nb.njit(cache=True)
 def nb_neg_logpdf(x, a, b):
     return -(nb_logpdf(x, a, b)).sum()
```

### Comparing `preliz-0.6.0/preliz/distributions/laplace.py` & `preliz-0.6.1/preliz/distributions/laplace.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/distributions/logistic.py` & `preliz-0.6.1/preliz/distributions/logistic.py`

 * *Files 4% similar despite different names*

```diff
@@ -142,15 +142,18 @@
 
 
 @nb.njit(cache=True)
 def nb_entropy(s):
     return np.log(s) + 2
 
 
-@nb.njit(cache=True)
+@nb.vectorize(nopython=True, cache=True)
 def nb_logpdf(x, mu, s):
-    return -np.log(s) - 2 * np.log(1 + np.exp(-(x - mu) / s)) - (x - mu) / s
+    if x == -np.inf:
+        return -np.inf
+    else:
+        return -np.log(s) - 2 * np.log1p(np.exp(-(x - mu) / s)) - (x - mu) / s
 
 
 @nb.njit(cache=True)
 def nb_neg_logpdf(x, mu, s):
     return -(nb_logpdf(x, mu, s)).sum()
```

### Comparing `preliz-0.6.0/preliz/distributions/logitnormal.py` & `preliz-0.6.1/preliz/distributions/logitnormal.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/distributions/lognormal.py` & `preliz-0.6.1/preliz/distributions/lognormal.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,17 +155,20 @@
 
 
 @nb.njit(cache=True)
 def nb_entropy(mu, sigma):
     return np.log((2 * np.pi) ** 0.5 * sigma * np.exp(mu + 0.5))
 
 
-@nb.njit(cache=True)
+@nb.vectorize(nopython=True, cache=True)
 def nb_logpdf(x, mu, sigma):
-    return -(np.log(x) + np.log(sigma) + 0.5 * np.log(2 * np.pi)) - ((np.log(x) - mu) ** 2) / (
-        2 * sigma**2
-    )
+    if x <= 0:
+        return -np.inf
+    else:
+        return -(np.log(x) + np.log(sigma) + 0.5 * np.log(2 * np.pi)) - ((np.log(x) - mu) ** 2) / (
+            2 * sigma**2
+        )
 
 
 @nb.njit(cache=True)
 def nb_neg_logpdf(x, mu, sigma):
     return -(nb_logpdf(x, mu, sigma)).sum()
```

### Comparing `preliz-0.6.0/preliz/distributions/moyal.py` & `preliz-0.6.1/preliz/distributions/moyal.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/distributions/negativebinomial.py` & `preliz-0.6.1/preliz/distributions/negativebinomial.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,15 +191,18 @@
 # @nb.jit
 # bdtrik not supported by numba
 def nb_ppf(q, n, p, lower, upper):
     x_vals = np.ceil(nbdtrik(q, n, p))
     return ppf_bounds_disc(x_vals, q, lower, upper)
 
 
-@nb.njit(cache=True)
+@nb.vectorize(nopython=True, cache=True)
 def nb_logpdf(y, n, p):
-    return gammaln(y + n) - gammaln(n) - gammaln(y + 1) + xlogy(n, p) + xlogy(y, 1 - p)
+    if y < 0:
+        return -np.inf
+    else:
+        return gammaln(y + n) - gammaln(n) - gammaln(y + 1) + xlogy(n, p) + xlogy(y, 1 - p)
 
 
 @nb.njit(cache=True)
 def nb_neg_logpdf(y, n, p):
     return -(nb_logpdf(y, n, p)).sum()
```

### Comparing `preliz-0.6.0/preliz/distributions/normal.py` & `preliz-0.6.1/preliz/distributions/normal.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/distributions/pareto.py` & `preliz-0.6.1/preliz/distributions/pareto.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # pylint: disable=attribute-defined-outside-init
 # pylint: disable=arguments-differ
 import numpy as np
 import numba as nb
 
 from ..internal.optimization import optimize_ml
-from ..internal.special import ppf_bounds_cont
+from ..internal.special import ppf_bounds_cont, xlogy
 from ..internal.distribution_helper import all_not_none, eps
 from .distributions import Continuous
 
 
 class Pareto(Continuous):
     r"""
     Pareto distribution.
@@ -164,15 +164,15 @@
     return np.log((m / alpha) * np.exp(1 + 1 / alpha))
 
 
 @nb.vectorize(nopython=True, cache=True)
 def nb_logpdf(x, alpha, m):
     if x < m:
         return -np.inf
-    return np.log(alpha) + alpha * np.log(m) - (alpha + 1) * np.log(x)
+    return np.log(alpha) + xlogy(alpha, m) - xlogy((alpha + 1), x)
 
 
 @nb.njit(cache=True)
 def nb_neg_logpdf(x, alpha, m):
     return -(nb_logpdf(x, alpha, m)).sum()
```

### Comparing `preliz-0.6.0/preliz/distributions/poisson.py` & `preliz-0.6.1/preliz/distributions/poisson.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,15 +148,18 @@
 
 
 @nb.njit(cache=True)
 def nb_fit_mle(sample):
     return np.mean(sample)
 
 
-@nb.njit(cache=True)
+@nb.vectorize(nopython=True, cache=True)
 def nb_logpdf(x, mu):
-    return xlogy(x, mu) - gammaln(x + 1) - mu
+    if x < 0:
+        return -np.inf
+    else:
+        return xlogy(x, mu) - gammaln(x + 1) - mu
 
 
 @nb.njit(cache=True)
 def nb_neg_logpdf(x, mu):
     return -(nb_logpdf(x, mu)).sum()
```

### Comparing `preliz-0.6.0/preliz/distributions/rice.py` & `preliz-0.6.1/preliz/distributions/rice.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/distributions/skewnormal.py` & `preliz-0.6.1/preliz/distributions/skewnormal.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/distributions/studentt.py` & `preliz-0.6.1/preliz/distributions/studentt.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/distributions/triangular.py` & `preliz-0.6.1/preliz/distributions/triangular.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/distributions/truncated.py` & `preliz-0.6.1/preliz/distributions/truncated.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/distributions/truncatednormal.py` & `preliz-0.6.1/preliz/distributions/truncatednormal.py`

 * *Files 1% similar despite different names*

```diff
@@ -389,22 +389,25 @@
     psi_beta = (0, 0) if beta == np.inf else (1, beta)
     return np.log((2 * np.pi * np.e) ** 0.5 * sigma * z) + (
         (1 / (2 * np.pi) ** 0.5 * np.exp(-0.5 * psi_alpha[1] ** 2)) * psi_alpha[1] * psi_alpha[0]
         - (1 / (2 * np.pi) ** 0.5 * np.exp(-0.5 * psi_beta[1] ** 2)) * psi_beta[1] * psi_beta[0]
     ) / (2 * z)
 
 
-@nb.njit(cache=True)
+@nb.vectorize(nopython=True, cache=True)
 def nb_logpdf(x, mu, sigma, lower, upper):
-    xi = (x - mu) / sigma
-    alpha = (lower - mu) / sigma
-    beta = (upper - mu) / sigma
-    z = 0.5 * (1 + erf(beta / 2**0.5)) - 0.5 * (1 + erf(alpha / 2**0.5))
-    logphi = np.log(1 / (2 * np.pi) ** 0.5) - xi**2 / 2
-    return logphi - (np.log(sigma) + np.log(z))
+    if x < lower or x > upper:
+        return -np.inf
+    else:
+        xi = (x - mu) / sigma
+        alpha = (lower - mu) / sigma
+        beta = (upper - mu) / sigma
+        z = 0.5 * (1 + erf(beta / 2**0.5)) - 0.5 * (1 + erf(alpha / 2**0.5))
+        logphi = np.log(1 / (2 * np.pi) ** 0.5) - xi**2 / 2
+        return logphi - (np.log(sigma) + np.log(z))
 
 
 @nb.njit(cache=True)
 def nb_neg_logpdf(x, mu, sigma, lower, upper):
     return -(nb_logpdf(x, mu, sigma, lower, upper)).sum()
```

### Comparing `preliz-0.6.0/preliz/distributions/uniform.py` & `preliz-0.6.1/preliz/distributions/uniform.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/distributions/vonmises.py` & `preliz-0.6.1/preliz/distributions/vonmises.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/distributions/wald.py` & `preliz-0.6.1/preliz/distributions/wald.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,18 +194,20 @@
     return 0.5 * np.log((2 * np.pi * np.e * mu**3) / lam) + 3 / 2 * np.exp(2 * lam / mu) * expi(
         -2 * lam / mu
     )
 
 
 @nb.vectorize(nopython=True, cache=True)
 def nb_logpdf(x, mu, lam):
-    if x > 0:
+    if x <= 0:
+        return -np.inf
+    elif x == np.inf:
+        return -np.inf
+    else:
         return (
             np.log(lam) - (np.log(2 * np.pi) + 3 * np.log(x)) - lam * (x - mu) ** 2 / (mu**2 * x)
         ) / 2
-    else:
-        return np.inf
 
 
 @nb.njit(cache=True)
 def nb_neg_logpdf(x, mu, lam):
     return -(nb_logpdf(x, mu, lam)).sum()
```

### Comparing `preliz-0.6.0/preliz/distributions/weibull.py` & `preliz-0.6.1/preliz/distributions/weibull.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from ..internal.optimization import optimize_ml
 from ..internal.special import (
     garcia_approximation,
     gamma,
     mean_and_std,
     cdf_bounds,
     ppf_bounds_cont,
+    xlogy,
 )
 
 
 class Weibull(Continuous):
     r"""
     Weibull distribution.
 
@@ -166,16 +167,19 @@
 
 
 @nb.njit(cache=True)
 def nb_entropy(alpha, beta):
     return np.euler_gamma * (1 - 1 / alpha) + np.log(beta / alpha) + 1
 
 
-@nb.njit(cache=True)
+@nb.vectorize(nopython=True, cache=True)
 def nb_logpdf(x, alpha, beta):
-    x_b = x / beta
-    return np.log(alpha / beta) + (alpha - 1) * np.log(x_b) - x_b**alpha
+    if x < 0:
+        return -np.inf
+    else:
+        x_b = x / beta
+        return np.log(alpha / beta) + xlogy((alpha - 1), x_b) - x_b**alpha
 
 
 @nb.njit(cache=True)
 def nb_neg_logpdf(x, alpha, beta):
     return -(nb_logpdf(x, alpha, beta)).sum()
```

### Comparing `preliz-0.6.0/preliz/distributions/zi_binomial.py` & `preliz-0.6.1/preliz/distributions/zi_binomial.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,18 +164,20 @@
     n_vals = np.ceil(bdtrik(q, n, p))
     x_vals = (1 - psi) + psi * n_vals
     return ppf_bounds_disc(x_vals, q, lower, upper)
 
 
 @nb.vectorize(nopython=True, cache=True)
 def nb_logpdf(psi, n, y, p):
-    if y == 0:
-        return np.log((1 - psi) + psi * (1 - p) ** n)
-    if y > n:
+    if y < 0:
+        return -np.inf
+    elif y > n:
         return -np.inf
+    elif y == 0:
+        return np.log((1 - psi) + psi * (1 - p) ** n)
     else:
         return (
             np.log(psi)
             + gammaln(n + 1)
             - (gammaln(y + 1) + gammaln(n - y + 1))
             + y * np.log(p)
             + (n - y) * np.log1p(-p)
```

### Comparing `preliz-0.6.0/preliz/distributions/zi_negativebinomial.py` & `preliz-0.6.1/preliz/distributions/zi_negativebinomial.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,15 +214,17 @@
     nb_vals = np.ceil(nbdtrik(q, n, p))
     x_vals = (1 - psi) + psi * nb_vals
     return ppf_bounds_disc(x_vals, q, lower, upper)
 
 
 @nb.vectorize(nopython=True, cache=True)
 def nb_logpdf(y, psi, n, p, mu):
-    if y == 0:
+    if y < 0:
+        return -np.inf
+    elif y == 0:
         return np.log((1 - psi) + psi * (n / (n + mu)) ** n)
     else:
         return (
             np.log(psi)
             + gammaln(y + n)
             - gammaln(n)
             - gammaln(y + 1)
```

### Comparing `preliz-0.6.0/preliz/distributions/zi_poisson.py` & `preliz-0.6.1/preliz/distributions/zi_poisson.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,15 @@
                 - 1 / (24 * self.mu**2)
                 - 19 / (360 * self.mu**3)
             )
             if self.psi == 1:
                 return poisson_entropy
             else:
                 # The var can be 0 with probability 1-psi or something else with probability psi
-                zero_entropy = -(1 - self.psi) * np.log(1 - self.psi) - self.psi * np.log(self.psi)
+                zero_entropy = -(1 - self.psi) * np.logp(1 - self.psi) - self.psi * np.log(self.psi)
                 # The total entropy is the weighted sum of the two entropies
                 return (1 - self.psi) * zero_entropy + self.psi * poisson_entropy
 
     def mean(self):
         return self.psi * self.mu
 
     def median(self):
@@ -171,15 +171,17 @@
     p_vals = np.where(temp >= q, vals1, vals)
     x_vals = (1 - psi) + psi * p_vals
     return ppf_bounds_disc(x_vals, q, lower, upper)
 
 
 @nb.vectorize(nopython=True, cache=True)
 def nb_logpdf(x, psi, mu):
-    if x == 0:
+    if x < 0:
+        return -np.inf
+    elif x == 0:
         return np.log(np.exp(-mu) * psi - psi + 1)
     else:
         return np.log(psi) + xlogy(x, mu) - gammaln(x + 1) - mu
 
 
 @nb.njit(cache=True)
 def nb_neg_logpdf(x, psi, mu):
```

### Comparing `preliz-0.6.0/preliz/internal/distribution_helper.py` & `preliz-0.6.1/preliz/internal/distribution_helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 def hdi_from_pdf(dist, mass=0.94):
     """
     Approximate the HDI by evaluating the pdf.
     This is faster, but potentially less accurate, than directly minimizing the
     interval as evaluating the ppf can be slow, specially for some distributions.
     """
+
     if dist.kind == "continuous":
         lower_ep, upper_ep = dist._finite_endpoints("full")
         x_vals = np.linspace(lower_ep, upper_ep, 10000)
         pdf = dist.pdf(x_vals)
         pdf = pdf[np.isfinite(pdf)]
         pdf = pdf / pdf.sum()
     else:
@@ -34,15 +35,19 @@
     mass_cum = 0
     indices = []
     for idx in sorted_idx:
         mass_cum += pdf[idx]
         indices.append(idx)
         if mass_cum >= mass:
             break
-    return x_vals[np.sort(indices)[[0, -1]]]
+
+    if indices:
+        return x_vals[np.sort(indices)[[0, -1]]]
+    else:
+        return np.nan, np.nan
 
 
 def all_not_none(*args):
     for arg in args:
         if arg is None:
             return False
     return True
```

### Comparing `preliz-0.6.0/preliz/internal/optimization.py` & `preliz-0.6.1/preliz/internal/optimization.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/internal/parser.py` & `preliz-0.6.1/preliz/internal/parser.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/internal/plot_helper.py` & `preliz-0.6.1/preliz/internal/plot_helper.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/internal/plot_helper_multivariate.py` & `preliz-0.6.1/preliz/internal/plot_helper_multivariate.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/internal/predictive_helper.py` & `preliz-0.6.1/preliz/internal/predictive_helper.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/internal/special.py` & `preliz-0.6.1/preliz/internal/special.py`

 * *Files 1% similar despite different names*

```diff
@@ -463,14 +463,22 @@
     if x == 0:
         return 0.0
     else:
         return x * np.log(y)
 
 
 @nb.vectorize(nopython=True, cache=True)
+def xlog1py(x, y):
+    if x == 0:
+        return 0.0
+    else:
+        return x * np.log1p(y)
+
+
+@nb.vectorize(nopython=True, cache=True)
 def xlogx(x):
     if x == 0:
         return 0.0
     else:
         return x * np.log(x)
```

### Comparing `preliz-0.6.0/preliz/ppls/pymc_io.py` & `preliz-0.6.1/preliz/ppls/pymc_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,19 @@
     return fmodel
 
 
 def get_pymc_to_preliz():
     """
     Generate dictionary mapping pymc to preliz distributions
     """
-    all_distributions = modules["preliz.distributions"].__all__
+    all_distributions = [
+        dist
+        for dist in modules["preliz.distributions"].__all__
+        if dist not in ["Truncated", "Censored", "Hurdle"]
+    ]
     pymc_to_preliz = dict(
         zip([dist.lower() for dist in all_distributions], get_distributions(all_distributions))
     )
     return pymc_to_preliz
 
 
 def get_guess(model, free_rvs):
```

### Comparing `preliz-0.6.0/preliz/predictive/ppa.py` & `preliz-0.6.1/preliz/predictive/ppa.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/predictive/ppe.py` & `preliz-0.6.1/preliz/predictive/ppe.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/predictive/predictive_explorer.py` & `preliz-0.6.1/preliz/predictive/predictive_explorer.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/tests/check_inside_notebook.ipynb` & `preliz-0.6.1/preliz/tests/check_inside_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/tests/plot_interactive.ipynb` & `preliz-0.6.1/preliz/tests/plot_interactive.ipynb`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/tests/ppa.ipynb` & `preliz-0.6.1/preliz/tests/ppa.ipynb`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/tests/predictive_explorer.ipynb` & `preliz-0.6.1/preliz/tests/predictive_explorer.ipynb`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/tests/quartile_int.ipynb` & `preliz-0.6.1/preliz/tests/quartile_int.ipynb`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/tests/roulette.ipynb` & `preliz-0.6.1/preliz/tests/roulette.ipynb`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/tests/test_beta_mode.py` & `preliz-0.6.1/preliz/tests/test_beta_mode.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/tests/test_censored.py` & `preliz-0.6.1/preliz/tests/test_censored.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/tests/test_dirichlet_mode.py` & `preliz-0.6.1/preliz/tests/test_dirichlet_mode.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/tests/test_discrete_weibull.py` & `preliz-0.6.1/preliz/tests/test_discrete_weibull.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/tests/test_distributions.py` & `preliz-0.6.1/preliz/tests/test_distributions.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/tests/test_helper.py` & `preliz-0.6.1/preliz/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/tests/test_hurdle.py` & `preliz-0.6.1/preliz/tests/test_hurdle.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/tests/test_maxent.py` & `preliz-0.6.1/preliz/tests/test_maxent.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,18 +99,18 @@
         (Moyal(mu=4), 0, 10, 0.9, (-np.inf, np.inf), (1.445)),
         (Normal(), -1, 1, 0.683, (-np.inf, np.inf), (0, 1)),
         (Normal(), 10, 12, 0.99, (-np.inf, np.inf), (11, 0.388)),
         (Normal(mu=0.5), -1, 1, 0.8, (-np.inf, np.inf), (0.581)),
         (Pareto(), 1, 4, 0.9, (1, np.inf), (1.660, 1)),
         (Pareto(m=2), 1, 4, 0.9, (2, np.inf), (3.321)),
         (Rice(), 0, 4, 0.7, (0, np.inf), (0, 2.577)),
-        (Rice(), 1, 10, 0.9, (0, np.inf), (3.453, 3.735)),
+        (Rice(), 1, 10, 0.9, (0, np.inf), (3.454, 3.734)),
         (Rice(nu=4), 0, 6, 0.9, (0, np.inf), (1.402)),
         (SkewNormal(), -2, 10, 0.9, (-np.inf, np.inf), (4.061, 3.648, -0.021)),
-        (SkewNormal(mu=-1), -2, 10, 0.9, (-np.inf, np.inf), (6.293, 4.908)),
+        (SkewNormal(mu=-1), -2, 10, 0.9, (-np.inf, np.inf), (6.292, 4.903)),
         (StudentT(), -1, 1, 0.683, (-np.inf, np.inf), (99.999, 0, 0.994)),
         (StudentT(nu=7), -1, 1, 0.683, (-np.inf, np.inf), (0, 0.928)),
         (
             Triangular(),
             0,
             4,
             0.8,
```

### Comparing `preliz-0.6.0/preliz/tests/test_mle.py` & `preliz-0.6.1/preliz/tests/test_mle.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/tests/test_optimization.py` & `preliz-0.6.1/preliz/tests/test_optimization.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/tests/test_plots.py` & `preliz-0.6.1/preliz/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/tests/test_quartile.py` & `preliz-0.6.1/preliz/tests/test_quartile.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/tests/test_roulette.py` & `preliz-0.6.1/preliz/tests/test_roulette.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/tests/test_scipy.py` & `preliz-0.6.1/preliz/tests/test_scipy.py`

 * *Files 11% similar despite different names*

```diff
@@ -201,62 +201,74 @@
         sc_rvs = scipy_dist.rvs(20000, random_state=rng)
         assert_almost_equal(pz_rvs.mean(), sc_rvs.mean(), decimal=1)
         assert_almost_equal(pz_rvs.std(), sc_rvs.std(), decimal=1)
 
     else:
         assert_almost_equal(actual_rvs, expected_rvs)
 
-    actual_pdf = preliz_dist.pdf(actual_rvs)
+    support = preliz_dist.support
+    if preliz_name == "VonMises":
+        extended_vals = actual_rvs
+    else:
+        extended_vals = np.concatenate(
+            [
+                actual_rvs,
+                support,
+                [support[0] - 1],
+                [support[0] - 2],
+                [support[1] + 1],
+                [support[1] + 2],
+            ]
+        )
+
+    actual_pdf = preliz_dist.pdf(extended_vals)
     if preliz_dist.kind == "continuous":
-        expected_pdf = scipy_dist.pdf(actual_rvs)
+        expected_pdf = scipy_dist.pdf(extended_vals)
     else:
-        expected_pdf = scipy_dist.pmf(actual_rvs)
+        expected_pdf = scipy_dist.pmf(extended_vals)
 
     if preliz_name == "LogitNormal":
         assert_almost_equal(actual_pdf, expected_pdf, decimal=1)
     elif preliz_name == "HalfStudentT":
         assert_almost_equal(actual_pdf, expected_pdf, decimal=2)
     else:
         assert_almost_equal(actual_pdf, expected_pdf, decimal=4)
 
-    support = preliz_dist.support
-    cdf_vals = np.concatenate([actual_rvs, support, [support[0] - 1], [support[1] + 1]])
-
-    actual_cdf = preliz_dist.cdf(cdf_vals)
-    expected_cdf = scipy_dist.cdf(cdf_vals)
+    actual_cdf = preliz_dist.cdf(extended_vals)
+    expected_cdf = scipy_dist.cdf(extended_vals)
 
     if preliz_name in ["HalfStudentT", "LogitNormal"]:
         assert_almost_equal(actual_cdf, expected_cdf, decimal=2)
     else:
         assert_almost_equal(actual_cdf, expected_cdf, decimal=6)
 
     x_vals = [-1, 0, 0.25, 0.5, 0.75, 1, 2]
     actual_ppf = preliz_dist.ppf(x_vals)
     expected_ppf = scipy_dist.ppf(x_vals)
     if preliz_name in ["HalfStudentT", "Wald", "LogitNormal", "SkewNormal", "ExGaussian"]:
         assert_almost_equal(actual_ppf, expected_ppf, decimal=2)
     else:
         assert_almost_equal(actual_ppf, expected_ppf)
 
-    actual_logpdf = preliz_dist.logpdf(actual_rvs)
+    actual_logpdf = preliz_dist.logpdf(extended_vals)
     if preliz_dist.kind == "continuous":
-        expected_logpdf = scipy_dist.logpdf(actual_rvs)
+        expected_logpdf = scipy_dist.logpdf(extended_vals)
     else:
-        expected_logpdf = scipy_dist.logpmf(actual_rvs)
+        expected_logpdf = scipy_dist.logpmf(extended_vals)
 
     if preliz_name == "HalfStudentT":
         assert_almost_equal(actual_logpdf, expected_logpdf, decimal=0)
     elif preliz_name == "LogitNormal":
         assert_almost_equal(actual_logpdf, expected_logpdf, decimal=1)
     elif preliz_name in ["SkewNormal"]:
         assert_almost_equal(actual_logpdf, expected_logpdf, decimal=6)
     else:
         assert_almost_equal(actual_logpdf, expected_logpdf)
 
-    actual_neg_logpdf = preliz_dist._neg_logpdf(actual_rvs)
+    actual_neg_logpdf = preliz_dist._neg_logpdf(extended_vals)
     expected_neg_logpdf = -expected_logpdf.sum()
     if preliz_name in ["HalfStudentT", "LogitNormal"]:
         assert_almost_equal(actual_neg_logpdf, expected_neg_logpdf, decimal=1)
     elif preliz_name in ["TruncatedNormal", "SkewNormal"]:
         assert_almost_equal(actual_neg_logpdf, expected_neg_logpdf, decimal=6)
     else:
         assert_almost_equal(actual_neg_logpdf, expected_neg_logpdf)
```

### Comparing `preliz-0.6.0/preliz/tests/test_special.py` & `preliz-0.6.1/preliz/tests/test_special.py`

 * *Files 25% similar despite different names*

```diff
@@ -63,7 +63,24 @@
     x = np.linspace(-0.1, 1.1, 100)
     assert_almost_equal(sc_special.logit(x), pz_special.logit(x))
 
 
 def test_expit():
     x = np.linspace(-20, 10, 500)
     assert_almost_equal(sc_special.expit(x), pz_special.expit(x))
+
+
+def test_xlogy():
+    x = np.linspace(0, 10, 10)
+    y = np.linspace(0, 10, 10)
+    assert_almost_equal(sc_special.xlogy(x, y), pz_special.xlogy(x, y))
+
+
+def test_xlog1py():
+    x = np.linspace(0, 10, 10)
+    y = np.linspace(0, 10, 10)
+    assert_almost_equal(sc_special.xlog1py(x, y), pz_special.xlog1py(x, y))
+
+
+def test_xlogx():
+    x = np.linspace(0.0, 10, 10)
+    assert_almost_equal(pz_special.xlogy(x, x), pz_special.xlogx(x))
```

### Comparing `preliz-0.6.0/preliz/tests/test_truncated.py` & `preliz-0.6.1/preliz/tests/test_truncated.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/unidimensional/beta_mode.py` & `preliz-0.6.1/preliz/unidimensional/beta_mode.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/unidimensional/dirichlet_mode.py` & `preliz-0.6.1/preliz/unidimensional/dirichlet_mode.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/unidimensional/maxent.py` & `preliz-0.6.1/preliz/unidimensional/maxent.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/unidimensional/mle.py` & `preliz-0.6.1/preliz/unidimensional/mle.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/unidimensional/quartile.py` & `preliz-0.6.1/preliz/unidimensional/quartile.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/unidimensional/quartile_int.py` & `preliz-0.6.1/preliz/unidimensional/quartile_int.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/preliz/unidimensional/roulette.py` & `preliz-0.6.1/preliz/unidimensional/roulette.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/pyproject.toml` & `preliz-0.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `preliz-0.6.0/PKG-INFO` & `preliz-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: preliz
-Version: 0.6.0
+Version: 0.6.1
 Summary: The place for all your prior elicitation needs.
 Author-email: ArviZ team <arviz.devs@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: Apache Software License
```

