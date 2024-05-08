# Comparing `tmp/readfish-2023.1.1.tar.gz` & `tmp/readfish-2024.1.0.tar.gz`

## Comparing `readfish-2023.1.1.tar` & `readfish-2024.1.0.tar`

### file list

```diff
@@ -1,151 +1,155 @@
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 readfish-2023.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 readfish-2023.1.1/CITATION.cff
--rw-r--r--   0        0        0     4158 2020-02-02 00:00:00.000000 readfish-2023.1.1/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 readfish-2023.1.1/.github/faq.yml
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 readfish-2023.1.1/.github/faq/FAQ.md
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 readfish-2023.1.1/.github/faq/suggest.md
--rw-r--r--   0        0        0     4054 2020-02-02 00:00:00.000000 readfish-2023.1.1/.github/workflows/CI.yml
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 readfish-2023.1.1/.github/workflows/faqtory.yml
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 readfish-2023.1.1/.github/workflows/stale.yml
--rw-r--r--   0        0        0    82708 2020-02-02 00:00:00.000000 readfish-2023.1.1/_static/readfish.jpg
--rw-r--r--   0        0        0   164136 2020-02-02 00:00:00.000000 readfish-2023.1.1/_static/readfish_dark.png
--rw-r--r--   0        0        0   190609 2020-02-02 00:00:00.000000 readfish-2023.1.1/_static/readfish_light.png
--rw-r--r--   0        0        0    12731 2020-02-02 00:00:00.000000 readfish-2023.1.1/_static/readfish_logo.jpg
--rw-r--r--   0        0        0     7046 2020-02-02 00:00:00.000000 readfish-2023.1.1/_static/readfish_small.jpg
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 readfish-2023.1.1/_static/example_tomls/COSMIC_cancer_panel.bed
--rw-r--r--   0        0        0   228736 2020-02-02 00:00:00.000000 readfish-2023.1.1/_static/images/PlaybackControlRun30Minutes.png
--rw-r--r--   0        0        0   206755 2020-02-02 00:00:00.000000 readfish-2023.1.1/_static/images/PlaybackRunTargeted.png
--rw-r--r--   0        0        0   222323 2020-02-02 00:00:00.000000 readfish-2023.1.1/_static/images/PlaybackRunTargetedPeak.png
--rw-r--r--   0        0        0   224078 2020-02-02 00:00:00.000000 readfish-2023.1.1/_static/images/PlaybackRunTargetedUnblockPeak.png
--rw-r--r--   0        0        0   155966 2020-02-02 00:00:00.000000 readfish-2023.1.1/_static/images/PlaybackRunUnblock.png
--rw-r--r--   0        0        0   156826 2020-02-02 00:00:00.000000 readfish-2023.1.1/_static/images/PlaybackRunUnblockCloseUp.png
--rw-r--r--   0        0        0   202426 2020-02-02 00:00:00.000000 readfish-2023.1.1/_static/images/PlaybackUnblockAll30minutes.png
--rw-r--r--   0        0        0   211500 2020-02-02 00:00:00.000000 readfish-2023.1.1/_static/images/PlaybackUnblockAllCloseUp.png
--rw-r--r--   0        0        0   145644 2020-02-02 00:00:00.000000 readfish-2023.1.1/_static/images/Unblock.png
--rw-r--r--   0        0        0   151624 2020-02-02 00:00:00.000000 readfish-2023.1.1/_static/images/UnblockAllMessages.png
--rw-r--r--   0        0        0   155720 2020-02-02 00:00:00.000000 readfish-2023.1.1/_static/images/Unblock_closeup.png
--rw-r--r--   0        0        0   151990 2020-02-02 00:00:00.000000 readfish-2023.1.1/_static/images/control.png
--rw-r--r--   0        0        0   284161 2020-02-02 00:00:00.000000 readfish-2023.1.1/_static/images/data_model.png
--rw-r--r--   0        0        0    38123 2020-02-02 00:00:00.000000 readfish-2023.1.1/_static/images/data_model.svg
--rw-r--r--   0        0        0    38123 2020-02-02 00:00:00.000000 readfish-2023.1.1/_static/images/data_model_no_bg.svg
--rw-r--r--   0        0        0    69772 2020-02-02 00:00:00.000000 readfish-2023.1.1/_static/images/message.png
--rw-r--r--   0        0        0   143794 2020-02-02 00:00:00.000000 readfish-2023.1.1/_static/images/minknow_messages.png
--rw-r--r--   0        0        0   103153 2020-02-02 00:00:00.000000 readfish-2023.1.1/_static/images/simulated_playback_run_options.png
--rw-r--r--   0        0        0     6826 2020-02-02 00:00:00.000000 readfish-2023.1.1/docs/FAQ.md
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 readfish-2023.1.1/docs/Makefile
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 readfish-2023.1.1/docs/changelog.md
--rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 readfish-2023.1.1/docs/conf.py
--rw-r--r--   0        0        0    10561 2020-02-02 00:00:00.000000 readfish-2023.1.1/docs/developers-guide.md
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 readfish-2023.1.1/docs/development.yml
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 readfish-2023.1.1/docs/getting-started.md
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 readfish-2023.1.1/docs/guppy-params.md
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 readfish-2023.1.1/docs/index.md
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 readfish-2023.1.1/docs/make.bat
--rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 readfish-2023.1.1/docs/post-analysis.md
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 readfish-2023.1.1/docs/readfish.console.rst
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 readfish-2023.1.1/docs/readfish.plugins.rst
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 readfish-2023.1.1/docs/readfish.rst
--rw-r--r--   0        0        0    19103 2020-02-02 00:00:00.000000 readfish-2023.1.1/docs/toml.md
--rw-r--r--   0        0        0   155966 2020-02-02 00:00:00.000000 readfish-2023.1.1/docs/images/PlaybackRunUnblock.png
--rw-r--r--   0        0        0   156826 2020-02-02 00:00:00.000000 readfish-2023.1.1/docs/images/PlaybackRunUnblockCloseUp.png
--rw-r--r--   0        0        0   145644 2020-02-02 00:00:00.000000 readfish-2023.1.1/docs/images/Unblock.png
--rw-r--r--   0        0        0   155720 2020-02-02 00:00:00.000000 readfish-2023.1.1/docs/images/Unblock_closeup.png
--rw-r--r--   0        0        0   151990 2020-02-02 00:00:00.000000 readfish-2023.1.1/docs/images/control.png
--rw-r--r--   0        0        0    69772 2020-02-02 00:00:00.000000 readfish-2023.1.1/docs/images/message.png
--rw-r--r--   0        0        0   143794 2020-02-02 00:00:00.000000 readfish-2023.1.1/docs/images/minknow_messages.png
--rw-r--r--   0        0        0    82708 2020-02-02 00:00:00.000000 readfish-2023.1.1/docs/images/readfish.jpg
--rw-r--r--   0        0        0   237831 2020-02-02 00:00:00.000000 readfish-2023.1.1/docs/images/readfish.png
--rw-r--r--   0        0        0   217946 2020-02-02 00:00:00.000000 readfish-2023.1.1/docs/images/readfish_dark.png
--rw-r--r--   0        0        0    12731 2020-02-02 00:00:00.000000 readfish-2023.1.1/docs/images/readfish_logo.jpg
--rw-r--r--   0        0        0     7046 2020-02-02 00:00:00.000000 readfish-2023.1.1/docs/images/readfish_small.jpg
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 readfish-2023.1.1/docs/questions/batch-times.question.md
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 readfish-2023.1.1/docs/questions/creating_readfish-environment.question.md
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 readfish-2023.1.1/docs/questions/key_error_adapter.md
--rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 readfish-2023.1.1/docs/questions/py-guppy-client-error.question.md
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 readfish-2023.1.1/docs/questions/py-guppy-client-version.question.md
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 readfish-2023.1.1/docs/questions/readfish-branches.question.md
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 readfish-2023.1.1/src/readfish/__about__.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 readfish-2023.1.1/src/readfish/__init__.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 readfish-2023.1.1/src/readfish/__main__.py
--rw-r--r--   0        0        0    11387 2020-02-02 00:00:00.000000 readfish-2023.1.1/src/readfish/_channels.py
--rw-r--r--   0        0        0     4214 2020-02-02 00:00:00.000000 readfish-2023.1.1/src/readfish/_cli_args.py
--rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 readfish-2023.1.1/src/readfish/_cli_base.py
--rw-r--r--   0        0        0    19412 2020-02-02 00:00:00.000000 readfish-2023.1.1/src/readfish/_config.py
--rw-r--r--   0        0        0     4883 2020-02-02 00:00:00.000000 readfish-2023.1.1/src/readfish/_loggers.py
--rw-r--r--   0        0        0     9417 2020-02-02 00:00:00.000000 readfish-2023.1.1/src/readfish/_read_until_client.py
--rw-r--r--   0        0        0    19105 2020-02-02 00:00:00.000000 readfish-2023.1.1/src/readfish/_statistics.py
--rw-r--r--   0        0        0    15654 2020-02-02 00:00:00.000000 readfish-2023.1.1/src/readfish/_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2023.1.1/src/readfish/entry_points/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2023.1.1/src/readfish/entry_points/demultiplex.py
--rw-r--r--   0        0        0     6122 2020-02-02 00:00:00.000000 readfish-2023.1.1/src/readfish/entry_points/stats.py
--rw-r--r--   0        0        0    25829 2020-02-02 00:00:00.000000 readfish-2023.1.1/src/readfish/entry_points/targets.py
--rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 readfish-2023.1.1/src/readfish/entry_points/unblock_all.py
--rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 readfish-2023.1.1/src/readfish/entry_points/validate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2023.1.1/src/readfish/plugins/__init__.py
--rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 readfish-2023.1.1/src/readfish/plugins/_filter.py
--rw-r--r--   0        0        0    12583 2020-02-02 00:00:00.000000 readfish-2023.1.1/src/readfish/plugins/_mappy.py
--rw-r--r--   0        0        0     4037 2020-02-02 00:00:00.000000 readfish-2023.1.1/src/readfish/plugins/_no_op.py
--rw-r--r--   0        0        0     4477 2020-02-02 00:00:00.000000 readfish-2023.1.1/src/readfish/plugins/abc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2023.1.1/src/readfish/plugins/deepnano_blitz.py
--rw-r--r--   0        0        0    11742 2020-02-02 00:00:00.000000 readfish-2023.1.1/src/readfish/plugins/guppy.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 readfish-2023.1.1/src/readfish/plugins/mappy.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 readfish-2023.1.1/src/readfish/plugins/mappy_rs.py
--rw-r--r--   0        0        0    29736 2020-02-02 00:00:00.000000 readfish-2023.1.1/src/readfish/plugins/utils.py
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 readfish-2023.1.1/src/readfish/read_until/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 readfish-2023.1.1/src/readfish/read_until/_version.py
--rw-r--r--   0        0        0    25181 2020-02-02 00:00:00.000000 readfish-2023.1.1/src/readfish/read_until/base.py
--rw-r--r--   0        0        0     9205 2020-02-02 00:00:00.000000 readfish-2023.1.1/src/readfish/read_until/read_cache.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 readfish-2023.1.1/tests/conftest.py
--rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 readfish-2023.1.1/tests/describe_test.py
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 readfish-2023.1.1/tests/stats_test.py
--rw-r--r--   0        0        0     4735 2020-02-02 00:00:00.000000 readfish-2023.1.1/tests/utils_test.py
--rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 readfish-2023.1.1/tests/validation_test.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 readfish-2023.1.1/tests/static/describe_test/describe_aligner_barcoded_expected.txt
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 readfish-2023.1.1/tests/static/describe_test/describe_aligner_barcoded_regions_expected.txt
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 readfish-2023.1.1/tests/static/describe_test/describe_aligner_regions_expected.txt
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 readfish-2023.1.1/tests/static/describe_test/describe_barcoded_experiment_expected.txt
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 readfish-2023.1.1/tests/static/describe_test/describe_barcoded_regions_experiment_expected.txt
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 readfish-2023.1.1/tests/static/describe_test/describe_experiment_regions_expected.txt
--rw-r--r--   0        0        0   531281 2020-02-02 00:00:00.000000 readfish-2023.1.1/tests/static/describe_test/yeast_8kb_contigs_test.mmi
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 readfish-2023.1.1/tests/static/guppy_validation_test/README.md
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 readfish-2023.1.1/tests/static/guppy_validation_test/fail/001_no_write_socket.txt
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 readfish-2023.1.1/tests/static/guppy_validation_test/fail/002_missing_socket.txt
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 readfish-2023.1.1/tests/static/guppy_validation_test/fail/003_no_read_socket.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2023.1.1/tests/static/guppy_validation_test/fail/5555_fail_nr
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2023.1.1/tests/static/guppy_validation_test/fail/5555_fail_nw
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 readfish-2023.1.1/tests/static/guppy_validation_test/pass/001_correct_debug.txt
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 readfish-2023.1.1/tests/static/guppy_validation_test/pass/002_correct_no_debug.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2023.1.1/tests/static/guppy_validation_test/pass/5555_pass
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 readfish-2023.1.1/tests/static/mappy_validation_test/README.md
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 readfish-2023.1.1/tests/static/mappy_validation_test/fail/001_wrong_reference_type.txt
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 readfish-2023.1.1/tests/static/mappy_validation_test/fail/002_reference_not_exist.txt
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 readfish-2023.1.1/tests/static/mappy_validation_test/fail/003_wrong_reference_type_mmi_gz.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2023.1.1/tests/static/mappy_validation_test/fail/i_am_a_fail_reference.mmi.gz
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2023.1.1/tests/static/mappy_validation_test/fail/i_am_a_fail_reference.txt
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 readfish-2023.1.1/tests/static/mappy_validation_test/pass/001_correct_reference_mmi.txt
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 readfish-2023.1.1/tests/static/mappy_validation_test/pass/002_correct_reference_fasta.txt
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 readfish-2023.1.1/tests/static/mappy_validation_test/pass/003_correct_reference_fastq.txt
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 readfish-2023.1.1/tests/static/mappy_validation_test/pass/004_correct_reference_fasta_gz.txt
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 readfish-2023.1.1/tests/static/mappy_validation_test/pass/005_correct_reference_fastq_gz.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2023.1.1/tests/static/mappy_validation_test/pass/hello.fasta
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2023.1.1/tests/static/mappy_validation_test/pass/hello.fasta.gz
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2023.1.1/tests/static/mappy_validation_test/pass/hello.fastq
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2023.1.1/tests/static/mappy_validation_test/pass/hello.fastq.gz
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2023.1.1/tests/static/mappy_validation_test/pass/hello.mmi
--rw-r--r--   0        0        0    14385 2020-02-02 00:00:00.000000 readfish-2023.1.1/tests/static/stats_test/expected_summary.txt
--rw-r--r--   0        0        0   997010 2020-02-02 00:00:00.000000 readfish-2023.1.1/tests/static/stats_test/simulated_reads.fastq
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 readfish-2023.1.1/tests/static/stats_test/stats.tsv
--rw-r--r--   0        0        0   531281 2020-02-02 00:00:00.000000 readfish-2023.1.1/tests/static/stats_test/yeast_8kb_contigs_test.mmi
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 readfish-2023.1.1/tests/static/toml_validation_test/README.md
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 readfish-2023.1.1/tests/static/toml_validation_test/fail/001_missing_keys.txt
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 readfish-2023.1.1/tests/static/toml_validation_test/fail/002_wrong_types.txt
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 readfish-2023.1.1/tests/static/toml_validation_test/fail/003_plugin_fail_0.txt
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 readfish-2023.1.1/tests/static/toml_validation_test/fail/003_plugin_fail_1.txt
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 readfish-2023.1.1/tests/static/toml_validation_test/fail/004_target_interval_check.txt
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 readfish-2023.1.1/tests/static/toml_validation_test/fail/COSMIC_cancer_panel_errors.bed
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 readfish-2023.1.1/tests/static/toml_validation_test/pass/001_simple_toml.txt
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 readfish-2023.1.1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 readfish-2023.1.1/LICENSE
--rw-r--r--   0        0        0    68736 2020-02-02 00:00:00.000000 readfish-2023.1.1/README.md
--rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 readfish-2023.1.1/pyproject.toml
--rw-r--r--   0        0        0    70968 2020-02-02 00:00:00.000000 readfish-2023.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 readfish-2024.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 readfish-2024.1.0/CITATION.cff
+-rw-r--r--   0        0        0     4158 2020-02-02 00:00:00.000000 readfish-2024.1.0/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 readfish-2024.1.0/.github/faq.yml
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 readfish-2024.1.0/.github/faq/FAQ.md
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 readfish-2024.1.0/.github/faq/suggest.md
+-rw-r--r--   0        0        0     4091 2020-02-02 00:00:00.000000 readfish-2024.1.0/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 readfish-2024.1.0/.github/workflows/faqtory.yml
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 readfish-2024.1.0/.github/workflows/stale.yml
+-rw-r--r--   0        0        0    82708 2020-02-02 00:00:00.000000 readfish-2024.1.0/_static/readfish.jpg
+-rw-r--r--   0        0        0   164136 2020-02-02 00:00:00.000000 readfish-2024.1.0/_static/readfish_dark.png
+-rw-r--r--   0        0        0   190609 2020-02-02 00:00:00.000000 readfish-2024.1.0/_static/readfish_light.png
+-rw-r--r--   0        0        0    12731 2020-02-02 00:00:00.000000 readfish-2024.1.0/_static/readfish_logo.jpg
+-rw-r--r--   0        0        0     7046 2020-02-02 00:00:00.000000 readfish-2024.1.0/_static/readfish_small.jpg
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 readfish-2024.1.0/_static/example_tomls/COSMIC_cancer_panel.bed
+-rw-r--r--   0        0        0   228736 2020-02-02 00:00:00.000000 readfish-2024.1.0/_static/images/PlaybackControlRun30Minutes.png
+-rw-r--r--   0        0        0   206755 2020-02-02 00:00:00.000000 readfish-2024.1.0/_static/images/PlaybackRunTargeted.png
+-rw-r--r--   0        0        0   222323 2020-02-02 00:00:00.000000 readfish-2024.1.0/_static/images/PlaybackRunTargetedPeak.png
+-rw-r--r--   0        0        0   224078 2020-02-02 00:00:00.000000 readfish-2024.1.0/_static/images/PlaybackRunTargetedUnblockPeak.png
+-rw-r--r--   0        0        0   155966 2020-02-02 00:00:00.000000 readfish-2024.1.0/_static/images/PlaybackRunUnblock.png
+-rw-r--r--   0        0        0   156826 2020-02-02 00:00:00.000000 readfish-2024.1.0/_static/images/PlaybackRunUnblockCloseUp.png
+-rw-r--r--   0        0        0   202426 2020-02-02 00:00:00.000000 readfish-2024.1.0/_static/images/PlaybackUnblockAll30minutes.png
+-rw-r--r--   0        0        0   211500 2020-02-02 00:00:00.000000 readfish-2024.1.0/_static/images/PlaybackUnblockAllCloseUp.png
+-rw-r--r--   0        0        0   145644 2020-02-02 00:00:00.000000 readfish-2024.1.0/_static/images/Unblock.png
+-rw-r--r--   0        0        0   151624 2020-02-02 00:00:00.000000 readfish-2024.1.0/_static/images/UnblockAllMessages.png
+-rw-r--r--   0        0        0   155720 2020-02-02 00:00:00.000000 readfish-2024.1.0/_static/images/Unblock_closeup.png
+-rw-r--r--   0        0        0   151990 2020-02-02 00:00:00.000000 readfish-2024.1.0/_static/images/control.png
+-rw-r--r--   0        0        0   284161 2020-02-02 00:00:00.000000 readfish-2024.1.0/_static/images/data_model.png
+-rw-r--r--   0        0        0    38123 2020-02-02 00:00:00.000000 readfish-2024.1.0/_static/images/data_model.svg
+-rw-r--r--   0        0        0    38123 2020-02-02 00:00:00.000000 readfish-2024.1.0/_static/images/data_model_no_bg.svg
+-rw-r--r--   0        0        0    69772 2020-02-02 00:00:00.000000 readfish-2024.1.0/_static/images/message.png
+-rw-r--r--   0        0        0   143794 2020-02-02 00:00:00.000000 readfish-2024.1.0/_static/images/minknow_messages.png
+-rw-r--r--   0        0        0   103153 2020-02-02 00:00:00.000000 readfish-2024.1.0/_static/images/simulated_playback_run_options.png
+-rw-r--r--   0        0        0     6826 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/FAQ.md
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/Makefile
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/changelog.md
+-rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/conf.py
+-rw-r--r--   0        0        0    10561 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/developers-guide.md
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/development.yml
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/getting-started.md
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/guppy-params.md
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/index.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/make.bat
+-rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/post-analysis.md
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/readfish.console.rst
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/readfish.plugins.rst
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/readfish.rst
+-rw-r--r--   0        0        0    19103 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/toml.md
+-rw-r--r--   0        0        0   155966 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/images/PlaybackRunUnblock.png
+-rw-r--r--   0        0        0   156826 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/images/PlaybackRunUnblockCloseUp.png
+-rw-r--r--   0        0        0   145644 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/images/Unblock.png
+-rw-r--r--   0        0        0   155720 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/images/Unblock_closeup.png
+-rw-r--r--   0        0        0   151990 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/images/control.png
+-rw-r--r--   0        0        0    69772 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/images/message.png
+-rw-r--r--   0        0        0   143794 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/images/minknow_messages.png
+-rw-r--r--   0        0        0    82708 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/images/readfish.jpg
+-rw-r--r--   0        0        0   237831 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/images/readfish.png
+-rw-r--r--   0        0        0   217946 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/images/readfish_dark.png
+-rw-r--r--   0        0        0    12731 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/images/readfish_logo.jpg
+-rw-r--r--   0        0        0     7046 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/images/readfish_small.jpg
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/questions/batch-times.question.md
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/questions/creating_readfish-environment.question.md
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/questions/key_error_adapter.md
+-rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/questions/py-guppy-client-error.question.md
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/questions/py-guppy-client-version.question.md
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/questions/readfish-branches.question.md
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/__about__.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/__init__.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/__main__.py
+-rw-r--r--   0        0        0    11387 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/_channels.py
+-rw-r--r--   0        0        0     5280 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/_cli_args.py
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/_cli_base.py
+-rw-r--r--   0        0        0    19412 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/_config.py
+-rw-r--r--   0        0        0     4964 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/_loggers.py
+-rw-r--r--   0        0        0     9594 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/_read_until_client.py
+-rw-r--r--   0        0        0    19105 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/_statistics.py
+-rw-r--r--   0        0        0    15654 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/entry_points/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/entry_points/demultiplex.py
+-rw-r--r--   0        0        0     6122 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/entry_points/stats.py
+-rw-r--r--   0        0        0    30418 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/entry_points/targets.py
+-rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/entry_points/unblock_all.py
+-rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/entry_points/validate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/plugins/__init__.py
+-rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/plugins/_filter.py
+-rw-r--r--   0        0        0    12534 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/plugins/_mappy.py
+-rw-r--r--   0        0        0     4037 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/plugins/_no_op.py
+-rw-r--r--   0        0        0     4477 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/plugins/abc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/plugins/deepnano_blitz.py
+-rw-r--r--   0        0        0    11742 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/plugins/guppy.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/plugins/mappy.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/plugins/mappy_rs.py
+-rw-r--r--   0        0        0    34976 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/plugins/utils.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/read_until/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/read_until/_version.py
+-rw-r--r--   0        0        0    25181 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/read_until/base.py
+-rw-r--r--   0        0        0     9205 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/read_until/read_cache.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/conftest.py
+-rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/describe_test.py
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/stats_test.py
+-rw-r--r--   0        0        0     4735 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/utils_test.py
+-rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/validation_test.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/describe_test/describe_aligner_barcoded_expected.txt
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/describe_test/describe_aligner_barcoded_regions_expected.txt
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/describe_test/describe_aligner_regions_expected.txt
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/describe_test/describe_barcoded_experiment_expected.txt
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/describe_test/describe_barcoded_regions_experiment_expected.txt
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/describe_test/describe_experiment_regions_expected.txt
+-rw-r--r--   0        0        0   531281 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/describe_test/yeast_8kb_contigs_test.mmi
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/guppy_validation_test/README.md
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/guppy_validation_test/fail/001_no_write_socket.txt
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/guppy_validation_test/fail/002_missing_socket.txt
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/guppy_validation_test/fail/003_no_read_socket.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/guppy_validation_test/fail/5555_fail_nr
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/guppy_validation_test/fail/5555_fail_nw
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/guppy_validation_test/pass/001_correct_debug.txt
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/guppy_validation_test/pass/002_correct_no_debug.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/guppy_validation_test/pass/5555_pass
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/mappy_validation_test/README.md
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/mappy_validation_test/fail/001_wrong_reference_type.txt
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/mappy_validation_test/fail/002_reference_not_exist.txt
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/mappy_validation_test/fail/003_wrong_reference_type_mmi_gz.txt
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/mappy_validation_test/fail/004_bad_reference_file_extension.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/mappy_validation_test/fail/bad_extension.mmi.cabbage
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/mappy_validation_test/fail/i_am_a_fail_reference.mmi.gz
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/mappy_validation_test/fail/i_am_a_fail_reference.txt
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/mappy_validation_test/pass/001_correct_reference_mmi.txt
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/mappy_validation_test/pass/002_correct_reference_fasta.txt
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/mappy_validation_test/pass/003_correct_reference_fastq.txt
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/mappy_validation_test/pass/004_correct_reference_fasta_gz.txt
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/mappy_validation_test/pass/005_correct_reference_fastq_gz.txt
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/mappy_validation_test/pass/006_passing_fna_mmi.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/mappy_validation_test/pass/GCA_000001405.15_GRCh38_no_alt_analysis_set.fna.mmi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/mappy_validation_test/pass/hello.fasta
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/mappy_validation_test/pass/hello.fasta.gz
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/mappy_validation_test/pass/hello.fastq
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/mappy_validation_test/pass/hello.fastq.gz
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/mappy_validation_test/pass/hello.mmi
+-rw-r--r--   0        0        0    14385 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/stats_test/expected_summary.txt
+-rw-r--r--   0        0        0   997010 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/stats_test/simulated_reads.fastq
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/stats_test/stats.tsv
+-rw-r--r--   0        0        0   531281 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/stats_test/yeast_8kb_contigs_test.mmi
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/toml_validation_test/README.md
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/toml_validation_test/fail/001_missing_keys.txt
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/toml_validation_test/fail/002_wrong_types.txt
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/toml_validation_test/fail/003_plugin_fail_0.txt
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/toml_validation_test/fail/003_plugin_fail_1.txt
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/toml_validation_test/fail/004_target_interval_check.txt
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/toml_validation_test/fail/COSMIC_cancer_panel_errors.bed
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/toml_validation_test/pass/001_simple_toml.txt
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 readfish-2024.1.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 readfish-2024.1.0/LICENSE
+-rw-r--r--   0        0        0    69691 2020-02-02 00:00:00.000000 readfish-2024.1.0/README.md
+-rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 readfish-2024.1.0/pyproject.toml
+-rw-r--r--   0        0        0    72472 2020-02-02 00:00:00.000000 readfish-2024.1.0/PKG-INFO
```

### Comparing `readfish-2023.1.1/.pre-commit-config.yaml` & `readfish-2024.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/CITATION.cff` & `readfish-2024.1.0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/.github/CONTRIBUTING.md` & `readfish-2024.1.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/.github/faq/suggest.md` & `readfish-2024.1.0/.github/faq/suggest.md`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/.github/workflows/CI.yml` & `readfish-2024.1.0/.github/workflows/CI.yml`

 * *Files 6% similar despite different names*

```diff
@@ -43,15 +43,15 @@
       - name: "Run tests"
         run: |
           set -xe
           python -VV
           python -m site
           python -m pip install -U pip setuptools wheel
           python -m pip install -e ".[tests]"
-          coverage run --omit "src/readfish/read_until/*.py" -pm pytest
+          coverage run --omit "src/readfish/read_until/*.py,src/readfish/entry_points/targets.py" -pm pytest
       - name: Upload coverage data
         uses: actions/upload-artifact@v3
         with:
           name: coverage-data
           path: .coverage*
           if-no-files-found: ignore
```

### Comparing `readfish-2023.1.1/.github/workflows/faqtory.yml` & `readfish-2024.1.0/.github/workflows/faqtory.yml`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/.github/workflows/stale.yml` & `readfish-2024.1.0/.github/workflows/stale.yml`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/_static/readfish.jpg` & `readfish-2024.1.0/_static/readfish.jpg`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/_static/readfish_dark.png` & `readfish-2024.1.0/_static/readfish_dark.png`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/_static/readfish_light.png` & `readfish-2024.1.0/_static/readfish_light.png`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/_static/readfish_logo.jpg` & `readfish-2024.1.0/_static/readfish_logo.jpg`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/_static/readfish_small.jpg` & `readfish-2024.1.0/_static/readfish_small.jpg`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/_static/images/PlaybackControlRun30Minutes.png` & `readfish-2024.1.0/_static/images/PlaybackControlRun30Minutes.png`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/_static/images/PlaybackRunTargeted.png` & `readfish-2024.1.0/_static/images/PlaybackRunTargeted.png`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/_static/images/PlaybackRunTargetedPeak.png` & `readfish-2024.1.0/_static/images/PlaybackRunTargetedPeak.png`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/_static/images/PlaybackRunTargetedUnblockPeak.png` & `readfish-2024.1.0/_static/images/PlaybackRunTargetedUnblockPeak.png`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/_static/images/PlaybackRunUnblock.png` & `readfish-2024.1.0/_static/images/PlaybackRunUnblock.png`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/_static/images/PlaybackRunUnblockCloseUp.png` & `readfish-2024.1.0/_static/images/PlaybackRunUnblockCloseUp.png`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/_static/images/PlaybackUnblockAll30minutes.png` & `readfish-2024.1.0/_static/images/PlaybackUnblockAll30minutes.png`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/_static/images/PlaybackUnblockAllCloseUp.png` & `readfish-2024.1.0/_static/images/PlaybackUnblockAllCloseUp.png`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/_static/images/Unblock.png` & `readfish-2024.1.0/_static/images/Unblock.png`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/_static/images/UnblockAllMessages.png` & `readfish-2024.1.0/_static/images/UnblockAllMessages.png`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/_static/images/Unblock_closeup.png` & `readfish-2024.1.0/_static/images/Unblock_closeup.png`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/_static/images/control.png` & `readfish-2024.1.0/_static/images/control.png`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/_static/images/data_model.png` & `readfish-2024.1.0/_static/images/data_model.png`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/_static/images/data_model.svg` & `readfish-2024.1.0/_static/images/data_model.svg`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/_static/images/data_model_no_bg.svg` & `readfish-2024.1.0/_static/images/data_model_no_bg.svg`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/_static/images/message.png` & `readfish-2024.1.0/_static/images/message.png`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/_static/images/minknow_messages.png` & `readfish-2024.1.0/_static/images/minknow_messages.png`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/_static/images/simulated_playback_run_options.png` & `readfish-2024.1.0/_static/images/simulated_playback_run_options.png`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/docs/FAQ.md` & `readfish-2024.1.0/docs/FAQ.md`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/docs/Makefile` & `readfish-2024.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/docs/conf.py` & `readfish-2024.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/docs/developers-guide.md` & `readfish-2024.1.0/docs/developers-guide.md`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/docs/getting-started.md` & `readfish-2024.1.0/docs/getting-started.md`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/docs/guppy-params.md` & `readfish-2024.1.0/docs/guppy-params.md`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/docs/make.bat` & `readfish-2024.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/docs/post-analysis.md` & `readfish-2024.1.0/docs/post-analysis.md`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/docs/readfish.console.rst` & `readfish-2024.1.0/docs/readfish.console.rst`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/docs/readfish.plugins.rst` & `readfish-2024.1.0/docs/readfish.plugins.rst`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/docs/readfish.rst` & `readfish-2024.1.0/docs/readfish.rst`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/docs/toml.md` & `readfish-2024.1.0/docs/toml.md`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/docs/images/PlaybackRunUnblock.png` & `readfish-2024.1.0/docs/images/PlaybackRunUnblock.png`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/docs/images/PlaybackRunUnblockCloseUp.png` & `readfish-2024.1.0/docs/images/PlaybackRunUnblockCloseUp.png`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/docs/images/Unblock.png` & `readfish-2024.1.0/docs/images/Unblock.png`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/docs/images/Unblock_closeup.png` & `readfish-2024.1.0/docs/images/Unblock_closeup.png`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/docs/images/control.png` & `readfish-2024.1.0/docs/images/control.png`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/docs/images/message.png` & `readfish-2024.1.0/docs/images/message.png`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/docs/images/minknow_messages.png` & `readfish-2024.1.0/docs/images/minknow_messages.png`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/docs/images/readfish.jpg` & `readfish-2024.1.0/docs/images/readfish.jpg`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/docs/images/readfish.png` & `readfish-2024.1.0/docs/images/readfish.png`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/docs/images/readfish_dark.png` & `readfish-2024.1.0/docs/images/readfish_dark.png`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/docs/images/readfish_logo.jpg` & `readfish-2024.1.0/docs/images/readfish_logo.jpg`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/docs/images/readfish_small.jpg` & `readfish-2024.1.0/docs/images/readfish_small.jpg`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/docs/questions/batch-times.question.md` & `readfish-2024.1.0/docs/questions/batch-times.question.md`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/docs/questions/creating_readfish-environment.question.md` & `readfish-2024.1.0/docs/questions/creating_readfish-environment.question.md`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/docs/questions/key_error_adapter.md` & `readfish-2024.1.0/docs/questions/key_error_adapter.md`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/docs/questions/py-guppy-client-error.question.md` & `readfish-2024.1.0/docs/questions/py-guppy-client-error.question.md`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/docs/questions/py-guppy-client-version.question.md` & `readfish-2024.1.0/docs/questions/py-guppy-client-version.question.md`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/src/readfish/_channels.py` & `readfish-2024.1.0/src/readfish/_channels.py`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/src/readfish/_cli_args.py` & `readfish-2024.1.0/src/readfish/_cli_args.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,29 @@
 """Store for command line arguments and defaults, these are used by readfish entry points.
 
 These are held here in an agnostic format and the actual CLI is generated by ``readfish._cli_base``.
 The two primary items that are exported are ``BASE_ARGS`` and ``DEVICE_BASE_ARGS`` which define different sets of command line arguments for different purposes.
 ``BASE_ARGS`` are the minimal required arguments for _all_ entry points as they used for initialising loggers.
 ``DEVICE_BASE_ARGS`` are the set of arguments that are used for connecting to a sequencer (device) and some other related settings for selective sequencing scripts.
 """
+
+from enum import Enum, unique
 from readfish._utils import nice_join
 
+
+@unique
+class Chemistry(Enum):
+    #: For the "smarter" version of duplex - does this read map to the previous reads opposite strand on the same contig. Won't work for no map based decisions
+    DUPLEX = "duplex"
+    #: Normal simplex chemistry - no duplex override shenanigans
+    SIMPLEX = "simplex"
+    #: Simple duplex - if we are going to unblock a read given the previous read on the same channel was stop receiving, sequence the current read instead.
+    DUPLEX_SIMPLE = "duplex_simple"
+
+
 DEFAULT_SERVER_HOST = "127.0.0.1"
 DEFAULT_SERVER_PORT = None
 DEFAULT_LOG_FORMAT = "%(asctime)s %(name)s %(message)s"
 DEFAULT_LOG_LEVEL = "info"
 DEFAULT_UNBLOCK = 0.1
 DEFAULT_THROTTLE = 0.4
 DEFAULT_MIN_CHUNK = 2000
@@ -85,15 +98,15 @@
             required=True,
         ),
     ),
     (
         "--unblock-duration",
         dict(
             metavar="UNBLOCK-DURATION",
-            type=int,
+            type=float,
             help="Time, in seconds, to apply unblock voltage (default: {})".format(
                 DEFAULT_UNBLOCK
             ),
             default=DEFAULT_UNBLOCK,
         ),
     ),
     (
@@ -123,13 +136,25 @@
             action="store_true",
             help="Run the readfish Until experiment without sending unblock commands",
         ),
     ),
     (
         "--wait-for-ready",
         dict(
-            help="Timeout for the MinKNOW data folder to appear, and the device to report it is ready to start sequencing. Default 60 seconds.",
+            help="Timeout for the MinKNOW data folder to appear, and the device to report it is ready to start sequencing in seconds. (default: 120s).",
             required=False,
-            default=60,
+            default=120,
+            type=int,
+        ),
+    ),
+    (
+        "--chemistry",
+        dict(
+            help="**EXPERIMENTAL** Choose between duplex and simplex chemistry mode. duplex_simple accepts a read if the previous channels read was stop receiving,"
+            "duplex checks that the previous reads alignment was on the same contig and opposite strand. default: SIMPLEX",
+            required=False,
+            type=str,
+            default=Chemistry.SIMPLEX,
+            choices=[chemistry.value for chemistry in Chemistry],
         ),
     ),
 ) + BASE_ARGS
```

### Comparing `readfish-2023.1.1/src/readfish/_cli_base.py` & `readfish-2024.1.0/src/readfish/_cli_base.py`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/src/readfish/_config.py` & `readfish-2024.1.0/src/readfish/_config.py`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/src/readfish/_loggers.py` & `readfish-2024.1.0/src/readfish/_loggers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 import logging
 import argparse
 from logging.handlers import QueueHandler, QueueListener
 import queue
 from typing import Callable
+from readfish.__about__ import __version__
 
 
 def setup_logger(
     name: str,
     header: str | None = None,
     log_format: str = "%(message)s",
     log_file: str | None = None,
@@ -105,7 +106,8 @@
     :param exclude: A list of attribute names to exclude from the output.
     """
     if exclude is None:
         exclude = []
     for attr in dir(args):
         if attr[0] != "_" and attr not in exclude and attr.lower() == attr:
             printer(f"{attr}={getattr(args, attr)!r}")
+    printer(f"Version={__version__}")
```

### Comparing `readfish-2023.1.1/src/readfish/_read_until_client.py` & `readfish-2024.1.0/src/readfish/_read_until_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,21 +30,23 @@
     protocol_service.PHASE_MUX_SCAN,
     protocol_service.PHASE_RESUMING,
     protocol_service.PHASE_PREPARING_FOR_MUX_SCAN,
     protocol_service.PHASE_PAUSING,
     protocol_service.PHASE_PAUSED,
 }
 #  Timeout in seconds for the run folder to appear
-TIMEOUT = 60
+TIMEOUT = 120
 
 
 class RUClient(ReadUntilClient):
     """Subclasses ONTs read_until_api ReadUntilClient adding extra function that logs unblocks read_ids."""
 
     def __init__(self, *args, **kwargs):
+        #  Default to TIMEOUT in the event we are not starting from the CLI.
+        # If started from CLI args.wait-for-ready is used - also defaults to 120s
         self.timeout = kwargs.pop("timeout", TIMEOUT)
         super().__init__(*args, **kwargs)
         # disable the read until client logger
         self.logger.disabled = True
         self.log = setup_logger(
             __name__,
             level=logging.INFO,
@@ -73,17 +75,17 @@
         self.wait_for_minknow_folder(self.timeout)
         # Attempt to create `unblocked_read_ids.txt` if this fails set the run
         # directory as the PWD this will also affect where the channels.toml
         # file is written to
         try:
             ids_log = self.mk_run_dir.joinpath("unblocked_read_ids.txt")
             ids_log.touch(exist_ok=True)
-        except PermissionError:
+        except (PermissionError, FileNotFoundError):
             # TODO: log message here that fallback output is in use
-            self.mk_run_dir = "."
+            self.mk_run_dir = Path(".")
             ids_log = self.mk_run_dir.joinpath("unblocked_read_ids.txt")
             ids_log.touch(exist_ok=True)
         self.unblock_logger = setup_logger(
             "unblock_logger",
             log_file=ids_log,
             log_format="%(message)s",
             queue_bound=-1,
@@ -166,18 +168,18 @@
             if self.phase_errors < self.max_phase_errors:
                 self.log.info(f"Got RPC exception\n{e}")
                 self.log.info("Run may have ended")
                 self.phase_errors += 1
             else:
                 raise SystemExit(1)
 
-    def wait_for_minknow_folder(self, timeout: int = TIMEOUT):
+    def wait_for_minknow_folder(self, timeout: int):
         """
         Rather than messing about with permissions wait for MinKNOW to create the run
-        folder. If the folder doesn't appear after TIMEOUT seconds then write to the
+        folder. If the folder doesn't appear after timeout seconds then write to the
         current working directory instead.
         """
         seconds_waited = 0
         while (
             not self.mk_run_dir.exists()
             and self.current_protocol_state in ACCEPTABLE_PROTOCOL_STATES
         ):
```

### Comparing `readfish-2023.1.1/src/readfish/_statistics.py` & `readfish-2024.1.0/src/readfish/_statistics.py`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/src/readfish/_utils.py` & `readfish-2024.1.0/src/readfish/_utils.py`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/src/readfish/entry_points/stats.py` & `readfish-2024.1.0/src/readfish/entry_points/stats.py`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/src/readfish/entry_points/targets.py` & `readfish-2024.1.0/src/readfish/entry_points/targets.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,25 +7,38 @@
     #. Initialise a connection to your chosen basecaller
     #. Initialise the read aligner
 
 Then, during sequencing the start of each read is sampled.
 These chunks of raw data are processed by the basecaller to produce FASTA, which is then aligned against the chosen reference genome.
 The result of the alignment is used, along with the targets provided in the :doc:`TOML <toml>` file, to make a decision on each read.
 
+In the new **experimental** Duplex mode, it is possible to override a decision for a read based on the action taken for a previous read.
+This is done by passing `--chemistry` and setting either duplex, or duplex simple.
+`duplex_simple` accepts a read if the previous channels read was stop receiving, `duplex` checks that the previous reads alignment was on the same contig and opposite strand.
+The default chemistry is simplex.
 
 Running this should result in a very short (<1kb, ideally 400-600 bases) unblock peak at the start of a read length histogram and longer sequenced reads.
 
 Example run command::
 
    readfish targets --device X3 \\
            --experiment-name "test" \\
            --toml my_exp.toml \\
            --log-file rf.log \\
            --debug-log chunks.tsv
 
+Example experimental duplex command::
+
+    readfish targets --device X3 \\
+           --experiment-name "test" \\
+           --toml my_exp.toml \\
+           --log-file rf.log \\
+           --debug-log chunks.tsv
+           --chemistry duplex
+
 In the debug_log chunks.tsv file, if this argument is passed, each line represents detailed information about a batch of
 read signal that has been processed in an iteration.
 
 The format of each line is as follows:
 loop_counter  number_reads  read_id  channel  read_number  seq_length  seen_count
 decision  action  condition  barcode  previous_action  timestamp  action_overridden
 
@@ -62,14 +75,15 @@
 +-------------------+-------------+---------------------------------------------------------------------------------------------------------------+
 
 Actions being overridden occurs when the readfish run is a dry run and the action is unblock, or when the read is the first read seen for a channel by readfish.
 This prevents trying to unblock reads of unknown length.
 
 
 """
+
 # Core imports
 from __future__ import annotations
 import argparse
 import logging
 import time
 from timeit import default_timer as timer
 from pathlib import Path
@@ -77,26 +91,32 @@
 
 # Third party imports
 from readfish.read_until.read_cache import AccumulatingCache
 from readfish.read_until import ReadUntilClient
 from minknow_api import protocol_service
 
 # Library
-from readfish._cli_args import DEVICE_BASE_ARGS
+from readfish._cli_args import DEVICE_BASE_ARGS, Chemistry
 from readfish._read_until_client import RUClient
 from readfish._config import Action, Conf, make_decision, _Condition
 from readfish._statistics import ReadfishStatistics
 from readfish._utils import (
     get_device,
     send_message,
     ChunkTracker,
     Severity,
 )
 from readfish.plugins.abc import AlignerABC, CallerABC
-from readfish.plugins.utils import Decision, PreviouslySentActionTracker, Result
+from readfish.plugins.utils import (
+    Decision,
+    PreviouslySentActionTracker,
+    Result,
+    DuplexTracker,
+    Strand,
+)
 
 
 _help = "Run targeted sequencing"
 _cli = DEVICE_BASE_ARGS + (
     (
         "--toml",
         dict(
@@ -119,53 +139,59 @@
             help="Number of bases to pad the target sequences with",
             default=0,
             type=int,
             metavar="PADDING",
         ),
     ),
 )
+# When sequencing in duplex mode, overriding a decided `Action` on a currently sequenced molecule
+# is not allowed if the previous molecules decision was one of these.
+DISALLOWED_DUPLEX_DECISIONS = {Decision.first_read_override, Decision.duplex_override}
 
 
 class Analysis:
     """
     Analysis class where the read until magic happens. Comprises of one run
     function that is run threaded in the run function at the base of this file.
     Arguments listed in the __init__ docs.
 
-    :param client: An instance of the ReadUntilClient object
-    :param conf: An instance of the Conf object
-    :param logger: The command level logger for this module
-    :param debug_log: Whether to output the Debug Log. log Name is generated. Defaults to False.
-    :param throttle: The number of seconds interval between requests to the ReadUntilClient, defaults to 0.1
-    :param unblock_duration: Time, in seconds, to apply unblock voltage, defaults to 0.5
-    :param dry_run: If True unblocks are replaced with `stop_receiving` commands, defaults to False
-    :param toml: The path to the toml file containing experiment conf. Used for reloading, defaults to "a.toml"
+    :param client: An instance of the ReadUntilClient object.
+    :param conf: An instance of the Conf object.
+    :param logger: The command level logger for this module.
+    :param debug_log: Whether to output the Debug Log. log Name is generated.
+    :param throttle: The time interval (seconds) between requests to the ReadUntilClient.
+    :param unblock_duration: Time, in seconds, to apply unblock voltage.
+    :param dry_run: If True unblocks are replaced with `stop_receiving` commands.
+    :param toml: The path to the toml file containing experiment conf. Used as the path for checking if the TOML needs reloading.
+    :param chemistry: Instance of Chemistry Enum, representing the chemistry of the run (Simplex/Duplex). Used for
+        decision making on strands that may be part of a duplex pair.
     """
 
     def __init__(
         self,
         client: ReadUntilClient,
         conf: Conf,
         logger: logging.Logger,
         debug_log: bool,
-        throttle: float = 0.1,
-        unblock_duration: float = 0.5,
-        dry_run: bool = False,
-        toml: str = "a.toml",
+        throttle: float,
+        unblock_duration: float,
+        dry_run: bool,
+        toml: str,
+        chemistry: Chemistry,
     ):
         self.client = client
         self.conf = conf
         self.logger = logger
         self.debug_log = debug_log
         self.throttle = throttle
         self.unblock_duration = unblock_duration
         self.dry_run = dry_run
         self.live_toml = Path(f"{toml}_live").resolve()
         self.run_information = self.client.connection.protocol.get_run_info()
-
+        self.chemistry = chemistry
         # Generate a run specific read log
         read_log_name = (
             f"{self.run_information.run_id}_readfish.tsv" if debug_log else None
         )
 
         self.logger.info("Fetching Run Configuration")
         self.break_reads_after_seconds = (
@@ -190,14 +216,16 @@
         self.mapper: AlignerABC = self.conf.mapper_settings.load_object("Aligner")
         self.logger.info("Aligner initialised")
         # count how often a read is seen
         self.chunk_tracker = ChunkTracker(self.client.channel_count)
 
         # This is an object to keep track of the last action sent to the client for each channel
         self.previous_action_tracker = PreviouslySentActionTracker()
+        # Keep track of previous alignments
+        self.duplex_tracker = DuplexTracker()
 
         # We assume that sequencing is already running.
         # If the run is not in sequencing phase when the read until loop starts will
         # be set to false and the first read seen can be unblocked.
         self.readfish_started_during_sequencing = True
 
         # This is a flag to prevent repeated logging of the same message
@@ -259,17 +287,19 @@
         """
         Check the chosen Action and amend it based on conditional checks.
         The action lists are appended to in place, so no return is required.
 
         Checks include:
             1. If the read is in a control region, the action is always stop_receiving.
             1. If the read is below the minimum chunks, use value in toml or default to proceed
-            1. If the read is above the maximum chunks, use value in toml or default unblock
+            1. If the read is above the maximum chunks, use value in toml or default unblock--throttle
             1. First read seen for channel and readfish started during sequencing, override to stop_receiving
             1. If action is unblock and we are dry-running, override to stop_receiving
+            1. If we are running in duplex chemistry, check the previous reads final decision and Action, and potentially sequence
+                the current read, instead of unblocking it.
 
         :param control: Indicates read from a channel in a control region
         :param action: What action was decided for this read before any meddling
         :param result: Information about the current read.
         :param seen_count: Number of times other chunks from the read have been observed.
         :param condition: The set of conditions for deciding the action.
         :param stop_receiving_action_list: List to append channels and read numbers for which 'stop receiving' action is decided.
@@ -302,37 +332,98 @@
             if below_min_chunks and action is not Action.proceed:
                 action = condition.below_min_chunks
                 result.decision = Decision.below_min_chunks
 
         # previous_action will be None if the read has not been seen before.
         previous_action = self.previous_action_tracker.get_action(result.channel)
         action_overridden = False
+        # If --duplex flag override decisions made based on the strand and contig alignment of the previous read.
+        # Unfinished bruv
+        if (
+            self.chemistry is Chemistry.DUPLEX
+            # Easy checks first, so wdon't do more complex processing unless we have to
+            and action == Action.unblock
+            and previous_action is Action.stop_receiving
+        ):
+            # Check if we think this read is possibly duplex
+            possible_duplex = any(
+                self.duplex_tracker.possible_duplex(
+                    result.channel, result.read_id, al.ctg, al.strand
+                )
+                for al in result.alignment_data
+            )
+            # Check the previous decision for this channel was not already an override
+            previous_decision_allowed = (
+                self.duplex_tracker.get_previous_decision(result.channel)
+                not in DISALLOWED_DUPLEX_DECISIONS
+            )
+            if possible_duplex and previous_decision_allowed:
+                self.logger.debug(
+                    f"Overriding read {result.read_id} as it is possibly second half of a duplex"
+                    f"- previous read action {previous_action}, current_action: {action},"
+                    f" previous_decision: {self.duplex_tracker.get_previous_decision(result.channel)}"
+                )
+                action_overridden = True
+                result.decision = Decision.duplex_override
+                action = Action.stop_receiving
+        # Duplex
+        elif (
+            self.chemistry is Chemistry.DUPLEX_SIMPLE
+            and previous_action is Action.stop_receiving
+            and action is Action.unblock
+        ):
+            previous_decision_allowed = (
+                self.duplex_tracker.get_previous_decision(result.channel)
+                not in DISALLOWED_DUPLEX_DECISIONS
+            )
+            if previous_decision_allowed:
+                self.logger.debug(
+                    f"Overriding to duplex - previous read action {previous_action}, current_action: {action},"
+                    f" previous_decision: {self.duplex_tracker.get_previous_decision(result.channel)}"
+                )
+                action = Action.stop_receiving
+                action_overridden = True
+                result.decision = Decision.duplex_override
 
+        # Override to stop receiving if this is the first read ona channel and we started mid sequencing
         if previous_action is None and self.readfish_started_during_sequencing:
             self.logger.debug(
                 f"This is the first suitable read chunk from channel {result.channel}. Translocated read length unknown, sequencing."
             )
             action_overridden = True
+            result.decision = Decision.first_read_override
             action = Action.stop_receiving
 
         if action is Action.stop_receiving:
             stop_receiving_action_list.append((result.channel, result.read_number))
-            # Add decided Action
-            self.previous_action_tracker.add_action(result.channel, action)
+
         elif action is Action.unblock:
             if self.dry_run:
                 # Log an 'unblock' action to previous action, but send a 'stop receiving' to prevent further read processing.
                 action_overridden = True
                 stop_receiving_action_list.append((result.channel, result.read_number))
             else:
                 unblock_batch_action_list.append(
                     (result.channel, result.read_number, result.read_id)
                 )
+
+        # If we have made a final decision for this read and we shouldn't see it again!
+        if action is Action.unblock or action is Action.stop_receiving:
             # Add decided Action
             self.previous_action_tracker.add_action(result.channel, action)
+            # Add duplex based tracking if we are in duplex mode
+            if self.chemistry is Chemistry.DUPLEX_SIMPLE:
+                self.duplex_tracker.set_decision(result.channel, result.decision)
+            elif self.chemistry is Chemistry.DUPLEX:
+                self.duplex_tracker.set_decision(result.channel, result.decision)
+                self.duplex_tracker.set_alignments(
+                    result.channel,
+                    [(al.ctg, Strand(al.strand)) for al in result.alignment_data],
+                )
+
         return (
             previous_action,
             action_overridden,
             action.name if action_overridden else None,
         )
 
     def run(self):
@@ -526,14 +617,15 @@
         conf=conf,
         logger=logger,
         debug_log=args.debug_log,
         unblock_duration=args.unblock_duration,
         throttle=args.throttle,
         dry_run=args.dry_run,
         toml=args.toml,
+        chemistry=Chemistry(args.chemistry),
     )
 
     # begin readfish function
     try:
         worker.run()
     except KeyboardInterrupt:
         logger.info("Keyboard interrupt received, stopping readfish.")
```

### Comparing `readfish-2023.1.1/src/readfish/entry_points/unblock_all.py` & `readfish-2024.1.0/src/readfish/entry_points/unblock_all.py`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/src/readfish/entry_points/validate.py` & `readfish-2024.1.0/src/readfish/entry_points/validate.py`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/src/readfish/plugins/_filter.py` & `readfish-2024.1.0/src/readfish/plugins/_filter.py`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/src/readfish/plugins/_mappy.py` & `readfish-2024.1.0/src/readfish/plugins/_mappy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Mapping interface for readfish, using Minimap2 mappy, or mappy-rs as dictated by the experiment TOML
 `mapper_settings.<PLUGIN>` section. See {ref}`plugin configuration <plugins-config>` section.
 """
+
 from __future__ import annotations
 from enum import Enum
 from itertools import chain, repeat
 from pathlib import Path
 from typing import Optional, Iterable
 
 from readfish._loggers import setup_logger
@@ -83,18 +84,15 @@
         """
         index: str = self.aligner_params["fn_idx_in"]
         file_extensions = [".fasta", ".fna", ".fsa", ".fa", ".fastq", ".fq"]
         file_extensions.extend([f"{f}.gz" for f in file_extensions])
         file_extensions.append(".mmi")
         if all((not Path(index).is_file(), index)):
             raise FileNotFoundError(f"{index} does not exist")
-        if (
-            "".join(map(str.lower, Path(index).suffixes)) not in set(file_extensions)
-            and index
-        ):
+        if not any(index.lower().endswith(suffix) for suffix in file_extensions):
             raise RuntimeError(
                 f"Provided index file appears to be of an incorrect type - should be one of {file_extensions}"
             )
 
     def disconnect(self) -> None:
         return
```

### Comparing `readfish-2023.1.1/src/readfish/plugins/_no_op.py` & `readfish-2024.1.0/src/readfish/plugins/_no_op.py`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/src/readfish/plugins/abc.py` & `readfish-2024.1.0/src/readfish/plugins/abc.py`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/src/readfish/plugins/guppy.py` & `readfish-2024.1.0/src/readfish/plugins/guppy.py`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/src/readfish/plugins/utils.py` & `readfish-2024.1.0/src/readfish/plugins/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,14 +26,24 @@
     """Enum representing the forward and reverse strand of DNA for alignments"""
 
     #: Forward strand
     forward = "+"
     #: Reverse strand
     reverse = "-"
 
+    def __invert__(self):
+        """Flip the strand, using bitwise NOT (~)
+
+        >>> ~Strand.forward
+        <Strand.reverse: '-'>
+        >>> ~Strand.reverse
+        <Strand.forward: '+'>
+        """
+        return Strand.forward if self is Strand.reverse else Strand.reverse
+
 
 STRANDS = {
     1: Strand.forward,
     "+": Strand.forward,
     Strand.forward: Strand.forward,
     -1: Strand.reverse,
     "-": Strand.reverse,
@@ -156,19 +166,24 @@
 
     >>> nested_list_dict = {"a": [], "b": [{}], "c": [[1, 2, [1, 2]], [], []]}
     >>> count_dict_elements(nested_list_dict)
     1
     """
     return sum(
         (
-            count_dict_elements(v) if isinstance(v, dict)
-            # If v is a list, tuple, sequence, dict etc., return the length of the container filtering out any empty sun elements,
-            else len(list(filterfalse(partial(is_empty), v)))
-            if isinstance(v, Container)
-            else 1
+            (
+                count_dict_elements(v)
+                if isinstance(v, dict)
+                # If v is a list, tuple, sequence, dict etc., return the length of the container filtering out any empty sun elements,
+                else (
+                    len(list(filterfalse(partial(is_empty), v)))
+                    if isinstance(v, Container)
+                    else 1
+                )
+            )
             for v in d.values()
         )
     )
 
 
 def _calculate_length(target_interval: TARGET_INTERVAL, genomes: dict[str, int]) -> int:
     """
@@ -416,14 +431,18 @@
     no_map = "no_map"
     #: The read did not basecall
     no_seq = "no_seq"
     #: Too many signal chunks have been collected for this read
     above_max_chunks = "above_max_chunks"
     #: Fewer signal chunks for this read collected than required
     below_min_chunks = "below_min_chunks"
+    #: Potential second half of a duplex read
+    duplex_override = "duplex_override"
+    #: Read sequenced as translocated portion was of unknown length at start of readfish
+    first_read_override = "first_read_override"
 
 
 @unique
 class Action(Enum):
     """
     Action to take for a read.
 
@@ -788,7 +807,115 @@
         This method checks the last action sent for a channel, returning the action if it exists,
         otherwise returning None.
 
         :param channel: The channel to check the last action for.
         :return: The last action sent for the channel, or None if no action has been sent.
         """
         return self.last_actions.get(channel, None)
+
+
+@attrs.define
+class DuplexTracker:
+    """
+    Wrapper class to keep track the alignment location of the latest read seen on a channel,
+    and previous decision made, tracking whether we made a duplex override on the last read
+    Specifically, we store a list of tuples of any target contig names and strands that were aligned to,
+    keyed to channel number and the previous decision for a read made on that channel.
+    The decision should only be updated when a read has been finalised and should not be seen again,
+    i.e a Stop receiving or Unblock has been sent to MinKNOW
+    No maps are specified as (*, *)
+    """
+
+    # Note - `readfish.src.plugins.utils.Alignment` could be used here, instead of tuple[str, Strand]
+    # We could then use the results of the ALignment directly, if we ever wanted to do something more complex
+    # for duplex
+    previous_alignments: Dict[int, list[tuple[str, Strand]]] = attrs.Factory(dict)
+    previous_decision: Dict[int, Decision] = attrs.Factory(dict)
+
+    def get_previous_decision(self, channel: int) -> Decision:
+        """
+        Get the previous decision seen on this channel.
+
+        :param channel: The channel number.
+        :return: Previously seen decision
+        >>> dt = DuplexTracker()
+        >>> dt.get_previous_decision(1) is None
+        True
+        >>> dt.set_decision(1, Decision.duplex_override)
+        >>> dt.get_previous_decision(1)
+        <Decision.duplex_override: 'duplex_override'>
+        """
+        return self.previous_decision.get(channel, None)
+
+    def set_decision(self, channel: int, decision: Decision) -> None:
+        """
+        Set the previous decision for a given channel number.
+
+        :param channel: The channel number.
+        :param decision: The decision taken. Should be the final decision,
+        i.e we won't see the read again.
+        >>> dt = DuplexTracker()
+        >>> dt.set_decision(1, Decision.no_map)
+        >>> dt.previous_decision[1]
+        <Decision.no_map: 'no_map'>
+        """
+        self.previous_decision[channel] = decision
+
+    def get_previous_alignments(self, channel: int) -> list[tuple[str, Strand]]:
+        """
+        Retrieves last alignments, including no maps seen on the given channel.
+
+        :param channel: The channel number to lookup the previous action for
+        :param read_id: Read of ID of the current alignment
+        :return: Returns a tuple of (contig_name, strand), for the last alignment seen on this channel
+
+        >>> dt = DuplexTracker()
+        >>> dt.get_previous_alignments(1) is None
+        True
+        >>> dt.set_alignments(1, [("contig1", Strand.forward), ("contig2", Strand.reverse)])
+        >>> dt.get_previous_alignments(1)
+        [('contig1', <Strand.forward: '+'>), ('contig2', <Strand.reverse: '-'>)]
+        """
+        return self.previous_alignments.get(channel, None)
+
+    def set_alignments(
+        self, channel: int, alignments: list[tuple[str, Strand]]
+    ) -> None:
+        """
+        Add an alignment that has been seen for a channel.
+
+        :param channel: The channel number to set the alignment for.
+        :param target_name: The name of the target contig aligned to
+        :param strand: The strand we have aligned to.
+
+        >>> dt = DuplexTracker()
+        >>> dt.set_alignments(1, [("contig3", Strand.forward), ("contig4", Strand.reverse)])
+        >>> dt.previous_alignments[1]
+        [('contig3', <Strand.forward: '+'>), ('contig4', <Strand.reverse: '-'>)]
+        """
+        self.previous_alignments[channel] = alignments
+
+    def possible_duplex(
+        self, channel: int, target_name: str, strand: Strand | str | int
+    ) -> bool:
+        """
+        Compare the current alignment target_name and strand for a given channel
+        with the previous alignment target_name and strand.
+
+        If the strand is opposite and the target is the same, return True, else False.
+        :param channel: Channel number to fetch alignment for
+        :param target_name: The name of the target contig for the current alignment
+        :param strand: The strand of the current alignment
+        :return: True if the strand is opposite and target contig the same
+
+        >>> dt = DuplexTracker()
+        >>> dt.set_alignments(1, [("contig5", Strand.forward)])
+        >>> dt.possible_duplex(1, "contig5", Strand.reverse)
+        True
+        >>> dt.possible_duplex(1, "contig6", Strand.reverse)
+        False
+        """
+        strand = Strand(strand)
+        return any(
+            prev_alignment == (target_name, ~strand)
+            for prev_alignment in self.get_previous_alignments(channel)
+        )
```

### Comparing `readfish-2023.1.1/src/readfish/read_until/base.py` & `readfish-2024.1.0/src/readfish/read_until/base.py`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/src/readfish/read_until/read_cache.py` & `readfish-2024.1.0/src/readfish/read_until/read_cache.py`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/tests/describe_test.py` & `readfish-2024.1.0/tests/describe_test.py`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/tests/stats_test.py` & `readfish-2024.1.0/tests/stats_test.py`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/tests/utils_test.py` & `readfish-2024.1.0/tests/utils_test.py`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/tests/validation_test.py` & `readfish-2024.1.0/tests/validation_test.py`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/tests/static/describe_test/describe_aligner_barcoded_expected.txt` & `readfish-2024.1.0/tests/static/describe_test/describe_aligner_barcoded_expected.txt`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/tests/static/describe_test/describe_aligner_barcoded_regions_expected.txt` & `readfish-2024.1.0/tests/static/describe_test/describe_aligner_barcoded_regions_expected.txt`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/tests/static/describe_test/describe_barcoded_regions_experiment_expected.txt` & `readfish-2024.1.0/tests/static/describe_test/describe_barcoded_regions_experiment_expected.txt`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/tests/static/describe_test/describe_experiment_regions_expected.txt` & `readfish-2024.1.0/tests/static/describe_test/describe_experiment_regions_expected.txt`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/tests/static/describe_test/yeast_8kb_contigs_test.mmi` & `readfish-2024.1.0/tests/static/describe_test/yeast_8kb_contigs_test.mmi`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/tests/static/guppy_validation_test/README.md` & `readfish-2024.1.0/tests/static/guppy_validation_test/README.md`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/tests/static/mappy_validation_test/README.md` & `readfish-2024.1.0/tests/static/mappy_validation_test/README.md`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/tests/static/stats_test/expected_summary.txt` & `readfish-2024.1.0/tests/static/stats_test/expected_summary.txt`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/tests/static/stats_test/simulated_reads.fastq` & `readfish-2024.1.0/tests/static/stats_test/simulated_reads.fastq`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/tests/static/stats_test/stats.tsv` & `readfish-2024.1.0/tests/static/stats_test/stats.tsv`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/tests/static/stats_test/yeast_8kb_contigs_test.mmi` & `readfish-2024.1.0/tests/static/stats_test/yeast_8kb_contigs_test.mmi`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/tests/static/toml_validation_test/README.md` & `readfish-2024.1.0/tests/static/toml_validation_test/README.md`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/tests/static/toml_validation_test/fail/004_target_interval_check.txt` & `readfish-2024.1.0/tests/static/toml_validation_test/fail/004_target_interval_check.txt`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/.gitignore` & `readfish-2024.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/LICENSE` & `readfish-2024.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/README.md` & `readfish-2024.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -241,39 +241,43 @@
 </details>
 <!-- end-simulate -->
 
 <!-- #### Configuring bulk FAST5 file Playback -->
 
 <details style="margin-top: 10px"><summary id="configuring-bulk-fast5-file"><h3 style="display: inline;">Configuring bulk FAST5 file Playback</h3></summary>
 
-Download an open access bulk FAST5 file, either [R9.4.1][bulk - R9] or [R10 (5khz)][bulk - R10 5khz].
+Download an open access bulk FAST5 file, either [R9.4.1 4khz][bulk - R9.4.1] or [R10 (5khz)][bulk - R10.4 5khz].
 This file is 21Gb so make sure you have sufficient space.
+A promethION bulkfile is also available but please note this is [R10.4 4khz][bulk - promethION - R10.4 4khz] and so will give slightly unexpected results on MinKNOW which assumes 5khz.
+This file is approx 35Gb in size.
 
 <!-- begin-new-playback -->
 Previously to set up Playback using a pre-recorded bulk FAST5 file, it was necessary to edit the sequencing configuration file that MinKNOW uses. This is currently no longer the case. The "old method" steps are left after this section for reference only or if the direct playback from a bulk file option is removed in future.
 
 To start sequencing using playback, simply begin setting up the run in the MinKNOW UI as you would usually. 
 Under Run Options you can select Simulated Playback and browse to the downloaded Bulk Fast5 file.
 
 ![Run Options Screenshot](https://github.com/LooseLab/readfish/blob/247185a1bdcbe1275c55a6b4b1e2c7273213af91/docs/_static/images/simulated_playback_run_options.png?raw=true "Run Options Screenshot")
 
 <!-- Included so these work in the github pages docs as well  -->
 [bulk - R9.4.1]: https://s3.amazonaws.com/nanopore-human-wgs/bulkfile/PLSP57501_20170308_FNFAF14035_MN16458_sequencing_run_NOTT_Hum_wh1rs2_60428.fast5
 [bulk - R10.4 5khz]: https://s3.amazonaws.com/nanopore-human-wgs/bulkfile/GXB02001_20230509_1250_FAW79338_X3_sequencing_run_NA12878_B1_19382aa5_ef4362cd.fast5
-
+[bulk - promethION - R10.4 4khz]: https://s3.amazonaws.com/nanopore-human-wgs/bulkfile/PC24B243_20220512_1516_PAK21362_3H_sequencing_run_NA12878_sheared20kb_3d5147fc.fast5
 <!-- end-new-playback -->
 > [!NOTE]  
 > Note - The below instructions, whilst they will still work, are no longer required. They are left here for reference only. As of Minknow 5.7, it is possible to select a bulk FAST5 file for playback in the MinKNOW UI.
 <!-- begin-obsolete -->
 
 <details style="margin-top: 10px"><summary id="configuring-sequencing-toml"><h3 style="display: inline;">Old method Configuring bulk FAST5 file Playback</h3></summary>
 To setup a simulation the sequencing configuration file that MinKNOW uses must be edited.
 Steps:
 
-1. Download an open access bulkfile - either [R9.4.1][bulk - R9] or [R10 (5khz)][bulk - R10 5khz]. These files are aproximately 21Gb so make sure you have plenty of space. The files are from NA12878 sequencing data using either R9.4.1 or R10.4 pores. Data is not barcoded and the libraries were ligation preps from DNA extracted from cell lines.
+1. Download an open access bulkfile - either [R9.4.1][bulk - R9.4.1] or [R10 (5khz)][bulk - R10.4 5khz]. These files are approximately 21Gb so make sure you have plenty of space. The files are from NA12878 sequencing data using either R9.4.1 or R10.4 pores. Data is not barcoded and the libraries were ligation preps from DNA extracted from cell lines. 
+
+1. A promethION bulkfile is also available but please note this is [R10.4, 4khz][bulk - promethION - R10.4 4khz], and so will give slightly unexpected results on MinKNOW which assumes 5khz.
 1. Copy a sequencing TOML file to the `user_scripts` folder:
 
     On Mac if your MinKNOW output directory is the default:
 
     ```console
     mkdir -p /Library/MinKNOW/data/user_scripts/simulations
     cp /Applications/MinKNOW.app/Contents/Resources/conf/package/sequencing/sequencing_MIN106_DNA.toml /Library/MinKNOW/data/user_scripts/simulations/sequencing_MIN106_DNA_sim.toml
@@ -541,20 +545,21 @@
 
 From the Nanopore World:
 Nick Loman, Josh Quick, John Tyson, Jared Simpson, Ewan Birney, Alexander Senf, Nick Goldman, Miten Jain, Lukas Weilguny
 
 And for our Awesome Logo please checkout out [@tim_bassford](https://twitter.com/tim_bassford) from [@TurbineCreative](https://twitter.com/TurbineCreative)!
 
 <!-- end-epilog -->
-[bulk - R9]: https://s3.amazonaws.com/nanopore-human-wgs/bulkfile/PLSP57501_20170308_FNFAF14035_MN16458_sequencing_run_NOTT_Hum_wh1rs2_60428.fast5
-[bulk - R10 5khz]: https://s3.amazonaws.com/nanopore-human-wgs/bulkfile/GXB02001_20230509_1250_FAW79338_X3_sequencing_run_NA12878_B1_19382aa5_ef4362cd.fast5
 [ONT]: https://nanoporetech.com
 
 <!-- start-changelog -->
 # Changelog
-## Unreleased changes
-None currently.
+## 2024.1.0
+1. bug fix type for `--wait-on-ready` type and actual function [(#327)](https://github.com/LooseLab/readfish/pull/327), [(#323)](https://github.com/LooseLab/readfish/pull/323)
+1. mutiple suffix `.mmi` support [(#330)](https://github.com/LooseLab/readfish/pull/330)
+1. Change the default `unblock_duration` on the `Analysis` class to use `DEFAULT_UNBLOCK` value defined in `_cli_args.py`. Change type on the Argparser for `--unblock-duration` to float. [(#313)](https://github.com/LooseLab/readfish/pull/313)
+1. Big dog Duplex feature - adds ability to select duplex reads that cover a target region. See pull request for details [(#324)](https://github.com/LooseLab/readfish/pull/324)
 ## 2023.1.1
 1. Fix Readme Logo link 🥳 (#296)
 1. Fix bug where we had accidentally started requiring barcoded TOMLs to specify a region. Thanks to @jamesemery for catching this. (#299)
 1. Correctly handle overriding a decision in internal statistics tracking. (#299)
 <!-- end-changelog -->
```

### Comparing `readfish-2023.1.1/pyproject.toml` & `readfish-2024.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `readfish-2023.1.1/PKG-INFO` & `readfish-2024.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: readfish
-Version: 2023.1.1
+Version: 2024.1.0
 Summary: ONT adaptive sampling
 Project-URL: Documentation, https://looselab.github.io/readfish
 Project-URL: Bug Tracker, https://github.com/LooseLab/readfish/issues
 Project-URL: Source Code, https://github.com/LooseLab/readfish
 Author: Alexander Payne
 Author-email: Rory Munro <rory.munro@nottingham.ac.uk>, Matt Loose <matt.loose@nottingham.ac.uk>
 License-Expression: MIT
@@ -28,18 +28,28 @@
 Requires-Dist: minknow-api
 Requires-Dist: more-itertools
 Requires-Dist: numpy
 Requires-Dist: readfish-summarise>=0.2.5
 Requires-Dist: readfish[all]
 Requires-Dist: rtoml
 Provides-Extra: all
-Requires-Dist: readfish[guppy,mappy,mappy-rs]; extra == 'all'
+Requires-Dist: mappy; extra == 'all'
+Requires-Dist: mappy-rs>=0.0.6; extra == 'all'
+Requires-Dist: ont-pyguppy-client-lib; extra == 'all'
 Provides-Extra: dev
+Requires-Dist: coverage[toml]; extra == 'dev'
+Requires-Dist: faqtory; extra == 'dev'
+Requires-Dist: furo; extra == 'dev'
+Requires-Dist: mappy; extra == 'dev'
+Requires-Dist: mappy-rs>=0.0.6; extra == 'dev'
+Requires-Dist: myst-parser; extra == 'dev'
+Requires-Dist: ont-pyguppy-client-lib; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
-Requires-Dist: readfish[all,docs,tests]; extra == 'dev'
+Requires-Dist: pytest; extra == 'dev'
+Requires-Dist: sphinx-copybutton; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: faqtory; extra == 'docs'
 Requires-Dist: furo; extra == 'docs'
 Requires-Dist: myst-parser; extra == 'docs'
 Requires-Dist: sphinx-copybutton; extra == 'docs'
 Provides-Extra: guppy
 Requires-Dist: ont-pyguppy-client-lib; extra == 'guppy'
@@ -47,15 +57,18 @@
 Requires-Dist: mappy; extra == 'mappy'
 Provides-Extra: mappy-rs
 Requires-Dist: mappy-rs>=0.0.6; extra == 'mappy-rs'
 Provides-Extra: tests
 Requires-Dist: coverage[toml]; extra == 'tests'
 Requires-Dist: pytest; extra == 'tests'
 Provides-Extra: tests-mappy
-Requires-Dist: readfish[guppy,mappy,tests]; extra == 'tests-mappy'
+Requires-Dist: coverage[toml]; extra == 'tests-mappy'
+Requires-Dist: mappy; extra == 'tests-mappy'
+Requires-Dist: ont-pyguppy-client-lib; extra == 'tests-mappy'
+Requires-Dist: pytest; extra == 'tests-mappy'
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img src="https://github.com/LooseLab/readfish/blob/main/docs/_static/readfish_logo.jpg?raw=true">
 </p>
 
 If you are anything like us (Matt), reading a README is the last thing you do when running code.
@@ -297,39 +310,43 @@
 </details>
 <!-- end-simulate -->
 
 <!-- #### Configuring bulk FAST5 file Playback -->
 
 <details style="margin-top: 10px"><summary id="configuring-bulk-fast5-file"><h3 style="display: inline;">Configuring bulk FAST5 file Playback</h3></summary>
 
-Download an open access bulk FAST5 file, either [R9.4.1][bulk - R9] or [R10 (5khz)][bulk - R10 5khz].
+Download an open access bulk FAST5 file, either [R9.4.1 4khz][bulk - R9.4.1] or [R10 (5khz)][bulk - R10.4 5khz].
 This file is 21Gb so make sure you have sufficient space.
+A promethION bulkfile is also available but please note this is [R10.4 4khz][bulk - promethION - R10.4 4khz] and so will give slightly unexpected results on MinKNOW which assumes 5khz.
+This file is approx 35Gb in size.
 
 <!-- begin-new-playback -->
 Previously to set up Playback using a pre-recorded bulk FAST5 file, it was necessary to edit the sequencing configuration file that MinKNOW uses. This is currently no longer the case. The "old method" steps are left after this section for reference only or if the direct playback from a bulk file option is removed in future.
 
 To start sequencing using playback, simply begin setting up the run in the MinKNOW UI as you would usually. 
 Under Run Options you can select Simulated Playback and browse to the downloaded Bulk Fast5 file.
 
 ![Run Options Screenshot](https://github.com/LooseLab/readfish/blob/247185a1bdcbe1275c55a6b4b1e2c7273213af91/docs/_static/images/simulated_playback_run_options.png?raw=true "Run Options Screenshot")
 
 <!-- Included so these work in the github pages docs as well  -->
 [bulk - R9.4.1]: https://s3.amazonaws.com/nanopore-human-wgs/bulkfile/PLSP57501_20170308_FNFAF14035_MN16458_sequencing_run_NOTT_Hum_wh1rs2_60428.fast5
 [bulk - R10.4 5khz]: https://s3.amazonaws.com/nanopore-human-wgs/bulkfile/GXB02001_20230509_1250_FAW79338_X3_sequencing_run_NA12878_B1_19382aa5_ef4362cd.fast5
-
+[bulk - promethION - R10.4 4khz]: https://s3.amazonaws.com/nanopore-human-wgs/bulkfile/PC24B243_20220512_1516_PAK21362_3H_sequencing_run_NA12878_sheared20kb_3d5147fc.fast5
 <!-- end-new-playback -->
 > [!NOTE]  
 > Note - The below instructions, whilst they will still work, are no longer required. They are left here for reference only. As of Minknow 5.7, it is possible to select a bulk FAST5 file for playback in the MinKNOW UI.
 <!-- begin-obsolete -->
 
 <details style="margin-top: 10px"><summary id="configuring-sequencing-toml"><h3 style="display: inline;">Old method Configuring bulk FAST5 file Playback</h3></summary>
 To setup a simulation the sequencing configuration file that MinKNOW uses must be edited.
 Steps:
 
-1. Download an open access bulkfile - either [R9.4.1][bulk - R9] or [R10 (5khz)][bulk - R10 5khz]. These files are aproximately 21Gb so make sure you have plenty of space. The files are from NA12878 sequencing data using either R9.4.1 or R10.4 pores. Data is not barcoded and the libraries were ligation preps from DNA extracted from cell lines.
+1. Download an open access bulkfile - either [R9.4.1][bulk - R9.4.1] or [R10 (5khz)][bulk - R10.4 5khz]. These files are approximately 21Gb so make sure you have plenty of space. The files are from NA12878 sequencing data using either R9.4.1 or R10.4 pores. Data is not barcoded and the libraries were ligation preps from DNA extracted from cell lines. 
+
+1. A promethION bulkfile is also available but please note this is [R10.4, 4khz][bulk - promethION - R10.4 4khz], and so will give slightly unexpected results on MinKNOW which assumes 5khz.
 1. Copy a sequencing TOML file to the `user_scripts` folder:
 
     On Mac if your MinKNOW output directory is the default:
 
     ```console
     mkdir -p /Library/MinKNOW/data/user_scripts/simulations
     cp /Applications/MinKNOW.app/Contents/Resources/conf/package/sequencing/sequencing_MIN106_DNA.toml /Library/MinKNOW/data/user_scripts/simulations/sequencing_MIN106_DNA_sim.toml
@@ -597,20 +614,21 @@
 
 From the Nanopore World:
 Nick Loman, Josh Quick, John Tyson, Jared Simpson, Ewan Birney, Alexander Senf, Nick Goldman, Miten Jain, Lukas Weilguny
 
 And for our Awesome Logo please checkout out [@tim_bassford](https://twitter.com/tim_bassford) from [@TurbineCreative](https://twitter.com/TurbineCreative)!
 
 <!-- end-epilog -->
-[bulk - R9]: https://s3.amazonaws.com/nanopore-human-wgs/bulkfile/PLSP57501_20170308_FNFAF14035_MN16458_sequencing_run_NOTT_Hum_wh1rs2_60428.fast5
-[bulk - R10 5khz]: https://s3.amazonaws.com/nanopore-human-wgs/bulkfile/GXB02001_20230509_1250_FAW79338_X3_sequencing_run_NA12878_B1_19382aa5_ef4362cd.fast5
 [ONT]: https://nanoporetech.com
 
 <!-- start-changelog -->
 # Changelog
-## Unreleased changes
-None currently.
+## 2024.1.0
+1. bug fix type for `--wait-on-ready` type and actual function [(#327)](https://github.com/LooseLab/readfish/pull/327), [(#323)](https://github.com/LooseLab/readfish/pull/323)
+1. mutiple suffix `.mmi` support [(#330)](https://github.com/LooseLab/readfish/pull/330)
+1. Change the default `unblock_duration` on the `Analysis` class to use `DEFAULT_UNBLOCK` value defined in `_cli_args.py`. Change type on the Argparser for `--unblock-duration` to float. [(#313)](https://github.com/LooseLab/readfish/pull/313)
+1. Big dog Duplex feature - adds ability to select duplex reads that cover a target region. See pull request for details [(#324)](https://github.com/LooseLab/readfish/pull/324)
 ## 2023.1.1
 1. Fix Readme Logo link 🥳 (#296)
 1. Fix bug where we had accidentally started requiring barcoded TOMLs to specify a region. Thanks to @jamesemery for catching this. (#299)
 1. Correctly handle overriding a decision in internal statistics tracking. (#299)
 <!-- end-changelog -->
```

