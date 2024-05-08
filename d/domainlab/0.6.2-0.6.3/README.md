# Comparing `tmp/domainlab-0.6.2.tar.gz` & `tmp/domainlab-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domainlab-0.6.2.tar", max compression
+gzip compressed data, was "domainlab-0.6.3.tar", max compression
```

## Comparing `domainlab-0.6.2.tar` & `domainlab-0.6.3.tar`

### file list

```diff
@@ -1,421 +1,421 @@
--rw-r--r--   0        0        0     1067 2023-10-11 14:43:45.236020 domainlab-0.6.2/LICENSE
--rw-r--r--   0        0        0     7436 2024-03-28 15:12:23.813173 domainlab-0.6.2/README.md
--rw-r--r--   0        0        0       27 2023-10-11 14:43:45.264020 domainlab-0.6.2/domainlab/.gitignore
--rw-r--r--   0        0        0      178 2023-10-11 14:43:45.264020 domainlab-0.6.2/domainlab/.pylintrc
--rw-r--r--   0        0        0      751 2024-01-29 15:48:58.236016 domainlab-0.6.2/domainlab/__init__.py
--rw-r--r--   0        0        0        0 2023-10-11 14:43:45.264020 domainlab-0.6.2/domainlab/algos/__init__.py
--rw-r--r--   0        0        0     1747 2024-01-29 15:48:58.236016 domainlab-0.6.2/domainlab/algos/a_algo_builder.py
--rw-r--r--   0        0        0      950 2024-01-29 15:48:58.236016 domainlab-0.6.2/domainlab/algos/builder_api_model.py
--rw-r--r--   0        0        0     5389 2024-01-29 15:48:58.236016 domainlab-0.6.2/domainlab/algos/builder_custom.py
--rw-r--r--   0        0        0     3379 2024-01-29 15:48:58.236016 domainlab-0.6.2/domainlab/algos/builder_dann.py
--rw-r--r--   0        0        0     2286 2024-03-28 15:12:20.465049 domainlab-0.6.2/domainlab/algos/builder_diva.py
--rw-r--r--   0        0        0     1774 2024-01-29 15:48:58.236016 domainlab-0.6.2/domainlab/algos/builder_erm.py
--rw-r--r--   0        0        0     1973 2024-01-29 15:48:58.236016 domainlab-0.6.2/domainlab/algos/builder_hduva.py
--rw-r--r--   0        0        0     3010 2024-03-28 15:12:20.465049 domainlab-0.6.2/domainlab/algos/builder_jigen1.py
--rw-r--r--   0        0        0        0 2023-10-11 14:43:45.264020 domainlab-0.6.2/domainlab/algos/msels/__init__.py
--rw-r--r--   0        0        0     2976 2024-03-28 15:12:23.813173 domainlab-0.6.2/domainlab/algos/msels/a_model_sel.py
--rw-r--r--   0        0        0     2056 2024-03-28 15:12:23.813173 domainlab-0.6.2/domainlab/algos/msels/c_msel_oracle.py
--rw-r--r--   0        0        0     1513 2024-03-28 15:12:23.813173 domainlab-0.6.2/domainlab/algos/msels/c_msel_tr_loss.py
--rw-r--r--   0        0        0     2559 2024-03-28 15:12:23.813173 domainlab-0.6.2/domainlab/algos/msels/c_msel_val.py
--rw-r--r--   0        0        0        0 2023-10-11 14:43:45.264020 domainlab-0.6.2/domainlab/algos/observers/__init__.py
--rw-r--r--   0        0        0     1551 2024-01-29 15:48:58.236016 domainlab-0.6.2/domainlab/algos/observers/a_observer.py
--rw-r--r--   0        0        0     6100 2024-03-28 15:12:23.813173 domainlab-0.6.2/domainlab/algos/observers/b_obvisitor.py
--rw-r--r--   0        0        0      682 2024-03-28 15:12:20.469049 domainlab-0.6.2/domainlab/algos/observers/c_obvisitor_cleanup.py
--rw-r--r--   0        0        0     1593 2024-01-29 15:48:58.236016 domainlab-0.6.2/domainlab/algos/observers/c_obvisitor_gen.py
--rw-r--r--   0        0        0        0 2023-10-11 14:43:45.268020 domainlab-0.6.2/domainlab/algos/trainers/__init__.py
--rw-r--r--   0        0        0     7387 2024-03-28 15:12:23.813173 domainlab-0.6.2/domainlab/algos/trainers/a_trainer.py
--rw-r--r--   0        0        0      842 2024-01-29 15:48:58.236016 domainlab-0.6.2/domainlab/algos/trainers/args_dial.py
--rw-r--r--   0        0        0        0 2024-01-29 15:48:58.236016 domainlab-0.6.2/domainlab/algos/trainers/compos/__init__.py
--rw-r--r--   0        0        0      613 2024-01-29 15:48:58.236016 domainlab-0.6.2/domainlab/algos/trainers/compos/matchdg_args.py
--rw-r--r--   0        0        0    18836 2024-03-28 15:12:20.469049 domainlab-0.6.2/domainlab/algos/trainers/compos/matchdg_match.py
--rw-r--r--   0        0        0     5095 2024-01-29 15:48:58.236016 domainlab-0.6.2/domainlab/algos/trainers/compos/matchdg_utils.py
--rw-r--r--   0        0        0     1971 2024-01-29 15:48:58.236016 domainlab-0.6.2/domainlab/algos/trainers/hyper_scheduler.py
--rw-r--r--   0        0        0     3556 2024-03-28 15:12:20.469049 domainlab-0.6.2/domainlab/algos/trainers/train_basic.py
--rw-r--r--   0        0        0     2094 2024-03-28 15:12:20.469049 domainlab-0.6.2/domainlab/algos/trainers/train_dial.py
--rw-r--r--   0        0        0     7802 2024-03-28 15:12:23.813173 domainlab-0.6.2/domainlab/algos/trainers/train_fishr.py
--rw-r--r--   0        0        0     2421 2024-01-29 15:48:58.236016 domainlab-0.6.2/domainlab/algos/trainers/train_hyper_scheduler.py
--rw-r--r--   0        0        0    15390 2024-03-28 15:12:20.469049 domainlab-0.6.2/domainlab/algos/trainers/train_matchdg.py
--rw-r--r--   0        0        0     4355 2024-01-29 15:48:58.236016 domainlab-0.6.2/domainlab/algos/trainers/train_mldg.py
--rw-r--r--   0        0        0     2316 2024-03-28 15:12:23.813173 domainlab-0.6.2/domainlab/algos/trainers/zoo_trainer.py
--rw-r--r--   0        0        0      317 2024-01-29 15:48:58.236016 domainlab-0.6.2/domainlab/algos/utils.py
--rw-r--r--   0        0        0     1975 2024-03-28 15:12:20.469049 domainlab-0.6.2/domainlab/algos/zoo_algos.py
--rw-r--r--   0        0        0    11134 2024-03-28 15:12:23.813173 domainlab-0.6.2/domainlab/arg_parser.py
--rw-r--r--   0        0        0      813 2024-01-29 15:48:58.236016 domainlab-0.6.2/domainlab/cli.py
--rw-r--r--   0        0        0        0 2023-10-11 14:43:45.268020 domainlab-0.6.2/domainlab/compos/__init__.py
--rw-r--r--   0        0        0     1524 2024-01-29 15:48:58.236016 domainlab-0.6.2/domainlab/compos/a_nn_builder.py
--rw-r--r--   0        0        0     1517 2024-01-29 15:48:58.236016 domainlab-0.6.2/domainlab/compos/builder_nn_alex.py
--rw-r--r--   0        0        0     1496 2024-01-29 15:48:58.236016 domainlab-0.6.2/domainlab/compos/builder_nn_conv_bn_relu_2.py
--rw-r--r--   0        0        0     1461 2024-01-29 15:48:58.236016 domainlab-0.6.2/domainlab/compos/builder_nn_external_from_file.py
--rw-r--r--   0        0        0        0 2023-10-11 14:43:45.268020 domainlab-0.6.2/domainlab/compos/nn_zoo/__init__.py
--rw-r--r--   0        0        0      854 2024-01-29 15:48:58.236016 domainlab-0.6.2/domainlab/compos/nn_zoo/net_adversarial.py
--rw-r--r--   0        0        0      740 2024-01-29 15:48:58.236016 domainlab-0.6.2/domainlab/compos/nn_zoo/net_classif.py
--rw-r--r--   0        0        0     2851 2024-01-29 15:48:58.236016 domainlab-0.6.2/domainlab/compos/nn_zoo/net_conv_conv_bn_pool_2.py
--rw-r--r--   0        0        0     2173 2024-01-29 15:48:58.236016 domainlab-0.6.2/domainlab/compos/nn_zoo/net_gated.py
--rw-r--r--   0        0        0     1077 2024-01-29 15:48:58.236016 domainlab-0.6.2/domainlab/compos/nn_zoo/nn.py
--rw-r--r--   0        0        0     2876 2024-01-29 15:48:58.236016 domainlab-0.6.2/domainlab/compos/nn_zoo/nn_alex.py
--rw-r--r--   0        0        0      860 2024-01-29 15:48:58.236016 domainlab-0.6.2/domainlab/compos/nn_zoo/nn_torchvision.py
--rw-r--r--   0        0        0        0 2023-10-11 14:43:45.268020 domainlab-0.6.2/domainlab/compos/pcr/__init__.py
--rw-r--r--   0        0        0     4858 2024-01-29 15:48:58.236016 domainlab-0.6.2/domainlab/compos/pcr/p_chain_handler.py
--rw-r--r--   0        0        0     1096 2024-01-29 15:48:58.236016 domainlab-0.6.2/domainlab/compos/pcr/request.py
--rw-r--r--   0        0        0      617 2023-10-11 14:43:45.268020 domainlab-0.6.2/domainlab/compos/utils_conv_get_flat_dim.py
--rw-r--r--   0        0        0        0 2023-10-11 14:43:45.268020 domainlab-0.6.2/domainlab/compos/vae/__init__.py
--rw-r--r--   0        0        0      799 2023-10-11 14:43:45.268020 domainlab-0.6.2/domainlab/compos/vae/a_model_builder.py
--rw-r--r--   0        0        0     1327 2024-01-29 15:48:58.236016 domainlab-0.6.2/domainlab/compos/vae/a_vae_builder.py
--rw-r--r--   0        0        0     1854 2024-01-29 15:48:58.240016 domainlab-0.6.2/domainlab/compos/vae/c_vae_adaptor_model_recon.py
--rw-r--r--   0        0        0     1347 2024-01-29 15:48:58.240016 domainlab-0.6.2/domainlab/compos/vae/c_vae_builder_classif.py
--rw-r--r--   0        0        0     3663 2024-01-29 15:48:58.240016 domainlab-0.6.2/domainlab/compos/vae/c_vae_recon.py
--rw-r--r--   0        0        0        0 2023-10-11 14:43:45.268020 domainlab-0.6.2/domainlab/compos/vae/compos/__init__.py
--rw-r--r--   0        0        0     2256 2024-01-29 15:48:58.240016 domainlab-0.6.2/domainlab/compos/vae/compos/decoder_concat_vec_reshape_conv.py
--rw-r--r--   0        0        0     2241 2024-01-29 15:48:58.240016 domainlab-0.6.2/domainlab/compos/vae/compos/decoder_concat_vec_reshape_conv_gated_conv.py
--rw-r--r--   0        0        0     1493 2024-01-29 15:48:58.240016 domainlab-0.6.2/domainlab/compos/vae/compos/decoder_cond_prior.py
--rw-r--r--   0        0        0     1604 2024-01-29 15:48:58.240016 domainlab-0.6.2/domainlab/compos/vae/compos/decoder_losses.py
--rw-r--r--   0        0        0     3027 2024-01-29 15:48:58.240016 domainlab-0.6.2/domainlab/compos/vae/compos/encoder.py
--rw-r--r--   0        0        0      771 2024-01-29 15:48:58.240016 domainlab-0.6.2/domainlab/compos/vae/compos/encoder_dirichlet.py
--rw-r--r--   0        0        0     1667 2024-01-29 15:48:58.240016 domainlab-0.6.2/domainlab/compos/vae/compos/encoder_domain_topic.py
--rw-r--r--   0        0        0     1557 2024-01-29 15:48:58.240016 domainlab-0.6.2/domainlab/compos/vae/compos/encoder_domain_topic_img2topic.py
--rw-r--r--   0        0        0     1732 2024-01-29 15:48:58.240016 domainlab-0.6.2/domainlab/compos/vae/compos/encoder_domain_topic_img_topic2zd.py
--rw-r--r--   0        0        0     5256 2024-01-29 15:48:58.240016 domainlab-0.6.2/domainlab/compos/vae/compos/encoder_xyd_parallel.py
--rw-r--r--   0        0        0     2813 2024-01-29 15:48:58.240016 domainlab-0.6.2/domainlab/compos/vae/compos/encoder_xydt_elevator.py
--rw-r--r--   0        0        0     1884 2024-01-29 15:48:58.240016 domainlab-0.6.2/domainlab/compos/vae/compos/encoder_zy.py
--rw-r--r--   0        0        0     1274 2024-01-29 15:48:58.240016 domainlab-0.6.2/domainlab/compos/vae/utils_request_chain_builder.py
--rw-r--r--   0        0        0     3817 2024-01-29 15:48:58.240016 domainlab-0.6.2/domainlab/compos/vae/zoo_vae_builders_classif.py
--rw-r--r--   0        0        0     1383 2024-01-29 15:48:58.240016 domainlab-0.6.2/domainlab/compos/vae/zoo_vae_builders_classif_topic.py
--rw-r--r--   0        0        0     1561 2024-01-29 15:48:58.240016 domainlab-0.6.2/domainlab/compos/zoo_nn.py
--rw-r--r--   0        0        0        0 2023-10-11 14:43:45.268020 domainlab-0.6.2/domainlab/dsets/__init__.py
--rw-r--r--   0        0        0     6071 2024-01-29 15:48:58.240016 domainlab-0.6.2/domainlab/dsets/a_dset_mnist_color_rgb_solo.py
--rw-r--r--   0        0        0     1350 2024-01-29 15:48:58.240016 domainlab-0.6.2/domainlab/dsets/dset_img_path_list.py
--rw-r--r--   0        0        0      845 2024-01-29 15:48:58.240016 domainlab-0.6.2/domainlab/dsets/dset_mnist_color_solo_default.py
--rw-r--r--   0        0        0     1455 2024-01-29 15:48:58.240016 domainlab-0.6.2/domainlab/dsets/dset_poly_domains_mnist_color_default.py
--rw-r--r--   0        0        0     6082 2024-01-29 15:48:58.240016 domainlab-0.6.2/domainlab/dsets/dset_subfolder.py
--rw-r--r--   0        0        0      226 2024-01-29 15:48:58.240016 domainlab-0.6.2/domainlab/dsets/utils_color_palette.py
--rw-r--r--   0        0        0     2377 2024-01-29 15:48:58.240016 domainlab-0.6.2/domainlab/dsets/utils_data.py
--rw-r--r--   0        0        0     7195 2024-01-29 15:48:58.240016 domainlab-0.6.2/domainlab/dsets/utils_wrapdset_patches.py
--rw-r--r--   0        0        0        0 2024-01-29 15:48:58.240016 domainlab-0.6.2/domainlab/exp/__init__.py
--rw-r--r--   0        0        0      750 2024-01-29 15:48:58.240016 domainlab-0.6.2/domainlab/exp/exp_cuda_seed.py
--rwxr-xr-x   0        0        0     4731 2024-03-28 15:12:23.813173 domainlab-0.6.2/domainlab/exp/exp_main.py
--rw-r--r--   0        0        0    10609 2024-03-28 15:12:23.813173 domainlab-0.6.2/domainlab/exp/exp_utils.py
--rw-r--r--   0        0        0        0 2023-10-11 14:43:45.268020 domainlab-0.6.2/domainlab/exp_protocol/__init__.py
--rw-r--r--   0        0        0     1753 2024-01-29 15:48:58.240016 domainlab-0.6.2/domainlab/exp_protocol/aggregate_results.py
--rw-r--r--   0        0        0     7481 2024-03-28 15:12:23.813173 domainlab-0.6.2/domainlab/exp_protocol/benchmark.smk
--rw-r--r--   0        0        0     6831 2024-03-28 15:12:20.469049 domainlab-0.6.2/domainlab/exp_protocol/run_experiment.py
--rw-r--r--   0        0        0     1236 2024-01-29 15:48:58.240016 domainlab-0.6.2/domainlab/mk_exp.py
--rw-r--r--   0        0        0        0 2023-10-11 14:43:45.268020 domainlab-0.6.2/domainlab/models/__init__.py
--rw-r--r--   0        0        0     6054 2024-03-28 15:12:20.469049 domainlab-0.6.2/domainlab/models/a_model.py
--rw-r--r--   0        0        0     8917 2024-03-28 15:12:23.813173 domainlab-0.6.2/domainlab/models/a_model_classif.py
--rw-r--r--   0        0        0      853 2024-01-29 15:48:58.240016 domainlab-0.6.2/domainlab/models/args_jigen.py
--rw-r--r--   0        0        0     2063 2024-01-29 15:48:58.240016 domainlab-0.6.2/domainlab/models/args_vae.py
--rw-r--r--   0        0        0     1370 2024-01-29 15:48:58.240016 domainlab-0.6.2/domainlab/models/interface_vae_xyd.py
--rw-r--r--   0        0        0      452 2024-01-29 15:48:58.240016 domainlab-0.6.2/domainlab/models/model_custom.py
--rw-r--r--   0        0        0     3785 2024-03-28 15:12:20.469049 domainlab-0.6.2/domainlab/models/model_dann.py
--rw-r--r--   0        0        0     5905 2024-03-28 15:12:20.469049 domainlab-0.6.2/domainlab/models/model_diva.py
--rw-r--r--   0        0        0     1719 2024-03-28 15:12:23.813173 domainlab-0.6.2/domainlab/models/model_erm.py
--rw-r--r--   0        0        0     8327 2024-03-28 15:12:20.469049 domainlab-0.6.2/domainlab/models/model_hduva.py
--rw-r--r--   0        0        0     4888 2024-03-28 15:12:20.469049 domainlab-0.6.2/domainlab/models/model_jigen.py
--rw-r--r--   0        0        0     1364 2024-01-29 15:48:58.240016 domainlab-0.6.2/domainlab/models/model_vae_xyd_classif.py
--rw-r--r--   0        0        0      105 2024-01-29 15:48:58.240016 domainlab-0.6.2/domainlab/tasks/__init__.py
--rw-r--r--   0        0        0     5826 2024-03-28 15:12:23.813173 domainlab-0.6.2/domainlab/tasks/a_task.py
--rw-r--r--   0        0        0     2128 2024-01-29 15:48:58.240016 domainlab-0.6.2/domainlab/tasks/a_task_classif.py
--rw-r--r--   0        0        0     3294 2024-03-28 15:12:23.813173 domainlab-0.6.2/domainlab/tasks/b_task.py
--rw-r--r--   0        0        0     1514 2024-01-29 15:48:58.240016 domainlab-0.6.2/domainlab/tasks/b_task_classif.py
--rw-r--r--   0        0        0     2099 2024-01-29 15:48:58.240016 domainlab-0.6.2/domainlab/tasks/task_dset.py
--rw-r--r--   0        0        0     3931 2024-01-29 15:48:58.240016 domainlab-0.6.2/domainlab/tasks/task_folder.py
--rw-r--r--   0        0        0     2540 2024-01-29 15:48:58.240016 domainlab-0.6.2/domainlab/tasks/task_folder_mk.py
--rw-r--r--   0        0        0     1993 2024-01-29 15:48:58.240016 domainlab-0.6.2/domainlab/tasks/task_mini_vlcs.py
--rw-r--r--   0        0        0     2357 2024-01-29 15:48:58.240016 domainlab-0.6.2/domainlab/tasks/task_mnist_color.py
--rw-r--r--   0        0        0     4851 2024-01-29 15:48:58.244016 domainlab-0.6.2/domainlab/tasks/task_pathlist.py
--rw-r--r--   0        0        0      897 2023-10-11 14:43:45.272020 domainlab-0.6.2/domainlab/tasks/task_utils.py
--rw-r--r--   0        0        0     8747 2024-01-29 15:48:58.244016 domainlab-0.6.2/domainlab/tasks/utils_task.py
--rw-r--r--   0        0        0     1954 2024-01-29 15:48:58.244016 domainlab-0.6.2/domainlab/tasks/utils_task_dset.py
--rw-r--r--   0        0        0     1791 2024-01-29 15:48:58.244016 domainlab-0.6.2/domainlab/tasks/zoo_tasks.py
--rw-r--r--   0        0        0        0 2023-10-11 14:43:45.272020 domainlab-0.6.2/domainlab/utils/__init__.py
--rw-r--r--   0        0        0     4722 2024-01-29 15:48:58.244016 domainlab-0.6.2/domainlab/utils/flows_gen_img_model.py
--rw-r--r--   0        0        0    23007 2024-03-28 15:12:23.813173 domainlab-0.6.2/domainlab/utils/generate_benchmark_plots.py
--rw-r--r--   0        0        0     1378 2024-01-29 15:48:58.244016 domainlab-0.6.2/domainlab/utils/get_git_tag.py
--rw-r--r--   0        0        0    17718 2024-01-29 15:48:58.244016 domainlab-0.6.2/domainlab/utils/hyperparameter_gridsearch.py
--rw-r--r--   0        0        0    17564 2024-01-29 15:48:58.244016 domainlab-0.6.2/domainlab/utils/hyperparameter_sampling.py
--rw-r--r--   0        0        0     1415 2024-01-29 15:48:58.244016 domainlab-0.6.2/domainlab/utils/logger.py
--rw-r--r--   0        0        0      802 2024-01-29 15:48:58.244016 domainlab-0.6.2/domainlab/utils/override_interface.py
--rw-r--r--   0        0        0     2216 2024-01-29 15:48:58.244016 domainlab-0.6.2/domainlab/utils/perf.py
--rw-r--r--   0        0        0     3783 2024-01-29 15:48:58.244016 domainlab-0.6.2/domainlab/utils/perf_metrics.py
--rw-r--r--   0        0        0     3371 2024-01-29 15:48:58.244016 domainlab-0.6.2/domainlab/utils/sanity_check.py
--rw-r--r--   0        0        0      915 2024-01-29 15:48:58.244016 domainlab-0.6.2/domainlab/utils/test_img.py
--rw-r--r--   0        0        0      336 2023-10-11 14:43:45.272020 domainlab-0.6.2/domainlab/utils/u_import.py
--rw-r--r--   0        0        0     2023 2024-01-29 15:48:58.244016 domainlab-0.6.2/domainlab/utils/u_import_net_module.py
--rw-r--r--   0        0        0      884 2024-01-29 15:48:58.244016 domainlab-0.6.2/domainlab/utils/utils_class.py
--rw-r--r--   0        0        0     1317 2024-01-29 15:48:58.244016 domainlab-0.6.2/domainlab/utils/utils_classif.py
--rw-r--r--   0        0        0      544 2024-01-29 15:48:58.244016 domainlab-0.6.2/domainlab/utils/utils_cuda.py
--rw-r--r--   0        0        0     1185 2024-01-29 15:48:58.244016 domainlab-0.6.2/domainlab/utils/utils_img_sav.py
--rw-r--r--   0        0        0       12 2024-01-29 15:48:58.244016 domainlab-0.6.2/domainlab/zdata/mixed_codec/caltech/auto/text.txt
--rw-r--r--   0        0        0     8579 2024-01-29 15:48:58.244016 domainlab-0.6.2/domainlab/zdata/mixed_codec/caltech/auto/train_imgs_150.jpg
--rw-r--r--   0        0        0     8521 2024-01-29 15:48:58.244016 domainlab-0.6.2/domainlab/zdata/mixed_codec/caltech/auto/train_imgs_151.jpg
--rw-r--r--   0        0        0    62574 2024-01-29 15:48:58.244016 domainlab-0.6.2/domainlab/zdata/mixed_codec/caltech/auto/train_imgs_152.png
--rw-r--r--   0        0        0     6984 2024-01-29 15:48:58.244016 domainlab-0.6.2/domainlab/zdata/mixed_codec/caltech/vogel/train_imgs_1.jpg
--rw-r--r--   0        0        0    10707 2024-01-29 15:48:58.244016 domainlab-0.6.2/domainlab/zdata/mixed_codec/caltech/vogel/train_imgs_2.jpg
--rw-r--r--   0        0        0    48698 2024-01-29 15:48:58.244016 domainlab-0.6.2/domainlab/zdata/mixed_codec/caltech/vogel/train_imgs_3.png
--rw-r--r--   0        0        0    10543 2024-01-29 15:48:58.244016 domainlab-0.6.2/domainlab/zdata/mixed_codec/sun/sofa/train_imgs_609.jpg
--rw-r--r--   0        0        0    12217 2024-01-29 15:48:58.244016 domainlab-0.6.2/domainlab/zdata/mixed_codec/sun/sofa/train_imgs_612.jpg
--rw-r--r--   0        0        0    10395 2024-01-29 15:48:58.248016 domainlab-0.6.2/domainlab/zdata/mixed_codec/sun/vehicle/train_imgs_17.jpg
--rw-r--r--   0        0        0     4734 2024-01-29 15:48:58.248016 domainlab-0.6.2/domainlab/zdata/mixed_codec/sun/vehicle/train_imgs_19.jpg
--rw-r--r--   0        0        0    10736 2024-01-29 15:48:58.248016 domainlab-0.6.2/domainlab/zdata/pacs_mini_10/art_painting/dog/pic_195.jpg
--rw-r--r--   0        0        0    35963 2024-01-29 15:48:58.248016 domainlab-0.6.2/domainlab/zdata/pacs_mini_10/art_painting/dog/pic_304.jpg
--rw-r--r--   0        0        0    39114 2024-01-29 15:48:58.248016 domainlab-0.6.2/domainlab/zdata/pacs_mini_10/art_painting/elephant/pic_026.jpg
--rw-r--r--   0        0        0    16324 2024-01-29 15:48:58.248016 domainlab-0.6.2/domainlab/zdata/pacs_mini_10/art_painting/giraffe/pic_243.jpg
--rw-r--r--   0        0        0    27254 2024-01-29 15:48:58.248016 domainlab-0.6.2/domainlab/zdata/pacs_mini_10/art_painting/guitar/pic_020.jpg
--rw-r--r--   0        0        0    37953 2024-01-29 15:48:58.248016 domainlab-0.6.2/domainlab/zdata/pacs_mini_10/art_painting/guitar/pic_182.jpg
--rw-r--r--   0        0        0    21398 2024-01-29 15:48:58.248016 domainlab-0.6.2/domainlab/zdata/pacs_mini_10/art_painting/horse/pic_142.jpg
--rw-r--r--   0        0        0    27377 2024-01-29 15:48:58.248016 domainlab-0.6.2/domainlab/zdata/pacs_mini_10/art_painting/person/pic_165.jpg
--rw-r--r--   0        0        0    18550 2024-01-29 15:48:58.248016 domainlab-0.6.2/domainlab/zdata/pacs_mini_10/art_painting/person/pic_199.jpg
--rw-r--r--   0        0        0    21402 2024-01-29 15:48:58.248016 domainlab-0.6.2/domainlab/zdata/pacs_mini_10/art_painting/person/pic_497.jpg
--rw-r--r--   0        0        0    20448 2024-01-29 15:48:58.248016 domainlab-0.6.2/domainlab/zdata/pacs_mini_10/cartoon/dog/pic_112.jpg
--rw-r--r--   0        0        0    26362 2024-01-29 15:48:58.248016 domainlab-0.6.2/domainlab/zdata/pacs_mini_10/cartoon/dog/pic_137.jpg
--rw-r--r--   0        0        0    20540 2024-01-29 15:48:58.248016 domainlab-0.6.2/domainlab/zdata/pacs_mini_10/cartoon/dog/pic_219.jpg
--rw-r--r--   0        0        0    18461 2024-01-29 15:48:58.248016 domainlab-0.6.2/domainlab/zdata/pacs_mini_10/cartoon/elephant/pic_332.jpg
--rw-r--r--   0        0        0    33171 2024-01-29 15:48:58.248016 domainlab-0.6.2/domainlab/zdata/pacs_mini_10/cartoon/giraffe/pic_377.jpg
--rw-r--r--   0        0        0    20113 2024-01-29 15:48:58.248016 domainlab-0.6.2/domainlab/zdata/pacs_mini_10/cartoon/giraffe/pic_382.jpg
--rw-r--r--   0        0        0    22002 2024-01-29 15:48:58.248016 domainlab-0.6.2/domainlab/zdata/pacs_mini_10/cartoon/horse/pic_064.jpg
--rw-r--r--   0        0        0    12438 2024-01-29 15:48:58.248016 domainlab-0.6.2/domainlab/zdata/pacs_mini_10/cartoon/house/pic_040.jpg
--rw-r--r--   0        0        0    21770 2024-01-29 15:48:58.248016 domainlab-0.6.2/domainlab/zdata/pacs_mini_10/cartoon/person/pic_111.jpg
--rw-r--r--   0        0        0    18691 2024-01-29 15:48:58.248016 domainlab-0.6.2/domainlab/zdata/pacs_mini_10/cartoon/person/pic_180.jpg
--rw-r--r--   0        0        0      498 2024-01-29 15:48:58.248016 domainlab-0.6.2/domainlab/zdata/pacs_mini_10/main.sh
--rw-r--r--   0        0        0    23240 2024-01-29 15:48:58.252016 domainlab-0.6.2/domainlab/zdata/pacs_mini_10/photo/dog/n02103406_1011.jpg
--rw-r--r--   0        0        0    23174 2024-01-29 15:48:58.252016 domainlab-0.6.2/domainlab/zdata/pacs_mini_10/photo/elephant/n02503517_6232.jpg
--rw-r--r--   0        0        0    11646 2024-01-29 15:48:58.252016 domainlab-0.6.2/domainlab/zdata/pacs_mini_10/photo/guitar/n02676566_7830.jpg
--rw-r--r--   0        0        0    21822 2024-01-29 15:48:58.252016 domainlab-0.6.2/domainlab/zdata/pacs_mini_10/photo/horse/105_0223.jpg
--rw-r--r--   0        0        0    25832 2024-01-29 15:48:58.252016 domainlab-0.6.2/domainlab/zdata/pacs_mini_10/photo/house/pic_046.jpg
--rw-r--r--   0        0        0    23408 2024-01-29 15:48:58.252016 domainlab-0.6.2/domainlab/zdata/pacs_mini_10/photo/house/pic_110.jpg
--rw-r--r--   0        0        0    27674 2024-01-29 15:48:58.252016 domainlab-0.6.2/domainlab/zdata/pacs_mini_10/photo/house/pic_146.jpg
--rw-r--r--   0        0        0    27298 2024-01-29 15:48:58.252016 domainlab-0.6.2/domainlab/zdata/pacs_mini_10/photo/house/pic_218.jpg
--rw-r--r--   0        0        0    23829 2024-01-29 15:48:58.252016 domainlab-0.6.2/domainlab/zdata/pacs_mini_10/photo/person/253_0221.jpg
--rw-r--r--   0        0        0    17983 2024-01-29 15:48:58.252016 domainlab-0.6.2/domainlab/zdata/pacs_mini_10/photo/person/253_0297.jpg
--rw-r--r--   0        0        0      544 2024-01-29 15:48:58.252016 domainlab-0.6.2/domainlab/zdata/pacs_mini_10/run_with_bash_copy_files_according2txt.sh
--rw-r--r--   0        0        0     8767 2024-01-29 15:48:58.252016 domainlab-0.6.2/domainlab/zdata/pacs_mini_10/sketch/dog/5302.png
--rw-r--r--   0        0        0     8032 2024-01-29 15:48:58.252016 domainlab-0.6.2/domainlab/zdata/pacs_mini_10/sketch/dog/5317.png
--rw-r--r--   0        0        0    13745 2024-01-29 15:48:58.252016 domainlab-0.6.2/domainlab/zdata/pacs_mini_10/sketch/dog/n02103406_3255-6.png
--rw-r--r--   0        0        0     6480 2024-01-29 15:48:58.252016 domainlab-0.6.2/domainlab/zdata/pacs_mini_10/sketch/elephant/5981.png
--rw-r--r--   0        0        0    13120 2024-01-29 15:48:58.252016 domainlab-0.6.2/domainlab/zdata/pacs_mini_10/sketch/elephant/n02503517_12688-4.png
--rw-r--r--   0        0        0    13602 2024-01-29 15:48:58.252016 domainlab-0.6.2/domainlab/zdata/pacs_mini_10/sketch/giraffe/n02439033_13384-2.png
--rw-r--r--   0        0        0    12858 2024-01-29 15:48:58.252016 domainlab-0.6.2/domainlab/zdata/pacs_mini_10/sketch/guitar/n02676566_8618-2.png
--rw-r--r--   0        0        0     8300 2024-01-29 15:48:58.252016 domainlab-0.6.2/domainlab/zdata/pacs_mini_10/sketch/guitar/n03467517_6423-3.png
--rw-r--r--   0        0        0    16388 2024-01-29 15:48:58.252016 domainlab-0.6.2/domainlab/zdata/pacs_mini_10/sketch/horse/n02374451_779-1.png
--rw-r--r--   0        0        0     8519 2024-01-29 15:48:58.252016 domainlab-0.6.2/domainlab/zdata/pacs_mini_10/sketch/house/8873.png
--rw-r--r--   0        0        0      336 2024-01-29 15:48:58.252016 domainlab-0.6.2/domainlab/zdata/pacs_split/art_painting_10.txt
--rw-r--r--   0        0        0     3335 2024-01-29 15:48:58.252016 domainlab-0.6.2/domainlab/zdata/pacs_split/art_painting_100.txt
--rw-r--r--   0        0        0     6988 2024-01-29 15:48:58.252016 domainlab-0.6.2/domainlab/zdata/pacs_split/art_painting_crossval_kfold.txt
--rw-r--r--   0        0        0    68794 2024-01-29 15:48:58.252016 domainlab-0.6.2/domainlab/zdata/pacs_split/art_painting_test_kfold.txt
--rw-r--r--   0        0        0    61806 2024-01-29 15:48:58.252016 domainlab-0.6.2/domainlab/zdata/pacs_split/art_painting_train_kfold.txt
--rw-r--r--   0        0        0      283 2024-01-29 15:48:58.252016 domainlab-0.6.2/domainlab/zdata/pacs_split/cartoon_10.txt
--rw-r--r--   0        0        0     2882 2024-01-29 15:48:58.252016 domainlab-0.6.2/domainlab/zdata/pacs_split/cartoon_100.txt
--rw-r--r--   0        0        0     6821 2024-01-29 15:48:58.252016 domainlab-0.6.2/domainlab/zdata/pacs_split/cartoon_crossval_kfold.txt
--rw-r--r--   0        0        0    67457 2024-01-29 15:48:58.252016 domainlab-0.6.2/domainlab/zdata/pacs_split/cartoon_test_kfold.txt
--rw-r--r--   0        0        0    60636 2024-01-29 15:48:58.252016 domainlab-0.6.2/domainlab/zdata/pacs_split/cartoon_train_kfold.txt
--rw-r--r--   0        0        0      288 2024-01-29 15:48:58.252016 domainlab-0.6.2/domainlab/zdata/pacs_split/photo_10.txt
--rw-r--r--   0        0        0     2940 2024-01-29 15:48:58.252016 domainlab-0.6.2/domainlab/zdata/pacs_split/photo_100.txt
--rw-r--r--   0        0        0     4714 2024-01-29 15:48:58.252016 domainlab-0.6.2/domainlab/zdata/pacs_split/photo_crossval_kfold.txt
--rw-r--r--   0        0        0    48735 2024-01-29 15:48:58.252016 domainlab-0.6.2/domainlab/zdata/pacs_split/photo_test_kfold.txt
--rw-r--r--   0        0        0    44021 2024-01-29 15:48:58.252016 domainlab-0.6.2/domainlab/zdata/pacs_split/photo_train_kfold.txt
--rw-r--r--   0        0        0      527 2024-01-29 15:48:58.252016 domainlab-0.6.2/domainlab/zdata/pacs_split/readme.txt
--rw-r--r--   0        0        0      317 2024-01-29 15:48:58.252016 domainlab-0.6.2/domainlab/zdata/pacs_split/sketch_10.txt
--rw-r--r--   0        0        0     3549 2024-01-29 15:48:58.252016 domainlab-0.6.2/domainlab/zdata/pacs_split/sketch_100.txt
--rw-r--r--   0        0        0    13338 2024-01-29 15:48:58.252016 domainlab-0.6.2/domainlab/zdata/pacs_split/sketch_crossval_kfold.txt
--rw-r--r--   0        0        0   137732 2024-01-29 15:48:58.256016 domainlab-0.6.2/domainlab/zdata/pacs_split/sketch_test_kfold.txt
--rw-r--r--   0        0        0   124394 2024-01-29 15:48:58.256016 domainlab-0.6.2/domainlab/zdata/pacs_split/sketch_train_kfold.txt
--rw-r--r--   0        0        0     7328 2024-01-29 15:48:58.256016 domainlab-0.6.2/domainlab/zdata/patches_permutation4jigsaw/permutations_100.npy
--rw-r--r--   0        0        0     2288 2024-01-29 15:48:58.256016 domainlab-0.6.2/domainlab/zdata/patches_permutation4jigsaw/permutations_30.npy
--rw-r--r--   0        0        0     2360 2024-01-29 15:48:58.256016 domainlab-0.6.2/domainlab/zdata/patches_permutation4jigsaw/permutations_31.npy
--rw-r--r--   0        0        0     1456 2024-01-29 15:48:58.256016 domainlab-0.6.2/domainlab/zdata/script/download_pacs.py
--rw-r--r--   0        0        0     8579 2024-01-29 15:48:58.256016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_150.jpg
--rw-r--r--   0        0        0     8521 2024-01-29 15:48:58.256016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_151.jpg
--rw-r--r--   0        0        0    10449 2024-01-29 15:48:58.256016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_152.jpg
--rw-r--r--   0        0        0     9205 2024-01-29 15:48:58.256016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_153.jpg
--rw-r--r--   0        0        0     7298 2024-01-29 15:48:58.256016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_154.jpg
--rw-r--r--   0        0        0     9788 2024-01-29 15:48:58.256016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_155.jpg
--rw-r--r--   0        0        0     9149 2024-01-29 15:48:58.256016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_156.jpg
--rw-r--r--   0        0        0     9900 2024-01-29 15:48:58.256016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_157.jpg
--rw-r--r--   0        0        0     8077 2024-01-29 15:48:58.256016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_158.jpg
--rw-r--r--   0        0        0     7873 2024-01-29 15:48:58.256016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_159.jpg
--rw-r--r--   0        0        0     7561 2024-01-29 15:48:58.256016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_160.jpg
--rw-r--r--   0        0        0     7589 2024-01-29 15:48:58.256016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_161.jpg
--rw-r--r--   0        0        0    10250 2024-01-29 15:48:58.256016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_162.jpg
--rw-r--r--   0        0        0     8990 2024-01-29 15:48:58.256016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_163.jpg
--rw-r--r--   0        0        0    11370 2024-01-29 15:48:58.256016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_164.jpg
--rw-r--r--   0        0        0     7264 2024-01-29 15:48:58.256016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_165.jpg
--rw-r--r--   0        0        0    10782 2024-01-29 15:48:58.256016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_166.jpg
--rw-r--r--   0        0        0     9162 2024-01-29 15:48:58.256016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_167.jpg
--rw-r--r--   0        0        0     6964 2024-01-29 15:48:58.256016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_168.jpg
--rw-r--r--   0        0        0     9243 2024-01-29 15:48:58.256016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_169.jpg
--rw-r--r--   0        0        0    20748 2024-01-29 15:48:58.256016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/hund/train_imgs_302.jpg
--rw-r--r--   0        0        0    13099 2024-01-29 15:48:58.256016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/hund/train_imgs_303.jpg
--rw-r--r--   0        0        0    12864 2024-01-29 15:48:58.256016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/hund/train_imgs_304.jpg
--rw-r--r--   0        0        0     9116 2024-01-29 15:48:58.256016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/hund/train_imgs_305.jpg
--rw-r--r--   0        0        0     5890 2024-01-29 15:48:58.256016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/hund/train_imgs_306.jpg
--rw-r--r--   0        0        0     7751 2024-01-29 15:48:58.256016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/hund/train_imgs_307.jpg
--rw-r--r--   0        0        0     9665 2024-01-29 15:48:58.256016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/hund/train_imgs_308.jpg
--rw-r--r--   0        0        0    11819 2024-01-29 15:48:58.256016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/hund/train_imgs_309.jpg
--rw-r--r--   0        0        0    10768 2024-01-29 15:48:58.256016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/hund/train_imgs_310.jpg
--rw-r--r--   0        0        0    16572 2024-01-29 15:48:58.256016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/hund/train_imgs_311.jpg
--rw-r--r--   0        0        0     8817 2024-01-29 15:48:58.256016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/hund/train_imgs_312.jpg
--rw-r--r--   0        0        0     9740 2024-01-29 15:48:58.256016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/mensch/train_imgs_344.jpg
--rw-r--r--   0        0        0    10158 2024-01-29 15:48:58.256016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/mensch/train_imgs_345.jpg
--rw-r--r--   0        0        0     9840 2024-01-29 15:48:58.256016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/mensch/train_imgs_346.jpg
--rw-r--r--   0        0        0    10481 2024-01-29 15:48:58.256016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/mensch/train_imgs_347.jpg
--rw-r--r--   0        0        0     8690 2024-01-29 15:48:58.256016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/mensch/train_imgs_348.jpg
--rw-r--r--   0        0        0    10165 2024-01-29 15:48:58.256016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/mensch/train_imgs_349.jpg
--rw-r--r--   0        0        0     9983 2024-01-29 15:48:58.256016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/mensch/train_imgs_350.jpg
--rw-r--r--   0        0        0    14865 2024-01-29 15:48:58.256016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/mensch/train_imgs_351.jpg
--rw-r--r--   0        0        0    12113 2024-01-29 15:48:58.256016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/mensch/train_imgs_352.jpg
--rw-r--r--   0        0        0     9920 2024-01-29 15:48:58.256016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/stuhl/train_imgs_227.jpg
--rw-r--r--   0        0        0    12394 2024-01-29 15:48:58.256016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/stuhl/train_imgs_228.jpg
--rw-r--r--   0        0        0     7599 2024-01-29 15:48:58.256016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/stuhl/train_imgs_229.jpg
--rw-r--r--   0        0        0    11468 2024-01-29 15:48:58.256016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/stuhl/train_imgs_230.jpg
--rw-r--r--   0        0        0     9058 2024-01-29 15:48:58.260016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/stuhl/train_imgs_231.jpg
--rw-r--r--   0        0        0     7892 2024-01-29 15:48:58.260016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/stuhl/train_imgs_232.jpg
--rw-r--r--   0        0        0     6984 2024-01-29 15:48:58.260016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/vogel/train_imgs_1.jpg
--rw-r--r--   0        0        0    10707 2024-01-29 15:48:58.260016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/vogel/train_imgs_2.jpg
--rw-r--r--   0        0        0     5810 2024-01-29 15:48:58.260016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/vogel/train_imgs_3.jpg
--rw-r--r--   0        0        0     6592 2024-01-29 15:48:58.260016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/vogel/train_imgs_4.jpg
--rw-r--r--   0        0        0     8453 2024-01-29 15:48:58.260016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/vogel/train_imgs_5.jpg
--rw-r--r--   0        0        0     6281 2024-01-29 15:48:58.260016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/vogel/train_imgs_6.jpg
--rw-r--r--   0        0        0     8756 2024-01-29 15:48:58.260016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/vogel/train_imgs_7.jpg
--rw-r--r--   0        0        0    16157 2024-01-29 15:48:58.260016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/vogel/train_imgs_8.jpg
--rw-r--r--   0        0        0     8404 2024-01-29 15:48:58.260016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/vogel/train_imgs_9.jpg
--rw-r--r--   0        0        0     3088 2024-01-29 15:48:58.260016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_1.jpg
--rw-r--r--   0        0        0    10181 2024-01-29 15:48:58.264016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_10.jpg
--rw-r--r--   0        0        0    11434 2024-01-29 15:48:58.264016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_11.jpg
--rw-r--r--   0        0        0    11728 2024-01-29 15:48:58.264016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_12.jpg
--rw-r--r--   0        0        0    11491 2024-01-29 15:48:58.264016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_13.jpg
--rw-r--r--   0        0        0     3988 2024-01-29 15:48:58.264016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_14.jpg
--rw-r--r--   0        0        0    13956 2024-01-29 15:48:58.264016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_15.jpg
--rw-r--r--   0        0        0    16745 2024-01-29 15:48:58.264016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_16.jpg
--rw-r--r--   0        0        0    14936 2024-01-29 15:48:58.264016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_17.jpg
--rw-r--r--   0        0        0    13577 2024-01-29 15:48:58.264016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_18.jpg
--rw-r--r--   0        0        0     9233 2024-01-29 15:48:58.264016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_19.jpg
--rw-r--r--   0        0        0     8456 2024-01-29 15:48:58.264016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_2.jpg
--rw-r--r--   0        0        0    13275 2024-01-29 15:48:58.264016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_20.jpg
--rw-r--r--   0        0        0    12724 2024-01-29 15:48:58.264016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_21.jpg
--rw-r--r--   0        0        0    10267 2024-01-29 15:48:58.264016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_22.jpg
--rw-r--r--   0        0        0     6757 2024-01-29 15:48:58.264016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_23.jpg
--rw-r--r--   0        0        0    10767 2024-01-29 15:48:58.264016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_24.jpg
--rw-r--r--   0        0        0     5647 2024-01-29 15:48:58.264016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_25.jpg
--rw-r--r--   0        0        0    11123 2024-01-29 15:48:58.264016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_26.jpg
--rw-r--r--   0        0        0    12004 2024-01-29 15:48:58.264016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_27.jpg
--rw-r--r--   0        0        0    11538 2024-01-29 15:48:58.264016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_28.jpg
--rw-r--r--   0        0        0     5494 2024-01-29 15:48:58.264016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_29.jpg
--rw-r--r--   0        0        0    13925 2024-01-29 15:48:58.264016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_3.jpg
--rw-r--r--   0        0        0    16120 2024-01-29 15:48:58.264016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_30.jpg
--rw-r--r--   0        0        0    11315 2024-01-29 15:48:58.264016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_31.jpg
--rw-r--r--   0        0        0     9502 2024-01-29 15:48:58.264016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_32.jpg
--rw-r--r--   0        0        0     5206 2024-01-29 15:48:58.264016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_33.jpg
--rw-r--r--   0        0        0    11163 2024-01-29 15:48:58.264016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_34.jpg
--rw-r--r--   0        0        0    13437 2024-01-29 15:48:58.264016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_35.jpg
--rw-r--r--   0        0        0    12934 2024-01-29 15:48:58.264016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_36.jpg
--rw-r--r--   0        0        0     8358 2024-01-29 15:48:58.264016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_37.jpg
--rw-r--r--   0        0        0    14004 2024-01-29 15:48:58.264016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_38.jpg
--rw-r--r--   0        0        0    17970 2024-01-29 15:48:58.264016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_39.jpg
--rw-r--r--   0        0        0    11457 2024-01-29 15:48:58.264016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_4.jpg
--rw-r--r--   0        0        0    17124 2024-01-29 15:48:58.264016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_40.jpg
--rw-r--r--   0        0        0     6786 2024-01-29 15:48:58.264016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_41.jpg
--rw-r--r--   0        0        0    14007 2024-01-29 15:48:58.264016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_42.jpg
--rw-r--r--   0        0        0     8201 2024-01-29 15:48:58.264016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_43.jpg
--rw-r--r--   0        0        0    12656 2024-01-29 15:48:58.264016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_44.jpg
--rw-r--r--   0        0        0     7061 2024-01-29 15:48:58.268016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_45.jpg
--rw-r--r--   0        0        0     9186 2024-01-29 15:48:58.268016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_46.jpg
--rw-r--r--   0        0        0    12622 2024-01-29 15:48:58.268016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_47.jpg
--rw-r--r--   0        0        0    10099 2024-01-29 15:48:58.268016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_48.jpg
--rw-r--r--   0        0        0     8449 2024-01-29 15:48:58.268016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_49.jpg
--rw-r--r--   0        0        0    13827 2024-01-29 15:48:58.268016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_5.jpg
--rw-r--r--   0        0        0     7836 2024-01-29 15:48:58.268016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_50.jpg
--rw-r--r--   0        0        0    13309 2024-01-29 15:48:58.268016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_6.jpg
--rw-r--r--   0        0        0     8804 2024-01-29 15:48:58.268016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_7.jpg
--rw-r--r--   0        0        0    16661 2024-01-29 15:48:58.268016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_8.jpg
--rw-r--r--   0        0        0    12472 2024-01-29 15:48:58.268016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_9.jpg
--rw-r--r--   0        0        0    12311 2024-01-29 15:48:58.268016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_51.jpg
--rw-r--r--   0        0        0     9994 2024-01-29 15:48:58.268016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_52.jpg
--rw-r--r--   0        0        0    11263 2024-01-29 15:48:58.268016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_54.jpg
--rw-r--r--   0        0        0     8117 2024-01-29 15:48:58.268016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_55.jpg
--rw-r--r--   0        0        0    11981 2024-01-29 15:48:58.268016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_56.jpg
--rw-r--r--   0        0        0    11448 2024-01-29 15:48:58.268016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_57.jpg
--rw-r--r--   0        0        0    12943 2024-01-29 15:48:58.268016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_58.jpg
--rw-r--r--   0        0        0     8420 2024-01-29 15:48:58.268016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_59.jpg
--rw-r--r--   0        0        0    12161 2024-01-29 15:48:58.268016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_60.jpg
--rw-r--r--   0        0        0     9955 2024-01-29 15:48:58.268016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_61.jpg
--rw-r--r--   0        0        0     5846 2024-01-29 15:48:58.268016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_64.jpg
--rw-r--r--   0        0        0    10990 2024-01-29 15:48:58.268016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_65.jpg
--rw-r--r--   0        0        0    12918 2024-01-29 15:48:58.268016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_69.jpg
--rw-r--r--   0        0        0     5970 2024-01-29 15:48:58.268016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_70.jpg
--rw-r--r--   0        0        0     6994 2024-01-29 15:48:58.268016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/husky/train_imgs_870.jpg
--rw-r--r--   0        0        0     7000 2024-01-29 15:48:58.268016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/husky/train_imgs_871.jpg
--rw-r--r--   0        0        0    12981 2024-01-29 15:48:58.268016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/husky/train_imgs_880.jpg
--rw-r--r--   0        0        0    14382 2024-01-29 15:48:58.268016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/husky/train_imgs_883.jpg
--rw-r--r--   0        0        0    15311 2024-01-29 15:48:58.268016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/husky/train_imgs_886.jpg
--rw-r--r--   0        0        0    10559 2024-01-29 15:48:58.268016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/husky/train_imgs_891.jpg
--rw-r--r--   0        0        0    10480 2024-01-29 15:48:58.268016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/sit/train_imgs_818.jpg
--rw-r--r--   0        0        0     8542 2024-01-29 15:48:58.268016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/sit/train_imgs_824.jpg
--rw-r--r--   0        0        0    14742 2024-01-29 15:48:58.268016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/sit/train_imgs_830.jpg
--rw-r--r--   0        0        0    12741 2024-01-29 15:48:58.268016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/sit/train_imgs_836.jpg
--rw-r--r--   0        0        0     7379 2024-01-29 15:48:58.268016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/sit/train_imgs_837.jpg
--rw-r--r--   0        0        0    10502 2024-01-29 15:48:58.268016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/sit/train_imgs_849.jpg
--rw-r--r--   0        0        0    12901 2024-01-29 15:48:58.268016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/sit/train_imgs_858.jpg
--rw-r--r--   0        0        0    12306 2024-01-29 15:48:58.268016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1253.jpg
--rw-r--r--   0        0        0    13135 2024-01-29 15:48:58.272016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1254.jpg
--rw-r--r--   0        0        0    11655 2024-01-29 15:48:58.272016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1255.jpg
--rw-r--r--   0        0        0     9249 2024-01-29 15:48:58.272016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1256.jpg
--rw-r--r--   0        0        0     9864 2024-01-29 15:48:58.272016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1257.jpg
--rw-r--r--   0        0        0     7916 2024-01-29 15:48:58.272016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1258.jpg
--rw-r--r--   0        0        0    12006 2024-01-29 15:48:58.272016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1259.jpg
--rw-r--r--   0        0        0    13587 2024-01-29 15:48:58.272016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1260.jpg
--rw-r--r--   0        0        0     9525 2024-01-29 15:48:58.272016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1261.jpg
--rw-r--r--   0        0        0    12319 2024-01-29 15:48:58.272016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1262.jpg
--rw-r--r--   0        0        0     5809 2024-01-29 15:48:58.272016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1263.jpg
--rw-r--r--   0        0        0    13131 2024-01-29 15:48:58.272016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1264.jpg
--rw-r--r--   0        0        0    14144 2024-01-29 15:48:58.272016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1265.jpg
--rw-r--r--   0        0        0     8858 2024-01-29 15:48:58.272016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1266.jpg
--rw-r--r--   0        0        0    10242 2024-01-29 15:48:58.272016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1267.jpg
--rw-r--r--   0        0        0     8147 2024-01-29 15:48:58.272016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1268.jpg
--rw-r--r--   0        0        0     9221 2024-01-29 15:48:58.272016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1269.jpg
--rw-r--r--   0        0        0    12554 2024-01-29 15:48:58.272016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1270.jpg
--rw-r--r--   0        0        0     9174 2024-01-29 15:48:58.272016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1271.jpg
--rw-r--r--   0        0        0     5625 2024-01-29 15:48:58.272016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/flying/train_imgs_1.jpg
--rw-r--r--   0        0        0     4786 2024-01-29 15:48:58.272016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/flying/train_imgs_10.jpg
--rw-r--r--   0        0        0     8218 2024-01-29 15:48:58.272016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/flying/train_imgs_11.jpg
--rw-r--r--   0        0        0     6646 2024-01-29 15:48:58.272016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/flying/train_imgs_13.jpg
--rw-r--r--   0        0        0    11530 2024-01-29 15:48:58.272016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/flying/train_imgs_2.jpg
--rw-r--r--   0        0        0     6545 2024-01-29 15:48:58.272016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/flying/train_imgs_3.jpg
--rw-r--r--   0        0        0     9187 2024-01-29 15:48:58.272016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/flying/train_imgs_5.jpg
--rw-r--r--   0        0        0     7042 2024-01-29 15:48:58.272016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/flying/train_imgs_7.jpg
--rw-r--r--   0        0        0    12976 2024-01-29 15:48:58.272016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_1272.jpg
--rw-r--r--   0        0        0    12113 2024-01-29 15:48:58.272016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_1273.jpg
--rw-r--r--   0        0        0    12114 2024-01-29 15:48:58.272016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_1274.jpg
--rw-r--r--   0        0        0    15100 2024-01-29 15:48:58.272016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_1275.jpg
--rw-r--r--   0        0        0    15273 2024-01-29 15:48:58.272016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_1276.jpg
--rw-r--r--   0        0        0    10102 2024-01-29 15:48:58.272016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_1277.jpg
--rw-r--r--   0        0        0    13358 2024-01-29 15:48:58.272016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_1278.jpg
--rw-r--r--   0        0        0    12459 2024-01-29 15:48:58.272016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_1279.jpg
--rw-r--r--   0        0        0     8222 2024-01-29 15:48:58.272016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_1280.jpg
--rw-r--r--   0        0        0    12945 2024-01-29 15:48:58.272016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_1281.jpg
--rw-r--r--   0        0        0    10501 2024-01-29 15:48:58.272016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_1282.jpg
--rw-r--r--   0        0        0    12615 2024-01-29 15:48:58.272016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_1428.jpg
--rw-r--r--   0        0        0    11671 2024-01-29 15:48:58.272016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_2065.jpg
--rw-r--r--   0        0        0    13922 2024-01-29 15:48:58.272016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_2066.jpg
--rw-r--r--   0        0        0    10507 2024-01-29 15:48:58.272016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_2067.jpg
--rw-r--r--   0        0        0    10543 2024-01-29 15:48:58.276016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/sofa/train_imgs_609.jpg
--rw-r--r--   0        0        0    12217 2024-01-29 15:48:58.276016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/sofa/train_imgs_612.jpg
--rw-r--r--   0        0        0    10078 2024-01-29 15:48:58.276016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/sofa/train_imgs_614.jpg
--rw-r--r--   0        0        0    12026 2024-01-29 15:48:58.276016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/sofa/train_imgs_620.jpg
--rw-r--r--   0        0        0    10395 2024-01-29 15:48:58.276016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/vehicle/train_imgs_17.jpg
--rw-r--r--   0        0        0     4734 2024-01-29 15:48:58.276016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/vehicle/train_imgs_19.jpg
--rw-r--r--   0        0        0     6622 2024-01-29 15:48:58.276016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/vehicle/train_imgs_21.jpg
--rw-r--r--   0        0        0    10454 2024-01-29 15:48:58.276016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/vehicle/train_imgs_22.jpg
--rw-r--r--   0        0        0    14578 2024-01-29 15:48:58.276016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/vehicle/train_imgs_23.jpg
--rw-r--r--   0        0        0    13182 2024-01-29 15:48:58.276016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/vehicle/train_imgs_24.jpg
--rw-r--r--   0        0        0     5087 2024-01-29 15:48:58.276016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/vehicle/train_imgs_25.jpg
--rw-r--r--   0        0        0    12330 2024-01-29 15:48:58.276016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/vehicle/train_imgs_26.jpg
--rw-r--r--   0        0        0    11213 2024-01-29 15:48:58.276016 domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/vehicle/train_imgs_478.jpg
--rw-r--r--   0        0        0      236 2024-01-29 15:48:58.276016 domainlab-0.6.2/domainlab/zdata/ztest_files/aggret_res_test1
--rw-r--r--   0        0        0     1000 2024-01-29 15:48:58.276016 domainlab-0.6.2/domainlab/zdata/ztest_files/aggret_res_test11
--rw-r--r--   0        0        0      657 2024-01-29 15:48:58.276016 domainlab-0.6.2/domainlab/zdata/ztest_files/aggret_res_test2
--rw-r--r--   0        0        0     2806 2024-01-29 15:48:58.276016 domainlab-0.6.2/domainlab/zdata/ztest_files/aggret_res_test21
--rw-r--r--   0        0        0       96 2024-01-29 15:48:58.276016 domainlab-0.6.2/domainlab/zdata/ztest_files/dummy_file.py
--rw-r--r--   0        0        0       66 2024-01-29 15:48:58.276016 domainlab-0.6.2/domainlab/zdata/ztest_files/test_parameter_samples.csv
--rw-r--r--   0        0        0     1034 2024-03-28 15:14:04.263033 domainlab-0.6.2/pyproject.toml
--rw-r--r--   0        0        0    11469 1970-01-01 00:00:00.000000 domainlab-0.6.2/setup.py
--rw-r--r--   0        0        0     8480 1970-01-01 00:00:00.000000 domainlab-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-01-29 11:26:27.396178 domainlab-0.6.3/LICENSE
+-rw-r--r--   0        0        0     7530 2024-05-07 14:42:19.183023 domainlab-0.6.3/README.md
+-rw-r--r--   0        0        0       27 2024-01-29 11:26:27.424178 domainlab-0.6.3/domainlab/.gitignore
+-rw-r--r--   0        0        0      178 2024-01-29 11:26:27.424178 domainlab-0.6.3/domainlab/.pylintrc
+-rw-r--r--   0        0        0      751 2024-02-14 14:51:41.800238 domainlab-0.6.3/domainlab/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-29 11:26:27.424178 domainlab-0.6.3/domainlab/algos/__init__.py
+-rw-r--r--   0        0        0     1747 2024-02-14 14:51:41.800238 domainlab-0.6.3/domainlab/algos/a_algo_builder.py
+-rw-r--r--   0        0        0      984 2024-05-07 14:42:19.183023 domainlab-0.6.3/domainlab/algos/builder_api_model.py
+-rw-r--r--   0        0        0     5465 2024-05-07 14:42:19.183023 domainlab-0.6.3/domainlab/algos/builder_custom.py
+-rw-r--r--   0        0        0     3413 2024-05-07 14:42:19.183023 domainlab-0.6.3/domainlab/algos/builder_dann.py
+-rw-r--r--   0        0        0     2320 2024-05-07 14:42:19.183023 domainlab-0.6.3/domainlab/algos/builder_diva.py
+-rw-r--r--   0        0        0     1808 2024-05-07 14:42:19.183023 domainlab-0.6.3/domainlab/algos/builder_erm.py
+-rw-r--r--   0        0        0     2007 2024-05-07 14:42:19.183023 domainlab-0.6.3/domainlab/algos/builder_hduva.py
+-rw-r--r--   0        0        0     3044 2024-05-07 14:42:19.183023 domainlab-0.6.3/domainlab/algos/builder_jigen1.py
+-rw-r--r--   0        0        0        0 2024-01-29 11:26:27.424178 domainlab-0.6.3/domainlab/algos/msels/__init__.py
+-rw-r--r--   0        0        0     3578 2024-05-07 14:42:19.183023 domainlab-0.6.3/domainlab/algos/msels/a_model_sel.py
+-rw-r--r--   0        0        0     2097 2024-05-07 14:42:19.183023 domainlab-0.6.3/domainlab/algos/msels/c_msel_oracle.py
+-rw-r--r--   0        0        0     1551 2024-05-07 14:42:19.183023 domainlab-0.6.3/domainlab/algos/msels/c_msel_tr_loss.py
+-rw-r--r--   0        0        0     2596 2024-05-07 14:42:19.183023 domainlab-0.6.3/domainlab/algos/msels/c_msel_val.py
+-rw-r--r--   0        0        0        0 2024-01-29 11:26:27.424178 domainlab-0.6.3/domainlab/algos/observers/__init__.py
+-rw-r--r--   0        0        0     1551 2024-02-14 14:51:41.800238 domainlab-0.6.3/domainlab/algos/observers/a_observer.py
+-rw-r--r--   0        0        0     6143 2024-05-07 14:42:19.183023 domainlab-0.6.3/domainlab/algos/observers/b_obvisitor.py
+-rw-r--r--   0        0        0      682 2024-02-14 14:51:41.800238 domainlab-0.6.3/domainlab/algos/observers/c_obvisitor_cleanup.py
+-rw-r--r--   0        0        0     1593 2024-02-14 14:51:41.800238 domainlab-0.6.3/domainlab/algos/observers/c_obvisitor_gen.py
+-rw-r--r--   0        0        0        0 2024-01-29 11:26:27.424178 domainlab-0.6.3/domainlab/algos/trainers/__init__.py
+-rw-r--r--   0        0        0     7446 2024-05-08 07:00:41.969076 domainlab-0.6.3/domainlab/algos/trainers/a_trainer.py
+-rw-r--r--   0        0        0      842 2024-02-14 14:51:41.800238 domainlab-0.6.3/domainlab/algos/trainers/args_dial.py
+-rw-r--r--   0        0        0        0 2024-02-13 14:36:50.564658 domainlab-0.6.3/domainlab/algos/trainers/compos/__init__.py
+-rw-r--r--   0        0        0      613 2024-02-14 14:51:41.800238 domainlab-0.6.3/domainlab/algos/trainers/compos/matchdg_args.py
+-rw-r--r--   0        0        0    18836 2024-02-14 14:51:41.800238 domainlab-0.6.3/domainlab/algos/trainers/compos/matchdg_match.py
+-rw-r--r--   0        0        0     5095 2024-02-14 14:51:41.800238 domainlab-0.6.3/domainlab/algos/trainers/compos/matchdg_utils.py
+-rw-r--r--   0        0        0     1971 2024-02-14 14:51:41.800238 domainlab-0.6.3/domainlab/algos/trainers/hyper_scheduler.py
+-rw-r--r--   0        0        0     3556 2024-02-14 14:51:41.800238 domainlab-0.6.3/domainlab/algos/trainers/train_basic.py
+-rw-r--r--   0        0        0     2094 2024-02-14 14:51:41.800238 domainlab-0.6.3/domainlab/algos/trainers/train_dial.py
+-rw-r--r--   0        0        0     7802 2024-05-07 14:42:19.183023 domainlab-0.6.3/domainlab/algos/trainers/train_fishr.py
+-rw-r--r--   0        0        0     2421 2024-02-14 14:51:41.800238 domainlab-0.6.3/domainlab/algos/trainers/train_hyper_scheduler.py
+-rw-r--r--   0        0        0    15390 2024-02-14 14:51:41.800238 domainlab-0.6.3/domainlab/algos/trainers/train_matchdg.py
+-rw-r--r--   0        0        0     4355 2024-02-14 14:51:41.800238 domainlab-0.6.3/domainlab/algos/trainers/train_mldg.py
+-rw-r--r--   0        0        0     2316 2024-05-08 07:00:36.677035 domainlab-0.6.3/domainlab/algos/trainers/zoo_trainer.py
+-rw-r--r--   0        0        0      317 2024-02-14 14:51:41.800238 domainlab-0.6.3/domainlab/algos/utils.py
+-rw-r--r--   0        0        0     1975 2024-02-14 14:51:41.800238 domainlab-0.6.3/domainlab/algos/zoo_algos.py
+-rw-r--r--   0        0        0    11306 2024-05-07 14:42:19.183023 domainlab-0.6.3/domainlab/arg_parser.py
+-rw-r--r--   0        0        0      813 2024-02-14 14:51:41.800238 domainlab-0.6.3/domainlab/cli.py
+-rw-r--r--   0        0        0        0 2024-01-29 11:26:27.424178 domainlab-0.6.3/domainlab/compos/__init__.py
+-rw-r--r--   0        0        0     1524 2024-02-14 14:51:41.800238 domainlab-0.6.3/domainlab/compos/a_nn_builder.py
+-rw-r--r--   0        0        0     1517 2024-02-14 14:51:41.800238 domainlab-0.6.3/domainlab/compos/builder_nn_alex.py
+-rw-r--r--   0        0        0     1496 2024-02-14 14:51:41.800238 domainlab-0.6.3/domainlab/compos/builder_nn_conv_bn_relu_2.py
+-rw-r--r--   0        0        0     1461 2024-02-14 14:51:41.800238 domainlab-0.6.3/domainlab/compos/builder_nn_external_from_file.py
+-rw-r--r--   0        0        0        0 2024-01-29 11:26:27.424178 domainlab-0.6.3/domainlab/compos/nn_zoo/__init__.py
+-rw-r--r--   0        0        0      854 2024-02-14 14:51:41.800238 domainlab-0.6.3/domainlab/compos/nn_zoo/net_adversarial.py
+-rw-r--r--   0        0        0      740 2024-02-14 14:51:41.800238 domainlab-0.6.3/domainlab/compos/nn_zoo/net_classif.py
+-rw-r--r--   0        0        0     2851 2024-02-14 14:51:41.800238 domainlab-0.6.3/domainlab/compos/nn_zoo/net_conv_conv_bn_pool_2.py
+-rw-r--r--   0        0        0     2173 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/compos/nn_zoo/net_gated.py
+-rw-r--r--   0        0        0     1077 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/compos/nn_zoo/nn.py
+-rw-r--r--   0        0        0     2876 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/compos/nn_zoo/nn_alex.py
+-rw-r--r--   0        0        0      860 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/compos/nn_zoo/nn_torchvision.py
+-rw-r--r--   0        0        0        0 2024-02-13 14:36:50.568659 domainlab-0.6.3/domainlab/compos/pcr/__init__.py
+-rw-r--r--   0        0        0     4858 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/compos/pcr/p_chain_handler.py
+-rw-r--r--   0        0        0     1096 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/compos/pcr/request.py
+-rw-r--r--   0        0        0      617 2024-01-29 11:26:27.428178 domainlab-0.6.3/domainlab/compos/utils_conv_get_flat_dim.py
+-rw-r--r--   0        0        0        0 2024-02-13 14:36:50.568659 domainlab-0.6.3/domainlab/compos/vae/__init__.py
+-rw-r--r--   0        0        0      799 2024-01-29 11:26:27.428178 domainlab-0.6.3/domainlab/compos/vae/a_model_builder.py
+-rw-r--r--   0        0        0     1327 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/compos/vae/a_vae_builder.py
+-rw-r--r--   0        0        0     1854 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/compos/vae/c_vae_adaptor_model_recon.py
+-rw-r--r--   0        0        0     1347 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/compos/vae/c_vae_builder_classif.py
+-rw-r--r--   0        0        0     3663 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/compos/vae/c_vae_recon.py
+-rw-r--r--   0        0        0        0 2024-02-13 14:36:50.568659 domainlab-0.6.3/domainlab/compos/vae/compos/__init__.py
+-rw-r--r--   0        0        0     2256 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/compos/vae/compos/decoder_concat_vec_reshape_conv.py
+-rw-r--r--   0        0        0     2241 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/compos/vae/compos/decoder_concat_vec_reshape_conv_gated_conv.py
+-rw-r--r--   0        0        0     1493 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/compos/vae/compos/decoder_cond_prior.py
+-rw-r--r--   0        0        0     1604 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/compos/vae/compos/decoder_losses.py
+-rw-r--r--   0        0        0     3027 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/compos/vae/compos/encoder.py
+-rw-r--r--   0        0        0      771 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/compos/vae/compos/encoder_dirichlet.py
+-rw-r--r--   0        0        0     1667 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/compos/vae/compos/encoder_domain_topic.py
+-rw-r--r--   0        0        0     1557 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/compos/vae/compos/encoder_domain_topic_img2topic.py
+-rw-r--r--   0        0        0     1732 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/compos/vae/compos/encoder_domain_topic_img_topic2zd.py
+-rw-r--r--   0        0        0     5256 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/compos/vae/compos/encoder_xyd_parallel.py
+-rw-r--r--   0        0        0     2813 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/compos/vae/compos/encoder_xydt_elevator.py
+-rw-r--r--   0        0        0     1884 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/compos/vae/compos/encoder_zy.py
+-rw-r--r--   0        0        0     1274 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/compos/vae/utils_request_chain_builder.py
+-rw-r--r--   0        0        0     3817 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/compos/vae/zoo_vae_builders_classif.py
+-rw-r--r--   0        0        0     1383 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/compos/vae/zoo_vae_builders_classif_topic.py
+-rw-r--r--   0        0        0     1561 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/compos/zoo_nn.py
+-rw-r--r--   0        0        0        0 2024-01-29 11:26:27.428178 domainlab-0.6.3/domainlab/dsets/__init__.py
+-rw-r--r--   0        0        0     6071 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/dsets/a_dset_mnist_color_rgb_solo.py
+-rw-r--r--   0        0        0     1350 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/dsets/dset_img_path_list.py
+-rw-r--r--   0        0        0      845 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/dsets/dset_mnist_color_solo_default.py
+-rw-r--r--   0        0        0     1455 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/dsets/dset_poly_domains_mnist_color_default.py
+-rw-r--r--   0        0        0     6238 2024-05-07 14:42:19.183023 domainlab-0.6.3/domainlab/dsets/dset_subfolder.py
+-rw-r--r--   0        0        0      226 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/dsets/utils_color_palette.py
+-rw-r--r--   0        0        0     2377 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/dsets/utils_data.py
+-rw-r--r--   0        0        0     7195 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/dsets/utils_wrapdset_patches.py
+-rw-r--r--   0        0        0        0 2024-02-13 14:36:50.568659 domainlab-0.6.3/domainlab/exp/__init__.py
+-rw-r--r--   0        0        0      750 2024-02-13 14:36:51.128659 domainlab-0.6.3/domainlab/exp/exp_cuda_seed.py
+-rwxr-xr-x   0        0        0     4779 2024-05-07 14:42:19.183023 domainlab-0.6.3/domainlab/exp/exp_main.py
+-rw-r--r--   0        0        0    10609 2024-05-07 14:42:19.183023 domainlab-0.6.3/domainlab/exp/exp_utils.py
+-rw-r--r--   0        0        0        0 2024-01-29 11:26:27.428178 domainlab-0.6.3/domainlab/exp_protocol/__init__.py
+-rw-r--r--   0        0        0     1753 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/exp_protocol/aggregate_results.py
+-rw-r--r--   0        0        0     7481 2024-05-07 14:42:19.183023 domainlab-0.6.3/domainlab/exp_protocol/benchmark.smk
+-rw-r--r--   0        0        0     6831 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/exp_protocol/run_experiment.py
+-rw-r--r--   0        0        0     1236 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/mk_exp.py
+-rw-r--r--   0        0        0        0 2024-01-29 11:26:27.428178 domainlab-0.6.3/domainlab/models/__init__.py
+-rw-r--r--   0        0        0     6054 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/models/a_model.py
+-rw-r--r--   0        0        0     8917 2024-05-07 14:42:19.183023 domainlab-0.6.3/domainlab/models/a_model_classif.py
+-rw-r--r--   0        0        0      853 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/models/args_jigen.py
+-rw-r--r--   0        0        0     2063 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/models/args_vae.py
+-rw-r--r--   0        0        0     1370 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/models/interface_vae_xyd.py
+-rw-r--r--   0        0        0      452 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/models/model_custom.py
+-rw-r--r--   0        0        0     3785 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/models/model_dann.py
+-rw-r--r--   0        0        0     5905 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/models/model_diva.py
+-rw-r--r--   0        0        0     1719 2024-05-07 14:42:19.183023 domainlab-0.6.3/domainlab/models/model_erm.py
+-rw-r--r--   0        0        0     8327 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/models/model_hduva.py
+-rw-r--r--   0        0        0     4888 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/models/model_jigen.py
+-rw-r--r--   0        0        0     1364 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/models/model_vae_xyd_classif.py
+-rw-r--r--   0        0        0      105 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/tasks/__init__.py
+-rw-r--r--   0        0        0     5826 2024-05-07 14:42:19.183023 domainlab-0.6.3/domainlab/tasks/a_task.py
+-rw-r--r--   0        0        0     2128 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/tasks/a_task_classif.py
+-rw-r--r--   0        0        0     3294 2024-05-07 14:42:19.183023 domainlab-0.6.3/domainlab/tasks/b_task.py
+-rw-r--r--   0        0        0     1514 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/tasks/b_task_classif.py
+-rw-r--r--   0        0        0     2099 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/tasks/task_dset.py
+-rw-r--r--   0        0        0     3931 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/tasks/task_folder.py
+-rw-r--r--   0        0        0     2540 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/tasks/task_folder_mk.py
+-rw-r--r--   0        0        0     1993 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/tasks/task_mini_vlcs.py
+-rw-r--r--   0        0        0     2357 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/tasks/task_mnist_color.py
+-rw-r--r--   0        0        0     4851 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/tasks/task_pathlist.py
+-rw-r--r--   0        0        0      897 2024-01-29 11:26:27.428178 domainlab-0.6.3/domainlab/tasks/task_utils.py
+-rw-r--r--   0        0        0     8747 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/tasks/utils_task.py
+-rw-r--r--   0        0        0     1954 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/tasks/utils_task_dset.py
+-rw-r--r--   0        0        0     1791 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/tasks/zoo_tasks.py
+-rw-r--r--   0        0        0        0 2024-01-29 11:26:27.428178 domainlab-0.6.3/domainlab/utils/__init__.py
+-rw-r--r--   0        0        0     4722 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/utils/flows_gen_img_model.py
+-rw-r--r--   0        0        0    23007 2024-05-07 14:42:19.183023 domainlab-0.6.3/domainlab/utils/generate_benchmark_plots.py
+-rw-r--r--   0        0        0     1378 2024-02-14 14:51:41.804238 domainlab-0.6.3/domainlab/utils/get_git_tag.py
+-rw-r--r--   0        0        0    17718 2024-02-14 14:51:41.808238 domainlab-0.6.3/domainlab/utils/hyperparameter_gridsearch.py
+-rw-r--r--   0        0        0    17564 2024-02-14 14:51:41.808238 domainlab-0.6.3/domainlab/utils/hyperparameter_sampling.py
+-rw-r--r--   0        0        0     1415 2024-02-14 14:51:41.808238 domainlab-0.6.3/domainlab/utils/logger.py
+-rw-r--r--   0        0        0      802 2024-02-14 14:51:41.808238 domainlab-0.6.3/domainlab/utils/override_interface.py
+-rw-r--r--   0        0        0     2216 2024-02-14 14:51:41.808238 domainlab-0.6.3/domainlab/utils/perf.py
+-rw-r--r--   0        0        0     3783 2024-02-14 14:51:41.808238 domainlab-0.6.3/domainlab/utils/perf_metrics.py
+-rw-r--r--   0        0        0     3371 2024-02-14 14:51:41.808238 domainlab-0.6.3/domainlab/utils/sanity_check.py
+-rw-r--r--   0        0        0      915 2024-02-14 14:51:41.808238 domainlab-0.6.3/domainlab/utils/test_img.py
+-rw-r--r--   0        0        0      336 2024-01-29 11:26:27.428178 domainlab-0.6.3/domainlab/utils/u_import.py
+-rw-r--r--   0        0        0     2023 2024-02-14 14:51:41.808238 domainlab-0.6.3/domainlab/utils/u_import_net_module.py
+-rw-r--r--   0        0        0      884 2024-02-14 14:51:41.808238 domainlab-0.6.3/domainlab/utils/utils_class.py
+-rw-r--r--   0        0        0     1317 2024-02-14 14:51:41.808238 domainlab-0.6.3/domainlab/utils/utils_classif.py
+-rw-r--r--   0        0        0      544 2024-02-14 14:51:41.808238 domainlab-0.6.3/domainlab/utils/utils_cuda.py
+-rw-r--r--   0        0        0     1185 2024-02-14 14:51:41.808238 domainlab-0.6.3/domainlab/utils/utils_img_sav.py
+-rw-r--r--   0        0        0       12 2024-02-14 14:51:41.808238 domainlab-0.6.3/domainlab/zdata/mixed_codec/caltech/auto/text.txt
+-rw-r--r--   0        0        0     8579 2024-02-14 14:51:41.808238 domainlab-0.6.3/domainlab/zdata/mixed_codec/caltech/auto/train_imgs_150.jpg
+-rw-r--r--   0        0        0     8521 2024-02-14 14:51:41.808238 domainlab-0.6.3/domainlab/zdata/mixed_codec/caltech/auto/train_imgs_151.jpg
+-rw-r--r--   0        0        0    62574 2024-02-14 14:51:41.808238 domainlab-0.6.3/domainlab/zdata/mixed_codec/caltech/auto/train_imgs_152.png
+-rw-r--r--   0        0        0     6984 2024-02-14 14:51:41.808238 domainlab-0.6.3/domainlab/zdata/mixed_codec/caltech/vogel/train_imgs_1.jpg
+-rw-r--r--   0        0        0    10707 2024-02-14 14:51:41.808238 domainlab-0.6.3/domainlab/zdata/mixed_codec/caltech/vogel/train_imgs_2.jpg
+-rw-r--r--   0        0        0    48698 2024-02-14 14:51:41.808238 domainlab-0.6.3/domainlab/zdata/mixed_codec/caltech/vogel/train_imgs_3.png
+-rw-r--r--   0        0        0    10543 2024-02-14 14:51:41.808238 domainlab-0.6.3/domainlab/zdata/mixed_codec/sun/sofa/train_imgs_609.jpg
+-rw-r--r--   0        0        0    12217 2024-02-14 14:51:41.808238 domainlab-0.6.3/domainlab/zdata/mixed_codec/sun/sofa/train_imgs_612.jpg
+-rw-r--r--   0        0        0    10395 2024-02-14 14:51:41.808238 domainlab-0.6.3/domainlab/zdata/mixed_codec/sun/vehicle/train_imgs_17.jpg
+-rw-r--r--   0        0        0     4734 2024-02-14 14:51:41.808238 domainlab-0.6.3/domainlab/zdata/mixed_codec/sun/vehicle/train_imgs_19.jpg
+-rw-r--r--   0        0        0    10736 2024-02-14 14:51:41.808238 domainlab-0.6.3/domainlab/zdata/pacs_mini_10/art_painting/dog/pic_195.jpg
+-rw-r--r--   0        0        0    35963 2024-02-14 14:51:41.808238 domainlab-0.6.3/domainlab/zdata/pacs_mini_10/art_painting/dog/pic_304.jpg
+-rw-r--r--   0        0        0    39114 2024-02-14 14:51:41.808238 domainlab-0.6.3/domainlab/zdata/pacs_mini_10/art_painting/elephant/pic_026.jpg
+-rw-r--r--   0        0        0    16324 2024-02-14 14:51:41.808238 domainlab-0.6.3/domainlab/zdata/pacs_mini_10/art_painting/giraffe/pic_243.jpg
+-rw-r--r--   0        0        0    27254 2024-02-14 14:51:41.808238 domainlab-0.6.3/domainlab/zdata/pacs_mini_10/art_painting/guitar/pic_020.jpg
+-rw-r--r--   0        0        0    37953 2024-02-14 14:51:41.808238 domainlab-0.6.3/domainlab/zdata/pacs_mini_10/art_painting/guitar/pic_182.jpg
+-rw-r--r--   0        0        0    21398 2024-02-14 14:51:41.808238 domainlab-0.6.3/domainlab/zdata/pacs_mini_10/art_painting/horse/pic_142.jpg
+-rw-r--r--   0        0        0    27377 2024-02-14 14:51:41.808238 domainlab-0.6.3/domainlab/zdata/pacs_mini_10/art_painting/person/pic_165.jpg
+-rw-r--r--   0        0        0    18550 2024-02-14 14:51:41.808238 domainlab-0.6.3/domainlab/zdata/pacs_mini_10/art_painting/person/pic_199.jpg
+-rw-r--r--   0        0        0    21402 2024-02-14 14:51:41.808238 domainlab-0.6.3/domainlab/zdata/pacs_mini_10/art_painting/person/pic_497.jpg
+-rw-r--r--   0        0        0    20448 2024-02-14 14:51:41.808238 domainlab-0.6.3/domainlab/zdata/pacs_mini_10/cartoon/dog/pic_112.jpg
+-rw-r--r--   0        0        0    26362 2024-02-14 14:51:41.808238 domainlab-0.6.3/domainlab/zdata/pacs_mini_10/cartoon/dog/pic_137.jpg
+-rw-r--r--   0        0        0    20540 2024-02-14 14:51:41.808238 domainlab-0.6.3/domainlab/zdata/pacs_mini_10/cartoon/dog/pic_219.jpg
+-rw-r--r--   0        0        0    18461 2024-02-14 14:51:41.808238 domainlab-0.6.3/domainlab/zdata/pacs_mini_10/cartoon/elephant/pic_332.jpg
+-rw-r--r--   0        0        0    33171 2024-02-14 14:51:41.808238 domainlab-0.6.3/domainlab/zdata/pacs_mini_10/cartoon/giraffe/pic_377.jpg
+-rw-r--r--   0        0        0    20113 2024-02-14 14:51:41.808238 domainlab-0.6.3/domainlab/zdata/pacs_mini_10/cartoon/giraffe/pic_382.jpg
+-rw-r--r--   0        0        0    22002 2024-02-14 14:51:41.808238 domainlab-0.6.3/domainlab/zdata/pacs_mini_10/cartoon/horse/pic_064.jpg
+-rw-r--r--   0        0        0    12438 2024-02-14 14:51:41.808238 domainlab-0.6.3/domainlab/zdata/pacs_mini_10/cartoon/house/pic_040.jpg
+-rw-r--r--   0        0        0    21770 2024-02-14 14:51:41.808238 domainlab-0.6.3/domainlab/zdata/pacs_mini_10/cartoon/person/pic_111.jpg
+-rw-r--r--   0        0        0    18691 2024-02-14 14:51:41.808238 domainlab-0.6.3/domainlab/zdata/pacs_mini_10/cartoon/person/pic_180.jpg
+-rw-r--r--   0        0        0      498 2024-02-14 14:51:41.808238 domainlab-0.6.3/domainlab/zdata/pacs_mini_10/main.sh
+-rw-r--r--   0        0        0    23240 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/pacs_mini_10/photo/dog/n02103406_1011.jpg
+-rw-r--r--   0        0        0    23174 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/pacs_mini_10/photo/elephant/n02503517_6232.jpg
+-rw-r--r--   0        0        0    11646 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/pacs_mini_10/photo/guitar/n02676566_7830.jpg
+-rw-r--r--   0        0        0    21822 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/pacs_mini_10/photo/horse/105_0223.jpg
+-rw-r--r--   0        0        0    25832 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/pacs_mini_10/photo/house/pic_046.jpg
+-rw-r--r--   0        0        0    23408 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/pacs_mini_10/photo/house/pic_110.jpg
+-rw-r--r--   0        0        0    27674 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/pacs_mini_10/photo/house/pic_146.jpg
+-rw-r--r--   0        0        0    27298 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/pacs_mini_10/photo/house/pic_218.jpg
+-rw-r--r--   0        0        0    23829 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/pacs_mini_10/photo/person/253_0221.jpg
+-rw-r--r--   0        0        0    17983 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/pacs_mini_10/photo/person/253_0297.jpg
+-rw-r--r--   0        0        0      544 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/pacs_mini_10/run_with_bash_copy_files_according2txt.sh
+-rw-r--r--   0        0        0     8767 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/pacs_mini_10/sketch/dog/5302.png
+-rw-r--r--   0        0        0     8032 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/pacs_mini_10/sketch/dog/5317.png
+-rw-r--r--   0        0        0    13745 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/pacs_mini_10/sketch/dog/n02103406_3255-6.png
+-rw-r--r--   0        0        0     6480 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/pacs_mini_10/sketch/elephant/5981.png
+-rw-r--r--   0        0        0    13120 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/pacs_mini_10/sketch/elephant/n02503517_12688-4.png
+-rw-r--r--   0        0        0    13602 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/pacs_mini_10/sketch/giraffe/n02439033_13384-2.png
+-rw-r--r--   0        0        0    12858 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/pacs_mini_10/sketch/guitar/n02676566_8618-2.png
+-rw-r--r--   0        0        0     8300 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/pacs_mini_10/sketch/guitar/n03467517_6423-3.png
+-rw-r--r--   0        0        0    16388 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/pacs_mini_10/sketch/horse/n02374451_779-1.png
+-rw-r--r--   0        0        0     8519 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/pacs_mini_10/sketch/house/8873.png
+-rw-r--r--   0        0        0      336 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/pacs_split/art_painting_10.txt
+-rw-r--r--   0        0        0     3335 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/pacs_split/art_painting_100.txt
+-rw-r--r--   0        0        0     6988 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/pacs_split/art_painting_crossval_kfold.txt
+-rw-r--r--   0        0        0    68794 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/pacs_split/art_painting_test_kfold.txt
+-rw-r--r--   0        0        0    61806 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/pacs_split/art_painting_train_kfold.txt
+-rw-r--r--   0        0        0      283 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/pacs_split/cartoon_10.txt
+-rw-r--r--   0        0        0     2882 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/pacs_split/cartoon_100.txt
+-rw-r--r--   0        0        0     6821 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/pacs_split/cartoon_crossval_kfold.txt
+-rw-r--r--   0        0        0    67457 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/pacs_split/cartoon_test_kfold.txt
+-rw-r--r--   0        0        0    60636 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/pacs_split/cartoon_train_kfold.txt
+-rw-r--r--   0        0        0      288 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/pacs_split/photo_10.txt
+-rw-r--r--   0        0        0     2940 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/pacs_split/photo_100.txt
+-rw-r--r--   0        0        0     4714 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/pacs_split/photo_crossval_kfold.txt
+-rw-r--r--   0        0        0    48735 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/pacs_split/photo_test_kfold.txt
+-rw-r--r--   0        0        0    44021 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/pacs_split/photo_train_kfold.txt
+-rw-r--r--   0        0        0      527 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/pacs_split/readme.txt
+-rw-r--r--   0        0        0      317 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/pacs_split/sketch_10.txt
+-rw-r--r--   0        0        0     3549 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/pacs_split/sketch_100.txt
+-rw-r--r--   0        0        0    13338 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/pacs_split/sketch_crossval_kfold.txt
+-rw-r--r--   0        0        0   137732 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/pacs_split/sketch_test_kfold.txt
+-rw-r--r--   0        0        0   124394 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/pacs_split/sketch_train_kfold.txt
+-rw-r--r--   0        0        0     7328 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/patches_permutation4jigsaw/permutations_100.npy
+-rw-r--r--   0        0        0     2288 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/patches_permutation4jigsaw/permutations_30.npy
+-rw-r--r--   0        0        0     2360 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/patches_permutation4jigsaw/permutations_31.npy
+-rw-r--r--   0        0        0     1456 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/script/download_pacs.py
+-rw-r--r--   0        0        0     8579 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_150.jpg
+-rw-r--r--   0        0        0     8521 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_151.jpg
+-rw-r--r--   0        0        0    10449 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_152.jpg
+-rw-r--r--   0        0        0     9205 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_153.jpg
+-rw-r--r--   0        0        0     7298 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_154.jpg
+-rw-r--r--   0        0        0     9788 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_155.jpg
+-rw-r--r--   0        0        0     9149 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_156.jpg
+-rw-r--r--   0        0        0     9900 2024-02-14 14:51:41.812238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_157.jpg
+-rw-r--r--   0        0        0     8077 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_158.jpg
+-rw-r--r--   0        0        0     7873 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_159.jpg
+-rw-r--r--   0        0        0     7561 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_160.jpg
+-rw-r--r--   0        0        0     7589 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_161.jpg
+-rw-r--r--   0        0        0    10250 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_162.jpg
+-rw-r--r--   0        0        0     8990 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_163.jpg
+-rw-r--r--   0        0        0    11370 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_164.jpg
+-rw-r--r--   0        0        0     7264 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_165.jpg
+-rw-r--r--   0        0        0    10782 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_166.jpg
+-rw-r--r--   0        0        0     9162 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_167.jpg
+-rw-r--r--   0        0        0     6964 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_168.jpg
+-rw-r--r--   0        0        0     9243 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_169.jpg
+-rw-r--r--   0        0        0    20748 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/hund/train_imgs_302.jpg
+-rw-r--r--   0        0        0    13099 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/hund/train_imgs_303.jpg
+-rw-r--r--   0        0        0    12864 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/hund/train_imgs_304.jpg
+-rw-r--r--   0        0        0     9116 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/hund/train_imgs_305.jpg
+-rw-r--r--   0        0        0     5890 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/hund/train_imgs_306.jpg
+-rw-r--r--   0        0        0     7751 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/hund/train_imgs_307.jpg
+-rw-r--r--   0        0        0     9665 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/hund/train_imgs_308.jpg
+-rw-r--r--   0        0        0    11819 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/hund/train_imgs_309.jpg
+-rw-r--r--   0        0        0    10768 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/hund/train_imgs_310.jpg
+-rw-r--r--   0        0        0    16572 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/hund/train_imgs_311.jpg
+-rw-r--r--   0        0        0     8817 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/hund/train_imgs_312.jpg
+-rw-r--r--   0        0        0     9740 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/mensch/train_imgs_344.jpg
+-rw-r--r--   0        0        0    10158 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/mensch/train_imgs_345.jpg
+-rw-r--r--   0        0        0     9840 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/mensch/train_imgs_346.jpg
+-rw-r--r--   0        0        0    10481 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/mensch/train_imgs_347.jpg
+-rw-r--r--   0        0        0     8690 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/mensch/train_imgs_348.jpg
+-rw-r--r--   0        0        0    10165 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/mensch/train_imgs_349.jpg
+-rw-r--r--   0        0        0     9983 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/mensch/train_imgs_350.jpg
+-rw-r--r--   0        0        0    14865 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/mensch/train_imgs_351.jpg
+-rw-r--r--   0        0        0    12113 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/mensch/train_imgs_352.jpg
+-rw-r--r--   0        0        0     9920 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/stuhl/train_imgs_227.jpg
+-rw-r--r--   0        0        0    12394 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/stuhl/train_imgs_228.jpg
+-rw-r--r--   0        0        0     7599 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/stuhl/train_imgs_229.jpg
+-rw-r--r--   0        0        0    11468 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/stuhl/train_imgs_230.jpg
+-rw-r--r--   0        0        0     9058 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/stuhl/train_imgs_231.jpg
+-rw-r--r--   0        0        0     7892 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/stuhl/train_imgs_232.jpg
+-rw-r--r--   0        0        0     6984 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/vogel/train_imgs_1.jpg
+-rw-r--r--   0        0        0    10707 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/vogel/train_imgs_2.jpg
+-rw-r--r--   0        0        0     5810 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/vogel/train_imgs_3.jpg
+-rw-r--r--   0        0        0     6592 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/vogel/train_imgs_4.jpg
+-rw-r--r--   0        0        0     8453 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/vogel/train_imgs_5.jpg
+-rw-r--r--   0        0        0     6281 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/vogel/train_imgs_6.jpg
+-rw-r--r--   0        0        0     8756 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/vogel/train_imgs_7.jpg
+-rw-r--r--   0        0        0    16157 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/vogel/train_imgs_8.jpg
+-rw-r--r--   0        0        0     8404 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/vogel/train_imgs_9.jpg
+-rw-r--r--   0        0        0     3088 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_1.jpg
+-rw-r--r--   0        0        0    10181 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_10.jpg
+-rw-r--r--   0        0        0    11434 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_11.jpg
+-rw-r--r--   0        0        0    11728 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_12.jpg
+-rw-r--r--   0        0        0    11491 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_13.jpg
+-rw-r--r--   0        0        0     3988 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_14.jpg
+-rw-r--r--   0        0        0    13956 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_15.jpg
+-rw-r--r--   0        0        0    16745 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_16.jpg
+-rw-r--r--   0        0        0    14936 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_17.jpg
+-rw-r--r--   0        0        0    13577 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_18.jpg
+-rw-r--r--   0        0        0     9233 2024-02-14 14:51:41.816238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_19.jpg
+-rw-r--r--   0        0        0     8456 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_2.jpg
+-rw-r--r--   0        0        0    13275 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_20.jpg
+-rw-r--r--   0        0        0    12724 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_21.jpg
+-rw-r--r--   0        0        0    10267 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_22.jpg
+-rw-r--r--   0        0        0     6757 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_23.jpg
+-rw-r--r--   0        0        0    10767 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_24.jpg
+-rw-r--r--   0        0        0     5647 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_25.jpg
+-rw-r--r--   0        0        0    11123 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_26.jpg
+-rw-r--r--   0        0        0    12004 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_27.jpg
+-rw-r--r--   0        0        0    11538 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_28.jpg
+-rw-r--r--   0        0        0     5494 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_29.jpg
+-rw-r--r--   0        0        0    13925 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_3.jpg
+-rw-r--r--   0        0        0    16120 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_30.jpg
+-rw-r--r--   0        0        0    11315 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_31.jpg
+-rw-r--r--   0        0        0     9502 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_32.jpg
+-rw-r--r--   0        0        0     5206 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_33.jpg
+-rw-r--r--   0        0        0    11163 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_34.jpg
+-rw-r--r--   0        0        0    13437 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_35.jpg
+-rw-r--r--   0        0        0    12934 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_36.jpg
+-rw-r--r--   0        0        0     8358 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_37.jpg
+-rw-r--r--   0        0        0    14004 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_38.jpg
+-rw-r--r--   0        0        0    17970 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_39.jpg
+-rw-r--r--   0        0        0    11457 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_4.jpg
+-rw-r--r--   0        0        0    17124 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_40.jpg
+-rw-r--r--   0        0        0     6786 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_41.jpg
+-rw-r--r--   0        0        0    14007 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_42.jpg
+-rw-r--r--   0        0        0     8201 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_43.jpg
+-rw-r--r--   0        0        0    12656 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_44.jpg
+-rw-r--r--   0        0        0     7061 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_45.jpg
+-rw-r--r--   0        0        0     9186 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_46.jpg
+-rw-r--r--   0        0        0    12622 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_47.jpg
+-rw-r--r--   0        0        0    10099 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_48.jpg
+-rw-r--r--   0        0        0     8449 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_49.jpg
+-rw-r--r--   0        0        0    13827 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_5.jpg
+-rw-r--r--   0        0        0     7836 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_50.jpg
+-rw-r--r--   0        0        0    13309 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_6.jpg
+-rw-r--r--   0        0        0     8804 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_7.jpg
+-rw-r--r--   0        0        0    16661 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_8.jpg
+-rw-r--r--   0        0        0    12472 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_9.jpg
+-rw-r--r--   0        0        0    12311 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_51.jpg
+-rw-r--r--   0        0        0     9994 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_52.jpg
+-rw-r--r--   0        0        0    11263 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_54.jpg
+-rw-r--r--   0        0        0     8117 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_55.jpg
+-rw-r--r--   0        0        0    11981 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_56.jpg
+-rw-r--r--   0        0        0    11448 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_57.jpg
+-rw-r--r--   0        0        0    12943 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_58.jpg
+-rw-r--r--   0        0        0     8420 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_59.jpg
+-rw-r--r--   0        0        0    12161 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_60.jpg
+-rw-r--r--   0        0        0     9955 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_61.jpg
+-rw-r--r--   0        0        0     5846 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_64.jpg
+-rw-r--r--   0        0        0    10990 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_65.jpg
+-rw-r--r--   0        0        0    12918 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_69.jpg
+-rw-r--r--   0        0        0     5970 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_70.jpg
+-rw-r--r--   0        0        0     6994 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/husky/train_imgs_870.jpg
+-rw-r--r--   0        0        0     7000 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/husky/train_imgs_871.jpg
+-rw-r--r--   0        0        0    12981 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/husky/train_imgs_880.jpg
+-rw-r--r--   0        0        0    14382 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/husky/train_imgs_883.jpg
+-rw-r--r--   0        0        0    15311 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/husky/train_imgs_886.jpg
+-rw-r--r--   0        0        0    10559 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/husky/train_imgs_891.jpg
+-rw-r--r--   0        0        0    10480 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/sit/train_imgs_818.jpg
+-rw-r--r--   0        0        0     8542 2024-02-14 14:51:41.820238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/sit/train_imgs_824.jpg
+-rw-r--r--   0        0        0    14742 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/sit/train_imgs_830.jpg
+-rw-r--r--   0        0        0    12741 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/sit/train_imgs_836.jpg
+-rw-r--r--   0        0        0     7379 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/sit/train_imgs_837.jpg
+-rw-r--r--   0        0        0    10502 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/sit/train_imgs_849.jpg
+-rw-r--r--   0        0        0    12901 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/sit/train_imgs_858.jpg
+-rw-r--r--   0        0        0    12306 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1253.jpg
+-rw-r--r--   0        0        0    13135 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1254.jpg
+-rw-r--r--   0        0        0    11655 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1255.jpg
+-rw-r--r--   0        0        0     9249 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1256.jpg
+-rw-r--r--   0        0        0     9864 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1257.jpg
+-rw-r--r--   0        0        0     7916 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1258.jpg
+-rw-r--r--   0        0        0    12006 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1259.jpg
+-rw-r--r--   0        0        0    13587 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1260.jpg
+-rw-r--r--   0        0        0     9525 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1261.jpg
+-rw-r--r--   0        0        0    12319 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1262.jpg
+-rw-r--r--   0        0        0     5809 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1263.jpg
+-rw-r--r--   0        0        0    13131 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1264.jpg
+-rw-r--r--   0        0        0    14144 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1265.jpg
+-rw-r--r--   0        0        0     8858 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1266.jpg
+-rw-r--r--   0        0        0    10242 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1267.jpg
+-rw-r--r--   0        0        0     8147 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1268.jpg
+-rw-r--r--   0        0        0     9221 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1269.jpg
+-rw-r--r--   0        0        0    12554 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1270.jpg
+-rw-r--r--   0        0        0     9174 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1271.jpg
+-rw-r--r--   0        0        0     5625 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/flying/train_imgs_1.jpg
+-rw-r--r--   0        0        0     4786 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/flying/train_imgs_10.jpg
+-rw-r--r--   0        0        0     8218 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/flying/train_imgs_11.jpg
+-rw-r--r--   0        0        0     6646 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/flying/train_imgs_13.jpg
+-rw-r--r--   0        0        0    11530 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/flying/train_imgs_2.jpg
+-rw-r--r--   0        0        0     6545 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/flying/train_imgs_3.jpg
+-rw-r--r--   0        0        0     9187 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/flying/train_imgs_5.jpg
+-rw-r--r--   0        0        0     7042 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/flying/train_imgs_7.jpg
+-rw-r--r--   0        0        0    12976 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_1272.jpg
+-rw-r--r--   0        0        0    12113 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_1273.jpg
+-rw-r--r--   0        0        0    12114 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_1274.jpg
+-rw-r--r--   0        0        0    15100 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_1275.jpg
+-rw-r--r--   0        0        0    15273 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_1276.jpg
+-rw-r--r--   0        0        0    10102 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_1277.jpg
+-rw-r--r--   0        0        0    13358 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_1278.jpg
+-rw-r--r--   0        0        0    12459 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_1279.jpg
+-rw-r--r--   0        0        0     8222 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_1280.jpg
+-rw-r--r--   0        0        0    12945 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_1281.jpg
+-rw-r--r--   0        0        0    10501 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_1282.jpg
+-rw-r--r--   0        0        0    12615 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_1428.jpg
+-rw-r--r--   0        0        0    11671 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_2065.jpg
+-rw-r--r--   0        0        0    13922 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_2066.jpg
+-rw-r--r--   0        0        0    10507 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_2067.jpg
+-rw-r--r--   0        0        0    10543 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/sofa/train_imgs_609.jpg
+-rw-r--r--   0        0        0    12217 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/sofa/train_imgs_612.jpg
+-rw-r--r--   0        0        0    10078 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/sofa/train_imgs_614.jpg
+-rw-r--r--   0        0        0    12026 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/sofa/train_imgs_620.jpg
+-rw-r--r--   0        0        0    10395 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/vehicle/train_imgs_17.jpg
+-rw-r--r--   0        0        0     4734 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/vehicle/train_imgs_19.jpg
+-rw-r--r--   0        0        0     6622 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/vehicle/train_imgs_21.jpg
+-rw-r--r--   0        0        0    10454 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/vehicle/train_imgs_22.jpg
+-rw-r--r--   0        0        0    14578 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/vehicle/train_imgs_23.jpg
+-rw-r--r--   0        0        0    13182 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/vehicle/train_imgs_24.jpg
+-rw-r--r--   0        0        0     5087 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/vehicle/train_imgs_25.jpg
+-rw-r--r--   0        0        0    12330 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/vehicle/train_imgs_26.jpg
+-rw-r--r--   0        0        0    11213 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/vehicle/train_imgs_478.jpg
+-rw-r--r--   0        0        0      236 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/ztest_files/aggret_res_test1
+-rw-r--r--   0        0        0     1000 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/ztest_files/aggret_res_test11
+-rw-r--r--   0        0        0      657 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/ztest_files/aggret_res_test2
+-rw-r--r--   0        0        0     2806 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/ztest_files/aggret_res_test21
+-rw-r--r--   0        0        0       96 2024-02-14 14:51:41.824238 domainlab-0.6.3/domainlab/zdata/ztest_files/dummy_file.py
+-rw-r--r--   0        0        0       69 2024-05-07 14:42:19.183023 domainlab-0.6.3/domainlab/zdata/ztest_files/test_parameter_samples.csv
+-rw-r--r--   0        0        0     1017 2024-05-08 07:04:05.090502 domainlab-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0    11609 1970-01-01 00:00:00.000000 domainlab-0.6.3/setup.py
+-rw-r--r--   0        0        0     8574 1970-01-01 00:00:00.000000 domainlab-0.6.3/PKG-INFO
```

### Comparing `domainlab-0.6.2/LICENSE` & `domainlab-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/README.md` & `domainlab-0.6.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -4,43 +4,56 @@
 [![codecov](https://codecov.io/gh/marrlab/DomainLab/branch/master/graph/badge.svg)](https://app.codecov.io/gh/marrlab/DomainLab)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/bc22a1f9afb742efb02b87284e04dc86)](https://www.codacy.com/gh/marrlab/DomainLab/dashboard)
 [![Documentation](https://img.shields.io/badge/Documentation-Here)](https://marrlab.github.io/DomainLab/)
 [![pages-build-deployment](https://github.com/marrlab/DomainLab/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/marrlab/DomainLab/actions/workflows/pages/pages-build-deployment)
 
 ## Distribution shifts, domain generalization and DomainLab
 
-Neural networks trained using data from a specific distribution (domain) usually fails to generalize to novel distributions (domains). Domain generalization aims at learning domain invariant features by utilizing data from multiple domains (data sites, corhorts, batches, vendors) so the learned feature can generalize to new unseen domains (distributions).
+Neural networks trained using data from a specific distribution (domain) usually fail to generalize to novel distributions (domains). Domain generalization aims at learning domain invariant features by utilizing data from multiple domains (data sites, cohorts, batches, vendors) so the learned feature can be generalized to new unseen domains (distributions).
 
-DomainLab is a software platform with state-of-the-art domain generalization algorithms implemented, designed by maximal decoupling of different software components thus enhances maximal code reuse.
+DomainLab is a software platform with state-of-the-art domain generalization algorithms implemented and designed by maximal decoupling of different software components thus enhancing maximal code reuse.
 
 ### DomainLab
 DomainLab decouples the following concepts or objects:
-- task $M$: In DomainLab, a task is a container for datasets from different domains. (e.g. from distribution $D_1$ and $D_2$). Task offer a static protocol to evaluate the generalization performance of a neural network: which dataset(s) is used for training, wich dataset(s) used for testing.  
-- neural network: a map $\phi$ from the input data to the feature space and a map $\varphi$ from feature space to output $\hat{y}$ (e.g. decision variable).
+- task $M$: In DomainLab, a task is a container for datasets from different domains. (e.g. from distribution $D_1$ and $D_2$). The task offers a static protocol to evaluate the generalization performance of a neural network: which dataset(s) is used for training, and which dataset(s) is used for testing.  
+- neural network: a map $\phi$ from the input data to the feature space and a map $\varphi$ from the feature space to output $\hat{y}$ (e.g. decision variable).
 - model: structural risk in the form of $\ell() + \mu R()$  where
-  - $\ell(Y, \hat{y}=\varphi(\phi(X)))$ is the task specific empirical loss (e.g. cross entropy for classification task).
+  - $\ell(Y, \hat{y}=\varphi(\phi(X)))$ is the task-specific empirical loss (e.g. cross entropy for classification task).
   - $R(\phi(X))$ is the penalty loss to boost domain invariant feature extraction using $\phi$.
   - $\mu$ is the corresponding multiplier to each penalty function factor.
 - trainer:  an object that guides the data flow to model and append further domain invariant losses
 like inter-domain feature alignment.
 
-We offer detailed documentation on how these models and trainers work in our documentation page: https://marrlab.github.io/DomainLab/
+We offer detailed documentation on how these models and trainers work on our documentation page: https://marrlab.github.io/DomainLab/
 
-DomainLab makes it possible to combine models with models, trainers with models, and trainers with trainers in a decorator pattern like line of code `Trainer A(Trainer B(Model C(Model D(network E), network E, network F)))` which correspond to $\ell() + \mu_a R_a() + \mu_b R_b + \mu_c R_c() + \mu_d R_d()$, where Model C and Model D share neural network E, but Model C has an extra neural network F. All models share the same neural network for feature extraction, but can have different auxilliary networks for $R()$.
+DomainLab makes it possible to combine models with models, trainers with models, and trainers with trainers in a decorator pattern like the line of code below
+
+```
+Trainer A(
+		  Trainer B(Model C(
+						    Model D(network E),
+							network E,
+							network F
+						   )
+				   )
+	     )
+```
+
+which correspond to $\ell() + \mu_a R_a() + \mu_b R_b + \mu_c R_c() + \mu_d R_d()$, where Model C and Model D share neural network E, but Model C has an extra neural network F. All models share the same neural network for feature extraction, but can have different auxiliary networks for $R()$.
 
 <div style="align: center; text-align:center;">
 <figure>  
 <img src="https://github.com/marrlab/DomainLab/blob/master/docs/figs/invarfeat4dg.png?raw=true" style="width:300px;"/> 
 </figure>
 </div>
 
 ## Getting started
 
 ### Installation
-For development version in Github, see [Installation and Dependencies handling](./docs/doc_install.md)
+For the development version in Github, see [Installation and Dependencies handling](./docs/doc_install.md)
 
 We also offer a PyPI version here https://pypi.org/project/domainlab/  which one could install via `pip install domainlab` and it is recommended to create a virtual environment for it.
 
 ### Task specification
 We offer various ways for the user to specify a scenario to evaluate the generalization performance via training on a limited number of datasets. See detail in
 [Task Specification](./docs/doc_tasks.md) 
 
@@ -51,15 +64,15 @@
 
 ```shell
 python main_out.py --help
 ```
 
 or 
 
-```shell
+```
 domainlab --help
 ```
 
 #### Command line configuration file
 
 `domainlab -c ./examples/conf/vlcs_diva_mldg_dial.yaml` (if you install via pip)
```

### Comparing `domainlab-0.6.2/domainlab/__init__.py` & `domainlab-0.6.3/domainlab/__init__.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/algos/a_algo_builder.py` & `domainlab-0.6.3/domainlab/algos/a_algo_builder.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/algos/builder_api_model.py` & `domainlab-0.6.3/domainlab/algos/builder_api_model.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,11 +16,11 @@
 
     def init_business(self, exp):
         """
         return trainer, model, observer
         """
         args = exp.args
         device = get_device(args)
-        model_sel = MSelOracleVisitor(MSelValPerf(max_es=args.es))
+        model_sel = MSelOracleVisitor(MSelValPerf(max_es=args.es), val_threshold=args.val_threshold)
         observer = ObVisitor(model_sel)
         trainer = TrainerChainNodeGetter(args.trainer)(default="hyperscheduler")
         return trainer, None, observer, device
```

### Comparing `domainlab-0.6.2/domainlab/algos/builder_custom.py` & `domainlab-0.6.3/domainlab/algos/builder_custom.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,16 @@
         def init_business(self, exp):
             """
             return trainer, model, observer
             """
             task = exp.task
             args = exp.args
             device = get_device(args)
-            model_sel = MSelOracleVisitor(MSelValPerf(max_es=args.es))
+            model_sel = MSelOracleVisitor(MSelValPerf(max_es=args.es),
+                                          val_threshold=args.val_threshold)
             observer = ObVisitor(model_sel)
             model = class_name_model(net_classifier=None, list_str_y=task.list_str_y)
             model = self.init_next_model(model, exp)
             self.set_nets_from_dictionary(args, task, model)
             trainer = self.get_trainer(args)
             trainer.init_business(model, task, observer, device, args)
             return trainer, model, observer, device
```

### Comparing `domainlab-0.6.2/domainlab/algos/builder_dann.py` & `domainlab-0.6.3/domainlab/algos/builder_dann.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         return trainer, model, observer
         """
         task = exp.task
         self._task = task
         args = exp.args
         task.get_list_domains_tr_te(args.tr_d, args.te_d)
         device = get_device(args)
-        msel = MSelOracleVisitor(MSelValPerf(max_es=args.es))
+        msel = MSelOracleVisitor(MSelValPerf(max_es=args.es), val_threshold=args.val_threshold)
         observer = ObVisitor(msel)
         observer = ObVisitorCleanUp(observer)
 
         builder = FeatExtractNNBuilderChainNodeGetter(
             args, arg_name_of_net="nname", arg_path_of_net="npath"
         )()  # request, @FIXME, constant string
```

### Comparing `domainlab-0.6.2/domainlab/algos/builder_diva.py` & `domainlab-0.6.3/domainlab/algos/builder_diva.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             gamma_d=args.gamma_d,
             gamma_y=args.gamma_y,
             beta_x=args.beta_x,
             beta_y=args.beta_y,
             beta_d=args.beta_d,
         )
         device = get_device(args)
-        model_sel = MSelOracleVisitor(MSelValPerf(max_es=args.es))
+        model_sel = MSelOracleVisitor(MSelValPerf(max_es=args.es), val_threshold=args.val_threshold)
         if not args.gen:
             observer = ObVisitor(model_sel)
         else:
             observer = ObVisitorGen(model_sel)
 
         observer = ObVisitorCleanUp(observer)
         trainer = self.get_trainer(args)
```

### Comparing `domainlab-0.6.2/domainlab/algos/builder_erm.py` & `domainlab-0.6.3/domainlab/algos/builder_erm.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     def init_business(self, exp):
         """
         return trainer, model, observer
         """
         task = exp.task
         args = exp.args
         device = get_device(args)
-        model_sel = MSelOracleVisitor(MSelValPerf(max_es=args.es))
+        model_sel = MSelOracleVisitor(MSelValPerf(max_es=args.es), val_threshold=args.val_threshold)
         observer = ObVisitor(model_sel)
 
         builder = FeatExtractNNBuilderChainNodeGetter(
             args, arg_name_of_net="nname", arg_path_of_net="npath"
         )()  # request, # @FIXME, constant string
 
         net = builder.init_business(
```

### Comparing `domainlab-0.6.2/domainlab/algos/builder_hduva.py` & `domainlab-0.6.3/domainlab/algos/builder_hduva.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,12 +39,12 @@
             gamma_y=args.gamma_y,
             beta_t=args.beta_t,
             beta_x=args.beta_x,
             beta_y=args.beta_y,
             beta_d=args.beta_d,
         )
         model = self.init_next_model(model, exp)
-        model_sel = MSelOracleVisitor(MSelValPerf(max_es=args.es))
+        model_sel = MSelOracleVisitor(MSelValPerf(max_es=args.es), val_threshold=args.val_threshold)
         observer = ObVisitorCleanUp(ObVisitor(model_sel))
         trainer = TrainerChainNodeGetter(args.trainer)(default="hyperscheduler")
         trainer.init_business(model, task, observer, device, args)
         return trainer, model, observer, device
```

### Comparing `domainlab-0.6.2/domainlab/algos/builder_jigen1.py` & `domainlab-0.6.3/domainlab/algos/builder_jigen1.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     def init_business(self, exp):
         """
         return trainer, model, observer
         """
         task = exp.task
         args = exp.args
         device = get_device(args)
-        msel = MSelOracleVisitor(msel=MSelValPerf(max_es=args.es))
+        msel = MSelOracleVisitor(msel=MSelValPerf(max_es=args.es), val_threshold=args.val_threshold)
         observer = ObVisitor(msel)
         observer = ObVisitorCleanUp(observer)
 
         builder = FeatExtractNNBuilderChainNodeGetter(
             args, arg_name_of_net="nname", arg_path_of_net="npath"
         )()  # request, @FIXME, constant string
```

### Comparing `domainlab-0.6.2/domainlab/algos/msels/a_model_sel.py` & `domainlab-0.6.3/domainlab/algos/msels/a_model_sel.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,23 +6,24 @@
 
 
 class AMSel(metaclass=abc.ABCMeta):
     """
     Abstract Model Selection
     """
 
-    def __init__(self):
+    def __init__(self, val_threshold = None):
         """
         trainer and tr_observer
         """
         self.trainer = None
         self._observer = None
         self.msel = None
         self._max_es = None
         self._model_selection_epoch = None
+        self._val_threshold = val_threshold
 
     def reset(self):
         """
         reset observer via reset model selector
         """
         if self.msel is not None:
             self.msel.reset()
@@ -69,25 +70,35 @@
     def base_update(self, clear_counter=False):
         """
         observer + visitor pattern to trainer
         if the best model should be updated
         return boolean
         """
 
-    def if_stop(self):
+    def if_stop(self, acc_val = None):
         """
-        check if trainer should stop
+        check if trainer should stop and additionally tests for validation threshold
         return boolean
         """
         # NOTE: since if_stop is not abstract, one has to
         # be careful to always override it in child class
         # only if the child class has a decorator which will
         # dispatched.
+        if self.msel is not None and acc_val is not None:
+            if self._val_threshold is not None and acc_val < self._val_threshold:
+                return False
+        return self.early_stop()
+
+    def early_stop(self):
+        """
+        check if trainer should stop
+        return boolean
+        """
         if self.msel is not None:
-            return self.msel.if_stop()
+            return self.msel.early_stop()
         raise NotImplementedError
 
     @property
     def best_val_acc(self):
         """
         decoratee best val acc
         """
@@ -117,7 +128,14 @@
     def model_selection_epoch(self):
         """
         the epoch when the model was selected
         """
         if self._model_selection_epoch is not None:
             return self._model_selection_epoch
         return -1
+
+    @property
+    def val_threshold(self):
+        """
+        the treshold below which we don't stop early
+        """
+        return self._val_threshold
```

### Comparing `domainlab-0.6.2/domainlab/algos/msels/c_msel_oracle.py` & `domainlab-0.6.3/domainlab/algos/msels/c_msel_oracle.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 
 class MSelOracleVisitor(AMSel):
     """
     save best out-of-domain test acc model, but do not affect
     how the final model is selected
     """
 
-    def __init__(self, msel=None):
+    def __init__(self, msel=None, val_threshold = None):
         """
         Decorator pattern
         """
-        super().__init__()
+        super().__init__(val_threshold)
         self.best_oracle_acc = 0
         self.msel = msel
 
     @property
     def oracle_last_setpoint_sel_te_acc(self):
         """
         last setpoint acc
@@ -48,21 +48,21 @@
             logger = Logger.get_logger()
             logger.info("new oracle model saved")
             flag = True
         if self.msel is not None:
             return self.msel.base_update(clear_counter)
         return flag
 
-    def if_stop(self):
+    def early_stop(self):
         """
         if should early stop
         oracle model selection does not intervene how models get selected
         by the innermost model selection
         """
         if self.msel is not None:
-            return self.msel.if_stop()
+            return self.msel.early_stop()
         return False
 
     def accept(self, trainer, observer4msel):
         if self.msel is not None:
             self.msel.accept(trainer, observer4msel)
         super().accept(trainer, observer4msel)
```

### Comparing `domainlab-0.6.2/domainlab/algos/msels/c_msel_tr_loss.py` & `domainlab-0.6.3/domainlab/algos/msels/c_msel_tr_loss.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
 class MSelTrLoss(AMSel):
     """
     1. Model selection using sum of loss across training domains
     2. Visitor pattern to trainer
     """
 
-    def __init__(self, max_es):
-        super().__init__()
+    def __init__(self, max_es, val_threshold = None):
+        super().__init__(val_threshold)
         # NOTE: super() must come first otherwise it will overwrite existing
         # values!
         self.reset()
         self._max_es = max_es
 
     def reset(self):
         self.best_loss = float("inf")
@@ -46,12 +46,12 @@
             logger.info(f"loss:{loss}, best loss: {self.best_loss}")
             flag = False  # do not update best model
             if clear_counter:
                 logger.info("clearing counter")
                 self.es_c = 0
         return flag
 
-    def if_stop(self):
+    def early_stop(self):
         """
         if should early stop
         """
         return self.es_c >= self.max_es
```

### Comparing `domainlab-0.6.2/domainlab/algos/msels/c_msel_val.py` & `domainlab-0.6.3/domainlab/algos/msels/c_msel_val.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 class MSelValPerf(MSelTrLoss):
     """
     1. Model selection using validation performance
     2. Visitor pattern to trainer
     """
 
-    def __init__(self, max_es):
-        super().__init__(max_es)  # construct self.observer4msel (observer)
+    def __init__(self, max_es, val_threshold = None):
+        super().__init__(max_es, val_threshold)  # construct self.observer4msel (observer)
         self.reset()
 
     def reset(self):
         super().reset()
         self._best_val_acc = 0.0
         self._sel_model_te_acc = 0.0
         self._best_te_metric = 0.0
```

### Comparing `domainlab-0.6.2/domainlab/algos/observers/a_observer.py` & `domainlab-0.6.3/domainlab/algos/observers/a_observer.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/algos/observers/b_obvisitor.py` & `domainlab-0.6.3/domainlab/algos/observers/b_obvisitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,16 @@
                     self.loader_te, self.device
                 )
                 self.metric_te = metric_te
         if self.model_sel.update(epoch):
             logger.info("better model found")
             self.host_trainer.model.save()
             logger.info("persisted")
-        flag_stop = self.model_sel.if_stop()
+        acc = self.metric_te.get("acc")
+        flag_stop = self.model_sel.if_stop(acc)
         flag_enough = epoch >= self.host_trainer.aconf.epos_min
         return flag_stop & flag_enough
 
     def accept(self, trainer):
         """
         accept invitation as a visitor
         """
```

### Comparing `domainlab-0.6.2/domainlab/algos/observers/c_obvisitor_cleanup.py` & `domainlab-0.6.3/domainlab/algos/observers/c_obvisitor_cleanup.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/algos/observers/c_obvisitor_gen.py` & `domainlab-0.6.3/domainlab/algos/observers/c_obvisitor_gen.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/algos/trainers/a_trainer.py` & `domainlab-0.6.3/domainlab/algos/trainers/a_trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,17 @@
         """
         # Note self.decoratee can be both model and trainer,
         # but self._decoratee can only be trainer!
         if self._decoratee is not None:
             self._decoratee.init_business(
                 model, task, observer, device, aconf, flag_accept
             )
-        self.model = model
+            self.model = self._decoratee
+        else:
+            self.model = model
         self.task = task
         self.task.init_business(trainer=self, args=aconf)
         self.model.list_d_tr = self.task.list_domain_tr
         self.observer = observer
         self.device = device
         self.aconf = aconf
         #
```

### Comparing `domainlab-0.6.2/domainlab/algos/trainers/args_dial.py` & `domainlab-0.6.3/domainlab/algos/trainers/args_dial.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/algos/trainers/compos/matchdg_args.py` & `domainlab-0.6.3/domainlab/algos/trainers/compos/matchdg_args.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/algos/trainers/compos/matchdg_match.py` & `domainlab-0.6.3/domainlab/algos/trainers/compos/matchdg_match.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/algos/trainers/compos/matchdg_utils.py` & `domainlab-0.6.3/domainlab/algos/trainers/compos/matchdg_utils.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/algos/trainers/hyper_scheduler.py` & `domainlab-0.6.3/domainlab/algos/trainers/hyper_scheduler.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/algos/trainers/train_basic.py` & `domainlab-0.6.3/domainlab/algos/trainers/train_basic.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/algos/trainers/train_dial.py` & `domainlab-0.6.3/domainlab/algos/trainers/train_dial.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/algos/trainers/train_fishr.py` & `domainlab-0.6.3/domainlab/algos/trainers/train_fishr.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/algos/trainers/train_hyper_scheduler.py` & `domainlab-0.6.3/domainlab/algos/trainers/train_hyper_scheduler.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/algos/trainers/train_matchdg.py` & `domainlab-0.6.3/domainlab/algos/trainers/train_matchdg.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/algos/trainers/train_mldg.py` & `domainlab-0.6.3/domainlab/algos/trainers/train_mldg.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/algos/trainers/zoo_trainer.py` & `domainlab-0.6.3/domainlab/algos/trainers/zoo_trainer.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/algos/zoo_algos.py` & `domainlab-0.6.3/domainlab/algos/zoo_algos.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/arg_parser.py` & `domainlab-0.6.3/domainlab/arg_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,14 +240,21 @@
         type=str,
         default=None,
         help="algorithm configuration name, (default None)",
     )
 
     parser.add_argument("--task", metavar="ta", type=str, help="task name")
 
+    parser.add_argument(
+        "--val_threshold",
+        type=float,
+        default=None,
+        help="Accuracy threshold before early stopping can be applied"
+    )
+
     arg_group_task = parser.add_argument_group("task args")
 
     arg_group_task.add_argument(
         "--bs", type=int, default=100, help="loader batch size for mixed domains"
     )
 
     arg_group_task.add_argument(
```

### Comparing `domainlab-0.6.2/domainlab/cli.py` & `domainlab-0.6.3/domainlab/cli.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/compos/a_nn_builder.py` & `domainlab-0.6.3/domainlab/compos/a_nn_builder.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/compos/builder_nn_alex.py` & `domainlab-0.6.3/domainlab/compos/builder_nn_alex.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/compos/builder_nn_conv_bn_relu_2.py` & `domainlab-0.6.3/domainlab/compos/builder_nn_conv_bn_relu_2.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/compos/builder_nn_external_from_file.py` & `domainlab-0.6.3/domainlab/compos/builder_nn_external_from_file.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/compos/nn_zoo/net_adversarial.py` & `domainlab-0.6.3/domainlab/compos/nn_zoo/net_adversarial.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/compos/nn_zoo/net_classif.py` & `domainlab-0.6.3/domainlab/compos/nn_zoo/net_classif.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/compos/nn_zoo/net_conv_conv_bn_pool_2.py` & `domainlab-0.6.3/domainlab/compos/nn_zoo/net_conv_conv_bn_pool_2.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/compos/nn_zoo/net_gated.py` & `domainlab-0.6.3/domainlab/compos/nn_zoo/net_gated.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/compos/nn_zoo/nn.py` & `domainlab-0.6.3/domainlab/compos/nn_zoo/nn.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/compos/nn_zoo/nn_alex.py` & `domainlab-0.6.3/domainlab/compos/nn_zoo/nn_alex.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/compos/nn_zoo/nn_torchvision.py` & `domainlab-0.6.3/domainlab/compos/nn_zoo/nn_torchvision.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/compos/pcr/p_chain_handler.py` & `domainlab-0.6.3/domainlab/compos/pcr/p_chain_handler.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/compos/pcr/request.py` & `domainlab-0.6.3/domainlab/compos/pcr/request.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/compos/utils_conv_get_flat_dim.py` & `domainlab-0.6.3/domainlab/compos/utils_conv_get_flat_dim.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/compos/vae/a_model_builder.py` & `domainlab-0.6.3/domainlab/compos/vae/a_model_builder.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/compos/vae/a_vae_builder.py` & `domainlab-0.6.3/domainlab/compos/vae/a_vae_builder.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/compos/vae/c_vae_adaptor_model_recon.py` & `domainlab-0.6.3/domainlab/compos/vae/c_vae_adaptor_model_recon.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/compos/vae/c_vae_builder_classif.py` & `domainlab-0.6.3/domainlab/compos/vae/c_vae_builder_classif.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/compos/vae/c_vae_recon.py` & `domainlab-0.6.3/domainlab/compos/vae/c_vae_recon.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/compos/vae/compos/decoder_concat_vec_reshape_conv.py` & `domainlab-0.6.3/domainlab/compos/vae/compos/decoder_concat_vec_reshape_conv.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/compos/vae/compos/decoder_concat_vec_reshape_conv_gated_conv.py` & `domainlab-0.6.3/domainlab/compos/vae/compos/decoder_concat_vec_reshape_conv_gated_conv.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/compos/vae/compos/decoder_cond_prior.py` & `domainlab-0.6.3/domainlab/compos/vae/compos/decoder_cond_prior.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/compos/vae/compos/decoder_losses.py` & `domainlab-0.6.3/domainlab/compos/vae/compos/decoder_losses.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/compos/vae/compos/encoder.py` & `domainlab-0.6.3/domainlab/compos/vae/compos/encoder.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/compos/vae/compos/encoder_dirichlet.py` & `domainlab-0.6.3/domainlab/compos/vae/compos/encoder_dirichlet.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/compos/vae/compos/encoder_domain_topic.py` & `domainlab-0.6.3/domainlab/compos/vae/compos/encoder_domain_topic.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/compos/vae/compos/encoder_domain_topic_img2topic.py` & `domainlab-0.6.3/domainlab/compos/vae/compos/encoder_domain_topic_img2topic.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/compos/vae/compos/encoder_domain_topic_img_topic2zd.py` & `domainlab-0.6.3/domainlab/compos/vae/compos/encoder_domain_topic_img_topic2zd.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/compos/vae/compos/encoder_xyd_parallel.py` & `domainlab-0.6.3/domainlab/compos/vae/compos/encoder_xyd_parallel.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/compos/vae/compos/encoder_xydt_elevator.py` & `domainlab-0.6.3/domainlab/compos/vae/compos/encoder_xydt_elevator.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/compos/vae/compos/encoder_zy.py` & `domainlab-0.6.3/domainlab/compos/vae/compos/encoder_zy.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/compos/vae/utils_request_chain_builder.py` & `domainlab-0.6.3/domainlab/compos/vae/utils_request_chain_builder.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/compos/vae/zoo_vae_builders_classif.py` & `domainlab-0.6.3/domainlab/compos/vae/zoo_vae_builders_classif.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/compos/vae/zoo_vae_builders_classif_topic.py` & `domainlab-0.6.3/domainlab/compos/vae/zoo_vae_builders_classif_topic.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/compos/zoo_nn.py` & `domainlab-0.6.3/domainlab/compos/zoo_nn.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/dsets/a_dset_mnist_color_rgb_solo.py` & `domainlab-0.6.3/domainlab/dsets/a_dset_mnist_color_rgb_solo.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/dsets/dset_img_path_list.py` & `domainlab-0.6.3/domainlab/dsets/dset_img_path_list.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/dsets/dset_mnist_color_solo_default.py` & `domainlab-0.6.3/domainlab/dsets/dset_mnist_color_solo_default.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/dsets/dset_poly_domains_mnist_color_default.py` & `domainlab-0.6.3/domainlab/dsets/dset_poly_domains_mnist_color_default.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/dsets/dset_subfolder.py` & `domainlab-0.6.3/domainlab/dsets/dset_subfolder.py`

 * *Files 6% similar despite different names*

```diff
@@ -148,13 +148,15 @@
                 for d in os.listdir(mdir)
                 if os.path.isdir(os.path.join(mdir, d)) and d in self.list_class_dir
             ]
         flag_user_input_classes_in_folder = set(self.list_class_dir) <= set(classes)
         if not flag_user_input_classes_in_folder:
             logger.info(f"user provided class names: {self.list_class_dir}")
             logger.info(f"subfolder names from folder: {mdir} {classes}")
+            unmatched_names = set(self.list_class_dir) - set(classes)
+            logger.info(f"unmatched class names provided by user: {unmatched_names}")
             raise RuntimeError(
                 "user provided class names does not match the subfolder names"
             )
         classes.sort()
         class_to_idx = {classes[i]: i for i in range(len(classes))}
         return classes, class_to_idx
```

### Comparing `domainlab-0.6.2/domainlab/dsets/utils_data.py` & `domainlab-0.6.3/domainlab/dsets/utils_data.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/dsets/utils_wrapdset_patches.py` & `domainlab-0.6.3/domainlab/dsets/utils_wrapdset_patches.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/exp/exp_cuda_seed.py` & `domainlab-0.6.3/domainlab/exp/exp_cuda_seed.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/exp/exp_main.py` & `domainlab-0.6.3/domainlab/exp/exp_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
             sancheck = SanityCheck(args, self.task)
             sancheck.dataset_sanity_check()
 
         if model is not None:
             self.model = model
         self.epochs = self.args.epos
         self.epoch_counter = 1
+        self.val_threshold = args.val_threshold
         if observer is None:
             observer = observer_default
         if not self.trainer.flag_initialized:
             self.trainer.init_business(self.model, self.task, observer, device, args)
         self.visitor = visitor(self)  # visitor depends on task initialization first
         # visitor must be initialized last after trainer is initialized
         self.experiment_duration = None
```

### Comparing `domainlab-0.6.2/domainlab/exp/exp_utils.py` & `domainlab-0.6.3/domainlab/exp/exp_utils.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/exp_protocol/aggregate_results.py` & `domainlab-0.6.3/domainlab/exp_protocol/aggregate_results.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/exp_protocol/benchmark.smk` & `domainlab-0.6.3/domainlab/exp_protocol/benchmark.smk`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/exp_protocol/run_experiment.py` & `domainlab-0.6.3/domainlab/exp_protocol/run_experiment.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/mk_exp.py` & `domainlab-0.6.3/domainlab/mk_exp.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/models/a_model.py` & `domainlab-0.6.3/domainlab/models/a_model.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/models/a_model_classif.py` & `domainlab-0.6.3/domainlab/models/a_model_classif.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/models/args_jigen.py` & `domainlab-0.6.3/domainlab/models/args_jigen.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/models/args_vae.py` & `domainlab-0.6.3/domainlab/models/args_vae.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/models/interface_vae_xyd.py` & `domainlab-0.6.3/domainlab/models/interface_vae_xyd.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/models/model_dann.py` & `domainlab-0.6.3/domainlab/models/model_dann.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/models/model_diva.py` & `domainlab-0.6.3/domainlab/models/model_diva.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/models/model_erm.py` & `domainlab-0.6.3/domainlab/models/model_erm.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/models/model_hduva.py` & `domainlab-0.6.3/domainlab/models/model_hduva.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/models/model_jigen.py` & `domainlab-0.6.3/domainlab/models/model_jigen.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/models/model_vae_xyd_classif.py` & `domainlab-0.6.3/domainlab/models/model_vae_xyd_classif.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/tasks/a_task.py` & `domainlab-0.6.3/domainlab/tasks/a_task.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/tasks/a_task_classif.py` & `domainlab-0.6.3/domainlab/tasks/a_task_classif.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/tasks/b_task.py` & `domainlab-0.6.3/domainlab/tasks/b_task.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/tasks/b_task_classif.py` & `domainlab-0.6.3/domainlab/tasks/b_task_classif.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/tasks/task_dset.py` & `domainlab-0.6.3/domainlab/tasks/task_dset.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/tasks/task_folder.py` & `domainlab-0.6.3/domainlab/tasks/task_folder.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/tasks/task_folder_mk.py` & `domainlab-0.6.3/domainlab/tasks/task_folder_mk.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/tasks/task_mini_vlcs.py` & `domainlab-0.6.3/domainlab/tasks/task_mini_vlcs.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/tasks/task_mnist_color.py` & `domainlab-0.6.3/domainlab/tasks/task_mnist_color.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/tasks/task_pathlist.py` & `domainlab-0.6.3/domainlab/tasks/task_pathlist.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/tasks/task_utils.py` & `domainlab-0.6.3/domainlab/tasks/task_utils.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/tasks/utils_task.py` & `domainlab-0.6.3/domainlab/tasks/utils_task.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/tasks/utils_task_dset.py` & `domainlab-0.6.3/domainlab/tasks/utils_task_dset.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/tasks/zoo_tasks.py` & `domainlab-0.6.3/domainlab/tasks/zoo_tasks.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/utils/flows_gen_img_model.py` & `domainlab-0.6.3/domainlab/utils/flows_gen_img_model.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/utils/generate_benchmark_plots.py` & `domainlab-0.6.3/domainlab/utils/generate_benchmark_plots.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/utils/get_git_tag.py` & `domainlab-0.6.3/domainlab/utils/get_git_tag.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/utils/hyperparameter_gridsearch.py` & `domainlab-0.6.3/domainlab/utils/hyperparameter_gridsearch.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/utils/hyperparameter_sampling.py` & `domainlab-0.6.3/domainlab/utils/hyperparameter_sampling.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/utils/logger.py` & `domainlab-0.6.3/domainlab/utils/logger.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/utils/override_interface.py` & `domainlab-0.6.3/domainlab/utils/override_interface.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/utils/perf.py` & `domainlab-0.6.3/domainlab/utils/perf.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/utils/perf_metrics.py` & `domainlab-0.6.3/domainlab/utils/perf_metrics.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/utils/sanity_check.py` & `domainlab-0.6.3/domainlab/utils/sanity_check.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/utils/test_img.py` & `domainlab-0.6.3/domainlab/utils/test_img.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/utils/u_import_net_module.py` & `domainlab-0.6.3/domainlab/utils/u_import_net_module.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/utils/utils_class.py` & `domainlab-0.6.3/domainlab/utils/utils_class.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/utils/utils_classif.py` & `domainlab-0.6.3/domainlab/utils/utils_classif.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/utils/utils_cuda.py` & `domainlab-0.6.3/domainlab/utils/utils_cuda.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/utils/utils_img_sav.py` & `domainlab-0.6.3/domainlab/utils/utils_img_sav.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/mixed_codec/caltech/auto/train_imgs_150.jpg` & `domainlab-0.6.3/domainlab/zdata/mixed_codec/caltech/auto/train_imgs_150.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/mixed_codec/caltech/auto/train_imgs_151.jpg` & `domainlab-0.6.3/domainlab/zdata/mixed_codec/caltech/auto/train_imgs_151.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/mixed_codec/caltech/auto/train_imgs_152.png` & `domainlab-0.6.3/domainlab/zdata/mixed_codec/caltech/auto/train_imgs_152.png`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/mixed_codec/caltech/vogel/train_imgs_1.jpg` & `domainlab-0.6.3/domainlab/zdata/mixed_codec/caltech/vogel/train_imgs_1.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/mixed_codec/caltech/vogel/train_imgs_2.jpg` & `domainlab-0.6.3/domainlab/zdata/mixed_codec/caltech/vogel/train_imgs_2.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/mixed_codec/caltech/vogel/train_imgs_3.png` & `domainlab-0.6.3/domainlab/zdata/mixed_codec/caltech/vogel/train_imgs_3.png`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/mixed_codec/sun/sofa/train_imgs_609.jpg` & `domainlab-0.6.3/domainlab/zdata/mixed_codec/sun/sofa/train_imgs_609.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/mixed_codec/sun/sofa/train_imgs_612.jpg` & `domainlab-0.6.3/domainlab/zdata/mixed_codec/sun/sofa/train_imgs_612.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/mixed_codec/sun/vehicle/train_imgs_17.jpg` & `domainlab-0.6.3/domainlab/zdata/mixed_codec/sun/vehicle/train_imgs_17.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/mixed_codec/sun/vehicle/train_imgs_19.jpg` & `domainlab-0.6.3/domainlab/zdata/mixed_codec/sun/vehicle/train_imgs_19.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_mini_10/art_painting/dog/pic_195.jpg` & `domainlab-0.6.3/domainlab/zdata/pacs_mini_10/art_painting/dog/pic_195.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_mini_10/art_painting/dog/pic_304.jpg` & `domainlab-0.6.3/domainlab/zdata/pacs_mini_10/art_painting/dog/pic_304.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_mini_10/art_painting/elephant/pic_026.jpg` & `domainlab-0.6.3/domainlab/zdata/pacs_mini_10/art_painting/elephant/pic_026.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_mini_10/art_painting/giraffe/pic_243.jpg` & `domainlab-0.6.3/domainlab/zdata/pacs_mini_10/art_painting/giraffe/pic_243.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_mini_10/art_painting/guitar/pic_020.jpg` & `domainlab-0.6.3/domainlab/zdata/pacs_mini_10/art_painting/guitar/pic_020.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_mini_10/art_painting/guitar/pic_182.jpg` & `domainlab-0.6.3/domainlab/zdata/pacs_mini_10/art_painting/guitar/pic_182.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_mini_10/art_painting/horse/pic_142.jpg` & `domainlab-0.6.3/domainlab/zdata/pacs_mini_10/art_painting/horse/pic_142.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_mini_10/art_painting/person/pic_165.jpg` & `domainlab-0.6.3/domainlab/zdata/pacs_mini_10/art_painting/person/pic_165.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_mini_10/art_painting/person/pic_199.jpg` & `domainlab-0.6.3/domainlab/zdata/pacs_mini_10/art_painting/person/pic_199.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_mini_10/art_painting/person/pic_497.jpg` & `domainlab-0.6.3/domainlab/zdata/pacs_mini_10/art_painting/person/pic_497.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_mini_10/cartoon/dog/pic_112.jpg` & `domainlab-0.6.3/domainlab/zdata/pacs_mini_10/cartoon/dog/pic_112.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_mini_10/cartoon/dog/pic_137.jpg` & `domainlab-0.6.3/domainlab/zdata/pacs_mini_10/cartoon/dog/pic_137.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_mini_10/cartoon/dog/pic_219.jpg` & `domainlab-0.6.3/domainlab/zdata/pacs_mini_10/cartoon/dog/pic_219.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_mini_10/cartoon/elephant/pic_332.jpg` & `domainlab-0.6.3/domainlab/zdata/pacs_mini_10/cartoon/elephant/pic_332.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_mini_10/cartoon/giraffe/pic_377.jpg` & `domainlab-0.6.3/domainlab/zdata/pacs_mini_10/cartoon/giraffe/pic_377.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_mini_10/cartoon/giraffe/pic_382.jpg` & `domainlab-0.6.3/domainlab/zdata/pacs_mini_10/cartoon/giraffe/pic_382.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_mini_10/cartoon/horse/pic_064.jpg` & `domainlab-0.6.3/domainlab/zdata/pacs_mini_10/cartoon/horse/pic_064.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_mini_10/cartoon/house/pic_040.jpg` & `domainlab-0.6.3/domainlab/zdata/pacs_mini_10/cartoon/house/pic_040.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_mini_10/cartoon/person/pic_111.jpg` & `domainlab-0.6.3/domainlab/zdata/pacs_mini_10/cartoon/person/pic_111.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_mini_10/cartoon/person/pic_180.jpg` & `domainlab-0.6.3/domainlab/zdata/pacs_mini_10/cartoon/person/pic_180.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_mini_10/photo/dog/n02103406_1011.jpg` & `domainlab-0.6.3/domainlab/zdata/pacs_mini_10/photo/dog/n02103406_1011.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_mini_10/photo/elephant/n02503517_6232.jpg` & `domainlab-0.6.3/domainlab/zdata/pacs_mini_10/photo/elephant/n02503517_6232.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_mini_10/photo/guitar/n02676566_7830.jpg` & `domainlab-0.6.3/domainlab/zdata/pacs_mini_10/photo/guitar/n02676566_7830.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_mini_10/photo/horse/105_0223.jpg` & `domainlab-0.6.3/domainlab/zdata/pacs_mini_10/photo/horse/105_0223.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_mini_10/photo/house/pic_046.jpg` & `domainlab-0.6.3/domainlab/zdata/pacs_mini_10/photo/house/pic_046.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_mini_10/photo/house/pic_110.jpg` & `domainlab-0.6.3/domainlab/zdata/pacs_mini_10/photo/house/pic_110.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_mini_10/photo/house/pic_146.jpg` & `domainlab-0.6.3/domainlab/zdata/pacs_mini_10/photo/house/pic_146.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_mini_10/photo/house/pic_218.jpg` & `domainlab-0.6.3/domainlab/zdata/pacs_mini_10/photo/house/pic_218.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_mini_10/photo/person/253_0221.jpg` & `domainlab-0.6.3/domainlab/zdata/pacs_mini_10/photo/person/253_0221.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_mini_10/photo/person/253_0297.jpg` & `domainlab-0.6.3/domainlab/zdata/pacs_mini_10/photo/person/253_0297.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_mini_10/run_with_bash_copy_files_according2txt.sh` & `domainlab-0.6.3/domainlab/zdata/pacs_mini_10/run_with_bash_copy_files_according2txt.sh`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_mini_10/sketch/dog/5302.png` & `domainlab-0.6.3/domainlab/zdata/pacs_mini_10/sketch/dog/5302.png`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_mini_10/sketch/dog/5317.png` & `domainlab-0.6.3/domainlab/zdata/pacs_mini_10/sketch/dog/5317.png`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_mini_10/sketch/dog/n02103406_3255-6.png` & `domainlab-0.6.3/domainlab/zdata/pacs_mini_10/sketch/dog/n02103406_3255-6.png`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_mini_10/sketch/elephant/5981.png` & `domainlab-0.6.3/domainlab/zdata/pacs_mini_10/sketch/elephant/5981.png`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_mini_10/sketch/elephant/n02503517_12688-4.png` & `domainlab-0.6.3/domainlab/zdata/pacs_mini_10/sketch/elephant/n02503517_12688-4.png`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_mini_10/sketch/giraffe/n02439033_13384-2.png` & `domainlab-0.6.3/domainlab/zdata/pacs_mini_10/sketch/giraffe/n02439033_13384-2.png`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_mini_10/sketch/guitar/n02676566_8618-2.png` & `domainlab-0.6.3/domainlab/zdata/pacs_mini_10/sketch/guitar/n02676566_8618-2.png`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_mini_10/sketch/guitar/n03467517_6423-3.png` & `domainlab-0.6.3/domainlab/zdata/pacs_mini_10/sketch/guitar/n03467517_6423-3.png`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_mini_10/sketch/horse/n02374451_779-1.png` & `domainlab-0.6.3/domainlab/zdata/pacs_mini_10/sketch/horse/n02374451_779-1.png`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_mini_10/sketch/house/8873.png` & `domainlab-0.6.3/domainlab/zdata/pacs_mini_10/sketch/house/8873.png`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_split/art_painting_100.txt` & `domainlab-0.6.3/domainlab/zdata/pacs_split/art_painting_100.txt`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_split/art_painting_crossval_kfold.txt` & `domainlab-0.6.3/domainlab/zdata/pacs_split/art_painting_crossval_kfold.txt`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_split/art_painting_test_kfold.txt` & `domainlab-0.6.3/domainlab/zdata/pacs_split/art_painting_test_kfold.txt`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_split/art_painting_train_kfold.txt` & `domainlab-0.6.3/domainlab/zdata/pacs_split/art_painting_train_kfold.txt`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_split/cartoon_100.txt` & `domainlab-0.6.3/domainlab/zdata/pacs_split/cartoon_100.txt`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_split/cartoon_crossval_kfold.txt` & `domainlab-0.6.3/domainlab/zdata/pacs_split/cartoon_crossval_kfold.txt`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_split/cartoon_test_kfold.txt` & `domainlab-0.6.3/domainlab/zdata/pacs_split/cartoon_test_kfold.txt`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_split/cartoon_train_kfold.txt` & `domainlab-0.6.3/domainlab/zdata/pacs_split/cartoon_train_kfold.txt`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_split/photo_100.txt` & `domainlab-0.6.3/domainlab/zdata/pacs_split/photo_100.txt`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_split/photo_crossval_kfold.txt` & `domainlab-0.6.3/domainlab/zdata/pacs_split/photo_crossval_kfold.txt`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_split/photo_test_kfold.txt` & `domainlab-0.6.3/domainlab/zdata/pacs_split/photo_test_kfold.txt`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_split/photo_train_kfold.txt` & `domainlab-0.6.3/domainlab/zdata/pacs_split/photo_train_kfold.txt`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_split/readme.txt` & `domainlab-0.6.3/domainlab/zdata/pacs_split/readme.txt`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_split/sketch_100.txt` & `domainlab-0.6.3/domainlab/zdata/pacs_split/sketch_100.txt`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_split/sketch_crossval_kfold.txt` & `domainlab-0.6.3/domainlab/zdata/pacs_split/sketch_crossval_kfold.txt`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_split/sketch_test_kfold.txt` & `domainlab-0.6.3/domainlab/zdata/pacs_split/sketch_test_kfold.txt`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/pacs_split/sketch_train_kfold.txt` & `domainlab-0.6.3/domainlab/zdata/pacs_split/sketch_train_kfold.txt`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/patches_permutation4jigsaw/permutations_100.npy` & `domainlab-0.6.3/domainlab/zdata/patches_permutation4jigsaw/permutations_100.npy`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/patches_permutation4jigsaw/permutations_30.npy` & `domainlab-0.6.3/domainlab/zdata/patches_permutation4jigsaw/permutations_30.npy`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/patches_permutation4jigsaw/permutations_31.npy` & `domainlab-0.6.3/domainlab/zdata/patches_permutation4jigsaw/permutations_31.npy`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/script/download_pacs.py` & `domainlab-0.6.3/domainlab/zdata/script/download_pacs.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_150.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_150.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_151.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_151.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_152.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_152.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_153.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_153.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_154.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_154.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_155.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_155.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_156.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_156.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_157.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_157.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_158.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_158.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_159.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_159.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_160.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_160.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_161.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_161.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_162.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_162.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_163.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_163.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_164.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_164.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_165.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_165.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_166.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_166.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_167.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_167.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_168.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_168.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_169.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/auto/train_imgs_169.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/hund/train_imgs_302.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/hund/train_imgs_302.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/hund/train_imgs_303.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/hund/train_imgs_303.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/hund/train_imgs_304.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/hund/train_imgs_304.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/hund/train_imgs_305.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/hund/train_imgs_305.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/hund/train_imgs_306.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/hund/train_imgs_306.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/hund/train_imgs_307.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/hund/train_imgs_307.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/hund/train_imgs_308.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/hund/train_imgs_308.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/hund/train_imgs_309.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/hund/train_imgs_309.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/hund/train_imgs_310.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/hund/train_imgs_310.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/hund/train_imgs_311.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/hund/train_imgs_311.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/hund/train_imgs_312.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/hund/train_imgs_312.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/mensch/train_imgs_344.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/mensch/train_imgs_344.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/mensch/train_imgs_345.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/mensch/train_imgs_345.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/mensch/train_imgs_346.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/mensch/train_imgs_346.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/mensch/train_imgs_347.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/mensch/train_imgs_347.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/mensch/train_imgs_348.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/mensch/train_imgs_348.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/mensch/train_imgs_349.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/mensch/train_imgs_349.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/mensch/train_imgs_350.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/mensch/train_imgs_350.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/mensch/train_imgs_351.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/mensch/train_imgs_351.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/mensch/train_imgs_352.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/mensch/train_imgs_352.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/stuhl/train_imgs_227.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/stuhl/train_imgs_227.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/stuhl/train_imgs_228.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/stuhl/train_imgs_228.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/stuhl/train_imgs_229.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/stuhl/train_imgs_229.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/stuhl/train_imgs_230.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/stuhl/train_imgs_230.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/stuhl/train_imgs_231.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/stuhl/train_imgs_231.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/stuhl/train_imgs_232.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/stuhl/train_imgs_232.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/vogel/train_imgs_1.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/vogel/train_imgs_1.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/vogel/train_imgs_2.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/vogel/train_imgs_2.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/vogel/train_imgs_3.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/vogel/train_imgs_3.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/vogel/train_imgs_4.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/vogel/train_imgs_4.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/vogel/train_imgs_5.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/vogel/train_imgs_5.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/vogel/train_imgs_6.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/vogel/train_imgs_6.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/vogel/train_imgs_7.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/vogel/train_imgs_7.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/vogel/train_imgs_8.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/vogel/train_imgs_8.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/caltech/vogel/train_imgs_9.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/caltech/vogel/train_imgs_9.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_1.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_1.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_10.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_10.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_11.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_11.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_12.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_12.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_13.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_13.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_14.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_14.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_15.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_15.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_16.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_16.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_17.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_17.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_18.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_18.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_19.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_19.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_2.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_2.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_20.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_20.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_21.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_21.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_22.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_22.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_23.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_23.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_24.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_24.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_25.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_25.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_26.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_26.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_27.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_27.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_28.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_28.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_29.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_29.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_3.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_3.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_30.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_30.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_31.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_31.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_32.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_32.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_33.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_33.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_34.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_34.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_35.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_35.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_36.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_36.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_37.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_37.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_38.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_38.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_39.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_39.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_4.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_4.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_40.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_40.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_41.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_41.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_42.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_42.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_43.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_43.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_44.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_44.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_45.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_45.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_46.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_46.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_47.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_47.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_48.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_48.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_49.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_49.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_5.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_5.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_50.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_50.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_6.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_6.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_7.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_7.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_8.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_8.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_9.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/bird/train_imgs_9.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_51.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_51.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_52.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_52.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_54.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_54.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_55.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_55.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_56.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_56.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_57.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_57.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_58.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_58.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_59.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_59.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_60.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_60.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_61.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_61.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_64.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_64.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_65.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_65.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_69.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_69.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_70.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/drive/train_imgs_70.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/husky/train_imgs_870.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/husky/train_imgs_870.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/husky/train_imgs_871.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/husky/train_imgs_871.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/husky/train_imgs_880.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/husky/train_imgs_880.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/husky/train_imgs_883.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/husky/train_imgs_883.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/husky/train_imgs_886.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/husky/train_imgs_886.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/husky/train_imgs_891.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/husky/train_imgs_891.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/sit/train_imgs_818.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/sit/train_imgs_818.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/sit/train_imgs_824.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/sit/train_imgs_824.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/sit/train_imgs_830.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/sit/train_imgs_830.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/sit/train_imgs_836.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/sit/train_imgs_836.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/sit/train_imgs_837.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/sit/train_imgs_837.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/sit/train_imgs_849.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/sit/train_imgs_849.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/labelme/sit/train_imgs_858.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/labelme/sit/train_imgs_858.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1253.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1253.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1254.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1254.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1255.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1255.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1256.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1256.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1257.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1257.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1258.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1258.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1259.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1259.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1260.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1260.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1261.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1261.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1262.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1262.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1263.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1263.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1264.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1264.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1265.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1265.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1266.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1266.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1267.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1267.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1268.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1268.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1269.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1269.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1270.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1270.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1271.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/dog/train_imgs_1271.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/flying/train_imgs_1.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/flying/train_imgs_1.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/flying/train_imgs_10.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/flying/train_imgs_10.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/flying/train_imgs_11.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/flying/train_imgs_11.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/flying/train_imgs_13.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/flying/train_imgs_13.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/flying/train_imgs_2.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/flying/train_imgs_2.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/flying/train_imgs_3.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/flying/train_imgs_3.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/flying/train_imgs_5.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/flying/train_imgs_5.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/flying/train_imgs_7.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/flying/train_imgs_7.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_1272.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_1272.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_1273.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_1273.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_1274.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_1274.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_1275.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_1275.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_1276.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_1276.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_1277.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_1277.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_1278.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_1278.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_1279.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_1279.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_1280.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_1280.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_1281.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_1281.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_1282.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_1282.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_1428.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_1428.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_2065.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_2065.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_2066.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_2066.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_2067.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/sapiens/train_imgs_2067.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/sofa/train_imgs_609.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/sofa/train_imgs_609.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/sofa/train_imgs_612.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/sofa/train_imgs_612.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/sofa/train_imgs_614.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/sofa/train_imgs_614.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/sofa/train_imgs_620.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/sofa/train_imgs_620.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/vehicle/train_imgs_17.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/vehicle/train_imgs_17.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/vehicle/train_imgs_19.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/vehicle/train_imgs_19.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/vehicle/train_imgs_21.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/vehicle/train_imgs_21.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/vehicle/train_imgs_22.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/vehicle/train_imgs_22.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/vehicle/train_imgs_23.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/vehicle/train_imgs_23.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/vehicle/train_imgs_24.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/vehicle/train_imgs_24.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/vehicle/train_imgs_25.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/vehicle/train_imgs_25.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/vehicle/train_imgs_26.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/vehicle/train_imgs_26.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/vlcs_mini/sun/vehicle/train_imgs_478.jpg` & `domainlab-0.6.3/domainlab/zdata/vlcs_mini/sun/vehicle/train_imgs_478.jpg`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/ztest_files/aggret_res_test11` & `domainlab-0.6.3/domainlab/zdata/ztest_files/aggret_res_test11`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/ztest_files/aggret_res_test2` & `domainlab-0.6.3/domainlab/zdata/ztest_files/aggret_res_test2`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/domainlab/zdata/ztest_files/aggret_res_test21` & `domainlab-0.6.3/domainlab/zdata/ztest_files/aggret_res_test21`

 * *Files identical despite different names*

### Comparing `domainlab-0.6.2/pyproject.toml` & `domainlab-0.6.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "domainlab"
-version = "0.6.2"
+version = "0.6.3"
 readme = "README.md"
 repository = "https://github.com/marrlab/DomainLab"
 homepage = "https://marrlab.github.io/DomainLab/"
 description = "Library of modular domain generalization for deep learning"
-authors = ["Xudong Sun <smilesun.east@gmail.com>", "Carla Feistner", "Alexej Gossmann <alexej.gossmann@fda.hhs.gov>", "Georg Schwarz", "et. al."]
+authors = ["Xudong Sun <smilesun.east@gmail.com>", "Carla Feistner", "Alexej Gossmann <alexej.gossmann@fda.hhs.gov>", "et. al."]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 numpy = "^1.23.4"
 matplotlib = "^3.6.1"
 seaborn = "0.12.2"
 torchmetrics = "^0.10.0"
```

### Comparing `domainlab-0.6.2/setup.py` & `domainlab-0.6.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,17 +86,17 @@
  'torchvision>=0.13.0,<0.14.0']
 
 entry_points = \
 {'console_scripts': ['domainlab = domainlab.cli:domainlab_cli']}
 
 setup_kwargs = {
     'name': 'domainlab',
-    'version': '0.6.2',
+    'version': '0.6.3',
     'description': 'Library of modular domain generalization for deep learning',
-    'long_description': '# DomainLab: modular python package for training domain invariant neural networks\n\n![GH Actions CI ](https://github.com/marrlab/DomainLab/actions/workflows/ci.yml/badge.svg?branch=master)\n[![codecov](https://codecov.io/gh/marrlab/DomainLab/branch/master/graph/badge.svg)](https://app.codecov.io/gh/marrlab/DomainLab)\n[![Codacy Badge](https://app.codacy.com/project/badge/Grade/bc22a1f9afb742efb02b87284e04dc86)](https://www.codacy.com/gh/marrlab/DomainLab/dashboard)\n[![Documentation](https://img.shields.io/badge/Documentation-Here)](https://marrlab.github.io/DomainLab/)\n[![pages-build-deployment](https://github.com/marrlab/DomainLab/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/marrlab/DomainLab/actions/workflows/pages/pages-build-deployment)\n\n## Distribution shifts, domain generalization and DomainLab\n\nNeural networks trained using data from a specific distribution (domain) usually fails to generalize to novel distributions (domains). Domain generalization aims at learning domain invariant features by utilizing data from multiple domains (data sites, corhorts, batches, vendors) so the learned feature can generalize to new unseen domains (distributions).\n\nDomainLab is a software platform with state-of-the-art domain generalization algorithms implemented, designed by maximal decoupling of different software components thus enhances maximal code reuse.\n\n### DomainLab\nDomainLab decouples the following concepts or objects:\n- task $M$: In DomainLab, a task is a container for datasets from different domains. (e.g. from distribution $D_1$ and $D_2$). Task offer a static protocol to evaluate the generalization performance of a neural network: which dataset(s) is used for training, wich dataset(s) used for testing.  \n- neural network: a map $\\phi$ from the input data to the feature space and a map $\\varphi$ from feature space to output $\\hat{y}$ (e.g. decision variable).\n- model: structural risk in the form of $\\ell() + \\mu R()$  where\n  - $\\ell(Y, \\hat{y}=\\varphi(\\phi(X)))$ is the task specific empirical loss (e.g. cross entropy for classification task).\n  - $R(\\phi(X))$ is the penalty loss to boost domain invariant feature extraction using $\\phi$.\n  - $\\mu$ is the corresponding multiplier to each penalty function factor.\n- trainer:  an object that guides the data flow to model and append further domain invariant losses\nlike inter-domain feature alignment.\n\nWe offer detailed documentation on how these models and trainers work in our documentation page: https://marrlab.github.io/DomainLab/\n\nDomainLab makes it possible to combine models with models, trainers with models, and trainers with trainers in a decorator pattern like line of code `Trainer A(Trainer B(Model C(Model D(network E), network E, network F)))` which correspond to $\\ell() + \\mu_a R_a() + \\mu_b R_b + \\mu_c R_c() + \\mu_d R_d()$, where Model C and Model D share neural network E, but Model C has an extra neural network F. All models share the same neural network for feature extraction, but can have different auxilliary networks for $R()$.\n\n<div style="align: center; text-align:center;">\n<figure>  \n<img src="https://github.com/marrlab/DomainLab/blob/master/docs/figs/invarfeat4dg.png?raw=true" style="width:300px;"/> \n</figure>\n</div>\n\n## Getting started\n\n### Installation\nFor development version in Github, see [Installation and Dependencies handling](./docs/doc_install.md)\n\nWe also offer a PyPI version here https://pypi.org/project/domainlab/  which one could install via `pip install domainlab` and it is recommended to create a virtual environment for it.\n\n### Task specification\nWe offer various ways for the user to specify a scenario to evaluate the generalization performance via training on a limited number of datasets. See detail in\n[Task Specification](./docs/doc_tasks.md) \n\n### Example and usage\n#### Available arguments for commandline\n\nThe following command tells which arguments/hyperparameters/multipliers are available to be set by the user and which model they are associated with\n\n```shell\npython main_out.py --help\n```\n\nor \n\n```shell\ndomainlab --help\n```\n\n#### Command line configuration file\n\n`domainlab -c ./examples/conf/vlcs_diva_mldg_dial.yaml` (if you install via pip)\n\nor if you clone this the code repository for DomainLab\n\n`python main_out.py -c ./examples/conf/vlcs_diva_mldg_dial.yaml`\n\nwhere the configuration file below can be downloaded [here](https://raw.githubusercontent.com/marrlab/DomainLab/master/examples/conf/vlcs_diva_mldg_dial.yaml)\n```\nte_d: caltech                       # domain name of test domain\ntpath: examples/tasks/task_vlcs.py  # python file path to specify the task\nbs: 2                               # batch size\nmodel: dann_diva                    # combine model DANN with DIVA\nepos: 1                             # number of epochs\ntrainer: mldg_dial                  # combine trainer MLDG and DIAL\ngamma_y: 700000.0                   # hyperparameter of diva\ngamma_d: 100000.0                   # hyperparameter of diva\nnpath: examples/nets/resnet.py      # neural network for class classification\nnpath_dom: examples/nets/resnet.py  # neural network for domain classification\n```\nSee details in [Command line usage](./docs/doc_usage_cmd.md)\n\n#### or Programm against DomainLab API\n\nSee example here: [Transformer as feature extractor, decorate JIGEN with DANN, training using MLDG decorated by DIAL](https://github.com/marrlab/DomainLab/blob/master/examples/api/jigen_dann_transformer.py)\n\n\n### Benchmark different methods\nDomainLab provides a powerful benchmark functionality.\nTo benchmark several algorithms(combination of neural networks, models, trainers and associated hyperparameters), a single line command along with a benchmark configuration files is sufficient. See details in [benchmarks documentation and tutorial](./docs/doc_benchmark.md)\n\nOne could simply run\n`bash run_benchmark_slurm.sh your_benchmark_configuration.yaml` to launch different experiments with specified configuraiton.\n\n\nFor example,  the following result (without any augmentation like flip) is for PACS dataset using ResNet. The reader should note that using different neural network, whether pre-trained or not, what kind of preprocessinga and augmentation to use can lead to very different result distributions, which is one of the features DomainLab provide: the above factors get decoupled in DomainLab. \n\n<div style="align: center; text-align:center;">\n<figure>  \n<img src="https://github.com/marrlab/DomainLab/blob/master/docs/figs/stochastic_variation_two_rows.png?raw=true" style="width:800px;"/>\n<div class="caption" style="align: center; text-align:center;">\n<figcaption>Benchmark results plot generated from DomainLab, where each rectangle represent one model trainer combination, each bar inside the rectangle represent a unique hyperparameter index associated with that method combination, each dot represent a random seeds.</figcaption>\n</div>\n</figure>\n</div>\n\n\n### Citation\n\nSource: https://arxiv.org/pdf/2403.14356.pdf\n\n```bibtex\n@misc{sun2024domainlab,\n  title={DomainLab: A modular Python package for domain generalization in deep learning},\n  author={Sun, Xudong and Feistner, Carla and Gossmann, Alexej and Schwarz, George and Umer, Rao Muhammad and Beer, Lisa and Rockenschaub, Patrick and Shrestha, Rahul Babu and Gruber, Armin and Chen, Nutan and others},\n  journal={https://arxiv.org/pdf/2403.14356.pdf},\n  year={2024}\n}\n```\n',
+    'long_description': '# DomainLab: modular python package for training domain invariant neural networks\n\n![GH Actions CI ](https://github.com/marrlab/DomainLab/actions/workflows/ci.yml/badge.svg?branch=master)\n[![codecov](https://codecov.io/gh/marrlab/DomainLab/branch/master/graph/badge.svg)](https://app.codecov.io/gh/marrlab/DomainLab)\n[![Codacy Badge](https://app.codacy.com/project/badge/Grade/bc22a1f9afb742efb02b87284e04dc86)](https://www.codacy.com/gh/marrlab/DomainLab/dashboard)\n[![Documentation](https://img.shields.io/badge/Documentation-Here)](https://marrlab.github.io/DomainLab/)\n[![pages-build-deployment](https://github.com/marrlab/DomainLab/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/marrlab/DomainLab/actions/workflows/pages/pages-build-deployment)\n\n## Distribution shifts, domain generalization and DomainLab\n\nNeural networks trained using data from a specific distribution (domain) usually fail to generalize to novel distributions (domains). Domain generalization aims at learning domain invariant features by utilizing data from multiple domains (data sites, cohorts, batches, vendors) so the learned feature can be generalized to new unseen domains (distributions).\n\nDomainLab is a software platform with state-of-the-art domain generalization algorithms implemented and designed by maximal decoupling of different software components thus enhancing maximal code reuse.\n\n### DomainLab\nDomainLab decouples the following concepts or objects:\n- task $M$: In DomainLab, a task is a container for datasets from different domains. (e.g. from distribution $D_1$ and $D_2$). The task offers a static protocol to evaluate the generalization performance of a neural network: which dataset(s) is used for training, and which dataset(s) is used for testing.  \n- neural network: a map $\\phi$ from the input data to the feature space and a map $\\varphi$ from the feature space to output $\\hat{y}$ (e.g. decision variable).\n- model: structural risk in the form of $\\ell() + \\mu R()$  where\n  - $\\ell(Y, \\hat{y}=\\varphi(\\phi(X)))$ is the task-specific empirical loss (e.g. cross entropy for classification task).\n  - $R(\\phi(X))$ is the penalty loss to boost domain invariant feature extraction using $\\phi$.\n  - $\\mu$ is the corresponding multiplier to each penalty function factor.\n- trainer:  an object that guides the data flow to model and append further domain invariant losses\nlike inter-domain feature alignment.\n\nWe offer detailed documentation on how these models and trainers work on our documentation page: https://marrlab.github.io/DomainLab/\n\nDomainLab makes it possible to combine models with models, trainers with models, and trainers with trainers in a decorator pattern like the line of code below\n\n```\nTrainer A(\n\t\t  Trainer B(Model C(\n\t\t\t\t\t\t    Model D(network E),\n\t\t\t\t\t\t\tnetwork E,\n\t\t\t\t\t\t\tnetwork F\n\t\t\t\t\t\t   )\n\t\t\t\t   )\n\t     )\n```\n\nwhich correspond to $\\ell() + \\mu_a R_a() + \\mu_b R_b + \\mu_c R_c() + \\mu_d R_d()$, where Model C and Model D share neural network E, but Model C has an extra neural network F. All models share the same neural network for feature extraction, but can have different auxiliary networks for $R()$.\n\n<div style="align: center; text-align:center;">\n<figure>  \n<img src="https://github.com/marrlab/DomainLab/blob/master/docs/figs/invarfeat4dg.png?raw=true" style="width:300px;"/> \n</figure>\n</div>\n\n## Getting started\n\n### Installation\nFor the development version in Github, see [Installation and Dependencies handling](./docs/doc_install.md)\n\nWe also offer a PyPI version here https://pypi.org/project/domainlab/  which one could install via `pip install domainlab` and it is recommended to create a virtual environment for it.\n\n### Task specification\nWe offer various ways for the user to specify a scenario to evaluate the generalization performance via training on a limited number of datasets. See detail in\n[Task Specification](./docs/doc_tasks.md) \n\n### Example and usage\n#### Available arguments for commandline\n\nThe following command tells which arguments/hyperparameters/multipliers are available to be set by the user and which model they are associated with\n\n```shell\npython main_out.py --help\n```\n\nor \n\n```\ndomainlab --help\n```\n\n#### Command line configuration file\n\n`domainlab -c ./examples/conf/vlcs_diva_mldg_dial.yaml` (if you install via pip)\n\nor if you clone this the code repository for DomainLab\n\n`python main_out.py -c ./examples/conf/vlcs_diva_mldg_dial.yaml`\n\nwhere the configuration file below can be downloaded [here](https://raw.githubusercontent.com/marrlab/DomainLab/master/examples/conf/vlcs_diva_mldg_dial.yaml)\n```\nte_d: caltech                       # domain name of test domain\ntpath: examples/tasks/task_vlcs.py  # python file path to specify the task\nbs: 2                               # batch size\nmodel: dann_diva                    # combine model DANN with DIVA\nepos: 1                             # number of epochs\ntrainer: mldg_dial                  # combine trainer MLDG and DIAL\ngamma_y: 700000.0                   # hyperparameter of diva\ngamma_d: 100000.0                   # hyperparameter of diva\nnpath: examples/nets/resnet.py      # neural network for class classification\nnpath_dom: examples/nets/resnet.py  # neural network for domain classification\n```\nSee details in [Command line usage](./docs/doc_usage_cmd.md)\n\n#### or Programm against DomainLab API\n\nSee example here: [Transformer as feature extractor, decorate JIGEN with DANN, training using MLDG decorated by DIAL](https://github.com/marrlab/DomainLab/blob/master/examples/api/jigen_dann_transformer.py)\n\n\n### Benchmark different methods\nDomainLab provides a powerful benchmark functionality.\nTo benchmark several algorithms(combination of neural networks, models, trainers and associated hyperparameters), a single line command along with a benchmark configuration files is sufficient. See details in [benchmarks documentation and tutorial](./docs/doc_benchmark.md)\n\nOne could simply run\n`bash run_benchmark_slurm.sh your_benchmark_configuration.yaml` to launch different experiments with specified configuraiton.\n\n\nFor example,  the following result (without any augmentation like flip) is for PACS dataset using ResNet. The reader should note that using different neural network, whether pre-trained or not, what kind of preprocessinga and augmentation to use can lead to very different result distributions, which is one of the features DomainLab provide: the above factors get decoupled in DomainLab. \n\n<div style="align: center; text-align:center;">\n<figure>  \n<img src="https://github.com/marrlab/DomainLab/blob/master/docs/figs/stochastic_variation_two_rows.png?raw=true" style="width:800px;"/>\n<div class="caption" style="align: center; text-align:center;">\n<figcaption>Benchmark results plot generated from DomainLab, where each rectangle represent one model trainer combination, each bar inside the rectangle represent a unique hyperparameter index associated with that method combination, each dot represent a random seeds.</figcaption>\n</div>\n</figure>\n</div>\n\n\n### Citation\n\nSource: https://arxiv.org/pdf/2403.14356.pdf\n\n```bibtex\n@misc{sun2024domainlab,\n  title={DomainLab: A modular Python package for domain generalization in deep learning},\n  author={Sun, Xudong and Feistner, Carla and Gossmann, Alexej and Schwarz, George and Umer, Rao Muhammad and Beer, Lisa and Rockenschaub, Patrick and Shrestha, Rahul Babu and Gruber, Armin and Chen, Nutan and others},\n  journal={https://arxiv.org/pdf/2403.14356.pdf},\n  year={2024}\n}\n```\n',
     'author': 'Xudong Sun',
     'author_email': 'smilesun.east@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://marrlab.github.io/DomainLab/',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `domainlab-0.6.2/PKG-INFO` & `domainlab-0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domainlab
-Version: 0.6.2
+Version: 0.6.3
 Summary: Library of modular domain generalization for deep learning
 Home-page: https://marrlab.github.io/DomainLab/
 Author: Xudong Sun
 Author-email: smilesun.east@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -31,43 +31,56 @@
 [![codecov](https://codecov.io/gh/marrlab/DomainLab/branch/master/graph/badge.svg)](https://app.codecov.io/gh/marrlab/DomainLab)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/bc22a1f9afb742efb02b87284e04dc86)](https://www.codacy.com/gh/marrlab/DomainLab/dashboard)
 [![Documentation](https://img.shields.io/badge/Documentation-Here)](https://marrlab.github.io/DomainLab/)
 [![pages-build-deployment](https://github.com/marrlab/DomainLab/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/marrlab/DomainLab/actions/workflows/pages/pages-build-deployment)
 
 ## Distribution shifts, domain generalization and DomainLab
 
-Neural networks trained using data from a specific distribution (domain) usually fails to generalize to novel distributions (domains). Domain generalization aims at learning domain invariant features by utilizing data from multiple domains (data sites, corhorts, batches, vendors) so the learned feature can generalize to new unseen domains (distributions).
+Neural networks trained using data from a specific distribution (domain) usually fail to generalize to novel distributions (domains). Domain generalization aims at learning domain invariant features by utilizing data from multiple domains (data sites, cohorts, batches, vendors) so the learned feature can be generalized to new unseen domains (distributions).
 
-DomainLab is a software platform with state-of-the-art domain generalization algorithms implemented, designed by maximal decoupling of different software components thus enhances maximal code reuse.
+DomainLab is a software platform with state-of-the-art domain generalization algorithms implemented and designed by maximal decoupling of different software components thus enhancing maximal code reuse.
 
 ### DomainLab
 DomainLab decouples the following concepts or objects:
-- task $M$: In DomainLab, a task is a container for datasets from different domains. (e.g. from distribution $D_1$ and $D_2$). Task offer a static protocol to evaluate the generalization performance of a neural network: which dataset(s) is used for training, wich dataset(s) used for testing.  
-- neural network: a map $\phi$ from the input data to the feature space and a map $\varphi$ from feature space to output $\hat{y}$ (e.g. decision variable).
+- task $M$: In DomainLab, a task is a container for datasets from different domains. (e.g. from distribution $D_1$ and $D_2$). The task offers a static protocol to evaluate the generalization performance of a neural network: which dataset(s) is used for training, and which dataset(s) is used for testing.  
+- neural network: a map $\phi$ from the input data to the feature space and a map $\varphi$ from the feature space to output $\hat{y}$ (e.g. decision variable).
 - model: structural risk in the form of $\ell() + \mu R()$  where
-  - $\ell(Y, \hat{y}=\varphi(\phi(X)))$ is the task specific empirical loss (e.g. cross entropy for classification task).
+  - $\ell(Y, \hat{y}=\varphi(\phi(X)))$ is the task-specific empirical loss (e.g. cross entropy for classification task).
   - $R(\phi(X))$ is the penalty loss to boost domain invariant feature extraction using $\phi$.
   - $\mu$ is the corresponding multiplier to each penalty function factor.
 - trainer:  an object that guides the data flow to model and append further domain invariant losses
 like inter-domain feature alignment.
 
-We offer detailed documentation on how these models and trainers work in our documentation page: https://marrlab.github.io/DomainLab/
+We offer detailed documentation on how these models and trainers work on our documentation page: https://marrlab.github.io/DomainLab/
 
-DomainLab makes it possible to combine models with models, trainers with models, and trainers with trainers in a decorator pattern like line of code `Trainer A(Trainer B(Model C(Model D(network E), network E, network F)))` which correspond to $\ell() + \mu_a R_a() + \mu_b R_b + \mu_c R_c() + \mu_d R_d()$, where Model C and Model D share neural network E, but Model C has an extra neural network F. All models share the same neural network for feature extraction, but can have different auxilliary networks for $R()$.
+DomainLab makes it possible to combine models with models, trainers with models, and trainers with trainers in a decorator pattern like the line of code below
+
+```
+Trainer A(
+		  Trainer B(Model C(
+						    Model D(network E),
+							network E,
+							network F
+						   )
+				   )
+	     )
+```
+
+which correspond to $\ell() + \mu_a R_a() + \mu_b R_b + \mu_c R_c() + \mu_d R_d()$, where Model C and Model D share neural network E, but Model C has an extra neural network F. All models share the same neural network for feature extraction, but can have different auxiliary networks for $R()$.
 
 <div style="align: center; text-align:center;">
 <figure>  
 <img src="https://github.com/marrlab/DomainLab/blob/master/docs/figs/invarfeat4dg.png?raw=true" style="width:300px;"/> 
 </figure>
 </div>
 
 ## Getting started
 
 ### Installation
-For development version in Github, see [Installation and Dependencies handling](./docs/doc_install.md)
+For the development version in Github, see [Installation and Dependencies handling](./docs/doc_install.md)
 
 We also offer a PyPI version here https://pypi.org/project/domainlab/  which one could install via `pip install domainlab` and it is recommended to create a virtual environment for it.
 
 ### Task specification
 We offer various ways for the user to specify a scenario to evaluate the generalization performance via training on a limited number of datasets. See detail in
 [Task Specification](./docs/doc_tasks.md) 
 
@@ -78,15 +91,15 @@
 
 ```shell
 python main_out.py --help
 ```
 
 or 
 
-```shell
+```
 domainlab --help
 ```
 
 #### Command line configuration file
 
 `domainlab -c ./examples/conf/vlcs_diva_mldg_dial.yaml` (if you install via pip)
```

