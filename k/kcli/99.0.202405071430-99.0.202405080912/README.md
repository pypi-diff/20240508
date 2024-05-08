# Comparing `tmp/kcli-99.0.202405071430.tar.gz` & `tmp/kcli-99.0.202405080912.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kcli-99.0.202405071430.tar", last modified: Tue May  7 14:30:53 2024, max compression
+gzip compressed data, was "kcli-99.0.202405080912.tar", last modified: Wed May  8 09:12:13 2024, max compression
```

## Comparing `kcli-99.0.202405071430.tar` & `kcli-99.0.202405080912.tar`

### file list

```diff
@@ -1,788 +1,784 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.461548 kcli-99.0.202405071430/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-07 14:30:53.461548 kcli-99.0.202405071430/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.365548 kcli-99.0.202405071430/extras/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/extras/Dockerfile_curl
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/extras/Dockerfile_kubectl
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/extras/autoscale.yml
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/extras/aws_peering.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/extras/aws_peering_cleaning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.365548 kcli-99.0.202405071430/extras/controller/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/extras/controller/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/extras/controller/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/extras/controller/crd.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/extras/controller/deploy.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.365548 kcli-99.0.202405071430/extras/controller/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/extras/controller/examples/cluster_simple.yml
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/extras/controller/examples/plan_complex.yml
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/extras/controller/examples/plan_simple.yml
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/extras/controller/examples/plan_simple_with_file.yml
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/extras/controller/examples/vm_centos8stream.yml
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/extras/controller/examples/vm_cirros.yml
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/extras/controller/examples/vm_empty.yml
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/extras/controller/examples/vm_fedora.yml
--rw-r--r--   0 runner    (1001) docker     (127)     9970 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/extras/controller/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/extras/controller/stress_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/extras/debian
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.365548 kcli-99.0.202405071430/extras/expose/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/extras/expose/kcli.conf
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/extras/expose/kcli.wsgi
--rwxr-xr-x   0 runner    (1001) docker     (127)      106 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/extras/genrst.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/extras/haproxy.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/extras/haproxy_multiple_clusters.cfg
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/extras/i_am_a_container
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/extras/k8sdeploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/extras/kfish.md
--rw-r--r--   0 runner    (1001) docker     (127)    38837 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/extras/kfish.png
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/extras/missing_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/extras/openstack.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/extras/openstack.sh.sample
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/extras/zerotier.service
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.369548 kcli-99.0.202405071430/kcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-07 14:30:52.000000 kcli-99.0.202405071430/kcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    27395 2024-05-07 14:30:52.000000 kcli-99.0.202405071430/kcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 14:30:52.000000 kcli-99.0.202405071430/kcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-07 14:30:52.000000 kcli-99.0.202405071430/kcli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 14:29:15.000000 kcli-99.0.202405071430/kcli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-07 14:30:52.000000 kcli-99.0.202405071430/kcli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-07 14:30:52.000000 kcli-99.0.202405071430/kcli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.369548 kcli-99.0.202405071430/kvirt/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.369548 kcli-99.0.202405071430/kvirt/ansibleutils/
--rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/ansibleutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    98904 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/baseconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)   171487 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/bottle.py
--rw-r--r--   0 runner    (1001) docker     (127)   278792 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.369548 kcli-99.0.202405071430/kvirt/cluster/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.369548 kcli-99.0.202405071430/kvirt/cluster/aks/
--rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/aks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/aks/fake.yml
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/aks/kcli_default.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.373548 kcli-99.0.202405071430/kvirt/cluster/eks/
--rw-r--r--   0 runner    (1001) docker     (127)    12290 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/eks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/eks/fake.yml
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/eks/kcli_default.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.373548 kcli-99.0.202405071430/kvirt/cluster/gke/
--rw-r--r--   0 runner    (1001) docker     (127)    12628 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/gke/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/gke/fake.yml
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/gke/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/gke/kubeconfig.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.377548 kcli-99.0.202405071430/kvirt/cluster/hypershift/
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/hypershift/99-apps.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/hypershift/99-forcedns
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/hypershift/99-notifications.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/hypershift/Corefile
--rw-r--r--   0 runner    (1001) docker     (127)    46690 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/hypershift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/hypershift/assisted_infra.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/hypershift/assisted_ingress.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/hypershift/autoapprovercron.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/hypershift/bmc.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/hypershift/calico.sh.j2
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/hypershift/cilium.sh.j2
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/hypershift/cloud_lb_apps.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/hypershift/disconnected.sh
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/hypershift/extras.service
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/hypershift/extras.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/hypershift/hostedcluster.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/hypershift/httpd.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/hypershift/ignition.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/hypershift/kcli_plan.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/hypershift/kcli_plan_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/hypershift/keepalived.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/hypershift/nmstateconfig.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/hypershift/nodepool.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/hypershift/nonlocalbind.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.377548 kcli-99.0.202405071430/kvirt/cluster/hypershift/staticpods/
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/hypershift/staticpods/coredns.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/hypershift/staticpods/keepalived.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/hypershift/staticpods/mdns.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.377548 kcli-99.0.202405071430/kvirt/cluster/k3s/
--rw-r--r--   0 runner    (1001) docker     (127)    14022 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/k3s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/k3s/bootstrap.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/k3s/bootstrap.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/k3s/cloud_lb_api.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/k3s/ctlplanes.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/k3s/ctlplanes.yml
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/k3s/join.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/k3s/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/k3s/keepalived.conf
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/k3s/keepalived.sh
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/k3s/workers.sh
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/k3s/workers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.381548 kcli-99.0.202405071430/kvirt/cluster/kubeadm/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/10-flannel.link
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/90-flannel.rules
--rw-r--r--   0 runner    (1001) docker     (127)    15906 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.353548 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.381548 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/argocd/
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/argocd/ingress.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/argocd/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/argocd/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/argocd/uninstall.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.381548 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/autolabeller/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/autolabeller/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/autolabeller/uninstall.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.381548 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/certmanager/
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/certmanager/install.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.381548 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/dashboard/admin.yml
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/dashboard/ingress.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/dashboard/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/dashboard/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/dashboard/user.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.385548 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/falco/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/falco/falco_advertisements.yml
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/falco/falco_ip.yml
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/falco/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/falco/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/falco/uninstall.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.385548 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/ingress/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/ingress/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/ingress/uninstall.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.385548 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/istio/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/istio/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/istio/istio-minimal-operator.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.385548 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/katacontainer/
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/katacontainer/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/katacontainer/uninstall.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.385548 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/knative/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/knative/cr_eventing.yml
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/knative/cr_serving.yml
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/knative/install.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.385548 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/kubevirt/
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/kubevirt/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/kubevirt/kcli_default.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.385548 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/metallb/
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/metallb/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/metallb/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/metallb/metallb_advertisement.yml
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/metallb/metallb_cr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/metallb/uninstall.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.385548 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/olm/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/olm/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/olm/uninstall.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.385548 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/policy_as_code/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/policy_as_code/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/policy_as_code/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/policy_as_code/uninstall.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.389548 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/rancher/
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/rancher/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/rancher/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/rancher/rancher_advertisements.yml
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/rancher/rancher_ip.yml
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/rancher/uninstall.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.389548 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/rook/
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/rook/install.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.389548 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/submariner/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/submariner/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/submariner/kcli_default.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.389548 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/tekton/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/tekton/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/tekton/uninstall.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     3158 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/bootstrap.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/bootstrap.yml
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/cloud_lb_api.yml
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/crictl.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/ctlplanes.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)      343 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/deploy.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      598 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/join.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/keepalived.conf
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/keepalived.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/nfs.sh
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/nfs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/pre_el.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/pre_ubuntu.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/registry.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubeadm/workers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.389548 kcli-99.0.202405071430/kvirt/cluster/kubecommon/
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubecommon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.389548 kcli-99.0.202405071430/kvirt/cluster/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)     8809 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/kubernetes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.389548 kcli-99.0.202405071430/kvirt/cluster/microshift/
--rw-r--r--   0 runner    (1001) docker     (127)     4779 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/microshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/microshift/kcli_plan.yml
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/microshift/kcli_plan_default.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.389548 kcli-99.0.202405071430/kvirt/cluster/microshift/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/microshift/scripts/00_sslip.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/microshift/scripts/01_clients.sh
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/microshift/scripts/02_crio.sh
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/microshift/scripts/03_microshift.sh
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/microshift/scripts/04_kubeconfig.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/microshift/scripts/05_acm.sh
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/microshift/scripts/deploy.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.397548 kcli-99.0.202405071430/kvirt/cluster/openshift/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/01-workload-partitioning
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/10-node-ip-hint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/20-localhost-fix.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/99-apps.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/99-autologin.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/99-bootstrap-deletion-2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/99-bootstrap-deletion.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/99-chrony.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/99-forcedns
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/99-forcedns-ibm
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/99-kubevirt-fix.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/99-metal3-fake-machine.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/99-metal3-provisioning.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/99-notifications.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/99-operatorhub.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/99-ovn.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/99-sno.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/Corefile
--rwxr-xr-x   0 runner    (1001) docker     (127)    97697 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.401548 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.401548 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/advanced-cluster-management/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/advanced-cluster-management/99-metal3-provisioning.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/advanced-cluster-management/assisted-service.sample.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)     2839 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/advanced-cluster-management/assisted-service.sh
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/advanced-cluster-management/cr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/advanced-cluster-management/gen_registries.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/advanced-cluster-management/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/advanced-cluster-management/post.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.401548 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/argocd/
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/argocd/configmap.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/argocd/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/argocd/kcli_default.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.401548 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/autolabeller/
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/autolabeller/cr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/autolabeller/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/autolabeller/install.yml
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/autolabeller/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/autolabeller/uninstall.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.401548 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/cluster-logging/
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/cluster-logging/cr.yml
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/cluster-logging/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/cr.sh
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/install.yml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.401548 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/istio/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/istio/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/istio/istio-cni.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.401548 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/kubernetes-nmstate-operator/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/kubernetes-nmstate-operator/cr.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.401548 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/kubevirt-hyperconverged/
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/kubevirt-hyperconverged/cr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/kubevirt-hyperconverged/kcli_default.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.401548 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/local-storage-operator/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/local-storage-operator/cr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/local-storage-operator/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/local-storage-operator/post.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.405548 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/lvms-operator/
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/lvms-operator/cr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/lvms-operator/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/lvms-operator/post.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.405548 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/metallb-operator/
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/metallb-operator/cr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/metallb-operator/kcli_default.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.405548 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/multicluster-engine/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/multicluster-engine/99-metal3-provisioning.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/multicluster-engine/assisted-service.sample.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)     2846 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/multicluster-engine/assisted-service.sh
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/multicluster-engine/cr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/multicluster-engine/gen_registries.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/multicluster-engine/kcli_default.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)       55 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/multicluster-engine/post.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.405548 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/nfs/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2297 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/nfs/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/nfs/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/nfs/uninstall.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.405548 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/odf-operator/
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/odf-operator/cr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/odf-operator/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/odf-operator/nad_cluster.yml
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/odf-operator/nad_public.yml
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/odf-operator/post.sh
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/odf-operator/pre.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.405548 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/serverless-operator/
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/serverless-operator/cr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/serverless-operator/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/serverless-operator/post.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.405548 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/users/
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/users/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/users/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/users/oauth.yml
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/users/oauth_hypershift.yml
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/apps/users/uninstall.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/autoapprovercron.yml
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/autorules.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/bootstrap.yml
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/calico.sh.j2
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/chrony.conf
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/cilium.sh.j2
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/cloud_bootstrap.yml
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/cloud_ctlplanes.yml
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/cloud_dns.yml
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/cloud_lb_api.yml
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/cloud_lb_apps.yml
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/cloud_workers.yml
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/cluster-ingress-02-config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/cluster-scheduler-02-config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/config.hcl.templ
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/ctlplanes.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.409548 kcli-99.0.202405071430/kvirt/cluster/openshift/customisation/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/customisation/00-kcli-namespace.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/customisation/97-autoapprovercron-sa.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/customisation/98-autoapprovercron-binding.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/customisation/99-autoapprovercron-cronjob.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/customisation/99-ingress-controller.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/customisation/99-iptables.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/customisation/99-monitoring.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/customisation/99-registry.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/dhcp.conf
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/dhcp.sh
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/dhcp.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.409548 kcli-99.0.202405071430/kvirt/cluster/openshift/disconnected/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.409548 kcli-99.0.202405071430/kvirt/cluster/openshift/disconnected/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)      389 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/disconnected/bin/sync_image.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/disconnected/haproxy.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/disconnected/registry.service
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.409548 kcli-99.0.202405071430/kvirt/cluster/openshift/disconnected/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)      201 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/disconnected/scripts/01_get_oc.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      243 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/disconnected/scripts/02_packages.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     2444 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/disconnected/scripts/03_mirror.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     2133 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/disconnected/scripts/03_registry.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      331 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/disconnected/scripts/04_extras.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     2381 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/disconnected/scripts/05_olm.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      197 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/disconnected/scripts/06_web.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      841 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/disconnected/scripts/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/disconnected/scripts/mirror-config.yaml.sample
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/disconnected.yml
--rw-r--r--   0 runner    (1001) docker     (127)     8945 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/fake_kubeconfig.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/fake_pull.json
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/haproxy.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/haproxy.cfg.kubevirt
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/httpd.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/icsp.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/ignition.j2
--rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/install-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/iso.sh
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/kcli-ipv6.conf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/keepalived.conf
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/nonlocalbind.conf
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/openshift-workload-pinning
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/patch_ipv6.json
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/relocate-ip-bootstrap.service
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/relocate-ip-bootstrap.sh
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/relocate-ip.sh
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/sno-finish.service
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/sno-finish.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/sno.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/sno_default.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.409548 kcli-99.0.202405071430/kvirt/cluster/openshift/staticpods/
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/staticpods/coredns.yml
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/staticpods/haproxy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/staticpods/keepalived.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/staticpods/mdns.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/openshift/workers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.409548 kcli-99.0.202405071430/kvirt/cluster/profiles/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/profiles/sample-kubeadm-default.yml
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/profiles/sample-openshift-compact.yml
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/profiles/sample-openshift-contrail.yml
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/profiles/sample-openshift-ipv6.yml
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/profiles/sample-openshift-sno-bm.yml
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/profiles/sample-openshift-sno.yml
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/cluster/sampleprovider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.413548 kcli-99.0.202405071430/kvirt/common/
--rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/common/Jenkinsfile.j2
--rw-r--r--   0 runner    (1001) docker     (127)   105983 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/common/autoscale.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     8945 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/common/fake_kubeconfig.json
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/common/ignition.j2
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/common/kubevirt_kcli_conf.j2
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/common/local_kcli_conf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/common/pipeline.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/common/pipeline_kube.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/common/playbook.j2
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/common/storage.sh.aws
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/common/storage.sh.gcp
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/common/storage.sh.ibmcloud
--rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/common/vm.ovf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/common/workflow.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/common/workflow_script.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)   191137 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.413548 kcli-99.0.202405071430/kvirt/container/
--rw-r--r--   0 runner    (1001) docker     (127)    14188 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/containerconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)    11002 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/defaults.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1475 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/ekstoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    25462 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/examples.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.413548 kcli-99.0.202405071430/kvirt/expose/
--rw-r--r--   0 runner    (1001) docker     (127)    12263 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/expose/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.357548 kcli-99.0.202405071430/kvirt/expose/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.413548 kcli-99.0.202405071430/kvirt/expose/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/expose/static/css/bootstrap-notify.css
--rw-r--r--   0 runner    (1001) docker     (127)   121125 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/expose/static/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/expose/static/css/dataTables.checkboxes.css
--rw-r--r--   0 runner    (1001) docker     (127)    13587 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/expose/static/css/jquery.dataTables.min.css
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/expose/static/css/kcli.css
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/expose/static/css/wheel.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.417548 kcli-99.0.202405071430/kvirt/expose/static/images/
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/expose/static/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/expose/static/images/sort_asc.png
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/expose/static/images/sort_both.png
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/expose/static/images/sort_desc.png
--rw-r--r--   0 runner    (1001) docker     (127)    24772 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/expose/static/images/wheel.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.417548 kcli-99.0.202405071430/kvirt/expose/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)    12398 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/expose/static/js/dataTables.checkboxes.min.js
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/expose/static/js/exposeactions.js
--rw-r--r--   0 runner    (1001) docker     (127)    83059 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/expose/static/js/jquery.dataTables.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    89795 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/expose/static/js/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/expose/static/js/list.js
--rw-r--r--   0 runner    (1001) docker     (127)     4319 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/expose/swagger.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.417548 kcli-99.0.202405071430/kvirt/expose/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/expose/templates/form.html
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/expose/templates/head.html
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/expose/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/expose/templates/infoplan.html
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/expose/templates/planstable.html
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/expose/templates/result.html
--rwxr-xr-x   0 runner    (1001) docker     (127)     1047 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/gketoken.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4333 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/ignitionmerger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.417548 kcli-99.0.202405071430/kvirt/internalplans/
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/internalplans/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.417548 kcli-99.0.202405071430/kvirt/jinjafilters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/jinjafilters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/jinjafilters/jinjafilters.py
--rw-r--r--   0 runner    (1001) docker     (127)     9972 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/keywords.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.417548 kcli-99.0.202405071430/kvirt/kfish/
--rw-r--r--   0 runner    (1001) docker     (127)    13060 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/kfish/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3395 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/klist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.417548 kcli-99.0.202405071430/kvirt/ksushy/
--rw-r--r--   0 runner    (1001) docker     (127)    13633 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/ksushy/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      121 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/ksushy/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.421548 kcli-99.0.202405071430/kvirt/ksushy/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/ksushy/templates/bios.json
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/ksushy/templates/interface.json
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/ksushy/templates/interfaces.json
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/ksushy/templates/manager.json
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/ksushy/templates/managers.json
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/ksushy/templates/root.json
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/ksushy/templates/system.json
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/ksushy/templates/systems.json
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/ksushy/templates/virtualmedia_cd.json
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/ksushy/templates/virtualmedias.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.421548 kcli-99.0.202405071430/kvirt/miniconsole/
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/miniconsole/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.421548 kcli-99.0.202405071430/kvirt/nameutils/
--rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/nameutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.421548 kcli-99.0.202405071430/kvirt/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.421548 kcli-99.0.202405071430/kvirt/providers/aws/
--rw-r--r--   0 runner    (1001) docker     (127)   106499 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/providers/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/providers/aws/assume_policy.json
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/providers/aws/ctlplane_policy.json
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/providers/aws/worker_policy.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.421548 kcli-99.0.202405071430/kvirt/providers/azure/
--rw-r--r--   0 runner    (1001) docker     (127)    78530 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/providers/azure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.421548 kcli-99.0.202405071430/kvirt/providers/fake/
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/providers/fake/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.421548 kcli-99.0.202405071430/kvirt/providers/gcp/
--rw-r--r--   0 runner    (1001) docker     (127)   101005 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/providers/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/providers/gcp/gcp-hack.service
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/providers/gcp/gcp-hack.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.421548 kcli-99.0.202405071430/kvirt/providers/ibm/
--rw-r--r--   0 runner    (1001) docker     (127)    65793 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/providers/ibm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.421548 kcli-99.0.202405071430/kvirt/providers/kubevirt/
--rw-r--r--   0 runner    (1001) docker     (127)    86428 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/providers/kubevirt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.421548 kcli-99.0.202405071430/kvirt/providers/kvm/
--rw-r--r--   0 runner    (1001) docker     (127)   186733 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/providers/kvm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/providers/kvm/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.421548 kcli-99.0.202405071430/kvirt/providers/openstack/
--rw-r--r--   0 runner    (1001) docker     (127)    58301 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/providers/openstack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.421548 kcli-99.0.202405071430/kvirt/providers/ovirt/
--rw-r--r--   0 runner    (1001) docker     (127)    63384 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/providers/ovirt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.425548 kcli-99.0.202405071430/kvirt/providers/packet/
--rw-r--r--   0 runner    (1001) docker     (127)    31823 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/providers/packet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.425548 kcli-99.0.202405071430/kvirt/providers/proxmox/
--rw-r--r--   0 runner    (1001) docker     (127)    35276 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/providers/proxmox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9555 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/providers/sampleprovider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.425548 kcli-99.0.202405071430/kvirt/providers/vsphere/
--rw-r--r--   0 runner    (1001) docker     (127)    73908 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/providers/vsphere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13503 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/providers/vsphere/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4893 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/providers/vsphere/tagging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.425548 kcli-99.0.202405071430/kvirt/providers/web/
--rw-r--r--   0 runner    (1001) docker     (127)    22043 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/providers/web/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.425548 kcli-99.0.202405071430/kvirt/version/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-07 14:30:52.000000 kcli-99.0.202405071430/kvirt/version/git
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.425548 kcli-99.0.202405071430/kvirt/web/
--rwxr-xr-x   0 runner    (1001) docker     (127)    46680 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.361548 kcli-99.0.202405071430/kvirt/web/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.425548 kcli-99.0.202405071430/kvirt/web/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/css/bootstrap-notify.css
--rw-r--r--   0 runner    (1001) docker     (127)    23409 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/css/bootstrap-theme.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   121125 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/css/dataTables.checkboxes.css
--rw-r--r--   0 runner    (1001) docker     (127)    13587 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/css/jquery.dataTables.min.css
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/css/kcli.css
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/css/navbar.css
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/css/spice.css
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/css/wheel.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.425548 kcli-99.0.202405071430/kvirt/web/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)    18028 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.429548 kcli-99.0.202405071430/kvirt/web/static/images/
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/images/Centos.png
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/images/Debian.png
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/images/Fedora.png
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/images/Redhat.png
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/images/Suse.png
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/images/Tux.png
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/images/Ubuntu.png
--rw-r--r--   0 runner    (1001) docker     (127)     4213 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/images/delete.png
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    23320 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/images/kcli-small.png
--rw-r--r--   0 runner    (1001) docker     (127)    27185 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/images/kcli.jpg
--rw-r--r--   0 runner    (1001) docker     (127)   113928 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/images/kcli.png
--rw-r--r--   0 runner    (1001) docker     (127)    48809 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/images/logo-header.svg
--rw-r--r--   0 runner    (1001) docker     (127)    48809 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/images/logo-main.svg
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/images/sort_asc.png
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/images/sort_both.png
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/images/sort_desc.png
--rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/images/start.png
--rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/images/stop.png
--rw-r--r--   0 runner    (1001) docker     (127)    24772 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/images/wheel.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.433548 kcli-99.0.202405071430/kvirt/web/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/bootstrap-notify.js
--rw-r--r--   0 runner    (1001) docker     (127)    37045 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/containeraction.js
--rw-r--r--   0 runner    (1001) docker     (127)    12398 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/dataTables.checkboxes.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/hostaction.js
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/imageaction.js
--rw-r--r--   0 runner    (1001) docker     (127)    83059 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/jquery.dataTables.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    87462 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/kcli.js
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/kubeaction.js
--rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/list.js
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/networkaction.js
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/planaction.js
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/poolaction.js
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/productaction.js
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/refresh.js
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/repoaction.js
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/snapshotaction.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.437548 kcli-99.0.202405071430/kvirt/web/static/js/spice/
--rw-r--r--   0 runner    (1001) docker     (127)     9944 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/spice/atKeynames.js
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/spice/bitmap.js
--rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/spice/cursor.js
--rw-r--r--   0 runner    (1001) docker     (127)    49214 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/spice/display.js
--rw-r--r--   0 runner    (1001) docker     (127)    13253 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/spice/enums.js
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/spice/filexfer.js
--rw-r--r--   0 runner    (1001) docker     (127)     9535 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/spice/inputs.js
--rw-r--r--   0 runner    (1001) docker     (127)     6176 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/spice/lz.js
--rw-r--r--   0 runner    (1001) docker     (127)    18370 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/spice/main.js
--rw-r--r--   0 runner    (1001) docker     (127)    12677 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/spice/playback.js
--rw-r--r--   0 runner    (1001) docker     (127)     7036 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/spice/png.js
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/spice/port.js
--rw-r--r--   0 runner    (1001) docker     (127)    44531 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/spice/quic.js
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/spice/resize.js
--rw-r--r--   0 runner    (1001) docker     (127)     7282 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/spice/simulatecursor.js
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/spice/spicearraybuffer.js
--rw-r--r--   0 runner    (1001) docker     (127)    18202 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/spice/spiceconn.js
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/spice/spicedataview.js
--rw-r--r--   0 runner    (1001) docker     (127)    33015 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/spice/spicemsg.js
--rw-r--r--   0 runner    (1001) docker     (127)    12767 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/spice/spicetype.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.437548 kcli-99.0.202405071430/kvirt/web/static/js/spice/thirdparty/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.437548 kcli-99.0.202405071430/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/.npmignore
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/rollup.config.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.437548 kcli-99.0.202405071430/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/src/babel-worker.js
--rw-r--r--   0 runner    (1001) docker     (127)     8601 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/src/browser-es-module-loader.js
--rw-r--r--   0 runner    (1001) docker     (127)    16580 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/spice/thirdparty/jsbn.js
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/spice/thirdparty/prng4.js
--rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/spice/thirdparty/rng.js
--rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/spice/thirdparty/rsa.js
--rw-r--r--   0 runner    (1001) docker     (127)    10671 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/spice/thirdparty/sha1.js
--rw-r--r--   0 runner    (1001) docker     (127)     6808 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/spice/ticket.js
--rw-r--r--   0 runner    (1001) docker     (127)    13628 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/spice/utils.js
--rw-r--r--   0 runner    (1001) docker     (127)    21577 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/spice/webm.js
--rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/spice/wire.js
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/vmaction.js
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/js/wheel.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.361548 kcli-99.0.202405071430/kvirt/web/static/vnc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.437548 kcli-99.0.202405071430/kvirt/web/static/vnc/app/
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/error-handler.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.441548 kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/
--rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/alt.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/clipboard.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/connect.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/ctrl.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/ctrlaltdel.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/disconnect.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/drag.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/error.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/esc.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/expander.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/fullscreen.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/handle.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/handle_bg.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.445548 kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/icons/
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/icons/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/icons/novnc-120x120.png
--rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/icons/novnc-144x144.png
--rw-r--r--   0 runner    (1001) docker     (127)     5216 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/icons/novnc-152x152.png
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/icons/novnc-16x16.png
--rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/icons/novnc-192x192.png
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/icons/novnc-24x24.png
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/icons/novnc-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/icons/novnc-48x48.png
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/icons/novnc-60x60.png
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/icons/novnc-64x64.png
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/icons/novnc-72x72.png
--rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/icons/novnc-76x76.png
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/icons/novnc-96x96.png
--rw-r--r--   0 runner    (1001) docker     (127)    11685 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/icons/novnc-icon-sm.svg
--rw-r--r--   0 runner    (1001) docker     (127)    11549 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/icons/novnc-icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/info.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6404 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/keyboard.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7000 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/mouse_left.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7002 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/mouse_middle.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/mouse_none.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7001 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/mouse_right.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/power.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/settings.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/tab.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/toggleextrakeys.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/warning.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/windows.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.445548 kcli-99.0.202405071430/kvirt/web/static/vnc/app/locale/
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/locale/cs.json
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/locale/de.json
--rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/locale/el.json
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/locale/es.json
--rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/locale/ja.json
--rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/locale/ko.json
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/locale/nl.json
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/locale/pl.json
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/locale/ru.json
--rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/locale/sv.json
--rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/locale/tr.json
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/locale/zh_CN.json
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/locale/zh_TW.json
--rw-r--r--   0 runner    (1001) docker     (127)     5682 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/localization.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.449548 kcli-99.0.202405071430/kvirt/web/static/vnc/app/sounds/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/sounds/CREDITS
--rw-r--r--   0 runner    (1001) docker     (127)     4531 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/sounds/bell.mp3
--rw-r--r--   0 runner    (1001) docker     (127)     8495 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/sounds/bell.oga
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.449548 kcli-99.0.202405071430/kvirt/web/static/vnc/app/styles/
--rw-r--r--   0 runner    (1001) docker     (127)    38580 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/styles/Orbitron700.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    17472 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/styles/Orbitron700.woff
--rw-r--r--   0 runner    (1001) docker     (127)    18450 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/styles/base.css
--rw-r--r--   0 runner    (1001) docker     (127)    56845 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/ui.js
--rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/app/webutil.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.449548 kcli-99.0.202405071430/kvirt/web/static/vnc/core/
--rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/core/base64.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.449548 kcli-99.0.202405071430/kvirt/web/static/vnc/core/decoders/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/core/decoders/copyrect.js
--rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/core/decoders/hextile.js
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/core/decoders/raw.js
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/core/decoders/rre.js
--rw-r--r--   0 runner    (1001) docker     (127)     9662 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/core/decoders/tight.js
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/core/decoders/tightpng.js
--rw-r--r--   0 runner    (1001) docker     (127)    11241 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/core/des.js
--rw-r--r--   0 runner    (1001) docker     (127)    20381 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/core/display.js
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/core/encodings.js
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/core/inflator.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.449548 kcli-99.0.202405071430/kvirt/web/static/vnc/core/input/
--rw-r--r--   0 runner    (1001) docker     (127)    11438 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/core/input/domkeytable.js
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/core/input/fixedkeys.js
--rw-r--r--   0 runner    (1001) docker     (127)    13090 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/core/input/keyboard.js
--rw-r--r--   0 runner    (1001) docker     (127)    34609 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/core/input/keysym.js
--rw-r--r--   0 runner    (1001) docker     (127)    25374 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/core/input/keysymdef.js
--rw-r--r--   0 runner    (1001) docker     (127)     9995 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/core/input/mouse.js
--rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/core/input/util.js
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/core/input/vkeys.js
--rw-r--r--   0 runner    (1001) docker     (127)    14256 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/core/input/xtscancodes.js
--rw-r--r--   0 runner    (1001) docker     (127)    74196 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/core/rfb.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.453549 kcli-99.0.202405071430/kvirt/web/static/vnc/core/util/
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/core/util/browser.js
--rw-r--r--   0 runner    (1001) docker     (127)     7556 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/core/util/cursor.js
--rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/core/util/events.js
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/core/util/eventtarget.js
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/core/util/logging.js
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/core/util/polyfill.js
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/core/util/strings.js
--rw-r--r--   0 runner    (1001) docker     (127)     9130 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/core/websock.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.453549 kcli-99.0.202405071430/kvirt/web/static/vnc/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.453549 kcli-99.0.202405071430/kvirt/web/static/vnc/vendor/browser-es-module-loader/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/vendor/browser-es-module-loader/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/vendor/browser-es-module-loader/rollup.config.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.453549 kcli-99.0.202405071430/kvirt/web/static/vnc/vendor/browser-es-module-loader/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/vendor/browser-es-module-loader/src/babel-worker.js
--rw-r--r--   0 runner    (1001) docker     (127)     8498 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/vendor/browser-es-module-loader/src/browser-es-module-loader.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.453549 kcli-99.0.202405071430/kvirt/web/static/vnc/vendor/pako/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/vendor/pako/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/vendor/pako/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.361548 kcli-99.0.202405071430/kvirt/web/static/vnc/vendor/pako/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.453549 kcli-99.0.202405071430/kvirt/web/static/vnc/vendor/pako/lib/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/vendor/pako/lib/utils/common.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.453549 kcli-99.0.202405071430/kvirt/web/static/vnc/vendor/pako/lib/zlib/
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/vendor/pako/lib/zlib/adler32.js
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/vendor/pako/lib/zlib/constants.js
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/vendor/pako/lib/zlib/crc32.js
--rw-r--r--   0 runner    (1001) docker     (127)    60016 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/vendor/pako/lib/zlib/deflate.js
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/vendor/pako/lib/zlib/gzheader.js
--rw-r--r--   0 runner    (1001) docker     (127)    11690 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/vendor/pako/lib/zlib/inffast.js
--rw-r--r--   0 runner    (1001) docker     (127)    47128 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/vendor/pako/lib/zlib/inflate.js
--rw-r--r--   0 runner    (1001) docker     (127)    11527 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/vendor/pako/lib/zlib/inftrees.js
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/vendor/pako/lib/zlib/messages.js
--rw-r--r--   0 runner    (1001) docker     (127)    38767 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/vendor/pako/lib/zlib/trees.js
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/vendor/pako/lib/zlib/zstream.js
--rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/static/vnc/vendor/promise.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.461548 kcli-99.0.202405071430/kvirt/web/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/templates/bootstrap.html
--rw-r--r--   0 runner    (1001) docker     (127)    14595 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/templates/console.html
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/templates/containercreate.html
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/templates/containerprofiles.html
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/templates/containerprofilestable.html
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/templates/containers.html
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/templates/containerstable.html
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/templates/head.html
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/templates/hosts.html
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/templates/hoststable.html
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/templates/imagecreate.html
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/templates/images.html
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/templates/imagestable.html
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/templates/isos.html
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/templates/isostable.html
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/templates/kubecreate.html
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/templates/kubeinfo.html
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/templates/kubeprofiles.html
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/templates/kubeprofilestable.html
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/templates/kubes.html
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/templates/kubestable.html
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/templates/navbar.html
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/templates/networkcreate.html
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/templates/networks.html
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/templates/networkstable.html
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/templates/plancreate.html
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/templates/plans.html
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/templates/planstable.html
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/templates/poolcreate.html
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/templates/pools.html
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/templates/poolstable.html
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/templates/productcreate.html
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/templates/products.html
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/templates/productstable.html
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/templates/repocreate.html
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/templates/repos.html
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/templates/repostable.html
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/templates/vmcreate.html
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/templates/vmprofiles.html
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/templates/vmprofilestable.html
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/templates/vms.html
--rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/kvirt/web/templates/vmstable.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.461548 kcli-99.0.202405071430/samples/
--rw-r--r--   0 runner    (1001) docker     (127)     8879 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/samples/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/samples/profiles.yml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 14:30:53.461548 kcli-99.0.202405071430/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-07 14:30:52.000000 kcli-99.0.202405071430/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:30:53.461548 kcli-99.0.202405071430/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-07 14:28:23.000000 kcli-99.0.202405071430/tests/test_kvirt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.058643 kcli-99.0.202405080912/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-08 09:12:13.058643 kcli-99.0.202405080912/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:12.970644 kcli-99.0.202405080912/extras/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/extras/Dockerfile_curl
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/extras/Dockerfile_kubectl
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/extras/autoscale.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/extras/aws_peering.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/extras/aws_peering_cleaning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:12.970644 kcli-99.0.202405080912/extras/controller/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/extras/controller/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/extras/controller/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/extras/controller/crd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/extras/controller/deploy.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:12.970644 kcli-99.0.202405080912/extras/controller/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/extras/controller/examples/cluster_simple.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/extras/controller/examples/plan_complex.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/extras/controller/examples/plan_simple.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/extras/controller/examples/plan_simple_with_file.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/extras/controller/examples/vm_centos8stream.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/extras/controller/examples/vm_cirros.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/extras/controller/examples/vm_empty.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/extras/controller/examples/vm_fedora.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     9970 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/extras/controller/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/extras/controller/stress_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/extras/debian
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:12.970644 kcli-99.0.202405080912/extras/expose/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/extras/expose/kcli.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/extras/expose/kcli.wsgi
+-rwxr-xr-x   0 runner    (1001) docker     (127)      106 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/extras/genrst.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/extras/haproxy.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/extras/haproxy_multiple_clusters.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/extras/i_am_a_container
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/extras/k8sdeploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/extras/kfish.md
+-rw-r--r--   0 runner    (1001) docker     (127)    38837 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/extras/kfish.png
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/extras/missing_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/extras/openstack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/extras/openstack.sh.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/extras/zerotier.service
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:12.974644 kcli-99.0.202405080912/kcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-08 09:12:12.000000 kcli-99.0.202405080912/kcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    27279 2024-05-08 09:12:12.000000 kcli-99.0.202405080912/kcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 09:12:12.000000 kcli-99.0.202405080912/kcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-08 09:12:12.000000 kcli-99.0.202405080912/kcli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 09:11:13.000000 kcli-99.0.202405080912/kcli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-08 09:12:12.000000 kcli-99.0.202405080912/kcli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-08 09:12:12.000000 kcli-99.0.202405080912/kcli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:12.974644 kcli-99.0.202405080912/kvirt/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:12.974644 kcli-99.0.202405080912/kvirt/ansibleutils/
+-rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/ansibleutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86900 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/baseconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)   171487 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/bottle.py
+-rw-r--r--   0 runner    (1001) docker     (127)   273083 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:12.974644 kcli-99.0.202405080912/kvirt/cluster/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:12.974644 kcli-99.0.202405080912/kvirt/cluster/aks/
+-rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/aks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/aks/fake.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/aks/kcli_default.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:12.974644 kcli-99.0.202405080912/kvirt/cluster/eks/
+-rw-r--r--   0 runner    (1001) docker     (127)    12290 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/eks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/eks/fake.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/eks/kcli_default.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:12.978644 kcli-99.0.202405080912/kvirt/cluster/gke/
+-rw-r--r--   0 runner    (1001) docker     (127)    12628 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/gke/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/gke/fake.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/gke/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/gke/kubeconfig.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:12.978644 kcli-99.0.202405080912/kvirt/cluster/hypershift/
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/hypershift/99-apps.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/hypershift/99-forcedns
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/hypershift/99-notifications.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/hypershift/Corefile
+-rw-r--r--   0 runner    (1001) docker     (127)    46690 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/hypershift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/hypershift/assisted_infra.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/hypershift/assisted_ingress.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/hypershift/autoapprovercron.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/hypershift/bmc.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/hypershift/calico.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/hypershift/cilium.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/hypershift/cloud_lb_apps.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/hypershift/disconnected.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/hypershift/extras.service
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/hypershift/extras.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/hypershift/hostedcluster.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/hypershift/httpd.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/hypershift/ignition.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/hypershift/kcli_plan.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/hypershift/kcli_plan_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/hypershift/keepalived.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/hypershift/nmstateconfig.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/hypershift/nodepool.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/hypershift/nonlocalbind.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:12.978644 kcli-99.0.202405080912/kvirt/cluster/hypershift/staticpods/
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/hypershift/staticpods/coredns.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/hypershift/staticpods/keepalived.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/hypershift/staticpods/mdns.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:12.982644 kcli-99.0.202405080912/kvirt/cluster/k3s/
+-rw-r--r--   0 runner    (1001) docker     (127)    14022 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/k3s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/k3s/bootstrap.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/k3s/bootstrap.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/k3s/cloud_lb_api.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/k3s/ctlplanes.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/k3s/ctlplanes.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/k3s/join.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/k3s/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/k3s/keepalived.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/k3s/keepalived.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/k3s/workers.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/k3s/workers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:12.982644 kcli-99.0.202405080912/kvirt/cluster/kubeadm/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/10-flannel.link
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/90-flannel.rules
+-rw-r--r--   0 runner    (1001) docker     (127)    15906 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:12.958644 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:12.986644 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/argocd/
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/argocd/ingress.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/argocd/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/argocd/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/argocd/uninstall.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:12.986644 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/autolabeller/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/autolabeller/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/autolabeller/uninstall.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:12.986644 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/certmanager/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/certmanager/install.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:12.986644 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/dashboard/admin.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/dashboard/ingress.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/dashboard/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/dashboard/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/dashboard/user.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:12.986644 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/falco/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/falco/falco_advertisements.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/falco/falco_ip.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/falco/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/falco/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/falco/uninstall.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:12.986644 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/ingress/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/ingress/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/ingress/uninstall.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:12.986644 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/istio/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/istio/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/istio/istio-minimal-operator.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:12.986644 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/katacontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/katacontainer/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/katacontainer/uninstall.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:12.986644 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/knative/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/knative/cr_eventing.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/knative/cr_serving.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/knative/install.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:12.986644 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/kubevirt/
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/kubevirt/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/kubevirt/kcli_default.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:12.990644 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/metallb/
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/metallb/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/metallb/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/metallb/metallb_advertisement.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/metallb/metallb_cr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/metallb/uninstall.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:12.990644 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/olm/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/olm/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/olm/uninstall.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:12.990644 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/policy_as_code/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/policy_as_code/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/policy_as_code/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/policy_as_code/uninstall.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:12.990644 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/rancher/
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/rancher/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/rancher/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/rancher/rancher_advertisements.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/rancher/rancher_ip.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/rancher/uninstall.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:12.990644 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/rook/
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/rook/install.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:12.990644 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/submariner/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/submariner/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/submariner/kcli_default.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:12.990644 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/tekton/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/tekton/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/tekton/uninstall.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3158 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/bootstrap.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/bootstrap.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/cloud_lb_api.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/crictl.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/ctlplanes.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      343 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/deploy.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      598 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/join.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/keepalived.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/keepalived.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/nfs.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/nfs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/pre_el.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/pre_ubuntu.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/registry.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubeadm/workers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:12.990644 kcli-99.0.202405080912/kvirt/cluster/kubecommon/
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubecommon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:12.990644 kcli-99.0.202405080912/kvirt/cluster/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)     8809 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/kubernetes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:12.990644 kcli-99.0.202405080912/kvirt/cluster/microshift/
+-rw-r--r--   0 runner    (1001) docker     (127)     4779 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/microshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/microshift/kcli_plan.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/microshift/kcli_plan_default.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:12.990644 kcli-99.0.202405080912/kvirt/cluster/microshift/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/microshift/scripts/00_sslip.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/microshift/scripts/01_clients.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/microshift/scripts/02_crio.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/microshift/scripts/03_microshift.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/microshift/scripts/04_kubeconfig.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/microshift/scripts/05_acm.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/microshift/scripts/deploy.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:12.998644 kcli-99.0.202405080912/kvirt/cluster/openshift/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/01-workload-partitioning
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/10-node-ip-hint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/20-localhost-fix.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/99-apps.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/99-autologin.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/99-bootstrap-deletion-2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/99-bootstrap-deletion.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/99-chrony.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/99-forcedns
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/99-forcedns-ibm
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/99-kubevirt-fix.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/99-metal3-fake-machine.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/99-metal3-provisioning.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/99-notifications.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/99-operatorhub.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/99-ovn.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/99-sno.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/Corefile
+-rwxr-xr-x   0 runner    (1001) docker     (127)    97697 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:12.998644 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.002644 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/advanced-cluster-management/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/advanced-cluster-management/99-metal3-provisioning.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/advanced-cluster-management/assisted-service.sample.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2839 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/advanced-cluster-management/assisted-service.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/advanced-cluster-management/cr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/advanced-cluster-management/gen_registries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/advanced-cluster-management/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/advanced-cluster-management/post.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.002644 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/argocd/
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/argocd/configmap.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/argocd/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/argocd/kcli_default.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.002644 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/autolabeller/
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/autolabeller/cr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/autolabeller/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/autolabeller/install.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/autolabeller/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/autolabeller/uninstall.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.002644 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/cluster-logging/
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/cluster-logging/cr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/cluster-logging/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/cr.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/install.yml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.002644 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/istio/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/istio/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/istio/istio-cni.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.002644 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/kubernetes-nmstate-operator/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/kubernetes-nmstate-operator/cr.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.002644 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/kubevirt-hyperconverged/
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/kubevirt-hyperconverged/cr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/kubevirt-hyperconverged/kcli_default.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.002644 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/local-storage-operator/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/local-storage-operator/cr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/local-storage-operator/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/local-storage-operator/post.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.002644 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/lvms-operator/
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/lvms-operator/cr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/lvms-operator/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/lvms-operator/post.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.002644 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/metallb-operator/
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/metallb-operator/cr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/metallb-operator/kcli_default.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.006644 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/multicluster-engine/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/multicluster-engine/99-metal3-provisioning.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/multicluster-engine/assisted-service.sample.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2846 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/multicluster-engine/assisted-service.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/multicluster-engine/cr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/multicluster-engine/gen_registries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/multicluster-engine/kcli_default.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)       55 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/multicluster-engine/post.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.006644 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/nfs/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2297 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/nfs/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/nfs/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/nfs/uninstall.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.006644 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/odf-operator/
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/odf-operator/cr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/odf-operator/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/odf-operator/nad_cluster.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/odf-operator/nad_public.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/odf-operator/post.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/odf-operator/pre.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.006644 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/serverless-operator/
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/serverless-operator/cr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/serverless-operator/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/serverless-operator/post.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.006644 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/users/
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/users/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/users/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/users/oauth.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/users/oauth_hypershift.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/apps/users/uninstall.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/autoapprovercron.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/autorules.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/bootstrap.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/calico.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/chrony.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/cilium.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/cloud_bootstrap.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/cloud_ctlplanes.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/cloud_dns.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/cloud_lb_api.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/cloud_lb_apps.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/cloud_workers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/cluster-ingress-02-config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/cluster-scheduler-02-config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/config.hcl.templ
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/ctlplanes.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.006644 kcli-99.0.202405080912/kvirt/cluster/openshift/customisation/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/customisation/00-kcli-namespace.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/customisation/97-autoapprovercron-sa.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/customisation/98-autoapprovercron-binding.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/customisation/99-autoapprovercron-cronjob.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/customisation/99-ingress-controller.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/customisation/99-iptables.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/customisation/99-monitoring.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/customisation/99-registry.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/dhcp.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/dhcp.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/dhcp.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.006644 kcli-99.0.202405080912/kvirt/cluster/openshift/disconnected/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.006644 kcli-99.0.202405080912/kvirt/cluster/openshift/disconnected/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      389 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/disconnected/bin/sync_image.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/disconnected/haproxy.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/disconnected/registry.service
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.010644 kcli-99.0.202405080912/kvirt/cluster/openshift/disconnected/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      201 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/disconnected/scripts/01_get_oc.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      243 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/disconnected/scripts/02_packages.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2444 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/disconnected/scripts/03_mirror.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2133 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/disconnected/scripts/03_registry.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      331 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/disconnected/scripts/04_extras.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2381 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/disconnected/scripts/05_olm.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      197 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/disconnected/scripts/06_web.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      841 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/disconnected/scripts/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/disconnected/scripts/mirror-config.yaml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/disconnected.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     8945 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/fake_kubeconfig.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/fake_pull.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/haproxy.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/haproxy.cfg.kubevirt
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/httpd.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/icsp.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/ignition.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/install-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/iso.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/kcli-ipv6.conf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/keepalived.conf
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/nonlocalbind.conf
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/openshift-workload-pinning
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/patch_ipv6.json
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/relocate-ip-bootstrap.service
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/relocate-ip-bootstrap.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/relocate-ip.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/sno-finish.service
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/sno-finish.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/sno.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/sno_default.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.010644 kcli-99.0.202405080912/kvirt/cluster/openshift/staticpods/
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/staticpods/coredns.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/staticpods/haproxy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/staticpods/keepalived.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/staticpods/mdns.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/openshift/workers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.010644 kcli-99.0.202405080912/kvirt/cluster/profiles/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/profiles/sample-kubeadm-default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/profiles/sample-openshift-compact.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/profiles/sample-openshift-contrail.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/profiles/sample-openshift-ipv6.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/profiles/sample-openshift-sno-bm.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/profiles/sample-openshift-sno.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/cluster/sampleprovider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.010644 kcli-99.0.202405080912/kvirt/common/
+-rw-r--r--   0 runner    (1001) docker     (127)   105983 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/common/autoscale.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     8945 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/common/fake_kubeconfig.json
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/common/ignition.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/common/kubevirt_kcli_conf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/common/local_kcli_conf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/common/storage.sh.aws
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/common/storage.sh.gcp
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/common/storage.sh.ibmcloud
+-rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/common/vm.ovf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/common/workflow.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/common/workflow_script.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)   191137 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.010644 kcli-99.0.202405080912/kvirt/container/
+-rw-r--r--   0 runner    (1001) docker     (127)    14188 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/containerconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11002 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/defaults.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1475 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/ekstoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25462 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/examples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.014644 kcli-99.0.202405080912/kvirt/expose/
+-rw-r--r--   0 runner    (1001) docker     (127)    12263 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/expose/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:12.962644 kcli-99.0.202405080912/kvirt/expose/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.014644 kcli-99.0.202405080912/kvirt/expose/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/expose/static/css/bootstrap-notify.css
+-rw-r--r--   0 runner    (1001) docker     (127)   121125 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/expose/static/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/expose/static/css/dataTables.checkboxes.css
+-rw-r--r--   0 runner    (1001) docker     (127)    13587 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/expose/static/css/jquery.dataTables.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/expose/static/css/kcli.css
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/expose/static/css/wheel.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.014644 kcli-99.0.202405080912/kvirt/expose/static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/expose/static/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/expose/static/images/sort_asc.png
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/expose/static/images/sort_both.png
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/expose/static/images/sort_desc.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24772 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/expose/static/images/wheel.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.014644 kcli-99.0.202405080912/kvirt/expose/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    12398 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/expose/static/js/dataTables.checkboxes.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/expose/static/js/exposeactions.js
+-rw-r--r--   0 runner    (1001) docker     (127)    83059 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/expose/static/js/jquery.dataTables.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    89795 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/expose/static/js/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/expose/static/js/list.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4319 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/expose/swagger.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.014644 kcli-99.0.202405080912/kvirt/expose/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/expose/templates/form.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/expose/templates/head.html
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/expose/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/expose/templates/infoplan.html
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/expose/templates/planstable.html
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/expose/templates/result.html
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1047 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/gketoken.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4333 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/ignitionmerger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.014644 kcli-99.0.202405080912/kvirt/internalplans/
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/internalplans/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.014644 kcli-99.0.202405080912/kvirt/jinjafilters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/jinjafilters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/jinjafilters/jinjafilters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9972 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/keywords.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.014644 kcli-99.0.202405080912/kvirt/kfish/
+-rw-r--r--   0 runner    (1001) docker     (127)    13060 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/kfish/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3395 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/klist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.014644 kcli-99.0.202405080912/kvirt/ksushy/
+-rw-r--r--   0 runner    (1001) docker     (127)    13634 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/ksushy/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      121 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/ksushy/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.018644 kcli-99.0.202405080912/kvirt/ksushy/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/ksushy/templates/bios.json
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/ksushy/templates/interface.json
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/ksushy/templates/interfaces.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/ksushy/templates/manager.json
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/ksushy/templates/managers.json
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/ksushy/templates/root.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/ksushy/templates/system.json
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/ksushy/templates/systems.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/ksushy/templates/virtualmedia_cd.json
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/ksushy/templates/virtualmedias.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.018644 kcli-99.0.202405080912/kvirt/miniconsole/
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/miniconsole/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.018644 kcli-99.0.202405080912/kvirt/nameutils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/nameutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.018644 kcli-99.0.202405080912/kvirt/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.018644 kcli-99.0.202405080912/kvirt/providers/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)   106499 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/providers/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/providers/aws/assume_policy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/providers/aws/ctlplane_policy.json
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/providers/aws/worker_policy.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.018644 kcli-99.0.202405080912/kvirt/providers/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)    78530 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/providers/azure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.018644 kcli-99.0.202405080912/kvirt/providers/fake/
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/providers/fake/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.018644 kcli-99.0.202405080912/kvirt/providers/gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)   101005 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/providers/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/providers/gcp/gcp-hack.service
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/providers/gcp/gcp-hack.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.018644 kcli-99.0.202405080912/kvirt/providers/ibm/
+-rw-r--r--   0 runner    (1001) docker     (127)    65793 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/providers/ibm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.018644 kcli-99.0.202405080912/kvirt/providers/kubevirt/
+-rw-r--r--   0 runner    (1001) docker     (127)    86428 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/providers/kubevirt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.022644 kcli-99.0.202405080912/kvirt/providers/kvm/
+-rw-r--r--   0 runner    (1001) docker     (127)   186733 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/providers/kvm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/providers/kvm/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.022644 kcli-99.0.202405080912/kvirt/providers/openstack/
+-rw-r--r--   0 runner    (1001) docker     (127)    58301 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/providers/openstack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.022644 kcli-99.0.202405080912/kvirt/providers/ovirt/
+-rw-r--r--   0 runner    (1001) docker     (127)    63384 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/providers/ovirt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.022644 kcli-99.0.202405080912/kvirt/providers/packet/
+-rw-r--r--   0 runner    (1001) docker     (127)    31823 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/providers/packet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.022644 kcli-99.0.202405080912/kvirt/providers/proxmox/
+-rw-r--r--   0 runner    (1001) docker     (127)    35276 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/providers/proxmox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9555 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/providers/sampleprovider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.022644 kcli-99.0.202405080912/kvirt/providers/vsphere/
+-rw-r--r--   0 runner    (1001) docker     (127)    73908 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/providers/vsphere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13503 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/providers/vsphere/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4893 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/providers/vsphere/tagging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.022644 kcli-99.0.202405080912/kvirt/providers/web/
+-rw-r--r--   0 runner    (1001) docker     (127)    22043 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/providers/web/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.022644 kcli-99.0.202405080912/kvirt/version/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-08 09:12:12.000000 kcli-99.0.202405080912/kvirt/version/git
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.022644 kcli-99.0.202405080912/kvirt/web/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    46680 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:12.966644 kcli-99.0.202405080912/kvirt/web/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.022644 kcli-99.0.202405080912/kvirt/web/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/css/bootstrap-notify.css
+-rw-r--r--   0 runner    (1001) docker     (127)    23409 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/css/bootstrap-theme.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   121125 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/css/dataTables.checkboxes.css
+-rw-r--r--   0 runner    (1001) docker     (127)    13587 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/css/jquery.dataTables.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/css/kcli.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/css/navbar.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/css/spice.css
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/css/wheel.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.026644 kcli-99.0.202405080912/kvirt/web/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    18028 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.026644 kcli-99.0.202405080912/kvirt/web/static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/images/Centos.png
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/images/Debian.png
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/images/Fedora.png
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/images/Redhat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/images/Suse.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/images/Tux.png
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/images/Ubuntu.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4213 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/images/delete.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    23320 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/images/kcli-small.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27185 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/images/kcli.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)   113928 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/images/kcli.png
+-rw-r--r--   0 runner    (1001) docker     (127)    48809 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/images/logo-header.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    48809 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/images/logo-main.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/images/sort_asc.png
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/images/sort_both.png
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/images/sort_desc.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/images/start.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/images/stop.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24772 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/images/wheel.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.030644 kcli-99.0.202405080912/kvirt/web/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/bootstrap-notify.js
+-rw-r--r--   0 runner    (1001) docker     (127)    37045 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/containeraction.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12398 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/dataTables.checkboxes.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/hostaction.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/imageaction.js
+-rw-r--r--   0 runner    (1001) docker     (127)    83059 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/jquery.dataTables.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    87462 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/kcli.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/kubeaction.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/list.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/networkaction.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/planaction.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/poolaction.js
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/productaction.js
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/refresh.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/repoaction.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/snapshotaction.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.034644 kcli-99.0.202405080912/kvirt/web/static/js/spice/
+-rw-r--r--   0 runner    (1001) docker     (127)     9944 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/spice/atKeynames.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/spice/bitmap.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/spice/cursor.js
+-rw-r--r--   0 runner    (1001) docker     (127)    49214 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/spice/display.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13253 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/spice/enums.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/spice/filexfer.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9535 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/spice/inputs.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6176 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/spice/lz.js
+-rw-r--r--   0 runner    (1001) docker     (127)    18370 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/spice/main.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12677 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/spice/playback.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7036 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/spice/png.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/spice/port.js
+-rw-r--r--   0 runner    (1001) docker     (127)    44531 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/spice/quic.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/spice/resize.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7282 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/spice/simulatecursor.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/spice/spicearraybuffer.js
+-rw-r--r--   0 runner    (1001) docker     (127)    18202 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/spice/spiceconn.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/spice/spicedataview.js
+-rw-r--r--   0 runner    (1001) docker     (127)    33015 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/spice/spicemsg.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12767 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/spice/spicetype.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.034644 kcli-99.0.202405080912/kvirt/web/static/js/spice/thirdparty/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.034644 kcli-99.0.202405080912/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/.npmignore
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/rollup.config.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.034644 kcli-99.0.202405080912/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/src/babel-worker.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8601 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/src/browser-es-module-loader.js
+-rw-r--r--   0 runner    (1001) docker     (127)    16580 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/spice/thirdparty/jsbn.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/spice/thirdparty/prng4.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/spice/thirdparty/rng.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/spice/thirdparty/rsa.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10671 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/spice/thirdparty/sha1.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6808 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/spice/ticket.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13628 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/spice/utils.js
+-rw-r--r--   0 runner    (1001) docker     (127)    21577 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/spice/webm.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/spice/wire.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/vmaction.js
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/js/wheel.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:12.966644 kcli-99.0.202405080912/kvirt/web/static/vnc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.038644 kcli-99.0.202405080912/kvirt/web/static/vnc/app/
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/error-handler.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.038644 kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/alt.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/clipboard.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/connect.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/ctrl.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/ctrlaltdel.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/disconnect.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/drag.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/error.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/esc.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/expander.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/fullscreen.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/handle.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/handle_bg.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.042644 kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/icons/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/icons/novnc-120x120.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/icons/novnc-144x144.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5216 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/icons/novnc-152x152.png
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/icons/novnc-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/icons/novnc-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/icons/novnc-24x24.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/icons/novnc-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/icons/novnc-48x48.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/icons/novnc-60x60.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/icons/novnc-64x64.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/icons/novnc-72x72.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/icons/novnc-76x76.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/icons/novnc-96x96.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11685 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/icons/novnc-icon-sm.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11549 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/icons/novnc-icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/info.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6404 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/keyboard.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7000 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/mouse_left.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7002 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/mouse_middle.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/mouse_none.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7001 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/mouse_right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/power.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/settings.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/tab.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/toggleextrakeys.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/warning.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/windows.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.042644 kcli-99.0.202405080912/kvirt/web/static/vnc/app/locale/
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/locale/cs.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/locale/de.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/locale/el.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/locale/es.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/locale/ja.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/locale/ko.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/locale/nl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/locale/pl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/locale/ru.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/locale/sv.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/locale/tr.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/locale/zh_CN.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/locale/zh_TW.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5682 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/localization.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.046644 kcli-99.0.202405080912/kvirt/web/static/vnc/app/sounds/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/sounds/CREDITS
+-rw-r--r--   0 runner    (1001) docker     (127)     4531 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/sounds/bell.mp3
+-rw-r--r--   0 runner    (1001) docker     (127)     8495 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/sounds/bell.oga
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.046644 kcli-99.0.202405080912/kvirt/web/static/vnc/app/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)    38580 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/styles/Orbitron700.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    17472 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/styles/Orbitron700.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    18450 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/styles/base.css
+-rw-r--r--   0 runner    (1001) docker     (127)    56845 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/ui.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/app/webutil.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.046644 kcli-99.0.202405080912/kvirt/web/static/vnc/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/core/base64.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.046644 kcli-99.0.202405080912/kvirt/web/static/vnc/core/decoders/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/core/decoders/copyrect.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/core/decoders/hextile.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/core/decoders/raw.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/core/decoders/rre.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9662 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/core/decoders/tight.js
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/core/decoders/tightpng.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11241 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/core/des.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20381 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/core/display.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/core/encodings.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/core/inflator.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.046644 kcli-99.0.202405080912/kvirt/web/static/vnc/core/input/
+-rw-r--r--   0 runner    (1001) docker     (127)    11438 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/core/input/domkeytable.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/core/input/fixedkeys.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13090 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/core/input/keyboard.js
+-rw-r--r--   0 runner    (1001) docker     (127)    34609 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/core/input/keysym.js
+-rw-r--r--   0 runner    (1001) docker     (127)    25374 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/core/input/keysymdef.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9995 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/core/input/mouse.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/core/input/util.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/core/input/vkeys.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14256 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/core/input/xtscancodes.js
+-rw-r--r--   0 runner    (1001) docker     (127)    74196 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/core/rfb.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.050644 kcli-99.0.202405080912/kvirt/web/static/vnc/core/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/core/util/browser.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7556 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/core/util/cursor.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/core/util/events.js
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/core/util/eventtarget.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/core/util/logging.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/core/util/polyfill.js
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/core/util/strings.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9130 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/core/websock.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.050644 kcli-99.0.202405080912/kvirt/web/static/vnc/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.050644 kcli-99.0.202405080912/kvirt/web/static/vnc/vendor/browser-es-module-loader/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/vendor/browser-es-module-loader/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/vendor/browser-es-module-loader/rollup.config.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.050644 kcli-99.0.202405080912/kvirt/web/static/vnc/vendor/browser-es-module-loader/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/vendor/browser-es-module-loader/src/babel-worker.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8498 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/vendor/browser-es-module-loader/src/browser-es-module-loader.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.050644 kcli-99.0.202405080912/kvirt/web/static/vnc/vendor/pako/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/vendor/pako/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/vendor/pako/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:12.966644 kcli-99.0.202405080912/kvirt/web/static/vnc/vendor/pako/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.050644 kcli-99.0.202405080912/kvirt/web/static/vnc/vendor/pako/lib/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/vendor/pako/lib/utils/common.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.050644 kcli-99.0.202405080912/kvirt/web/static/vnc/vendor/pako/lib/zlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/vendor/pako/lib/zlib/adler32.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/vendor/pako/lib/zlib/constants.js
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/vendor/pako/lib/zlib/crc32.js
+-rw-r--r--   0 runner    (1001) docker     (127)    60016 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/vendor/pako/lib/zlib/deflate.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/vendor/pako/lib/zlib/gzheader.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11690 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/vendor/pako/lib/zlib/inffast.js
+-rw-r--r--   0 runner    (1001) docker     (127)    47128 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/vendor/pako/lib/zlib/inflate.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11527 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/vendor/pako/lib/zlib/inftrees.js
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/vendor/pako/lib/zlib/messages.js
+-rw-r--r--   0 runner    (1001) docker     (127)    38767 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/vendor/pako/lib/zlib/trees.js
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/vendor/pako/lib/zlib/zstream.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/static/vnc/vendor/promise.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.058643 kcli-99.0.202405080912/kvirt/web/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/templates/bootstrap.html
+-rw-r--r--   0 runner    (1001) docker     (127)    14595 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/templates/console.html
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/templates/containercreate.html
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/templates/containerprofiles.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/templates/containerprofilestable.html
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/templates/containers.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/templates/containerstable.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/templates/head.html
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/templates/hosts.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/templates/hoststable.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/templates/imagecreate.html
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/templates/images.html
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/templates/imagestable.html
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/templates/isos.html
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/templates/isostable.html
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/templates/kubecreate.html
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/templates/kubeinfo.html
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/templates/kubeprofiles.html
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/templates/kubeprofilestable.html
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/templates/kubes.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/templates/kubestable.html
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/templates/navbar.html
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/templates/networkcreate.html
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/templates/networks.html
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/templates/networkstable.html
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/templates/plancreate.html
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/templates/plans.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/templates/planstable.html
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/templates/poolcreate.html
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/templates/pools.html
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/templates/poolstable.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/templates/productcreate.html
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/templates/products.html
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/templates/productstable.html
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/templates/repocreate.html
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/templates/repos.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/templates/repostable.html
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/templates/vmcreate.html
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/templates/vmprofiles.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/templates/vmprofilestable.html
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/templates/vms.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/kvirt/web/templates/vmstable.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.058643 kcli-99.0.202405080912/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)     8879 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/samples/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/samples/profiles.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 09:12:13.058643 kcli-99.0.202405080912/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-08 09:12:12.000000 kcli-99.0.202405080912/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:12:13.058643 kcli-99.0.202405080912/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-08 09:10:22.000000 kcli-99.0.202405080912/tests/test_kvirt.py
```

### Comparing `kcli-99.0.202405071430/LICENSE` & `kcli-99.0.202405080912/LICENSE`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/MANIFEST.in` & `kcli-99.0.202405080912/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/PKG-INFO` & `kcli-99.0.202405080912/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kcli
-Version: 99.0.202405071430
+Version: 99.0.202405080912
 Summary: Provisioner/Manager for Libvirt/Vsphere/Aws/Gcp/Kubevirt/Ovirt/Openstack/IBM Cloud and containers
 Home-page: http://github.com/karmab/kcli
 Author: Karim Boumedhel
 Author-email: karimboumedhel@gmail.com
 License: ASL
 Platform: UNKNOWN
 Provides-Extra: all
```

### Comparing `kcli-99.0.202405071430/README.md` & `kcli-99.0.202405080912/README.md`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/extras/autoscale.yml` & `kcli-99.0.202405080912/extras/autoscale.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/extras/aws_peering.py` & `kcli-99.0.202405080912/extras/aws_peering.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/extras/aws_peering_cleaning.py` & `kcli-99.0.202405080912/extras/aws_peering_cleaning.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/extras/controller/README.md` & `kcli-99.0.202405080912/extras/controller/README.md`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/extras/controller/crd.yml` & `kcli-99.0.202405080912/extras/controller/crd.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/extras/controller/deploy.yml` & `kcli-99.0.202405080912/extras/controller/deploy.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/extras/controller/examples/plan_complex.yml` & `kcli-99.0.202405080912/extras/controller/examples/plan_complex.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/extras/controller/handlers.py` & `kcli-99.0.202405080912/extras/controller/handlers.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/extras/controller/stress_test.yml` & `kcli-99.0.202405080912/extras/controller/stress_test.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/extras/debian` & `kcli-99.0.202405080912/extras/debian`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/extras/haproxy.cfg` & `kcli-99.0.202405080912/extras/haproxy.cfg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/extras/haproxy_multiple_clusters.cfg` & `kcli-99.0.202405080912/extras/haproxy_multiple_clusters.cfg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/extras/k8sdeploy.yml` & `kcli-99.0.202405080912/extras/k8sdeploy.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/extras/kfish.md` & `kcli-99.0.202405080912/extras/kfish.md`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/extras/kfish.png` & `kcli-99.0.202405080912/extras/kfish.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/extras/openstack.py` & `kcli-99.0.202405080912/extras/openstack.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/extras/openstack.sh.sample` & `kcli-99.0.202405080912/extras/openstack.sh.sample`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/extras/zerotier.service` & `kcli-99.0.202405080912/extras/zerotier.service`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kcli.egg-info/PKG-INFO` & `kcli-99.0.202405080912/kcli.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kcli
-Version: 99.0.202405071430
+Version: 99.0.202405080912
 Summary: Provisioner/Manager for Libvirt/Vsphere/Aws/Gcp/Kubevirt/Ovirt/Openstack/IBM Cloud and containers
 Home-page: http://github.com/karmab/kcli
 Author: Karim Boumedhel
 Author-email: karimboumedhel@gmail.com
 License: ASL
 Platform: UNKNOWN
 Provides-Extra: all
```

### Comparing `kcli-99.0.202405071430/kcli.egg-info/SOURCES.txt` & `kcli-99.0.202405080912/kcli.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -330,24 +330,20 @@
 kvirt/cluster/openshift/staticpods/mdns.yml
 kvirt/cluster/profiles/sample-kubeadm-default.yml
 kvirt/cluster/profiles/sample-openshift-compact.yml
 kvirt/cluster/profiles/sample-openshift-contrail.yml
 kvirt/cluster/profiles/sample-openshift-ipv6.yml
 kvirt/cluster/profiles/sample-openshift-sno-bm.yml
 kvirt/cluster/profiles/sample-openshift-sno.yml
-kvirt/common/Jenkinsfile.j2
 kvirt/common/__init__.py
 kvirt/common/autoscale.yaml.j2
 kvirt/common/fake_kubeconfig.json
 kvirt/common/ignition.j2
 kvirt/common/kubevirt_kcli_conf.j2
 kvirt/common/local_kcli_conf.j2
-kvirt/common/pipeline.yml.j2
-kvirt/common/pipeline_kube.yml.j2
-kvirt/common/playbook.j2
 kvirt/common/storage.sh.aws
 kvirt/common/storage.sh.gcp
 kvirt/common/storage.sh.ibmcloud
 kvirt/common/vm.ovf.j2
 kvirt/common/workflow.yml.j2
 kvirt/common/workflow_script.yml.j2
 kvirt/container/__init__.py
```

### Comparing `kcli-99.0.202405071430/kcli.egg-info/requires.txt` & `kcli-99.0.202405080912/kcli.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/ansibleutils/__init__.py` & `kcli-99.0.202405080912/kvirt/ansibleutils/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/baseconfig.py` & `kcli-99.0.202405080912/kvirt/baseconfig.py`

 * *Files 12% similar despite different names*

```diff
@@ -189,15 +189,14 @@
         defaults['placement'] = default.get('placement', kdefaults.PLACEMENT)
         defaults['yamlinventory'] = default.get('yamlinventory', kdefaults.YAMLINVENTORY)
         defaults['cpuhotplug'] = bool(default.get('cpuhotplug', kdefaults.CPUHOTPLUG))
         defaults['memoryhotplug'] = bool(default.get('memoryhotplug', kdefaults.MEMORYHOTPLUG))
         defaults['virttype'] = default.get('virttype', kdefaults.VIRTTYPE)
         defaults['tpm'] = default.get('tpm', kdefaults.TPM)
         defaults['rng'] = default.get('rng', kdefaults.RNG)
-        defaults['jenkinsmode'] = default.get('jenkinsmode', kdefaults.JENKINSMODE)
         defaults['vmuser'] = default.get('vmuser', kdefaults.VMUSER)
         defaults['vmport'] = default.get('vmport', kdefaults.VMPORT)
         defaults['vmrules'] = default.get('vmrules', kdefaults.VMRULES)
         defaults['vmrules_strict'] = default.get('vmrules_strict', kdefaults.VMRULES_STRICT)
         defaults['securitygroups'] = default.get('securitygroups', kdefaults.SECURITYGROUPS)
         defaults['rootpassword'] = default.get('rootpassword', kdefaults.ROOTPASSWORD)
         defaults['wait'] = default.get('wait', kdefaults.WAIT)
@@ -363,15 +362,14 @@
         self.cpuflags = options.get('cpuflags')
         self.cpupinning = options.get('cpupinning')
         self.numamode = options.get('numamode')
         self.numa = options.get('numa')
         self.pcidevices = options.get('pcidevices')
         self.tpm = options.get('tpm')
         self.rng = options.get('rng')
-        self.jenkinsmode = options.get('jenkinsmode')
         self.numcpus = options.get('numcpus')
         self.memory = options.get('memory')
         self.disks = options.get('disks')
         self.disksize = options.get('disksize')
         self.diskinterface = options.get('diskinterface')
         self.diskthin = options.get('diskthin')
         self.guestid = options.get('guestid')
@@ -1034,200 +1032,14 @@
     def delete_confpool(self, confpool, quiet=False):
         return self._delete_yaml_object(confpool, self.confpools, 'confpool', quiet=quiet)
 
     def update_confpool(self, confpool, overrides={}, quiet=False):
         return self._update_yaml_file(confpool, self.confpools, 'confpool', overrides=overrides, quiet=quiet,
                                       ignore_aliases=True)
 
-    def create_jenkins_pipeline(self, plan, inputfile, overrides={}, kube=False):
-        _type = 'plan'
-        if kube:
-            _type = 'generic'
-            plandir = os.path.dirname(kubeadm.create.__code__.co_filename)
-            if 'type' in overrides:
-                _type = overrides['type']
-                del overrides['type']
-                if _type == 'openshift':
-                    plandir = os.path.dirname(openshift.create.__code__.co_filename)
-                elif _type != 'generic':
-                    error(f"Incorrect kubernetes type {_type}. Choose between generic or openshift")
-                    sys.exit(1)
-                inputfile = f"{plandir}/ctlplanes.yml"
-        if 'jenkinsmode' in overrides:
-            jenkinsmode = overrides['jenkinsmode']
-            del overrides['jenkinsmode']
-        else:
-            jenkinsmode = self.jenkinsmode
-        if jenkinsmode not in ['docker', 'podman', 'kubernetes']:
-            error(f"Incorrect jenkins mode {self.jenkinsmode}. Choose between docker, podman or kubernetes")
-            sys.exit(1)
-        inputfile = os.path.expanduser(inputfile) if inputfile is not None else 'kcli_plan.yml'
-        basedir = os.path.dirname(inputfile)
-        if basedir == "":
-            basedir = '.'
-        if plan is None:
-            plan = os.path.basename(inputfile).replace('.yml', '').replace('.yaml', '')
-        if not os.path.exists(inputfile):
-            error("No input file found nor default kcli_plan.yml. Leaving....")
-            sys.exit(1)
-        parameters = {}
-        if os.path.exists(f"{basedir}/{plan}_default.yml"):
-            parameterfile = f"{basedir}/{plan}_default.yml"
-            parameters.update(common.get_parameters(parameterfile))
-        if os.path.exists(f"{basedir}/kcli_default.yml"):
-            parameterfile = f"{basedir}/kcli_default.yml"
-            parameters.update(common.get_parameters(parameterfile))
-        inputfile_default = "%s_default%s" % os.path.splitext(inputfile)
-        if os.path.exists(f"{basedir}/{inputfile_default}"):
-            parameterfile = f"{basedir}/{inputfile_default}"
-            parameters.update(common.get_parameters(parameterfile))
-        parameters.update(common.get_parameters(inputfile, planfile=True))
-        parameters.update(overrides)
-        jenkinsdir = os.path.dirname(common.__file__)
-        env = Environment(loader=FileSystemLoader(jenkinsdir), extensions=['jinja2.ext.do'], trim_blocks=True,
-                          lstrip_blocks=True)
-        for jinjafilter in jinjafilters.jinjafilters:
-            env.filters[jinjafilter] = jinjafilters.jinjafilters[jinjafilter]
-        try:
-            templ = env.get_template(os.path.basename("Jenkinsfile.j2"))
-        except TemplateSyntaxError as e:
-            error(f"Error rendering line {e.lineno} of file {e.filename}. Got: {e.message}")
-            sys.exit(1)
-        except TemplateError as e:
-            error(f"Error rendering file {inputfile}. Got: {e.message}")
-            sys.exit(1)
-        parameterline = " ".join(["-P %s=${params.%s}" % (parameter, parameter) for parameter in parameters])
-        jenkinsfile = templ.render(parameters=parameters, parameterline=parameterline, jenkinsmode=jenkinsmode,
-                                   _type=_type)
-        return jenkinsfile
-
-    def create_github_pipeline(self, plan, inputfile, paramfile=None, overrides={}, kube=False, script=False):
-        if not kube:
-            inputfile = os.path.expanduser(inputfile) if inputfile is not None else 'kcli_plan.yml'
-            basedir = os.path.dirname(inputfile)
-            if basedir == "":
-                basedir = '.'
-            if not os.path.exists(inputfile):
-                error("No input file found nor default kcli_plan.yml. Leaving....")
-                sys.exit(1)
-            if plan is None:
-                plan = os.path.basename(inputfile).replace('.yml', '').replace('.yaml', '')
-        else:
-            inputfile = None
-            if plan is None:
-                plan = 'myplan'
-        if 'plan' in overrides:
-            del overrides['plan']
-        runner = 'ubuntu-latest'
-        if 'runner' in overrides:
-            runner = overrides['runner']
-            del overrides['runner']
-        client = 'local'
-        if 'client' in overrides:
-            client = overrides['client']
-            del overrides['client']
-        kubetype = 'generic'
-        if kube:
-            if 'kubetype' in overrides:
-                kubetype = overrides['kubetype']
-                del overrides['kubetype']
-        runscript = 'true'
-        if script:
-            if 'runscript' in overrides:
-                runscript = str(overrides['runscript']).lower()
-                del overrides['runscript']
-        workflowdir = os.path.dirname(common.__file__)
-        env = Environment(loader=FileSystemLoader(workflowdir), extensions=['jinja2.ext.do'], trim_blocks=True,
-                          lstrip_blocks=True)
-        for jinjafilter in jinjafilters.jinjafilters:
-            env.filters[jinjafilter] = jinjafilters.jinjafilters[jinjafilter]
-        try:
-            workflowfile = "workflow_script.yml.j2" if script else "workflow.yml.j2"
-            templ = env.get_template(os.path.basename(workflowfile))
-        except TemplateSyntaxError as e:
-            error(f"Error rendering line {e.lineno} of file {e.filename}. Got: {e.message}")
-            sys.exit(1)
-        except TemplateError as e:
-            error(f"Error rendering file {inputfile}. Got: {e.message}")
-            sys.exit(1)
-        paramline = []
-        for parameter in overrides:
-            newparam = "%s" % parameter.upper()
-            paramline.append(f"-P {parameter}=${newparam}")
-        parameterline = " ".join(paramline)
-        paramfileline = "--paramfile $PARAMFILE" if paramfile is not None else ""
-        gitbase = os.popen('git rev-parse --show-prefix 2>/dev/null').read().strip()
-        workflowfile = templ.render(plan=plan, inputfile=inputfile, parameters=overrides, parameterline=parameterline,
-                                    paramfileline=paramfileline, paramfile=paramfile, gitbase=gitbase, runner=runner,
-                                    client=client, kube=kube, kubetype=kubetype, runscript=runscript)
-        return workflowfile
-
-    def create_tekton_pipeline(self, plan, inputfile, paramfile=None, overrides={}, kube=False):
-        if not kube:
-            inputfile = os.path.expanduser(inputfile) if inputfile is not None else 'kcli_plan.yml'
-            basedir = os.path.dirname(inputfile)
-            if basedir == "":
-                basedir = '.'
-            if not os.path.exists(inputfile):
-                error("No input file found nor default kcli_plan.yml. Leaving....")
-                sys.exit(1)
-            if plan is None:
-                plan = os.path.basename(inputfile).replace('.yml', '').replace('.yaml', '')
-        else:
-            inputfile = None
-            if plan is None:
-                plan = 'myplan'
-        if 'plan' in overrides:
-            del overrides['plan']
-        client = 'local'
-        if 'client' in overrides:
-            client = overrides['client']
-            del overrides['client']
-        kubetype = 'generic'
-        if kube:
-            if 'kubetype' in overrides:
-                kubetype = overrides['kubetype']
-                del overrides['kubetype']
-        workflowdir = os.path.dirname(common.__file__)
-        env = Environment(loader=FileSystemLoader(workflowdir), extensions=['jinja2.ext.do'], trim_blocks=True,
-                          lstrip_blocks=True)
-        for jinjafilter in jinjafilters.jinjafilters:
-            env.filters[jinjafilter] = jinjafilters.jinjafilters[jinjafilter]
-        try:
-            workflowfile = "pipeline_kube.yml.j2" if kube else "pipeline.yml.j2"
-            templ = env.get_template(os.path.basename(workflowfile))
-        except TemplateSyntaxError as e:
-            error(f"Error rendering line {e.lineno} of file {e.filename}. Got: {e.message}")
-            sys.exit(1)
-        except TemplateError as e:
-            error(f"Error rendering file {inputfile}. Got: {e.message}")
-            sys.exit(1)
-        paramline = []
-        for parameter in overrides:
-            paramline.append('-P %s="$%s"' % (parameter, parameter.upper()))
-        parameterline = " ".join(paramline)
-        giturl, gitbase = None, None
-        paramfileline = None
-        if kube:
-            paramfiledata = ''
-            if paramfile is not None:
-                paramfiledata = open(paramfile).read()
-                paramfileline = 'echo -ne """%s""" > kcli_parameters.yml' % paramfiledata
-                paramfileline = paramfileline.replace('\n', '\n      ')
-            if "pull_secret" not in paramfiledata and "pull_secret" not in overrides:
-                parameterline += " -P pull_secret=/home/tekton/.kcli/openshift_pull.json"
-        else:
-            paramfileline = "--paramfile $PARAMFILE" if paramfile is not None else ""
-            giturl = os.popen('git config --get remote.origin.url').read().strip()
-            gitbase = os.popen('git rev-parse --show-prefix 2>/dev/null').read().strip()
-        workflowfile = templ.render(plan=plan, inputfile=inputfile, parameters=overrides, parameterline=parameterline,
-                                    paramfileline=paramfileline, paramfile=paramfile, gitbase=gitbase, giturl=giturl,
-                                    client=client, kube=kube, kubetype=kubetype)
-        return workflowfile
-
     def info_kube_generic(self, quiet, web=False):
         plandir = os.path.dirname(kubeadm.create.__code__.co_filename)
         inputfile = f'{plandir}/ctlplanes.yml'
         self.info_plan(inputfile, quiet=quiet, web=web)
 
     def info_kube_hypershift(self, quiet, web=False):
         plandir = os.path.dirname(hypershift.create.__code__.co_filename)
@@ -1401,56 +1213,14 @@
         if store:
             pprint(f"Generating playbook_{hostname}.yml")
             with open(f"playbook_{hostname}.yml", 'w') as f:
                 f.write(playbookfile)
         else:
             print(playbookfile)
 
-    def create_playbook(self, inputfile, overrides={}, store=False):
-        playbookdir = os.path.dirname(common.__file__)
-        env = Environment(loader=FileSystemLoader(playbookdir), extensions=['jinja2.ext.do'],
-                          trim_blocks=True, lstrip_blocks=True)
-        for jinjafilter in jinjafilters.jinjafilters:
-            env.filters[jinjafilter] = jinjafilters.jinjafilters[jinjafilter]
-        inputfile = os.path.expanduser(inputfile) if inputfile is not None else 'kcli_plan.yml'
-        basedir = os.path.dirname(inputfile)
-        if basedir == "":
-            basedir = '.'
-        pprint(f"Using plan {inputfile}...")
-        pprint("Make sure to export ANSIBLE_JINJA2_EXTENSIONS=jinja2.ext.do")
-        jinjadir = os.path.dirname(jinjafilters.__file__)
-        if not os.path.exists('filter_plugins'):
-            pprint("Creating symlink to kcli jinja filters")
-            os.symlink(jinjadir, 'filter_plugins')
-        if not os.path.exists(inputfile):
-            error("No input file found nor default kcli_plan.yml. Leaving....")
-            sys.exit(1)
-        plan = 'xxx'
-        entries, overrides, basefile, basedir = self.process_inputfile(plan, inputfile, overrides=overrides, full=True)
-        config_data = {}
-        config_data['config_host'] = self.ini[self.client].get('host', '127.0.0.1')
-        config_data['config_type'] = config_data.get('config_type', 'kvm')
-        default_user = getuser() if config_data['config_type'] == 'kvm'\
-            and config_data['config_host'] in ['localhost', '127.0.0.1'] else 'root'
-        config_data['config_user'] = config_data.get('config_user', default_user)
-        overrides.update(config_data)
-        renderfile = self.process_inputfile(plan, inputfile, overrides=overrides, onfly=False, ignore=True)
-        try:
-            data = yaml.safe_load(renderfile)
-        except:
-            error("Couldnt' parse plan. Leaving....")
-            sys.exit(1)
-        for key in data:
-            if 'type' in data[key] and data[key]['type'] != 'kvm':
-                continue
-            elif 'scripts' not in data[key] and 'files' not in data[key] and 'cmds' not in data[key]:
-                continue
-            else:
-                self.create_vm_playbook(key, data[key], overrides=overrides, store=store, env=env)
-
     def create_plan_template(self, directory, overrides, skipfiles=False, skipscripts=False):
         pprint(f"Creating plan template in {directory}...")
         if container_mode():
             directory = f"/workdir/{directory}"
         if not os.path.exists(directory):
             os.makedirs(directory)
             os.makedirs(f"{directory}/scripts")
```

### Comparing `kcli-99.0.202405071430/kvirt/bottle.py` & `kcli-99.0.202405080912/kvirt/bottle.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cli.py` & `kcli-99.0.202405080912/kvirt/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -2131,26 +2131,14 @@
                          overrides=overrides, pre=pre, post=post, threaded=threaded)
     if result and 'reason' in result:
         error(result['reason'])
     code = 0 if result and result.get('result') == 'success' else 1
     sys.exit(code)
 
 
-def create_playbook(args):
-    store = args.store
-    overrides = handle_parameters(args.param, args.paramfile)
-    inputfile = overrides.get('inputfile') or args.inputfile or 'kcli_plan.yml'
-    if container_mode():
-        inputfile = f"/workdir/{inputfile}"
-    baseconfig = Kbaseconfig(client=args.client, debug=args.debug)
-    _type = baseconfig.ini[baseconfig.client].get('type', 'kvm')
-    overrides.update({'type': _type})
-    baseconfig.create_playbook(inputfile, overrides=overrides, store=store)
-
-
 def update_plan(args):
     plan = args.plan
     url = args.url
     path = args.path
     container = args.container
     overrides = handle_parameters(args.param, args.paramfile)
     autostart = overrides.get('autostart', False)
@@ -2501,57 +2489,14 @@
 
 def download_openshift_installer(args):
     overrides = handle_parameters(args.param, args.paramfile)
     baseconfig = Kbaseconfig(client=args.client, debug=args.debug, offline=True)
     return baseconfig.download_openshift_installer(overrides)
 
 
-def create_pipeline_github(args):
-    plan = args.plan
-    kube = args.kube
-    script = args.script
-    overrides = handle_parameters(args.param, args.paramfile)
-    inputfile = overrides.get('inputfile') or args.inputfile or 'kcli_plan.yml'
-    if container_mode():
-        inputfile = f"/workdir/{inputfile}"
-    paramfile = args.paramfile[0] if args.paramfile else None
-    baseconfig = Kbaseconfig(client=args.client, debug=args.debug)
-    renderfile = baseconfig.create_github_pipeline(plan, inputfile, paramfile=paramfile, overrides=overrides,
-                                                   kube=kube, script=script)
-    print(renderfile)
-
-
-def create_pipeline_jenkins(args):
-    plan = args.plan
-    kube = args.kube
-    overrides = handle_parameters(args.param, args.paramfile)
-    inputfile = overrides.get('inputfile') or args.inputfile or 'kcli_plan.yml'
-    if container_mode():
-        inputfile = f"/workdir/{inputfile}"
-    baseconfig = Kbaseconfig(client=args.client, debug=args.debug)
-    if not kube and not os.path.exists(inputfile):
-        error(f"Input file {inputfile} not found")
-        sys.exit(1)
-    renderfile = baseconfig.create_jenkins_pipeline(plan, inputfile, overrides=overrides, kube=kube)
-    print(renderfile)
-
-
-def create_pipeline_tekton(args):
-    overrides = handle_parameters(args.param, args.paramfile)
-    inputfile = overrides.get('inputfile') or args.inputfile or 'kcli_plan.yml'
-    if container_mode():
-        inputfile = f"/workdir/{inputfile}"
-    paramfile = args.paramfile[0] if args.paramfile else None
-    kube = args.kube
-    plan = args.plan
-    baseconfig = Kbaseconfig(client=args.client, debug=args.debug)
-    renderfile = baseconfig.create_tekton_pipeline(plan, inputfile, paramfile=paramfile, overrides=overrides, kube=kube)
-    print(renderfile)
-
-
 def render_file(args):
     plan = None
     ignore = args.ignore
     overrides = {}
     allparamfiles = [paramfile for paramfile in glob("*_default.y*ml")]
     for paramfile in allparamfiles:
         overrides.update(common.get_overrides(paramfile=paramfile))
@@ -3936,49 +3881,14 @@
     openshiftsnocreate_parser.add_argument('-t', '--threaded', help='Run threaded', action='store_true')
     openshiftsnocreate_parser.add_argument('cluster', metavar='CLUSTER', nargs='?', type=valid_cluster)
     openshiftsnocreate_parser.set_defaults(func=create_openshift_sno)
     create_subparsers.add_parser('openshift-sno', parents=[openshiftsnocreate_parser],
                                  description=openshiftsnocreate_desc, help=openshiftsnocreate_desc,
                                  epilog=openshiftsnocreate_epilog, formatter_class=rawhelp)
 
-    pipelinecreate_desc = 'Create Pipeline'
-    pipelinecreate_parser = create_subparsers.add_parser('pipeline', description=pipelinecreate_desc,
-                                                         help=pipelinecreate_desc)
-    pipelinecreate_subparsers = pipelinecreate_parser.add_subparsers(metavar='', dest='subcommand_create_pipeline')
-
-    githubpipelinecreate_desc = 'Create Github Pipeline'
-    githubpipelinecreate_parser = pipelinecreate_subparsers.add_parser('github', description=githubpipelinecreate_desc,
-                                                                       parents=[parent_parser],
-                                                                       help=githubpipelinecreate_desc, aliases=['gha'])
-    githubpipelinecreate_parser.add_argument('-f', '--inputfile', help='Input Plan (or script) file')
-    githubpipelinecreate_parser.add_argument('-k', '--kube', action='store_true', help='Create kube pipeline')
-    githubpipelinecreate_parser.add_argument('-s', '--script', action='store_true', help='Create script pipeline')
-    githubpipelinecreate_parser.add_argument('plan', metavar='PLAN', nargs='?')
-    githubpipelinecreate_parser.set_defaults(func=create_pipeline_github)
-
-    jenkinspipelinecreate_desc = 'Create Jenkins Pipeline'
-    jenkinspipelinecreate_parser = pipelinecreate_subparsers.add_parser('jenkins',
-                                                                        description=jenkinspipelinecreate_desc,
-                                                                        parents=[parent_parser],
-                                                                        help=jenkinspipelinecreate_desc)
-    jenkinspipelinecreate_parser.add_argument('-f', '--inputfile', help='Input Plan file')
-    jenkinspipelinecreate_parser.add_argument('-k', '--kube', action='store_true', help='Create kube pipeline')
-    jenkinspipelinecreate_parser.add_argument('plan', metavar='PLAN', nargs='?')
-    jenkinspipelinecreate_parser.set_defaults(func=create_pipeline_jenkins)
-
-    tektonpipelinecreate_desc = 'Create Tekton Pipeline'
-    tektonpipelinecreate_parser = pipelinecreate_subparsers.add_parser('tekton',
-                                                                       description=tektonpipelinecreate_desc,
-                                                                       parents=[parent_parser],
-                                                                       help=tektonpipelinecreate_desc)
-    tektonpipelinecreate_parser.add_argument('-f', '--inputfile', help='Input Plan file')
-    tektonpipelinecreate_parser.add_argument('-k', '--kube', action='store_true', help='Create kube pipeline')
-    tektonpipelinecreate_parser.add_argument('plan', metavar='PLAN', nargs='?')
-    tektonpipelinecreate_parser.set_defaults(func=create_pipeline_tekton)
-
     plancreate_desc = 'Create Plan'
     plancreate_epilog = f"examples:\n{examples.plancreate}"
     plancreate_parser = create_subparsers.add_parser('plan', description=plancreate_desc, help=plancreate_desc,
                                                      parents=[parent_parser], epilog=plancreate_epilog,
                                                      formatter_class=rawhelp)
     plancreate_parser.add_argument('-A', '--ansible', help='Generate ansible inventory', action='store_true')
     plancreate_parser.add_argument('-u', '--url', help='Url for plan', metavar='URL', type=valid_url)
@@ -4018,21 +3928,14 @@
     plansnapshotcreate_parser = create_subparsers.add_parser('plan-snapshot', description=plansnapshotcreate_desc,
                                                              help=plansnapshotcreate_desc)
 
     plansnapshotcreate_parser.add_argument('-p', '--plan', help='plan name', required=True, metavar='PLAN')
     plansnapshotcreate_parser.add_argument('snapshot', metavar='SNAPSHOT')
     plansnapshotcreate_parser.set_defaults(func=create_snapshot_plan)
 
-    playbookcreate_desc = 'Create playbook from plan'
-    playbookcreate_parser = create_subparsers.add_parser('playbook', description=playbookcreate_desc,
-                                                         help=playbookcreate_desc, parents=[parent_parser])
-    playbookcreate_parser.add_argument('-f', '--inputfile', help='Input Plan/File', default='kcli_plan.yml')
-    playbookcreate_parser.add_argument('-s', '--store', action='store_true', help="Store results in files")
-    playbookcreate_parser.set_defaults(func=create_playbook)
-
     poolcreate_desc = 'Create Pool'
     poolcreate_parser = create_subparsers.add_parser('pool', description=poolcreate_desc, help=poolcreate_desc)
     poolcreate_parser.add_argument('-f', '--full', action='store_true')
     poolcreate_parser.add_argument('-t', '--pooltype', help='Type of the pool', choices=('dir', 'lvm', 'zfs'),
                                    default='dir')
     poolcreate_parser.add_argument('-p', '--path', help='Path of the pool', metavar='PATH')
     poolcreate_parser.add_argument('--thinpool', help='Existing thin pool to use with lvm', metavar='THINPOOL')
```

### Comparing `kcli-99.0.202405071430/kvirt/cluster/aks/__init__.py` & `kcli-99.0.202405080912/kvirt/cluster/aks/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/eks/__init__.py` & `kcli-99.0.202405080912/kvirt/cluster/eks/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/gke/__init__.py` & `kcli-99.0.202405080912/kvirt/cluster/gke/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/hypershift/99-apps.yaml` & `kcli-99.0.202405080912/kvirt/cluster/hypershift/99-apps.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/hypershift/99-forcedns` & `kcli-99.0.202405080912/kvirt/cluster/hypershift/99-forcedns`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/hypershift/99-notifications.yaml` & `kcli-99.0.202405080912/kvirt/cluster/hypershift/99-notifications.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/hypershift/Corefile` & `kcli-99.0.202405080912/kvirt/cluster/hypershift/Corefile`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/hypershift/__init__.py` & `kcli-99.0.202405080912/kvirt/cluster/hypershift/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/hypershift/assisted_infra.yml` & `kcli-99.0.202405080912/kvirt/cluster/hypershift/assisted_infra.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/hypershift/assisted_ingress.yml` & `kcli-99.0.202405080912/kvirt/cluster/hypershift/assisted_ingress.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/hypershift/autoapprovercron.yml` & `kcli-99.0.202405080912/kvirt/cluster/hypershift/autoapprovercron.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/hypershift/bmc.yml.j2` & `kcli-99.0.202405080912/kvirt/cluster/hypershift/bmc.yml.j2`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/hypershift/calico.sh.j2` & `kcli-99.0.202405080912/kvirt/cluster/hypershift/calico.sh.j2`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/hypershift/cilium.sh.j2` & `kcli-99.0.202405080912/kvirt/cluster/hypershift/cilium.sh.j2`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/hypershift/disconnected.sh` & `kcli-99.0.202405080912/kvirt/cluster/hypershift/disconnected.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/hypershift/extras.sh` & `kcli-99.0.202405080912/kvirt/cluster/hypershift/extras.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/hypershift/hostedcluster.yaml` & `kcli-99.0.202405080912/kvirt/cluster/hypershift/hostedcluster.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/hypershift/httpd.yaml` & `kcli-99.0.202405080912/kvirt/cluster/hypershift/httpd.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/hypershift/ignition.sh` & `kcli-99.0.202405080912/kvirt/cluster/hypershift/ignition.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/hypershift/kcli_plan.yml` & `kcli-99.0.202405080912/kvirt/cluster/hypershift/kcli_plan.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/hypershift/kcli_plan_default.yml` & `kcli-99.0.202405080912/kvirt/cluster/hypershift/kcli_plan_default.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/hypershift/nmstateconfig.yml.j2` & `kcli-99.0.202405080912/kvirt/cluster/hypershift/nmstateconfig.yml.j2`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/hypershift/nodepool.yaml` & `kcli-99.0.202405080912/kvirt/cluster/hypershift/nodepool.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/hypershift/staticpods/coredns.yml` & `kcli-99.0.202405080912/kvirt/cluster/hypershift/staticpods/coredns.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/hypershift/staticpods/keepalived.yml` & `kcli-99.0.202405080912/kvirt/cluster/hypershift/staticpods/keepalived.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/hypershift/staticpods/mdns.yml` & `kcli-99.0.202405080912/kvirt/cluster/hypershift/staticpods/mdns.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/k3s/__init__.py` & `kcli-99.0.202405080912/kvirt/cluster/k3s/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/k3s/bootstrap.sh` & `kcli-99.0.202405080912/kvirt/cluster/k3s/bootstrap.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/k3s/bootstrap.yml` & `kcli-99.0.202405080912/kvirt/cluster/k3s/bootstrap.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/k3s/ctlplanes.sh` & `kcli-99.0.202405080912/kvirt/cluster/k3s/ctlplanes.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/k3s/ctlplanes.yml` & `kcli-99.0.202405080912/kvirt/cluster/k3s/ctlplanes.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/k3s/kcli_default.yml` & `kcli-99.0.202405080912/kvirt/cluster/k3s/kcli_default.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/k3s/workers.yml` & `kcli-99.0.202405080912/kvirt/cluster/k3s/workers.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/kubeadm/__init__.py` & `kcli-99.0.202405080912/kvirt/cluster/kubeadm/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/argocd/install.sh` & `kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/argocd/install.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/dashboard/install.sh` & `kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/dashboard/install.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/falco/install.sh` & `kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/falco/install.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/istio/istio-minimal-operator.yaml` & `kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/istio/istio-minimal-operator.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/katacontainer/install.sh` & `kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/katacontainer/install.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/katacontainer/uninstall.sh` & `kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/katacontainer/uninstall.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/kubevirt/install.sh` & `kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/kubevirt/install.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/metallb/install.sh` & `kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/metallb/install.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/metallb/metallb_advertisement.yml` & `kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/metallb/metallb_advertisement.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/rancher/install.sh` & `kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/rancher/install.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/kubeadm/apps/rook/install.sh` & `kcli-99.0.202405080912/kvirt/cluster/kubeadm/apps/rook/install.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/kubeadm/bootstrap.sh` & `kcli-99.0.202405080912/kvirt/cluster/kubeadm/bootstrap.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/kubeadm/bootstrap.yml` & `kcli-99.0.202405080912/kvirt/cluster/kubeadm/bootstrap.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/kubeadm/ctlplanes.yml` & `kcli-99.0.202405080912/kvirt/cluster/kubeadm/ctlplanes.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/kubeadm/join.sh` & `kcli-99.0.202405080912/kvirt/cluster/kubeadm/join.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/kubeadm/kcli_default.yml` & `kcli-99.0.202405080912/kvirt/cluster/kubeadm/kcli_default.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/kubeadm/keepalived.conf` & `kcli-99.0.202405080912/kvirt/cluster/kubeadm/keepalived.conf`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/kubeadm/nfs.sh` & `kcli-99.0.202405080912/kvirt/cluster/kubeadm/nfs.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/kubeadm/pre_el.sh` & `kcli-99.0.202405080912/kvirt/cluster/kubeadm/pre_el.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/kubeadm/pre_ubuntu.sh` & `kcli-99.0.202405080912/kvirt/cluster/kubeadm/pre_ubuntu.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/kubeadm/registry.yml` & `kcli-99.0.202405080912/kvirt/cluster/kubeadm/registry.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/kubeadm/workers.yml` & `kcli-99.0.202405080912/kvirt/cluster/kubeadm/workers.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/kubecommon/__init__.py` & `kcli-99.0.202405080912/kvirt/cluster/kubecommon/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/kubernetes/__init__.py` & `kcli-99.0.202405080912/kvirt/cluster/kubernetes/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/microshift/__init__.py` & `kcli-99.0.202405080912/kvirt/cluster/microshift/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/microshift/kcli_plan.yml` & `kcli-99.0.202405080912/kvirt/cluster/microshift/kcli_plan.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/microshift/kcli_plan_default.yml` & `kcli-99.0.202405080912/kvirt/cluster/microshift/kcli_plan_default.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/microshift/scripts/01_clients.sh` & `kcli-99.0.202405080912/kvirt/cluster/microshift/scripts/01_clients.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/microshift/scripts/03_microshift.sh` & `kcli-99.0.202405080912/kvirt/cluster/microshift/scripts/03_microshift.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/microshift/scripts/05_acm.sh` & `kcli-99.0.202405080912/kvirt/cluster/microshift/scripts/05_acm.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/microshift/scripts/deploy.sh` & `kcli-99.0.202405080912/kvirt/cluster/microshift/scripts/deploy.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/10-node-ip-hint.yaml` & `kcli-99.0.202405080912/kvirt/cluster/openshift/10-node-ip-hint.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/20-localhost-fix.yaml` & `kcli-99.0.202405080912/kvirt/cluster/openshift/20-localhost-fix.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/99-apps.yaml` & `kcli-99.0.202405080912/kvirt/cluster/openshift/99-apps.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/99-autologin.yaml` & `kcli-99.0.202405080912/kvirt/cluster/openshift/99-autologin.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/99-bootstrap-deletion-2.yaml` & `kcli-99.0.202405080912/kvirt/cluster/openshift/99-bootstrap-deletion-2.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/99-bootstrap-deletion.yaml` & `kcli-99.0.202405080912/kvirt/cluster/openshift/99-bootstrap-deletion.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/99-chrony.yaml` & `kcli-99.0.202405080912/kvirt/cluster/openshift/99-chrony.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/99-forcedns` & `kcli-99.0.202405080912/kvirt/cluster/openshift/99-forcedns`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/99-kubevirt-fix.yaml` & `kcli-99.0.202405080912/kvirt/cluster/openshift/99-kubevirt-fix.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/99-notifications.yaml` & `kcli-99.0.202405080912/kvirt/cluster/openshift/99-notifications.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/99-sno.yaml` & `kcli-99.0.202405080912/kvirt/cluster/openshift/99-sno.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/Corefile` & `kcli-99.0.202405080912/kvirt/cluster/openshift/Corefile`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/__init__.py` & `kcli-99.0.202405080912/kvirt/cluster/openshift/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/apps/advanced-cluster-management/assisted-service.sample.yml` & `kcli-99.0.202405080912/kvirt/cluster/openshift/apps/advanced-cluster-management/assisted-service.sample.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/apps/advanced-cluster-management/assisted-service.sh` & `kcli-99.0.202405080912/kvirt/cluster/openshift/apps/advanced-cluster-management/assisted-service.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/apps/advanced-cluster-management/gen_registries.py` & `kcli-99.0.202405080912/kvirt/cluster/openshift/apps/advanced-cluster-management/gen_registries.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/apps/advanced-cluster-management/post.sh` & `kcli-99.0.202405080912/kvirt/cluster/openshift/apps/advanced-cluster-management/post.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/apps/argocd/configmap.yml` & `kcli-99.0.202405080912/kvirt/cluster/openshift/apps/argocd/configmap.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/apps/argocd/install.sh` & `kcli-99.0.202405080912/kvirt/cluster/openshift/apps/argocd/install.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/apps/autolabeller/cr.yml` & `kcli-99.0.202405080912/kvirt/cluster/openshift/apps/autolabeller/cr.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/apps/autolabeller/install.yml` & `kcli-99.0.202405080912/kvirt/cluster/openshift/apps/autolabeller/install.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/apps/cluster-logging/cr.yml` & `kcli-99.0.202405080912/kvirt/cluster/openshift/apps/cluster-logging/cr.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/apps/install.yml.j2` & `kcli-99.0.202405080912/kvirt/cluster/openshift/apps/install.yml.j2`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/apps/kubevirt-hyperconverged/cr.yml` & `kcli-99.0.202405080912/kvirt/cluster/openshift/apps/kubevirt-hyperconverged/cr.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/apps/local-storage-operator/cr.yml` & `kcli-99.0.202405080912/kvirt/cluster/openshift/apps/local-storage-operator/cr.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/apps/local-storage-operator/post.sh` & `kcli-99.0.202405080912/kvirt/cluster/openshift/apps/local-storage-operator/post.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/apps/lvms-operator/cr.yml` & `kcli-99.0.202405080912/kvirt/cluster/openshift/apps/lvms-operator/cr.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/apps/lvms-operator/post.sh` & `kcli-99.0.202405080912/kvirt/cluster/openshift/apps/lvms-operator/post.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/apps/metallb-operator/cr.yml` & `kcli-99.0.202405080912/kvirt/cluster/openshift/apps/metallb-operator/cr.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/apps/multicluster-engine/assisted-service.sample.yml` & `kcli-99.0.202405080912/kvirt/cluster/openshift/apps/multicluster-engine/assisted-service.sample.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/apps/multicluster-engine/assisted-service.sh` & `kcli-99.0.202405080912/kvirt/cluster/openshift/apps/multicluster-engine/assisted-service.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/apps/multicluster-engine/gen_registries.py` & `kcli-99.0.202405080912/kvirt/cluster/openshift/apps/multicluster-engine/gen_registries.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/apps/nfs/install.sh` & `kcli-99.0.202405080912/kvirt/cluster/openshift/apps/nfs/install.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/apps/odf-operator/cr.yml` & `kcli-99.0.202405080912/kvirt/cluster/openshift/apps/odf-operator/cr.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/apps/odf-operator/post.sh` & `kcli-99.0.202405080912/kvirt/cluster/openshift/apps/odf-operator/post.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/apps/odf-operator/pre.sh` & `kcli-99.0.202405080912/kvirt/cluster/openshift/apps/odf-operator/pre.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/apps/users/install.sh` & `kcli-99.0.202405080912/kvirt/cluster/openshift/apps/users/install.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/autoapprovercron.yml` & `kcli-99.0.202405080912/kvirt/cluster/openshift/autoapprovercron.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/autorules.yml` & `kcli-99.0.202405080912/kvirt/cluster/openshift/autorules.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/bootstrap.yml` & `kcli-99.0.202405080912/kvirt/cluster/openshift/bootstrap.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/cilium.sh.j2` & `kcli-99.0.202405080912/kvirt/cluster/openshift/cilium.sh.j2`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/cloud_bootstrap.yml` & `kcli-99.0.202405080912/kvirt/cluster/openshift/cloud_bootstrap.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/cloud_ctlplanes.yml` & `kcli-99.0.202405080912/kvirt/cluster/openshift/cloud_ctlplanes.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/cloud_workers.yml` & `kcli-99.0.202405080912/kvirt/cluster/openshift/cloud_workers.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/ctlplanes.yml` & `kcli-99.0.202405080912/kvirt/cluster/openshift/ctlplanes.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/customisation/99-autoapprovercron-cronjob.yaml` & `kcli-99.0.202405080912/kvirt/cluster/openshift/customisation/99-autoapprovercron-cronjob.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/customisation/99-iptables.yaml` & `kcli-99.0.202405080912/kvirt/cluster/openshift/customisation/99-iptables.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/dhcp.yml` & `kcli-99.0.202405080912/kvirt/cluster/openshift/dhcp.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/disconnected/haproxy.cfg` & `kcli-99.0.202405080912/kvirt/cluster/openshift/disconnected/haproxy.cfg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/disconnected/scripts/03_mirror.sh` & `kcli-99.0.202405080912/kvirt/cluster/openshift/disconnected/scripts/03_mirror.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/disconnected/scripts/03_registry.sh` & `kcli-99.0.202405080912/kvirt/cluster/openshift/disconnected/scripts/03_registry.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/disconnected/scripts/05_olm.sh` & `kcli-99.0.202405080912/kvirt/cluster/openshift/disconnected/scripts/05_olm.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/disconnected/scripts/deploy.sh` & `kcli-99.0.202405080912/kvirt/cluster/openshift/disconnected/scripts/deploy.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/disconnected/scripts/mirror-config.yaml.sample` & `kcli-99.0.202405080912/kvirt/cluster/openshift/disconnected/scripts/mirror-config.yaml.sample`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/disconnected.yml` & `kcli-99.0.202405080912/kvirt/cluster/openshift/disconnected.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/fake_kubeconfig.json` & `kcli-99.0.202405080912/kvirt/cluster/openshift/fake_kubeconfig.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/haproxy.cfg` & `kcli-99.0.202405080912/kvirt/cluster/openshift/haproxy.cfg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/haproxy.cfg.kubevirt` & `kcli-99.0.202405080912/kvirt/cluster/openshift/haproxy.cfg.kubevirt`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/httpd.yaml` & `kcli-99.0.202405080912/kvirt/cluster/openshift/httpd.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/ignition.j2` & `kcli-99.0.202405080912/kvirt/cluster/openshift/ignition.j2`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/install-config.yaml` & `kcli-99.0.202405080912/kvirt/cluster/openshift/install-config.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/iso.sh` & `kcli-99.0.202405080912/kvirt/cluster/openshift/iso.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/kcli_default.yml` & `kcli-99.0.202405080912/kvirt/cluster/openshift/kcli_default.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/keepalived.conf` & `kcli-99.0.202405080912/kvirt/cluster/openshift/keepalived.conf`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/relocate-ip.sh` & `kcli-99.0.202405080912/kvirt/cluster/openshift/relocate-ip.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/sno-finish.sh` & `kcli-99.0.202405080912/kvirt/cluster/openshift/sno-finish.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/sno.yml` & `kcli-99.0.202405080912/kvirt/cluster/openshift/sno.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/sno_default.yml` & `kcli-99.0.202405080912/kvirt/cluster/openshift/sno_default.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/staticpods/coredns.yml` & `kcli-99.0.202405080912/kvirt/cluster/openshift/staticpods/coredns.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/staticpods/haproxy.yml` & `kcli-99.0.202405080912/kvirt/cluster/openshift/staticpods/haproxy.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/staticpods/keepalived.yml` & `kcli-99.0.202405080912/kvirt/cluster/openshift/staticpods/keepalived.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/staticpods/mdns.yml` & `kcli-99.0.202405080912/kvirt/cluster/openshift/staticpods/mdns.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/cluster/openshift/workers.yml` & `kcli-99.0.202405080912/kvirt/cluster/openshift/workers.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/common/__init__.py` & `kcli-99.0.202405080912/kvirt/common/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/common/autoscale.yaml.j2` & `kcli-99.0.202405080912/kvirt/common/autoscale.yaml.j2`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/common/fake_kubeconfig.json` & `kcli-99.0.202405080912/kvirt/common/fake_kubeconfig.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/common/ignition.j2` & `kcli-99.0.202405080912/kvirt/common/ignition.j2`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/common/pipeline.yml.j2` & `kcli-99.0.202405080912/kvirt/common/workflow.yml.j2`

 * *Files 27% similar despite different names*

```diff
@@ -1,134 +1,78 @@
-apiVersion: tekton.dev/v1beta1
-kind: Task
-metadata:
- name: kcli-plan-{{ plan }}
-spec:
- params:
- - name: plan
-   description: plan
-   type: string
-   default: "{{ plan }}"
- - name: inputfile
-   description: inputfile
-   type: string
-   default: "{{ gitbase + inputfile }}"
- - name: url
-   description: url
-   type: string
-   default: "{{ giturl }}"
- - name: commit
-   description: commit
-   type: string
-   default: "main"
-{% if paramfile != None %}
- - name: paramfile
-   type: string
-   default: "{{ paramfile }}"
-{% endif %}
-{% for param in parameters %}
- - name: {{ param }}
-   description: {{ param }}
-   type: string
-   default: "{{ parameters[param] }}"
-{% endfor %}
- steps:
-  - name: git-clone
-    image: "gcr.io/tekton-releases/github.com/tektoncd/pipeline/cmd/git-init:v0.21.0"
-    env:
-    - name: URL
-      value: $(params.url)
-    - name: COMMIT
-      value: $(params.commit)
-    script: |
-     #!/usr/bin/env sh
-     cd /source
-     git clone $URL .
-     git checkout $COMMIT
-    volumeMounts:
-    - mountPath: /source
-      name: git-source
-  - name: deploy
-    image: "quay.io/karmab/kcli:latest"
-    env:
-    - name: PLAN
-      value: $(params.plan)
-    - name: INPUTFILE
-      value: $(params.inputfile)
-{% if paramfile != None %}
-    - name: PARAMFILE
-      value: $(params.paramfile)
+name: {{ plan }} 
+on:
+  workflow_dispatch:
+    inputs:
+      RUNNER:
+        description: 'Runner Name'
+        required: true
+        default: '{{ runner }}'
+      CLIENT:
+        description: 'Client name'
+        required: true
+        default: '{{ client }}'
+      PLAN:
+        description: 'Plan Name'
+        required: true
+        default: {{ plan }}
+{% if not kube %}
+      INPUTFILE:
+        description: 'Input file'
+        required: true
+        default: {{ gitbase + inputfile }}
 {% endif %}
-{% for param in parameters %}
-    - name: {{ param|upper }}
-      value: $(params.{{ param }})
-{% endfor %}
-    - name: PYTHONUNBUFFERED
-      value: "true"
-    script: |
-     #!/usr/bin/env bash
-     cd /source
-     echo kcli create plan --force $INPUTFILE {{ paramfileline }} {{ parameterline }} $PLAN
-     kcli create plan --force -f $INPUTFILE {{ paramfileline }} {{ parameterline }} $PLAN
-    volumeMounts:
-    - mountPath: /home/tekton/.kcli
-      name: kcli-config
-    - mountPath: /source
-      name: git-source
- volumes:
- - configMap:
-     defaultMode: 0700
-     name: kcli-config
-   name: kcli-config
- - name: git-source
-   emptyDir: {}
----
-apiVersion: tekton.dev/v1beta1
-kind: Pipeline
-metadata:
-  name: kcli-plan-{{ plan }}
-spec:
-  description: deploy plan {{ plan }}
-  params:
-  - name: plan
-    type: string
-    default: "{{ plan }}"
-  - name: inputfile
-    type: string
-    default: "{{ gitbase + inputfile }}"
 {% if paramfile != None %}
-  - name: paramfile
-    type: string
-    default: "{{ paramfile }}"
+      PARAMFILE:
+        description: 'paramfile'
+        required: false
+        default: {{ gitbase + paramfile }}
 {% endif %}
-  - name: commit
-    type: string
-    default: "main"
-{% if parameters %}
-{% for param in parameters %}
-  - name: {{ param }}
-    description: {{ param }}
-    type: string
-    default: "{{ parameters[param] }}"
+{% for parameter in parameters %}
+      {{ parameter|upper }}:
+        description: '{{ parameter }}'
+        required: false
+        default: {{ parameters[parameter] }}
 {% endfor %}
+
+env:
+ HOME: {{ parameters['home']|default('/root') }}
+ CLIENT: {% raw %}${{github.event.inputs.CLIENT}}{% endraw %}
+
+{% if not kube %}
+ INPUTFILE: {% raw %}${{github.event.inputs.INPUTFILE}}{% endraw %}
+
 {% endif %}
-  tasks:
-  - name: kcli-plan-{{ plan }}
-    taskRef:
-      name: kcli-plan-{{ plan }}
-    params:
-    - name: plan
-      value: $(params.plan)
-    - name: inputfile
-      value: $(params.inputfile)
 {% if paramfile != None %}
-    - name: paramfile
-      value: $(params.paramfile)
+ PARAMFILE: {% raw %}${{github.event.inputs.PARAMFILE}}{% endraw %}
+
 {% endif %}
-    - name: url
-      value: {{ giturl }}
-    - name: commit
-      value: $(params.commit)
-{% for param in parameters %}
-    - name: {{ param }}
-      value: $(params.{{ param }})
+{% for parameter in parameters %}
+ {{ parameter|upper }}: {% raw %}${{github.event.inputs.{% endraw %}{{ parameter|upper}}{% raw %}}}{% endraw %}
+
 {% endfor %}
+
+jobs:
+    requirements:
+      runs-on: {% raw %}${{github.event.inputs.RUNNER}}{% endraw %}
+
+
+      steps:
+       - uses: actions/checkout@v2
+       - run: git pull origin ${GITHUB_REF##*/}
+       - name: Install kcli
+         run: |
+           curl https://raw.githubusercontent.com/karmab/kcli/main/install.sh | bash
+           # kcli create pool -p /var/lib/libvirt/images default
+           # sudo setfacl -m u:$(id -un):rwx /var/lib/libvirt/images
+
+    deploy-plan:
+      needs: requirements
+      runs-on: {% raw %}${{github.event.inputs.RUNNER}}{% endraw %}
+  
+      steps:
+{% if kube %}
+       - name: Deploy kcli cluster
+         run: kcli -C $CLIENT create cluster {{ kubetype }} --force {{ paramfileline }} {{ parameterline }} $PLAN
+{% else %}
+       - name: Deploy kcli plan
+         run: kcli -C $CLIENT create plan --force -f $INPUTFILE {{ paramfileline }} {{ parameterline }} $PLAN
+{% endif %}
```

### Comparing `kcli-99.0.202405071430/kvirt/common/storage.sh.aws` & `kcli-99.0.202405080912/kvirt/common/storage.sh.aws`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/common/storage.sh.gcp` & `kcli-99.0.202405080912/kvirt/common/storage.sh.gcp`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/common/vm.ovf.j2` & `kcli-99.0.202405080912/kvirt/common/vm.ovf.j2`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/common/workflow.yml.j2` & `kcli-99.0.202405080912/kvirt/common/workflow_script.yml.j2`

 * *Files 14% similar despite different names*

```diff
@@ -6,24 +6,22 @@
         description: 'Runner Name'
         required: true
         default: '{{ runner }}'
       CLIENT:
         description: 'Client name'
         required: true
         default: '{{ client }}'
-      PLAN:
-        description: 'Plan Name'
+      SCRIPT:
+        description: 'Run script'
         required: true
-        default: {{ plan }}
-{% if not kube %}
-      INPUTFILE:
-        description: 'Input file'
+        default: '{{ gitbase + inputfile }}'
+      RUN_SCRIPT:
+        description: 'Run script'
         required: true
-        default: {{ gitbase + inputfile }}
-{% endif %}
+        default: '{{ runscript }}'
 {% if paramfile != None %}
       PARAMFILE:
         description: 'paramfile'
         required: false
         default: {{ gitbase + paramfile }}
 {% endif %}
 {% for parameter in parameters %}
@@ -33,18 +31,18 @@
         default: {{ parameters[parameter] }}
 {% endfor %}
 
 env:
  HOME: {{ parameters['home']|default('/root') }}
  CLIENT: {% raw %}${{github.event.inputs.CLIENT}}{% endraw %}
 
-{% if not kube %}
- INPUTFILE: {% raw %}${{github.event.inputs.INPUTFILE}}{% endraw %}
+ SCRIPT: {% raw %}${{github.event.inputs.SCRIPT}}{% endraw %}
+
+ RUN_SCRIPT: {% raw %}${{github.event.inputs.RUN_SCRIPT}}{% endraw %}
 
-{% endif %}
 {% if paramfile != None %}
  PARAMFILE: {% raw %}${{github.event.inputs.PARAMFILE}}{% endraw %}
 
 {% endif %}
 {% for parameter in parameters %}
  {{ parameter|upper }}: {% raw %}${{github.event.inputs.{% endraw %}{{ parameter|upper}}{% raw %}}}{% endraw %}
 
@@ -60,19 +58,21 @@
        - run: git pull origin ${GITHUB_REF##*/}
        - name: Install kcli
          run: |
            curl https://raw.githubusercontent.com/karmab/kcli/main/install.sh | bash
            # kcli create pool -p /var/lib/libvirt/images default
            # sudo setfacl -m u:$(id -un):rwx /var/lib/libvirt/images
 
-    deploy-plan:
+    render-run-script:
       needs: requirements
       runs-on: {% raw %}${{github.event.inputs.RUNNER}}{% endraw %}
   
       steps:
-{% if kube %}
-       - name: Deploy kcli cluster
-         run: kcli -C $CLIENT create cluster {{ kubetype }} --force {{ paramfileline }} {{ parameterline }} $PLAN
-{% else %}
-       - name: Deploy kcli plan
-         run: kcli -C $CLIENT create plan --force -f $INPUTFILE {{ paramfileline }} {{ parameterline }} $PLAN
-{% endif %}
+       - name: Render script
+         run: kcli -C $CLIENT render -f $SCRIPT {{ paramfileline }} {{ parameterline }} > run.sh
+
+       - name: Display script
+         run: cat run.sh
+
+       - name: Run script
+         run: bash run.sh
+         if: $RUN_SCRIPT == 'true'
```

### Comparing `kcli-99.0.202405071430/kvirt/config.py` & `kcli-99.0.202405080912/kvirt/config.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/container/__init__.py` & `kcli-99.0.202405080912/kvirt/container/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/containerconfig.py` & `kcli-99.0.202405080912/kvirt/containerconfig.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/defaults.py` & `kcli-99.0.202405080912/kvirt/defaults.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/ekstoken.py` & `kcli-99.0.202405080912/kvirt/ekstoken.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/examples.py` & `kcli-99.0.202405080912/kvirt/examples.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/expose/__init__.py` & `kcli-99.0.202405080912/kvirt/expose/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/expose/static/css/bootstrap.min.css` & `kcli-99.0.202405080912/kvirt/expose/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/expose/static/css/jquery.dataTables.min.css` & `kcli-99.0.202405080912/kvirt/expose/static/css/jquery.dataTables.min.css`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/expose/static/css/kcli.css` & `kcli-99.0.202405080912/kvirt/expose/static/css/kcli.css`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/expose/static/images/favicon.ico` & `kcli-99.0.202405080912/kvirt/expose/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/expose/static/images/wheel.gif` & `kcli-99.0.202405080912/kvirt/expose/static/images/wheel.gif`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/expose/static/js/dataTables.checkboxes.min.js` & `kcli-99.0.202405080912/kvirt/expose/static/js/dataTables.checkboxes.min.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/expose/static/js/jquery.dataTables.min.js` & `kcli-99.0.202405080912/kvirt/expose/static/js/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/expose/static/js/jquery.min.js` & `kcli-99.0.202405080912/kvirt/expose/static/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/expose/swagger.yml` & `kcli-99.0.202405080912/kvirt/expose/swagger.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/expose/templates/form.html` & `kcli-99.0.202405080912/kvirt/expose/templates/form.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/expose/templates/head.html` & `kcli-99.0.202405080912/kvirt/expose/templates/head.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/expose/templates/infoplan.html` & `kcli-99.0.202405080912/kvirt/expose/templates/infoplan.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/expose/templates/planstable.html` & `kcli-99.0.202405080912/kvirt/expose/templates/planstable.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/expose/templates/result.html` & `kcli-99.0.202405080912/kvirt/expose/templates/result.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/gketoken.py` & `kcli-99.0.202405080912/kvirt/gketoken.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/ignitionmerger.py` & `kcli-99.0.202405080912/kvirt/ignitionmerger.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/internalplans/__init__.py` & `kcli-99.0.202405080912/kvirt/internalplans/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/jinjafilters/jinjafilters.py` & `kcli-99.0.202405080912/kvirt/jinjafilters/jinjafilters.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/keywords.yaml` & `kcli-99.0.202405080912/kvirt/keywords.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/kfish/__init__.py` & `kcli-99.0.202405080912/kvirt/kfish/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/klist.py` & `kcli-99.0.202405080912/kvirt/klist.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/ksushy/__init__.py` & `kcli-99.0.202405080912/kvirt/ksushy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 def credentials(user, password):
     if default_user is None or default_password is None:
         return True
     elif user is None or password is None:
         return False
-    elif user == default_user or password == default_password:
+    elif user == default_user and password == default_password:
         return True
     else:
         return False
 
 
 class SSLCherryPy(ServerAdapter):
     def run(self, handler):
```

### Comparing `kcli-99.0.202405071430/kvirt/ksushy/templates/bios.json` & `kcli-99.0.202405080912/kvirt/ksushy/templates/bios.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/ksushy/templates/manager.json` & `kcli-99.0.202405080912/kvirt/ksushy/templates/manager.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/ksushy/templates/managers.json` & `kcli-99.0.202405080912/kvirt/ksushy/templates/managers.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/ksushy/templates/root.json` & `kcli-99.0.202405080912/kvirt/ksushy/templates/root.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/ksushy/templates/system.json` & `kcli-99.0.202405080912/kvirt/ksushy/templates/system.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/ksushy/templates/virtualmedia_cd.json` & `kcli-99.0.202405080912/kvirt/ksushy/templates/virtualmedia_cd.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/ksushy/templates/virtualmedias.json` & `kcli-99.0.202405080912/kvirt/ksushy/templates/virtualmedias.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/miniconsole/__init__.py` & `kcli-99.0.202405080912/kvirt/miniconsole/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/nameutils/__init__.py` & `kcli-99.0.202405080912/kvirt/nameutils/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/providers/aws/__init__.py` & `kcli-99.0.202405080912/kvirt/providers/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/providers/aws/ctlplane_policy.json` & `kcli-99.0.202405080912/kvirt/providers/aws/ctlplane_policy.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/providers/azure/__init__.py` & `kcli-99.0.202405080912/kvirt/providers/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/providers/gcp/__init__.py` & `kcli-99.0.202405080912/kvirt/providers/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/providers/ibm/__init__.py` & `kcli-99.0.202405080912/kvirt/providers/ibm/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/providers/kubevirt/__init__.py` & `kcli-99.0.202405080912/kvirt/providers/kubevirt/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/providers/kvm/__init__.py` & `kcli-99.0.202405080912/kvirt/providers/kvm/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/providers/kvm/helpers.py` & `kcli-99.0.202405080912/kvirt/providers/kvm/helpers.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/providers/openstack/__init__.py` & `kcli-99.0.202405080912/kvirt/providers/openstack/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/providers/ovirt/__init__.py` & `kcli-99.0.202405080912/kvirt/providers/ovirt/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/providers/packet/__init__.py` & `kcli-99.0.202405080912/kvirt/providers/packet/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/providers/proxmox/__init__.py` & `kcli-99.0.202405080912/kvirt/providers/proxmox/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/providers/sampleprovider.py` & `kcli-99.0.202405080912/kvirt/providers/sampleprovider.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/providers/vsphere/__init__.py` & `kcli-99.0.202405080912/kvirt/providers/vsphere/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/providers/vsphere/helpers.py` & `kcli-99.0.202405080912/kvirt/providers/vsphere/helpers.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/providers/vsphere/tagging.py` & `kcli-99.0.202405080912/kvirt/providers/vsphere/tagging.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/providers/web/__init__.py` & `kcli-99.0.202405080912/kvirt/providers/web/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/__init__.py` & `kcli-99.0.202405080912/kvirt/web/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/css/bootstrap-theme.min.css` & `kcli-99.0.202405080912/kvirt/web/static/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/css/bootstrap.min.css` & `kcli-99.0.202405080912/kvirt/web/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/css/jquery.dataTables.min.css` & `kcli-99.0.202405080912/kvirt/web/static/css/jquery.dataTables.min.css`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/css/kcli.css` & `kcli-99.0.202405080912/kvirt/web/static/css/kcli.css`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/css/navbar.css` & `kcli-99.0.202405080912/kvirt/web/static/css/navbar.css`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/css/spice.css` & `kcli-99.0.202405080912/kvirt/web/static/css/spice.css`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/fonts/glyphicons-halflings-regular.woff2` & `kcli-99.0.202405080912/kvirt/web/static/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/images/Centos.png` & `kcli-99.0.202405080912/kvirt/web/static/images/Centos.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/images/Fedora.png` & `kcli-99.0.202405080912/kvirt/web/static/images/Fedora.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/images/Redhat.png` & `kcli-99.0.202405080912/kvirt/web/static/images/Redhat.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/images/Suse.png` & `kcli-99.0.202405080912/kvirt/web/static/images/Suse.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/images/Tux.png` & `kcli-99.0.202405080912/kvirt/web/static/images/Tux.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/images/Ubuntu.png` & `kcli-99.0.202405080912/kvirt/web/static/images/Ubuntu.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/images/delete.png` & `kcli-99.0.202405080912/kvirt/web/static/images/delete.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/images/favicon.ico` & `kcli-99.0.202405080912/kvirt/web/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/images/kcli-small.png` & `kcli-99.0.202405080912/kvirt/web/static/images/kcli-small.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/images/kcli.jpg` & `kcli-99.0.202405080912/kvirt/web/static/images/kcli.jpg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/images/kcli.png` & `kcli-99.0.202405080912/kvirt/web/static/images/kcli.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/images/logo-header.svg` & `kcli-99.0.202405080912/kvirt/web/static/images/logo-header.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/images/logo-main.svg` & `kcli-99.0.202405080912/kvirt/web/static/images/logo-main.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/images/start.png` & `kcli-99.0.202405080912/kvirt/web/static/images/start.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/images/stop.png` & `kcli-99.0.202405080912/kvirt/web/static/images/stop.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/images/wheel.gif` & `kcli-99.0.202405080912/kvirt/web/static/images/wheel.gif`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/js/bootstrap-notify.js` & `kcli-99.0.202405080912/kvirt/web/static/js/bootstrap-notify.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/js/bootstrap.min.js` & `kcli-99.0.202405080912/kvirt/web/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/js/containeraction.js` & `kcli-99.0.202405080912/kvirt/web/static/js/containeraction.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/js/dataTables.checkboxes.min.js` & `kcli-99.0.202405080912/kvirt/web/static/js/dataTables.checkboxes.min.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/js/hostaction.js` & `kcli-99.0.202405080912/kvirt/web/static/js/hostaction.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/js/imageaction.js` & `kcli-99.0.202405080912/kvirt/web/static/js/imageaction.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/js/jquery.dataTables.min.js` & `kcli-99.0.202405080912/kvirt/web/static/js/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/js/jquery.min.js` & `kcli-99.0.202405080912/kvirt/web/static/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/js/kcli.js` & `kcli-99.0.202405080912/kvirt/web/static/js/kcli.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/js/kubeaction.js` & `kcli-99.0.202405080912/kvirt/web/static/js/kubeaction.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/js/list.js` & `kcli-99.0.202405080912/kvirt/web/static/js/list.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/js/networkaction.js` & `kcli-99.0.202405080912/kvirt/web/static/js/networkaction.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/js/planaction.js` & `kcli-99.0.202405080912/kvirt/web/static/js/planaction.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/js/poolaction.js` & `kcli-99.0.202405080912/kvirt/web/static/js/poolaction.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/js/productaction.js` & `kcli-99.0.202405080912/kvirt/web/static/js/productaction.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/js/repoaction.js` & `kcli-99.0.202405080912/kvirt/web/static/js/repoaction.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/js/snapshotaction.js` & `kcli-99.0.202405080912/kvirt/web/static/js/snapshotaction.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/js/spice/atKeynames.js` & `kcli-99.0.202405080912/kvirt/web/static/js/spice/atKeynames.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/js/spice/bitmap.js` & `kcli-99.0.202405080912/kvirt/web/static/js/spice/bitmap.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/js/spice/cursor.js` & `kcli-99.0.202405080912/kvirt/web/static/js/spice/cursor.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/js/spice/display.js` & `kcli-99.0.202405080912/kvirt/web/static/js/spice/display.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/js/spice/enums.js` & `kcli-99.0.202405080912/kvirt/web/static/js/spice/enums.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/js/spice/filexfer.js` & `kcli-99.0.202405080912/kvirt/web/static/js/spice/filexfer.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/js/spice/inputs.js` & `kcli-99.0.202405080912/kvirt/web/static/js/spice/inputs.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/js/spice/lz.js` & `kcli-99.0.202405080912/kvirt/web/static/js/spice/lz.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/js/spice/main.js` & `kcli-99.0.202405080912/kvirt/web/static/js/spice/main.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/js/spice/playback.js` & `kcli-99.0.202405080912/kvirt/web/static/js/spice/playback.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/js/spice/png.js` & `kcli-99.0.202405080912/kvirt/web/static/js/spice/png.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/js/spice/port.js` & `kcli-99.0.202405080912/kvirt/web/static/js/spice/port.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/js/spice/quic.js` & `kcli-99.0.202405080912/kvirt/web/static/js/spice/quic.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/js/spice/resize.js` & `kcli-99.0.202405080912/kvirt/web/static/js/spice/resize.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/js/spice/simulatecursor.js` & `kcli-99.0.202405080912/kvirt/web/static/js/spice/simulatecursor.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/js/spice/spicearraybuffer.js` & `kcli-99.0.202405080912/kvirt/web/static/js/spice/spicearraybuffer.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/js/spice/spiceconn.js` & `kcli-99.0.202405080912/kvirt/web/static/js/spice/spiceconn.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/js/spice/spicedataview.js` & `kcli-99.0.202405080912/kvirt/web/static/js/spice/spicedataview.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/js/spice/spicemsg.js` & `kcli-99.0.202405080912/kvirt/web/static/js/spice/spicemsg.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/js/spice/spicetype.js` & `kcli-99.0.202405080912/kvirt/web/static/js/spice/spicetype.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/src/babel-worker.js` & `kcli-99.0.202405080912/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/src/babel-worker.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/src/browser-es-module-loader.js` & `kcli-99.0.202405080912/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/src/browser-es-module-loader.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/js/spice/thirdparty/jsbn.js` & `kcli-99.0.202405080912/kvirt/web/static/js/spice/thirdparty/jsbn.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/js/spice/thirdparty/prng4.js` & `kcli-99.0.202405080912/kvirt/web/static/js/spice/thirdparty/prng4.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/js/spice/thirdparty/rng.js` & `kcli-99.0.202405080912/kvirt/web/static/js/spice/thirdparty/rng.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/js/spice/thirdparty/rsa.js` & `kcli-99.0.202405080912/kvirt/web/static/js/spice/thirdparty/rsa.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/js/spice/thirdparty/sha1.js` & `kcli-99.0.202405080912/kvirt/web/static/js/spice/thirdparty/sha1.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/js/spice/ticket.js` & `kcli-99.0.202405080912/kvirt/web/static/js/spice/ticket.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/js/spice/utils.js` & `kcli-99.0.202405080912/kvirt/web/static/js/spice/utils.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/js/spice/webm.js` & `kcli-99.0.202405080912/kvirt/web/static/js/spice/webm.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/js/spice/wire.js` & `kcli-99.0.202405080912/kvirt/web/static/js/spice/wire.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/js/vmaction.js` & `kcli-99.0.202405080912/kvirt/web/static/js/vmaction.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/error-handler.js` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/error-handler.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/alt.svg` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/alt.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/clipboard.svg` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/clipboard.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/connect.svg` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/connect.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/ctrl.svg` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/ctrl.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/ctrlaltdel.svg` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/ctrlaltdel.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/disconnect.svg` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/disconnect.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/drag.svg` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/drag.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/error.svg` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/error.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/esc.svg` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/esc.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/expander.svg` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/expander.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/fullscreen.svg` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/fullscreen.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/handle.svg` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/handle.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/handle_bg.svg` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/handle_bg.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/icons/Makefile` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/icons/Makefile`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/icons/novnc-120x120.png` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/icons/novnc-120x120.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/icons/novnc-144x144.png` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/icons/novnc-144x144.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/icons/novnc-152x152.png` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/icons/novnc-152x152.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/icons/novnc-16x16.png` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/icons/novnc-16x16.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/icons/novnc-192x192.png` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/icons/novnc-192x192.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/icons/novnc-24x24.png` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/icons/novnc-24x24.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/icons/novnc-32x32.png` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/icons/novnc-32x32.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/icons/novnc-48x48.png` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/icons/novnc-48x48.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/icons/novnc-60x60.png` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/icons/novnc-60x60.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/icons/novnc-64x64.png` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/icons/novnc-64x64.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/icons/novnc-72x72.png` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/icons/novnc-72x72.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/icons/novnc-76x76.png` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/icons/novnc-76x76.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/icons/novnc-96x96.png` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/icons/novnc-96x96.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/icons/novnc-icon-sm.svg` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/icons/novnc-icon-sm.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/icons/novnc-icon.svg` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/icons/novnc-icon.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/info.svg` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/info.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/keyboard.svg` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/keyboard.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/mouse_left.svg` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/mouse_left.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/mouse_middle.svg` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/mouse_middle.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/mouse_none.svg` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/mouse_none.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/mouse_right.svg` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/mouse_right.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/power.svg` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/power.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/settings.svg` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/settings.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/tab.svg` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/tab.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/toggleextrakeys.svg` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/toggleextrakeys.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/warning.svg` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/warning.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/images/windows.svg` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/images/windows.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/locale/cs.json` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/locale/cs.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/locale/de.json` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/locale/de.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/locale/el.json` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/locale/el.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/locale/es.json` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/locale/es.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/locale/ja.json` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/locale/ja.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/locale/ko.json` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/locale/ko.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/locale/nl.json` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/locale/nl.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/locale/pl.json` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/locale/pl.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/locale/ru.json` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/locale/ru.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/locale/sv.json` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/locale/sv.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/locale/tr.json` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/locale/tr.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/locale/zh_CN.json` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/locale/zh_CN.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/locale/zh_TW.json` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/locale/zh_TW.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/localization.js` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/localization.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/sounds/bell.mp3` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/sounds/bell.mp3`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/sounds/bell.oga` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/sounds/bell.oga`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/styles/Orbitron700.ttf` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/styles/Orbitron700.ttf`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/styles/Orbitron700.woff` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/styles/Orbitron700.woff`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/styles/base.css` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/styles/base.css`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/ui.js` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/ui.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/app/webutil.js` & `kcli-99.0.202405080912/kvirt/web/static/vnc/app/webutil.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/core/base64.js` & `kcli-99.0.202405080912/kvirt/web/static/vnc/core/base64.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/core/decoders/copyrect.js` & `kcli-99.0.202405080912/kvirt/web/static/vnc/core/decoders/copyrect.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/core/decoders/hextile.js` & `kcli-99.0.202405080912/kvirt/web/static/vnc/core/decoders/hextile.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/core/decoders/raw.js` & `kcli-99.0.202405080912/kvirt/web/static/vnc/core/decoders/raw.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/core/decoders/rre.js` & `kcli-99.0.202405080912/kvirt/web/static/vnc/core/decoders/rre.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/core/decoders/tight.js` & `kcli-99.0.202405080912/kvirt/web/static/vnc/core/decoders/tight.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/core/decoders/tightpng.js` & `kcli-99.0.202405080912/kvirt/web/static/vnc/core/decoders/tightpng.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/core/des.js` & `kcli-99.0.202405080912/kvirt/web/static/vnc/core/des.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/core/display.js` & `kcli-99.0.202405080912/kvirt/web/static/vnc/core/display.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/core/encodings.js` & `kcli-99.0.202405080912/kvirt/web/static/vnc/core/encodings.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/core/inflator.js` & `kcli-99.0.202405080912/kvirt/web/static/vnc/core/inflator.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/core/input/domkeytable.js` & `kcli-99.0.202405080912/kvirt/web/static/vnc/core/input/domkeytable.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/core/input/fixedkeys.js` & `kcli-99.0.202405080912/kvirt/web/static/vnc/core/input/fixedkeys.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/core/input/keyboard.js` & `kcli-99.0.202405080912/kvirt/web/static/vnc/core/input/keyboard.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/core/input/keysym.js` & `kcli-99.0.202405080912/kvirt/web/static/vnc/core/input/keysym.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/core/input/keysymdef.js` & `kcli-99.0.202405080912/kvirt/web/static/vnc/core/input/keysymdef.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/core/input/mouse.js` & `kcli-99.0.202405080912/kvirt/web/static/vnc/core/input/mouse.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/core/input/util.js` & `kcli-99.0.202405080912/kvirt/web/static/vnc/core/input/util.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/core/input/vkeys.js` & `kcli-99.0.202405080912/kvirt/web/static/vnc/core/input/vkeys.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/core/input/xtscancodes.js` & `kcli-99.0.202405080912/kvirt/web/static/vnc/core/input/xtscancodes.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/core/rfb.js` & `kcli-99.0.202405080912/kvirt/web/static/vnc/core/rfb.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/core/util/browser.js` & `kcli-99.0.202405080912/kvirt/web/static/vnc/core/util/browser.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/core/util/cursor.js` & `kcli-99.0.202405080912/kvirt/web/static/vnc/core/util/cursor.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/core/util/events.js` & `kcli-99.0.202405080912/kvirt/web/static/vnc/core/util/events.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/core/util/eventtarget.js` & `kcli-99.0.202405080912/kvirt/web/static/vnc/core/util/eventtarget.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/core/util/logging.js` & `kcli-99.0.202405080912/kvirt/web/static/vnc/core/util/logging.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/core/util/polyfill.js` & `kcli-99.0.202405080912/kvirt/web/static/vnc/core/util/polyfill.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/core/websock.js` & `kcli-99.0.202405080912/kvirt/web/static/vnc/core/websock.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/vendor/browser-es-module-loader/src/babel-worker.js` & `kcli-99.0.202405080912/kvirt/web/static/vnc/vendor/browser-es-module-loader/src/babel-worker.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/vendor/browser-es-module-loader/src/browser-es-module-loader.js` & `kcli-99.0.202405080912/kvirt/web/static/vnc/vendor/browser-es-module-loader/src/browser-es-module-loader.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/vendor/pako/LICENSE` & `kcli-99.0.202405080912/kvirt/web/static/vnc/vendor/pako/LICENSE`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/vendor/pako/lib/utils/common.js` & `kcli-99.0.202405080912/kvirt/web/static/vnc/vendor/pako/lib/utils/common.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/vendor/pako/lib/zlib/adler32.js` & `kcli-99.0.202405080912/kvirt/web/static/vnc/vendor/pako/lib/zlib/adler32.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/vendor/pako/lib/zlib/constants.js` & `kcli-99.0.202405080912/kvirt/web/static/vnc/vendor/pako/lib/zlib/constants.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/vendor/pako/lib/zlib/crc32.js` & `kcli-99.0.202405080912/kvirt/web/static/vnc/vendor/pako/lib/zlib/crc32.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/vendor/pako/lib/zlib/deflate.js` & `kcli-99.0.202405080912/kvirt/web/static/vnc/vendor/pako/lib/zlib/deflate.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/vendor/pako/lib/zlib/gzheader.js` & `kcli-99.0.202405080912/kvirt/web/static/vnc/vendor/pako/lib/zlib/gzheader.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/vendor/pako/lib/zlib/inffast.js` & `kcli-99.0.202405080912/kvirt/web/static/vnc/vendor/pako/lib/zlib/inffast.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/vendor/pako/lib/zlib/inflate.js` & `kcli-99.0.202405080912/kvirt/web/static/vnc/vendor/pako/lib/zlib/inflate.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/vendor/pako/lib/zlib/inftrees.js` & `kcli-99.0.202405080912/kvirt/web/static/vnc/vendor/pako/lib/zlib/inftrees.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/vendor/pako/lib/zlib/messages.js` & `kcli-99.0.202405080912/kvirt/web/static/vnc/vendor/pako/lib/zlib/messages.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/vendor/pako/lib/zlib/trees.js` & `kcli-99.0.202405080912/kvirt/web/static/vnc/vendor/pako/lib/zlib/trees.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/vendor/pako/lib/zlib/zstream.js` & `kcli-99.0.202405080912/kvirt/web/static/vnc/vendor/pako/lib/zlib/zstream.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/static/vnc/vendor/promise.js` & `kcli-99.0.202405080912/kvirt/web/static/vnc/vendor/promise.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/templates/bootstrap.html` & `kcli-99.0.202405080912/kvirt/web/templates/bootstrap.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/templates/console.html` & `kcli-99.0.202405080912/kvirt/web/templates/console.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/templates/containercreate.html` & `kcli-99.0.202405080912/kvirt/web/templates/containercreate.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/templates/containerprofilestable.html` & `kcli-99.0.202405080912/kvirt/web/templates/containerprofilestable.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/templates/containerstable.html` & `kcli-99.0.202405080912/kvirt/web/templates/containerstable.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/templates/head.html` & `kcli-99.0.202405080912/kvirt/web/templates/head.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/templates/hoststable.html` & `kcli-99.0.202405080912/kvirt/web/templates/hoststable.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/templates/imagecreate.html` & `kcli-99.0.202405080912/kvirt/web/templates/imagecreate.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/templates/imagestable.html` & `kcli-99.0.202405080912/kvirt/web/templates/imagestable.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/templates/kubecreate.html` & `kcli-99.0.202405080912/kvirt/web/templates/kubecreate.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/templates/kubeinfo.html` & `kcli-99.0.202405080912/kvirt/web/templates/kubeinfo.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/templates/kubeprofilestable.html` & `kcli-99.0.202405080912/kvirt/web/templates/kubeprofilestable.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/templates/kubestable.html` & `kcli-99.0.202405080912/kvirt/web/templates/kubestable.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/templates/navbar.html` & `kcli-99.0.202405080912/kvirt/web/templates/navbar.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/templates/networkcreate.html` & `kcli-99.0.202405080912/kvirt/web/templates/networkcreate.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/templates/networks.html` & `kcli-99.0.202405080912/kvirt/web/templates/networks.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/templates/networkstable.html` & `kcli-99.0.202405080912/kvirt/web/templates/networkstable.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/templates/plancreate.html` & `kcli-99.0.202405080912/kvirt/web/templates/plancreate.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/templates/planstable.html` & `kcli-99.0.202405080912/kvirt/web/templates/planstable.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/templates/poolcreate.html` & `kcli-99.0.202405080912/kvirt/web/templates/poolcreate.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/templates/poolstable.html` & `kcli-99.0.202405080912/kvirt/web/templates/poolstable.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/templates/productcreate.html` & `kcli-99.0.202405080912/kvirt/web/templates/productcreate.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/templates/productstable.html` & `kcli-99.0.202405080912/kvirt/web/templates/productstable.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/templates/repocreate.html` & `kcli-99.0.202405080912/kvirt/web/templates/repocreate.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/templates/repostable.html` & `kcli-99.0.202405080912/kvirt/web/templates/repostable.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/templates/vmcreate.html` & `kcli-99.0.202405080912/kvirt/web/templates/vmcreate.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/templates/vmprofilestable.html` & `kcli-99.0.202405080912/kvirt/web/templates/vmprofilestable.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/kvirt/web/templates/vmstable.html` & `kcli-99.0.202405080912/kvirt/web/templates/vmstable.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/samples/config.yml` & `kcli-99.0.202405080912/samples/config.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/samples/profiles.yml` & `kcli-99.0.202405080912/samples/profiles.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202405071430/setup.py` & `kcli-99.0.202405080912/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 description = 'Provisioner/Manager for Libvirt/Vsphere/Aws/Gcp/Kubevirt/Ovirt/Openstack/IBM Cloud and containers'
 long_description = description
 if os.path.exists('README.rst'):
     long_description = open('README.rst').read()
 
 setup(
     name='kcli',
-    version='99.0.202405071430',
+    version='99.0.202405080912',
     include_package_data=True,
     packages=find_packages(),
     zip_safe=False,
     description=description,
     long_description=long_description,
     url='http://github.com/karmab/kcli',
     author='Karim Boumedhel',
```

### Comparing `kcli-99.0.202405071430/tests/test_kvirt.py` & `kcli-99.0.202405080912/tests/test_kvirt.py`

 * *Files identical despite different names*

