# Comparing `tmp/kvxopt-1.3.2.0.tar.gz` & `tmp/kvxopt-1.3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kvxopt-1.3.2.0.tar", last modified: Mon Oct 16 17:59:18 2023, max compression
+gzip compressed data, was "kvxopt-1.3.2.1.tar", last modified: Wed May  8 16:49:13 2024, max compression
```

## Comparing `kvxopt-1.3.2.0.tar` & `kvxopt-1.3.2.1.tar`

### file list

```diff
@@ -1,582 +1,582 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-10-16 17:59:18.691321 kvxopt-1.3.2.0/
--rw-r--r--   0 runner     (501) staff       (20)       36 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/.gitattributes
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-10-16 17:59:18.276078 kvxopt-1.3.2.0/.github/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-10-16 17:59:18.296690 kvxopt-1.3.2.0/.github/workflows/
--rw-r--r--   0 runner     (501) staff       (20)     3155 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/.github/workflows/linux_build.yml
--rw-r--r--   0 runner     (501) staff       (20)     3051 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/.github/workflows/macos_build.yml
--rw-r--r--   0 runner     (501) staff       (20)    10620 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/.github/workflows/windows_build.yml
--rw-r--r--   0 runner     (501) staff       (20)      169 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/.gitignore
--rw-r--r--   0 runner     (501) staff       (20)     1472 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/INSTALL
--rw-r--r--   0 runner     (501) staff       (20)     5807 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/Jenkinsfile
--rw-r--r--   0 runner     (501) staff       (20)    35993 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)      217 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     1592 2023-10-16 17:59:18.691543 kvxopt-1.3.2.0/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     2634 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-10-16 17:59:18.297172 kvxopt-1.3.2.0/doc/
--rw-r--r--   0 runner     (501) staff       (20)     2321 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/Makefile
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-10-16 17:59:18.312562 kvxopt-1.3.2.0/doc/html/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-10-16 17:59:18.315485 kvxopt-1.3.2.0/doc/html/_images/
--rw-r--r--   0 runner     (501) staff       (20)     9062 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/floorplan.png
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-10-16 17:59:18.553769 kvxopt-1.3.2.0/doc/html/_images/math/
--rw-r--r--   0 runner     (501) staff       (20)      416 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/00b60df5731428a5a02b49ca7bc4d5aaa7afac9c.png
--rw-r--r--   0 runner     (501) staff       (20)     1078 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/00e8f621cc91c8f430e504b66fb085743c4814cb.png
--rw-r--r--   0 runner     (501) staff       (20)     1269 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/01824df8f8806530b722445b6f9cde3a8e732f07.png
--rw-r--r--   0 runner     (501) staff       (20)      255 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/0202eb241774e15b6d1398f17dd161778e602b90.png
--rw-r--r--   0 runner     (501) staff       (20)      494 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/022ccd45e165efaafd4897b98a41553943db3f05.png
--rw-r--r--   0 runner     (501) staff       (20)      323 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/036001c78514c5de2ab5c899cb2b005a905ba3a5.png
--rw-r--r--   0 runner     (501) staff       (20)      747 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/03cfea18434ec87caa164206e463d7a230e1cb5c.png
--rw-r--r--   0 runner     (501) staff       (20)     1275 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/03da04b738c1b20d64d873e8f3c18eccc4c7bc84.png
--rw-r--r--   0 runner     (501) staff       (20)     1538 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/04163b47432b93c2e42e10bab40066847581fc79.png
--rw-r--r--   0 runner     (501) staff       (20)      405 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/04342bcceed278806ffa3c6deee7f762c50a6eab.png
--rw-r--r--   0 runner     (501) staff       (20)     1331 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/04b02267d8a264913c39b04bf73ab88181b03cfc.png
--rw-r--r--   0 runner     (501) staff       (20)     1400 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/056427854bd8d5a1fa428fff460d45b749aebc2a.png
--rw-r--r--   0 runner     (501) staff       (20)      558 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/05c3b434aba8ec5e2ac1cdfcc3e3bb7ca8a69775.png
--rw-r--r--   0 runner     (501) staff       (20)     7496 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/0667e780fc9b2d0fad01d14184553aba1cd6b81b.png
--rw-r--r--   0 runner     (501) staff       (20)      341 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/06fa9ba19a3d38408ac220954e05a6105bec867c.png
--rw-r--r--   0 runner     (501) staff       (20)      846 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/072b7c28c9bc48c8509301fcff6dfb5095db4a07.png
--rw-r--r--   0 runner     (501) staff       (20)     1476 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/073b4fb9749f6ab5523c701bbe38a97c5fa94288.png
--rw-r--r--   0 runner     (501) staff       (20)      372 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/07478b8108c1b9d0c0317e8bc57b8776263d0a85.png
--rw-r--r--   0 runner     (501) staff       (20)     1057 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/0790b49262067229d1ce8165c4a66b4afa62cda9.png
--rw-r--r--   0 runner     (501) staff       (20)     1317 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/081eab67b8ad47c824c773f9ce571fe5883895bf.png
--rw-r--r--   0 runner     (501) staff       (20)      933 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/08390710b56f1bdd0cf7346dd20ee9b3a5984ea1.png
--rw-r--r--   0 runner     (501) staff       (20)     3059 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/0b6da08d6fc1f85c1382af2c64a51fa0129e47fd.png
--rw-r--r--   0 runner     (501) staff       (20)     1585 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/0b75ca09d0ef9d47484865bd353fc1e234d0ffae.png
--rw-r--r--   0 runner     (501) staff       (20)     1616 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/0bf595687ae571b0147a101f606500879246b152.png
--rw-r--r--   0 runner     (501) staff       (20)      849 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/0e7509809ae807b340e6d7cd64cc157ce0c8a4ff.png
--rw-r--r--   0 runner     (501) staff       (20)     1359 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/0e95b3c9bb477c1d27aa253d83fe2d3e1922b3ef.png
--rw-r--r--   0 runner     (501) staff       (20)      275 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/0edac3a6b0973196c5005c560d87e755c0ea5c86.png
--rw-r--r--   0 runner     (501) staff       (20)      971 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/0f2f6181474c4d231456601880211909048d0548.png
--rw-r--r--   0 runner     (501) staff       (20)     1667 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/0f36e4d687eeb224ee6593ac11df99a1d4451ba9.png
--rw-r--r--   0 runner     (501) staff       (20)     1670 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/0fc13f815b495c77d502992ae392d16844c0950b.png
--rw-r--r--   0 runner     (501) staff       (20)      263 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/0fcab9067b50b87e868c4fd70f213a086addb964.png
--rw-r--r--   0 runner     (501) staff       (20)      205 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/106b04b320e75010b1d8029e59244f234f75e6f9.png
--rw-r--r--   0 runner     (501) staff       (20)     1411 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/10d754c37b304c217ee6f80c9a3c4c7bcbbcba9d.png
--rw-r--r--   0 runner     (501) staff       (20)     1467 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/11969d386f3f62d281586721cb47b9bc640ea082.png
--rw-r--r--   0 runner     (501) staff       (20)      879 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/12354e7e046bba1f8384eebcc70a2d9a09930e8e.png
--rw-r--r--   0 runner     (501) staff       (20)     5190 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/124ef7067b147c5c7f031fc0fc06a822029456c1.png
--rw-r--r--   0 runner     (501) staff       (20)     1446 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/1337abb9748b0985f66823f48527ff07692b910a.png
--rw-r--r--   0 runner     (501) staff       (20)     3584 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/13abf6ff1ab819235d06737ba4cc4b56c12cf29f.png
--rw-r--r--   0 runner     (501) staff       (20)      237 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/141bbefb74014fc5e43499901bf78607ae335583.png
--rw-r--r--   0 runner     (501) staff       (20)     1356 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/145a22013f61134f2b61c99bdc4bf56a23e7ba62.png
--rw-r--r--   0 runner     (501) staff       (20)      358 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/146bec31bf294e89657786d59d21f9c4307ed72f.png
--rw-r--r--   0 runner     (501) staff       (20)      629 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/15ccba8c9b68894aeb55e081c819b82da74b90ed.png
--rw-r--r--   0 runner     (501) staff       (20)      300 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/161320f045cc4315c31907ec05fe170909e3c274.png
--rw-r--r--   0 runner     (501) staff       (20)      259 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/166d5d3acaad3170290c97811491b74b32041dad.png
--rw-r--r--   0 runner     (501) staff       (20)      414 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/172415a1aefbbb006e616ac35d880030890ad136.png
--rw-r--r--   0 runner     (501) staff       (20)      295 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/183e9814ec579a80697d078963ce0412589322f1.png
--rw-r--r--   0 runner     (501) staff       (20)     2470 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/191bc203fa207a53847c892bc9bc56a69a1c60c1.png
--rw-r--r--   0 runner     (501) staff       (20)      239 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/19eef1966f7c545af3ac8c0fa486974d873e3c65.png
--rw-r--r--   0 runner     (501) staff       (20)      400 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/1b1815f8a1dcb49152792554f110261420c96b3c.png
--rw-r--r--   0 runner     (501) staff       (20)      241 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/1b5e577d6216dca3af7d87aa122a0b9b360d6cb3.png
--rw-r--r--   0 runner     (501) staff       (20)      287 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/1cfcab44d097a385b6e2fb16cfefc2f062ab999f.png
--rw-r--r--   0 runner     (501) staff       (20)      833 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/1e0371cc3025278f588fd7d0ccfcc2510ff2f8cf.png
--rw-r--r--   0 runner     (501) staff       (20)      320 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/1e45a7a687f92b2a29b62ce1dddb23a8eefeedca.png
--rw-r--r--   0 runner     (501) staff       (20)     2440 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/1e7e60bfda710d3db286c7b54852b9cb3e77c861.png
--rw-r--r--   0 runner     (501) staff       (20)      337 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/1e913e459d7bcb538986828dad39d548fa73228f.png
--rw-r--r--   0 runner     (501) staff       (20)      259 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/1ebe654cc7b8f2a0d8100aa5825cf2b9021adbbc.png
--rw-r--r--   0 runner     (501) staff       (20)      269 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/1f2cf406b1224eb3a604895ac84524c6aed56983.png
--rw-r--r--   0 runner     (501) staff       (20)      289 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/1fbee781f84569077719a167b64e12064360fac1.png
--rw-r--r--   0 runner     (501) staff       (20)      244 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/211284f68205c3e66773eaf026f32a0acdd3dfb3.png
--rw-r--r--   0 runner     (501) staff       (20)     1792 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/211a6aeaec6adf6a5dd8e0c7de1c4e9f4635ad25.png
--rw-r--r--   0 runner     (501) staff       (20)     1858 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/21281aa0c6a6c01b835faeb9de4a5ba91527df33.png
--rw-r--r--   0 runner     (501) staff       (20)     1325 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/2149e945c5e7e174b2a1146a3669a5a0b1c65f32.png
--rw-r--r--   0 runner     (501) staff       (20)     1635 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/21f2b425bff574fa56ee14ddbb7517747adb4266.png
--rw-r--r--   0 runner     (501) staff       (20)     1373 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/2211f73518e89008db8e07b1bb8a7b8881d0263f.png
--rw-r--r--   0 runner     (501) staff       (20)     2344 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/23507579d8ee310e9bc7a287d88d48f8f5ab891f.png
--rw-r--r--   0 runner     (501) staff       (20)      283 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/249b38285050bda51fd1579d716b5553f8114a0d.png
--rw-r--r--   0 runner     (501) staff       (20)      513 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/26e45da42a12ddc160256fb6cbbb944eeba0dee8.png
--rw-r--r--   0 runner     (501) staff       (20)     5636 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/2877bec99a56fcd4a3f6b39b56c2fe14acb7ee94.png
--rw-r--r--   0 runner     (501) staff       (20)      614 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/294ea142766a27b4576f8c3240182c9220174aad.png
--rw-r--r--   0 runner     (501) staff       (20)      730 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/296e9942f8952b0eda9b312b690a6662f47008e9.png
--rw-r--r--   0 runner     (501) staff       (20)     1264 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/2ac45fcc15c7339cc8ecbdb592c53bc49bf33c73.png
--rw-r--r--   0 runner     (501) staff       (20)     2921 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/2c0f91e60d2f13fdeba173121a264d745555e902.png
--rw-r--r--   0 runner     (501) staff       (20)      567 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/2e7d885be2f8d9a7556b4e6dded7b42315803547.png
--rw-r--r--   0 runner     (501) staff       (20)     1558 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/306121f2c5a959611abb74ce19acd25173d3cb33.png
--rw-r--r--   0 runner     (501) staff       (20)     1595 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/3157de5f84013f57240cf058275c3ae9deb3287a.png
--rw-r--r--   0 runner     (501) staff       (20)      330 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/317f05bfc503c0f2967f94d5108fa418a7e4578e.png
--rw-r--r--   0 runner     (501) staff       (20)     1688 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/322793af4baec9f7ebaa53c4c21f4a468036799a.png
--rw-r--r--   0 runner     (501) staff       (20)     2184 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/32cab048b453581f0ca59dc31e33e56b7c8b3a0e.png
--rw-r--r--   0 runner     (501) staff       (20)      423 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/3352e62eefabf4e08a86652e339b0ef936c86ced.png
--rw-r--r--   0 runner     (501) staff       (20)      932 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/340c54d7b4f301eb582e5ce306364e1cc4fe20b1.png
--rw-r--r--   0 runner     (501) staff       (20)     1275 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/34a857941bc037025e34cfc7d5ddf0cba068c3f7.png
--rw-r--r--   0 runner     (501) staff       (20)      450 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/36c1c1b5e868253601aefce353956d96322883ae.png
--rw-r--r--   0 runner     (501) staff       (20)      524 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/36dfce98812a98045ee08f8608788e512eed0fe3.png
--rw-r--r--   0 runner     (501) staff       (20)     3059 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/3725c3144c904e39aef17290ef9fdefa9e3adfe0.png
--rw-r--r--   0 runner     (501) staff       (20)      994 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/37ab88a567d07e7cd18072c1f9878e17b26e1a6a.png
--rw-r--r--   0 runner     (501) staff       (20)     1832 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/385dad5a2df2ddd65900bef4c4ab58d4a4a0829d.png
--rw-r--r--   0 runner     (501) staff       (20)      452 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/38e9e9d3b438f8da362e850c8eb1c0252af8373a.png
--rw-r--r--   0 runner     (501) staff       (20)     2384 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/3910830c8976bd5c91219274bd08ca0401852b45.png
--rw-r--r--   0 runner     (501) staff       (20)     1430 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/39848b64dc282be81d51d8786746c0b13bd48bcc.png
--rw-r--r--   0 runner     (501) staff       (20)     1693 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/3a138e23ab33c536c23ad13ff28606737fe7e610.png
--rw-r--r--   0 runner     (501) staff       (20)      446 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/3ae50aaf765cd8eb0463a159845004ccae1c3cff.png
--rw-r--r--   0 runner     (501) staff       (20)     1894 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/3b0de39a2c386bc0f8d5ee56519cab864e57d389.png
--rw-r--r--   0 runner     (501) staff       (20)     1475 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/3b8df11e628aac991d176b270cf335fd89834cfc.png
--rw-r--r--   0 runner     (501) staff       (20)      240 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/3bb6de8fbb6eb7f9723920dea5cd674c8c713f45.png
--rw-r--r--   0 runner     (501) staff       (20)      263 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/3bfb3a64189a14b2704f4610827762d5e3145114.png
--rw-r--r--   0 runner     (501) staff       (20)     4639 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/3f12bcd60dcbf296614984241c025a909a803e1e.png
--rw-r--r--   0 runner     (501) staff       (20)      894 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/3f1dd94c34f67811ddb2df9812cfb065dea10aac.png
--rw-r--r--   0 runner     (501) staff       (20)      546 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/3f7c5e248ea93d509e428921ea91f68e03f1b029.png
--rw-r--r--   0 runner     (501) staff       (20)      528 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/3fb48872eb2d412f7878dd8934dab8823ce6422b.png
--rw-r--r--   0 runner     (501) staff       (20)     1539 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/3fd3b9b7b701e9534c715081f10fd72d4c4670f6.png
--rw-r--r--   0 runner     (501) staff       (20)     1204 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/42e6ff06c5afcf7438f6b7bd0027c3c738feceb6.png
--rw-r--r--   0 runner     (501) staff       (20)      462 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/4357a4e29a351ac6ae90924cc00e06184fbd8412.png
--rw-r--r--   0 runner     (501) staff       (20)      523 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/4568da7a353653545f711003d54f38db128766df.png
--rw-r--r--   0 runner     (501) staff       (20)      330 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/459f00b80184047c37413367f1bc32570987f2c1.png
--rw-r--r--   0 runner     (501) staff       (20)     1894 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/45ab4648d9d463e88b6a823609eaac81787d876f.png
--rw-r--r--   0 runner     (501) staff       (20)     1323 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/45bf7a5d17860fe8ca50fd24ff910e00ce5f8a39.png
--rw-r--r--   0 runner     (501) staff       (20)     1655 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/45ca0c9c05f16b36175b595487b17f411e30a5d6.png
--rw-r--r--   0 runner     (501) staff       (20)     1855 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/46362a8b56ad9a6cb816f0062260ad22a76b6f08.png
--rw-r--r--   0 runner     (501) staff       (20)      211 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/470aa65888a2971c9346e573f12b37ea406b8ec9.png
--rw-r--r--   0 runner     (501) staff       (20)     1270 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/4786cdb10b56effd1cbd6730d8a8497748d072c0.png
--rw-r--r--   0 runner     (501) staff       (20)      963 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/4798110dbfdeb1ecd95e4f30fe61ccf31ce4f503.png
--rw-r--r--   0 runner     (501) staff       (20)     1025 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/482017ed70f2f392091ce55bf925c4d264ca15ba.png
--rw-r--r--   0 runner     (501) staff       (20)     1626 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/485e65f87f30e5ab52138c945744fe97e6dd87dc.png
--rw-r--r--   0 runner     (501) staff       (20)      891 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/487040712ec6e78e6ce843fdedb84752b97c2547.png
--rw-r--r--   0 runner     (501) staff       (20)      234 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/4a3598141469c2555591e66606a1b86d4ec6dca9.png
--rw-r--r--   0 runner     (501) staff       (20)      288 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/4abba779877abb276b98ccb2b4ba9bf2e41947ab.png
--rw-r--r--   0 runner     (501) staff       (20)      321 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/4ac9a8351b68de952fda2e33246216aa5edb2818.png
--rw-r--r--   0 runner     (501) staff       (20)      266 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/4bc3e94a67870b41b7c20179693e889251e2c136.png
--rw-r--r--   0 runner     (501) staff       (20)      275 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/4bcdc64a07db3d7711bc2889fe6459e2ae4e65d6.png
--rw-r--r--   0 runner     (501) staff       (20)      230 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/4c120f773ab4e1c59ad2bd44aae969ce24dd190a.png
--rw-r--r--   0 runner     (501) staff       (20)     1495 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/4c8eef5c3334015a2ce256c6afde864dcac2b7ad.png
--rw-r--r--   0 runner     (501) staff       (20)      245 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/4db5b6e16e06f929ce3f675c5e535d06ffb02ff7.png
--rw-r--r--   0 runner     (501) staff       (20)      290 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/4dc6347ee63e4c699378bbfd3c9c00e328e6a91d.png
--rw-r--r--   0 runner     (501) staff       (20)     1700 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/4e317307fb34d4308336c7711497db123b7d9def.png
--rw-r--r--   0 runner     (501) staff       (20)     1693 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/4e3f3707720cdc0ad65a45a1568034b0499846a9.png
--rw-r--r--   0 runner     (501) staff       (20)      412 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/4f58d165825711e6619115afb28c246c00440fa2.png
--rw-r--r--   0 runner     (501) staff       (20)     1353 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/4f7be1be65d6087c8016b324e3d3e258e12f405d.png
--rw-r--r--   0 runner     (501) staff       (20)     1299 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/5046b770f82749051a01f8f102c8e5ff69c4a3e4.png
--rw-r--r--   0 runner     (501) staff       (20)      340 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/5052552450b786edab8e0415c96dfa848bc40be1.png
--rw-r--r--   0 runner     (501) staff       (20)      263 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/52ddc0cde6d632f631533173562fe3ca375b1f32.png
--rw-r--r--   0 runner     (501) staff       (20)     1623 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/54cbbb3d4691d21c5f1604825fce3e264ef4e7cb.png
--rw-r--r--   0 runner     (501) staff       (20)     2151 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/55eedb919b02b7a0654137bd319d8bb919ad3067.png
--rw-r--r--   0 runner     (501) staff       (20)     1554 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/56ac83c03464e42463c625f1f9ef1833a2927d2e.png
--rw-r--r--   0 runner     (501) staff       (20)     2569 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/56ebcc22b7fc4da65f58f0819b21a4c7da613bd4.png
--rw-r--r--   0 runner     (501) staff       (20)     1149 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/582940bfca19aac437939d3e7b6be8c577797dad.png
--rw-r--r--   0 runner     (501) staff       (20)      446 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/5866199ac7f27f9fa8f345c8d6bd6f14fc869908.png
--rw-r--r--   0 runner     (501) staff       (20)      286 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/58dfeba24c101319ed253c88f1b03e306ab30e1f.png
--rw-r--r--   0 runner     (501) staff       (20)      228 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/5a939c5280da7202ca4531f175a7780ad5e1f80a.png
--rw-r--r--   0 runner     (501) staff       (20)      239 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/5b7752c757e0b691a80ab8227eadb8a8389dc58a.png
--rw-r--r--   0 runner     (501) staff       (20)     1703 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/5d759a9a1a42876f1cefe2c9fc361df2a167d545.png
--rw-r--r--   0 runner     (501) staff       (20)      546 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/5dacf40fdb001db01bc47f5b86fcb7ce6dc4a0e2.png
--rw-r--r--   0 runner     (501) staff       (20)     1809 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/5fa951f18d59f8caa1d2bc6ec81f6a0c945bfe75.png
--rw-r--r--   0 runner     (501) staff       (20)      430 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/60d0a6fc7c07bee2dc81830096d4d310add8f5eb.png
--rw-r--r--   0 runner     (501) staff       (20)     1256 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/61425e89ec518b2689e5063426419950648cd2dc.png
--rw-r--r--   0 runner     (501) staff       (20)      824 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/61a7d25e3673146402ed26716d6eb60e8e9d18fa.png
--rw-r--r--   0 runner     (501) staff       (20)     1574 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/620321226792601132c52174a5287a8c93e9bc5f.png
--rw-r--r--   0 runner     (501) staff       (20)     1955 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/627d2d6ebe12e40470cbb763687cffb52453abe1.png
--rw-r--r--   0 runner     (501) staff       (20)      524 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/62cd1c16ca3ef9e2b0d5696a6a49b6b5a6d19130.png
--rw-r--r--   0 runner     (501) staff       (20)     1180 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/64824b782d63f742bca8b398e0f12b485771f257.png
--rw-r--r--   0 runner     (501) staff       (20)     2236 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/6565000626ccf19f09a9258e78e141cb5ce46180.png
--rw-r--r--   0 runner     (501) staff       (20)      769 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/66599856ec5735a610623bbe8242fc777d5f4100.png
--rw-r--r--   0 runner     (501) staff       (20)     9750 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/6669c8a566ba908085156b5c4a539af53616f383.png
--rw-r--r--   0 runner     (501) staff       (20)     2840 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/66e3f8da85954ae75f6016f5784d0ec468c2451c.png
--rw-r--r--   0 runner     (501) staff       (20)     1941 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/68ea4366a8e9dac6f50d5b899ac5c385374d9673.png
--rw-r--r--   0 runner     (501) staff       (20)     1415 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/694498e646bcebcf71487704e8bbabe9b2665425.png
--rw-r--r--   0 runner     (501) staff       (20)      331 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/6981ec4aaaf7392f4bf828ef63be506799574e5e.png
--rw-r--r--   0 runner     (501) staff       (20)      428 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/69ff02759612b6bf7f038a67b9fb4b557f2be247.png
--rw-r--r--   0 runner     (501) staff       (20)     1610 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/6b3a21804f75fb45e7f9963fc6c0621fcf710cc7.png
--rw-r--r--   0 runner     (501) staff       (20)     1457 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/6b3d942743e5a56e5030cfaab836f542fec9019c.png
--rw-r--r--   0 runner     (501) staff       (20)      268 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/6c74a61cdf90a8a3b50f62a58910b84d0fe23678.png
--rw-r--r--   0 runner     (501) staff       (20)     1738 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/6d9473d4787aece2804514f0796e6abeb2ce4dda.png
--rw-r--r--   0 runner     (501) staff       (20)     2209 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/6dd83f47897e8af1a287a2cb577906b4c142c166.png
--rw-r--r--   0 runner     (501) staff       (20)     1095 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/6efd575f4ef0199dda05d5b8f4a187112a62224b.png
--rw-r--r--   0 runner     (501) staff       (20)      458 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/700c6a7cc89a7142ae312c5cb4f1f5b78da350dd.png
--rw-r--r--   0 runner     (501) staff       (20)      290 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/7046228257af6ebbbde8ef7c8f944119e0a768d0.png
--rw-r--r--   0 runner     (501) staff       (20)     1233 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/7056acd535c8f98331e8dd89e48cc0e927d42b12.png
--rw-r--r--   0 runner     (501) staff       (20)     2610 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/7075b711b50c004803b51912b9dca99d35c65d35.png
--rw-r--r--   0 runner     (501) staff       (20)     1211 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/70b640ff0659b7d33287ba001e5b26c6c93a96ba.png
--rw-r--r--   0 runner     (501) staff       (20)      950 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/716fbcea39bcb0c1e19a3e26c60836bf5b111b91.png
--rw-r--r--   0 runner     (501) staff       (20)     3140 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/727233e1f841277ba9bce9859cd9fbbe664f1667.png
--rw-r--r--   0 runner     (501) staff       (20)      659 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/738092734154893db4338bbdedae2ef8c48eade3.png
--rw-r--r--   0 runner     (501) staff       (20)      790 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/73e26546f3f051d6cc494fa37072d2eac9856ac1.png
--rw-r--r--   0 runner     (501) staff       (20)     1828 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/7627c2662a2a563bf350d8d618dd7e6d40c35e2e.png
--rw-r--r--   0 runner     (501) staff       (20)     1398 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/767b9280eb4c7a6ad46be67cb9782508dc6d1f22.png
--rw-r--r--   0 runner     (501) staff       (20)     1278 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/783499b0add3c6f6f392a2b8d39402a6aa232020.png
--rw-r--r--   0 runner     (501) staff       (20)     1119 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/78d5bb409e88f612d4afe2cca2f43186923387e6.png
--rw-r--r--   0 runner     (501) staff       (20)      503 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/7911e1577218dbb02d5e98a311635e1b2347ff57.png
--rw-r--r--   0 runner     (501) staff       (20)      420 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/79b3736681052735beb52087fe8a1b6c188338fb.png
--rw-r--r--   0 runner     (501) staff       (20)     2286 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/7b25a0b8e9e5569bb0e977a9ea61b5daedb78e11.png
--rw-r--r--   0 runner     (501) staff       (20)     1350 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/7b694e55a0813fe78e01121684b12a40fad86d86.png
--rw-r--r--   0 runner     (501) staff       (20)      243 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/7daf0d4815e763eb90f0d5f1dc406f668c1e21db.png
--rw-r--r--   0 runner     (501) staff       (20)      601 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/7dcb78b012b54b09f8760cec52ce8ae1389f0f11.png
--rw-r--r--   0 runner     (501) staff       (20)      377 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/7e3e2e4f92024433a9ad4d75422c991d86d1ec57.png
--rw-r--r--   0 runner     (501) staff       (20)      547 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/7e65c1c7c403764759e8813348c1b7e2d560f1fa.png
--rw-r--r--   0 runner     (501) staff       (20)     1608 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/7eac6332e16c5424a4b290d2b9f9445c5214a1d1.png
--rw-r--r--   0 runner     (501) staff       (20)     2840 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/7faf4e55287d19aeb554d113cd37857aeb2700b4.png
--rw-r--r--   0 runner     (501) staff       (20)      252 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/801e28cfd4de6fd9c1e00f5e71e5ce7b29ad57f7.png
--rw-r--r--   0 runner     (501) staff       (20)      273 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/808724526b9ab0aff711bd48855599a13f4f41c5.png
--rw-r--r--   0 runner     (501) staff       (20)     7061 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/80e21626c375d52667de27ff84715270afb8ca70.png
--rw-r--r--   0 runner     (501) staff       (20)      359 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/812c22f26f3cabffdd7214c59716aef9a9fedca2.png
--rw-r--r--   0 runner     (501) staff       (20)     1366 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/81787f23988417db8fee122d8cc6141a1985c4b7.png
--rw-r--r--   0 runner     (501) staff       (20)      516 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/817f53603d7e46d0c89d94f741f3ff760e7b4e64.png
--rw-r--r--   0 runner     (501) staff       (20)      574 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/81868e29eaf33185bcc60e1d6ff7b0e307f2f892.png
--rw-r--r--   0 runner     (501) staff       (20)     1025 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/82a55744f92063b61aaffddd2380a5cbf8a2b1c6.png
--rw-r--r--   0 runner     (501) staff       (20)     1015 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/82d7fac4e1442a73c02aa8bd6fedab161db0f758.png
--rw-r--r--   0 runner     (501) staff       (20)     1507 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/838e2b03a608af26db2efa9096182aa54d809a3d.png
--rw-r--r--   0 runner     (501) staff       (20)     4580 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/84e264805077d2cf923fe75d31e2ed50021618da.png
--rw-r--r--   0 runner     (501) staff       (20)      406 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/8621cd51e6bdca11da768ea315ebf1b8c319a975.png
--rw-r--r--   0 runner     (501) staff       (20)     1163 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/86384124ce2e714ba7b80c295f44157d2da07413.png
--rw-r--r--   0 runner     (501) staff       (20)     1078 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/8655418fcbc61747ed3bd70aa2d1ecc1db06a5c9.png
--rw-r--r--   0 runner     (501) staff       (20)     1198 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/86a2d178f8f888b9c84ff42573fdaf015c8bfbb2.png
--rw-r--r--   0 runner     (501) staff       (20)     1780 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/86cec286c2bbedaa7760445bc5a1a242cb84d2c2.png
--rw-r--r--   0 runner     (501) staff       (20)     1447 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/870c60a6ab1247468ddfc5be8f68ffbe3479dfda.png
--rw-r--r--   0 runner     (501) staff       (20)     1359 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/8871516499f79705d3818c3251aacd463f7c5146.png
--rw-r--r--   0 runner     (501) staff       (20)      601 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/887be39f02687d3e3a1565193924f04d7ccbb743.png
--rw-r--r--   0 runner     (501) staff       (20)      213 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/888f7c323ac0341871e867220ae2d76467d74d6e.png
--rw-r--r--   0 runner     (501) staff       (20)     1721 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/895591ad55b7e2cec6ade3bbb0bb1a0b76fe0910.png
--rw-r--r--   0 runner     (501) staff       (20)      255 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/89878909dbb648acdc4a44ded1bd982d7bddef5d.png
--rw-r--r--   0 runner     (501) staff       (20)     1128 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/89d343471476626b56bc496f09d8fad108cb82a6.png
--rw-r--r--   0 runner     (501) staff       (20)      313 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/8adc14b919839192224a68d21c0cae3a8b783c04.png
--rw-r--r--   0 runner     (501) staff       (20)      436 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/8b5c5ce382e60258664c8b9eef58be7dad76daf3.png
--rw-r--r--   0 runner     (501) staff       (20)      458 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/8ba9d3d0710a882764a58249d7a443b475a5b7d8.png
--rw-r--r--   0 runner     (501) staff       (20)     2061 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/8c1dcc7704e1d156a5f896c8c0a3326c2722a3fa.png
--rw-r--r--   0 runner     (501) staff       (20)     1021 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/8c51b26db8908731ed17a76ed86a9fe1c99aa02b.png
--rw-r--r--   0 runner     (501) staff       (20)      498 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/8cb2d6eb037326c227a257ebad6eae725bd40148.png
--rw-r--r--   0 runner     (501) staff       (20)      207 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/8d051150f8669295ecdbe92367941012175a824d.png
--rw-r--r--   0 runner     (501) staff       (20)      329 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/8d1638c06d78232d12c1df1eac99cc20f863d50e.png
--rw-r--r--   0 runner     (501) staff       (20)     1693 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/8d26408b917ad631b6ae90f7650b19b691fe2bb6.png
--rw-r--r--   0 runner     (501) staff       (20)      929 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/8d53a80f87a15ba0d310801a0af822da73c3fcaf.png
--rw-r--r--   0 runner     (501) staff       (20)      370 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/8d7aeb80b08f9d220de852b224d6a4693f6ddff9.png
--rw-r--r--   0 runner     (501) staff       (20)     1361 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/8edd44acd8c3889706afee3c81bb907c3f415683.png
--rw-r--r--   0 runner     (501) staff       (20)      244 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/8fb1fc12384d9c1b73b81b87315f7654511a2c0e.png
--rw-r--r--   0 runner     (501) staff       (20)     1093 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/8fcff6b5a5c95afb39f5abaedac94b7086911410.png
--rw-r--r--   0 runner     (501) staff       (20)     1275 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/908a083a0806ab219190adac99ec60da04c65f48.png
--rw-r--r--   0 runner     (501) staff       (20)      253 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/9098c1c4618d7a0f321cee441aabee7f1b57a19b.png
--rw-r--r--   0 runner     (501) staff       (20)      278 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/90cab5ae70bdb6e45756490226ba488f522c4c4e.png
--rw-r--r--   0 runner     (501) staff       (20)      966 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/9173aacc17760942bd0ce61e5ad70788a84297d5.png
--rw-r--r--   0 runner     (501) staff       (20)      414 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/936adf4ee141541b19f32162898758c0de10fa8d.png
--rw-r--r--   0 runner     (501) staff       (20)     1327 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/957b97bc1591647fef3ac407dd3dd3e99c37fcd5.png
--rw-r--r--   0 runner     (501) staff       (20)     3108 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/95a6e48cc402e2e0cee2fe87d159320f12dcadfc.png
--rw-r--r--   0 runner     (501) staff       (20)     1186 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/95af1725828b1a188bbb0d933ffc78ef94788a48.png
--rw-r--r--   0 runner     (501) staff       (20)     1102 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/95c7fad2a12f832a0675a00c80c4a8894297d2b8.png
--rw-r--r--   0 runner     (501) staff       (20)      225 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/9630132210b904754c9ab272b61cb527d12263ca.png
--rw-r--r--   0 runner     (501) staff       (20)     1154 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/973e7149b3e7c5fd4b7a92e36771cc6c2d6e620b.png
--rw-r--r--   0 runner     (501) staff       (20)      233 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/97f89cf71150cd2020df53f6aabca4a64f63eb5f.png
--rw-r--r--   0 runner     (501) staff       (20)      216 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/9b444cf6329a14140aee8ff5a06ff30772cc1c2f.png
--rw-r--r--   0 runner     (501) staff       (20)      305 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/9de723874f4fca54fc9d4a4bf2f19c1b305b5a74.png
--rw-r--r--   0 runner     (501) staff       (20)     2290 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/9f18ba54fa478c728e3a3536166f874c17aa7c04.png
--rw-r--r--   0 runner     (501) staff       (20)      625 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/9f2f3a7e9359d5459533e3d50282ebae0ca36465.png
--rw-r--r--   0 runner     (501) staff       (20)     3918 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/a121b0efd1dfa559be59e332b528608d97906c46.png
--rw-r--r--   0 runner     (501) staff       (20)     1143 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/a133c9dd8091526f677cfcc502fbf773387d84bf.png
--rw-r--r--   0 runner     (501) staff       (20)      379 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/a156920bb8825b9428df86c5bfe4e3ce5b51f0f8.png
--rw-r--r--   0 runner     (501) staff       (20)      536 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/a38b44a27c1755531418f8bb853736ab038d7e9e.png
--rw-r--r--   0 runner     (501) staff       (20)     1265 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/a444daac219907b51a5edd730d624c53328d693f.png
--rw-r--r--   0 runner     (501) staff       (20)      258 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/a44c09dc69d687fd66b7a1a12197c0299aa5db1c.png
--rw-r--r--   0 runner     (501) staff       (20)     1340 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/a4594eb66f65c9a3e69736f82fdb072d08b8ddcc.png
--rw-r--r--   0 runner     (501) staff       (20)      413 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/a45d21a76729b863a1a60fe7ebb40a96a4ec69e5.png
--rw-r--r--   0 runner     (501) staff       (20)     7041 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/a5d23ddad04b332c54e468fd62d6493589d61339.png
--rw-r--r--   0 runner     (501) staff       (20)     1453 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/a6b6966ce67e827face4426ab49db20ec6a74a9e.png
--rw-r--r--   0 runner     (501) staff       (20)     1612 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/a810215e77878dec996b87e0d3007d8a6ded6b3c.png
--rw-r--r--   0 runner     (501) staff       (20)     1119 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/aa4d3057edd3aea1af61b5571a9e06258b978843.png
--rw-r--r--   0 runner     (501) staff       (20)      486 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/aadbbd5ab63719ff3a6c78a984dd3702cf3174c7.png
--rw-r--r--   0 runner     (501) staff       (20)      722 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/aaf1e4f8649093b3b1a2a201c97238b5d922ff96.png
--rw-r--r--   0 runner     (501) staff       (20)     1465 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/aaf2039a0ca644d308dc578303aa096fd3775907.png
--rw-r--r--   0 runner     (501) staff       (20)     5186 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/ab466a647f375d548d3b12c0c1ecb79704cef8d0.png
--rw-r--r--   0 runner     (501) staff       (20)      313 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/ac0d697baa79826d5fa42ee6fb1be506ff2ac3f8.png
--rw-r--r--   0 runner     (501) staff       (20)     1569 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/ac5ad3214d3caf44e5cc4e9514908ba2a7bb48dc.png
--rw-r--r--   0 runner     (501) staff       (20)      414 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/acc14817c5834249a732434e2919dfd4f708fffc.png
--rw-r--r--   0 runner     (501) staff       (20)     1358 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/ad2c8101af3f233ceefa1ec6865721f302b84cfd.png
--rw-r--r--   0 runner     (501) staff       (20)     1215 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/ae4ca00a7da101aa137fa6b84b5467ce39b05349.png
--rw-r--r--   0 runner     (501) staff       (20)     1601 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/ae6d9abfed9fac62837d0c88a97a8afc81b5e712.png
--rw-r--r--   0 runner     (501) staff       (20)      479 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/b0f4d6da17f2d5db3b4617e0e0d14eaf0b976b4b.png
--rw-r--r--   0 runner     (501) staff       (20)      418 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/b24f57eba06df79d80853a953d7805ab789ce829.png
--rw-r--r--   0 runner     (501) staff       (20)     1708 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/b3b09dbd48529f16a62f1020d2172bb9551e3296.png
--rw-r--r--   0 runner     (501) staff       (20)     2190 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/b6c16fed84a824ab88468f81a2b505ac69ad7505.png
--rw-r--r--   0 runner     (501) staff       (20)      245 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/b7dd8acc0d0af36b58c42bc14eeeca05c6286fba.png
--rw-r--r--   0 runner     (501) staff       (20)     1796 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/b7e4addc1a00973125d6c3b9ba5bd951e6486df5.png
--rw-r--r--   0 runner     (501) staff       (20)     1406 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/b8c391eb9c602cc714b875704be76879e335e243.png
--rw-r--r--   0 runner     (501) staff       (20)      633 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/b934c490f51b68bde94c85bb2c77c160a78731bc.png
--rw-r--r--   0 runner     (501) staff       (20)      251 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/b988975be41fd13b4d091c10202ba19374643586.png
--rw-r--r--   0 runner     (501) staff       (20)     4780 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/b9f9b8057126c1f181b745e36de7f60ecbe4e41d.png
--rw-r--r--   0 runner     (501) staff       (20)      237 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/badad346f6fbe2e237af99bfbd9a93a4da53a3da.png
--rw-r--r--   0 runner     (501) staff       (20)      886 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/bc28eed8cb92072618037ffe78d36cdf031045b0.png
--rw-r--r--   0 runner     (501) staff       (20)      496 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/bc7ea4e9d78396e86d86c117f1b22f739b77aa10.png
--rw-r--r--   0 runner     (501) staff       (20)      291 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/bca8217ac2efcad7312d6e496b4e4c82d8d179f6.png
--rw-r--r--   0 runner     (501) staff       (20)     1574 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/bcfcc32ea50d37180cedf362db80a4901cbc05bd.png
--rw-r--r--   0 runner     (501) staff       (20)      760 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/bd041563b2dc47337d212c089f31e14b6b95e033.png
--rw-r--r--   0 runner     (501) staff       (20)      348 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/bd466edf158386c56b457fb6aeb74b97766afdc6.png
--rw-r--r--   0 runner     (501) staff       (20)     1472 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/c0ff36623c1ad325126fbebd6724e58809c4fdd2.png
--rw-r--r--   0 runner     (501) staff       (20)     1361 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/c20519763e75b58870bd25238b358057e2da4b86.png
--rw-r--r--   0 runner     (501) staff       (20)      247 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/c2aa3dff9bffb099e9dff196fd36aed56ec16baf.png
--rw-r--r--   0 runner     (501) staff       (20)     1284 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/c34401e75e80cc822827c5d5175de08a5bbffced.png
--rw-r--r--   0 runner     (501) staff       (20)     2099 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/c72b037a60f8e81dc19add786e6d148794471f80.png
--rw-r--r--   0 runner     (501) staff       (20)     1220 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/c7fb856181b7b0b9f3cf0ca66c11fe63ea2b7278.png
--rw-r--r--   0 runner     (501) staff       (20)      292 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/c8ed607e197ca518179a4030e6aed34c1d339e7e.png
--rw-r--r--   0 runner     (501) staff       (20)     1643 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/c94d8558b73b7597cc60b6a0ec7c758f40c88a8d.png
--rw-r--r--   0 runner     (501) staff       (20)      737 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/c9a3af023076f58fe1ee0b35f88cad484ba194fa.png
--rw-r--r--   0 runner     (501) staff       (20)      266 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/cb5de54f699cf4b3c7c1a3e87313d11d536c0d88.png
--rw-r--r--   0 runner     (501) staff       (20)      340 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/cb92702d2163f15e2bf7e6a34b182302ae65f3b7.png
--rw-r--r--   0 runner     (501) staff       (20)      279 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/cbb49321318d94ba656d1ce115187d55c90322b4.png
--rw-r--r--   0 runner     (501) staff       (20)      231 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/cc87ee665749db882f94e0d3707eb23e39638650.png
--rw-r--r--   0 runner     (501) staff       (20)     1834 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/ccfd8c814cc1234e5dc5fce8871570757d15515c.png
--rw-r--r--   0 runner     (501) staff       (20)     1308 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/cd4c2f3674b5e0def3984a035f720209c8391074.png
--rw-r--r--   0 runner     (501) staff       (20)      720 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/d2241f81f782d8593f9390f06af621fd3be21ab8.png
--rw-r--r--   0 runner     (501) staff       (20)     1383 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/d246dde9fc63993c5b8df2eaccfa78ef89ad875d.png
--rw-r--r--   0 runner     (501) staff       (20)     1041 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/d33cbbeb57b535cc4b2562e25475f7afc74ae85b.png
--rw-r--r--   0 runner     (501) staff       (20)     1909 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/d3b5cc5b170fbda975293f38dea08b951f37142f.png
--rw-r--r--   0 runner     (501) staff       (20)     1388 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/d452b345239711d0be1016ccde4ddfea5930b072.png
--rw-r--r--   0 runner     (501) staff       (20)     2019 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/d504b5e2a3245798a6ad5678ea1951fc914e8fac.png
--rw-r--r--   0 runner     (501) staff       (20)      572 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/d56da07a3d18c9fc980ecc0a9696603bd8d8dcd2.png
--rw-r--r--   0 runner     (501) staff       (20)     1461 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/d5a4cdcdf8e599dc8e0d8a8c1301f02f9e8b4fb3.png
--rw-r--r--   0 runner     (501) staff       (20)      937 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/d66b4ab25c0eef60d649ef489104789f43f45a0b.png
--rw-r--r--   0 runner     (501) staff       (20)      430 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/d706fc3d557d35b283be36ac9e240324b68b34b9.png
--rw-r--r--   0 runner     (501) staff       (20)     3059 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/d767754db8d214ccf0dcaf05b48317d378fbddb5.png
--rw-r--r--   0 runner     (501) staff       (20)      273 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/d907a3c4e1257ec91ba2b8475cc048392650b648.png
--rw-r--r--   0 runner     (501) staff       (20)     1380 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/d9aec1e99d1bcb92578727e61fb60d877c0964b7.png
--rw-r--r--   0 runner     (501) staff       (20)      581 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/da8dad38c611fbd068672223f3f152e89ee7477e.png
--rw-r--r--   0 runner     (501) staff       (20)      261 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/db5b465a483d35549d1b8a4577cc4163f9ece3aa.png
--rw-r--r--   0 runner     (501) staff       (20)      302 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/db7426d70cdd8a4c33c3f1b8f7bdc9ba1b62c43a.png
--rw-r--r--   0 runner     (501) staff       (20)     1353 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/dba423937c7e0c09118ccac03f01a4a3be60e2c3.png
--rw-r--r--   0 runner     (501) staff       (20)     1898 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/dcab68360c480e6aaf0001fa1fb3f6451ba747f0.png
--rw-r--r--   0 runner     (501) staff       (20)     2686 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/deb40d5eca48a271c62dc3937746712359cd3b05.png
--rw-r--r--   0 runner     (501) staff       (20)      304 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/e00cdcd92f7a9d17060f49d50fad98569a249cd0.png
--rw-r--r--   0 runner     (501) staff       (20)      277 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/e00d4db37b602d888e9a5f2bc30bb8ad68d14ce9.png
--rw-r--r--   0 runner     (501) staff       (20)     1855 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/e2f6bbba20da0d51564b1855eb2da3072d841441.png
--rw-r--r--   0 runner     (501) staff       (20)     1088 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/e35d7cbe33a34f4456eea34b9bd28642bfc52fa4.png
--rw-r--r--   0 runner     (501) staff       (20)      858 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/e3a50552a1b736116240d899eea184ca3106ba0c.png
--rw-r--r--   0 runner     (501) staff       (20)      948 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/e3f4c5bf9e0470ceafd97d572163a4dfefc39743.png
--rw-r--r--   0 runner     (501) staff       (20)      414 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/e44d29f0cbcc5fa7a0f3f83d3bddc988f9b022ea.png
--rw-r--r--   0 runner     (501) staff       (20)      248 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/e4762cec46619bf7781cae62216214f909395368.png
--rw-r--r--   0 runner     (501) staff       (20)     1025 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/e50141a6a4a3490d1acc94e54f7de36ac5f7e8eb.png
--rw-r--r--   0 runner     (501) staff       (20)      298 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/e55e27c7fb666f42abe96fbf168eddf1fa6c9eb2.png
--rw-r--r--   0 runner     (501) staff       (20)      774 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/e61f71e6c396a94105e3437275d3449a61f9d802.png
--rw-r--r--   0 runner     (501) staff       (20)      446 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/e71fcd98134a69534acee44a765e20abefe6e316.png
--rw-r--r--   0 runner     (501) staff       (20)      237 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/e8dea8254118f111b5fb20895b03528c17566f06.png
--rw-r--r--   0 runner     (501) staff       (20)     1097 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/e97fe83d126fdd192e9bc593cea89698fb36ffe5.png
--rw-r--r--   0 runner     (501) staff       (20)      243 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/e9bc7da808d33a16a8347f27a519bd067186aa66.png
--rw-r--r--   0 runner     (501) staff       (20)      465 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/eb21ee2e4d5e09a543f19ff14ce49d682ad586af.png
--rw-r--r--   0 runner     (501) staff       (20)     1609 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/eb873a106ad1868e288ae26783dd930d360fdef5.png
--rw-r--r--   0 runner     (501) staff       (20)      164 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/ecdff306b10b7e2991a2c20df2fccba0f947155b.png
--rw-r--r--   0 runner     (501) staff       (20)     1665 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/ed29c4b1667b0282bad6523664351811e0f23dab.png
--rw-r--r--   0 runner     (501) staff       (20)      254 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/ed38fa24f1c94891bd312012aab3f6673be3eb83.png
--rw-r--r--   0 runner     (501) staff       (20)      252 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/ed7fb0260e58d3ca5851e823ff991dae4cde5671.png
--rw-r--r--   0 runner     (501) staff       (20)     1235 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/ee3c949541ac51ceadec0a62713cdd8a42a2e4ab.png
--rw-r--r--   0 runner     (501) staff       (20)      438 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/ef10ae5e9279f912e2a62fa15fc274fee32bb7d1.png
--rw-r--r--   0 runner     (501) staff       (20)     1340 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/efe5c37bc03bf3d5826fd02dc5b43a0a51e7c271.png
--rw-r--r--   0 runner     (501) staff       (20)      414 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/f2cb671262e4538a530f4241ee603253c3e01118.png
--rw-r--r--   0 runner     (501) staff       (20)      375 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/f3a047615f8cef5f6ce18b309a433eb73ef8e13b.png
--rw-r--r--   0 runner     (501) staff       (20)    11364 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/f59b4bcd76f97da1f13ba87bc76bf52b442b4381.png
--rw-r--r--   0 runner     (501) staff       (20)     3798 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/f86c7a0b45da8cc7f4a00c20bf654b3df94ff06a.png
--rw-r--r--   0 runner     (501) staff       (20)      747 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/facdb23d2bcdc9cf5d90ab695c86965ac188e3e5.png
--rw-r--r--   0 runner     (501) staff       (20)     4014 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/fb07faac9fe824b206392c19b7a1a2c6dd70e1ee.png
--rw-r--r--   0 runner     (501) staff       (20)     1457 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/fc16f4da2e0dd685363c204baf675d6244c52fbb.png
--rw-r--r--   0 runner     (501) staff       (20)      248 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/fc18e7de656eaf3eacbb104912233162cf9042e4.png
--rw-r--r--   0 runner     (501) staff       (20)     2030 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/fcc17fd59806862a629796f0d7f0e8f43778e7bd.png
--rw-r--r--   0 runner     (501) staff       (20)     2610 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/math/fe748f1ddebc2719b738533481dc2070aa3f8b04.png
--rw-r--r--   0 runner     (501) staff       (20)    24912 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/normappr.png
--rw-r--r--   0 runner     (501) staff       (20)    46408 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/portfolio1.png
--rw-r--r--   0 runner     (501) staff       (20)    28141 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_images/portfolio2.png
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-10-16 17:59:18.566532 kvxopt-1.3.2.0/doc/html/_static/
--rw-r--r--   0 runner     (501) staff       (20)     4418 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0 runner     (501) staff       (20)    15280 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_static/basic.css
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-10-16 17:59:18.567660 kvxopt-1.3.2.0/doc/html/_static/css/
--rw-r--r--   0 runner     (501) staff       (20)     3275 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_static/css/badge_only.css
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-10-16 17:59:18.586763 kvxopt-1.3.2.0/doc/html/_static/css/fonts/
--rw-r--r--   0 runner     (501) staff       (20)    87624 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0 runner     (501) staff       (20)    67312 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0 runner     (501) staff       (20)    86288 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0 runner     (501) staff       (20)    66444 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0 runner     (501) staff       (20)   165742 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0 runner     (501) staff       (20)   444379 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0 runner     (501) staff       (20)   165548 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 runner     (501) staff       (20)    98024 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0 runner     (501) staff       (20)    77160 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 runner     (501) staff       (20)   323344 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0 runner     (501) staff       (20)   193308 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0 runner     (501) staff       (20)   309728 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_static/css/fonts/lato-bold.woff
--rw-r--r--   0 runner     (501) staff       (20)   184912 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_static/css/fonts/lato-bold.woff2
--rw-r--r--   0 runner     (501) staff       (20)   328412 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0 runner     (501) staff       (20)   195704 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0 runner     (501) staff       (20)   309192 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_static/css/fonts/lato-normal.woff
--rw-r--r--   0 runner     (501) staff       (20)   182708 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_static/css/fonts/lato-normal.woff2
--rw-r--r--   0 runner     (501) staff       (20)   129674 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_static/css/theme.css
--rw-r--r--   0 runner     (501) staff       (20)    11060 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_static/cvxopt.css
--rw-r--r--   0 runner     (501) staff       (20)     8171 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_static/doctools.js
--rw-r--r--   0 runner     (501) staff       (20)      423 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_static/documentation_options.js
--rw-r--r--   0 runner     (501) staff       (20)      286 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_static/file.png
--rw-r--r--   0 runner     (501) staff       (20)   288580 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_static/jquery-3.6.0.js
--rw-r--r--   0 runner     (501) staff       (20)    89501 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_static/jquery.js
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-10-16 17:59:18.589573 kvxopt-1.3.2.0/doc/html/_static/js/
--rw-r--r--   0 runner     (501) staff       (20)      934 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_static/js/badge_only.js
--rw-r--r--   0 runner     (501) staff       (20)     4370 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_static/js/html5shiv-printshiv.min.js
--rw-r--r--   0 runner     (501) staff       (20)     2734 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_static/js/html5shiv.min.js
--rw-r--r--   0 runner     (501) staff       (20)     5023 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_static/js/theme.js
--rw-r--r--   0 runner     (501) staff       (20)     4758 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_static/language_data.js
--rw-r--r--   0 runner     (501) staff       (20)       90 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_static/minus.png
--rw-r--r--   0 runner     (501) staff       (20)       90 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_static/plus.png
--rw-r--r--   0 runner     (501) staff       (20)     4919 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_static/pygments.css
--rw-r--r--   0 runner     (501) staff       (20)    17088 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_static/searchtools.js
--rw-r--r--   0 runner     (501) staff       (20)    68420 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_static/underscore-1.13.1.js
--rw-r--r--   0 runner     (501) staff       (20)    19530 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/_static/underscore.js
--rw-r--r--   0 runner     (501) staff       (20)   104767 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/blas.html
--rw-r--r--   0 runner     (501) staff       (20)    38735 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/c-api.html
--rw-r--r--   0 runner     (501) staff       (20)   233726 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/coneprog.html
--rw-r--r--   0 runner     (501) staff       (20)     6580 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/copyright.html
--rw-r--r--   0 runner     (501) staff       (20)    23074 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/fftw.html
--rw-r--r--   0 runner     (501) staff       (20)    13377 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/index.html
--rw-r--r--   0 runner     (501) staff       (20)    11425 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/intro.html
--rw-r--r--   0 runner     (501) staff       (20)   236474 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/lapack.html
--rw-r--r--   0 runner     (501) staff       (20)   155220 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/matrices.html
--rw-r--r--   0 runner     (501) staff       (20)    90620 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/modeling.html
--rw-r--r--   0 runner     (501) staff       (20)     1942 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/objects.inv
--rw-r--r--   0 runner     (501) staff       (20)    18961 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/printing.html
--rw-r--r--   0 runner     (501) staff       (20)     5157 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/search.html
--rw-r--r--   0 runner     (501) staff       (20)    40104 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/searchindex.js
--rw-r--r--   0 runner     (501) staff       (20)   154192 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/solvers.html
--rw-r--r--   0 runner     (501) staff       (20)    81016 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/html/spsolvers.html
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-10-16 17:59:18.604079 kvxopt-1.3.2.0/doc/source/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-10-16 17:59:18.605022 kvxopt-1.3.2.0/doc/source/.static/
--rw-r--r--   0 runner     (501) staff       (20)    11060 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/source/.static/cvxopt.css
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-10-16 17:59:18.605499 kvxopt-1.3.2.0/doc/source/.templates/
--rw-r--r--   0 runner     (501) staff       (20)      436 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/source/.templates/layout.html
--rw-r--r--   0 runner     (501) staff       (20)    34002 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/source/blas.rst
--rw-r--r--   0 runner     (501) staff       (20)     7802 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/source/c-api.rst
--rw-r--r--   0 runner     (501) staff       (20)    77236 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/source/coneprog.rst
--rw-r--r--   0 runner     (501) staff       (20)     6008 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/source/conf.py
--rw-r--r--   0 runner     (501) staff       (20)      848 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/source/copyright.rst
--rw-r--r--   0 runner     (501) staff       (20)     7172 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/source/fftw.rst
--rw-r--r--   0 runner     (501) staff       (20)     9062 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/source/floorplan.png
--rw-r--r--   0 runner     (501) staff       (20)      448 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/source/index.rst
--rw-r--r--   0 runner     (501) staff       (20)     3116 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/source/intro.rst
--rw-r--r--   0 runner     (501) staff       (20)    60668 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/source/lapack.rst
--rw-r--r--   0 runner     (501) staff       (20)    44308 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/source/matrices.rst
--rw-r--r--   0 runner     (501) staff       (20)    25482 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/source/modeling.rst
--rw-r--r--   0 runner     (501) staff       (20)    24912 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/source/normappr.png
--rw-r--r--   0 runner     (501) staff       (20)    46408 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/source/portfolio1.png
--rw-r--r--   0 runner     (501) staff       (20)    28141 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/source/portfolio2.png
--rw-r--r--   0 runner     (501) staff       (20)     4952 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/source/printing.rst
--rw-r--r--   0 runner     (501) staff       (20)    47718 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/source/solvers.rst
--rw-r--r--   0 runner     (501) staff       (20)    32751 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/doc/source/spsolvers.rst
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-10-16 17:59:18.281357 kvxopt-1.3.2.0/examples/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-10-16 17:59:18.606135 kvxopt-1.3.2.0/examples/book/
--rw-r--r--   0 runner     (501) staff       (20)      271 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/book/README
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-10-16 17:59:18.608789 kvxopt-1.3.2.0/examples/book/chap4/
--rwxr-xr-x   0 runner     (501) staff       (20)     1957 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/book/chap4/portfolio.py
--rw-r--r--   0 runner     (501) staff       (20)    26660 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/book/chap4/rls.bin
--rwxr-xr-x   0 runner     (501) staff       (20)     2317 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/book/chap4/rls.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-10-16 17:59:18.621318 kvxopt-1.3.2.0/examples/book/chap6/
--rwxr-xr-x   0 runner     (501) staff       (20)     7364 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/book/chap6/basispursuit.py
--rwxr-xr-x   0 runner     (501) staff       (20)     4365 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/book/chap6/consumerpref.py
--rw-r--r--   0 runner     (501) staff       (20)     2190 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/book/chap6/cvxfit.bin
--rwxr-xr-x   0 runner     (501) staff       (20)     1524 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/book/chap6/cvxfit.py
--rw-r--r--   0 runner     (501) staff       (20)     1965 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/book/chap6/huber.bin
--rwxr-xr-x   0 runner     (501) staff       (20)     1956 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/book/chap6/huber.py
--rwxr-xr-x   0 runner     (501) staff       (20)     2193 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/book/chap6/inputdesign.py
--rwxr-xr-x   0 runner     (501) staff       (20)     2497 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/book/chap6/penalties.py
--rw-r--r--   0 runner     (501) staff       (20)     1996 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/book/chap6/polapprox.bin
--rwxr-xr-x   0 runner     (501) staff       (20)     4407 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/book/chap6/polapprox.py
--rw-r--r--   0 runner     (501) staff       (20)     5006 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/book/chap6/regsel.bin
--rwxr-xr-x   0 runner     (501) staff       (20)     3518 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/book/chap6/regsel.py
--rw-r--r--   0 runner     (501) staff       (20)    83504 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/book/chap6/robls.bin
--rwxr-xr-x   0 runner     (501) staff       (20)     4398 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/book/chap6/robls.py
--rwxr-xr-x   0 runner     (501) staff       (20)     2807 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/book/chap6/smoothrec.py
--rwxr-xr-x   0 runner     (501) staff       (20)     9117 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/book/chap6/tv.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-10-16 17:59:18.625131 kvxopt-1.3.2.0/examples/book/chap7/
--rwxr-xr-x   0 runner     (501) staff       (20)     3253 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/book/chap7/chernoff.py
--rwxr-xr-x   0 runner     (501) staff       (20)     5122 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/book/chap7/expdesign.py
--rw-r--r--   0 runner     (501) staff       (20)     2842 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/book/chap7/logreg.bin
--rwxr-xr-x   0 runner     (501) staff       (20)     1241 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/book/chap7/logreg.py
--rwxr-xr-x   0 runner     (501) staff       (20)     2718 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/book/chap7/maxent.py
--rwxr-xr-x   0 runner     (501) staff       (20)     6681 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/book/chap7/probbounds.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-10-16 17:59:18.628745 kvxopt-1.3.2.0/examples/book/chap8/
--rwxr-xr-x   0 runner     (501) staff       (20)     6223 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/book/chap8/centers.py
--rwxr-xr-x   0 runner     (501) staff       (20)     7142 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/book/chap8/ellipsoids.py
--rwxr-xr-x   0 runner     (501) staff       (20)     6268 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/book/chap8/floorplan.py
--rw-r--r--   0 runner     (501) staff       (20)     4657 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/book/chap8/linsep.bin
--rwxr-xr-x   0 runner     (501) staff       (20)     3797 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/book/chap8/linsep.py
--rw-r--r--   0 runner     (501) staff       (20)      783 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/book/chap8/placement.bin
--rwxr-xr-x   0 runner     (501) staff       (20)     5160 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/book/chap8/placement.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-10-16 17:59:18.629252 kvxopt-1.3.2.0/examples/doc/
--rw-r--r--   0 runner     (501) staff       (20)      267 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/doc/README
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-10-16 17:59:18.631737 kvxopt-1.3.2.0/examples/doc/chap10/
--rwxr-xr-x   0 runner     (501) staff       (20)      507 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/doc/chap10/l1svc.py
--rwxr-xr-x   0 runner     (501) staff       (20)     1169 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/doc/chap10/lp.py
--rwxr-xr-x   0 runner     (501) staff       (20)      694 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/doc/chap10/normappr.py
--rwxr-xr-x   0 runner     (501) staff       (20)      515 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/doc/chap10/roblp.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-10-16 17:59:18.632294 kvxopt-1.3.2.0/examples/doc/chap4/
--rwxr-xr-x   0 runner     (501) staff       (20)     1865 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/doc/chap4/acent.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-10-16 17:59:18.634133 kvxopt-1.3.2.0/examples/doc/chap7/
--rw-r--r--   0 runner     (501) staff       (20)    62593 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/doc/chap7/covsel.bin
--rwxr-xr-x   0 runner     (501) staff       (20)     2486 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/doc/chap7/covsel.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-10-16 17:59:18.640531 kvxopt-1.3.2.0/examples/doc/chap8/
--rwxr-xr-x   0 runner     (501) staff       (20)      851 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/doc/chap8/conelp.py
--rwxr-xr-x   0 runner     (501) staff       (20)      634 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/doc/chap8/coneqp.py
--rwxr-xr-x   0 runner     (501) staff       (20)     3999 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/doc/chap8/l1.py
--rwxr-xr-x   0 runner     (501) staff       (20)     4373 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/doc/chap8/l1regls.py
--rwxr-xr-x   0 runner     (501) staff       (20)      271 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/doc/chap8/lp.py
--rwxr-xr-x   0 runner     (501) staff       (20)     3335 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/doc/chap8/mcsdp.py
--rwxr-xr-x   0 runner     (501) staff       (20)     1941 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/doc/chap8/portfolio.py
--rwxr-xr-x   0 runner     (501) staff       (20)     4254 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/doc/chap8/qcl1.py
--rwxr-xr-x   0 runner     (501) staff       (20)      741 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/doc/chap8/sdp.py
--rwxr-xr-x   0 runner     (501) staff       (20)      527 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/doc/chap8/socp.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-10-16 17:59:18.644269 kvxopt-1.3.2.0/examples/doc/chap9/
--rwxr-xr-x   0 runner     (501) staff       (20)     1000 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/doc/chap9/acent.py
--rwxr-xr-x   0 runner     (501) staff       (20)      970 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/doc/chap9/acent2.py
--rwxr-xr-x   0 runner     (501) staff       (20)     6264 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/doc/chap9/floorplan.py
--rwxr-xr-x   0 runner     (501) staff       (20)      589 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/doc/chap9/gp.py
--rwxr-xr-x   0 runner     (501) staff       (20)     2163 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/doc/chap9/l2ac.py
--rwxr-xr-x   0 runner     (501) staff       (20)     1335 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/doc/chap9/robls.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-10-16 17:59:18.645897 kvxopt-1.3.2.0/examples/filterdemo/
--rw-r--r--   0 runner     (501) staff       (20)      457 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/filterdemo/README
--rwxr-xr-x   0 runner     (501) staff       (20)     3679 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/filterdemo/filterdemo_cli
--rwxr-xr-x   0 runner     (501) staff       (20)     7387 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/examples/filterdemo/filterdemo_gui
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-10-16 17:59:18.649016 kvxopt-1.3.2.0/kvxopt.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     1592 2023-10-16 17:59:17.000000 kvxopt-1.3.2.0/kvxopt.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)    28686 2023-10-16 17:59:18.000000 kvxopt-1.3.2.0/kvxopt.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-10-16 17:59:17.000000 kvxopt-1.3.2.0/kvxopt.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-10-16 17:59:17.000000 kvxopt-1.3.2.0/kvxopt.egg-info/not-zip-safe
--rw-r--r--   0 runner     (501) staff       (20)       61 2023-10-16 17:59:17.000000 kvxopt-1.3.2.0/kvxopt.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)      204 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/pyproject.toml
--rw-r--r--   0 runner     (501) staff       (20)      148 2023-10-16 17:59:18.692447 kvxopt-1.3.2.0/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)    17484 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-10-16 17:59:18.282087 kvxopt-1.3.2.0/src/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-10-16 17:59:18.662018 kvxopt-1.3.2.0/src/C/
--rw-r--r--   0 runner     (501) staff       (20)     7703 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/src/C/amd.c
--rw-r--r--   0 runner     (501) staff       (20)    68958 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/src/C/base.c
--rw-r--r--   0 runner     (501) staff       (20)   139358 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/src/C/blas.c
--rw-r--r--   0 runner     (501) staff       (20)     3543 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/src/C/blas_redefines.h
--rw-r--r--   0 runner     (501) staff       (20)    36999 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/src/C/cholmod.c
--rw-r--r--   0 runner     (501) staff       (20)     5442 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/src/C/cvxopt.h
--rw-r--r--   0 runner     (501) staff       (20)    75347 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/src/C/dense.c
--rw-r--r--   0 runner     (501) staff       (20)    19626 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/src/C/dsdp.c
--rw-r--r--   0 runner     (501) staff       (20)    34318 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/src/C/fftw.c
--rw-r--r--   0 runner     (501) staff       (20)    42231 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/src/C/glpk.c
--rw-r--r--   0 runner     (501) staff       (20)     6978 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/src/C/gsl.c
--rw-r--r--   0 runner     (501) staff       (20)    23071 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/src/C/gurobi.c
--rw-r--r--   0 runner     (501) staff       (20)    28574 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/src/C/klu.c
--rw-r--r--   0 runner     (501) staff       (20)   281701 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/src/C/lapack.c
--rw-r--r--   0 runner     (501) staff       (20)     3535 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/src/C/misc.h
--rw-r--r--   0 runner     (501) staff       (20)    38101 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/src/C/misc_solvers.c
--rw-r--r--   0 runner     (501) staff       (20)    19197 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/src/C/osqp.c
--rw-r--r--   0 runner     (501) staff       (20)   141567 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/src/C/sparse.c
--rw-r--r--   0 runner     (501) staff       (20)    25015 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/src/C/umfpack.c
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-10-16 17:59:18.669803 kvxopt-1.3.2.0/src/python/
--rw-r--r--   0 runner     (501) staff       (20)    10614 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/src/python/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      416 2023-10-16 17:59:17.000000 kvxopt-1.3.2.0/src/python/_version.py
--rw-r--r--   0 runner     (501) staff       (20)   172008 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/src/python/coneprog.py
--rw-r--r--   0 runner     (501) staff       (20)    83899 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/src/python/cvxprog.py
--rw-r--r--   0 runner     (501) staff       (20)      885 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/src/python/info.py
--rw-r--r--   0 runner     (501) staff       (20)    54949 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/src/python/misc.py
--rw-r--r--   0 runner     (501) staff       (20)   100979 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/src/python/modeling.py
--rw-r--r--   0 runner     (501) staff       (20)    37174 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/src/python/msk.py
--rw-r--r--   0 runner     (501) staff       (20)     5483 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/src/python/printing.py
--rw-r--r--   0 runner     (501) staff       (20)     1562 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/src/python/solvers.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-10-16 17:59:18.690771 kvxopt-1.3.2.0/tests/
--rw-r--r--   0 runner     (501) staff       (20)   778267 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/tests/ACTIVSg2000.mtx
--rw-r--r--   0 runner     (501) staff       (20)  1025924 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/tests/bcsstk13.mtx
--rw-r--r--   0 runner     (501) staff       (20)  2035740 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/tests/bcsstk24.mtx
--rw-r--r--   0 runner     (501) staff       (20)    48147 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/tests/boeing2.mps
--rw-r--r--   0 runner     (501) staff       (20)    55059 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/tests/bp_800.mtx
--rw-r--r--   0 runner     (501) staff       (20)     5487 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/tests/test_basic.py
--rw-r--r--   0 runner     (501) staff       (20)      772 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/tests/test_blas.py
--rw-r--r--   0 runner     (501) staff       (20)    11685 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/tests/test_custom_kkt.py
--rw-r--r--   0 runner     (501) staff       (20)     2206 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/tests/test_dsdp.py
--rw-r--r--   0 runner     (501) staff       (20)     2685 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/tests/test_examples.py
--rw-r--r--   0 runner     (501) staff       (20)     3160 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/tests/test_glpk.py
--rw-r--r--   0 runner     (501) staff       (20)      698 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/tests/test_gsl.py
--rw-r--r--   0 runner     (501) staff       (20)     4312 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/tests/test_gurobi.py
--rw-r--r--   0 runner     (501) staff       (20)     1791 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/tests/test_modeling.py
--rw-r--r--   0 runner     (501) staff       (20)     2516 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/tests/test_mosek.py
--rw-r--r--   0 runner     (501) staff       (20)     4706 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/tests/test_osqp.py
--rw-r--r--   0 runner     (501) staff       (20)     8799 2023-10-16 17:58:10.000000 kvxopt-1.3.2.0/tests/test_sparse_solvers.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-08 16:49:13.532658 kvxopt-1.3.2.1/
+-rw-r--r--   0 runner     (501) staff       (20)       36 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/.gitattributes
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-08 16:49:13.382535 kvxopt-1.3.2.1/.github/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-08 16:49:13.386700 kvxopt-1.3.2.1/.github/workflows/
+-rw-r--r--   0 runner     (501) staff       (20)     3196 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/.github/workflows/linux_build.yml
+-rw-r--r--   0 runner     (501) staff       (20)     3056 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/.github/workflows/macos_build.yml
+-rw-r--r--   0 runner     (501) staff       (20)    10620 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/.github/workflows/windows_build.yml
+-rw-r--r--   0 runner     (501) staff       (20)      169 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/.gitignore
+-rw-r--r--   0 runner     (501) staff       (20)     1472 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/INSTALL
+-rw-r--r--   0 runner     (501) staff       (20)     5807 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/Jenkinsfile
+-rw-r--r--   0 runner     (501) staff       (20)    35993 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)      217 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)     1592 2024-05-08 16:49:13.532944 kvxopt-1.3.2.1/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     2634 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-08 16:49:13.386819 kvxopt-1.3.2.1/doc/
+-rw-r--r--   0 runner     (501) staff       (20)     2321 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/Makefile
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-08 16:49:13.390541 kvxopt-1.3.2.1/doc/html/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-08 16:49:13.391259 kvxopt-1.3.2.1/doc/html/_images/
+-rw-r--r--   0 runner     (501) staff       (20)     9062 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/floorplan.png
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-08 16:49:13.456042 kvxopt-1.3.2.1/doc/html/_images/math/
+-rw-r--r--   0 runner     (501) staff       (20)      416 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/00b60df5731428a5a02b49ca7bc4d5aaa7afac9c.png
+-rw-r--r--   0 runner     (501) staff       (20)     1078 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/00e8f621cc91c8f430e504b66fb085743c4814cb.png
+-rw-r--r--   0 runner     (501) staff       (20)     1269 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/01824df8f8806530b722445b6f9cde3a8e732f07.png
+-rw-r--r--   0 runner     (501) staff       (20)      255 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/0202eb241774e15b6d1398f17dd161778e602b90.png
+-rw-r--r--   0 runner     (501) staff       (20)      494 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/022ccd45e165efaafd4897b98a41553943db3f05.png
+-rw-r--r--   0 runner     (501) staff       (20)      323 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/036001c78514c5de2ab5c899cb2b005a905ba3a5.png
+-rw-r--r--   0 runner     (501) staff       (20)      747 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/03cfea18434ec87caa164206e463d7a230e1cb5c.png
+-rw-r--r--   0 runner     (501) staff       (20)     1275 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/03da04b738c1b20d64d873e8f3c18eccc4c7bc84.png
+-rw-r--r--   0 runner     (501) staff       (20)     1538 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/04163b47432b93c2e42e10bab40066847581fc79.png
+-rw-r--r--   0 runner     (501) staff       (20)      405 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/04342bcceed278806ffa3c6deee7f762c50a6eab.png
+-rw-r--r--   0 runner     (501) staff       (20)     1331 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/04b02267d8a264913c39b04bf73ab88181b03cfc.png
+-rw-r--r--   0 runner     (501) staff       (20)     1400 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/056427854bd8d5a1fa428fff460d45b749aebc2a.png
+-rw-r--r--   0 runner     (501) staff       (20)      558 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/05c3b434aba8ec5e2ac1cdfcc3e3bb7ca8a69775.png
+-rw-r--r--   0 runner     (501) staff       (20)     7496 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/0667e780fc9b2d0fad01d14184553aba1cd6b81b.png
+-rw-r--r--   0 runner     (501) staff       (20)      341 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/06fa9ba19a3d38408ac220954e05a6105bec867c.png
+-rw-r--r--   0 runner     (501) staff       (20)      846 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/072b7c28c9bc48c8509301fcff6dfb5095db4a07.png
+-rw-r--r--   0 runner     (501) staff       (20)     1476 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/073b4fb9749f6ab5523c701bbe38a97c5fa94288.png
+-rw-r--r--   0 runner     (501) staff       (20)      372 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/07478b8108c1b9d0c0317e8bc57b8776263d0a85.png
+-rw-r--r--   0 runner     (501) staff       (20)     1057 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/0790b49262067229d1ce8165c4a66b4afa62cda9.png
+-rw-r--r--   0 runner     (501) staff       (20)     1317 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/081eab67b8ad47c824c773f9ce571fe5883895bf.png
+-rw-r--r--   0 runner     (501) staff       (20)      933 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/08390710b56f1bdd0cf7346dd20ee9b3a5984ea1.png
+-rw-r--r--   0 runner     (501) staff       (20)     3059 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/0b6da08d6fc1f85c1382af2c64a51fa0129e47fd.png
+-rw-r--r--   0 runner     (501) staff       (20)     1585 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/0b75ca09d0ef9d47484865bd353fc1e234d0ffae.png
+-rw-r--r--   0 runner     (501) staff       (20)     1616 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/0bf595687ae571b0147a101f606500879246b152.png
+-rw-r--r--   0 runner     (501) staff       (20)      849 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/0e7509809ae807b340e6d7cd64cc157ce0c8a4ff.png
+-rw-r--r--   0 runner     (501) staff       (20)     1359 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/0e95b3c9bb477c1d27aa253d83fe2d3e1922b3ef.png
+-rw-r--r--   0 runner     (501) staff       (20)      275 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/0edac3a6b0973196c5005c560d87e755c0ea5c86.png
+-rw-r--r--   0 runner     (501) staff       (20)      971 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/0f2f6181474c4d231456601880211909048d0548.png
+-rw-r--r--   0 runner     (501) staff       (20)     1667 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/0f36e4d687eeb224ee6593ac11df99a1d4451ba9.png
+-rw-r--r--   0 runner     (501) staff       (20)     1670 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/0fc13f815b495c77d502992ae392d16844c0950b.png
+-rw-r--r--   0 runner     (501) staff       (20)      263 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/0fcab9067b50b87e868c4fd70f213a086addb964.png
+-rw-r--r--   0 runner     (501) staff       (20)      205 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/106b04b320e75010b1d8029e59244f234f75e6f9.png
+-rw-r--r--   0 runner     (501) staff       (20)     1411 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/10d754c37b304c217ee6f80c9a3c4c7bcbbcba9d.png
+-rw-r--r--   0 runner     (501) staff       (20)     1467 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/11969d386f3f62d281586721cb47b9bc640ea082.png
+-rw-r--r--   0 runner     (501) staff       (20)      879 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/12354e7e046bba1f8384eebcc70a2d9a09930e8e.png
+-rw-r--r--   0 runner     (501) staff       (20)     5190 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/124ef7067b147c5c7f031fc0fc06a822029456c1.png
+-rw-r--r--   0 runner     (501) staff       (20)     1446 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/1337abb9748b0985f66823f48527ff07692b910a.png
+-rw-r--r--   0 runner     (501) staff       (20)     3584 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/13abf6ff1ab819235d06737ba4cc4b56c12cf29f.png
+-rw-r--r--   0 runner     (501) staff       (20)      237 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/141bbefb74014fc5e43499901bf78607ae335583.png
+-rw-r--r--   0 runner     (501) staff       (20)     1356 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/145a22013f61134f2b61c99bdc4bf56a23e7ba62.png
+-rw-r--r--   0 runner     (501) staff       (20)      358 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/146bec31bf294e89657786d59d21f9c4307ed72f.png
+-rw-r--r--   0 runner     (501) staff       (20)      629 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/15ccba8c9b68894aeb55e081c819b82da74b90ed.png
+-rw-r--r--   0 runner     (501) staff       (20)      300 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/161320f045cc4315c31907ec05fe170909e3c274.png
+-rw-r--r--   0 runner     (501) staff       (20)      259 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/166d5d3acaad3170290c97811491b74b32041dad.png
+-rw-r--r--   0 runner     (501) staff       (20)      414 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/172415a1aefbbb006e616ac35d880030890ad136.png
+-rw-r--r--   0 runner     (501) staff       (20)      295 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/183e9814ec579a80697d078963ce0412589322f1.png
+-rw-r--r--   0 runner     (501) staff       (20)     2470 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/191bc203fa207a53847c892bc9bc56a69a1c60c1.png
+-rw-r--r--   0 runner     (501) staff       (20)      239 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/19eef1966f7c545af3ac8c0fa486974d873e3c65.png
+-rw-r--r--   0 runner     (501) staff       (20)      400 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/1b1815f8a1dcb49152792554f110261420c96b3c.png
+-rw-r--r--   0 runner     (501) staff       (20)      241 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/1b5e577d6216dca3af7d87aa122a0b9b360d6cb3.png
+-rw-r--r--   0 runner     (501) staff       (20)      287 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/1cfcab44d097a385b6e2fb16cfefc2f062ab999f.png
+-rw-r--r--   0 runner     (501) staff       (20)      833 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/1e0371cc3025278f588fd7d0ccfcc2510ff2f8cf.png
+-rw-r--r--   0 runner     (501) staff       (20)      320 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/1e45a7a687f92b2a29b62ce1dddb23a8eefeedca.png
+-rw-r--r--   0 runner     (501) staff       (20)     2440 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/1e7e60bfda710d3db286c7b54852b9cb3e77c861.png
+-rw-r--r--   0 runner     (501) staff       (20)      337 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/1e913e459d7bcb538986828dad39d548fa73228f.png
+-rw-r--r--   0 runner     (501) staff       (20)      259 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/1ebe654cc7b8f2a0d8100aa5825cf2b9021adbbc.png
+-rw-r--r--   0 runner     (501) staff       (20)      269 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/1f2cf406b1224eb3a604895ac84524c6aed56983.png
+-rw-r--r--   0 runner     (501) staff       (20)      289 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/1fbee781f84569077719a167b64e12064360fac1.png
+-rw-r--r--   0 runner     (501) staff       (20)      244 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/211284f68205c3e66773eaf026f32a0acdd3dfb3.png
+-rw-r--r--   0 runner     (501) staff       (20)     1792 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/211a6aeaec6adf6a5dd8e0c7de1c4e9f4635ad25.png
+-rw-r--r--   0 runner     (501) staff       (20)     1858 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/21281aa0c6a6c01b835faeb9de4a5ba91527df33.png
+-rw-r--r--   0 runner     (501) staff       (20)     1325 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/2149e945c5e7e174b2a1146a3669a5a0b1c65f32.png
+-rw-r--r--   0 runner     (501) staff       (20)     1635 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/21f2b425bff574fa56ee14ddbb7517747adb4266.png
+-rw-r--r--   0 runner     (501) staff       (20)     1373 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/2211f73518e89008db8e07b1bb8a7b8881d0263f.png
+-rw-r--r--   0 runner     (501) staff       (20)     2344 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/23507579d8ee310e9bc7a287d88d48f8f5ab891f.png
+-rw-r--r--   0 runner     (501) staff       (20)      283 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/249b38285050bda51fd1579d716b5553f8114a0d.png
+-rw-r--r--   0 runner     (501) staff       (20)      513 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/26e45da42a12ddc160256fb6cbbb944eeba0dee8.png
+-rw-r--r--   0 runner     (501) staff       (20)     5636 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/2877bec99a56fcd4a3f6b39b56c2fe14acb7ee94.png
+-rw-r--r--   0 runner     (501) staff       (20)      614 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/294ea142766a27b4576f8c3240182c9220174aad.png
+-rw-r--r--   0 runner     (501) staff       (20)      730 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/296e9942f8952b0eda9b312b690a6662f47008e9.png
+-rw-r--r--   0 runner     (501) staff       (20)     1264 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/2ac45fcc15c7339cc8ecbdb592c53bc49bf33c73.png
+-rw-r--r--   0 runner     (501) staff       (20)     2921 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/2c0f91e60d2f13fdeba173121a264d745555e902.png
+-rw-r--r--   0 runner     (501) staff       (20)      567 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/2e7d885be2f8d9a7556b4e6dded7b42315803547.png
+-rw-r--r--   0 runner     (501) staff       (20)     1558 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/306121f2c5a959611abb74ce19acd25173d3cb33.png
+-rw-r--r--   0 runner     (501) staff       (20)     1595 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/3157de5f84013f57240cf058275c3ae9deb3287a.png
+-rw-r--r--   0 runner     (501) staff       (20)      330 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/317f05bfc503c0f2967f94d5108fa418a7e4578e.png
+-rw-r--r--   0 runner     (501) staff       (20)     1688 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/322793af4baec9f7ebaa53c4c21f4a468036799a.png
+-rw-r--r--   0 runner     (501) staff       (20)     2184 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/32cab048b453581f0ca59dc31e33e56b7c8b3a0e.png
+-rw-r--r--   0 runner     (501) staff       (20)      423 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/3352e62eefabf4e08a86652e339b0ef936c86ced.png
+-rw-r--r--   0 runner     (501) staff       (20)      932 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/340c54d7b4f301eb582e5ce306364e1cc4fe20b1.png
+-rw-r--r--   0 runner     (501) staff       (20)     1275 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/34a857941bc037025e34cfc7d5ddf0cba068c3f7.png
+-rw-r--r--   0 runner     (501) staff       (20)      450 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/36c1c1b5e868253601aefce353956d96322883ae.png
+-rw-r--r--   0 runner     (501) staff       (20)      524 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/36dfce98812a98045ee08f8608788e512eed0fe3.png
+-rw-r--r--   0 runner     (501) staff       (20)     3059 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/3725c3144c904e39aef17290ef9fdefa9e3adfe0.png
+-rw-r--r--   0 runner     (501) staff       (20)      994 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/37ab88a567d07e7cd18072c1f9878e17b26e1a6a.png
+-rw-r--r--   0 runner     (501) staff       (20)     1832 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/385dad5a2df2ddd65900bef4c4ab58d4a4a0829d.png
+-rw-r--r--   0 runner     (501) staff       (20)      452 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/38e9e9d3b438f8da362e850c8eb1c0252af8373a.png
+-rw-r--r--   0 runner     (501) staff       (20)     2384 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/3910830c8976bd5c91219274bd08ca0401852b45.png
+-rw-r--r--   0 runner     (501) staff       (20)     1430 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/39848b64dc282be81d51d8786746c0b13bd48bcc.png
+-rw-r--r--   0 runner     (501) staff       (20)     1693 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/3a138e23ab33c536c23ad13ff28606737fe7e610.png
+-rw-r--r--   0 runner     (501) staff       (20)      446 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/3ae50aaf765cd8eb0463a159845004ccae1c3cff.png
+-rw-r--r--   0 runner     (501) staff       (20)     1894 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/3b0de39a2c386bc0f8d5ee56519cab864e57d389.png
+-rw-r--r--   0 runner     (501) staff       (20)     1475 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/3b8df11e628aac991d176b270cf335fd89834cfc.png
+-rw-r--r--   0 runner     (501) staff       (20)      240 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/3bb6de8fbb6eb7f9723920dea5cd674c8c713f45.png
+-rw-r--r--   0 runner     (501) staff       (20)      263 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/3bfb3a64189a14b2704f4610827762d5e3145114.png
+-rw-r--r--   0 runner     (501) staff       (20)     4639 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/3f12bcd60dcbf296614984241c025a909a803e1e.png
+-rw-r--r--   0 runner     (501) staff       (20)      894 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/3f1dd94c34f67811ddb2df9812cfb065dea10aac.png
+-rw-r--r--   0 runner     (501) staff       (20)      546 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/3f7c5e248ea93d509e428921ea91f68e03f1b029.png
+-rw-r--r--   0 runner     (501) staff       (20)      528 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/3fb48872eb2d412f7878dd8934dab8823ce6422b.png
+-rw-r--r--   0 runner     (501) staff       (20)     1539 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/3fd3b9b7b701e9534c715081f10fd72d4c4670f6.png
+-rw-r--r--   0 runner     (501) staff       (20)     1204 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/42e6ff06c5afcf7438f6b7bd0027c3c738feceb6.png
+-rw-r--r--   0 runner     (501) staff       (20)      462 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/4357a4e29a351ac6ae90924cc00e06184fbd8412.png
+-rw-r--r--   0 runner     (501) staff       (20)      523 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/4568da7a353653545f711003d54f38db128766df.png
+-rw-r--r--   0 runner     (501) staff       (20)      330 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/459f00b80184047c37413367f1bc32570987f2c1.png
+-rw-r--r--   0 runner     (501) staff       (20)     1894 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/45ab4648d9d463e88b6a823609eaac81787d876f.png
+-rw-r--r--   0 runner     (501) staff       (20)     1323 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/45bf7a5d17860fe8ca50fd24ff910e00ce5f8a39.png
+-rw-r--r--   0 runner     (501) staff       (20)     1655 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/45ca0c9c05f16b36175b595487b17f411e30a5d6.png
+-rw-r--r--   0 runner     (501) staff       (20)     1855 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/46362a8b56ad9a6cb816f0062260ad22a76b6f08.png
+-rw-r--r--   0 runner     (501) staff       (20)      211 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/470aa65888a2971c9346e573f12b37ea406b8ec9.png
+-rw-r--r--   0 runner     (501) staff       (20)     1270 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/4786cdb10b56effd1cbd6730d8a8497748d072c0.png
+-rw-r--r--   0 runner     (501) staff       (20)      963 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/4798110dbfdeb1ecd95e4f30fe61ccf31ce4f503.png
+-rw-r--r--   0 runner     (501) staff       (20)     1025 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/482017ed70f2f392091ce55bf925c4d264ca15ba.png
+-rw-r--r--   0 runner     (501) staff       (20)     1626 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/485e65f87f30e5ab52138c945744fe97e6dd87dc.png
+-rw-r--r--   0 runner     (501) staff       (20)      891 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/487040712ec6e78e6ce843fdedb84752b97c2547.png
+-rw-r--r--   0 runner     (501) staff       (20)      234 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/4a3598141469c2555591e66606a1b86d4ec6dca9.png
+-rw-r--r--   0 runner     (501) staff       (20)      288 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/4abba779877abb276b98ccb2b4ba9bf2e41947ab.png
+-rw-r--r--   0 runner     (501) staff       (20)      321 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/4ac9a8351b68de952fda2e33246216aa5edb2818.png
+-rw-r--r--   0 runner     (501) staff       (20)      266 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/4bc3e94a67870b41b7c20179693e889251e2c136.png
+-rw-r--r--   0 runner     (501) staff       (20)      275 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/4bcdc64a07db3d7711bc2889fe6459e2ae4e65d6.png
+-rw-r--r--   0 runner     (501) staff       (20)      230 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/4c120f773ab4e1c59ad2bd44aae969ce24dd190a.png
+-rw-r--r--   0 runner     (501) staff       (20)     1495 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/4c8eef5c3334015a2ce256c6afde864dcac2b7ad.png
+-rw-r--r--   0 runner     (501) staff       (20)      245 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/4db5b6e16e06f929ce3f675c5e535d06ffb02ff7.png
+-rw-r--r--   0 runner     (501) staff       (20)      290 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/4dc6347ee63e4c699378bbfd3c9c00e328e6a91d.png
+-rw-r--r--   0 runner     (501) staff       (20)     1700 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/4e317307fb34d4308336c7711497db123b7d9def.png
+-rw-r--r--   0 runner     (501) staff       (20)     1693 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/4e3f3707720cdc0ad65a45a1568034b0499846a9.png
+-rw-r--r--   0 runner     (501) staff       (20)      412 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/4f58d165825711e6619115afb28c246c00440fa2.png
+-rw-r--r--   0 runner     (501) staff       (20)     1353 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/4f7be1be65d6087c8016b324e3d3e258e12f405d.png
+-rw-r--r--   0 runner     (501) staff       (20)     1299 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/5046b770f82749051a01f8f102c8e5ff69c4a3e4.png
+-rw-r--r--   0 runner     (501) staff       (20)      340 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/5052552450b786edab8e0415c96dfa848bc40be1.png
+-rw-r--r--   0 runner     (501) staff       (20)      263 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/52ddc0cde6d632f631533173562fe3ca375b1f32.png
+-rw-r--r--   0 runner     (501) staff       (20)     1623 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/54cbbb3d4691d21c5f1604825fce3e264ef4e7cb.png
+-rw-r--r--   0 runner     (501) staff       (20)     2151 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/55eedb919b02b7a0654137bd319d8bb919ad3067.png
+-rw-r--r--   0 runner     (501) staff       (20)     1554 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/56ac83c03464e42463c625f1f9ef1833a2927d2e.png
+-rw-r--r--   0 runner     (501) staff       (20)     2569 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/56ebcc22b7fc4da65f58f0819b21a4c7da613bd4.png
+-rw-r--r--   0 runner     (501) staff       (20)     1149 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/582940bfca19aac437939d3e7b6be8c577797dad.png
+-rw-r--r--   0 runner     (501) staff       (20)      446 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/5866199ac7f27f9fa8f345c8d6bd6f14fc869908.png
+-rw-r--r--   0 runner     (501) staff       (20)      286 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/58dfeba24c101319ed253c88f1b03e306ab30e1f.png
+-rw-r--r--   0 runner     (501) staff       (20)      228 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/5a939c5280da7202ca4531f175a7780ad5e1f80a.png
+-rw-r--r--   0 runner     (501) staff       (20)      239 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/5b7752c757e0b691a80ab8227eadb8a8389dc58a.png
+-rw-r--r--   0 runner     (501) staff       (20)     1703 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/5d759a9a1a42876f1cefe2c9fc361df2a167d545.png
+-rw-r--r--   0 runner     (501) staff       (20)      546 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/5dacf40fdb001db01bc47f5b86fcb7ce6dc4a0e2.png
+-rw-r--r--   0 runner     (501) staff       (20)     1809 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/5fa951f18d59f8caa1d2bc6ec81f6a0c945bfe75.png
+-rw-r--r--   0 runner     (501) staff       (20)      430 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/60d0a6fc7c07bee2dc81830096d4d310add8f5eb.png
+-rw-r--r--   0 runner     (501) staff       (20)     1256 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/61425e89ec518b2689e5063426419950648cd2dc.png
+-rw-r--r--   0 runner     (501) staff       (20)      824 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/61a7d25e3673146402ed26716d6eb60e8e9d18fa.png
+-rw-r--r--   0 runner     (501) staff       (20)     1574 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/620321226792601132c52174a5287a8c93e9bc5f.png
+-rw-r--r--   0 runner     (501) staff       (20)     1955 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/627d2d6ebe12e40470cbb763687cffb52453abe1.png
+-rw-r--r--   0 runner     (501) staff       (20)      524 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/62cd1c16ca3ef9e2b0d5696a6a49b6b5a6d19130.png
+-rw-r--r--   0 runner     (501) staff       (20)     1180 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/64824b782d63f742bca8b398e0f12b485771f257.png
+-rw-r--r--   0 runner     (501) staff       (20)     2236 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/6565000626ccf19f09a9258e78e141cb5ce46180.png
+-rw-r--r--   0 runner     (501) staff       (20)      769 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/66599856ec5735a610623bbe8242fc777d5f4100.png
+-rw-r--r--   0 runner     (501) staff       (20)     9750 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/6669c8a566ba908085156b5c4a539af53616f383.png
+-rw-r--r--   0 runner     (501) staff       (20)     2840 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/66e3f8da85954ae75f6016f5784d0ec468c2451c.png
+-rw-r--r--   0 runner     (501) staff       (20)     1941 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/68ea4366a8e9dac6f50d5b899ac5c385374d9673.png
+-rw-r--r--   0 runner     (501) staff       (20)     1415 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/694498e646bcebcf71487704e8bbabe9b2665425.png
+-rw-r--r--   0 runner     (501) staff       (20)      331 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/6981ec4aaaf7392f4bf828ef63be506799574e5e.png
+-rw-r--r--   0 runner     (501) staff       (20)      428 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/69ff02759612b6bf7f038a67b9fb4b557f2be247.png
+-rw-r--r--   0 runner     (501) staff       (20)     1610 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/6b3a21804f75fb45e7f9963fc6c0621fcf710cc7.png
+-rw-r--r--   0 runner     (501) staff       (20)     1457 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/6b3d942743e5a56e5030cfaab836f542fec9019c.png
+-rw-r--r--   0 runner     (501) staff       (20)      268 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/6c74a61cdf90a8a3b50f62a58910b84d0fe23678.png
+-rw-r--r--   0 runner     (501) staff       (20)     1738 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/6d9473d4787aece2804514f0796e6abeb2ce4dda.png
+-rw-r--r--   0 runner     (501) staff       (20)     2209 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/6dd83f47897e8af1a287a2cb577906b4c142c166.png
+-rw-r--r--   0 runner     (501) staff       (20)     1095 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/6efd575f4ef0199dda05d5b8f4a187112a62224b.png
+-rw-r--r--   0 runner     (501) staff       (20)      458 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/700c6a7cc89a7142ae312c5cb4f1f5b78da350dd.png
+-rw-r--r--   0 runner     (501) staff       (20)      290 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/7046228257af6ebbbde8ef7c8f944119e0a768d0.png
+-rw-r--r--   0 runner     (501) staff       (20)     1233 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/7056acd535c8f98331e8dd89e48cc0e927d42b12.png
+-rw-r--r--   0 runner     (501) staff       (20)     2610 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/7075b711b50c004803b51912b9dca99d35c65d35.png
+-rw-r--r--   0 runner     (501) staff       (20)     1211 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/70b640ff0659b7d33287ba001e5b26c6c93a96ba.png
+-rw-r--r--   0 runner     (501) staff       (20)      950 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/716fbcea39bcb0c1e19a3e26c60836bf5b111b91.png
+-rw-r--r--   0 runner     (501) staff       (20)     3140 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/727233e1f841277ba9bce9859cd9fbbe664f1667.png
+-rw-r--r--   0 runner     (501) staff       (20)      659 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/738092734154893db4338bbdedae2ef8c48eade3.png
+-rw-r--r--   0 runner     (501) staff       (20)      790 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/73e26546f3f051d6cc494fa37072d2eac9856ac1.png
+-rw-r--r--   0 runner     (501) staff       (20)     1828 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/7627c2662a2a563bf350d8d618dd7e6d40c35e2e.png
+-rw-r--r--   0 runner     (501) staff       (20)     1398 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/767b9280eb4c7a6ad46be67cb9782508dc6d1f22.png
+-rw-r--r--   0 runner     (501) staff       (20)     1278 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/783499b0add3c6f6f392a2b8d39402a6aa232020.png
+-rw-r--r--   0 runner     (501) staff       (20)     1119 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/78d5bb409e88f612d4afe2cca2f43186923387e6.png
+-rw-r--r--   0 runner     (501) staff       (20)      503 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/7911e1577218dbb02d5e98a311635e1b2347ff57.png
+-rw-r--r--   0 runner     (501) staff       (20)      420 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/79b3736681052735beb52087fe8a1b6c188338fb.png
+-rw-r--r--   0 runner     (501) staff       (20)     2286 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/7b25a0b8e9e5569bb0e977a9ea61b5daedb78e11.png
+-rw-r--r--   0 runner     (501) staff       (20)     1350 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/7b694e55a0813fe78e01121684b12a40fad86d86.png
+-rw-r--r--   0 runner     (501) staff       (20)      243 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/7daf0d4815e763eb90f0d5f1dc406f668c1e21db.png
+-rw-r--r--   0 runner     (501) staff       (20)      601 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/7dcb78b012b54b09f8760cec52ce8ae1389f0f11.png
+-rw-r--r--   0 runner     (501) staff       (20)      377 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/7e3e2e4f92024433a9ad4d75422c991d86d1ec57.png
+-rw-r--r--   0 runner     (501) staff       (20)      547 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/7e65c1c7c403764759e8813348c1b7e2d560f1fa.png
+-rw-r--r--   0 runner     (501) staff       (20)     1608 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/7eac6332e16c5424a4b290d2b9f9445c5214a1d1.png
+-rw-r--r--   0 runner     (501) staff       (20)     2840 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/7faf4e55287d19aeb554d113cd37857aeb2700b4.png
+-rw-r--r--   0 runner     (501) staff       (20)      252 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/801e28cfd4de6fd9c1e00f5e71e5ce7b29ad57f7.png
+-rw-r--r--   0 runner     (501) staff       (20)      273 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/808724526b9ab0aff711bd48855599a13f4f41c5.png
+-rw-r--r--   0 runner     (501) staff       (20)     7061 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/80e21626c375d52667de27ff84715270afb8ca70.png
+-rw-r--r--   0 runner     (501) staff       (20)      359 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/812c22f26f3cabffdd7214c59716aef9a9fedca2.png
+-rw-r--r--   0 runner     (501) staff       (20)     1366 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/81787f23988417db8fee122d8cc6141a1985c4b7.png
+-rw-r--r--   0 runner     (501) staff       (20)      516 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/817f53603d7e46d0c89d94f741f3ff760e7b4e64.png
+-rw-r--r--   0 runner     (501) staff       (20)      574 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/81868e29eaf33185bcc60e1d6ff7b0e307f2f892.png
+-rw-r--r--   0 runner     (501) staff       (20)     1025 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/82a55744f92063b61aaffddd2380a5cbf8a2b1c6.png
+-rw-r--r--   0 runner     (501) staff       (20)     1015 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/82d7fac4e1442a73c02aa8bd6fedab161db0f758.png
+-rw-r--r--   0 runner     (501) staff       (20)     1507 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/838e2b03a608af26db2efa9096182aa54d809a3d.png
+-rw-r--r--   0 runner     (501) staff       (20)     4580 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/84e264805077d2cf923fe75d31e2ed50021618da.png
+-rw-r--r--   0 runner     (501) staff       (20)      406 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/8621cd51e6bdca11da768ea315ebf1b8c319a975.png
+-rw-r--r--   0 runner     (501) staff       (20)     1163 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/86384124ce2e714ba7b80c295f44157d2da07413.png
+-rw-r--r--   0 runner     (501) staff       (20)     1078 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/8655418fcbc61747ed3bd70aa2d1ecc1db06a5c9.png
+-rw-r--r--   0 runner     (501) staff       (20)     1198 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/86a2d178f8f888b9c84ff42573fdaf015c8bfbb2.png
+-rw-r--r--   0 runner     (501) staff       (20)     1780 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/86cec286c2bbedaa7760445bc5a1a242cb84d2c2.png
+-rw-r--r--   0 runner     (501) staff       (20)     1447 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/870c60a6ab1247468ddfc5be8f68ffbe3479dfda.png
+-rw-r--r--   0 runner     (501) staff       (20)     1359 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/8871516499f79705d3818c3251aacd463f7c5146.png
+-rw-r--r--   0 runner     (501) staff       (20)      601 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/887be39f02687d3e3a1565193924f04d7ccbb743.png
+-rw-r--r--   0 runner     (501) staff       (20)      213 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/888f7c323ac0341871e867220ae2d76467d74d6e.png
+-rw-r--r--   0 runner     (501) staff       (20)     1721 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/895591ad55b7e2cec6ade3bbb0bb1a0b76fe0910.png
+-rw-r--r--   0 runner     (501) staff       (20)      255 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/89878909dbb648acdc4a44ded1bd982d7bddef5d.png
+-rw-r--r--   0 runner     (501) staff       (20)     1128 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/89d343471476626b56bc496f09d8fad108cb82a6.png
+-rw-r--r--   0 runner     (501) staff       (20)      313 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/8adc14b919839192224a68d21c0cae3a8b783c04.png
+-rw-r--r--   0 runner     (501) staff       (20)      436 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/8b5c5ce382e60258664c8b9eef58be7dad76daf3.png
+-rw-r--r--   0 runner     (501) staff       (20)      458 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/8ba9d3d0710a882764a58249d7a443b475a5b7d8.png
+-rw-r--r--   0 runner     (501) staff       (20)     2061 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/8c1dcc7704e1d156a5f896c8c0a3326c2722a3fa.png
+-rw-r--r--   0 runner     (501) staff       (20)     1021 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/8c51b26db8908731ed17a76ed86a9fe1c99aa02b.png
+-rw-r--r--   0 runner     (501) staff       (20)      498 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/8cb2d6eb037326c227a257ebad6eae725bd40148.png
+-rw-r--r--   0 runner     (501) staff       (20)      207 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/8d051150f8669295ecdbe92367941012175a824d.png
+-rw-r--r--   0 runner     (501) staff       (20)      329 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/8d1638c06d78232d12c1df1eac99cc20f863d50e.png
+-rw-r--r--   0 runner     (501) staff       (20)     1693 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/8d26408b917ad631b6ae90f7650b19b691fe2bb6.png
+-rw-r--r--   0 runner     (501) staff       (20)      929 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/8d53a80f87a15ba0d310801a0af822da73c3fcaf.png
+-rw-r--r--   0 runner     (501) staff       (20)      370 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/8d7aeb80b08f9d220de852b224d6a4693f6ddff9.png
+-rw-r--r--   0 runner     (501) staff       (20)     1361 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/8edd44acd8c3889706afee3c81bb907c3f415683.png
+-rw-r--r--   0 runner     (501) staff       (20)      244 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/8fb1fc12384d9c1b73b81b87315f7654511a2c0e.png
+-rw-r--r--   0 runner     (501) staff       (20)     1093 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/8fcff6b5a5c95afb39f5abaedac94b7086911410.png
+-rw-r--r--   0 runner     (501) staff       (20)     1275 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/908a083a0806ab219190adac99ec60da04c65f48.png
+-rw-r--r--   0 runner     (501) staff       (20)      253 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/9098c1c4618d7a0f321cee441aabee7f1b57a19b.png
+-rw-r--r--   0 runner     (501) staff       (20)      278 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/90cab5ae70bdb6e45756490226ba488f522c4c4e.png
+-rw-r--r--   0 runner     (501) staff       (20)      966 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/9173aacc17760942bd0ce61e5ad70788a84297d5.png
+-rw-r--r--   0 runner     (501) staff       (20)      414 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/936adf4ee141541b19f32162898758c0de10fa8d.png
+-rw-r--r--   0 runner     (501) staff       (20)     1327 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/957b97bc1591647fef3ac407dd3dd3e99c37fcd5.png
+-rw-r--r--   0 runner     (501) staff       (20)     3108 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/95a6e48cc402e2e0cee2fe87d159320f12dcadfc.png
+-rw-r--r--   0 runner     (501) staff       (20)     1186 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/95af1725828b1a188bbb0d933ffc78ef94788a48.png
+-rw-r--r--   0 runner     (501) staff       (20)     1102 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/95c7fad2a12f832a0675a00c80c4a8894297d2b8.png
+-rw-r--r--   0 runner     (501) staff       (20)      225 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/9630132210b904754c9ab272b61cb527d12263ca.png
+-rw-r--r--   0 runner     (501) staff       (20)     1154 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/973e7149b3e7c5fd4b7a92e36771cc6c2d6e620b.png
+-rw-r--r--   0 runner     (501) staff       (20)      233 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/97f89cf71150cd2020df53f6aabca4a64f63eb5f.png
+-rw-r--r--   0 runner     (501) staff       (20)      216 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/9b444cf6329a14140aee8ff5a06ff30772cc1c2f.png
+-rw-r--r--   0 runner     (501) staff       (20)      305 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/9de723874f4fca54fc9d4a4bf2f19c1b305b5a74.png
+-rw-r--r--   0 runner     (501) staff       (20)     2290 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/9f18ba54fa478c728e3a3536166f874c17aa7c04.png
+-rw-r--r--   0 runner     (501) staff       (20)      625 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/9f2f3a7e9359d5459533e3d50282ebae0ca36465.png
+-rw-r--r--   0 runner     (501) staff       (20)     3918 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/a121b0efd1dfa559be59e332b528608d97906c46.png
+-rw-r--r--   0 runner     (501) staff       (20)     1143 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/a133c9dd8091526f677cfcc502fbf773387d84bf.png
+-rw-r--r--   0 runner     (501) staff       (20)      379 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/a156920bb8825b9428df86c5bfe4e3ce5b51f0f8.png
+-rw-r--r--   0 runner     (501) staff       (20)      536 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/a38b44a27c1755531418f8bb853736ab038d7e9e.png
+-rw-r--r--   0 runner     (501) staff       (20)     1265 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/a444daac219907b51a5edd730d624c53328d693f.png
+-rw-r--r--   0 runner     (501) staff       (20)      258 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/a44c09dc69d687fd66b7a1a12197c0299aa5db1c.png
+-rw-r--r--   0 runner     (501) staff       (20)     1340 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/a4594eb66f65c9a3e69736f82fdb072d08b8ddcc.png
+-rw-r--r--   0 runner     (501) staff       (20)      413 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/a45d21a76729b863a1a60fe7ebb40a96a4ec69e5.png
+-rw-r--r--   0 runner     (501) staff       (20)     7041 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/a5d23ddad04b332c54e468fd62d6493589d61339.png
+-rw-r--r--   0 runner     (501) staff       (20)     1453 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/a6b6966ce67e827face4426ab49db20ec6a74a9e.png
+-rw-r--r--   0 runner     (501) staff       (20)     1612 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/a810215e77878dec996b87e0d3007d8a6ded6b3c.png
+-rw-r--r--   0 runner     (501) staff       (20)     1119 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/aa4d3057edd3aea1af61b5571a9e06258b978843.png
+-rw-r--r--   0 runner     (501) staff       (20)      486 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/aadbbd5ab63719ff3a6c78a984dd3702cf3174c7.png
+-rw-r--r--   0 runner     (501) staff       (20)      722 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/aaf1e4f8649093b3b1a2a201c97238b5d922ff96.png
+-rw-r--r--   0 runner     (501) staff       (20)     1465 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/aaf2039a0ca644d308dc578303aa096fd3775907.png
+-rw-r--r--   0 runner     (501) staff       (20)     5186 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/ab466a647f375d548d3b12c0c1ecb79704cef8d0.png
+-rw-r--r--   0 runner     (501) staff       (20)      313 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/ac0d697baa79826d5fa42ee6fb1be506ff2ac3f8.png
+-rw-r--r--   0 runner     (501) staff       (20)     1569 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/ac5ad3214d3caf44e5cc4e9514908ba2a7bb48dc.png
+-rw-r--r--   0 runner     (501) staff       (20)      414 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/acc14817c5834249a732434e2919dfd4f708fffc.png
+-rw-r--r--   0 runner     (501) staff       (20)     1358 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/ad2c8101af3f233ceefa1ec6865721f302b84cfd.png
+-rw-r--r--   0 runner     (501) staff       (20)     1215 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/ae4ca00a7da101aa137fa6b84b5467ce39b05349.png
+-rw-r--r--   0 runner     (501) staff       (20)     1601 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/ae6d9abfed9fac62837d0c88a97a8afc81b5e712.png
+-rw-r--r--   0 runner     (501) staff       (20)      479 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/b0f4d6da17f2d5db3b4617e0e0d14eaf0b976b4b.png
+-rw-r--r--   0 runner     (501) staff       (20)      418 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/b24f57eba06df79d80853a953d7805ab789ce829.png
+-rw-r--r--   0 runner     (501) staff       (20)     1708 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/b3b09dbd48529f16a62f1020d2172bb9551e3296.png
+-rw-r--r--   0 runner     (501) staff       (20)     2190 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/b6c16fed84a824ab88468f81a2b505ac69ad7505.png
+-rw-r--r--   0 runner     (501) staff       (20)      245 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/b7dd8acc0d0af36b58c42bc14eeeca05c6286fba.png
+-rw-r--r--   0 runner     (501) staff       (20)     1796 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/b7e4addc1a00973125d6c3b9ba5bd951e6486df5.png
+-rw-r--r--   0 runner     (501) staff       (20)     1406 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/b8c391eb9c602cc714b875704be76879e335e243.png
+-rw-r--r--   0 runner     (501) staff       (20)      633 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/b934c490f51b68bde94c85bb2c77c160a78731bc.png
+-rw-r--r--   0 runner     (501) staff       (20)      251 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/b988975be41fd13b4d091c10202ba19374643586.png
+-rw-r--r--   0 runner     (501) staff       (20)     4780 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/b9f9b8057126c1f181b745e36de7f60ecbe4e41d.png
+-rw-r--r--   0 runner     (501) staff       (20)      237 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/badad346f6fbe2e237af99bfbd9a93a4da53a3da.png
+-rw-r--r--   0 runner     (501) staff       (20)      886 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/bc28eed8cb92072618037ffe78d36cdf031045b0.png
+-rw-r--r--   0 runner     (501) staff       (20)      496 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/bc7ea4e9d78396e86d86c117f1b22f739b77aa10.png
+-rw-r--r--   0 runner     (501) staff       (20)      291 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/bca8217ac2efcad7312d6e496b4e4c82d8d179f6.png
+-rw-r--r--   0 runner     (501) staff       (20)     1574 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/bcfcc32ea50d37180cedf362db80a4901cbc05bd.png
+-rw-r--r--   0 runner     (501) staff       (20)      760 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/bd041563b2dc47337d212c089f31e14b6b95e033.png
+-rw-r--r--   0 runner     (501) staff       (20)      348 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/bd466edf158386c56b457fb6aeb74b97766afdc6.png
+-rw-r--r--   0 runner     (501) staff       (20)     1472 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/c0ff36623c1ad325126fbebd6724e58809c4fdd2.png
+-rw-r--r--   0 runner     (501) staff       (20)     1361 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/c20519763e75b58870bd25238b358057e2da4b86.png
+-rw-r--r--   0 runner     (501) staff       (20)      247 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/c2aa3dff9bffb099e9dff196fd36aed56ec16baf.png
+-rw-r--r--   0 runner     (501) staff       (20)     1284 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/c34401e75e80cc822827c5d5175de08a5bbffced.png
+-rw-r--r--   0 runner     (501) staff       (20)     2099 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/c72b037a60f8e81dc19add786e6d148794471f80.png
+-rw-r--r--   0 runner     (501) staff       (20)     1220 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/c7fb856181b7b0b9f3cf0ca66c11fe63ea2b7278.png
+-rw-r--r--   0 runner     (501) staff       (20)      292 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/c8ed607e197ca518179a4030e6aed34c1d339e7e.png
+-rw-r--r--   0 runner     (501) staff       (20)     1643 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/c94d8558b73b7597cc60b6a0ec7c758f40c88a8d.png
+-rw-r--r--   0 runner     (501) staff       (20)      737 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/c9a3af023076f58fe1ee0b35f88cad484ba194fa.png
+-rw-r--r--   0 runner     (501) staff       (20)      266 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/cb5de54f699cf4b3c7c1a3e87313d11d536c0d88.png
+-rw-r--r--   0 runner     (501) staff       (20)      340 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/cb92702d2163f15e2bf7e6a34b182302ae65f3b7.png
+-rw-r--r--   0 runner     (501) staff       (20)      279 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/cbb49321318d94ba656d1ce115187d55c90322b4.png
+-rw-r--r--   0 runner     (501) staff       (20)      231 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/cc87ee665749db882f94e0d3707eb23e39638650.png
+-rw-r--r--   0 runner     (501) staff       (20)     1834 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/ccfd8c814cc1234e5dc5fce8871570757d15515c.png
+-rw-r--r--   0 runner     (501) staff       (20)     1308 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/cd4c2f3674b5e0def3984a035f720209c8391074.png
+-rw-r--r--   0 runner     (501) staff       (20)      720 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/d2241f81f782d8593f9390f06af621fd3be21ab8.png
+-rw-r--r--   0 runner     (501) staff       (20)     1383 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/d246dde9fc63993c5b8df2eaccfa78ef89ad875d.png
+-rw-r--r--   0 runner     (501) staff       (20)     1041 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/d33cbbeb57b535cc4b2562e25475f7afc74ae85b.png
+-rw-r--r--   0 runner     (501) staff       (20)     1909 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/d3b5cc5b170fbda975293f38dea08b951f37142f.png
+-rw-r--r--   0 runner     (501) staff       (20)     1388 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/d452b345239711d0be1016ccde4ddfea5930b072.png
+-rw-r--r--   0 runner     (501) staff       (20)     2019 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/d504b5e2a3245798a6ad5678ea1951fc914e8fac.png
+-rw-r--r--   0 runner     (501) staff       (20)      572 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/d56da07a3d18c9fc980ecc0a9696603bd8d8dcd2.png
+-rw-r--r--   0 runner     (501) staff       (20)     1461 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/d5a4cdcdf8e599dc8e0d8a8c1301f02f9e8b4fb3.png
+-rw-r--r--   0 runner     (501) staff       (20)      937 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/d66b4ab25c0eef60d649ef489104789f43f45a0b.png
+-rw-r--r--   0 runner     (501) staff       (20)      430 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/d706fc3d557d35b283be36ac9e240324b68b34b9.png
+-rw-r--r--   0 runner     (501) staff       (20)     3059 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/d767754db8d214ccf0dcaf05b48317d378fbddb5.png
+-rw-r--r--   0 runner     (501) staff       (20)      273 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/d907a3c4e1257ec91ba2b8475cc048392650b648.png
+-rw-r--r--   0 runner     (501) staff       (20)     1380 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/d9aec1e99d1bcb92578727e61fb60d877c0964b7.png
+-rw-r--r--   0 runner     (501) staff       (20)      581 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/da8dad38c611fbd068672223f3f152e89ee7477e.png
+-rw-r--r--   0 runner     (501) staff       (20)      261 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/db5b465a483d35549d1b8a4577cc4163f9ece3aa.png
+-rw-r--r--   0 runner     (501) staff       (20)      302 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/db7426d70cdd8a4c33c3f1b8f7bdc9ba1b62c43a.png
+-rw-r--r--   0 runner     (501) staff       (20)     1353 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/dba423937c7e0c09118ccac03f01a4a3be60e2c3.png
+-rw-r--r--   0 runner     (501) staff       (20)     1898 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/dcab68360c480e6aaf0001fa1fb3f6451ba747f0.png
+-rw-r--r--   0 runner     (501) staff       (20)     2686 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/deb40d5eca48a271c62dc3937746712359cd3b05.png
+-rw-r--r--   0 runner     (501) staff       (20)      304 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/e00cdcd92f7a9d17060f49d50fad98569a249cd0.png
+-rw-r--r--   0 runner     (501) staff       (20)      277 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/e00d4db37b602d888e9a5f2bc30bb8ad68d14ce9.png
+-rw-r--r--   0 runner     (501) staff       (20)     1855 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/e2f6bbba20da0d51564b1855eb2da3072d841441.png
+-rw-r--r--   0 runner     (501) staff       (20)     1088 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/e35d7cbe33a34f4456eea34b9bd28642bfc52fa4.png
+-rw-r--r--   0 runner     (501) staff       (20)      858 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/e3a50552a1b736116240d899eea184ca3106ba0c.png
+-rw-r--r--   0 runner     (501) staff       (20)      948 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/e3f4c5bf9e0470ceafd97d572163a4dfefc39743.png
+-rw-r--r--   0 runner     (501) staff       (20)      414 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/e44d29f0cbcc5fa7a0f3f83d3bddc988f9b022ea.png
+-rw-r--r--   0 runner     (501) staff       (20)      248 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/e4762cec46619bf7781cae62216214f909395368.png
+-rw-r--r--   0 runner     (501) staff       (20)     1025 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/e50141a6a4a3490d1acc94e54f7de36ac5f7e8eb.png
+-rw-r--r--   0 runner     (501) staff       (20)      298 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/e55e27c7fb666f42abe96fbf168eddf1fa6c9eb2.png
+-rw-r--r--   0 runner     (501) staff       (20)      774 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/e61f71e6c396a94105e3437275d3449a61f9d802.png
+-rw-r--r--   0 runner     (501) staff       (20)      446 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/e71fcd98134a69534acee44a765e20abefe6e316.png
+-rw-r--r--   0 runner     (501) staff       (20)      237 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/e8dea8254118f111b5fb20895b03528c17566f06.png
+-rw-r--r--   0 runner     (501) staff       (20)     1097 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/e97fe83d126fdd192e9bc593cea89698fb36ffe5.png
+-rw-r--r--   0 runner     (501) staff       (20)      243 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/e9bc7da808d33a16a8347f27a519bd067186aa66.png
+-rw-r--r--   0 runner     (501) staff       (20)      465 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/eb21ee2e4d5e09a543f19ff14ce49d682ad586af.png
+-rw-r--r--   0 runner     (501) staff       (20)     1609 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/eb873a106ad1868e288ae26783dd930d360fdef5.png
+-rw-r--r--   0 runner     (501) staff       (20)      164 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/ecdff306b10b7e2991a2c20df2fccba0f947155b.png
+-rw-r--r--   0 runner     (501) staff       (20)     1665 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/ed29c4b1667b0282bad6523664351811e0f23dab.png
+-rw-r--r--   0 runner     (501) staff       (20)      254 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/ed38fa24f1c94891bd312012aab3f6673be3eb83.png
+-rw-r--r--   0 runner     (501) staff       (20)      252 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/ed7fb0260e58d3ca5851e823ff991dae4cde5671.png
+-rw-r--r--   0 runner     (501) staff       (20)     1235 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/ee3c949541ac51ceadec0a62713cdd8a42a2e4ab.png
+-rw-r--r--   0 runner     (501) staff       (20)      438 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/ef10ae5e9279f912e2a62fa15fc274fee32bb7d1.png
+-rw-r--r--   0 runner     (501) staff       (20)     1340 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/efe5c37bc03bf3d5826fd02dc5b43a0a51e7c271.png
+-rw-r--r--   0 runner     (501) staff       (20)      414 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/f2cb671262e4538a530f4241ee603253c3e01118.png
+-rw-r--r--   0 runner     (501) staff       (20)      375 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/f3a047615f8cef5f6ce18b309a433eb73ef8e13b.png
+-rw-r--r--   0 runner     (501) staff       (20)    11364 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/f59b4bcd76f97da1f13ba87bc76bf52b442b4381.png
+-rw-r--r--   0 runner     (501) staff       (20)     3798 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/f86c7a0b45da8cc7f4a00c20bf654b3df94ff06a.png
+-rw-r--r--   0 runner     (501) staff       (20)      747 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/facdb23d2bcdc9cf5d90ab695c86965ac188e3e5.png
+-rw-r--r--   0 runner     (501) staff       (20)     4014 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/fb07faac9fe824b206392c19b7a1a2c6dd70e1ee.png
+-rw-r--r--   0 runner     (501) staff       (20)     1457 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/fc16f4da2e0dd685363c204baf675d6244c52fbb.png
+-rw-r--r--   0 runner     (501) staff       (20)      248 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/fc18e7de656eaf3eacbb104912233162cf9042e4.png
+-rw-r--r--   0 runner     (501) staff       (20)     2030 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/fcc17fd59806862a629796f0d7f0e8f43778e7bd.png
+-rw-r--r--   0 runner     (501) staff       (20)     2610 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/math/fe748f1ddebc2719b738533481dc2070aa3f8b04.png
+-rw-r--r--   0 runner     (501) staff       (20)    24912 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/normappr.png
+-rw-r--r--   0 runner     (501) staff       (20)    46408 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/portfolio1.png
+-rw-r--r--   0 runner     (501) staff       (20)    28141 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_images/portfolio2.png
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-08 16:49:13.467159 kvxopt-1.3.2.1/doc/html/_static/
+-rw-r--r--   0 runner     (501) staff       (20)     4418 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0 runner     (501) staff       (20)    15280 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_static/basic.css
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-08 16:49:13.467501 kvxopt-1.3.2.1/doc/html/_static/css/
+-rw-r--r--   0 runner     (501) staff       (20)     3275 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_static/css/badge_only.css
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-08 16:49:13.473930 kvxopt-1.3.2.1/doc/html/_static/css/fonts/
+-rw-r--r--   0 runner     (501) staff       (20)    87624 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0 runner     (501) staff       (20)    67312 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0 runner     (501) staff       (20)    86288 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0 runner     (501) staff       (20)    66444 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0 runner     (501) staff       (20)   165742 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 runner     (501) staff       (20)   444379 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 runner     (501) staff       (20)   165548 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 runner     (501) staff       (20)    98024 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 runner     (501) staff       (20)    77160 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 runner     (501) staff       (20)   323344 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0 runner     (501) staff       (20)   193308 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0 runner     (501) staff       (20)   309728 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0 runner     (501) staff       (20)   184912 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0 runner     (501) staff       (20)   328412 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0 runner     (501) staff       (20)   195704 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0 runner     (501) staff       (20)   309192 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0 runner     (501) staff       (20)   182708 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0 runner     (501) staff       (20)   129674 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_static/css/theme.css
+-rw-r--r--   0 runner     (501) staff       (20)    11060 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_static/cvxopt.css
+-rw-r--r--   0 runner     (501) staff       (20)     8171 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_static/doctools.js
+-rw-r--r--   0 runner     (501) staff       (20)      423 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_static/documentation_options.js
+-rw-r--r--   0 runner     (501) staff       (20)      286 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_static/file.png
+-rw-r--r--   0 runner     (501) staff       (20)   288580 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_static/jquery-3.6.0.js
+-rw-r--r--   0 runner     (501) staff       (20)    89501 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_static/jquery.js
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-08 16:49:13.476697 kvxopt-1.3.2.1/doc/html/_static/js/
+-rw-r--r--   0 runner     (501) staff       (20)      934 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_static/js/badge_only.js
+-rw-r--r--   0 runner     (501) staff       (20)     4370 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0 runner     (501) staff       (20)     2734 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_static/js/html5shiv.min.js
+-rw-r--r--   0 runner     (501) staff       (20)     5023 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_static/js/theme.js
+-rw-r--r--   0 runner     (501) staff       (20)     4758 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_static/language_data.js
+-rw-r--r--   0 runner     (501) staff       (20)       90 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_static/minus.png
+-rw-r--r--   0 runner     (501) staff       (20)       90 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_static/plus.png
+-rw-r--r--   0 runner     (501) staff       (20)     4919 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_static/pygments.css
+-rw-r--r--   0 runner     (501) staff       (20)    17088 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_static/searchtools.js
+-rw-r--r--   0 runner     (501) staff       (20)    68420 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_static/underscore-1.13.1.js
+-rw-r--r--   0 runner     (501) staff       (20)    19530 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/_static/underscore.js
+-rw-r--r--   0 runner     (501) staff       (20)   104767 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/blas.html
+-rw-r--r--   0 runner     (501) staff       (20)    38735 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/c-api.html
+-rw-r--r--   0 runner     (501) staff       (20)   233726 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/coneprog.html
+-rw-r--r--   0 runner     (501) staff       (20)     6580 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/copyright.html
+-rw-r--r--   0 runner     (501) staff       (20)    23074 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/fftw.html
+-rw-r--r--   0 runner     (501) staff       (20)    13377 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/index.html
+-rw-r--r--   0 runner     (501) staff       (20)    11425 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/intro.html
+-rw-r--r--   0 runner     (501) staff       (20)   236474 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/lapack.html
+-rw-r--r--   0 runner     (501) staff       (20)   155220 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/matrices.html
+-rw-r--r--   0 runner     (501) staff       (20)    90620 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/modeling.html
+-rw-r--r--   0 runner     (501) staff       (20)     1942 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/objects.inv
+-rw-r--r--   0 runner     (501) staff       (20)    18961 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/printing.html
+-rw-r--r--   0 runner     (501) staff       (20)     5157 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/search.html
+-rw-r--r--   0 runner     (501) staff       (20)    40104 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/searchindex.js
+-rw-r--r--   0 runner     (501) staff       (20)   154192 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/solvers.html
+-rw-r--r--   0 runner     (501) staff       (20)    81016 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/html/spsolvers.html
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-08 16:49:13.485418 kvxopt-1.3.2.1/doc/source/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-08 16:49:13.486512 kvxopt-1.3.2.1/doc/source/.static/
+-rw-r--r--   0 runner     (501) staff       (20)    11060 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/source/.static/cvxopt.css
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-08 16:49:13.487209 kvxopt-1.3.2.1/doc/source/.templates/
+-rw-r--r--   0 runner     (501) staff       (20)      436 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/source/.templates/layout.html
+-rw-r--r--   0 runner     (501) staff       (20)    34002 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/source/blas.rst
+-rw-r--r--   0 runner     (501) staff       (20)     7802 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/source/c-api.rst
+-rw-r--r--   0 runner     (501) staff       (20)    77236 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/source/coneprog.rst
+-rw-r--r--   0 runner     (501) staff       (20)     6008 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/source/conf.py
+-rw-r--r--   0 runner     (501) staff       (20)      848 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/source/copyright.rst
+-rw-r--r--   0 runner     (501) staff       (20)     7172 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/source/fftw.rst
+-rw-r--r--   0 runner     (501) staff       (20)     9062 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/source/floorplan.png
+-rw-r--r--   0 runner     (501) staff       (20)      448 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/source/index.rst
+-rw-r--r--   0 runner     (501) staff       (20)     3116 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/source/intro.rst
+-rw-r--r--   0 runner     (501) staff       (20)    60668 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/source/lapack.rst
+-rw-r--r--   0 runner     (501) staff       (20)    44308 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/source/matrices.rst
+-rw-r--r--   0 runner     (501) staff       (20)    25482 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/source/modeling.rst
+-rw-r--r--   0 runner     (501) staff       (20)    24912 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/source/normappr.png
+-rw-r--r--   0 runner     (501) staff       (20)    46408 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/source/portfolio1.png
+-rw-r--r--   0 runner     (501) staff       (20)    28141 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/source/portfolio2.png
+-rw-r--r--   0 runner     (501) staff       (20)     4952 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/source/printing.rst
+-rw-r--r--   0 runner     (501) staff       (20)    47718 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/source/solvers.rst
+-rw-r--r--   0 runner     (501) staff       (20)    32751 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/doc/source/spsolvers.rst
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-08 16:49:13.384060 kvxopt-1.3.2.1/examples/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-08 16:49:13.487648 kvxopt-1.3.2.1/examples/book/
+-rw-r--r--   0 runner     (501) staff       (20)      271 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/book/README
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-08 16:49:13.489505 kvxopt-1.3.2.1/examples/book/chap4/
+-rwxr-xr-x   0 runner     (501) staff       (20)     1957 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/book/chap4/portfolio.py
+-rw-r--r--   0 runner     (501) staff       (20)    26660 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/book/chap4/rls.bin
+-rwxr-xr-x   0 runner     (501) staff       (20)     2317 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/book/chap4/rls.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-08 16:49:13.496872 kvxopt-1.3.2.1/examples/book/chap6/
+-rwxr-xr-x   0 runner     (501) staff       (20)     7364 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/book/chap6/basispursuit.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     4365 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/book/chap6/consumerpref.py
+-rw-r--r--   0 runner     (501) staff       (20)     2190 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/book/chap6/cvxfit.bin
+-rwxr-xr-x   0 runner     (501) staff       (20)     1524 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/book/chap6/cvxfit.py
+-rw-r--r--   0 runner     (501) staff       (20)     1965 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/book/chap6/huber.bin
+-rwxr-xr-x   0 runner     (501) staff       (20)     1956 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/book/chap6/huber.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2193 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/book/chap6/inputdesign.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2497 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/book/chap6/penalties.py
+-rw-r--r--   0 runner     (501) staff       (20)     1996 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/book/chap6/polapprox.bin
+-rwxr-xr-x   0 runner     (501) staff       (20)     4407 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/book/chap6/polapprox.py
+-rw-r--r--   0 runner     (501) staff       (20)     5006 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/book/chap6/regsel.bin
+-rwxr-xr-x   0 runner     (501) staff       (20)     3518 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/book/chap6/regsel.py
+-rw-r--r--   0 runner     (501) staff       (20)    83504 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/book/chap6/robls.bin
+-rwxr-xr-x   0 runner     (501) staff       (20)     4398 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/book/chap6/robls.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2807 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/book/chap6/smoothrec.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     9117 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/book/chap6/tv.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-08 16:49:13.498371 kvxopt-1.3.2.1/examples/book/chap7/
+-rwxr-xr-x   0 runner     (501) staff       (20)     3253 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/book/chap7/chernoff.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     5122 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/book/chap7/expdesign.py
+-rw-r--r--   0 runner     (501) staff       (20)     2842 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/book/chap7/logreg.bin
+-rwxr-xr-x   0 runner     (501) staff       (20)     1241 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/book/chap7/logreg.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2718 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/book/chap7/maxent.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     6681 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/book/chap7/probbounds.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-08 16:49:13.501994 kvxopt-1.3.2.1/examples/book/chap8/
+-rwxr-xr-x   0 runner     (501) staff       (20)     6223 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/book/chap8/centers.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     7142 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/book/chap8/ellipsoids.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     6268 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/book/chap8/floorplan.py
+-rw-r--r--   0 runner     (501) staff       (20)     4657 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/book/chap8/linsep.bin
+-rwxr-xr-x   0 runner     (501) staff       (20)     3797 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/book/chap8/linsep.py
+-rw-r--r--   0 runner     (501) staff       (20)      783 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/book/chap8/placement.bin
+-rwxr-xr-x   0 runner     (501) staff       (20)     5160 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/book/chap8/placement.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-08 16:49:13.502373 kvxopt-1.3.2.1/examples/doc/
+-rw-r--r--   0 runner     (501) staff       (20)      267 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/doc/README
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-08 16:49:13.503942 kvxopt-1.3.2.1/examples/doc/chap10/
+-rwxr-xr-x   0 runner     (501) staff       (20)      507 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/doc/chap10/l1svc.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     1169 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/doc/chap10/lp.py
+-rwxr-xr-x   0 runner     (501) staff       (20)      694 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/doc/chap10/normappr.py
+-rwxr-xr-x   0 runner     (501) staff       (20)      515 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/doc/chap10/roblp.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-08 16:49:13.504262 kvxopt-1.3.2.1/examples/doc/chap4/
+-rwxr-xr-x   0 runner     (501) staff       (20)     1865 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/doc/chap4/acent.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-08 16:49:13.504610 kvxopt-1.3.2.1/examples/doc/chap7/
+-rw-r--r--   0 runner     (501) staff       (20)    62593 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/doc/chap7/covsel.bin
+-rwxr-xr-x   0 runner     (501) staff       (20)     2486 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/doc/chap7/covsel.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-08 16:49:13.510446 kvxopt-1.3.2.1/examples/doc/chap8/
+-rwxr-xr-x   0 runner     (501) staff       (20)      851 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/doc/chap8/conelp.py
+-rwxr-xr-x   0 runner     (501) staff       (20)      634 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/doc/chap8/coneqp.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     3999 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/doc/chap8/l1.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     4373 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/doc/chap8/l1regls.py
+-rwxr-xr-x   0 runner     (501) staff       (20)      271 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/doc/chap8/lp.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     3335 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/doc/chap8/mcsdp.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     1941 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/doc/chap8/portfolio.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     4254 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/doc/chap8/qcl1.py
+-rwxr-xr-x   0 runner     (501) staff       (20)      741 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/doc/chap8/sdp.py
+-rwxr-xr-x   0 runner     (501) staff       (20)      527 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/doc/chap8/socp.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-08 16:49:13.512999 kvxopt-1.3.2.1/examples/doc/chap9/
+-rwxr-xr-x   0 runner     (501) staff       (20)     1000 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/doc/chap9/acent.py
+-rwxr-xr-x   0 runner     (501) staff       (20)      970 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/doc/chap9/acent2.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     6264 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/doc/chap9/floorplan.py
+-rwxr-xr-x   0 runner     (501) staff       (20)      589 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/doc/chap9/gp.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2163 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/doc/chap9/l2ac.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     1335 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/doc/chap9/robls.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-08 16:49:13.513833 kvxopt-1.3.2.1/examples/filterdemo/
+-rw-r--r--   0 runner     (501) staff       (20)      457 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/filterdemo/README
+-rwxr-xr-x   0 runner     (501) staff       (20)     3679 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/filterdemo/filterdemo_cli
+-rwxr-xr-x   0 runner     (501) staff       (20)     7387 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/examples/filterdemo/filterdemo_gui
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-08 16:49:13.514763 kvxopt-1.3.2.1/kvxopt.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     1592 2024-05-08 16:49:13.000000 kvxopt-1.3.2.1/kvxopt.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)    28686 2024-05-08 16:49:13.000000 kvxopt-1.3.2.1/kvxopt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-05-08 16:49:13.000000 kvxopt-1.3.2.1/kvxopt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-05-08 16:49:13.000000 kvxopt-1.3.2.1/kvxopt.egg-info/not-zip-safe
+-rw-r--r--   0 runner     (501) staff       (20)       61 2024-05-08 16:49:13.000000 kvxopt-1.3.2.1/kvxopt.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)      204 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/pyproject.toml
+-rw-r--r--   0 runner     (501) staff       (20)      148 2024-05-08 16:49:13.533722 kvxopt-1.3.2.1/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)    18885 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-08 16:49:13.384504 kvxopt-1.3.2.1/src/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-08 16:49:13.518766 kvxopt-1.3.2.1/src/C/
+-rw-r--r--   0 runner     (501) staff       (20)     7703 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/src/C/amd.c
+-rw-r--r--   0 runner     (501) staff       (20)    68958 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/src/C/base.c
+-rw-r--r--   0 runner     (501) staff       (20)   139358 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/src/C/blas.c
+-rw-r--r--   0 runner     (501) staff       (20)     3543 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/src/C/blas_redefines.h
+-rw-r--r--   0 runner     (501) staff       (20)    36999 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/src/C/cholmod.c
+-rw-r--r--   0 runner     (501) staff       (20)    75347 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/src/C/dense.c
+-rw-r--r--   0 runner     (501) staff       (20)    19626 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/src/C/dsdp.c
+-rw-r--r--   0 runner     (501) staff       (20)    34318 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/src/C/fftw.c
+-rw-r--r--   0 runner     (501) staff       (20)    42231 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/src/C/glpk.c
+-rw-r--r--   0 runner     (501) staff       (20)     6978 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/src/C/gsl.c
+-rw-r--r--   0 runner     (501) staff       (20)    23071 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/src/C/gurobi.c
+-rw-r--r--   0 runner     (501) staff       (20)    28572 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/src/C/klu.c
+-rw-r--r--   0 runner     (501) staff       (20)     5442 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/src/C/kvxopt.h
+-rw-r--r--   0 runner     (501) staff       (20)   281701 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/src/C/lapack.c
+-rw-r--r--   0 runner     (501) staff       (20)     3535 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/src/C/misc.h
+-rw-r--r--   0 runner     (501) staff       (20)    38101 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/src/C/misc_solvers.c
+-rw-r--r--   0 runner     (501) staff       (20)    19197 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/src/C/osqp.c
+-rw-r--r--   0 runner     (501) staff       (20)   141567 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/src/C/sparse.c
+-rw-r--r--   0 runner     (501) staff       (20)    25015 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/src/C/umfpack.c
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-08 16:49:13.521407 kvxopt-1.3.2.1/src/python/
+-rw-r--r--   0 runner     (501) staff       (20)    10614 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/src/python/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      416 2024-05-08 16:49:13.000000 kvxopt-1.3.2.1/src/python/_version.py
+-rw-r--r--   0 runner     (501) staff       (20)   172008 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/src/python/coneprog.py
+-rw-r--r--   0 runner     (501) staff       (20)    83899 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/src/python/cvxprog.py
+-rw-r--r--   0 runner     (501) staff       (20)      885 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/src/python/info.py
+-rw-r--r--   0 runner     (501) staff       (20)    54949 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/src/python/misc.py
+-rw-r--r--   0 runner     (501) staff       (20)   100979 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/src/python/modeling.py
+-rw-r--r--   0 runner     (501) staff       (20)    37174 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/src/python/msk.py
+-rw-r--r--   0 runner     (501) staff       (20)     5483 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/src/python/printing.py
+-rw-r--r--   0 runner     (501) staff       (20)     1562 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/src/python/solvers.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-08 16:49:13.532262 kvxopt-1.3.2.1/tests/
+-rw-r--r--   0 runner     (501) staff       (20)   778267 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/tests/ACTIVSg2000.mtx
+-rw-r--r--   0 runner     (501) staff       (20)  1025924 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/tests/bcsstk13.mtx
+-rw-r--r--   0 runner     (501) staff       (20)  2035740 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/tests/bcsstk24.mtx
+-rw-r--r--   0 runner     (501) staff       (20)    48147 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/tests/boeing2.mps
+-rw-r--r--   0 runner     (501) staff       (20)    55059 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/tests/bp_800.mtx
+-rw-r--r--   0 runner     (501) staff       (20)     5487 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/tests/test_basic.py
+-rw-r--r--   0 runner     (501) staff       (20)      772 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/tests/test_blas.py
+-rw-r--r--   0 runner     (501) staff       (20)    11685 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/tests/test_custom_kkt.py
+-rw-r--r--   0 runner     (501) staff       (20)     2206 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/tests/test_dsdp.py
+-rw-r--r--   0 runner     (501) staff       (20)     2685 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/tests/test_examples.py
+-rw-r--r--   0 runner     (501) staff       (20)     3160 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/tests/test_glpk.py
+-rw-r--r--   0 runner     (501) staff       (20)      698 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/tests/test_gsl.py
+-rw-r--r--   0 runner     (501) staff       (20)     4312 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/tests/test_gurobi.py
+-rw-r--r--   0 runner     (501) staff       (20)     1791 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/tests/test_modeling.py
+-rw-r--r--   0 runner     (501) staff       (20)     2516 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/tests/test_mosek.py
+-rw-r--r--   0 runner     (501) staff       (20)     4706 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/tests/test_osqp.py
+-rw-r--r--   0 runner     (501) staff       (20)     8799 2024-05-08 16:47:53.000000 kvxopt-1.3.2.1/tests/test_sparse_solvers.py
```

### Comparing `kvxopt-1.3.2.0/.github/workflows/linux_build.yml` & `kvxopt-1.3.2.1/.github/workflows/linux_build.yml`

 * *Files 9% similar despite different names*

```diff
@@ -10,22 +10,22 @@
     runs-on: ubuntu-latest
     env:
       KVXOPT_BUILD_GSL: 1
       KVXOPT_BUILD_FFTW: 1
       KVXOPT_BUILD_GLPK: 1
       KVXOPT_BUILD_DSDP: 1
       KVXOPT_BUILD_OSQP: 1
-      SUITESPARSE_VERSION: 7.2.1
-      SUITESPARSE_SHA256: 304e959a163ff74f8f4055dade3e0b5498d9aa3b1c483633bb400620f521509f
+      SUITESPARSE_VERSION: 7.7.0
+      SUITESPARSE_SHA256: 529b067f5d80981f45ddf6766627b8fc5af619822f068f342aab776e683df4f3
       OSQP_VERSION:  0.6.3
 
     strategy:
       fail-fast: false
       matrix:
-        python-version: ['3.7', '3.8', '3.9', '3.10', '3.11']
+        python-version: ['3.8', '3.9', '3.10', '3.11']
         suite-sparse: [lib_suitesparse]
 
     steps:
       - uses: actions/checkout@v3
       - name: Setup Python ${{ matrix.python-version }}
         uses: actions/setup-python@v3
         with:
@@ -77,16 +77,17 @@
       - name: Test
         run: |
           echo ${KVXOPT_SUITESPARSE_SRC_DIR}
           python -c 'from kvxopt import blas,dsdp,lapack,glpk,osqp,fftw,gsl,cholmod,umfpack,klu'
           pytest --cov=kvxopt --cov-report=xml tests/
 
       - name: Upload coverage to Codecov
-        uses: codecov/codecov-action@v2
+        uses: codecov/codecov-action@v4
         with:
           directory: ./coverage/reports/
           env_vars: OS,PYTHON
           files: ./coverage.xml
           fail_ci_if_error: true
           flags: unittests
-          name: codecov-kvxopt
+          token: ${{ secrets.CODECOV_TOKEN }}
+          slug: sanurielf/kvxopt
           verbose: true
```

### Comparing `kvxopt-1.3.2.0/.github/workflows/macos_build.yml` & `kvxopt-1.3.2.1/.github/workflows/macos_build.yml`

 * *Files 4% similar despite different names*

```diff
@@ -10,21 +10,21 @@
     runs-on: macos-latest
     env:
       KVXOPT_BUILD_GSL: 1
       KVXOPT_BUILD_FFTW: 1
       KVXOPT_BUILD_GLPK: 1
       KVXOPT_BUILD_OSQP: 1
       KVXOPT_BUILD_DSDP: 0
-      SUITESPARSE_VERSION: 7.2.1
-      SUITESPARSE_SHA256: 304e959a163ff74f8f4055dade3e0b5498d9aa3b1c483633bb400620f521509f
+      SUITESPARSE_VERSION: 7.7.0
+      SUITESPARSE_SHA256: 529b067f5d80981f45ddf6766627b8fc5af619822f068f342aab776e683df4f3
 
     strategy:
       fail-fast: false
       matrix:
-        python-version: ['3.7', '3.8', '3.9', '3.10', '3.11']
+        python-version: ['3.8', '3.9', '3.10', '3.11']
         suite-sparse: [lib_suitesparse]
 
     steps:
       - uses: actions/checkout@v3
       - name: Setup Python ${{ matrix.python-version }}
         uses: actions/setup-python@v3
         with:
@@ -51,15 +51,15 @@
             echo "KVXOPT_FFTW_LIB_DIR=$(brew --prefix)/lib" >> $GITHUB_ENV
 
 
       - name: Config suite-sparse library
         run: |
             brew install suite-sparse
             brew list suite-sparse
-            echo "KVXOPT_SUITESPARSE_INC_DIR=$(brew --prefix)/include" >> $GITHUB_ENV
+            echo "KVXOPT_SUITESPARSE_INC_DIR=$(brew --prefix)/include/suitesparse" >> $GITHUB_ENV
             echo "KVXOPT_SUITESPARSE_LIB_DIR=$(brew --prefix)/lib" >> $GITHUB_ENV
 
         if: ${{ matrix.suite-sparse == 'lib_suitesparse' }}
 
       - name: Config suite-sparse source
         run: |
             wget https://github.com/DrTimothyAldenDavis/SuiteSparse/archive/v${SUITESPARSE_VERSION}.tar.gz
```

### Comparing `kvxopt-1.3.2.0/.github/workflows/windows_build.yml` & `kvxopt-1.3.2.1/.github/workflows/windows_build.yml`

 * *Files 2% similar despite different names*

```diff
@@ -141,16 +141,16 @@
     env:
       KVXOPT_BUILD_GSL: 1
       KVXOPT_BUILD_FFTW: 1
       KVXOPT_BUILD_GLPK: 1
       KVXOPT_BUILD_DSDP: 0
       KVXOPT_MSVC: 1
       KVXOPT_BUILD_OSQP: 1
-      SUITESPARSE_VERSION: 7.2.1
-      SUITESPARSE_SHA256: 304e959a163ff74f8f4055dade3e0b5498d9aa3b1c483633bb400620f521509f
+      SUITESPARSE_VERSION: 7.7.0
+      SUITESPARSE_SHA256: 529b067f5d80981f45ddf6766627b8fc5af619822f068f342aab776e683df4f3
       OPENBLAS_VERSION: 0.3.23
       FFTW_VERSION: 3.3.5
 
     strategy:
       matrix:
         python-version: ['3.8', '3.9', '3.10', '3.11']
         suite-sparse: [src_suitesparse]
```

### Comparing `kvxopt-1.3.2.0/INSTALL` & `kvxopt-1.3.2.1/INSTALL`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/Jenkinsfile` & `kvxopt-1.3.2.1/Jenkinsfile`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/LICENSE` & `kvxopt-1.3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/PKG-INFO` & `kvxopt-1.3.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: kvxopt
-Version: 1.3.2.0
+Version: 1.3.2.1
 Summary: Convex optimization package and Suite Sparse interface
 Home-page: UNKNOWN
 Author: M. Andersen, J. Dahl, L. Vandenberghe, and U. Sandoval
 Author-email: martin.skovgaard.andersen@gmail.com, dahl.joachim@gmail.com, vandenbe@ee.ucla.edu, sanurielf@gmail.com
 License: GNU GPL version 3
 Project-URL: Source, https://github.com/sanurielf/kvxopt
 Description:
```

### Comparing `kvxopt-1.3.2.0/README.md` & `kvxopt-1.3.2.1/README.md`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/Makefile` & `kvxopt-1.3.2.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/floorplan.png` & `kvxopt-1.3.2.1/doc/html/_images/floorplan.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/00e8f621cc91c8f430e504b66fb085743c4814cb.png` & `kvxopt-1.3.2.1/doc/html/_images/math/00e8f621cc91c8f430e504b66fb085743c4814cb.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/01824df8f8806530b722445b6f9cde3a8e732f07.png` & `kvxopt-1.3.2.1/doc/html/_images/math/01824df8f8806530b722445b6f9cde3a8e732f07.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/03cfea18434ec87caa164206e463d7a230e1cb5c.png` & `kvxopt-1.3.2.1/doc/html/_images/math/03cfea18434ec87caa164206e463d7a230e1cb5c.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/03da04b738c1b20d64d873e8f3c18eccc4c7bc84.png` & `kvxopt-1.3.2.1/doc/html/_images/math/03da04b738c1b20d64d873e8f3c18eccc4c7bc84.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/04163b47432b93c2e42e10bab40066847581fc79.png` & `kvxopt-1.3.2.1/doc/html/_images/math/04163b47432b93c2e42e10bab40066847581fc79.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/04b02267d8a264913c39b04bf73ab88181b03cfc.png` & `kvxopt-1.3.2.1/doc/html/_images/math/04b02267d8a264913c39b04bf73ab88181b03cfc.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/056427854bd8d5a1fa428fff460d45b749aebc2a.png` & `kvxopt-1.3.2.1/doc/html/_images/math/056427854bd8d5a1fa428fff460d45b749aebc2a.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/05c3b434aba8ec5e2ac1cdfcc3e3bb7ca8a69775.png` & `kvxopt-1.3.2.1/doc/html/_images/math/05c3b434aba8ec5e2ac1cdfcc3e3bb7ca8a69775.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/0667e780fc9b2d0fad01d14184553aba1cd6b81b.png` & `kvxopt-1.3.2.1/doc/html/_images/math/0667e780fc9b2d0fad01d14184553aba1cd6b81b.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/072b7c28c9bc48c8509301fcff6dfb5095db4a07.png` & `kvxopt-1.3.2.1/doc/html/_images/math/072b7c28c9bc48c8509301fcff6dfb5095db4a07.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/073b4fb9749f6ab5523c701bbe38a97c5fa94288.png` & `kvxopt-1.3.2.1/doc/html/_images/math/073b4fb9749f6ab5523c701bbe38a97c5fa94288.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/0790b49262067229d1ce8165c4a66b4afa62cda9.png` & `kvxopt-1.3.2.1/doc/html/_images/math/0790b49262067229d1ce8165c4a66b4afa62cda9.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/081eab67b8ad47c824c773f9ce571fe5883895bf.png` & `kvxopt-1.3.2.1/doc/html/_images/math/081eab67b8ad47c824c773f9ce571fe5883895bf.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/08390710b56f1bdd0cf7346dd20ee9b3a5984ea1.png` & `kvxopt-1.3.2.1/doc/html/_images/math/08390710b56f1bdd0cf7346dd20ee9b3a5984ea1.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/0b6da08d6fc1f85c1382af2c64a51fa0129e47fd.png` & `kvxopt-1.3.2.1/doc/html/_images/math/0b6da08d6fc1f85c1382af2c64a51fa0129e47fd.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/0b75ca09d0ef9d47484865bd353fc1e234d0ffae.png` & `kvxopt-1.3.2.1/doc/html/_images/math/0b75ca09d0ef9d47484865bd353fc1e234d0ffae.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/0bf595687ae571b0147a101f606500879246b152.png` & `kvxopt-1.3.2.1/doc/html/_images/math/0bf595687ae571b0147a101f606500879246b152.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/0e7509809ae807b340e6d7cd64cc157ce0c8a4ff.png` & `kvxopt-1.3.2.1/doc/html/_images/math/0e7509809ae807b340e6d7cd64cc157ce0c8a4ff.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/0e95b3c9bb477c1d27aa253d83fe2d3e1922b3ef.png` & `kvxopt-1.3.2.1/doc/html/_images/math/0e95b3c9bb477c1d27aa253d83fe2d3e1922b3ef.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/0f2f6181474c4d231456601880211909048d0548.png` & `kvxopt-1.3.2.1/doc/html/_images/math/0f2f6181474c4d231456601880211909048d0548.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/0f36e4d687eeb224ee6593ac11df99a1d4451ba9.png` & `kvxopt-1.3.2.1/doc/html/_images/math/0f36e4d687eeb224ee6593ac11df99a1d4451ba9.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/0fc13f815b495c77d502992ae392d16844c0950b.png` & `kvxopt-1.3.2.1/doc/html/_images/math/0fc13f815b495c77d502992ae392d16844c0950b.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/10d754c37b304c217ee6f80c9a3c4c7bcbbcba9d.png` & `kvxopt-1.3.2.1/doc/html/_images/math/10d754c37b304c217ee6f80c9a3c4c7bcbbcba9d.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/11969d386f3f62d281586721cb47b9bc640ea082.png` & `kvxopt-1.3.2.1/doc/html/_images/math/11969d386f3f62d281586721cb47b9bc640ea082.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/12354e7e046bba1f8384eebcc70a2d9a09930e8e.png` & `kvxopt-1.3.2.1/doc/html/_images/math/12354e7e046bba1f8384eebcc70a2d9a09930e8e.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/124ef7067b147c5c7f031fc0fc06a822029456c1.png` & `kvxopt-1.3.2.1/doc/html/_images/math/124ef7067b147c5c7f031fc0fc06a822029456c1.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/1337abb9748b0985f66823f48527ff07692b910a.png` & `kvxopt-1.3.2.1/doc/html/_images/math/1337abb9748b0985f66823f48527ff07692b910a.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/13abf6ff1ab819235d06737ba4cc4b56c12cf29f.png` & `kvxopt-1.3.2.1/doc/html/_images/math/13abf6ff1ab819235d06737ba4cc4b56c12cf29f.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/145a22013f61134f2b61c99bdc4bf56a23e7ba62.png` & `kvxopt-1.3.2.1/doc/html/_images/math/145a22013f61134f2b61c99bdc4bf56a23e7ba62.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/15ccba8c9b68894aeb55e081c819b82da74b90ed.png` & `kvxopt-1.3.2.1/doc/html/_images/math/15ccba8c9b68894aeb55e081c819b82da74b90ed.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/191bc203fa207a53847c892bc9bc56a69a1c60c1.png` & `kvxopt-1.3.2.1/doc/html/_images/math/191bc203fa207a53847c892bc9bc56a69a1c60c1.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/1e0371cc3025278f588fd7d0ccfcc2510ff2f8cf.png` & `kvxopt-1.3.2.1/doc/html/_images/math/1e0371cc3025278f588fd7d0ccfcc2510ff2f8cf.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/1e7e60bfda710d3db286c7b54852b9cb3e77c861.png` & `kvxopt-1.3.2.1/doc/html/_images/math/1e7e60bfda710d3db286c7b54852b9cb3e77c861.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/211a6aeaec6adf6a5dd8e0c7de1c4e9f4635ad25.png` & `kvxopt-1.3.2.1/doc/html/_images/math/211a6aeaec6adf6a5dd8e0c7de1c4e9f4635ad25.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/21281aa0c6a6c01b835faeb9de4a5ba91527df33.png` & `kvxopt-1.3.2.1/doc/html/_images/math/21281aa0c6a6c01b835faeb9de4a5ba91527df33.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/2149e945c5e7e174b2a1146a3669a5a0b1c65f32.png` & `kvxopt-1.3.2.1/doc/html/_images/math/2149e945c5e7e174b2a1146a3669a5a0b1c65f32.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/21f2b425bff574fa56ee14ddbb7517747adb4266.png` & `kvxopt-1.3.2.1/doc/html/_images/math/21f2b425bff574fa56ee14ddbb7517747adb4266.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/2211f73518e89008db8e07b1bb8a7b8881d0263f.png` & `kvxopt-1.3.2.1/doc/html/_images/math/2211f73518e89008db8e07b1bb8a7b8881d0263f.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/23507579d8ee310e9bc7a287d88d48f8f5ab891f.png` & `kvxopt-1.3.2.1/doc/html/_images/math/23507579d8ee310e9bc7a287d88d48f8f5ab891f.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/26e45da42a12ddc160256fb6cbbb944eeba0dee8.png` & `kvxopt-1.3.2.1/doc/html/_images/math/26e45da42a12ddc160256fb6cbbb944eeba0dee8.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/2877bec99a56fcd4a3f6b39b56c2fe14acb7ee94.png` & `kvxopt-1.3.2.1/doc/html/_images/math/2877bec99a56fcd4a3f6b39b56c2fe14acb7ee94.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/294ea142766a27b4576f8c3240182c9220174aad.png` & `kvxopt-1.3.2.1/doc/html/_images/math/294ea142766a27b4576f8c3240182c9220174aad.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/296e9942f8952b0eda9b312b690a6662f47008e9.png` & `kvxopt-1.3.2.1/doc/html/_images/math/296e9942f8952b0eda9b312b690a6662f47008e9.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/2ac45fcc15c7339cc8ecbdb592c53bc49bf33c73.png` & `kvxopt-1.3.2.1/doc/html/_images/math/2ac45fcc15c7339cc8ecbdb592c53bc49bf33c73.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/2c0f91e60d2f13fdeba173121a264d745555e902.png` & `kvxopt-1.3.2.1/doc/html/_images/math/2c0f91e60d2f13fdeba173121a264d745555e902.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/2e7d885be2f8d9a7556b4e6dded7b42315803547.png` & `kvxopt-1.3.2.1/doc/html/_images/math/2e7d885be2f8d9a7556b4e6dded7b42315803547.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/306121f2c5a959611abb74ce19acd25173d3cb33.png` & `kvxopt-1.3.2.1/doc/html/_images/math/306121f2c5a959611abb74ce19acd25173d3cb33.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/3157de5f84013f57240cf058275c3ae9deb3287a.png` & `kvxopt-1.3.2.1/doc/html/_images/math/3157de5f84013f57240cf058275c3ae9deb3287a.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/322793af4baec9f7ebaa53c4c21f4a468036799a.png` & `kvxopt-1.3.2.1/doc/html/_images/math/322793af4baec9f7ebaa53c4c21f4a468036799a.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/32cab048b453581f0ca59dc31e33e56b7c8b3a0e.png` & `kvxopt-1.3.2.1/doc/html/_images/math/32cab048b453581f0ca59dc31e33e56b7c8b3a0e.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/340c54d7b4f301eb582e5ce306364e1cc4fe20b1.png` & `kvxopt-1.3.2.1/doc/html/_images/math/340c54d7b4f301eb582e5ce306364e1cc4fe20b1.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/34a857941bc037025e34cfc7d5ddf0cba068c3f7.png` & `kvxopt-1.3.2.1/doc/html/_images/math/34a857941bc037025e34cfc7d5ddf0cba068c3f7.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/36dfce98812a98045ee08f8608788e512eed0fe3.png` & `kvxopt-1.3.2.1/doc/html/_images/math/36dfce98812a98045ee08f8608788e512eed0fe3.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/3725c3144c904e39aef17290ef9fdefa9e3adfe0.png` & `kvxopt-1.3.2.1/doc/html/_images/math/3725c3144c904e39aef17290ef9fdefa9e3adfe0.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/37ab88a567d07e7cd18072c1f9878e17b26e1a6a.png` & `kvxopt-1.3.2.1/doc/html/_images/math/37ab88a567d07e7cd18072c1f9878e17b26e1a6a.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/385dad5a2df2ddd65900bef4c4ab58d4a4a0829d.png` & `kvxopt-1.3.2.1/doc/html/_images/math/385dad5a2df2ddd65900bef4c4ab58d4a4a0829d.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/3910830c8976bd5c91219274bd08ca0401852b45.png` & `kvxopt-1.3.2.1/doc/html/_images/math/3910830c8976bd5c91219274bd08ca0401852b45.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/39848b64dc282be81d51d8786746c0b13bd48bcc.png` & `kvxopt-1.3.2.1/doc/html/_images/math/39848b64dc282be81d51d8786746c0b13bd48bcc.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/3a138e23ab33c536c23ad13ff28606737fe7e610.png` & `kvxopt-1.3.2.1/doc/html/_images/math/3a138e23ab33c536c23ad13ff28606737fe7e610.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/3b0de39a2c386bc0f8d5ee56519cab864e57d389.png` & `kvxopt-1.3.2.1/doc/html/_images/math/3b0de39a2c386bc0f8d5ee56519cab864e57d389.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/3b8df11e628aac991d176b270cf335fd89834cfc.png` & `kvxopt-1.3.2.1/doc/html/_images/math/3b8df11e628aac991d176b270cf335fd89834cfc.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/3f12bcd60dcbf296614984241c025a909a803e1e.png` & `kvxopt-1.3.2.1/doc/html/_images/math/3f12bcd60dcbf296614984241c025a909a803e1e.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/3f1dd94c34f67811ddb2df9812cfb065dea10aac.png` & `kvxopt-1.3.2.1/doc/html/_images/math/3f1dd94c34f67811ddb2df9812cfb065dea10aac.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/3f7c5e248ea93d509e428921ea91f68e03f1b029.png` & `kvxopt-1.3.2.1/doc/html/_images/math/3f7c5e248ea93d509e428921ea91f68e03f1b029.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/3fb48872eb2d412f7878dd8934dab8823ce6422b.png` & `kvxopt-1.3.2.1/doc/html/_images/math/3fb48872eb2d412f7878dd8934dab8823ce6422b.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/3fd3b9b7b701e9534c715081f10fd72d4c4670f6.png` & `kvxopt-1.3.2.1/doc/html/_images/math/3fd3b9b7b701e9534c715081f10fd72d4c4670f6.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/42e6ff06c5afcf7438f6b7bd0027c3c738feceb6.png` & `kvxopt-1.3.2.1/doc/html/_images/math/42e6ff06c5afcf7438f6b7bd0027c3c738feceb6.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/4568da7a353653545f711003d54f38db128766df.png` & `kvxopt-1.3.2.1/doc/html/_images/math/4568da7a353653545f711003d54f38db128766df.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/45ab4648d9d463e88b6a823609eaac81787d876f.png` & `kvxopt-1.3.2.1/doc/html/_images/math/45ab4648d9d463e88b6a823609eaac81787d876f.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/45bf7a5d17860fe8ca50fd24ff910e00ce5f8a39.png` & `kvxopt-1.3.2.1/doc/html/_images/math/45bf7a5d17860fe8ca50fd24ff910e00ce5f8a39.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/45ca0c9c05f16b36175b595487b17f411e30a5d6.png` & `kvxopt-1.3.2.1/doc/html/_images/math/45ca0c9c05f16b36175b595487b17f411e30a5d6.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/46362a8b56ad9a6cb816f0062260ad22a76b6f08.png` & `kvxopt-1.3.2.1/doc/html/_images/math/46362a8b56ad9a6cb816f0062260ad22a76b6f08.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/4786cdb10b56effd1cbd6730d8a8497748d072c0.png` & `kvxopt-1.3.2.1/doc/html/_images/math/4786cdb10b56effd1cbd6730d8a8497748d072c0.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/4798110dbfdeb1ecd95e4f30fe61ccf31ce4f503.png` & `kvxopt-1.3.2.1/doc/html/_images/math/4798110dbfdeb1ecd95e4f30fe61ccf31ce4f503.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/482017ed70f2f392091ce55bf925c4d264ca15ba.png` & `kvxopt-1.3.2.1/doc/html/_images/math/482017ed70f2f392091ce55bf925c4d264ca15ba.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/485e65f87f30e5ab52138c945744fe97e6dd87dc.png` & `kvxopt-1.3.2.1/doc/html/_images/math/485e65f87f30e5ab52138c945744fe97e6dd87dc.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/487040712ec6e78e6ce843fdedb84752b97c2547.png` & `kvxopt-1.3.2.1/doc/html/_images/math/487040712ec6e78e6ce843fdedb84752b97c2547.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/4c8eef5c3334015a2ce256c6afde864dcac2b7ad.png` & `kvxopt-1.3.2.1/doc/html/_images/math/4c8eef5c3334015a2ce256c6afde864dcac2b7ad.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/4e317307fb34d4308336c7711497db123b7d9def.png` & `kvxopt-1.3.2.1/doc/html/_images/math/4e317307fb34d4308336c7711497db123b7d9def.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/4e3f3707720cdc0ad65a45a1568034b0499846a9.png` & `kvxopt-1.3.2.1/doc/html/_images/math/4e3f3707720cdc0ad65a45a1568034b0499846a9.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/4f7be1be65d6087c8016b324e3d3e258e12f405d.png` & `kvxopt-1.3.2.1/doc/html/_images/math/4f7be1be65d6087c8016b324e3d3e258e12f405d.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/5046b770f82749051a01f8f102c8e5ff69c4a3e4.png` & `kvxopt-1.3.2.1/doc/html/_images/math/5046b770f82749051a01f8f102c8e5ff69c4a3e4.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/54cbbb3d4691d21c5f1604825fce3e264ef4e7cb.png` & `kvxopt-1.3.2.1/doc/html/_images/math/54cbbb3d4691d21c5f1604825fce3e264ef4e7cb.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/55eedb919b02b7a0654137bd319d8bb919ad3067.png` & `kvxopt-1.3.2.1/doc/html/_images/math/55eedb919b02b7a0654137bd319d8bb919ad3067.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/56ac83c03464e42463c625f1f9ef1833a2927d2e.png` & `kvxopt-1.3.2.1/doc/html/_images/math/56ac83c03464e42463c625f1f9ef1833a2927d2e.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/56ebcc22b7fc4da65f58f0819b21a4c7da613bd4.png` & `kvxopt-1.3.2.1/doc/html/_images/math/56ebcc22b7fc4da65f58f0819b21a4c7da613bd4.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/582940bfca19aac437939d3e7b6be8c577797dad.png` & `kvxopt-1.3.2.1/doc/html/_images/math/582940bfca19aac437939d3e7b6be8c577797dad.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/5d759a9a1a42876f1cefe2c9fc361df2a167d545.png` & `kvxopt-1.3.2.1/doc/html/_images/math/5d759a9a1a42876f1cefe2c9fc361df2a167d545.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/5dacf40fdb001db01bc47f5b86fcb7ce6dc4a0e2.png` & `kvxopt-1.3.2.1/doc/html/_images/math/5dacf40fdb001db01bc47f5b86fcb7ce6dc4a0e2.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/5fa951f18d59f8caa1d2bc6ec81f6a0c945bfe75.png` & `kvxopt-1.3.2.1/doc/html/_images/math/5fa951f18d59f8caa1d2bc6ec81f6a0c945bfe75.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/61425e89ec518b2689e5063426419950648cd2dc.png` & `kvxopt-1.3.2.1/doc/html/_images/math/61425e89ec518b2689e5063426419950648cd2dc.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/61a7d25e3673146402ed26716d6eb60e8e9d18fa.png` & `kvxopt-1.3.2.1/doc/html/_images/math/61a7d25e3673146402ed26716d6eb60e8e9d18fa.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/620321226792601132c52174a5287a8c93e9bc5f.png` & `kvxopt-1.3.2.1/doc/html/_images/math/620321226792601132c52174a5287a8c93e9bc5f.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/627d2d6ebe12e40470cbb763687cffb52453abe1.png` & `kvxopt-1.3.2.1/doc/html/_images/math/627d2d6ebe12e40470cbb763687cffb52453abe1.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/62cd1c16ca3ef9e2b0d5696a6a49b6b5a6d19130.png` & `kvxopt-1.3.2.1/doc/html/_images/math/62cd1c16ca3ef9e2b0d5696a6a49b6b5a6d19130.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/64824b782d63f742bca8b398e0f12b485771f257.png` & `kvxopt-1.3.2.1/doc/html/_images/math/64824b782d63f742bca8b398e0f12b485771f257.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/6565000626ccf19f09a9258e78e141cb5ce46180.png` & `kvxopt-1.3.2.1/doc/html/_images/math/6565000626ccf19f09a9258e78e141cb5ce46180.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/66599856ec5735a610623bbe8242fc777d5f4100.png` & `kvxopt-1.3.2.1/doc/html/_images/math/66599856ec5735a610623bbe8242fc777d5f4100.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/6669c8a566ba908085156b5c4a539af53616f383.png` & `kvxopt-1.3.2.1/doc/html/_images/math/6669c8a566ba908085156b5c4a539af53616f383.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/66e3f8da85954ae75f6016f5784d0ec468c2451c.png` & `kvxopt-1.3.2.1/doc/html/_images/math/66e3f8da85954ae75f6016f5784d0ec468c2451c.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/68ea4366a8e9dac6f50d5b899ac5c385374d9673.png` & `kvxopt-1.3.2.1/doc/html/_images/math/68ea4366a8e9dac6f50d5b899ac5c385374d9673.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/694498e646bcebcf71487704e8bbabe9b2665425.png` & `kvxopt-1.3.2.1/doc/html/_images/math/694498e646bcebcf71487704e8bbabe9b2665425.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/6b3a21804f75fb45e7f9963fc6c0621fcf710cc7.png` & `kvxopt-1.3.2.1/doc/html/_images/math/6b3a21804f75fb45e7f9963fc6c0621fcf710cc7.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/6b3d942743e5a56e5030cfaab836f542fec9019c.png` & `kvxopt-1.3.2.1/doc/html/_images/math/6b3d942743e5a56e5030cfaab836f542fec9019c.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/6d9473d4787aece2804514f0796e6abeb2ce4dda.png` & `kvxopt-1.3.2.1/doc/html/_images/math/6d9473d4787aece2804514f0796e6abeb2ce4dda.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/6dd83f47897e8af1a287a2cb577906b4c142c166.png` & `kvxopt-1.3.2.1/doc/html/_images/math/6dd83f47897e8af1a287a2cb577906b4c142c166.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/6efd575f4ef0199dda05d5b8f4a187112a62224b.png` & `kvxopt-1.3.2.1/doc/html/_images/math/6efd575f4ef0199dda05d5b8f4a187112a62224b.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/7056acd535c8f98331e8dd89e48cc0e927d42b12.png` & `kvxopt-1.3.2.1/doc/html/_images/math/7056acd535c8f98331e8dd89e48cc0e927d42b12.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/7075b711b50c004803b51912b9dca99d35c65d35.png` & `kvxopt-1.3.2.1/doc/html/_images/math/7075b711b50c004803b51912b9dca99d35c65d35.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/70b640ff0659b7d33287ba001e5b26c6c93a96ba.png` & `kvxopt-1.3.2.1/doc/html/_images/math/70b640ff0659b7d33287ba001e5b26c6c93a96ba.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/716fbcea39bcb0c1e19a3e26c60836bf5b111b91.png` & `kvxopt-1.3.2.1/doc/html/_images/math/716fbcea39bcb0c1e19a3e26c60836bf5b111b91.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/727233e1f841277ba9bce9859cd9fbbe664f1667.png` & `kvxopt-1.3.2.1/doc/html/_images/math/727233e1f841277ba9bce9859cd9fbbe664f1667.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/738092734154893db4338bbdedae2ef8c48eade3.png` & `kvxopt-1.3.2.1/doc/html/_images/math/738092734154893db4338bbdedae2ef8c48eade3.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/73e26546f3f051d6cc494fa37072d2eac9856ac1.png` & `kvxopt-1.3.2.1/doc/html/_images/math/73e26546f3f051d6cc494fa37072d2eac9856ac1.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/7627c2662a2a563bf350d8d618dd7e6d40c35e2e.png` & `kvxopt-1.3.2.1/doc/html/_images/math/7627c2662a2a563bf350d8d618dd7e6d40c35e2e.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/767b9280eb4c7a6ad46be67cb9782508dc6d1f22.png` & `kvxopt-1.3.2.1/doc/html/_images/math/767b9280eb4c7a6ad46be67cb9782508dc6d1f22.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/783499b0add3c6f6f392a2b8d39402a6aa232020.png` & `kvxopt-1.3.2.1/doc/html/_images/math/783499b0add3c6f6f392a2b8d39402a6aa232020.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/78d5bb409e88f612d4afe2cca2f43186923387e6.png` & `kvxopt-1.3.2.1/doc/html/_images/math/78d5bb409e88f612d4afe2cca2f43186923387e6.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/7b25a0b8e9e5569bb0e977a9ea61b5daedb78e11.png` & `kvxopt-1.3.2.1/doc/html/_images/math/7b25a0b8e9e5569bb0e977a9ea61b5daedb78e11.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/7b694e55a0813fe78e01121684b12a40fad86d86.png` & `kvxopt-1.3.2.1/doc/html/_images/math/7b694e55a0813fe78e01121684b12a40fad86d86.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/7dcb78b012b54b09f8760cec52ce8ae1389f0f11.png` & `kvxopt-1.3.2.1/doc/html/_images/math/7dcb78b012b54b09f8760cec52ce8ae1389f0f11.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/7e65c1c7c403764759e8813348c1b7e2d560f1fa.png` & `kvxopt-1.3.2.1/doc/html/_images/math/7e65c1c7c403764759e8813348c1b7e2d560f1fa.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/7eac6332e16c5424a4b290d2b9f9445c5214a1d1.png` & `kvxopt-1.3.2.1/doc/html/_images/math/7eac6332e16c5424a4b290d2b9f9445c5214a1d1.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/7faf4e55287d19aeb554d113cd37857aeb2700b4.png` & `kvxopt-1.3.2.1/doc/html/_images/math/7faf4e55287d19aeb554d113cd37857aeb2700b4.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/80e21626c375d52667de27ff84715270afb8ca70.png` & `kvxopt-1.3.2.1/doc/html/_images/math/80e21626c375d52667de27ff84715270afb8ca70.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/81787f23988417db8fee122d8cc6141a1985c4b7.png` & `kvxopt-1.3.2.1/doc/html/_images/math/81787f23988417db8fee122d8cc6141a1985c4b7.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/817f53603d7e46d0c89d94f741f3ff760e7b4e64.png` & `kvxopt-1.3.2.1/doc/html/_images/math/817f53603d7e46d0c89d94f741f3ff760e7b4e64.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/81868e29eaf33185bcc60e1d6ff7b0e307f2f892.png` & `kvxopt-1.3.2.1/doc/html/_images/math/81868e29eaf33185bcc60e1d6ff7b0e307f2f892.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/82a55744f92063b61aaffddd2380a5cbf8a2b1c6.png` & `kvxopt-1.3.2.1/doc/html/_images/math/82a55744f92063b61aaffddd2380a5cbf8a2b1c6.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/82d7fac4e1442a73c02aa8bd6fedab161db0f758.png` & `kvxopt-1.3.2.1/doc/html/_images/math/82d7fac4e1442a73c02aa8bd6fedab161db0f758.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/838e2b03a608af26db2efa9096182aa54d809a3d.png` & `kvxopt-1.3.2.1/doc/html/_images/math/838e2b03a608af26db2efa9096182aa54d809a3d.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/84e264805077d2cf923fe75d31e2ed50021618da.png` & `kvxopt-1.3.2.1/doc/html/_images/math/84e264805077d2cf923fe75d31e2ed50021618da.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/86384124ce2e714ba7b80c295f44157d2da07413.png` & `kvxopt-1.3.2.1/doc/html/_images/math/86384124ce2e714ba7b80c295f44157d2da07413.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/8655418fcbc61747ed3bd70aa2d1ecc1db06a5c9.png` & `kvxopt-1.3.2.1/doc/html/_images/math/8655418fcbc61747ed3bd70aa2d1ecc1db06a5c9.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/86a2d178f8f888b9c84ff42573fdaf015c8bfbb2.png` & `kvxopt-1.3.2.1/doc/html/_images/math/86a2d178f8f888b9c84ff42573fdaf015c8bfbb2.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/86cec286c2bbedaa7760445bc5a1a242cb84d2c2.png` & `kvxopt-1.3.2.1/doc/html/_images/math/86cec286c2bbedaa7760445bc5a1a242cb84d2c2.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/870c60a6ab1247468ddfc5be8f68ffbe3479dfda.png` & `kvxopt-1.3.2.1/doc/html/_images/math/870c60a6ab1247468ddfc5be8f68ffbe3479dfda.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/8871516499f79705d3818c3251aacd463f7c5146.png` & `kvxopt-1.3.2.1/doc/html/_images/math/8871516499f79705d3818c3251aacd463f7c5146.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/887be39f02687d3e3a1565193924f04d7ccbb743.png` & `kvxopt-1.3.2.1/doc/html/_images/math/887be39f02687d3e3a1565193924f04d7ccbb743.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/895591ad55b7e2cec6ade3bbb0bb1a0b76fe0910.png` & `kvxopt-1.3.2.1/doc/html/_images/math/895591ad55b7e2cec6ade3bbb0bb1a0b76fe0910.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/89d343471476626b56bc496f09d8fad108cb82a6.png` & `kvxopt-1.3.2.1/doc/html/_images/math/89d343471476626b56bc496f09d8fad108cb82a6.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/8c1dcc7704e1d156a5f896c8c0a3326c2722a3fa.png` & `kvxopt-1.3.2.1/doc/html/_images/math/8c1dcc7704e1d156a5f896c8c0a3326c2722a3fa.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/8c51b26db8908731ed17a76ed86a9fe1c99aa02b.png` & `kvxopt-1.3.2.1/doc/html/_images/math/8c51b26db8908731ed17a76ed86a9fe1c99aa02b.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/8d26408b917ad631b6ae90f7650b19b691fe2bb6.png` & `kvxopt-1.3.2.1/doc/html/_images/math/8d26408b917ad631b6ae90f7650b19b691fe2bb6.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/8d53a80f87a15ba0d310801a0af822da73c3fcaf.png` & `kvxopt-1.3.2.1/doc/html/_images/math/8d53a80f87a15ba0d310801a0af822da73c3fcaf.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/8edd44acd8c3889706afee3c81bb907c3f415683.png` & `kvxopt-1.3.2.1/doc/html/_images/math/8edd44acd8c3889706afee3c81bb907c3f415683.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/8fcff6b5a5c95afb39f5abaedac94b7086911410.png` & `kvxopt-1.3.2.1/doc/html/_images/math/8fcff6b5a5c95afb39f5abaedac94b7086911410.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/908a083a0806ab219190adac99ec60da04c65f48.png` & `kvxopt-1.3.2.1/doc/html/_images/math/908a083a0806ab219190adac99ec60da04c65f48.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/9173aacc17760942bd0ce61e5ad70788a84297d5.png` & `kvxopt-1.3.2.1/doc/html/_images/math/9173aacc17760942bd0ce61e5ad70788a84297d5.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/957b97bc1591647fef3ac407dd3dd3e99c37fcd5.png` & `kvxopt-1.3.2.1/doc/html/_images/math/957b97bc1591647fef3ac407dd3dd3e99c37fcd5.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/95a6e48cc402e2e0cee2fe87d159320f12dcadfc.png` & `kvxopt-1.3.2.1/doc/html/_images/math/95a6e48cc402e2e0cee2fe87d159320f12dcadfc.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/95af1725828b1a188bbb0d933ffc78ef94788a48.png` & `kvxopt-1.3.2.1/doc/html/_images/math/95af1725828b1a188bbb0d933ffc78ef94788a48.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/95c7fad2a12f832a0675a00c80c4a8894297d2b8.png` & `kvxopt-1.3.2.1/doc/html/_images/math/95c7fad2a12f832a0675a00c80c4a8894297d2b8.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/973e7149b3e7c5fd4b7a92e36771cc6c2d6e620b.png` & `kvxopt-1.3.2.1/doc/html/_images/math/973e7149b3e7c5fd4b7a92e36771cc6c2d6e620b.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/9f18ba54fa478c728e3a3536166f874c17aa7c04.png` & `kvxopt-1.3.2.1/doc/html/_images/math/9f18ba54fa478c728e3a3536166f874c17aa7c04.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/9f2f3a7e9359d5459533e3d50282ebae0ca36465.png` & `kvxopt-1.3.2.1/doc/html/_images/math/9f2f3a7e9359d5459533e3d50282ebae0ca36465.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/a121b0efd1dfa559be59e332b528608d97906c46.png` & `kvxopt-1.3.2.1/doc/html/_images/math/a121b0efd1dfa559be59e332b528608d97906c46.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/a133c9dd8091526f677cfcc502fbf773387d84bf.png` & `kvxopt-1.3.2.1/doc/html/_images/math/a133c9dd8091526f677cfcc502fbf773387d84bf.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/a38b44a27c1755531418f8bb853736ab038d7e9e.png` & `kvxopt-1.3.2.1/doc/html/_images/math/a38b44a27c1755531418f8bb853736ab038d7e9e.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/a444daac219907b51a5edd730d624c53328d693f.png` & `kvxopt-1.3.2.1/doc/html/_images/math/a444daac219907b51a5edd730d624c53328d693f.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/a4594eb66f65c9a3e69736f82fdb072d08b8ddcc.png` & `kvxopt-1.3.2.1/doc/html/_images/math/a4594eb66f65c9a3e69736f82fdb072d08b8ddcc.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/a5d23ddad04b332c54e468fd62d6493589d61339.png` & `kvxopt-1.3.2.1/doc/html/_images/math/a5d23ddad04b332c54e468fd62d6493589d61339.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/a6b6966ce67e827face4426ab49db20ec6a74a9e.png` & `kvxopt-1.3.2.1/doc/html/_images/math/a6b6966ce67e827face4426ab49db20ec6a74a9e.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/a810215e77878dec996b87e0d3007d8a6ded6b3c.png` & `kvxopt-1.3.2.1/doc/html/_images/math/a810215e77878dec996b87e0d3007d8a6ded6b3c.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/aa4d3057edd3aea1af61b5571a9e06258b978843.png` & `kvxopt-1.3.2.1/doc/html/_images/math/aa4d3057edd3aea1af61b5571a9e06258b978843.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/aaf1e4f8649093b3b1a2a201c97238b5d922ff96.png` & `kvxopt-1.3.2.1/doc/html/_images/math/aaf1e4f8649093b3b1a2a201c97238b5d922ff96.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/aaf2039a0ca644d308dc578303aa096fd3775907.png` & `kvxopt-1.3.2.1/doc/html/_images/math/aaf2039a0ca644d308dc578303aa096fd3775907.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/ab466a647f375d548d3b12c0c1ecb79704cef8d0.png` & `kvxopt-1.3.2.1/doc/html/_images/math/ab466a647f375d548d3b12c0c1ecb79704cef8d0.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/ac5ad3214d3caf44e5cc4e9514908ba2a7bb48dc.png` & `kvxopt-1.3.2.1/doc/html/_images/math/ac5ad3214d3caf44e5cc4e9514908ba2a7bb48dc.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/ad2c8101af3f233ceefa1ec6865721f302b84cfd.png` & `kvxopt-1.3.2.1/doc/html/_images/math/ad2c8101af3f233ceefa1ec6865721f302b84cfd.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/ae4ca00a7da101aa137fa6b84b5467ce39b05349.png` & `kvxopt-1.3.2.1/doc/html/_images/math/ae4ca00a7da101aa137fa6b84b5467ce39b05349.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/ae6d9abfed9fac62837d0c88a97a8afc81b5e712.png` & `kvxopt-1.3.2.1/doc/html/_images/math/ae6d9abfed9fac62837d0c88a97a8afc81b5e712.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/b3b09dbd48529f16a62f1020d2172bb9551e3296.png` & `kvxopt-1.3.2.1/doc/html/_images/math/b3b09dbd48529f16a62f1020d2172bb9551e3296.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/b6c16fed84a824ab88468f81a2b505ac69ad7505.png` & `kvxopt-1.3.2.1/doc/html/_images/math/b6c16fed84a824ab88468f81a2b505ac69ad7505.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/b7e4addc1a00973125d6c3b9ba5bd951e6486df5.png` & `kvxopt-1.3.2.1/doc/html/_images/math/b7e4addc1a00973125d6c3b9ba5bd951e6486df5.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/b8c391eb9c602cc714b875704be76879e335e243.png` & `kvxopt-1.3.2.1/doc/html/_images/math/b8c391eb9c602cc714b875704be76879e335e243.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/b934c490f51b68bde94c85bb2c77c160a78731bc.png` & `kvxopt-1.3.2.1/doc/html/_images/math/b934c490f51b68bde94c85bb2c77c160a78731bc.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/b9f9b8057126c1f181b745e36de7f60ecbe4e41d.png` & `kvxopt-1.3.2.1/doc/html/_images/math/b9f9b8057126c1f181b745e36de7f60ecbe4e41d.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/bc28eed8cb92072618037ffe78d36cdf031045b0.png` & `kvxopt-1.3.2.1/doc/html/_images/math/bc28eed8cb92072618037ffe78d36cdf031045b0.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/bcfcc32ea50d37180cedf362db80a4901cbc05bd.png` & `kvxopt-1.3.2.1/doc/html/_images/math/bcfcc32ea50d37180cedf362db80a4901cbc05bd.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/bd041563b2dc47337d212c089f31e14b6b95e033.png` & `kvxopt-1.3.2.1/doc/html/_images/math/bd041563b2dc47337d212c089f31e14b6b95e033.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/c0ff36623c1ad325126fbebd6724e58809c4fdd2.png` & `kvxopt-1.3.2.1/doc/html/_images/math/c0ff36623c1ad325126fbebd6724e58809c4fdd2.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/c20519763e75b58870bd25238b358057e2da4b86.png` & `kvxopt-1.3.2.1/doc/html/_images/math/c20519763e75b58870bd25238b358057e2da4b86.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/c34401e75e80cc822827c5d5175de08a5bbffced.png` & `kvxopt-1.3.2.1/doc/html/_images/math/c34401e75e80cc822827c5d5175de08a5bbffced.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/c72b037a60f8e81dc19add786e6d148794471f80.png` & `kvxopt-1.3.2.1/doc/html/_images/math/c72b037a60f8e81dc19add786e6d148794471f80.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/c7fb856181b7b0b9f3cf0ca66c11fe63ea2b7278.png` & `kvxopt-1.3.2.1/doc/html/_images/math/c7fb856181b7b0b9f3cf0ca66c11fe63ea2b7278.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/c94d8558b73b7597cc60b6a0ec7c758f40c88a8d.png` & `kvxopt-1.3.2.1/doc/html/_images/math/c94d8558b73b7597cc60b6a0ec7c758f40c88a8d.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/c9a3af023076f58fe1ee0b35f88cad484ba194fa.png` & `kvxopt-1.3.2.1/doc/html/_images/math/c9a3af023076f58fe1ee0b35f88cad484ba194fa.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/ccfd8c814cc1234e5dc5fce8871570757d15515c.png` & `kvxopt-1.3.2.1/doc/html/_images/math/ccfd8c814cc1234e5dc5fce8871570757d15515c.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/cd4c2f3674b5e0def3984a035f720209c8391074.png` & `kvxopt-1.3.2.1/doc/html/_images/math/cd4c2f3674b5e0def3984a035f720209c8391074.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/d2241f81f782d8593f9390f06af621fd3be21ab8.png` & `kvxopt-1.3.2.1/doc/html/_images/math/d2241f81f782d8593f9390f06af621fd3be21ab8.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/d246dde9fc63993c5b8df2eaccfa78ef89ad875d.png` & `kvxopt-1.3.2.1/doc/html/_images/math/d246dde9fc63993c5b8df2eaccfa78ef89ad875d.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/d33cbbeb57b535cc4b2562e25475f7afc74ae85b.png` & `kvxopt-1.3.2.1/doc/html/_images/math/d33cbbeb57b535cc4b2562e25475f7afc74ae85b.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/d3b5cc5b170fbda975293f38dea08b951f37142f.png` & `kvxopt-1.3.2.1/doc/html/_images/math/d3b5cc5b170fbda975293f38dea08b951f37142f.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/d452b345239711d0be1016ccde4ddfea5930b072.png` & `kvxopt-1.3.2.1/doc/html/_images/math/d452b345239711d0be1016ccde4ddfea5930b072.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/d504b5e2a3245798a6ad5678ea1951fc914e8fac.png` & `kvxopt-1.3.2.1/doc/html/_images/math/d504b5e2a3245798a6ad5678ea1951fc914e8fac.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/d56da07a3d18c9fc980ecc0a9696603bd8d8dcd2.png` & `kvxopt-1.3.2.1/doc/html/_images/math/d56da07a3d18c9fc980ecc0a9696603bd8d8dcd2.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/d5a4cdcdf8e599dc8e0d8a8c1301f02f9e8b4fb3.png` & `kvxopt-1.3.2.1/doc/html/_images/math/d5a4cdcdf8e599dc8e0d8a8c1301f02f9e8b4fb3.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/d66b4ab25c0eef60d649ef489104789f43f45a0b.png` & `kvxopt-1.3.2.1/doc/html/_images/math/d66b4ab25c0eef60d649ef489104789f43f45a0b.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/d767754db8d214ccf0dcaf05b48317d378fbddb5.png` & `kvxopt-1.3.2.1/doc/html/_images/math/d767754db8d214ccf0dcaf05b48317d378fbddb5.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/d9aec1e99d1bcb92578727e61fb60d877c0964b7.png` & `kvxopt-1.3.2.1/doc/html/_images/math/d9aec1e99d1bcb92578727e61fb60d877c0964b7.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/da8dad38c611fbd068672223f3f152e89ee7477e.png` & `kvxopt-1.3.2.1/doc/html/_images/math/da8dad38c611fbd068672223f3f152e89ee7477e.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/dba423937c7e0c09118ccac03f01a4a3be60e2c3.png` & `kvxopt-1.3.2.1/doc/html/_images/math/dba423937c7e0c09118ccac03f01a4a3be60e2c3.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/dcab68360c480e6aaf0001fa1fb3f6451ba747f0.png` & `kvxopt-1.3.2.1/doc/html/_images/math/dcab68360c480e6aaf0001fa1fb3f6451ba747f0.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/deb40d5eca48a271c62dc3937746712359cd3b05.png` & `kvxopt-1.3.2.1/doc/html/_images/math/deb40d5eca48a271c62dc3937746712359cd3b05.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/e2f6bbba20da0d51564b1855eb2da3072d841441.png` & `kvxopt-1.3.2.1/doc/html/_images/math/e2f6bbba20da0d51564b1855eb2da3072d841441.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/e35d7cbe33a34f4456eea34b9bd28642bfc52fa4.png` & `kvxopt-1.3.2.1/doc/html/_images/math/e35d7cbe33a34f4456eea34b9bd28642bfc52fa4.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/e3a50552a1b736116240d899eea184ca3106ba0c.png` & `kvxopt-1.3.2.1/doc/html/_images/math/e3a50552a1b736116240d899eea184ca3106ba0c.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/e3f4c5bf9e0470ceafd97d572163a4dfefc39743.png` & `kvxopt-1.3.2.1/doc/html/_images/math/e3f4c5bf9e0470ceafd97d572163a4dfefc39743.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/e50141a6a4a3490d1acc94e54f7de36ac5f7e8eb.png` & `kvxopt-1.3.2.1/doc/html/_images/math/e50141a6a4a3490d1acc94e54f7de36ac5f7e8eb.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/e61f71e6c396a94105e3437275d3449a61f9d802.png` & `kvxopt-1.3.2.1/doc/html/_images/math/e61f71e6c396a94105e3437275d3449a61f9d802.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/e97fe83d126fdd192e9bc593cea89698fb36ffe5.png` & `kvxopt-1.3.2.1/doc/html/_images/math/e97fe83d126fdd192e9bc593cea89698fb36ffe5.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/eb873a106ad1868e288ae26783dd930d360fdef5.png` & `kvxopt-1.3.2.1/doc/html/_images/math/eb873a106ad1868e288ae26783dd930d360fdef5.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/ed29c4b1667b0282bad6523664351811e0f23dab.png` & `kvxopt-1.3.2.1/doc/html/_images/math/ed29c4b1667b0282bad6523664351811e0f23dab.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/ee3c949541ac51ceadec0a62713cdd8a42a2e4ab.png` & `kvxopt-1.3.2.1/doc/html/_images/math/ee3c949541ac51ceadec0a62713cdd8a42a2e4ab.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/efe5c37bc03bf3d5826fd02dc5b43a0a51e7c271.png` & `kvxopt-1.3.2.1/doc/html/_images/math/efe5c37bc03bf3d5826fd02dc5b43a0a51e7c271.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/f59b4bcd76f97da1f13ba87bc76bf52b442b4381.png` & `kvxopt-1.3.2.1/doc/html/_images/math/f59b4bcd76f97da1f13ba87bc76bf52b442b4381.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/f86c7a0b45da8cc7f4a00c20bf654b3df94ff06a.png` & `kvxopt-1.3.2.1/doc/html/_images/math/f86c7a0b45da8cc7f4a00c20bf654b3df94ff06a.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/facdb23d2bcdc9cf5d90ab695c86965ac188e3e5.png` & `kvxopt-1.3.2.1/doc/html/_images/math/facdb23d2bcdc9cf5d90ab695c86965ac188e3e5.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/fb07faac9fe824b206392c19b7a1a2c6dd70e1ee.png` & `kvxopt-1.3.2.1/doc/html/_images/math/fb07faac9fe824b206392c19b7a1a2c6dd70e1ee.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/fc16f4da2e0dd685363c204baf675d6244c52fbb.png` & `kvxopt-1.3.2.1/doc/html/_images/math/fc16f4da2e0dd685363c204baf675d6244c52fbb.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/fcc17fd59806862a629796f0d7f0e8f43778e7bd.png` & `kvxopt-1.3.2.1/doc/html/_images/math/fcc17fd59806862a629796f0d7f0e8f43778e7bd.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/math/fe748f1ddebc2719b738533481dc2070aa3f8b04.png` & `kvxopt-1.3.2.1/doc/html/_images/math/fe748f1ddebc2719b738533481dc2070aa3f8b04.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/normappr.png` & `kvxopt-1.3.2.1/doc/html/_images/normappr.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/portfolio1.png` & `kvxopt-1.3.2.1/doc/html/_images/portfolio1.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_images/portfolio2.png` & `kvxopt-1.3.2.1/doc/html/_images/portfolio2.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_static/_sphinx_javascript_frameworks_compat.js` & `kvxopt-1.3.2.1/doc/html/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_static/basic.css` & `kvxopt-1.3.2.1/doc/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_static/css/badge_only.css` & `kvxopt-1.3.2.1/doc/html/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_static/css/fonts/Roboto-Slab-Bold.woff` & `kvxopt-1.3.2.1/doc/html/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_static/css/fonts/Roboto-Slab-Bold.woff2` & `kvxopt-1.3.2.1/doc/html/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_static/css/fonts/Roboto-Slab-Regular.woff` & `kvxopt-1.3.2.1/doc/html/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_static/css/fonts/Roboto-Slab-Regular.woff2` & `kvxopt-1.3.2.1/doc/html/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_static/css/fonts/fontawesome-webfont.eot` & `kvxopt-1.3.2.1/doc/html/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_static/css/fonts/fontawesome-webfont.svg` & `kvxopt-1.3.2.1/doc/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_static/css/fonts/fontawesome-webfont.ttf` & `kvxopt-1.3.2.1/doc/html/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_static/css/fonts/fontawesome-webfont.woff` & `kvxopt-1.3.2.1/doc/html/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_static/css/fonts/fontawesome-webfont.woff2` & `kvxopt-1.3.2.1/doc/html/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_static/css/fonts/lato-bold-italic.woff` & `kvxopt-1.3.2.1/doc/html/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_static/css/fonts/lato-bold-italic.woff2` & `kvxopt-1.3.2.1/doc/html/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_static/css/fonts/lato-bold.woff` & `kvxopt-1.3.2.1/doc/html/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_static/css/fonts/lato-bold.woff2` & `kvxopt-1.3.2.1/doc/html/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_static/css/fonts/lato-normal-italic.woff` & `kvxopt-1.3.2.1/doc/html/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_static/css/fonts/lato-normal-italic.woff2` & `kvxopt-1.3.2.1/doc/html/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_static/css/fonts/lato-normal.woff` & `kvxopt-1.3.2.1/doc/html/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_static/css/fonts/lato-normal.woff2` & `kvxopt-1.3.2.1/doc/html/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_static/css/theme.css` & `kvxopt-1.3.2.1/doc/html/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_static/cvxopt.css` & `kvxopt-1.3.2.1/doc/html/_static/cvxopt.css`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_static/doctools.js` & `kvxopt-1.3.2.1/doc/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_static/jquery-3.6.0.js` & `kvxopt-1.3.2.1/doc/html/_static/jquery-3.6.0.js`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_static/jquery.js` & `kvxopt-1.3.2.1/doc/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_static/js/badge_only.js` & `kvxopt-1.3.2.1/doc/html/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_static/js/html5shiv-printshiv.min.js` & `kvxopt-1.3.2.1/doc/html/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_static/js/html5shiv.min.js` & `kvxopt-1.3.2.1/doc/html/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_static/js/theme.js` & `kvxopt-1.3.2.1/doc/html/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_static/language_data.js` & `kvxopt-1.3.2.1/doc/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_static/pygments.css` & `kvxopt-1.3.2.1/doc/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_static/searchtools.js` & `kvxopt-1.3.2.1/doc/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_static/underscore-1.13.1.js` & `kvxopt-1.3.2.1/doc/html/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/_static/underscore.js` & `kvxopt-1.3.2.1/doc/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/blas.html` & `kvxopt-1.3.2.1/doc/html/blas.html`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/c-api.html` & `kvxopt-1.3.2.1/doc/html/c-api.html`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
            <div itemprop="articleBody">
              
   <section id="c-api">
 <span id="c-capi"></span><h1>C API<a class="headerlink" href="#c-api" title="Permalink to this heading"></a></h1>
 <p>The API can be used to extend CVXOPT with interfaces to external C routines
 and libraries.  A C program that creates or manipulates the dense or sparse
-matrix objects defined in CVXOPT must include the <code class="xref py py-const docutils literal notranslate"><span class="pre">cvxopt.h</span></code> header
+matrix objects defined in CVXOPT must include the <code class="xref py py-const docutils literal notranslate"><span class="pre">kvxopt.h</span></code> header
 file in the <code class="xref py py-const docutils literal notranslate"><span class="pre">src</span></code> directory of the distribution.</p>
 <p>Before the C API can be used in an extension module it must be initialized
 by calling the macro <code class="xref c c-macro docutils literal notranslate"><span class="pre">import_cvxopt</span></code>.  As an example we show the
 module initialization from the <code class="xref py py-mod docutils literal notranslate"><span class="pre">cvxopt.blas</span></code> module, which itself uses
 the API:</p>
 <div class="highlight-c notranslate"><div class="highlight"><pre><span></span><span class="cp">#if PY_MAJOR_VERSION &gt;= 3</span>
 
@@ -123,15 +123,15 @@
 <span class="p">}</span><span class="w"></span>
 
 <span class="cp">#endif</span>
 </pre></div>
 </div>
 <section id="dense-matrices">
 <h2>Dense Matrices<a class="headerlink" href="#dense-matrices" title="Permalink to this heading"></a></h2>
-<p>As can be seen from the header file <code class="xref py py-const docutils literal notranslate"><span class="pre">cvxopt.h</span></code>, a <code class="xref py py-class docutils literal notranslate"><span class="pre">matrix</span></code> is
+<p>As can be seen from the header file <code class="xref py py-const docutils literal notranslate"><span class="pre">kvxopt.h</span></code>, a <code class="xref py py-class docutils literal notranslate"><span class="pre">matrix</span></code> is
 essentially a  structure with four fields.  The fields <code class="xref c c-member docutils literal notranslate"><span class="pre">nrows</span></code> and
 <code class="xref c c-member docutils literal notranslate"><span class="pre">ncols</span></code> are two integers that specify the dimensions.  The
 <code class="xref c c-member docutils literal notranslate"><span class="pre">id</span></code> field controls the type of the matrix and can have values
 <code class="xref py py-const docutils literal notranslate"><span class="pre">DOUBLE</span></code>, <code class="xref py py-const docutils literal notranslate"><span class="pre">INT</span></code>, and <code class="xref py py-const docutils literal notranslate"><span class="pre">COMPLEX</span></code>.  The <code class="xref c c-member docutils literal notranslate"><span class="pre">buffer</span></code>
 field is an array that contains the matrix elements stored contiguously in
 column-major order.</p>
 <p>The following C functions can be used to create matrices.</p>
```

#### html2text {}

```diff
@@ -19,15 +19,15 @@
 _C_V_X_O_P_T_ _U_s_e_r_'_s_ _G_u_i_d_e
     * »
     * C API
 ===============================================================================
 ************ CC AAPPII_? ************
 The API can be used to extend CVXOPT with interfaces to external C routines and
 libraries. A C program that creates or manipulates the dense or sparse matrix
-objects defined in CVXOPT must include the cvxopt.h header file in the src
+objects defined in CVXOPT must include the kvxopt.h header file in the src
 directory of the distribution.
 Before the C API can be used in an extension module it must be initialized by
 calling the macro import_cvxopt. As an example we show the module
 initialization from the cvxopt.blas module, which itself uses the API:
 #if PY_MAJOR_VERSION >= 3
 
 static PyModuleDef blas_module = {
@@ -54,15 +54,15 @@
   PyObject *m;
   m = Py_InitModule3("cvxopt.blas", blas_functions, blas__doc__);
   if (import_cvxopt() < 0) return ;
 }
 
 #endif
 ********** DDeennssee MMaattrriicceess_? **********
-As can be seen from the header file cvxopt.h, a matrix is essentially a
+As can be seen from the header file kvxopt.h, a matrix is essentially a
 structure with four fields. The fields nrows and ncols are two integers that
 specify the dimensions. The id field controls the type of the matrix and can
 have values DOUBLE, INT, and COMPLEX. The buffer field is an array that
 contains the matrix elements stored contiguously in column-major order.
 The following C functions can be used to create matrices.
   matrix *Matrix_New(int nrows, int ncols, int id)_
       Returns a matrix object of typeidwithnrowsrows andncolscolumns. The
```

### Comparing `kvxopt-1.3.2.0/doc/html/coneprog.html` & `kvxopt-1.3.2.1/doc/html/coneprog.html`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/copyright.html` & `kvxopt-1.3.2.1/doc/html/copyright.html`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/fftw.html` & `kvxopt-1.3.2.1/doc/html/fftw.html`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/index.html` & `kvxopt-1.3.2.1/doc/html/index.html`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/intro.html` & `kvxopt-1.3.2.1/doc/html/intro.html`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/lapack.html` & `kvxopt-1.3.2.1/doc/html/lapack.html`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/matrices.html` & `kvxopt-1.3.2.1/doc/html/matrices.html`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/modeling.html` & `kvxopt-1.3.2.1/doc/html/modeling.html`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/objects.inv` & `kvxopt-1.3.2.1/doc/html/objects.inv`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/printing.html` & `kvxopt-1.3.2.1/doc/html/printing.html`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/search.html` & `kvxopt-1.3.2.1/doc/html/search.html`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/searchindex.js` & `kvxopt-1.3.2.1/doc/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/solvers.html` & `kvxopt-1.3.2.1/doc/html/solvers.html`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/html/spsolvers.html` & `kvxopt-1.3.2.1/doc/html/spsolvers.html`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/source/.static/cvxopt.css` & `kvxopt-1.3.2.1/doc/source/.static/cvxopt.css`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/source/blas.rst` & `kvxopt-1.3.2.1/doc/source/blas.rst`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/source/c-api.rst` & `kvxopt-1.3.2.1/doc/source/c-api.rst`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/source/coneprog.rst` & `kvxopt-1.3.2.1/doc/source/coneprog.rst`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/source/conf.py` & `kvxopt-1.3.2.1/doc/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,17 +42,17 @@
 project = "CVXOPT User's Guide"
 copyright = '2004-2023, M.S. Andersen, J. Dahl, L. Vandenberghe'
 
 # The default replacements for |version| and |release|, also used in various
 # other places throughout the built documents.
 #
 # The short X.Y version.
-version = '1.3.2.0'
+version = '1.3.2.1'
 # The full version, including alpha/beta/rc tags.
-release = '1.3.2.0'
+release = '1.3.2.1'
 
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
 #today = ''
 # Else, today_fmt is used as the format for a strftime call.
 today_fmt = '%B %d, %Y'
```

### Comparing `kvxopt-1.3.2.0/doc/source/copyright.rst` & `kvxopt-1.3.2.1/doc/source/copyright.rst`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/source/fftw.rst` & `kvxopt-1.3.2.1/doc/source/fftw.rst`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/source/floorplan.png` & `kvxopt-1.3.2.1/doc/source/floorplan.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/source/intro.rst` & `kvxopt-1.3.2.1/doc/source/intro.rst`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/source/lapack.rst` & `kvxopt-1.3.2.1/doc/source/lapack.rst`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/source/matrices.rst` & `kvxopt-1.3.2.1/doc/source/matrices.rst`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/source/modeling.rst` & `kvxopt-1.3.2.1/doc/source/modeling.rst`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/source/normappr.png` & `kvxopt-1.3.2.1/doc/source/normappr.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/source/portfolio1.png` & `kvxopt-1.3.2.1/doc/source/portfolio1.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/source/portfolio2.png` & `kvxopt-1.3.2.1/doc/source/portfolio2.png`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/source/printing.rst` & `kvxopt-1.3.2.1/doc/source/printing.rst`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/source/solvers.rst` & `kvxopt-1.3.2.1/doc/source/solvers.rst`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/doc/source/spsolvers.rst` & `kvxopt-1.3.2.1/doc/source/spsolvers.rst`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/book/chap4/portfolio.py` & `kvxopt-1.3.2.1/examples/book/chap4/portfolio.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/book/chap4/rls.bin` & `kvxopt-1.3.2.1/examples/book/chap4/rls.bin`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/book/chap4/rls.py` & `kvxopt-1.3.2.1/examples/book/chap4/rls.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/book/chap6/basispursuit.py` & `kvxopt-1.3.2.1/examples/book/chap6/basispursuit.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/book/chap6/consumerpref.py` & `kvxopt-1.3.2.1/examples/book/chap6/consumerpref.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/book/chap6/cvxfit.bin` & `kvxopt-1.3.2.1/examples/book/chap6/cvxfit.bin`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/book/chap6/cvxfit.py` & `kvxopt-1.3.2.1/examples/book/chap6/cvxfit.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/book/chap6/huber.bin` & `kvxopt-1.3.2.1/examples/book/chap6/huber.bin`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/book/chap6/huber.py` & `kvxopt-1.3.2.1/examples/book/chap6/huber.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/book/chap6/inputdesign.py` & `kvxopt-1.3.2.1/examples/book/chap6/inputdesign.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/book/chap6/penalties.py` & `kvxopt-1.3.2.1/examples/book/chap6/penalties.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/book/chap6/polapprox.bin` & `kvxopt-1.3.2.1/examples/book/chap6/polapprox.bin`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/book/chap6/polapprox.py` & `kvxopt-1.3.2.1/examples/book/chap6/polapprox.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/book/chap6/regsel.bin` & `kvxopt-1.3.2.1/examples/book/chap6/regsel.bin`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/book/chap6/regsel.py` & `kvxopt-1.3.2.1/examples/book/chap6/regsel.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/book/chap6/robls.bin` & `kvxopt-1.3.2.1/examples/book/chap6/robls.bin`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/book/chap6/robls.py` & `kvxopt-1.3.2.1/examples/book/chap6/robls.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/book/chap6/smoothrec.py` & `kvxopt-1.3.2.1/examples/book/chap6/smoothrec.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/book/chap6/tv.py` & `kvxopt-1.3.2.1/examples/book/chap6/tv.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/book/chap7/chernoff.py` & `kvxopt-1.3.2.1/examples/book/chap7/chernoff.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/book/chap7/expdesign.py` & `kvxopt-1.3.2.1/examples/book/chap7/expdesign.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/book/chap7/logreg.bin` & `kvxopt-1.3.2.1/examples/book/chap7/logreg.bin`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/book/chap7/logreg.py` & `kvxopt-1.3.2.1/examples/book/chap7/logreg.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/book/chap7/maxent.py` & `kvxopt-1.3.2.1/examples/book/chap7/maxent.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/book/chap7/probbounds.py` & `kvxopt-1.3.2.1/examples/book/chap7/probbounds.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/book/chap8/centers.py` & `kvxopt-1.3.2.1/examples/book/chap8/centers.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/book/chap8/ellipsoids.py` & `kvxopt-1.3.2.1/examples/book/chap8/ellipsoids.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/book/chap8/floorplan.py` & `kvxopt-1.3.2.1/examples/book/chap8/floorplan.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/book/chap8/linsep.bin` & `kvxopt-1.3.2.1/examples/book/chap8/linsep.bin`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/book/chap8/linsep.py` & `kvxopt-1.3.2.1/examples/book/chap8/linsep.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/book/chap8/placement.bin` & `kvxopt-1.3.2.1/examples/book/chap8/placement.bin`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/book/chap8/placement.py` & `kvxopt-1.3.2.1/examples/book/chap8/placement.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/doc/chap10/lp.py` & `kvxopt-1.3.2.1/examples/doc/chap10/lp.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/doc/chap10/normappr.py` & `kvxopt-1.3.2.1/examples/doc/chap10/normappr.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/doc/chap10/roblp.py` & `kvxopt-1.3.2.1/examples/doc/chap10/roblp.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/doc/chap4/acent.py` & `kvxopt-1.3.2.1/examples/doc/chap4/acent.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/doc/chap7/covsel.bin` & `kvxopt-1.3.2.1/examples/doc/chap7/covsel.bin`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/doc/chap7/covsel.py` & `kvxopt-1.3.2.1/examples/doc/chap7/covsel.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/doc/chap8/conelp.py` & `kvxopt-1.3.2.1/examples/doc/chap8/conelp.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/doc/chap8/coneqp.py` & `kvxopt-1.3.2.1/examples/doc/chap8/coneqp.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/doc/chap8/l1.py` & `kvxopt-1.3.2.1/examples/doc/chap8/l1.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/doc/chap8/l1regls.py` & `kvxopt-1.3.2.1/examples/doc/chap8/l1regls.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/doc/chap8/mcsdp.py` & `kvxopt-1.3.2.1/examples/doc/chap8/mcsdp.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/doc/chap8/portfolio.py` & `kvxopt-1.3.2.1/examples/doc/chap8/portfolio.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/doc/chap8/qcl1.py` & `kvxopt-1.3.2.1/examples/doc/chap8/qcl1.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/doc/chap8/sdp.py` & `kvxopt-1.3.2.1/examples/doc/chap8/sdp.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/doc/chap8/socp.py` & `kvxopt-1.3.2.1/examples/doc/chap8/socp.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/doc/chap9/acent.py` & `kvxopt-1.3.2.1/examples/doc/chap9/acent.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/doc/chap9/acent2.py` & `kvxopt-1.3.2.1/examples/doc/chap9/acent2.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/doc/chap9/floorplan.py` & `kvxopt-1.3.2.1/examples/doc/chap9/floorplan.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/doc/chap9/gp.py` & `kvxopt-1.3.2.1/examples/doc/chap9/gp.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/doc/chap9/l2ac.py` & `kvxopt-1.3.2.1/examples/doc/chap9/l2ac.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/doc/chap9/robls.py` & `kvxopt-1.3.2.1/examples/doc/chap9/robls.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/filterdemo/filterdemo_cli` & `kvxopt-1.3.2.1/examples/filterdemo/filterdemo_cli`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/examples/filterdemo/filterdemo_gui` & `kvxopt-1.3.2.1/examples/filterdemo/filterdemo_gui`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/kvxopt.egg-info/PKG-INFO` & `kvxopt-1.3.2.1/kvxopt.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: kvxopt
-Version: 1.3.2.0
+Version: 1.3.2.1
 Summary: Convex optimization package and Suite Sparse interface
 Home-page: UNKNOWN
 Author: M. Andersen, J. Dahl, L. Vandenberghe, and U. Sandoval
 Author-email: martin.skovgaard.andersen@gmail.com, dahl.joachim@gmail.com, vandenbe@ee.ucla.edu, sanurielf@gmail.com
 License: GNU GPL version 3
 Project-URL: Source, https://github.com/sanurielf/kvxopt
 Description:
```

### Comparing `kvxopt-1.3.2.0/kvxopt.egg-info/SOURCES.txt` & `kvxopt-1.3.2.1/kvxopt.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -502,22 +502,22 @@
 kvxopt.egg-info/not-zip-safe
 kvxopt.egg-info/top_level.txt
 src/C/amd.c
 src/C/base.c
 src/C/blas.c
 src/C/blas_redefines.h
 src/C/cholmod.c
-src/C/cvxopt.h
 src/C/dense.c
 src/C/dsdp.c
 src/C/fftw.c
 src/C/glpk.c
 src/C/gsl.c
 src/C/gurobi.c
 src/C/klu.c
+src/C/kvxopt.h
 src/C/lapack.c
 src/C/misc.h
 src/C/misc_solvers.c
 src/C/osqp.c
 src/C/sparse.c
 src/C/umfpack.c
 src/python/__init__.py
```

### Comparing `kvxopt-1.3.2.0/setup.py` & `kvxopt-1.3.2.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -163,15 +163,14 @@
 
 if sys.maxsize > 2**31:
     DLONG = True
 else:
     DLONG = False
 
 
-
 # Macros
 MACROS = []
 if BLAS_NOUNDERSCORES: MACROS.append(('BLAS_NO_UNDERSCORE',''))
 
 # optional modules
 
 if BUILD_GSL:
@@ -289,33 +288,78 @@
     sources = ['src/C/klu.c'])
 else:
 
     klu_sources = [ 'src/C/klu.c',
                   SUITESPARSE_SRC_DIR + '/SuiteSparse_config/SuiteSparse_config.c']
 
     if DLONG:
-        klu_sources += \
-            glob(SUITESPARSE_SRC_DIR + '/AMD/Source/*_l*.c') +\
-            glob(SUITESPARSE_SRC_DIR + '/BTF/Source/*_l_*.c') +\
-            [SUITESPARSE_SRC_DIR + '/COLAMD/Source/colamd_l.c'] +\
-            [SUITESPARSE_SRC_DIR + '/KLU/Source/klu_l.c'] +\
-            glob(SUITESPARSE_SRC_DIR + '/KLU/Source/klu_l*.c') +\
-            glob(SUITESPARSE_SRC_DIR + '/KLU/Source/klu_zl*.c')
+        klu_sources += (
+            glob(SUITESPARSE_SRC_DIR + "/AMD/Source/*_l*.c")
+            + glob(SUITESPARSE_SRC_DIR + "/BTF/Source/*_l_*.c")
+            + [SUITESPARSE_SRC_DIR + "/COLAMD/Source/colamd_l.c"]
+            + [
+                SUITESPARSE_SRC_DIR + "/KLU/Source/" + x + ".c"
+                for x in [
+                    "klu_l",
+                    "klu_zl",
+                    "klu_l_memory",
+                    "klu_l_analyze_given",
+                    "klu_l_scale",
+                    "klu_zl_scale",
+                    "klu_l_kernel",
+                    "klu_zl_kernel",
+                    "klu_zl_factor",
+                    "klu_zl_solve",
+                    "klu_l_free_numeric",
+                    "klu_zl_free_numeric",
+                    "klu_l_analyze",
+                    "klu_l_defaults",
+                    "klu_l_solve",
+                    "klu_l_factor",
+                    "klu_zl_extract",
+                    "klu_zl_tsolve",
+                    "klu_l_tsolve",
+                    "klu_l_free_symbolic",
+                    "klu_l_extract",
+                ]
+            ]
+        )
     else:
-        klu_sources += \
-            glob(SUITESPARSE_SRC_DIR + '/AMD/Source/*[!_l]*.c') +\
-            glob(SUITESPARSE_SRC_DIR + '/BTF/Source/*[!_l_]*.c') +\
-            [SUITESPARSE_SRC_DIR + '/COLAMD/Source/colamd.c'] +\
-            [SUITESPARSE_SRC_DIR + '/KLU/Source/klu.c'] +\
-            list(set(glob(SUITESPARSE_SRC_DIR + '/KLU/Source/klu_[!l]*.c')) &
-                 set(glob(SUITESPARSE_SRC_DIR + '/KLU/Source/klu_[!zl]*.c'))) +\
-            [SUITESPARSE_SRC_DIR + '/KLU/Source/klu_z.c'] +\
-            glob(SUITESPARSE_SRC_DIR + '/KLU/Source/klu_z_*.c')
+        klu_sources += (
+            glob(SUITESPARSE_SRC_DIR + "/AMD/Source/*[!_l]*.c")
+            + glob(SUITESPARSE_SRC_DIR + "/BTF/Source/*[!_l_]*.c")
+            + [SUITESPARSE_SRC_DIR + "/COLAMD/Source/colamd.c"]
+            + [
+                SUITESPARSE_SRC_DIR + "/KLU/Source/" + x + ".c"
+                for x in [
+                    "klu",
+                    "klu_z",
+                    "klu_memory",
+                    "klu_analyze_given",
+                    "klu_scale",
+                    "klu_z_scale",
+                    "klu_analyze",
+                    "klu_kernel",
+                    "klu_z_kernel",
+                    "klu_free_numeric",
+                    "klu_z_free_numeric",
+                    "klu_defaults",
+                    "klu_solve",
+                    "klu_tsolve",
+                    "klu_z_solve",
+                    "klu_z_tsolve",
+                    "klu_factor",
+                    "klu_z_factor",
+                    "klu_extract",
+                    "klu_z_extract",
+                    "klu_free_symbolic",
+                ]
+            ]
+        )
 
-    print(klu_sources)
     klu = Extension('klu',
         include_dirs = [ SUITESPARSE_SRC_DIR + '/KLU/Include',
             SUITESPARSE_SRC_DIR + '/KLU/Source',
             SUITESPARSE_SRC_DIR + '/AMD/Include',
             SUITESPARSE_SRC_DIR + '/AMD/Source',
             SUITESPARSE_SRC_DIR + '/COLAMD/Include',
             SUITESPARSE_SRC_DIR + '/COLAMD/Source',
@@ -335,17 +379,21 @@
 if not SUITESPARSE_SRC_DIR:
     cholmod = Extension('cholmod',
         libraries = ['cholmod','colamd','amd'] + SUITESPARSE_CONF_LIB + LAPACK_LIB + BLAS_LIB + RT_LIB,
         include_dirs = [SUITESPARSE_INC_DIR],
         library_dirs = [SUITESPARSE_LIB_DIR, BLAS_LIB_DIR],
         sources = [ 'src/C/cholmod.c' ])
 else:
-    cholmod_sources = [ 'src/C/cholmod.c' ] +\
-        [SUITESPARSE_SRC_DIR + '/SuiteSparse_config/SuiteSparse_config.c'] +\
-        [SUITESPARSE_SRC_DIR + '/CHOLMOD/Check/cholmod_check.c']
+    cholmod_sources = (
+        ["src/C/cholmod.c"]
+        + [SUITESPARSE_SRC_DIR + "/SuiteSparse_config/SuiteSparse_config.c"]
+        + glob(SUITESPARSE_SRC_DIR + "/CHOLMOD/Check/cholmod_*.c")
+        + glob(SUITESPARSE_SRC_DIR + "/CHOLMOD/Utility/cholmod_*.c")
+        + glob(SUITESPARSE_SRC_DIR + "/CHOLMOD/MatrixOps/cholmod_*.c")
+    )
 
     if DLONG:
         cholmod_sources += \
         [SUITESPARSE_SRC_DIR + '/AMD/Source/amd_l' + s for s in ['_postorder.c', '_post_tree.c', '2.c']] +\
         [SUITESPARSE_SRC_DIR + '/COLAMD/Source/colamd_l.c'] +\
         glob(SUITESPARSE_SRC_DIR + '/CHOLMOD/Core/cholmod_l_*.c') +\
         glob(SUITESPARSE_SRC_DIR + '/CHOLMOD/Cholesky/cholmod_l_*.c') +\
@@ -354,15 +402,14 @@
         cholmod_sources += \
         [SUITESPARSE_SRC_DIR + '/AMD/Source/amd_' + s for s in ['postorder.c', 'post_tree.c', '2.c']] +\
         [SUITESPARSE_SRC_DIR + '/COLAMD/Source/colamd.c'] +\
         glob(SUITESPARSE_SRC_DIR + '/CHOLMOD/Core/cholmod_[!l_]*.c') +\
         glob(SUITESPARSE_SRC_DIR + '/CHOLMOD/Cholesky/cholmod_[!l_]*.c') +\
         glob(SUITESPARSE_SRC_DIR + '/CHOLMOD/Supernodal/cholmod_[!l_]*.c')
 
-
     cholmod = Extension('cholmod',
         library_dirs = [ BLAS_LIB_DIR ],
         libraries = LAPACK_LIB + BLAS_LIB,
         include_dirs = [ SUITESPARSE_SRC_DIR + '/CHOLMOD/Include',
             SUITESPARSE_SRC_DIR + '/COLAMD',
             SUITESPARSE_SRC_DIR + '/AMD/Include',
             SUITESPARSE_SRC_DIR + '/COLAMD/Include',
```

### Comparing `kvxopt-1.3.2.0/src/C/amd.c` & `kvxopt-1.3.2.1/src/C/amd.c`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU General Public License
  * along with this program.  If not, see <http://www.gnu.org/licenses/>.
  */
 
-#include "cvxopt.h"
+#include "kvxopt.h"
 #include "amd.h"
 #include "misc.h"
 
 /* defined in pyconfig.h */
 #if (SIZEOF_INT < SIZEOF_SIZE_T)
 #define amd_order amd_l_order
 #define amd_defaults amd_l_defaults
```

### Comparing `kvxopt-1.3.2.0/src/C/base.c` & `kvxopt-1.3.2.1/src/C/base.c`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  * You should have received a copy of the GNU General Public License
  * along with this program.  If not, see <http://www.gnu.org/licenses/>.
  */
 
 #define BASE_MODULE
 
 #include "Python.h"
-#include "cvxopt.h"
+#include "kvxopt.h"
 #include "misc.h"
 
 #include <complexobject.h>
 
 PyDoc_STRVAR(base__doc__,"Convex optimization package");
 
 extern PyTypeObject matrix_tp ;
```

### Comparing `kvxopt-1.3.2.0/src/C/blas.c` & `kvxopt-1.3.2.1/src/C/blas.c`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU General Public License
  * along with this program.  If not, see <http://www.gnu.org/licenses/>.
  */
 
 #include "Python.h"
-#include "cvxopt.h"
+#include "kvxopt.h"
 #include "misc.h"
 
 #ifndef _MSC_VER
 typedef complex double complex_t;
 #else
 typedef _Dcomplex complex_t;
 #endif
```

### Comparing `kvxopt-1.3.2.0/src/C/blas_redefines.h` & `kvxopt-1.3.2.1/src/C/blas_redefines.h`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/src/C/cholmod.c` & `kvxopt-1.3.2.1/src/C/cholmod.c`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  *
  * You should have received a copy of the GNU General Public License
  * along with this program.  If not, see <http://www.gnu.org/licenses/>.
  */
 
 #define NO_ANSI99_COMPLEX
 
-#include "cvxopt.h"
+#include "kvxopt.h"
 #include "misc.h"
 #include "cholmod.h"
 #include "complex.h"
 
 #ifndef _MSC_VER
 typedef double complex complex_t;
 #else
```

### Comparing `kvxopt-1.3.2.0/src/C/cvxopt.h` & `kvxopt-1.3.2.1/src/C/kvxopt.h`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/src/C/dense.c` & `kvxopt-1.3.2.1/src/C/dense.c`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  * You should have received a copy of the GNU General Public License
  * along with this program.  If not, see <http://www.gnu.org/licenses/>.
  */
 
 #define BASE_MODULE
 
 #include "Python.h"
-#include "cvxopt.h"
+#include "kvxopt.h"
 #include "misc.h"
 #include <complexobject.h>
 #include <limits.h>
 
 /* prototyping and forward declarations */
 extern void (*axpy[])(int *, number *, void *, int *, void *, int *) ;
 extern void (*scal[])(int *, number *, void *, int *) ;
```

### Comparing `kvxopt-1.3.2.0/src/C/dsdp.c` & `kvxopt-1.3.2.1/src/C/dsdp.c`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU General Public License
  * along with this program.  If not, see <http://www.gnu.org/licenses/>.
  */
 
-#include "cvxopt.h"
+#include "kvxopt.h"
 #include "misc.h"
 #include "dsdp5.h"
 #include "math.h"
 
 PyDoc_STRVAR(dsdp__doc__,"Interface to DSDP version 5.8.\n\n"
     "Software for Semidefinite Programming.\n\n"
     "Three control parameters can be modified by making an entry in \n"
```

### Comparing `kvxopt-1.3.2.0/src/C/fftw.c` & `kvxopt-1.3.2.1/src/C/fftw.c`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU General Public License
  * along with this program.  If not, see <http://www.gnu.org/licenses/>.
  */
 
-#include "cvxopt.h"
+#include "kvxopt.h"
 #include "misc.h"
 #include <fftw3.h>
 
 #ifndef _MSC_VER
 typedef complex double complex_t;
 #else
 typedef _Dcomplex complex_t;
```

### Comparing `kvxopt-1.3.2.0/src/C/glpk.c` & `kvxopt-1.3.2.1/src/C/glpk.c`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU General Public License
  * along with this program.  If not, see <http://www.gnu.org/licenses/>.
  */
 
-#include "cvxopt.h"
+#include "kvxopt.h"
 #include "misc.h"
 #include <glpk.h>
 #include <float.h>
 #include <limits.h>
 
 PyDoc_STRVAR(glpk__doc__,
     "Interface to the simplex and mixed integer LP algorithms in GLPK.\n\n"
```

### Comparing `kvxopt-1.3.2.0/src/C/gsl.c` & `kvxopt-1.3.2.1/src/C/gsl.c`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU General Public License
  * along with this program.  If not, see <http://www.gnu.org/licenses/>.
  */
 
-#include "cvxopt.h"
+#include "kvxopt.h"
 
 #include <complex.h>
 
 #include "misc.h"
 
 #include <gsl/gsl_rng.h>
 #include <gsl/gsl_randist.h>
```

### Comparing `kvxopt-1.3.2.0/src/C/gurobi.c` & `kvxopt-1.3.2.1/src/C/gurobi.c`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
  * but WITHOUT ANY WARRANTY; without even the implied warranty of
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU General Public License
  * along with this program.  If not, see <http://www.gnu.org/licenses/>.
  */
-#include "cvxopt.h"
+#include "kvxopt.h"
 #include "gurobi_c.h"
 #include "misc.h"
 
 // Status codes from
 // https://www.gurobi.com/documentation/9.1/refman/optimization_status_codes.html#sec:StatusCodes
 const char *STATUS_CODES[] = {"",
                               "loaded",
```

### Comparing `kvxopt-1.3.2.0/src/C/klu.c` & `kvxopt-1.3.2.1/src/C/klu.c`

 * *Files 1% similar despite different names*

```diff
@@ -14,19 +14,18 @@
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU General Public License
  * along with this program.  If not, see <http://www.gnu.org/licenses/>.
  */
 
 
-#include "cvxopt.h"
+#include "kvxopt.h"
 #include "klu.h"
 #include "misc.h"
 
-
 // KLU functions and  types/structures
 #if (SIZEOF_INT < SIZEOF_SIZE_T)
 #define KLUD(name) klu_l_ ## name
 #define KLUZ(name) klu_zl_ ## name
 #define KLU(name) klu_l_ ## name
 #else
 #define KLUD(name) klu_ ## name
```

### Comparing `kvxopt-1.3.2.0/src/C/lapack.c` & `kvxopt-1.3.2.1/src/C/lapack.c`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU General Public License
  * along with this program.  If not, see <http://www.gnu.org/licenses/>.
  */
 
 #include "Python.h"
-#include "cvxopt.h"
+#include "kvxopt.h"
 #include "misc.h"
 
 #ifndef _MSC_VER
 typedef complex double complex_t;
 #else
 typedef _Dcomplex complex_t;
 #endif
```

### Comparing `kvxopt-1.3.2.0/src/C/misc.h` & `kvxopt-1.3.2.1/src/C/misc.h`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/src/C/misc_solvers.c` & `kvxopt-1.3.2.1/src/C/misc_solvers.c`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU General Public License
  * along with this program.  If not, see <http://www.gnu.org/licenses/>.
  */
 
 #include "Python.h"
-#include "cvxopt.h"
+#include "kvxopt.h"
 #include "misc.h"
 #include "math.h"
 #include "float.h"
 
 PyDoc_STRVAR(misc_solvers__doc__, "Miscellaneous functions used by the "
     "CVXOPT solvers.");
```

### Comparing `kvxopt-1.3.2.0/src/C/osqp.c` & `kvxopt-1.3.2.1/src/C/osqp.c`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  * You should have received a copy of the GNU General Public License
  * along with this program.  If not, see <http://www.gnu.org/licenses/>.
  */
 
 #include "osqp.h"
 
 #include "cs.h"
-#include "cvxopt.h"
+#include "kvxopt.h"
 #include "misc.h"
 
 #define xstr(s) str(s)
 #define str(s) #s
 
 #define IF_PARSE_FLOAT_OPT(opt_name, key, value)                             \
     if (!PYSTRING_COMPARE(key, str(opt_name))) {                             \
```

### Comparing `kvxopt-1.3.2.0/src/C/sparse.c` & `kvxopt-1.3.2.1/src/C/sparse.c`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  * You should have received a copy of the GNU General Public License
  * along with this program.  If not, see <http://www.gnu.org/licenses/>.
  */
 
 #define BASE_MODULE
 
 #include "Python.h"
-#include "cvxopt.h"
+#include "kvxopt.h"
 #include "misc.h"
 
 #include <complexobject.h>
 
 #define CONJ(flag, val) (flag == 'C' ? conj(val) : val)
 
 extern const int  E_SIZE[];
```

### Comparing `kvxopt-1.3.2.0/src/C/umfpack.c` & `kvxopt-1.3.2.1/src/C/umfpack.c`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU General Public License
  * along with this program.  If not, see <http://www.gnu.org/licenses/>.
  */
 
-#include "cvxopt.h"
+#include "kvxopt.h"
 #include "umfpack.h"
 #include "misc.h"
 
 #if (SIZEOF_INT < SIZEOF_SIZE_T)
 #define UMFD(name) umfpack_dl_ ## name
 #define UMFZ(name) umfpack_zl_ ## name
 #else
```

### Comparing `kvxopt-1.3.2.0/src/python/__init__.py` & `kvxopt-1.3.2.1/src/python/__init__.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/src/python/coneprog.py` & `kvxopt-1.3.2.1/src/python/coneprog.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/src/python/cvxprog.py` & `kvxopt-1.3.2.1/src/python/cvxprog.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/src/python/info.py` & `kvxopt-1.3.2.1/src/python/info.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/src/python/misc.py` & `kvxopt-1.3.2.1/src/python/misc.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/src/python/modeling.py` & `kvxopt-1.3.2.1/src/python/modeling.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/src/python/msk.py` & `kvxopt-1.3.2.1/src/python/msk.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/src/python/printing.py` & `kvxopt-1.3.2.1/src/python/printing.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/src/python/solvers.py` & `kvxopt-1.3.2.1/src/python/solvers.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/tests/ACTIVSg2000.mtx` & `kvxopt-1.3.2.1/tests/ACTIVSg2000.mtx`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/tests/bcsstk13.mtx` & `kvxopt-1.3.2.1/tests/bcsstk13.mtx`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/tests/bcsstk24.mtx` & `kvxopt-1.3.2.1/tests/bcsstk24.mtx`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/tests/boeing2.mps` & `kvxopt-1.3.2.1/tests/boeing2.mps`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/tests/bp_800.mtx` & `kvxopt-1.3.2.1/tests/bp_800.mtx`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/tests/test_basic.py` & `kvxopt-1.3.2.1/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/tests/test_blas.py` & `kvxopt-1.3.2.1/tests/test_blas.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/tests/test_custom_kkt.py` & `kvxopt-1.3.2.1/tests/test_custom_kkt.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/tests/test_dsdp.py` & `kvxopt-1.3.2.1/tests/test_dsdp.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/tests/test_examples.py` & `kvxopt-1.3.2.1/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/tests/test_glpk.py` & `kvxopt-1.3.2.1/tests/test_glpk.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/tests/test_gsl.py` & `kvxopt-1.3.2.1/tests/test_gsl.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/tests/test_gurobi.py` & `kvxopt-1.3.2.1/tests/test_gurobi.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/tests/test_modeling.py` & `kvxopt-1.3.2.1/tests/test_modeling.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/tests/test_mosek.py` & `kvxopt-1.3.2.1/tests/test_mosek.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/tests/test_osqp.py` & `kvxopt-1.3.2.1/tests/test_osqp.py`

 * *Files identical despite different names*

### Comparing `kvxopt-1.3.2.0/tests/test_sparse_solvers.py` & `kvxopt-1.3.2.1/tests/test_sparse_solvers.py`

 * *Files identical despite different names*

