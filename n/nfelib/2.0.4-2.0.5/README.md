# Comparing `tmp/nfelib-2.0.4.zip` & `tmp/nfelib-2.0.5.zip`

## zipinfo {}

```diff
@@ -1,783 +1,704 @@
-Zip file size: 1476153 bytes, number of entries: 781
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib.egg-info/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/tests/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/
--rw-rw-r--  2.0 unx     1074 b- defN 23-Jun-04 19:38 nfelib-2.0.4/MIT-LICENSE
--rw-rw-r--  2.0 unx       38 b- defN 23-Jun-29 01:20 nfelib-2.0.4/setup.py
--rw-rw-r--  2.0 unx     1451 b- defN 24-Mar-02 19:02 nfelib-2.0.4/setup.cfg
--rw-rw-r--  2.0 unx     6368 b- defN 24-Feb-24 11:12 nfelib-2.0.4/README.md
--rw-rw-r--  2.0 unx     7588 b- defN 24-Mar-02 19:02 nfelib-2.0.4/PKG-INFO
--rw-rw-r--  2.0 unx       64 b- defN 23-Jun-04 19:38 nfelib-2.0.4/MANIFEST.in
--rw-rw-r--  2.0 unx        7 b- defN 24-Mar-02 19:02 nfelib-2.0.4/nfelib.egg-info/top_level.txt
--rw-rw-r--  2.0 unx    33901 b- defN 24-Mar-02 19:02 nfelib-2.0.4/nfelib.egg-info/SOURCES.txt
--rw-rw-r--  2.0 unx       73 b- defN 24-Mar-02 19:02 nfelib-2.0.4/nfelib.egg-info/requires.txt
--rw-rw-r--  2.0 unx        1 b- defN 24-Mar-02 19:02 nfelib-2.0.4/nfelib.egg-info/dependency_links.txt
--rw-rw-r--  2.0 unx     7588 b- defN 24-Mar-02 19:02 nfelib-2.0.4/nfelib.egg-info/PKG-INFO
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/tests/nfse/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/tests/mdfe/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/tests/nfe_evento_cce/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/tests/cte/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/tests/cce/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/tests/nfe/
--rw-rw-r--  2.0 unx      453 b- defN 24-Jan-31 16:40 nfelib-2.0.4/tests/fingerprint_out.txt
--rwxrwxr-x  2.0 unx     2534 b- defN 24-Feb-24 11:12 nfelib-2.0.4/tests/test_fingerprint.py
--rw-rw-r--  2.0 unx    11598 b- defN 24-Feb-24 11:12 nfelib-2.0.4/tests/output_nfse.xml
--rw-rw-r--  2.0 unx      632 b- defN 24-Feb-24 11:12 nfelib-2.0.4/tests/output_nfse_pedRegEvento.xml
--rw-rw-r--  2.0 unx        0 b- defN 23-Jun-04 19:38 nfelib-2.0.4/tests/__init__.py
--rw-rw-r--  2.0 unx     1507 b- defN 24-Feb-24 11:12 nfelib-2.0.4/tests/output_nfse_dps.xml
--rw-rw-r--  2.0 unx     4370 b- defN 24-Feb-24 11:12 nfelib-2.0.4/tests/output_cte.xml
--rw-rw-r--  2.0 unx      453 b- defN 24-Feb-24 11:36 nfelib-2.0.4/tests/fingerprint.txt
--rw-rw-r--  2.0 unx     1230 b- defN 24-Feb-24 11:12 nfelib-2.0.4/tests/output.xml
--rw-rw-r--  2.0 unx     1207 b- defN 24-Feb-24 11:12 nfelib-2.0.4/tests/output_nfe_evento_cce.xml
--rw-rw-r--  2.0 unx      224 b- defN 24-Feb-24 11:12 nfelib-2.0.4/tests/output_mdfe.xml
--rw-rw-r--  2.0 unx      482 b- defN 24-Feb-24 11:12 nfelib-2.0.4/tests/output_nfe_inut.xml
--rw-rw-r--  2.0 unx    46226 b- defN 24-Feb-24 11:12 nfelib-2.0.4/tests/output_nfe_leiaute.xml
--rw-rw-r--  2.0 unx    41634 b- defN 24-Feb-24 11:12 nfelib-2.0.4/tests/input.xml
--rw-rw-r--  2.0 unx     2549 b- defN 23-Jul-08 23:32 nfelib-2.0.4/tests/test_all.py
--rw-rw-r--  2.0 unx     2608 b- defN 23-Jun-24 18:18 nfelib-2.0.4/tests/nfse/test_nfse.py
--rw-rw-r--  2.0 unx     1054 b- defN 23-Jun-24 18:18 nfelib-2.0.4/tests/mdfe/test_mdfe.py
--rw-rw-r--  2.0 unx     1102 b- defN 23-Jun-24 18:18 nfelib-2.0.4/tests/nfe_evento_cce/test_cce.py
--rw-rw-r--  2.0 unx     1049 b- defN 23-Jul-08 23:32 nfelib-2.0.4/tests/cte/test_cte.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/tests/cce/v1_00/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/tests/cce/v1_00/leiauteCCe/
--rw-rw-r--  2.0 unx     1128 b- defN 23-Jun-04 19:38 nfelib-2.0.4/tests/cce/v1_00/leiauteCCe/35180803102452000172550010000476051695511860-01-cce.xml
--rw-rw-r--  2.0 unx       23 b- defN 23-Jun-24 18:18 nfelib-2.0.4/tests/nfe/__init__.py
--rw-rw-r--  2.0 unx     4504 b- defN 23-Jul-08 23:32 nfelib-2.0.4/tests/nfe/test_nfe_legacy.py
--rw-rw-r--  2.0 unx     6289 b- defN 23-Jul-08 23:32 nfelib-2.0.4/tests/nfe/test_nfe.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfse/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/v4_00/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/mdfe/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe_evento_mde/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe_epec/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe_entrega/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe_dist_dfe/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe_evento_cancel/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/cte_dist_dfe/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/bpe/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/mdfe_dist_dfe/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe_evento_cce/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe_ator_interessado/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/cte/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe_evento_generico/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe_cons/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/odoo/
--rw-rw-r--  2.0 unx     3435 b- defN 24-Mar-02 18:59 nfelib-2.0.4/nfelib/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfse/samples/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfse/bindings/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfse/schemas/
--rw-rw-r--  2.0 unx       15 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfse/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfse/samples/v1_0/
--rw-rw-r--  2.0 unx     1344 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfse/samples/v1_0/ConsultarNFSeRPS-ped-sitnfserps.xml
--rw-rw-r--  2.0 unx     1344 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfse/samples/v1_0/GerarNFSeEnvio-env-loterps.xml
--rw-rw-r--  2.0 unx      728 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfse/samples/v1_0/CancelarNFSe-ped-cannfse.xml
--rw-rw-r--  2.0 unx    10940 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfse/samples/v1_0/ConsultarNFSeEnvio-ped-sitnfse.xml
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfse/bindings/v1_0/
--rw-rw-r--  2.0 unx       15 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfse/bindings/__init__.py
--rw-rw-r--  2.0 unx      374 b- defN 23-Jun-24 20:51 nfelib-2.0.4/nfelib/nfse/bindings/v1_0/ped_reg_evento_v1_00.py
--rw-rw-r--  2.0 unx     5796 b- defN 23-Jun-24 20:51 nfelib-2.0.4/nfelib/nfse/bindings/v1_0/__init__.py
--rw-rw-r--  2.0 unx    35465 b- defN 23-Jun-24 20:51 nfelib-2.0.4/nfelib/nfse/bindings/v1_0/tipos_eventos_v1_00.py
--rw-rw-r--  2.0 unx      354 b- defN 23-Jun-24 20:51 nfelib-2.0.4/nfelib/nfse/bindings/v1_0/nfse_v1_00.py
--rw-rw-r--  2.0 unx   101233 b- defN 23-Jun-24 20:51 nfelib-2.0.4/nfelib/nfse/bindings/v1_0/tipos_complexos_v1_00.py
--rw-rw-r--  2.0 unx      352 b- defN 23-Jun-24 20:51 nfelib-2.0.4/nfelib/nfse/bindings/v1_0/dps_v1_00.py
--rw-rw-r--  2.0 unx    16022 b- defN 23-Jun-24 20:51 nfelib-2.0.4/nfelib/nfse/bindings/v1_0/tipos_simples_v1_00.py
--rw-rw-r--  2.0 unx     6384 b- defN 23-Jun-24 20:51 nfelib-2.0.4/nfelib/nfse/bindings/v1_0/xmldsig_core_schema_v1_00.py
--rw-rw-r--  2.0 unx      356 b- defN 23-Jun-24 20:51 nfelib-2.0.4/nfelib/nfse/bindings/v1_0/evento_v1_00.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfse/schemas/v1_0/
--rw-rw-r--  2.0 unx    29312 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfse/schemas/v1_0/tiposEventos_v1.00.xsd
--rw-rw-r--  2.0 unx      648 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfse/schemas/v1_0/NFSe_v1.00.xsd
--rw-rw-r--  2.0 unx      752 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfse/schemas/v1_0/pedRegEvento_v1.00.xsd
--rw-rw-r--  2.0 unx    78115 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfse/schemas/v1_0/tiposComplexos_v1.00.xsd
--rw-rw-r--  2.0 unx      587 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfse/schemas/v1_0/DPS_v1.00.xsd
--rw-rw-r--  2.0 unx     3406 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfse/schemas/v1_0/xmldsig-core-schema_v1.00.xsd
--rw-rw-r--  2.0 unx    57965 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfse/schemas/v1_0/tiposSimples_v1.00.xsd
--rw-rw-r--  2.0 unx      743 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfse/schemas/v1_0/evento_v1.00.xsd
--rw-rw-r--  2.0 unx    88685 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/v4_00/retConsStatServ.py
--rw-rw-r--  2.0 unx  1859480 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/v4_00/retEnviNFe.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/v4_00/__init__.py
--rw-rw-r--  2.0 unx      280 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/v4_00/README.txt
--rw-rw-r--  2.0 unx   235328 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/v4_00/retEnvConfRecebto.py
--rw-rw-r--  2.0 unx   231041 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/v4_00/retEnvEvento.py
--rw-rw-r--  2.0 unx     2966 b- defN 23-Jun-24 20:57 nfelib-2.0.4/nfelib/v4_00/leiauteNFe_sub.py
--rw-rw-r--  2.0 unx   188157 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/v4_00/retInutNFe.py
--rw-rw-r--  2.0 unx   159793 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/v4_00/retConsCad.py
--rw-rw-r--  2.0 unx    80047 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/v4_00/distDFeInt.py
--rw-rw-r--  2.0 unx    79013 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/v4_00/retDistDFeInt.py
--rw-rw-r--  2.0 unx  1859541 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/v4_00/retConsReciNFe.py
--rw-rw-r--  2.0 unx   239970 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/v4_00/retEnvCCe.py
--rw-rw-r--  2.0 unx   237200 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/v4_00/retEnvEventoCancNFe.py
--rw-rw-r--  2.0 unx   289846 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/v4_00/retConsSitNFe.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/mdfe/samples/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/mdfe/bindings/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/mdfe/schemas/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/mdfe/odoo/
--rw-rw-r--  2.0 unx       15 b- defN 23-Jun-04 19:38 nfelib-2.0.4/nfelib/mdfe/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/mdfe/samples/v3_0/
--rw-rw-r--  2.0 unx      947 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/samples/v3_0/inclusaoDFe1101154119060611747300015058001000000001111700344401-ped-eve.xml
--rw-rw-r--  2.0 unx     1407 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/samples/v3_0/pagamentoOperacao1101103511031029073900013955001000000001105112804101-ped-eve.xml
--rw-rw-r--  2.0 unx     1816 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/samples/v3_0/PagamentoOperacaoMDFe_1101164120039999999999999958001000000999999999999901-ped-eve.xml
--rw-rw-r--  2.0 unx     3789 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/samples/v3_0/26999999999999999999999999999999999999999991-mdfe.xml
--rw-rw-r--  2.0 unx     2719 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/samples/v3_0/41190876676436000167580010000500001000437558-mdfe.xml
--rw-rw-r--  2.0 unx     2057 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/samples/v3_0/50170876063965000276580010000011311421039568-mdfe.xml
--rw-rw-r--  2.0 unx     3574 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/samples/v3_0/ComPagtoPIX_41210780568835000181580010402005751006005791-procMDFe.xml
--rw-rw-r--  2.0 unx      180 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/samples/v3_0/310000007934162-ped-rec.xml
--rw-rw-r--  2.0 unx      702 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/samples/v3_0/cancelameto1101103511031029073900013955001000000001105112804101-ped-eve.xml
--rw-rw-r--  2.0 unx      732 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/samples/v3_0/encerramento1101123511031029073900013955001000000001105112804101-ped-eve.xml
--rw-rw-r--  2.0 unx      739 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/samples/v3_0/inclusaocondutor31131223864838000129580000000000051003000003-ped-eve.xml
--rw-rw-r--  2.0 unx      226 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/samples/v3_0/01010101010-ped-cons-mdfe-naoenc.xml
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/
--rw-rw-r--  2.0 unx       15 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/bindings/__init__.py
--rw-rw-r--  2.0 unx      601 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/ret_cons_stat_serv_mdfe_v3_00.py
--rw-rw-r--  2.0 unx     6770 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/xmldsig_core_schema_v1_01.py
--rw-rw-r--  2.0 unx     5571 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/cons_stat_serv_tipos_basico_v3_00.py
--rw-rw-r--  2.0 unx     7084 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/__init__.py
--rw-rw-r--  2.0 unx      545 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/proc_evento_mdfe_v3_00.py
--rw-rw-r--  2.0 unx     6239 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/cons_sit_mdfe_tipos_basico_v3_00.py
--rw-rw-r--  2.0 unx     5995 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/mdfe_consulta_dfe_tipos_basico_v3_00.py
--rw-rw-r--  2.0 unx      552 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/ret_evento_mdfe_v3_00.py
--rw-rw-r--  2.0 unx     7833 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/leiaute_dist_mdfe_v3_00.py
--rw-rw-r--  2.0 unx      571 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/mdfe_consulta_dfe_v3_00.py
--rw-rw-r--  2.0 unx    11143 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/ev_pagto_oper_mdfe_v3_00.py
--rw-rw-r--  2.0 unx      505 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/ret_mdfe_v3_00.py
--rw-rw-r--  2.0 unx     1963 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/ev_inc_condutor_mdfe_v3_00.py
--rw-rw-r--  2.0 unx     3502 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/tipos_geral_mdfe_v3_00.py
--rw-rw-r--  2.0 unx      584 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/ret_cons_sit_mdfe_v3_00.py
--rw-rw-r--  2.0 unx      579 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/ret_cons_reci_mdfe_v3_00.py
--rw-rw-r--  2.0 unx      549 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/ret_envi_mdfe_v3_00.py
--rw-rw-r--  2.0 unx      546 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/envi_mdfe_v3_00.py
--rw-rw-r--  2.0 unx      580 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/cons_mdfe_nao_enc_v3_00.py
--rw-rw-r--  2.0 unx     5622 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/cons_mdfe_nao_enc_tipos_basico_v3_00.py
--rw-rw-r--  2.0 unx      519 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/ret_dist_mdfe_v3_00.py
--rw-rw-r--  2.0 unx      538 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/evento_mdfe_v3_00.py
--rw-rw-r--  2.0 unx    35874 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/mdfe_modal_rodoviario_v3_00.py
--rw-rw-r--  2.0 unx    14799 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/evento_mdfe_tipos_basico_v3_00.py
--rw-rw-r--  2.0 unx     1660 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/ev_canc_mdfe_v3_00.py
--rw-rw-r--  2.0 unx    10218 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/mdfe_modal_aquaviario_v3_00.py
--rw-rw-r--  2.0 unx      593 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/ret_cons_mdfe_nao_enc_v3_00.py
--rw-rw-r--  2.0 unx      584 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/ret_mdfe_consulta_dfe_v3_00.py
--rw-rw-r--  2.0 unx      531 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/dist_mdfe_v3_00.py
--rw-rw-r--  2.0 unx     4353 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/cons_reci_mdfe_tipos_basico_v3_00.py
--rw-rw-r--  2.0 unx     5673 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/mdfe_modal_ferroviario_v3_00.py
--rw-rw-r--  2.0 unx     3482 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/ev_inclusao_dfe_mdfe_v3_00.py
--rw-rw-r--  2.0 unx      571 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/cons_sit_mdfe_v3_00.py
--rw-rw-r--  2.0 unx   126107 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/mdfe_tipos_basico_v3_00.py
--rw-rw-r--  2.0 unx      493 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/mdfe_v3_00.py
--rw-rw-r--  2.0 unx     2307 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/ev_enc_mdfe_v3_00.py
--rw-rw-r--  2.0 unx     3231 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/mdfe_modal_aereo_v3_00.py
--rw-rw-r--  2.0 unx      556 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/cons_reci_mdfe_v3_00.py
--rw-rw-r--  2.0 unx     2310 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/proc_mdfe_v3_00.py
--rw-rw-r--  2.0 unx      583 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/cons_stat_serv_mdfe_v3_00.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/
--rw-rw-r--  2.0 unx     6549 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/consReciMDFeTiposBasico_v3.00.xsd
--rw-rw-r--  2.0 unx      614 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/retConsReciMDFe_v3.00.xsd
--rw-rw-r--  2.0 unx      623 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/retConsMDFeNaoEnc_v3.00.xsd
--rw-rw-r--  2.0 unx      620 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/consStatServMDFe_v3.00.xsd
--rw-rw-r--  2.0 unx     1935 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/evIncCondutorMDFe_v3.00.xsd
--rw-rw-r--  2.0 unx     4033 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/consStatServTiposBasico_v3.00.xsd
--rw-rw-r--  2.0 unx      673 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/retMDFe_v3.00.xsd
--rw-rw-r--  2.0 unx    36487 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/mdfeModalRodoviario_v3.00.xsd
--rw-rw-r--  2.0 unx     1564 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/evCancMDFe_v3.00.xsd
--rw-rw-r--  2.0 unx      592 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/distMDFe_v3.00.xsd
--rw-rw-r--  2.0 unx      614 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/retMDFeConsultaDFe_v3.00.xsd
--rw-rw-r--  2.0 unx     3479 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/mdfeModalAereo_v3.00.xsd
--rw-rw-r--  2.0 unx     5523 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/mdfeModalFerroviario_v3.00.xsd
--rw-rw-r--  2.0 unx      597 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/eventoMDFe_v3.00.xsd
--rw-rw-r--  2.0 unx      632 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/retConsStatServMDFe_v3.00.xsd
--rw-rw-r--  2.0 unx    10610 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/evPagtoOperMDFe_v3.00.xsd
--rw-rw-r--  2.0 unx      605 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/retEventoMDFe_v3.00.xsd
--rw-rw-r--  2.0 unx      597 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/consReciMDFe_v3.00.xsd
--rw-rw-r--  2.0 unx      561 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/mdfeConsultaDFe_v3.00.xsd
--rw-rw-r--  2.0 unx      571 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/consMDFeNaoEnc_v3.00.xsd
--rw-rw-r--  2.0 unx     1677 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/procMDFe_v3.00.xsd
--rw-rw-r--  2.0 unx      711 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/enviMDFe_v3.00.xsd
--rw-rw-r--  2.0 unx     3274 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/evInclusaoDFeMDFe_v3.00.xsd
--rw-rw-r--  2.0 unx    24229 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/tiposGeralMDFe_v3.00.xsd
--rw-rw-r--  2.0 unx     3958 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/mdfeConsultaDFeTiposBasico_v3.00.xsd
--rw-rw-r--  2.0 unx    99783 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/mdfeTiposBasico_v3.00.xsd
--rw-rw-r--  2.0 unx    10365 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/mdfeModalAquaviario_v3.00.xsd
--rw-rw-r--  2.0 unx      561 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/mdfe_v3.00.xsd
--rw-rw-r--  2.0 unx      603 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/retEnviMDFe_v3.00.xsd
--rw-rw-r--  2.0 unx      569 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/consSitMDFe_v3.00.xsd
--rw-rw-r--  2.0 unx     4559 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/consSitMDFeTiposBasico_v3.00.xsd
--rw-rw-r--  2.0 unx      623 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/retConsMDFeNaoEnc_v1.00.xsd
--rw-rw-r--  2.0 unx     5554 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/leiauteDistMDFe_v3.00.xsd
--rw-rw-r--  2.0 unx     4309 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/consMDFeNaoEncTiposBasico_v3.00.xsd
--rw-rw-r--  2.0 unx     3749 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/xmldsig-core-schema_v1.01.xsd
--rw-rw-r--  2.0 unx    10018 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/eventoMDFeTiposBasico_v3.00.xsd
--rw-rw-r--  2.0 unx      587 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/procEventoMDFe_v3.00.xsd
--rw-rw-r--  2.0 unx      574 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/retDistMDFe_v3.00.xsd
--rw-rw-r--  2.0 unx      622 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/retConsSitMDFe_v3.00.xsd
--rw-rw-r--  2.0 unx     1967 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/evEncMDFe_v3.00.xsd
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/
--rw-rw-r--  2.0 unx       15 b- defN 23-Jul-08 21:39 nfelib-2.0.4/nfelib/mdfe/odoo/__init__.py
--rw-rw-r--  2.0 unx      374 b- defN 23-Jul-08 21:56 nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/ret_cons_stat_serv_mdfe_v3_00.py
--rw-rw-r--  2.0 unx     3260 b- defN 23-Jul-08 21:56 nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/cons_stat_serv_tipos_basico_v3_00.py
--rw-rw-r--  2.0 unx      366 b- defN 23-Jul-08 21:56 nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/proc_evento_mdfe_v3_00.py
--rw-rw-r--  2.0 unx     4056 b- defN 23-Jul-08 21:56 nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/cons_sit_mdfe_tipos_basico_v3_00.py
--rw-rw-r--  2.0 unx     4178 b- defN 23-Jul-08 21:56 nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/mdfe_consulta_dfe_tipos_basico_v3_00.py
--rw-rw-r--  2.0 unx      365 b- defN 23-Jul-08 21:56 nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/ret_evento_mdfe_v3_00.py
--rw-rw-r--  2.0 unx     5858 b- defN 23-Jul-08 21:56 nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/leiaute_dist_mdfe_v3_00.py
--rw-rw-r--  2.0 unx      377 b- defN 23-Jul-08 21:56 nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/mdfe_consulta_dfe_v3_00.py
--rw-rw-r--  2.0 unx     9050 b- defN 23-Jul-08 21:56 nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/ev_pagto_oper_mdfe_v3_00.py
--rw-rw-r--  2.0 unx      356 b- defN 23-Jul-08 21:56 nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/ret_mdfe_v3_00.py
--rw-rw-r--  2.0 unx     1628 b- defN 23-Jul-08 21:56 nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/ev_inc_condutor_mdfe_v3_00.py
--rw-rw-r--  2.0 unx     3223 b- defN 23-Jul-08 21:56 nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/tipos_geral_mdfe_v3_00.py
--rw-rw-r--  2.0 unx      372 b- defN 23-Jul-08 21:56 nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/ret_cons_sit_mdfe_v3_00.py
--rw-rw-r--  2.0 unx      374 b- defN 23-Jul-08 21:56 nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/ret_cons_reci_mdfe_v3_00.py
--rw-rw-r--  2.0 unx      360 b- defN 23-Jul-08 21:56 nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/ret_envi_mdfe_v3_00.py
--rw-rw-r--  2.0 unx      357 b- defN 23-Jul-08 21:56 nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/envi_mdfe_v3_00.py
--rw-rw-r--  2.0 unx      376 b- defN 23-Jul-08 21:56 nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/cons_mdfe_nao_enc_v3_00.py
--rw-rw-r--  2.0 unx     4002 b- defN 23-Jul-08 21:56 nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/cons_mdfe_nao_enc_tipos_basico_v3_00.py
--rw-rw-r--  2.0 unx      359 b- defN 23-Jul-08 21:56 nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/ret_dist_mdfe_v3_00.py
--rw-rw-r--  2.0 unx      362 b- defN 23-Jul-08 21:56 nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/evento_mdfe_v3_00.py
--rw-rw-r--  2.0 unx    27004 b- defN 23-Jul-08 21:56 nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/mdfe_modal_rodoviario_v3_00.py
--rw-rw-r--  2.0 unx     8297 b- defN 23-Jul-08 21:56 nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/evento_mdfe_tipos_basico_v3_00.py
--rw-rw-r--  2.0 unx     1346 b- defN 23-Jul-08 21:56 nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/ev_canc_mdfe_v3_00.py
--rw-rw-r--  2.0 unx     8086 b- defN 23-Jul-08 21:56 nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/mdfe_modal_aquaviario_v3_00.py
--rw-rw-r--  2.0 unx      379 b- defN 23-Jul-08 21:56 nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/ret_cons_mdfe_nao_enc_v3_00.py
--rw-rw-r--  2.0 unx      380 b- defN 23-Jul-08 21:56 nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/ret_mdfe_consulta_dfe_v3_00.py
--rw-rw-r--  2.0 unx      356 b- defN 23-Jul-08 21:56 nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/dist_mdfe_v3_00.py
--rw-rw-r--  2.0 unx     2884 b- defN 23-Jul-08 21:56 nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/cons_reci_mdfe_tipos_basico_v3_00.py
--rw-rw-r--  2.0 unx     3182 b- defN 23-Jul-08 21:56 nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/mdfe_modal_ferroviario_v3_00.py
--rw-rw-r--  2.0 unx     2669 b- defN 23-Jul-08 21:56 nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/ev_inclusao_dfe_mdfe_v3_00.py
--rw-rw-r--  2.0 unx      369 b- defN 23-Jul-08 21:56 nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/cons_sit_mdfe_v3_00.py
--rw-rw-r--  2.0 unx    70270 b- defN 23-Jul-08 21:56 nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/mdfe_tipos_basico_v3_00.py
--rw-rw-r--  2.0 unx      353 b- defN 23-Jul-08 21:56 nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/mdfe_v3_00.py
--rw-rw-r--  2.0 unx     1794 b- defN 23-Jul-08 21:56 nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/ev_enc_mdfe_v3_00.py
--rw-rw-r--  2.0 unx     1970 b- defN 23-Jul-08 21:56 nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/mdfe_modal_aereo_v3_00.py
--rw-rw-r--  2.0 unx      371 b- defN 23-Jul-08 21:56 nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/cons_reci_mdfe_v3_00.py
--rw-rw-r--  2.0 unx     1468 b- defN 23-Jul-08 21:56 nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/proc_mdfe_v3_00.py
--rw-rw-r--  2.0 unx      371 b- defN 23-Jul-08 21:56 nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/cons_stat_serv_mdfe_v3_00.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe_evento_mde/bindings/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe_evento_mde/schemas/
--rw-rw-r--  2.0 unx       15 b- defN 23-Jun-04 19:38 nfelib-2.0.4/nfelib/nfe_evento_mde/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe_evento_mde/bindings/v1_0/
--rw-rw-r--  2.0 unx       15 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_evento_mde/bindings/__init__.py
--rw-rw-r--  2.0 unx      561 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_evento_mde/bindings/v1_0/proc_conf_recebto_nfe_v1_00.py
--rw-rw-r--  2.0 unx     6770 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_evento_mde/bindings/v1_0/xmldsig_core_schema_v1_01.py
--rw-rw-r--  2.0 unx      309 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_evento_mde/bindings/v1_0/tipos_basico_v1_03.py
--rw-rw-r--  2.0 unx     1670 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_evento_mde/bindings/v1_0/__init__.py
--rw-rw-r--  2.0 unx     1578 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_evento_mde/bindings/v1_0/e210240_v1_00.py
--rw-rw-r--  2.0 unx    20302 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_evento_mde/bindings/v1_0/leiaute_conf_recebto_v1_00.py
--rw-rw-r--  2.0 unx      541 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_evento_mde/bindings/v1_0/conf_recebto_v1_00.py
--rw-rw-r--  2.0 unx      570 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_evento_mde/bindings/v1_0/ret_env_conf_recebto_v1_00.py
--rw-rw-r--  2.0 unx      570 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_evento_mde/bindings/v1_0/env_conf_recebto_v1_00.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe_evento_mde/schemas/v1_0/
--rw-rw-r--  2.0 unx    15624 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_evento_mde/schemas/v1_0/leiauteConfRecebto_v1.00.xsd
--rw-rw-r--  2.0 unx      598 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_evento_mde/schemas/v1_0/procConfRecebtoNFe_v1.00.xsd
--rw-rw-r--  2.0 unx     1767 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_evento_mde/schemas/v1_0/e210220_v1.00.xsd
--rw-rw-r--  2.0 unx     1269 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_evento_mde/schemas/v1_0/e210200_v1.00.xsd
--rw-rw-r--  2.0 unx     1755 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_evento_mde/schemas/v1_0/e210240_v1.00.xsd
--rw-rw-r--  2.0 unx      612 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_evento_mde/schemas/v1_0/envConfRecebto_v1.00.xsd
--rw-rw-r--  2.0 unx     1253 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_evento_mde/schemas/v1_0/e210210_v1.00.xsd
--rw-rw-r--  2.0 unx      586 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_evento_mde/schemas/v1_0/confRecebto_v1.00.xsd
--rw-rw-r--  2.0 unx    30140 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_evento_mde/schemas/v1_0/tiposBasico_v1.03.xsd
--rw-rw-r--  2.0 unx      603 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_evento_mde/schemas/v1_0/retEnvConfRecebto_v1.00.xsd
--rw-rw-r--  2.0 unx     3749 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_evento_mde/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe_epec/bindings/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe_epec/schemas/
--rw-rw-r--  2.0 unx       15 b- defN 23-Jun-04 19:38 nfelib-2.0.4/nfelib/nfe_epec/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe_epec/bindings/v1_0/
--rw-rw-r--  2.0 unx       15 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_epec/bindings/__init__.py
--rw-rw-r--  2.0 unx     1435 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_epec/bindings/v1_0/__init__.py
--rw-rw-r--  2.0 unx    10677 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_epec/bindings/v1_0/e110140_v1_00.py
--rw-rw-r--  2.0 unx    37803 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_epec/bindings/v1_0/leiaute_epec_v1_00.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe_epec/schemas/v1_0/
--rw-rw-r--  2.0 unx      585 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_epec/schemas/v1_0/EPEC_v1.00.xsd
--rw-rw-r--  2.0 unx     4475 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_epec/schemas/v1_0/e110140_v1.00.xsd
--rw-rw-r--  2.0 unx      608 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_epec/schemas/v1_0/envEPEC_v1.00.xsd
--rw-rw-r--  2.0 unx      601 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_epec/schemas/v1_0/procEPEC_v1.00.xsd
--rw-rw-r--  2.0 unx    17318 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_epec/schemas/v1_0/leiauteEPEC_v1.00.xsd
--rw-rw-r--  2.0 unx    30140 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_epec/schemas/v1_0/tiposBasico_v1.03.xsd
--rw-rw-r--  2.0 unx     3749 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_epec/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
--rw-rw-r--  2.0 unx      601 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_epec/schemas/v1_0/retEnvEPEC_v1.00.xsd
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe_entrega/bindings/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe_entrega/schemas/
--rw-rw-r--  2.0 unx       15 b- defN 23-Jun-04 19:38 nfelib-2.0.4/nfelib/nfe_entrega/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe_entrega/bindings/v1_0/
--rw-rw-r--  2.0 unx       15 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_entrega/bindings/__init__.py
--rw-rw-r--  2.0 unx     6770 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_entrega/bindings/v1_0/xmldsig_core_schema_v1_01.py
--rw-rw-r--  2.0 unx     1012 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_entrega/bindings/v1_0/tipos_basico_v1_03.py
--rw-rw-r--  2.0 unx     1782 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_entrega/bindings/v1_0/__init__.py
--rw-rw-r--  2.0 unx      549 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_entrega/bindings/v1_0/evento_entrega_nfe_v1_00.py
--rw-rw-r--  2.0 unx      565 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_entrega/bindings/v1_0/proc_evento_entrega_nfe_v1_00.py
--rw-rw-r--  2.0 unx      577 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_entrega/bindings/v1_0/ret_evento_entrega_nfe_v1_00.py
--rw-rw-r--  2.0 unx    17661 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_entrega/bindings/v1_0/leiaute_evento_entrega_nfe_v1_00.py
--rw-rw-r--  2.0 unx      581 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_entrega/bindings/v1_0/env_evento_entrega_nfe_v1_00.py
--rw-rw-r--  2.0 unx     5351 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_entrega/bindings/v1_0/e110130_v1_00.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe_entrega/schemas/v1_0/
--rw-rw-r--  2.0 unx      744 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_entrega/schemas/v1_0/envEventoCancEntregaNFe_v1.00.xsd
--rw-rw-r--  2.0 unx      601 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_entrega/schemas/v1_0/procEventoEntregaNFe_v1.00.xsd
--rw-rw-r--  2.0 unx      615 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_entrega/schemas/v1_0/EventoCancEntregaNFe_v1.00.xsd
--rw-rw-r--  2.0 unx      616 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_entrega/schemas/v1_0/retEventoCancEntregaNFe_v1.00.xsd
--rw-rw-r--  2.0 unx      596 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_entrega/schemas/v1_0/EventoEntregaNFe_v1.00.xsd
--rw-rw-r--  2.0 unx     4424 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_entrega/schemas/v1_0/e110130_v1.00.xsd
--rw-rw-r--  2.0 unx    11920 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_entrega/schemas/v1_0/leiauteEventoCancEntregaNFe_v1.00.xsd
--rw-rw-r--  2.0 unx    12382 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_entrega/schemas/v1_0/leiauteEventoEntregaNFe_v1.00.xsd
--rw-rw-r--  2.0 unx      724 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_entrega/schemas/v1_0/envEventoEntregaNFe_v1.00.xsd
--rw-rw-r--  2.0 unx    32624 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_entrega/schemas/v1_0/tiposBasico_v1.03.xsd
--rw-rw-r--  2.0 unx      612 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_entrega/schemas/v1_0/retEventoEntregaNFe_v1.00.xsd
--rw-rw-r--  2.0 unx     3749 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_entrega/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
--rw-rw-r--  2.0 unx     2191 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_entrega/schemas/v1_0/e110131_v1.00.xsd
--rw-rw-r--  2.0 unx      634 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_entrega/schemas/v1_0/procEventoCancEntregaNFe_v1.00.xsd
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe_dist_dfe/bindings/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe_dist_dfe/schemas/
--rw-rw-r--  2.0 unx       15 b- defN 23-Jun-04 19:38 nfelib-2.0.4/nfelib/nfe_dist_dfe/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe_dist_dfe/bindings/v1_0/
--rw-rw-r--  2.0 unx       15 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_dist_dfe/bindings/__init__.py
--rw-rw-r--  2.0 unx     4873 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_dist_dfe/bindings/v1_0/res_evento_v1_01.py
--rw-rw-r--  2.0 unx     6770 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_dist_dfe/bindings/v1_0/xmldsig_core_schema_v1_01.py
--rw-rw-r--  2.0 unx     1375 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_dist_dfe/bindings/v1_0/__init__.py
--rw-rw-r--  2.0 unx     5501 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_dist_dfe/bindings/v1_0/ret_dist_dfe_int_v1_01.py
--rw-rw-r--  2.0 unx     5290 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_dist_dfe/bindings/v1_0/res_nfe_v1_01.py
--rw-rw-r--  2.0 unx     4141 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_dist_dfe/bindings/v1_0/dist_dfe_int_v1_01.py
--rw-rw-r--  2.0 unx     1770 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_dist_dfe/bindings/v1_0/tipos_dist_dfe_v1_01.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe_dist_dfe/schemas/v1_0/
--rw-rw-r--  2.0 unx     4407 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_dist_dfe/schemas/v1_0/retDistDFeInt_v1.01.xsd
--rw-rw-r--  2.0 unx     8230 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_dist_dfe/schemas/v1_0/tiposDistDFe_v1.01.xsd
--rw-rw-r--  2.0 unx     4034 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_dist_dfe/schemas/v1_0/distDFeInt_v1.01.xsd
--rw-rw-r--  2.0 unx     4495 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_dist_dfe/schemas/v1_0/resEvento_v1.01.xsd
--rw-rw-r--  2.0 unx     4933 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_dist_dfe/schemas/v1_0/resNFe_v1.01.xsd
--rw-rw-r--  2.0 unx     3747 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_dist_dfe/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe_evento_cancel/bindings/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe_evento_cancel/schemas/
--rw-rw-r--  2.0 unx       15 b- defN 23-Jun-04 19:38 nfelib-2.0.4/nfelib/nfe_evento_cancel/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe_evento_cancel/bindings/v1_0/
--rw-rw-r--  2.0 unx       15 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_evento_cancel/bindings/__init__.py
--rw-rw-r--  2.0 unx     1954 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_evento_cancel/bindings/v1_0/e110111_v1_00.py
--rw-rw-r--  2.0 unx      560 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_evento_cancel/bindings/v1_0/ret_env_evento_canc_nfe_v1_00.py
--rw-rw-r--  2.0 unx     6770 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_evento_cancel/bindings/v1_0/xmldsig_core_schema_v1_01.py
--rw-rw-r--  2.0 unx     1012 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_evento_cancel/bindings/v1_0/tipos_basico_v1_03.py
--rw-rw-r--  2.0 unx     1773 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_evento_cancel/bindings/v1_0/__init__.py
--rw-rw-r--  2.0 unx      560 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_evento_cancel/bindings/v1_0/env_evento_canc_nfe_v1_00.py
--rw-rw-r--  2.0 unx      551 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_evento_cancel/bindings/v1_0/proc_evento_canc_nfe_v1_00.py
--rw-rw-r--  2.0 unx    20018 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_evento_cancel/bindings/v1_0/leiaute_evento_canc_nfe_v1_00.py
--rw-rw-r--  2.0 unx      531 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_evento_cancel/bindings/v1_0/evento_canc_nfe_v1_00.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe_evento_cancel/schemas/v1_0/
--rw-rw-r--  2.0 unx      595 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_evento_cancel/schemas/v1_0/envEventoCancNFe_v1.00.xsd
--rw-rw-r--  2.0 unx      572 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_evento_cancel/schemas/v1_0/eventoCancNFe_v1.00.xsd
--rw-rw-r--  2.0 unx    13952 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_evento_cancel/schemas/v1_0/leiauteEventoCancNFe_v1.00.xsd
--rw-rw-r--  2.0 unx     1770 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_evento_cancel/schemas/v1_0/e110111_v1.00.xsd
--rw-rw-r--  2.0 unx      581 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_evento_cancel/schemas/v1_0/procEventoCancNFe_v1.00.xsd
--rw-rw-r--  2.0 unx      589 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_evento_cancel/schemas/v1_0/retEnvEventoCancNFe_v1.00.xsd
--rw-rw-r--  2.0 unx    32400 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_evento_cancel/schemas/v1_0/tiposBasico_v1.03.xsd
--rw-rw-r--  2.0 unx     3749 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_evento_cancel/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/cte_dist_dfe/bindings/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/cte_dist_dfe/schemas/
--rw-rw-r--  2.0 unx       15 b- defN 23-Jun-04 19:38 nfelib-2.0.4/nfelib/cte_dist_dfe/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/cte_dist_dfe/bindings/v1_0/
--rw-rw-r--  2.0 unx       15 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/cte_dist_dfe/bindings/__init__.py
--rw-rw-r--  2.0 unx     3502 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/cte_dist_dfe/bindings/v1_0/dist_dfe_int_v1_00.py
--rw-rw-r--  2.0 unx     6770 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/cte_dist_dfe/bindings/v1_0/xmldsig_core_schema_v1_01.py
--rw-rw-r--  2.0 unx     1002 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/cte_dist_dfe/bindings/v1_0/__init__.py
--rw-rw-r--  2.0 unx     1067 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/cte_dist_dfe/bindings/v1_0/tipos_dist_dfe_v1_00.py
--rw-rw-r--  2.0 unx     5420 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/cte_dist_dfe/bindings/v1_0/ret_dist_dfe_int_v1_00.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/cte_dist_dfe/schemas/v1_0/
--rw-rw-r--  2.0 unx     3407 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/cte_dist_dfe/schemas/v1_0/distDFeInt_v1.00.xsd
--rw-rw-r--  2.0 unx     4283 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/cte_dist_dfe/schemas/v1_0/retDistDFeInt_v1.00.xsd
--rw-rw-r--  2.0 unx     3747 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/cte_dist_dfe/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
--rw-rw-r--  2.0 unx     8554 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/cte_dist_dfe/schemas/v1_0/tiposDistDFe_v1.00.xsd
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/bpe/bindings/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/bpe/schemas/
--rw-rw-r--  2.0 unx       15 b- defN 23-Jun-04 19:38 nfelib-2.0.4/nfelib/bpe/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/bpe/bindings/v1_0/
--rw-rw-r--  2.0 unx       15 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/bpe/bindings/__init__.py
--rw-rw-r--  2.0 unx     4651 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/bpe/bindings/v1_0/cons_sit_bpe_tipos_basico_v1_00.py
--rw-rw-r--  2.0 unx     6770 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/bpe/bindings/v1_0/xmldsig_core_schema_v1_01.py
--rw-rw-r--  2.0 unx     4296 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/bpe/bindings/v1_0/__init__.py
--rw-rw-r--  2.0 unx     5551 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/bpe/bindings/v1_0/cons_stat_serv_bpe_tipos_basico_v1_00.py
--rw-rw-r--  2.0 unx     1588 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/bpe/bindings/v1_0/ev_nao_emb_bpe_v1_00.py
--rw-rw-r--  2.0 unx     1657 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/bpe/bindings/v1_0/ev_alteracao_poltrona_v1_00.py
--rw-rw-r--  2.0 unx      531 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/bpe/bindings/v1_0/evento_bpe_v1_00.py
--rw-rw-r--  2.0 unx     2681 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/bpe/bindings/v1_0/tipos_geral_bpe_v1_00.py
--rw-rw-r--  2.0 unx      505 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/bpe/bindings/v1_0/bpe_tm_v1_00.py
--rw-rw-r--  2.0 unx      529 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/bpe/bindings/v1_0/proc_evento_bpe_v1_00.py
--rw-rw-r--  2.0 unx      539 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/bpe/bindings/v1_0/ret_evento_bpe_v1_00.py
--rw-rw-r--  2.0 unx      581 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/bpe/bindings/v1_0/cons_stat_serv_bpe_v1_00.py
--rw-rw-r--  2.0 unx      472 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/bpe/bindings/v1_0/bpe_v1_00.py
--rw-rw-r--  2.0 unx      575 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/bpe/bindings/v1_0/ret_cons_sit_bpe_v1_00.py
--rw-rw-r--  2.0 unx      562 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/bpe/bindings/v1_0/cons_sit_bpe_v1_00.py
--rw-rw-r--  2.0 unx     2310 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/bpe/bindings/v1_0/proc_bpe_tm_v1_00.py
--rw-rw-r--  2.0 unx    13972 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/bpe/bindings/v1_0/evento_bpe_tipos_basico_v1_00.py
--rw-rw-r--  2.0 unx      497 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/bpe/bindings/v1_0/ret_bpe_v1_00.py
--rw-rw-r--  2.0 unx     1915 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/bpe/bindings/v1_0/ev_excesso_bagagem_v1_00.py
--rw-rw-r--  2.0 unx      599 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/bpe/bindings/v1_0/ret_cons_stat_serv_bpe_v1_00.py
--rw-rw-r--  2.0 unx     1542 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/bpe/bindings/v1_0/ev_canc_bpe_v1_00.py
--rw-rw-r--  2.0 unx     2295 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/bpe/bindings/v1_0/proc_bpe_v1_00.py
--rw-rw-r--  2.0 unx   131130 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/bpe/bindings/v1_0/bpe_tipos_basico_v1_00.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/bpe/schemas/v1_0/
--rw-rw-r--  2.0 unx      698 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/bpe/schemas/v1_0/eventoBPe_v1.00.xsd
--rw-rw-r--  2.0 unx      619 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/bpe/schemas/v1_0/consStatServBPe_v1.00.xsd
--rw-rw-r--  2.0 unx   107163 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/bpe/schemas/v1_0/bpeTiposBasico_v1.00.xsd
--rw-rw-r--  2.0 unx      594 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/bpe/schemas/v1_0/retEventoBPe_v1.00.xsd
--rw-rw-r--  2.0 unx    23114 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/bpe/schemas/v1_0/tiposGeralBPe_v1.00.xsd
--rw-rw-r--  2.0 unx     1411 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/bpe/schemas/v1_0/evCancBPe_v1.00.xsd
--rw-rw-r--  2.0 unx     1570 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/bpe/schemas/v1_0/evNaoEmbBPe_v1.00.xsd
--rw-rw-r--  2.0 unx      616 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/bpe/schemas/v1_0/retConsSitBPe_v1.00.xsd
--rw-rw-r--  2.0 unx      649 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/bpe/schemas/v1_0/bpe_v1.00.xsd
--rw-rw-r--  2.0 unx     2028 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/bpe/schemas/v1_0/evExcessoBagagem_v1.00.xsd
--rw-rw-r--  2.0 unx      562 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/bpe/schemas/v1_0/retBPe_v1.00.xsd
--rw-rw-r--  2.0 unx     9549 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/bpe/schemas/v1_0/eventoBPeTiposBasico_v1.00.xsd
--rw-rw-r--  2.0 unx     1668 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/bpe/schemas/v1_0/procBPe_v1.00.xsd
--rw-rw-r--  2.0 unx     1677 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/bpe/schemas/v1_0/procBPeTM_v1.00.xsd
--rw-rw-r--  2.0 unx      631 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/bpe/schemas/v1_0/retConsStatServBPe_v1.00.xsd
--rw-rw-r--  2.0 unx     1862 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/bpe/schemas/v1_0/evAlteracaoPoltrona_v1.00.xsd
--rw-rw-r--  2.0 unx     3270 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/bpe/schemas/v1_0/consSitBPeTiposBasico_v1.00.xsd
--rw-rw-r--  2.0 unx      678 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/bpe/schemas/v1_0/bpeTM_v1.00.xsd
--rw-rw-r--  2.0 unx     3749 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/bpe/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
--rw-rw-r--  2.0 unx      582 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/bpe/schemas/v1_0/procEventoBPe_v1.00.xsd
--rw-rw-r--  2.0 unx      563 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/bpe/schemas/v1_0/consSitBPe_v1.00.xsd
--rw-rw-r--  2.0 unx     4106 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/bpe/schemas/v1_0/consStatServBPeTiposBasico_v1.00.xsd
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/mdfe_dist_dfe/bindings/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/mdfe_dist_dfe/schemas/
--rw-rw-r--  2.0 unx       15 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe_dist_dfe/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/mdfe_dist_dfe/bindings/v1_0/
--rw-rw-r--  2.0 unx       15 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe_dist_dfe/bindings/__init__.py
--rw-rw-r--  2.0 unx     3279 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/mdfe_dist_dfe/bindings/v1_0/dist_dfe_int_v1_00.py
--rw-rw-r--  2.0 unx     6770 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/mdfe_dist_dfe/bindings/v1_0/xmldsig_core_schema_v1_01.py
--rw-rw-r--  2.0 unx     1028 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/mdfe_dist_dfe/bindings/v1_0/__init__.py
--rw-rw-r--  2.0 unx      352 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/mdfe_dist_dfe/bindings/v1_0/tipos_dist_dfe_v1_00.py
--rw-rw-r--  2.0 unx      310 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/mdfe_dist_dfe/bindings/v1_0/tipos_geral_mdfe_v1_00.py
--rw-rw-r--  2.0 unx     5453 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/mdfe_dist_dfe/bindings/v1_0/ret_dist_dfe_int_v1_00.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/mdfe_dist_dfe/schemas/v1_0/
--rw-rw-r--  2.0 unx    22419 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe_dist_dfe/schemas/v1_0/tiposGeralMDFe_v1.00.xsd
--rw-rw-r--  2.0 unx     2843 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe_dist_dfe/schemas/v1_0/distDFeInt_v1.00.xsd
--rw-rw-r--  2.0 unx     4248 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe_dist_dfe/schemas/v1_0/retDistDFeInt_v1.00.xsd
--rw-rw-r--  2.0 unx     3747 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe_dist_dfe/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
--rw-rw-r--  2.0 unx     6807 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/mdfe_dist_dfe/schemas/v1_0/tiposDistDFe_v1.00.xsd
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe_evento_cce/samples/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe_evento_cce/bindings/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe_evento_cce/schemas/
--rw-rw-r--  2.0 unx       15 b- defN 23-Jun-04 19:38 nfelib-2.0.4/nfelib/nfe_evento_cce/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe_evento_cce/samples/v1_0/
--rw-rw-r--  2.0 unx     1207 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_evento_cce/samples/v1_0/35180803102452000172550010000476051695511860-01-cce.xml
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe_evento_cce/bindings/v1_0/
--rw-rw-r--  2.0 unx       15 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_evento_cce/bindings/__init__.py
--rw-rw-r--  2.0 unx      514 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_evento_cce/bindings/v1_0/cce_v1_00.py
--rw-rw-r--  2.0 unx     6770 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_evento_cce/bindings/v1_0/xmldsig_core_schema_v1_01.py
--rw-rw-r--  2.0 unx      309 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_evento_cce/bindings/v1_0/tipos_basico_v1_03.py
--rw-rw-r--  2.0 unx     1705 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_evento_cce/bindings/v1_0/__init__.py
--rw-rw-r--  2.0 unx      541 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_evento_cce/bindings/v1_0/proc_cce_nfe_v1_00.py
--rw-rw-r--  2.0 unx    22394 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_evento_cce/bindings/v1_0/leiaute_cce_v1_00.py
--rw-rw-r--  2.0 unx     1850 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_evento_cce/bindings/v1_0/e110110_v1_00.py
--rw-rw-r--  2.0 unx      543 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_evento_cce/bindings/v1_0/ret_env_cce_v1_00.py
--rw-rw-r--  2.0 unx      543 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_evento_cce/bindings/v1_0/env_cce_v1_00.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe_evento_cce/schemas/v1_0/
--rw-rw-r--  2.0 unx    17276 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_evento_cce/schemas/v1_0/leiauteCCe_v1.00.xsd
--rw-rw-r--  2.0 unx      657 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_evento_cce/schemas/v1_0/CCe_v1.00.xsd
--rw-rw-r--  2.0 unx      627 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_evento_cce/schemas/v1_0/procCCeNFe_v1.00.xsd
--rw-rw-r--  2.0 unx     3340 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_evento_cce/schemas/v1_0/e110110_v1.00.xsd
--rw-rw-r--  2.0 unx      630 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_evento_cce/schemas/v1_0/envCCe_v1.00.xsd
--rw-rw-r--  2.0 unx    30140 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_evento_cce/schemas/v1_0/tiposBasico_v1.03.xsd
--rw-rw-r--  2.0 unx     3749 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_evento_cce/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
--rw-rw-r--  2.0 unx      627 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_evento_cce/schemas/v1_0/retEnvCCe_v1.00.xsd
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe_ator_interessado/bindings/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe_ator_interessado/schemas/
--rw-rw-r--  2.0 unx       15 b- defN 23-Jun-04 19:38 nfelib-2.0.4/nfelib/nfe_ator_interessado/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe_ator_interessado/bindings/v1_0/
--rw-rw-r--  2.0 unx       15 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_ator_interessado/bindings/__init__.py
--rw-rw-r--  2.0 unx     6770 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_ator_interessado/bindings/v1_0/xmldsig_core_schema_v1_01.py
--rw-rw-r--  2.0 unx     1657 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_ator_interessado/bindings/v1_0/tipos_basico_v1_03.py
--rw-rw-r--  2.0 unx     2035 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_ator_interessado/bindings/v1_0/__init__.py
--rw-rw-r--  2.0 unx      583 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_ator_interessado/bindings/v1_0/ret_env_evento_ator_interessado_v1_00.py
--rw-rw-r--  2.0 unx      573 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_ator_interessado/bindings/v1_0/proc_evento_ator_interessado_v1_00.py
--rw-rw-r--  2.0 unx     4481 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_ator_interessado/bindings/v1_0/mod_110150_v1_00.py
--rw-rw-r--  2.0 unx      557 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_ator_interessado/bindings/v1_0/evento_ator_interessado_v1_00.py
--rw-rw-r--  2.0 unx    21825 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_ator_interessado/bindings/v1_0/leiaute_evento_ator_interessado_v1_00.py
--rw-rw-r--  2.0 unx      586 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_ator_interessado/bindings/v1_0/env_evento_ator_interessado_v1_00.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe_ator_interessado/schemas/v1_0/
--rw-rw-r--  2.0 unx      609 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_ator_interessado/schemas/v1_0/retEnvEventoAtorInteressado_v1.00.xsd
--rw-rw-r--  2.0 unx      600 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_ator_interessado/schemas/v1_0/procEventoAtorInteressado_v1.00.xsd
--rw-rw-r--  2.0 unx     3942 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_ator_interessado/schemas/v1_0/110150_v1.00.xsd
--rw-rw-r--  2.0 unx    15700 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_ator_interessado/schemas/v1_0/leiauteEventoAtorInteressado_v1.00.xsd
--rw-rw-r--  2.0 unx      618 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_ator_interessado/schemas/v1_0/envEventoAtorInteressado_v1.00.xsd
--rw-rw-r--  2.0 unx      595 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_ator_interessado/schemas/v1_0/eventoAtorInteressado_v1.00.xsd
--rw-rw-r--  2.0 unx    31796 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_ator_interessado/schemas/v1_0/tiposBasico_v1.03.xsd
--rw-rw-r--  2.0 unx     3749 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_ator_interessado/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/cte/samples/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/cte/bindings/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/cte/schemas/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/cte/odoo/
--rw-rw-r--  2.0 unx       15 b- defN 23-Jun-04 19:38 nfelib-2.0.4/nfelib/cte/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/cte/samples/v4_0/
--rw-rw-r--  2.0 unx     3436 b- defN 23-Jul-08 23:32 nfelib-2.0.4/nfelib/cte/samples/v4_0/51160624686092000173570010000000031000000020-cte.XML
--rw-rw-r--  2.0 unx     1558 b- defN 23-Jul-08 23:32 nfelib-2.0.4/nfelib/cte/samples/v4_0/cce35150107565416000104570000000012301000012300-ped-eve.xml
--rw-rw-r--  2.0 unx    10117 b- defN 23-Jul-08 23:32 nfelib-2.0.4/nfelib/cte/samples/v4_0/35190602427026001207570040000522031000522035-cte-multimodal.xml
--rw-rw-r--  2.0 unx     3168 b- defN 23-Jul-08 23:32 nfelib-2.0.4/nfelib/cte/samples/v4_0/35170799999999999999670000000000261309301440-cte-of.xml
--rw-rw-r--  2.0 unx     4378 b- defN 23-Jul-09 00:10 nfelib-2.0.4/nfelib/cte/samples/v4_0/43120178408960000182570010000000041000000047-cte.xml
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/cte/bindings/v4_0/
--rw-rw-r--  2.0 unx       15 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/cte/bindings/__init__.py
--rw-rw-r--  2.0 unx     1770 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/cte/bindings/v4_0/ev_reg_multimodal_v4_00.py
--rw-rw-r--  2.0 unx      595 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/cte/bindings/v4_0/ret_cons_stat_serv_cte_v4_00.py
--rw-rw-r--  2.0 unx     3787 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/cte/bindings/v4_0/cte_multi_modal_v4_00.py
--rw-rw-r--  2.0 unx     6899 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/cte/bindings/v4_0/ev_epeccte_v4_00.py
--rw-rw-r--  2.0 unx     6770 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/cte/bindings/v4_0/xmldsig_core_schema_v1_01.py
--rw-rw-r--  2.0 unx     5860 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/cte/bindings/v4_0/cons_stat_serv_tipos_basico_v4_00.py
--rw-rw-r--  2.0 unx     8463 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/cte/bindings/v4_0/__init__.py
--rw-rw-r--  2.0 unx     2304 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/cte/bindings/v4_0/proc_gtve_v4_00.py
--rw-rw-r--  2.0 unx     5941 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/cte/bindings/v4_0/ev_iecte_v4_00.py
--rw-rw-r--  2.0 unx      565 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/cte/bindings/v4_0/ret_inut_cte_v4_00.py
--rw-rw-r--  2.0 unx     2295 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/cte/bindings/v4_0/proc_cte_v4_00.py
--rw-rw-r--  2.0 unx      535 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/cte/bindings/v4_0/proc_inut_cte_v4_00.py
--rw-rw-r--  2.0 unx     1662 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/cte/bindings/v4_0/ev_canc_prest_desacordo_v4_00.py
--rw-rw-r--  2.0 unx     4687 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/cte/bindings/v4_0/cte_modal_rodoviario_v4_00.py
--rw-rw-r--  2.0 unx      479 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/cte/bindings/v4_0/cte_v4_00.py
--rw-rw-r--  2.0 unx      575 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/cte/bindings/v4_0/ret_cons_sit_cte_v4_00.py
--rw-rw-r--  2.0 unx     6927 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/cte/bindings/v4_0/ev_cce_cte_v4_00.py
--rw-rw-r--  2.0 unx    18409 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/cte/bindings/v4_0/evento_cte_tipos_basico_v4_00.py
--rw-rw-r--  2.0 unx     4335 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/cte/bindings/v4_0/tipos_geral_cte_v4_00.py
--rw-rw-r--  2.0 unx     1541 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/cte/bindings/v4_0/ev_canc_cte_v4_00.py
--rw-rw-r--  2.0 unx      532 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/cte/bindings/v4_0/ret_gtve_v4_00.py
--rw-rw-r--  2.0 unx     7465 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/cte/bindings/v4_0/cte_modal_rodoviario_os_v4_00.py
--rw-rw-r--  2.0 unx      530 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/cte/bindings/v4_0/proc_evento_cte_v4_00.py
--rw-rw-r--  2.0 unx     8260 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/cte/bindings/v4_0/cte_modal_aquaviario_v4_00.py
--rw-rw-r--  2.0 unx    11301 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/cte/bindings/v4_0/ev_gtv_v4_00.py
--rw-rw-r--  2.0 unx     1781 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/cte/bindings/v4_0/cte_modal_dutoviario_v4_00.py
--rw-rw-r--  2.0 unx   345750 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/cte/bindings/v4_0/cte_tipos_basico_v4_00.py
--rw-rw-r--  2.0 unx      531 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/cte/bindings/v4_0/evento_cte_v4_00.py
--rw-rw-r--  2.0 unx      504 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/cte/bindings/v4_0/cte_os_v4_00.py
--rw-rw-r--  2.0 unx      539 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/cte/bindings/v4_0/ret_evento_cte_v4_00.py
--rw-rw-r--  2.0 unx     5480 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/cte/bindings/v4_0/ev_cecte_v4_00.py
--rw-rw-r--  2.0 unx      527 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/cte/bindings/v4_0/ret_cte_v4_00.py
--rw-rw-r--  2.0 unx      577 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/cte/bindings/v4_0/cons_stat_serv_cte_v4_00.py
--rw-rw-r--  2.0 unx      538 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/cte/bindings/v4_0/ret_cte_os_v4_00.py
--rw-rw-r--  2.0 unx     6179 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/cte/bindings/v4_0/cons_sit_cte_tipos_basico_v4_00.py
--rw-rw-r--  2.0 unx     1677 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/cte/bindings/v4_0/ev_canc_iecte_v4_00.py
--rw-rw-r--  2.0 unx      562 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/cte/bindings/v4_0/cons_sit_cte_v4_00.py
--rw-rw-r--  2.0 unx     1685 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/cte/bindings/v4_0/ev_canc_cecte_v4_00.py
--rw-rw-r--  2.0 unx      577 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/cte/bindings/v4_0/inut_cte_v4_00.py
--rw-rw-r--  2.0 unx    14186 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/cte/bindings/v4_0/inut_cte_tipos_basico_v4_00.py
--rw-rw-r--  2.0 unx     2314 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/cte/bindings/v4_0/proc_cte_os_v4_00.py
--rw-rw-r--  2.0 unx      476 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/cte/bindings/v4_0/gtve_v4_00.py
--rw-rw-r--  2.0 unx     8881 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/cte/bindings/v4_0/cte_modal_ferroviario_v4_00.py
--rw-rw-r--  2.0 unx    10486 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/cte/bindings/v4_0/cte_modal_aereo_v4_00.py
--rw-rw-r--  2.0 unx     1774 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/cte/bindings/v4_0/ev_prest_desacordo_v4_00.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/cte/schemas/v4_0/
--rw-rw-r--  2.0 unx     4259 b- defN 23-Feb-27 11:40 nfelib-2.0.4/nfelib/cte/schemas/v4_0/cteModalRodoviario_v4.00.xsd
--rw-rw-r--  2.0 unx   272180 b- defN 24-Feb-24 11:12 nfelib-2.0.4/nfelib/cte/schemas/v4_0/cteTiposBasico_v4.00.xsd
--rw-rw-r--  2.0 unx    10576 b- defN 23-Feb-27 11:40 nfelib-2.0.4/nfelib/cte/schemas/v4_0/evGTV_v4.00.xsd
--rw-rw-r--  2.0 unx      700 b- defN 23-Feb-27 11:40 nfelib-2.0.4/nfelib/cte/schemas/v4_0/retEventoCTe_v4.00.xsd
--rw-rw-r--  2.0 unx     8583 b- defN 23-Feb-27 11:40 nfelib-2.0.4/nfelib/cte/schemas/v4_0/cteModalFerroviario_v4.00.xsd
--rw-rw-r--  2.0 unx     6338 b- defN 23-Feb-27 11:40 nfelib-2.0.4/nfelib/cte/schemas/v4_0/evCCeCTe_v4.00.xsd
--rw-rw-r--  2.0 unx      698 b- defN 23-Feb-27 11:40 nfelib-2.0.4/nfelib/cte/schemas/v4_0/eventoCTe_v4.00.xsd
--rw-rw-r--  2.0 unx     2213 b- defN 23-Feb-27 11:40 nfelib-2.0.4/nfelib/cte/schemas/v4_0/evRegMultimodal_v4.00.xsd
--rw-rw-r--  2.0 unx      706 b- defN 23-Feb-27 11:40 nfelib-2.0.4/nfelib/cte/schemas/v4_0/retCTeOS_v4.00.xsd
--rw-rw-r--  2.0 unx      702 b- defN 23-Feb-27 11:40 nfelib-2.0.4/nfelib/cte/schemas/v4_0/retGTVe_v4.00.xsd
--rw-rw-r--  2.0 unx      699 b- defN 23-Feb-27 11:40 nfelib-2.0.4/nfelib/cte/schemas/v4_0/retCTe_v4.00.xsd
--rw-rw-r--  2.0 unx     2075 b- defN 23-Feb-27 11:40 nfelib-2.0.4/nfelib/cte/schemas/v4_0/evPrestDesacordo_v4.00.xsd
--rw-rw-r--  2.0 unx     9313 b- defN 23-Feb-27 11:40 nfelib-2.0.4/nfelib/cte/schemas/v4_0/inutCTeTiposBasico_v4.00.xsd
--rw-rw-r--  2.0 unx     5494 b- defN 23-Mar-09 13:51 nfelib-2.0.4/nfelib/cte/schemas/v4_0/evIECTe_v4.00.xsd
--rw-rw-r--  2.0 unx     1707 b- defN 23-Feb-27 09:00 nfelib-2.0.4/nfelib/cte/schemas/v4_0/evCancPrestDesacordo_v4.00.xsd
--rw-rw-r--  2.0 unx      734 b- defN 23-Feb-27 11:40 nfelib-2.0.4/nfelib/cte/schemas/v4_0/retConsStatServCTe_v4.00.xsd
--rw-rw-r--  2.0 unx     4469 b- defN 23-Feb-27 11:40 nfelib-2.0.4/nfelib/cte/schemas/v4_0/consStatServTiposBasico_v4.00.xsd
--rw-rw-r--  2.0 unx    11173 b- defN 23-Feb-27 11:40 nfelib-2.0.4/nfelib/cte/schemas/v4_0/cteModalAereo_v4.00.xsd
--rw-rw-r--  2.0 unx     1673 b- defN 23-Feb-27 11:40 nfelib-2.0.4/nfelib/cte/schemas/v4_0/procGTVe_v4.00.xsd
--rw-rw-r--  2.0 unx     6498 b- defN 23-Feb-27 11:40 nfelib-2.0.4/nfelib/cte/schemas/v4_0/evEPECCTe_v4.00.xsd
--rw-rw-r--  2.0 unx     8005 b- defN 23-Feb-27 11:40 nfelib-2.0.4/nfelib/cte/schemas/v4_0/cteModalRodoviarioOS_v4.00.xsd
--rw-rw-r--  2.0 unx     1348 b- defN 23-Feb-27 11:40 nfelib-2.0.4/nfelib/cte/schemas/v4_0/cteModalDutoviario_v4.00.xsd
--rw-rw-r--  2.0 unx    24294 b- defN 23-Feb-27 11:40 nfelib-2.0.4/nfelib/cte/schemas/v4_0/tiposGeralCTe_v4.00.xsd
--rw-rw-r--  2.0 unx      651 b- defN 23-Feb-27 11:40 nfelib-2.0.4/nfelib/cte/schemas/v4_0/GTVe_v4.00.xsd
--rw-rw-r--  2.0 unx     1648 b- defN 23-Mar-09 13:52 nfelib-2.0.4/nfelib/cte/schemas/v4_0/evCancIECTe_v4.00.xsd
--rw-rw-r--  2.0 unx     4015 b- defN 23-Feb-27 11:40 nfelib-2.0.4/nfelib/cte/schemas/v4_0/cteMultiModal_v4.00.xsd
--rw-rw-r--  2.0 unx      834 b- defN 23-Feb-27 11:40 nfelib-2.0.4/nfelib/cte/schemas/v4_0/retInutCTe_v4.00.xsd
--rw-rw-r--  2.0 unx      800 b- defN 23-Feb-27 11:40 nfelib-2.0.4/nfelib/cte/schemas/v4_0/procEventoCTe_v4.00.xsd
--rw-rw-r--  2.0 unx     4690 b- defN 23-Feb-27 11:40 nfelib-2.0.4/nfelib/cte/schemas/v4_0/evCECTe_v4.00.xsd
--rw-rw-r--  2.0 unx      741 b- defN 23-Feb-27 11:40 nfelib-2.0.4/nfelib/cte/schemas/v4_0/inutCTe_v4.00.xsd
--rw-rw-r--  2.0 unx    13190 b- defN 23-Apr-28 08:26 nfelib-2.0.4/nfelib/cte/schemas/v4_0/eventoCTeTiposBasico_v4.00.xsd
--rw-rw-r--  2.0 unx      677 b- defN 23-Feb-27 11:40 nfelib-2.0.4/nfelib/cte/schemas/v4_0/cteOS_v4.00.xsd
--rw-rw-r--  2.0 unx     4735 b- defN 23-Feb-27 11:40 nfelib-2.0.4/nfelib/cte/schemas/v4_0/consSitCTeTiposBasico_v4.00.xsd
--rw-rw-r--  2.0 unx      722 b- defN 23-Feb-27 11:40 nfelib-2.0.4/nfelib/cte/schemas/v4_0/consStatServCTe_v4.00.xsd
--rw-rw-r--  2.0 unx     1679 b- defN 23-Feb-27 11:40 nfelib-2.0.4/nfelib/cte/schemas/v4_0/procCTeOS_v4.00.xsd
--rw-rw-r--  2.0 unx      722 b- defN 23-Feb-27 11:40 nfelib-2.0.4/nfelib/cte/schemas/v4_0/retConsSitCTe_v4.00.xsd
--rw-rw-r--  2.0 unx      669 b- defN 23-Feb-27 11:40 nfelib-2.0.4/nfelib/cte/schemas/v4_0/consSitCTe_v4.00.xsd
--rw-rw-r--  2.0 unx     7868 b- defN 23-Feb-27 11:40 nfelib-2.0.4/nfelib/cte/schemas/v4_0/cteModalAquaviario_v4.00.xsd
--rw-rw-r--  2.0 unx      656 b- defN 23-Feb-27 11:40 nfelib-2.0.4/nfelib/cte/schemas/v4_0/cte_v4.00.xsd
--rw-rw-r--  2.0 unx      695 b- defN 23-Feb-27 11:40 nfelib-2.0.4/nfelib/cte/schemas/v4_0/procInutCTe_v4.00.xsd
--rw-rw-r--  2.0 unx     1668 b- defN 23-Feb-27 11:40 nfelib-2.0.4/nfelib/cte/schemas/v4_0/procCTe_v4.00.xsd
--rw-rw-r--  2.0 unx     1673 b- defN 23-Feb-27 11:40 nfelib-2.0.4/nfelib/cte/schemas/v4_0/evCancCECTe_v4.00.xsd
--rw-rw-r--  2.0 unx     1516 b- defN 23-Feb-27 11:40 nfelib-2.0.4/nfelib/cte/schemas/v4_0/evCancCTe_v4.00.xsd
--rw-rw-r--  2.0 unx     3749 b- defN 23-Feb-27 11:40 nfelib-2.0.4/nfelib/cte/schemas/v4_0/xmldsig-core-schema_v1.01.xsd
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/cte/odoo/v4_0/
--rw-rw-r--  2.0 unx       15 b- defN 23-Jul-08 23:52 nfelib-2.0.4/nfelib/cte/odoo/__init__.py
--rw-rw-r--  2.0 unx     1439 b- defN 23-Jul-09 20:20 nfelib-2.0.4/nfelib/cte/odoo/v4_0/ev_reg_multimodal_v4_00.py
--rw-rw-r--  2.0 unx      373 b- defN 23-Jul-09 20:20 nfelib-2.0.4/nfelib/cte/odoo/v4_0/ret_cons_stat_serv_cte_v4_00.py
--rw-rw-r--  2.0 unx     2810 b- defN 23-Jul-09 20:20 nfelib-2.0.4/nfelib/cte/odoo/v4_0/cte_multi_modal_v4_00.py
--rw-rw-r--  2.0 unx     5782 b- defN 23-Jul-09 20:20 nfelib-2.0.4/nfelib/cte/odoo/v4_0/ev_epeccte_v4_00.py
--rw-rw-r--  2.0 unx     3463 b- defN 23-Jul-09 20:20 nfelib-2.0.4/nfelib/cte/odoo/v4_0/cons_stat_serv_tipos_basico_v4_00.py
--rw-rw-r--  2.0 unx     1454 b- defN 23-Jul-09 20:20 nfelib-2.0.4/nfelib/cte/odoo/v4_0/proc_gtve_v4_00.py
--rw-rw-r--  2.0 unx     4679 b- defN 23-Jul-09 20:20 nfelib-2.0.4/nfelib/cte/odoo/v4_0/ev_iecte_v4_00.py
--rw-rw-r--  2.0 unx      362 b- defN 23-Jul-09 20:20 nfelib-2.0.4/nfelib/cte/odoo/v4_0/ret_inut_cte_v4_00.py
--rw-rw-r--  2.0 unx     1442 b- defN 23-Jul-09 20:20 nfelib-2.0.4/nfelib/cte/odoo/v4_0/proc_cte_v4_00.py
--rw-rw-r--  2.0 unx      363 b- defN 23-Jul-09 20:20 nfelib-2.0.4/nfelib/cte/odoo/v4_0/proc_inut_cte_v4_00.py
--rw-rw-r--  2.0 unx     1704 b- defN 23-Jul-09 20:20 nfelib-2.0.4/nfelib/cte/odoo/v4_0/ev_canc_prest_desacordo_v4_00.py
--rw-rw-r--  2.0 unx     2881 b- defN 23-Jul-09 20:20 nfelib-2.0.4/nfelib/cte/odoo/v4_0/cte_modal_rodoviario_v4_00.py
--rw-rw-r--  2.0 unx      350 b- defN 23-Jul-09 20:20 nfelib-2.0.4/nfelib/cte/odoo/v4_0/cte_v4_00.py
--rw-rw-r--  2.0 unx      369 b- defN 23-Jul-09 20:20 nfelib-2.0.4/nfelib/cte/odoo/v4_0/ret_cons_sit_cte_v4_00.py
--rw-rw-r--  2.0 unx     8089 b- defN 23-Jul-09 20:20 nfelib-2.0.4/nfelib/cte/odoo/v4_0/ev_cce_cte_v4_00.py
--rw-rw-r--  2.0 unx    10608 b- defN 23-Jul-09 20:20 nfelib-2.0.4/nfelib/cte/odoo/v4_0/evento_cte_tipos_basico_v4_00.py
--rw-rw-r--  2.0 unx     3886 b- defN 23-Jul-09 20:20 nfelib-2.0.4/nfelib/cte/odoo/v4_0/tipos_geral_cte_v4_00.py
--rw-rw-r--  2.0 unx     1123 b- defN 23-Jul-09 20:20 nfelib-2.0.4/nfelib/cte/odoo/v4_0/ev_canc_cte_v4_00.py
--rw-rw-r--  2.0 unx      354 b- defN 23-Jul-09 20:20 nfelib-2.0.4/nfelib/cte/odoo/v4_0/ret_gtve_v4_00.py
--rw-rw-r--  2.0 unx     5697 b- defN 23-Jul-09 20:20 nfelib-2.0.4/nfelib/cte/odoo/v4_0/cte_modal_rodoviario_os_v4_00.py
--rw-rw-r--  2.0 unx      364 b- defN 23-Jul-09 20:20 nfelib-2.0.4/nfelib/cte/odoo/v4_0/proc_evento_cte_v4_00.py
--rw-rw-r--  2.0 unx     6564 b- defN 23-Jul-09 20:20 nfelib-2.0.4/nfelib/cte/odoo/v4_0/cte_modal_aquaviario_v4_00.py
--rw-rw-r--  2.0 unx     7311 b- defN 23-Jul-09 20:20 nfelib-2.0.4/nfelib/cte/odoo/v4_0/ev_gtv_v4_00.py
--rw-rw-r--  2.0 unx      989 b- defN 23-Jul-09 20:20 nfelib-2.0.4/nfelib/cte/odoo/v4_0/cte_modal_dutoviario_v4_00.py
--rw-rw-r--  2.0 unx   165752 b- defN 23-Jul-09 20:20 nfelib-2.0.4/nfelib/cte/odoo/v4_0/cte_tipos_basico_v4_00.py
--rw-rw-r--  2.0 unx      360 b- defN 23-Jul-09 20:20 nfelib-2.0.4/nfelib/cte/odoo/v4_0/evento_cte_v4_00.py
--rw-rw-r--  2.0 unx      352 b- defN 23-Jul-09 20:20 nfelib-2.0.4/nfelib/cte/odoo/v4_0/cte_os_v4_00.py
--rw-rw-r--  2.0 unx      363 b- defN 23-Jul-09 20:20 nfelib-2.0.4/nfelib/cte/odoo/v4_0/ret_evento_cte_v4_00.py
--rw-rw-r--  2.0 unx     3946 b- defN 23-Jul-09 20:20 nfelib-2.0.4/nfelib/cte/odoo/v4_0/ev_cecte_v4_00.py
--rw-rw-r--  2.0 unx      353 b- defN 23-Jul-09 20:20 nfelib-2.0.4/nfelib/cte/odoo/v4_0/ret_cte_v4_00.py
--rw-rw-r--  2.0 unx      370 b- defN 23-Jul-09 20:20 nfelib-2.0.4/nfelib/cte/odoo/v4_0/cons_stat_serv_cte_v4_00.py
--rw-rw-r--  2.0 unx      355 b- defN 23-Jul-09 20:20 nfelib-2.0.4/nfelib/cte/odoo/v4_0/ret_cte_os_v4_00.py
--rw-rw-r--  2.0 unx     3787 b- defN 23-Jul-09 20:20 nfelib-2.0.4/nfelib/cte/odoo/v4_0/cons_sit_cte_tipos_basico_v4_00.py
--rw-rw-r--  2.0 unx     1536 b- defN 23-Jul-09 20:20 nfelib-2.0.4/nfelib/cte/odoo/v4_0/ev_canc_iecte_v4_00.py
--rw-rw-r--  2.0 unx      366 b- defN 23-Jul-09 20:20 nfelib-2.0.4/nfelib/cte/odoo/v4_0/cons_sit_cte_v4_00.py
--rw-rw-r--  2.0 unx     1550 b- defN 23-Jul-09 20:20 nfelib-2.0.4/nfelib/cte/odoo/v4_0/ev_canc_cecte_v4_00.py
--rw-rw-r--  2.0 unx      359 b- defN 23-Jul-09 20:20 nfelib-2.0.4/nfelib/cte/odoo/v4_0/inut_cte_v4_00.py
--rw-rw-r--  2.0 unx     7441 b- defN 23-Jul-09 20:20 nfelib-2.0.4/nfelib/cte/odoo/v4_0/inut_cte_tipos_basico_v4_00.py
--rw-rw-r--  2.0 unx     1492 b- defN 23-Jul-09 20:20 nfelib-2.0.4/nfelib/cte/odoo/v4_0/proc_cte_os_v4_00.py
--rw-rw-r--  2.0 unx      351 b- defN 23-Jul-09 20:20 nfelib-2.0.4/nfelib/cte/odoo/v4_0/gtve_v4_00.py
--rw-rw-r--  2.0 unx     5739 b- defN 23-Jul-09 20:20 nfelib-2.0.4/nfelib/cte/odoo/v4_0/cte_modal_ferroviario_v4_00.py
--rw-rw-r--  2.0 unx    11100 b- defN 23-Jul-09 20:20 nfelib-2.0.4/nfelib/cte/odoo/v4_0/cte_modal_aereo_v4_00.py
--rw-rw-r--  2.0 unx     1482 b- defN 23-Jul-09 20:20 nfelib-2.0.4/nfelib/cte/odoo/v4_0/ev_prest_desacordo_v4_00.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe_evento_generico/bindings/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe_evento_generico/schemas/
--rw-rw-r--  2.0 unx       15 b- defN 23-Jun-04 19:38 nfelib-2.0.4/nfelib/nfe_evento_generico/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe_evento_generico/bindings/v1_0/
--rw-rw-r--  2.0 unx       15 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_evento_generico/bindings/__init__.py
--rw-rw-r--  2.0 unx     6770 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_evento_generico/bindings/v1_0/xmldsig_core_schema_v1_01.py
--rw-rw-r--  2.0 unx      309 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_evento_generico/bindings/v1_0/tipos_basico_v1_03.py
--rw-rw-r--  2.0 unx     1346 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_evento_generico/bindings/v1_0/__init__.py
--rw-rw-r--  2.0 unx      540 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_evento_generico/bindings/v1_0/env_evento_v1_00.py
--rw-rw-r--  2.0 unx      540 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_evento_generico/bindings/v1_0/ret_env_evento_v1_00.py
--rw-rw-r--  2.0 unx      542 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_evento_generico/bindings/v1_0/proc_evento_nfe_v1_00.py
--rw-rw-r--  2.0 unx    19324 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_evento_generico/bindings/v1_0/leiaute_evento_v1_00.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe_evento_generico/schemas/v1_0/
--rw-rw-r--  2.0 unx      575 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_evento_generico/schemas/v1_0/envEvento_v1.00.xsd
--rw-rw-r--  2.0 unx    14282 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_evento_generico/schemas/v1_0/leiauteEvento_v1.00.xsd
--rw-rw-r--  2.0 unx      572 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_evento_generico/schemas/v1_0/procEventoNFe_v1.00.xsd
--rw-rw-r--  2.0 unx      569 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_evento_generico/schemas/v1_0/retEnvEvento_v1.00.xsd
--rw-rw-r--  2.0 unx    30140 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_evento_generico/schemas/v1_0/tiposBasico_v1.03.xsd
--rw-rw-r--  2.0 unx     3749 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_evento_generico/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe_cons/bindings/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe_cons/schemas/
--rw-rw-r--  2.0 unx       15 b- defN 23-Jun-04 19:38 nfelib-2.0.4/nfelib/nfe_cons/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe_cons/bindings/v2_0/
--rw-rw-r--  2.0 unx       15 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_cons/bindings/__init__.py
--rw-rw-r--  2.0 unx     6770 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_cons/bindings/v2_0/xmldsig_core_schema_v1_01.py
--rw-rw-r--  2.0 unx      934 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_cons/bindings/v2_0/tipos_basico_v1_03.py
--rw-rw-r--  2.0 unx     1504 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_cons/bindings/v2_0/__init__.py
--rw-rw-r--  2.0 unx      585 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_cons/bindings/v2_0/cons_sit_nfe_v2_01.py
--rw-rw-r--  2.0 unx    29843 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_cons/bindings/v2_0/leiaute_cons_sit_nfe_v2_01.py
--rw-rw-r--  2.0 unx      575 b- defN 24-Feb-24 11:36 nfelib-2.0.4/nfelib/nfe_cons/bindings/v2_0/ret_cons_sit_nfe_v2_01.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe_cons/schemas/v2_0/
--rw-rw-r--  2.0 unx      655 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_cons/schemas/v2_0/consSitNFe_v2.01.xsd
--rw-rw-r--  2.0 unx    22200 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_cons/schemas/v2_0/leiauteConsSitNFe_v2.01.xsd
--rw-rw-r--  2.0 unx    29554 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_cons/schemas/v2_0/tiposBasico_v1.03.xsd
--rw-rw-r--  2.0 unx     3749 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_cons/schemas/v2_0/xmldsig-core-schema_v1.01.xsd
--rw-rw-r--  2.0 unx      686 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe_cons/schemas/v2_0/retConsSitNFe_v2.01.xsd
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe/samples/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe/bindings/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe/ws/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe/schemas/
--rw-rw-r--  2.0 unx       15 b- defN 23-Jun-28 18:34 nfelib-2.0.4/nfelib/nfe/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe/samples/v4_0/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteNFe/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteInutNFe/
--rw-rw-r--  2.0 unx    10647 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476711079516696-nfe.xml
--rw-rw-r--  2.0 unx     7180 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteNFe/42220575277525000178550030000292481295366801-procNFe.xml
--rw-rw-r--  2.0 unx    37663 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000474491454651420-nfe.xml
--rw-rw-r--  2.0 unx    14538 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476051695511860-nfe.xml
--rw-rw-r--  2.0 unx    32177 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476491552806942-nfe.xml
--rw-rw-r--  2.0 unx     9218 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteNFe/41170706117473000150550010000463202612756525-procNFe.xml
--rw-rw-r--  2.0 unx    68825 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476861118934859-nfe.xml
--rw-rw-r--  2.0 unx    10834 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteNFe/42210775277525000178550030000266631762885493-procNFe.xml
--rw-rw-r--  2.0 unx     9301 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476781421693968-nfe.xml
--rw-rw-r--  2.0 unx    12034 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteNFe/42211275277525000178550030000276771368212013-procNFe.xml
--rw-rw-r--  2.0 unx    11802 b- defN 23-Nov-08 09:13 nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteNFe/26180875335849000115550010000016871192213331-nfe.xml
--rw-rw-r--  2.0 unx     9767 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476121675985748-nfe.xml
--rw-rw-r--  2.0 unx    46079 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000474501597356342-nfe.xml
--rw-rw-r--  2.0 unx     5549 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteNFe/NFe35200159594315000157550010000000012062777161.xml
--rw-rw-r--  2.0 unx    19459 b- defN 24-Jan-31 16:43 nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000474281920007498-nfe.xml
--rw-rw-r--  2.0 unx    46216 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000474641681223493-nfe.xml
--rw-rw-r--  2.0 unx      484 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteInutNFe/41080676472349000430550010000001041671821888-ped-inu.xml
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe/bindings/v4_0/
--rw-rw-r--  2.0 unx       15 b- defN 23-Jun-24 18:18 nfelib-2.0.4/nfelib/nfe/bindings/__init__.py
--rw-rw-r--  2.0 unx    30307 b- defN 24-Mar-02 18:56 nfelib-2.0.4/nfelib/nfe/bindings/v4_0/leiaute_cons_sit_nfe_v4_00.py
--rw-rw-r--  2.0 unx      561 b- defN 24-Mar-02 18:56 nfelib-2.0.4/nfelib/nfe/bindings/v4_0/ret_cons_sit_nfe_v4_00.py
--rw-rw-r--  2.0 unx      512 b- defN 24-Mar-02 18:56 nfelib-2.0.4/nfelib/nfe/bindings/v4_0/cons_cad_v2_00.py
--rw-rw-r--  2.0 unx     6770 b- defN 24-Mar-02 18:56 nfelib-2.0.4/nfelib/nfe/bindings/v4_0/xmldsig_core_schema_v1_01.py
--rw-rw-r--  2.0 unx     7598 b- defN 24-Mar-02 18:56 nfelib-2.0.4/nfelib/nfe/bindings/v4_0/__init__.py
--rw-rw-r--  2.0 unx      579 b- defN 24-Mar-02 18:56 nfelib-2.0.4/nfelib/nfe/bindings/v4_0/ret_inut_nfe_v4_00.py
--rw-rw-r--  2.0 unx      556 b- defN 24-Mar-02 18:56 nfelib-2.0.4/nfelib/nfe/bindings/v4_0/inut_nfe_v4_00.py
--rw-rw-r--  2.0 unx      459 b- defN 24-Mar-02 18:56 nfelib-2.0.4/nfelib/nfe/bindings/v4_0/nfe_v4_00.py
--rw-rw-r--  2.0 unx      567 b- defN 24-Mar-02 18:56 nfelib-2.0.4/nfelib/nfe/bindings/v4_0/cons_reci_nfe_v4_00.py
--rw-rw-r--  2.0 unx     2676 b- defN 24-Mar-02 18:56 nfelib-2.0.4/nfelib/nfe/bindings/v4_0/tipos_basico_v4_00.py
--rw-rw-r--  2.0 unx      576 b- defN 24-Mar-02 18:56 nfelib-2.0.4/nfelib/nfe/bindings/v4_0/ret_cons_stat_serv_v4_00.py
--rw-rw-r--  2.0 unx    16440 b- defN 24-Mar-02 18:56 nfelib-2.0.4/nfelib/nfe/bindings/v4_0/leiaute_consulta_cadastro_v2_00.py
--rw-rw-r--  2.0 unx      552 b- defN 24-Mar-02 18:56 nfelib-2.0.4/nfelib/nfe/bindings/v4_0/cons_stat_serv_v4_00.py
--rw-rw-r--  2.0 unx    13133 b- defN 24-Mar-02 18:56 nfelib-2.0.4/nfelib/nfe/bindings/v4_0/leiaute_inut_nfe_v4_00.py
--rw-rw-r--  2.0 unx      571 b- defN 24-Mar-02 18:56 nfelib-2.0.4/nfelib/nfe/bindings/v4_0/cons_sit_nfe_v4_00.py
--rw-rw-r--  2.0 unx      591 b- defN 24-Mar-02 18:56 nfelib-2.0.4/nfelib/nfe/bindings/v4_0/ret_cons_reci_nfe_v4_00.py
--rw-rw-r--  2.0 unx     5962 b- defN 24-Mar-02 18:56 nfelib-2.0.4/nfelib/nfe/bindings/v4_0/leiaute_cons_stat_serv_v4_00.py
--rw-rw-r--  2.0 unx      549 b- defN 24-Mar-02 18:56 nfelib-2.0.4/nfelib/nfe/bindings/v4_0/envi_nfe_v4_00.py
--rw-rw-r--  2.0 unx      467 b- defN 24-Mar-02 18:56 nfelib-2.0.4/nfelib/nfe/bindings/v4_0/proc_nfe_v4_00.py
--rw-rw-r--  2.0 unx      533 b- defN 24-Mar-02 18:56 nfelib-2.0.4/nfelib/nfe/bindings/v4_0/proc_inut_nfe_v4_00.py
--rw-rw-r--  2.0 unx      572 b- defN 24-Mar-02 18:56 nfelib-2.0.4/nfelib/nfe/bindings/v4_0/ret_envi_nfe_v4_00.py
--rw-rw-r--  2.0 unx   494616 b- defN 24-Mar-02 18:56 nfelib-2.0.4/nfelib/nfe/bindings/v4_0/leiaute_nfe_v4_00.py
--rw-rw-r--  2.0 unx      558 b- defN 24-Mar-02 18:56 nfelib-2.0.4/nfelib/nfe/bindings/v4_0/ret_cons_cad_v2_00.py
--rw-rw-r--  2.0 unx       26 b- defN 23-Jul-08 23:32 nfelib-2.0.4/nfelib/nfe/ws/__init__.py
--rw-rw-r--  2.0 unx     4498 b- defN 24-Jan-31 16:43 nfelib-2.0.4/nfelib/nfe/ws/edoc_legacy.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/nfe/schemas/v4_0/
--r--r--r--  2.0 unx     3902 b- defN 22-Jul-18 09:41 nfelib-2.0.4/nfelib/nfe/schemas/v4_0/leiauteConsStatServ_v4.00.xsd
--r--r--r--  2.0 unx      628 b- defN 22-Jul-18 09:41 nfelib-2.0.4/nfelib/nfe/schemas/v4_0/retConsReciNFe_v4.00.xsd
--r--r--r--  2.0 unx      595 b- defN 22-Jul-18 09:41 nfelib-2.0.4/nfelib/nfe/schemas/v4_0/consStatServ_v4.00.xsd
--r--r--r--  2.0 unx      522 b- defN 22-Jul-18 09:41 nfelib-2.0.4/nfelib/nfe/schemas/v4_0/procNFe_v4.00.xsd
--r--r--r--  2.0 unx      623 b- defN 22-Jul-18 09:41 nfelib-2.0.4/nfelib/nfe/schemas/v4_0/retInutNFe_v4.00.xsd
--r--r--r--  2.0 unx      579 b- defN 22-Jul-18 09:41 nfelib-2.0.4/nfelib/nfe/schemas/v4_0/procInutNFe_v4.00.xsd
--rw-rw-r--  2.0 unx      600 b- defN 24-Jan-31 18:37 nfelib-2.0.4/nfelib/nfe/schemas/v4_0/consCad_v2.00.xsd
--r--r--r--  2.0 unx    20000 b- defN 22-Jul-18 09:41 nfelib-2.0.4/nfelib/nfe/schemas/v4_0/leiauteConsSitNFe_v4.00.xsd
--r--r--r--  2.0 unx      522 b- defN 22-Jul-18 09:41 nfelib-2.0.4/nfelib/nfe/schemas/v4_0/nfe_v4.00.xsd
--rw-rw-r--  2.0 unx      606 b- defN 24-Jan-31 18:37 nfelib-2.0.4/nfelib/nfe/schemas/v4_0/retConsCad_v2.00.xsd
--r--r--r--  2.0 unx      610 b- defN 22-Jul-18 09:41 nfelib-2.0.4/nfelib/nfe/schemas/v4_0/consReciNFe_v4.00.xsd
--r--r--r--  2.0 unx     7801 b- defN 22-Jul-18 09:41 nfelib-2.0.4/nfelib/nfe/schemas/v4_0/leiauteInutNFe_v4.00.xsd
--r--r--r--  2.0 unx      600 b- defN 23-Jul-12 10:08 nfelib-2.0.4/nfelib/nfe/schemas/v4_0/enviNFe_v4.00.xsd
--r--r--r--  2.0 unx      606 b- defN 22-Jul-18 09:41 nfelib-2.0.4/nfelib/nfe/schemas/v4_0/inutNFe_v4.00.xsd
--rw-rw-r--  2.0 unx    15469 b- defN 24-Jan-31 18:37 nfelib-2.0.4/nfelib/nfe/schemas/v4_0/leiauteConsultaCadastro_v2.00.xsd
--r--r--r--  2.0 unx      617 b- defN 22-Jul-18 09:41 nfelib-2.0.4/nfelib/nfe/schemas/v4_0/retEnviNFe_v4.00.xsd
--r--r--r--  2.0 unx      568 b- defN 22-Jul-18 09:41 nfelib-2.0.4/nfelib/nfe/schemas/v4_0/consSitNFe_v4.00.xsd
--r--r--r--  2.0 unx    21976 b- defN 23-Mar-29 13:44 nfelib-2.0.4/nfelib/nfe/schemas/v4_0/tiposBasico_v4.00.xsd
--rw-rw-r--  2.0 unx   334026 b- defN 24-Mar-02 18:56 nfelib-2.0.4/nfelib/nfe/schemas/v4_0/leiauteNFe_v4.00.xsd
--r--r--r--  2.0 unx      604 b- defN 22-Jul-18 09:41 nfelib-2.0.4/nfelib/nfe/schemas/v4_0/retConsStatServ_v4.00.xsd
--rw-rw-r--  2.0 unx    32310 b- defN 24-Jan-31 18:37 nfelib-2.0.4/nfelib/nfe/schemas/v4_0/tiposBasico_v1.03.xsd
--r--r--r--  2.0 unx      602 b- defN 22-Jul-18 09:41 nfelib-2.0.4/nfelib/nfe/schemas/v4_0/retConsSitNFe_v4.00.xsd
--r--r--r--  2.0 unx     3747 b- defN 23-Jul-12 10:08 nfelib-2.0.4/nfelib/nfe/schemas/v4_0/xmldsig-core-schema_v1.01.xsd
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/odoo/nfe/
--rw-rw-r--  2.0 unx       15 b- defN 23-Aug-26 00:40 nfelib-2.0.4/nfelib/odoo/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 24-Mar-02 19:02 nfelib-2.0.4/nfelib/odoo/nfe/v4_0/
--rw-rw-r--  2.0 unx       15 b- defN 24-Mar-02 18:56 nfelib-2.0.4/nfelib/odoo/nfe/__init__.py
--rw-rw-r--  2.0 unx    17607 b- defN 24-Mar-02 18:56 nfelib-2.0.4/nfelib/odoo/nfe/v4_0/leiaute_cons_sit_nfe_v4_00.py
--rw-rw-r--  2.0 unx      364 b- defN 24-Mar-02 18:56 nfelib-2.0.4/nfelib/odoo/nfe/v4_0/ret_cons_sit_nfe_v4_00.py
--rw-rw-r--  2.0 unx      363 b- defN 24-Mar-02 18:56 nfelib-2.0.4/nfelib/odoo/nfe/v4_0/cons_cad_v2_00.py
--rw-rw-r--  2.0 unx      357 b- defN 24-Mar-02 18:56 nfelib-2.0.4/nfelib/odoo/nfe/v4_0/ret_inut_nfe_v4_00.py
--rw-rw-r--  2.0 unx      354 b- defN 24-Mar-02 18:56 nfelib-2.0.4/nfelib/odoo/nfe/v4_0/inut_nfe_v4_00.py
--rw-rw-r--  2.0 unx      345 b- defN 24-Mar-02 18:56 nfelib-2.0.4/nfelib/odoo/nfe/v4_0/nfe_v4_00.py
--rw-rw-r--  2.0 unx      353 b- defN 24-Mar-02 18:56 nfelib-2.0.4/nfelib/odoo/nfe/v4_0/cons_reci_nfe_v4_00.py
--rw-rw-r--  2.0 unx     2698 b- defN 24-Mar-02 18:56 nfelib-2.0.4/nfelib/odoo/nfe/v4_0/tipos_basico_v4_00.py
--rw-rw-r--  2.0 unx      368 b- defN 24-Mar-02 18:56 nfelib-2.0.4/nfelib/odoo/nfe/v4_0/ret_cons_stat_serv_v4_00.py
--rw-rw-r--  2.0 unx    10446 b- defN 24-Mar-02 18:56 nfelib-2.0.4/nfelib/odoo/nfe/v4_0/leiaute_consulta_cadastro_v2_00.py
--rw-rw-r--  2.0 unx      365 b- defN 24-Mar-02 18:56 nfelib-2.0.4/nfelib/odoo/nfe/v4_0/cons_stat_serv_v4_00.py
--rw-rw-r--  2.0 unx     7036 b- defN 24-Mar-02 18:56 nfelib-2.0.4/nfelib/odoo/nfe/v4_0/leiaute_inut_nfe_v4_00.py
--rw-rw-r--  2.0 unx      361 b- defN 24-Mar-02 18:56 nfelib-2.0.4/nfelib/odoo/nfe/v4_0/cons_sit_nfe_v4_00.py
--rw-rw-r--  2.0 unx      356 b- defN 24-Mar-02 18:56 nfelib-2.0.4/nfelib/odoo/nfe/v4_0/ret_cons_reci_nfe_v4_00.py
--rw-rw-r--  2.0 unx     3767 b- defN 24-Mar-02 18:56 nfelib-2.0.4/nfelib/odoo/nfe/v4_0/leiaute_cons_stat_serv_v4_00.py
--rw-rw-r--  2.0 unx      349 b- defN 24-Mar-02 18:56 nfelib-2.0.4/nfelib/odoo/nfe/v4_0/envi_nfe_v4_00.py
--rw-rw-r--  2.0 unx      349 b- defN 24-Mar-02 18:56 nfelib-2.0.4/nfelib/odoo/nfe/v4_0/proc_nfe_v4_00.py
--rw-rw-r--  2.0 unx      358 b- defN 24-Mar-02 18:56 nfelib-2.0.4/nfelib/odoo/nfe/v4_0/proc_inut_nfe_v4_00.py
--rw-rw-r--  2.0 unx      352 b- defN 24-Mar-02 18:56 nfelib-2.0.4/nfelib/odoo/nfe/v4_0/ret_envi_nfe_v4_00.py
--rw-rw-r--  2.0 unx   184917 b- defN 24-Mar-02 18:56 nfelib-2.0.4/nfelib/odoo/nfe/v4_0/leiaute_nfe_v4_00.py
--rw-rw-r--  2.0 unx      366 b- defN 24-Mar-02 18:56 nfelib-2.0.4/nfelib/odoo/nfe/v4_0/ret_cons_cad_v2_00.py
-781 files, 10974515 bytes uncompressed, 1324421 bytes compressed:  87.9%
+Zip file size: 1367482 bytes, number of entries: 702
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib.egg-info/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/tests/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/
+-rw-rw-r--  2.0 unx     1074 b- defN 24-Apr-05 08:24 nfelib-2.0.5/MIT-LICENSE
+-rw-rw-r--  2.0 unx       38 b- defN 24-Apr-05 08:24 nfelib-2.0.5/setup.py
+-rw-rw-r--  2.0 unx     1493 b- defN 24-May-08 11:09 nfelib-2.0.5/setup.cfg
+-rw-rw-r--  2.0 unx     7477 b- defN 24-May-08 10:59 nfelib-2.0.5/README.md
+-rw-rw-r--  2.0 unx     8697 b- defN 24-May-08 11:09 nfelib-2.0.5/PKG-INFO
+-rw-rw-r--  2.0 unx       64 b- defN 24-Apr-05 08:24 nfelib-2.0.5/MANIFEST.in
+-rw-rw-r--  2.0 unx        7 b- defN 24-May-08 11:09 nfelib-2.0.5/nfelib.egg-info/top_level.txt
+-rw-rw-r--  2.0 unx    30786 b- defN 24-May-08 11:09 nfelib-2.0.5/nfelib.egg-info/SOURCES.txt
+-rw-rw-r--  2.0 unx      113 b- defN 24-May-08 11:09 nfelib-2.0.5/nfelib.egg-info/requires.txt
+-rw-rw-r--  2.0 unx        1 b- defN 24-May-08 11:09 nfelib-2.0.5/nfelib.egg-info/dependency_links.txt
+-rw-rw-r--  2.0 unx     8697 b- defN 24-May-08 11:09 nfelib-2.0.5/nfelib.egg-info/PKG-INFO
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/tests/nfse/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/tests/mdfe/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/tests/nfe_evento_cce/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/tests/cte/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/tests/cce/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/tests/nfe/
+-rwxrwxr-x  2.0 unx     2534 b- defN 24-Apr-05 08:24 nfelib-2.0.5/tests/test_fingerprint.py
+-rw-rw-r--  2.0 unx    11598 b- defN 24-May-08 09:53 nfelib-2.0.5/tests/output_nfse.xml
+-rw-rw-r--  2.0 unx      632 b- defN 24-May-08 09:53 nfelib-2.0.5/tests/output_nfse_pedRegEvento.xml
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-05 08:24 nfelib-2.0.5/tests/__init__.py
+-rw-rw-r--  2.0 unx     1507 b- defN 24-May-08 09:53 nfelib-2.0.5/tests/output_nfse_dps.xml
+-rw-rw-r--  2.0 unx     4370 b- defN 24-May-08 09:53 nfelib-2.0.5/tests/output_cte.xml
+-rw-rw-r--  2.0 unx      453 b- defN 24-May-08 11:08 nfelib-2.0.5/tests/fingerprint.txt
+-rw-rw-r--  2.0 unx     1230 b- defN 24-May-08 09:53 nfelib-2.0.5/tests/output.xml
+-rw-rw-r--  2.0 unx     1207 b- defN 24-May-08 09:53 nfelib-2.0.5/tests/output_nfe_evento_cce.xml
+-rw-rw-r--  2.0 unx      224 b- defN 24-May-08 09:53 nfelib-2.0.5/tests/output_mdfe.xml
+-rw-rw-r--  2.0 unx      482 b- defN 24-May-08 09:53 nfelib-2.0.5/tests/output_nfe_inut.xml
+-rw-rw-r--  2.0 unx    46226 b- defN 24-May-08 09:53 nfelib-2.0.5/tests/output_nfe_leiaute.xml
+-rw-rw-r--  2.0 unx    41634 b- defN 24-May-08 09:53 nfelib-2.0.5/tests/input.xml
+-rw-rw-r--  2.0 unx     2549 b- defN 24-Apr-05 08:24 nfelib-2.0.5/tests/test_all.py
+-rw-rw-r--  2.0 unx     2608 b- defN 24-Apr-05 08:24 nfelib-2.0.5/tests/nfse/test_nfse.py
+-rw-rw-r--  2.0 unx     1054 b- defN 24-Apr-05 08:24 nfelib-2.0.5/tests/mdfe/test_mdfe.py
+-rw-rw-r--  2.0 unx     1102 b- defN 24-Apr-05 08:24 nfelib-2.0.5/tests/nfe_evento_cce/test_cce.py
+-rw-rw-r--  2.0 unx     1049 b- defN 24-Apr-05 08:24 nfelib-2.0.5/tests/cte/test_cte.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/tests/cce/v1_00/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/tests/cce/v1_00/leiauteCCe/
+-rw-rw-r--  2.0 unx     1128 b- defN 24-Apr-05 08:24 nfelib-2.0.5/tests/cce/v1_00/leiauteCCe/35180803102452000172550010000476051695511860-01-cce.xml
+-rw-rw-r--  2.0 unx       23 b- defN 24-Apr-05 08:24 nfelib-2.0.5/tests/nfe/__init__.py
+-rw-rw-r--  2.0 unx     4504 b- defN 24-Apr-05 08:24 nfelib-2.0.5/tests/nfe/test_nfe_legacy.py
+-rw-rw-r--  2.0 unx     8764 b- defN 24-Apr-08 21:49 nfelib-2.0.5/tests/nfe/test_nfe.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfse/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/v4_00/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/mdfe/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_evento_mde/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_insucesso/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_epec/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_entrega/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_dist_dfe/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_evento_cancel/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/cte_dist_dfe/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/bpe/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/mdfe_dist_dfe/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_evento_cce/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_ator_interessado/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/cte/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_evento_generico/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_cons/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe/
+-rw-rw-r--  2.0 unx     7673 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfse/samples/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfse/bindings/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfse/schemas/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfse/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfse/samples/v1_0/
+-rw-rw-r--  2.0 unx     1344 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfse/samples/v1_0/ConsultarNFSeRPS-ped-sitnfserps.xml
+-rw-rw-r--  2.0 unx     1344 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfse/samples/v1_0/GerarNFSeEnvio-env-loterps.xml
+-rw-rw-r--  2.0 unx      728 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfse/samples/v1_0/CancelarNFSe-ped-cannfse.xml
+-rw-rw-r--  2.0 unx    10940 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfse/samples/v1_0/ConsultarNFSeEnvio-ped-sitnfse.xml
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfse/bindings/v1_0/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfse/bindings/__init__.py
+-rw-rw-r--  2.0 unx      516 b- defN 24-Apr-08 21:49 nfelib-2.0.5/nfelib/nfse/bindings/v1_0/ped_reg_evento_v1_00.py
+-rw-rw-r--  2.0 unx     5937 b- defN 24-Apr-08 21:49 nfelib-2.0.5/nfelib/nfse/bindings/v1_0/__init__.py
+-rw-rw-r--  2.0 unx    36107 b- defN 24-Apr-08 21:49 nfelib-2.0.5/nfelib/nfse/bindings/v1_0/tipos_eventos_v1_00.py
+-rw-rw-r--  2.0 unx      496 b- defN 24-Apr-08 21:49 nfelib-2.0.5/nfelib/nfse/bindings/v1_0/nfse_v1_00.py
+-rw-rw-r--  2.0 unx   102239 b- defN 24-Apr-08 21:49 nfelib-2.0.5/nfelib/nfse/bindings/v1_0/tipos_complexos_v1_00.py
+-rw-rw-r--  2.0 unx      494 b- defN 24-Apr-08 21:49 nfelib-2.0.5/nfelib/nfse/bindings/v1_0/dps_v1_00.py
+-rw-rw-r--  2.0 unx    16194 b- defN 24-Apr-08 21:49 nfelib-2.0.5/nfelib/nfse/bindings/v1_0/tipos_simples_v1_00.py
+-rw-rw-r--  2.0 unx     6770 b- defN 24-Apr-08 21:49 nfelib-2.0.5/nfelib/nfse/bindings/v1_0/xmldsig_core_schema_v1_00.py
+-rw-rw-r--  2.0 unx      498 b- defN 24-Apr-08 21:49 nfelib-2.0.5/nfelib/nfse/bindings/v1_0/evento_v1_00.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfse/schemas/v1_0/
+-rw-rw-r--  2.0 unx    29312 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfse/schemas/v1_0/tiposEventos_v1.00.xsd
+-rw-rw-r--  2.0 unx      648 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfse/schemas/v1_0/NFSe_v1.00.xsd
+-rw-rw-r--  2.0 unx      752 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfse/schemas/v1_0/pedRegEvento_v1.00.xsd
+-rw-rw-r--  2.0 unx    78115 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfse/schemas/v1_0/tiposComplexos_v1.00.xsd
+-rw-rw-r--  2.0 unx      587 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfse/schemas/v1_0/DPS_v1.00.xsd
+-rw-rw-r--  2.0 unx     3406 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfse/schemas/v1_0/xmldsig-core-schema_v1.00.xsd
+-rw-rw-r--  2.0 unx    57965 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfse/schemas/v1_0/tiposSimples_v1.00.xsd
+-rw-rw-r--  2.0 unx      743 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfse/schemas/v1_0/evento_v1.00.xsd
+-rw-rw-r--  2.0 unx    88685 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/v4_00/retConsStatServ.py
+-rw-rw-r--  2.0 unx  1859480 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/v4_00/retEnviNFe.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/v4_00/__init__.py
+-rw-rw-r--  2.0 unx      280 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/v4_00/README.txt
+-rw-rw-r--  2.0 unx   235328 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/v4_00/retEnvConfRecebto.py
+-rw-rw-r--  2.0 unx   231041 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/v4_00/retEnvEvento.py
+-rw-rw-r--  2.0 unx     3387 b- defN 24-Apr-08 21:49 nfelib-2.0.5/nfelib/v4_00/leiauteNFe_sub.py
+-rw-rw-r--  2.0 unx   188157 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/v4_00/retInutNFe.py
+-rw-rw-r--  2.0 unx   159793 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/v4_00/retConsCad.py
+-rw-rw-r--  2.0 unx    80047 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/v4_00/distDFeInt.py
+-rw-rw-r--  2.0 unx    79013 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/v4_00/retDistDFeInt.py
+-rw-rw-r--  2.0 unx  1859541 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/v4_00/retConsReciNFe.py
+-rw-rw-r--  2.0 unx   239970 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/v4_00/retEnvCCe.py
+-rw-rw-r--  2.0 unx   237200 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/v4_00/retEnvEventoCancNFe.py
+-rw-rw-r--  2.0 unx   289846 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/v4_00/retConsSitNFe.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/mdfe/samples/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/mdfe/bindings/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/mdfe/schemas/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/mdfe/samples/v3_0/
+-rw-rw-r--  2.0 unx      947 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/samples/v3_0/inclusaoDFe1101154119060611747300015058001000000001111700344401-ped-eve.xml
+-rw-rw-r--  2.0 unx     1407 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/samples/v3_0/pagamentoOperacao1101103511031029073900013955001000000001105112804101-ped-eve.xml
+-rw-rw-r--  2.0 unx     1816 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/samples/v3_0/PagamentoOperacaoMDFe_1101164120039999999999999958001000000999999999999901-ped-eve.xml
+-rw-rw-r--  2.0 unx     3789 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/samples/v3_0/26999999999999999999999999999999999999999991-mdfe.xml
+-rw-rw-r--  2.0 unx     2719 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/samples/v3_0/41190876676436000167580010000500001000437558-mdfe.xml
+-rw-rw-r--  2.0 unx     2057 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/samples/v3_0/50170876063965000276580010000011311421039568-mdfe.xml
+-rw-rw-r--  2.0 unx     3574 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/samples/v3_0/ComPagtoPIX_41210780568835000181580010402005751006005791-procMDFe.xml
+-rw-rw-r--  2.0 unx      180 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/samples/v3_0/310000007934162-ped-rec.xml
+-rw-rw-r--  2.0 unx      702 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/samples/v3_0/cancelameto1101103511031029073900013955001000000001105112804101-ped-eve.xml
+-rw-rw-r--  2.0 unx      732 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/samples/v3_0/encerramento1101123511031029073900013955001000000001105112804101-ped-eve.xml
+-rw-rw-r--  2.0 unx      739 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/samples/v3_0/inclusaocondutor31131223864838000129580000000000051003000003-ped-eve.xml
+-rw-rw-r--  2.0 unx      226 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/samples/v3_0/01010101010-ped-cons-mdfe-naoenc.xml
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/__init__.py
+-rw-rw-r--  2.0 unx      601 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ret_cons_stat_serv_mdfe_v3_00.py
+-rw-rw-r--  2.0 unx     6770 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/xmldsig_core_schema_v1_01.py
+-rw-rw-r--  2.0 unx     5571 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/cons_stat_serv_tipos_basico_v3_00.py
+-rw-rw-r--  2.0 unx     7084 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/__init__.py
+-rw-rw-r--  2.0 unx      545 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/proc_evento_mdfe_v3_00.py
+-rw-rw-r--  2.0 unx     6239 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/cons_sit_mdfe_tipos_basico_v3_00.py
+-rw-rw-r--  2.0 unx     5995 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/mdfe_consulta_dfe_tipos_basico_v3_00.py
+-rw-rw-r--  2.0 unx      552 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ret_evento_mdfe_v3_00.py
+-rw-rw-r--  2.0 unx     7833 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/leiaute_dist_mdfe_v3_00.py
+-rw-rw-r--  2.0 unx      571 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/mdfe_consulta_dfe_v3_00.py
+-rw-rw-r--  2.0 unx    11143 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ev_pagto_oper_mdfe_v3_00.py
+-rw-rw-r--  2.0 unx      505 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ret_mdfe_v3_00.py
+-rw-rw-r--  2.0 unx     1963 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ev_inc_condutor_mdfe_v3_00.py
+-rw-rw-r--  2.0 unx     3502 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/tipos_geral_mdfe_v3_00.py
+-rw-rw-r--  2.0 unx      584 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ret_cons_sit_mdfe_v3_00.py
+-rw-rw-r--  2.0 unx      579 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ret_cons_reci_mdfe_v3_00.py
+-rw-rw-r--  2.0 unx      549 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ret_envi_mdfe_v3_00.py
+-rw-rw-r--  2.0 unx      546 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/envi_mdfe_v3_00.py
+-rw-rw-r--  2.0 unx      580 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/cons_mdfe_nao_enc_v3_00.py
+-rw-rw-r--  2.0 unx     5622 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/cons_mdfe_nao_enc_tipos_basico_v3_00.py
+-rw-rw-r--  2.0 unx      519 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ret_dist_mdfe_v3_00.py
+-rw-rw-r--  2.0 unx      538 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/evento_mdfe_v3_00.py
+-rw-rw-r--  2.0 unx    35874 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/mdfe_modal_rodoviario_v3_00.py
+-rw-rw-r--  2.0 unx    14799 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/evento_mdfe_tipos_basico_v3_00.py
+-rw-rw-r--  2.0 unx     1660 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ev_canc_mdfe_v3_00.py
+-rw-rw-r--  2.0 unx    10218 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/mdfe_modal_aquaviario_v3_00.py
+-rw-rw-r--  2.0 unx      593 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ret_cons_mdfe_nao_enc_v3_00.py
+-rw-rw-r--  2.0 unx      584 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ret_mdfe_consulta_dfe_v3_00.py
+-rw-rw-r--  2.0 unx      531 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/dist_mdfe_v3_00.py
+-rw-rw-r--  2.0 unx     4353 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/cons_reci_mdfe_tipos_basico_v3_00.py
+-rw-rw-r--  2.0 unx     5673 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/mdfe_modal_ferroviario_v3_00.py
+-rw-rw-r--  2.0 unx     3482 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ev_inclusao_dfe_mdfe_v3_00.py
+-rw-rw-r--  2.0 unx      571 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/cons_sit_mdfe_v3_00.py
+-rw-rw-r--  2.0 unx   126107 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/mdfe_tipos_basico_v3_00.py
+-rw-rw-r--  2.0 unx      493 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/mdfe_v3_00.py
+-rw-rw-r--  2.0 unx     2307 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ev_enc_mdfe_v3_00.py
+-rw-rw-r--  2.0 unx     3231 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/mdfe_modal_aereo_v3_00.py
+-rw-rw-r--  2.0 unx      556 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/cons_reci_mdfe_v3_00.py
+-rw-rw-r--  2.0 unx     2310 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/proc_mdfe_v3_00.py
+-rw-rw-r--  2.0 unx      583 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/cons_stat_serv_mdfe_v3_00.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/
+-rw-rw-r--  2.0 unx     6549 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/consReciMDFeTiposBasico_v3.00.xsd
+-rw-rw-r--  2.0 unx      614 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retConsReciMDFe_v3.00.xsd
+-rw-rw-r--  2.0 unx      623 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retConsMDFeNaoEnc_v3.00.xsd
+-rw-rw-r--  2.0 unx      620 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/consStatServMDFe_v3.00.xsd
+-rw-rw-r--  2.0 unx     1935 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/evIncCondutorMDFe_v3.00.xsd
+-rw-rw-r--  2.0 unx     4033 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/consStatServTiposBasico_v3.00.xsd
+-rw-rw-r--  2.0 unx      673 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retMDFe_v3.00.xsd
+-rw-rw-r--  2.0 unx    36487 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/mdfeModalRodoviario_v3.00.xsd
+-rw-rw-r--  2.0 unx     1564 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/evCancMDFe_v3.00.xsd
+-rw-rw-r--  2.0 unx      592 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/distMDFe_v3.00.xsd
+-rw-rw-r--  2.0 unx      614 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retMDFeConsultaDFe_v3.00.xsd
+-rw-rw-r--  2.0 unx     3479 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/mdfeModalAereo_v3.00.xsd
+-rw-rw-r--  2.0 unx     5523 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/mdfeModalFerroviario_v3.00.xsd
+-rw-rw-r--  2.0 unx      597 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/eventoMDFe_v3.00.xsd
+-rw-rw-r--  2.0 unx      632 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retConsStatServMDFe_v3.00.xsd
+-rw-rw-r--  2.0 unx    10610 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/evPagtoOperMDFe_v3.00.xsd
+-rw-rw-r--  2.0 unx      605 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retEventoMDFe_v3.00.xsd
+-rw-rw-r--  2.0 unx      597 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/consReciMDFe_v3.00.xsd
+-rw-rw-r--  2.0 unx      561 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/mdfeConsultaDFe_v3.00.xsd
+-rw-rw-r--  2.0 unx      571 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/consMDFeNaoEnc_v3.00.xsd
+-rw-rw-r--  2.0 unx     1677 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/procMDFe_v3.00.xsd
+-rw-rw-r--  2.0 unx      711 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/enviMDFe_v3.00.xsd
+-rw-rw-r--  2.0 unx     3274 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/evInclusaoDFeMDFe_v3.00.xsd
+-rw-rw-r--  2.0 unx    24229 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/tiposGeralMDFe_v3.00.xsd
+-rw-rw-r--  2.0 unx     3958 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/mdfeConsultaDFeTiposBasico_v3.00.xsd
+-rw-rw-r--  2.0 unx    99783 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/mdfeTiposBasico_v3.00.xsd
+-rw-rw-r--  2.0 unx    10365 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/mdfeModalAquaviario_v3.00.xsd
+-rw-rw-r--  2.0 unx      561 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/mdfe_v3.00.xsd
+-rw-rw-r--  2.0 unx      603 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retEnviMDFe_v3.00.xsd
+-rw-rw-r--  2.0 unx      569 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/consSitMDFe_v3.00.xsd
+-rw-rw-r--  2.0 unx     4559 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/consSitMDFeTiposBasico_v3.00.xsd
+-rw-rw-r--  2.0 unx      623 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retConsMDFeNaoEnc_v1.00.xsd
+-rw-rw-r--  2.0 unx     5554 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/leiauteDistMDFe_v3.00.xsd
+-rw-rw-r--  2.0 unx     4309 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/consMDFeNaoEncTiposBasico_v3.00.xsd
+-rw-rw-r--  2.0 unx     3749 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/xmldsig-core-schema_v1.01.xsd
+-rw-rw-r--  2.0 unx    10018 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/eventoMDFeTiposBasico_v3.00.xsd
+-rw-rw-r--  2.0 unx      587 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/procEventoMDFe_v3.00.xsd
+-rw-rw-r--  2.0 unx      574 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retDistMDFe_v3.00.xsd
+-rw-rw-r--  2.0 unx      622 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retConsSitMDFe_v3.00.xsd
+-rw-rw-r--  2.0 unx     1967 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/evEncMDFe_v3.00.xsd
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_mde/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/__init__.py
+-rw-rw-r--  2.0 unx      561 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/proc_conf_recebto_nfe_v1_00.py
+-rw-rw-r--  2.0 unx     6770 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/xmldsig_core_schema_v1_01.py
+-rw-rw-r--  2.0 unx      309 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/tipos_basico_v1_03.py
+-rw-rw-r--  2.0 unx     1670 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/__init__.py
+-rw-rw-r--  2.0 unx     1578 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/e210240_v1_00.py
+-rw-rw-r--  2.0 unx    20302 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/leiaute_conf_recebto_v1_00.py
+-rw-rw-r--  2.0 unx      541 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/conf_recebto_v1_00.py
+-rw-rw-r--  2.0 unx      570 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/ret_env_conf_recebto_v1_00.py
+-rw-rw-r--  2.0 unx      570 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/env_conf_recebto_v1_00.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/
+-rw-rw-r--  2.0 unx    15624 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/leiauteConfRecebto_v1.00.xsd
+-rw-rw-r--  2.0 unx      598 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/procConfRecebtoNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx     1767 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/e210220_v1.00.xsd
+-rw-rw-r--  2.0 unx     1269 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/e210200_v1.00.xsd
+-rw-rw-r--  2.0 unx     1755 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/e210240_v1.00.xsd
+-rw-rw-r--  2.0 unx      612 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/envConfRecebto_v1.00.xsd
+-rw-rw-r--  2.0 unx     1253 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/e210210_v1.00.xsd
+-rw-rw-r--  2.0 unx      586 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/confRecebto_v1.00.xsd
+-rw-rw-r--  2.0 unx    30140 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/tiposBasico_v1.03.xsd
+-rw-rw-r--  2.0 unx      603 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/retEnvConfRecebto_v1.00.xsd
+-rw-rw-r--  2.0 unx     3749 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_insucesso/bindings/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_insucesso/schemas/
+-rw-rw-r--  2.0 unx      154 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/nfe_insucesso/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/
+-rw-rw-r--  2.0 unx      154 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/nfe_insucesso/bindings/__init__.py
+-rw-rw-r--  2.0 unx     5466 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/tmp0000.py
+-rw-rw-r--  2.0 unx     6769 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/xmldsig_core_schema_v1_01.py
+-rw-rw-r--  2.0 unx     1010 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/tipos_basico_v1_03.py
+-rw-rw-r--  2.0 unx     1811 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/__init__.py
+-rw-rw-r--  2.0 unx      578 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/ret_evento_insucesso_nfe_v1_00.py
+-rw-rw-r--  2.0 unx      583 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/env_evento_insucesso_nfe_v1_00.py
+-rw-rw-r--  2.0 unx      550 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/evento_insucesso_nfe_v1_00.py
+-rw-rw-r--  2.0 unx    16741 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/leiaute_evento_insucesso_nfe_v1_00.py
+-rw-rw-r--  2.0 unx      566 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/proc_evento_insucesso_nfe_v1_00.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/
+-rw-rw-r--  2.0 unx      725 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/envEventoInsucessoNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx     4651 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/tmp0000.xsd
+-rw-rw-r--  2.0 unx     4459 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/e110192_v1.00.xsd
+-rw-rw-r--  2.0 unx      612 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/retEventoCancInsucessoNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx      601 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/procEventoInsucessoNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx    11599 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/leiauteEventoCancInsucessoNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx      596 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/EventoInsucessoNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx      612 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/retEventoInsucessoNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx    11613 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/leiauteEventoInsucessoNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx     1774 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/e110193_v1.00.xsd
+-rw-rw-r--  2.0 unx      617 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/EventoCancInsucessoNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx    32624 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/tiposBasico_v1.03.xsd
+-rw-rw-r--  2.0 unx     3749 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
+-rw-rw-r--  2.0 unx      634 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/procEventoCancInsucessoNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx      745 b- defN 24-May-08 11:08 nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/envEventoCancInsucessoNFe_v1.00.xsd
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_epec/bindings/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_epec/schemas/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_epec/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_epec/bindings/v1_0/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_epec/bindings/__init__.py
+-rw-rw-r--  2.0 unx     1435 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_epec/bindings/v1_0/__init__.py
+-rw-rw-r--  2.0 unx    10677 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_epec/bindings/v1_0/e110140_v1_00.py
+-rw-rw-r--  2.0 unx    37803 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_epec/bindings/v1_0/leiaute_epec_v1_00.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_epec/schemas/v1_0/
+-rw-rw-r--  2.0 unx      585 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_epec/schemas/v1_0/EPEC_v1.00.xsd
+-rw-rw-r--  2.0 unx     4475 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_epec/schemas/v1_0/e110140_v1.00.xsd
+-rw-rw-r--  2.0 unx      608 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_epec/schemas/v1_0/envEPEC_v1.00.xsd
+-rw-rw-r--  2.0 unx      601 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_epec/schemas/v1_0/procEPEC_v1.00.xsd
+-rw-rw-r--  2.0 unx    17318 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_epec/schemas/v1_0/leiauteEPEC_v1.00.xsd
+-rw-rw-r--  2.0 unx    30140 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_epec/schemas/v1_0/tiposBasico_v1.03.xsd
+-rw-rw-r--  2.0 unx     3749 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_epec/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
+-rw-rw-r--  2.0 unx      601 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_epec/schemas/v1_0/retEnvEPEC_v1.00.xsd
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_entrega/bindings/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_entrega/schemas/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_entrega/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_entrega/bindings/__init__.py
+-rw-rw-r--  2.0 unx     6770 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/xmldsig_core_schema_v1_01.py
+-rw-rw-r--  2.0 unx     1012 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/tipos_basico_v1_03.py
+-rw-rw-r--  2.0 unx     1782 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/__init__.py
+-rw-rw-r--  2.0 unx      549 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/evento_entrega_nfe_v1_00.py
+-rw-rw-r--  2.0 unx      565 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/proc_evento_entrega_nfe_v1_00.py
+-rw-rw-r--  2.0 unx      577 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/ret_evento_entrega_nfe_v1_00.py
+-rw-rw-r--  2.0 unx    17661 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/leiaute_evento_entrega_nfe_v1_00.py
+-rw-rw-r--  2.0 unx      581 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/env_evento_entrega_nfe_v1_00.py
+-rw-rw-r--  2.0 unx     5351 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/e110130_v1_00.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/
+-rw-rw-r--  2.0 unx      744 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/envEventoCancEntregaNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx      601 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/procEventoEntregaNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx      615 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/EventoCancEntregaNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx      616 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/retEventoCancEntregaNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx      596 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/EventoEntregaNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx     4424 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/e110130_v1.00.xsd
+-rw-rw-r--  2.0 unx    11920 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/leiauteEventoCancEntregaNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx    12382 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/leiauteEventoEntregaNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx      724 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/envEventoEntregaNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx    32624 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/tiposBasico_v1.03.xsd
+-rw-rw-r--  2.0 unx      612 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/retEventoEntregaNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx     3749 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
+-rw-rw-r--  2.0 unx     2191 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/e110131_v1.00.xsd
+-rw-rw-r--  2.0 unx      634 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/procEventoCancEntregaNFe_v1.00.xsd
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_dist_dfe/schemas/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_dist_dfe/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/v1_0/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/__init__.py
+-rw-rw-r--  2.0 unx     4873 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/v1_0/res_evento_v1_01.py
+-rw-rw-r--  2.0 unx     6770 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/v1_0/xmldsig_core_schema_v1_01.py
+-rw-rw-r--  2.0 unx     1375 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/v1_0/__init__.py
+-rw-rw-r--  2.0 unx     5501 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/v1_0/ret_dist_dfe_int_v1_01.py
+-rw-rw-r--  2.0 unx     5290 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/v1_0/res_nfe_v1_01.py
+-rw-rw-r--  2.0 unx     4141 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/v1_0/dist_dfe_int_v1_01.py
+-rw-rw-r--  2.0 unx     1770 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/v1_0/tipos_dist_dfe_v1_01.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_dist_dfe/schemas/v1_0/
+-rw-rw-r--  2.0 unx     4407 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_dist_dfe/schemas/v1_0/retDistDFeInt_v1.01.xsd
+-rw-rw-r--  2.0 unx     8230 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_dist_dfe/schemas/v1_0/tiposDistDFe_v1.01.xsd
+-rw-rw-r--  2.0 unx     4034 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_dist_dfe/schemas/v1_0/distDFeInt_v1.01.xsd
+-rw-rw-r--  2.0 unx     4495 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_dist_dfe/schemas/v1_0/resEvento_v1.01.xsd
+-rw-rw-r--  2.0 unx     4933 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_dist_dfe/schemas/v1_0/resNFe_v1.01.xsd
+-rw-rw-r--  2.0 unx     3747 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_dist_dfe/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cancel/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/__init__.py
+-rw-rw-r--  2.0 unx     1954 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/e110111_v1_00.py
+-rw-rw-r--  2.0 unx      560 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/ret_env_evento_canc_nfe_v1_00.py
+-rw-rw-r--  2.0 unx     6770 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/xmldsig_core_schema_v1_01.py
+-rw-rw-r--  2.0 unx     1012 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/tipos_basico_v1_03.py
+-rw-rw-r--  2.0 unx     1773 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/__init__.py
+-rw-rw-r--  2.0 unx      560 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/env_evento_canc_nfe_v1_00.py
+-rw-rw-r--  2.0 unx      551 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/proc_evento_canc_nfe_v1_00.py
+-rw-rw-r--  2.0 unx    20018 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/leiaute_evento_canc_nfe_v1_00.py
+-rw-rw-r--  2.0 unx      531 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/evento_canc_nfe_v1_00.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/v1_0/
+-rw-rw-r--  2.0 unx      595 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/v1_0/envEventoCancNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx      572 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/v1_0/eventoCancNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx    13952 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/v1_0/leiauteEventoCancNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx     1770 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/v1_0/e110111_v1.00.xsd
+-rw-rw-r--  2.0 unx      581 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/v1_0/procEventoCancNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx      589 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/v1_0/retEnvEventoCancNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx    32400 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/v1_0/tiposBasico_v1.03.xsd
+-rw-rw-r--  2.0 unx     3749 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/cte_dist_dfe/bindings/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/cte_dist_dfe/schemas/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/cte_dist_dfe/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/cte_dist_dfe/bindings/v1_0/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/cte_dist_dfe/bindings/__init__.py
+-rw-rw-r--  2.0 unx     3502 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/cte_dist_dfe/bindings/v1_0/dist_dfe_int_v1_00.py
+-rw-rw-r--  2.0 unx     6770 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/cte_dist_dfe/bindings/v1_0/xmldsig_core_schema_v1_01.py
+-rw-rw-r--  2.0 unx     1002 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/cte_dist_dfe/bindings/v1_0/__init__.py
+-rw-rw-r--  2.0 unx     1067 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/cte_dist_dfe/bindings/v1_0/tipos_dist_dfe_v1_00.py
+-rw-rw-r--  2.0 unx     5420 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/cte_dist_dfe/bindings/v1_0/ret_dist_dfe_int_v1_00.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/cte_dist_dfe/schemas/v1_0/
+-rw-rw-r--  2.0 unx     3407 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/cte_dist_dfe/schemas/v1_0/distDFeInt_v1.00.xsd
+-rw-rw-r--  2.0 unx     4283 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/cte_dist_dfe/schemas/v1_0/retDistDFeInt_v1.00.xsd
+-rw-rw-r--  2.0 unx     3747 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/cte_dist_dfe/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
+-rw-rw-r--  2.0 unx     8554 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/cte_dist_dfe/schemas/v1_0/tiposDistDFe_v1.00.xsd
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/bpe/bindings/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/bpe/schemas/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/bpe/bindings/v1_0/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/bindings/__init__.py
+-rw-rw-r--  2.0 unx     4651 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/bindings/v1_0/cons_sit_bpe_tipos_basico_v1_00.py
+-rw-rw-r--  2.0 unx     6770 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/bindings/v1_0/xmldsig_core_schema_v1_01.py
+-rw-rw-r--  2.0 unx     4296 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/bindings/v1_0/__init__.py
+-rw-rw-r--  2.0 unx     5551 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/bindings/v1_0/cons_stat_serv_bpe_tipos_basico_v1_00.py
+-rw-rw-r--  2.0 unx     1588 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/bindings/v1_0/ev_nao_emb_bpe_v1_00.py
+-rw-rw-r--  2.0 unx     1657 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/bindings/v1_0/ev_alteracao_poltrona_v1_00.py
+-rw-rw-r--  2.0 unx      531 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/bindings/v1_0/evento_bpe_v1_00.py
+-rw-rw-r--  2.0 unx     2681 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/bindings/v1_0/tipos_geral_bpe_v1_00.py
+-rw-rw-r--  2.0 unx      505 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/bindings/v1_0/bpe_tm_v1_00.py
+-rw-rw-r--  2.0 unx      529 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/bindings/v1_0/proc_evento_bpe_v1_00.py
+-rw-rw-r--  2.0 unx      539 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/bindings/v1_0/ret_evento_bpe_v1_00.py
+-rw-rw-r--  2.0 unx      581 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/bindings/v1_0/cons_stat_serv_bpe_v1_00.py
+-rw-rw-r--  2.0 unx      472 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/bindings/v1_0/bpe_v1_00.py
+-rw-rw-r--  2.0 unx      575 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/bindings/v1_0/ret_cons_sit_bpe_v1_00.py
+-rw-rw-r--  2.0 unx      562 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/bindings/v1_0/cons_sit_bpe_v1_00.py
+-rw-rw-r--  2.0 unx     2310 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/bindings/v1_0/proc_bpe_tm_v1_00.py
+-rw-rw-r--  2.0 unx    13972 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/bindings/v1_0/evento_bpe_tipos_basico_v1_00.py
+-rw-rw-r--  2.0 unx      497 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/bindings/v1_0/ret_bpe_v1_00.py
+-rw-rw-r--  2.0 unx     1915 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/bindings/v1_0/ev_excesso_bagagem_v1_00.py
+-rw-rw-r--  2.0 unx      599 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/bindings/v1_0/ret_cons_stat_serv_bpe_v1_00.py
+-rw-rw-r--  2.0 unx     1542 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/bindings/v1_0/ev_canc_bpe_v1_00.py
+-rw-rw-r--  2.0 unx     2295 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/bindings/v1_0/proc_bpe_v1_00.py
+-rw-rw-r--  2.0 unx   131130 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/bindings/v1_0/bpe_tipos_basico_v1_00.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/bpe/schemas/v1_0/
+-rw-rw-r--  2.0 unx      698 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/schemas/v1_0/eventoBPe_v1.00.xsd
+-rw-rw-r--  2.0 unx      619 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/schemas/v1_0/consStatServBPe_v1.00.xsd
+-rw-rw-r--  2.0 unx   107163 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/schemas/v1_0/bpeTiposBasico_v1.00.xsd
+-rw-rw-r--  2.0 unx      594 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/schemas/v1_0/retEventoBPe_v1.00.xsd
+-rw-rw-r--  2.0 unx    23114 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/schemas/v1_0/tiposGeralBPe_v1.00.xsd
+-rw-rw-r--  2.0 unx     1411 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/schemas/v1_0/evCancBPe_v1.00.xsd
+-rw-rw-r--  2.0 unx     1570 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/schemas/v1_0/evNaoEmbBPe_v1.00.xsd
+-rw-rw-r--  2.0 unx      616 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/schemas/v1_0/retConsSitBPe_v1.00.xsd
+-rw-rw-r--  2.0 unx      649 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/schemas/v1_0/bpe_v1.00.xsd
+-rw-rw-r--  2.0 unx     2028 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/schemas/v1_0/evExcessoBagagem_v1.00.xsd
+-rw-rw-r--  2.0 unx      562 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/schemas/v1_0/retBPe_v1.00.xsd
+-rw-rw-r--  2.0 unx     9549 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/schemas/v1_0/eventoBPeTiposBasico_v1.00.xsd
+-rw-rw-r--  2.0 unx     1668 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/schemas/v1_0/procBPe_v1.00.xsd
+-rw-rw-r--  2.0 unx     1677 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/schemas/v1_0/procBPeTM_v1.00.xsd
+-rw-rw-r--  2.0 unx      631 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/schemas/v1_0/retConsStatServBPe_v1.00.xsd
+-rw-rw-r--  2.0 unx     1862 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/schemas/v1_0/evAlteracaoPoltrona_v1.00.xsd
+-rw-rw-r--  2.0 unx     3270 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/schemas/v1_0/consSitBPeTiposBasico_v1.00.xsd
+-rw-rw-r--  2.0 unx      678 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/schemas/v1_0/bpeTM_v1.00.xsd
+-rw-rw-r--  2.0 unx     3749 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
+-rw-rw-r--  2.0 unx      582 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/schemas/v1_0/procEventoBPe_v1.00.xsd
+-rw-rw-r--  2.0 unx      563 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/schemas/v1_0/consSitBPe_v1.00.xsd
+-rw-rw-r--  2.0 unx     4106 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/bpe/schemas/v1_0/consStatServBPeTiposBasico_v1.00.xsd
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/mdfe_dist_dfe/bindings/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/mdfe_dist_dfe/schemas/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe_dist_dfe/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/mdfe_dist_dfe/bindings/v1_0/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe_dist_dfe/bindings/__init__.py
+-rw-rw-r--  2.0 unx     3279 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe_dist_dfe/bindings/v1_0/dist_dfe_int_v1_00.py
+-rw-rw-r--  2.0 unx     6770 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe_dist_dfe/bindings/v1_0/xmldsig_core_schema_v1_01.py
+-rw-rw-r--  2.0 unx     1028 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe_dist_dfe/bindings/v1_0/__init__.py
+-rw-rw-r--  2.0 unx      352 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe_dist_dfe/bindings/v1_0/tipos_dist_dfe_v1_00.py
+-rw-rw-r--  2.0 unx      310 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe_dist_dfe/bindings/v1_0/tipos_geral_mdfe_v1_00.py
+-rw-rw-r--  2.0 unx     5453 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe_dist_dfe/bindings/v1_0/ret_dist_dfe_int_v1_00.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/mdfe_dist_dfe/schemas/v1_0/
+-rw-rw-r--  2.0 unx    22419 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe_dist_dfe/schemas/v1_0/tiposGeralMDFe_v1.00.xsd
+-rw-rw-r--  2.0 unx     2843 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe_dist_dfe/schemas/v1_0/distDFeInt_v1.00.xsd
+-rw-rw-r--  2.0 unx     4248 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe_dist_dfe/schemas/v1_0/retDistDFeInt_v1.00.xsd
+-rw-rw-r--  2.0 unx     3747 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe_dist_dfe/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
+-rw-rw-r--  2.0 unx     6807 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/mdfe_dist_dfe/schemas/v1_0/tiposDistDFe_v1.00.xsd
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_evento_cce/samples/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cce/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_evento_cce/samples/v1_0/
+-rw-rw-r--  2.0 unx     1207 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cce/samples/v1_0/35180803102452000172550010000476051695511860-01-cce.xml
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/__init__.py
+-rw-rw-r--  2.0 unx      514 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/cce_v1_00.py
+-rw-rw-r--  2.0 unx     6770 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/xmldsig_core_schema_v1_01.py
+-rw-rw-r--  2.0 unx      309 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/tipos_basico_v1_03.py
+-rw-rw-r--  2.0 unx     1705 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/__init__.py
+-rw-rw-r--  2.0 unx      541 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/proc_cce_nfe_v1_00.py
+-rw-rw-r--  2.0 unx    22394 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/leiaute_cce_v1_00.py
+-rw-rw-r--  2.0 unx     1850 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/e110110_v1_00.py
+-rw-rw-r--  2.0 unx      543 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/ret_env_cce_v1_00.py
+-rw-rw-r--  2.0 unx      543 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/env_cce_v1_00.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/v1_0/
+-rw-rw-r--  2.0 unx    17276 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/v1_0/leiauteCCe_v1.00.xsd
+-rw-rw-r--  2.0 unx      657 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/v1_0/CCe_v1.00.xsd
+-rw-rw-r--  2.0 unx      627 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/v1_0/procCCeNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx     3340 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/v1_0/e110110_v1.00.xsd
+-rw-rw-r--  2.0 unx      630 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/v1_0/envCCe_v1.00.xsd
+-rw-rw-r--  2.0 unx    30140 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/v1_0/tiposBasico_v1.03.xsd
+-rw-rw-r--  2.0 unx     3749 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
+-rw-rw-r--  2.0 unx      627 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/v1_0/retEnvCCe_v1.00.xsd
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_ator_interessado/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/__init__.py
+-rw-rw-r--  2.0 unx     6770 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/xmldsig_core_schema_v1_01.py
+-rw-rw-r--  2.0 unx     1657 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/tipos_basico_v1_03.py
+-rw-rw-r--  2.0 unx     2035 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/__init__.py
+-rw-rw-r--  2.0 unx      583 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/ret_env_evento_ator_interessado_v1_00.py
+-rw-rw-r--  2.0 unx      573 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/proc_evento_ator_interessado_v1_00.py
+-rw-rw-r--  2.0 unx     4481 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/mod_110150_v1_00.py
+-rw-rw-r--  2.0 unx      557 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/evento_ator_interessado_v1_00.py
+-rw-rw-r--  2.0 unx    21825 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/leiaute_evento_ator_interessado_v1_00.py
+-rw-rw-r--  2.0 unx      586 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/env_evento_ator_interessado_v1_00.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/v1_0/
+-rw-rw-r--  2.0 unx      609 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/v1_0/retEnvEventoAtorInteressado_v1.00.xsd
+-rw-rw-r--  2.0 unx      600 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/v1_0/procEventoAtorInteressado_v1.00.xsd
+-rw-rw-r--  2.0 unx     3942 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/v1_0/110150_v1.00.xsd
+-rw-rw-r--  2.0 unx    15700 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/v1_0/leiauteEventoAtorInteressado_v1.00.xsd
+-rw-rw-r--  2.0 unx      618 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/v1_0/envEventoAtorInteressado_v1.00.xsd
+-rw-rw-r--  2.0 unx      595 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/v1_0/eventoAtorInteressado_v1.00.xsd
+-rw-rw-r--  2.0 unx    31796 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/v1_0/tiposBasico_v1.03.xsd
+-rw-rw-r--  2.0 unx     3749 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/cte/samples/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/cte/bindings/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/cte/schemas/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/cte/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/cte/samples/v4_0/
+-rw-rw-r--  2.0 unx     3436 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/cte/samples/v4_0/51160624686092000173570010000000031000000020-cte.XML
+-rw-rw-r--  2.0 unx     1558 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/cte/samples/v4_0/cce35150107565416000104570000000012301000012300-ped-eve.xml
+-rw-rw-r--  2.0 unx    10117 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/cte/samples/v4_0/35190602427026001207570040000522031000522035-cte-multimodal.xml
+-rw-rw-r--  2.0 unx     3168 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/cte/samples/v4_0/35170799999999999999670000000000261309301440-cte-of.xml
+-rw-rw-r--  2.0 unx     4378 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/cte/samples/v4_0/43120178408960000182570010000000041000000047-cte.xml
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/cte/bindings/v4_0/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/cte/bindings/__init__.py
+-rw-rw-r--  2.0 unx     1769 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_reg_multimodal_v4_00.py
+-rw-rw-r--  2.0 unx      594 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/ret_cons_stat_serv_cte_v4_00.py
+-rw-rw-r--  2.0 unx     3786 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_multi_modal_v4_00.py
+-rw-rw-r--  2.0 unx     6898 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_epeccte_v4_00.py
+-rw-rw-r--  2.0 unx     6769 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/xmldsig_core_schema_v1_01.py
+-rw-rw-r--  2.0 unx     5859 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/cons_stat_serv_tipos_basico_v4_00.py
+-rw-rw-r--  2.0 unx     8883 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/__init__.py
+-rw-rw-r--  2.0 unx     2303 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/proc_gtve_v4_00.py
+-rw-rw-r--  2.0 unx     5940 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_iecte_v4_00.py
+-rw-rw-r--  2.0 unx      564 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/ret_inut_cte_v4_00.py
+-rw-rw-r--  2.0 unx     2294 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/proc_cte_v4_00.py
+-rw-rw-r--  2.0 unx      534 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/proc_inut_cte_v4_00.py
+-rw-rw-r--  2.0 unx     1661 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_canc_prest_desacordo_v4_00.py
+-rw-rw-r--  2.0 unx     4686 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_modal_rodoviario_v4_00.py
+-rw-rw-r--  2.0 unx      478 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_v4_00.py
+-rw-rw-r--  2.0 unx      574 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/ret_cons_sit_cte_v4_00.py
+-rw-rw-r--  2.0 unx     6926 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_cce_cte_v4_00.py
+-rw-rw-r--  2.0 unx    18408 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/evento_cte_tipos_basico_v4_00.py
+-rw-rw-r--  2.0 unx     4334 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/tipos_geral_cte_v4_00.py
+-rw-rw-r--  2.0 unx     1540 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_canc_cte_v4_00.py
+-rw-rw-r--  2.0 unx      531 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/ret_gtve_v4_00.py
+-rw-rw-r--  2.0 unx      559 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/ret_cte_simp_v4_00.py
+-rw-rw-r--  2.0 unx     7464 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_modal_rodoviario_os_v4_00.py
+-rw-rw-r--  2.0 unx      529 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/proc_evento_cte_v4_00.py
+-rw-rw-r--  2.0 unx     8259 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_modal_aquaviario_v4_00.py
+-rw-rw-r--  2.0 unx    11300 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_gtv_v4_00.py
+-rw-rw-r--  2.0 unx     1780 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_modal_dutoviario_v4_00.py
+-rw-rw-r--  2.0 unx   424251 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_tipos_basico_v4_00.py
+-rw-rw-r--  2.0 unx      530 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/evento_cte_v4_00.py
+-rw-rw-r--  2.0 unx      503 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_os_v4_00.py
+-rw-rw-r--  2.0 unx      538 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/ret_evento_cte_v4_00.py
+-rw-rw-r--  2.0 unx     5479 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_cecte_v4_00.py
+-rw-rw-r--  2.0 unx      526 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/ret_cte_v4_00.py
+-rw-rw-r--  2.0 unx      576 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/cons_stat_serv_cte_v4_00.py
+-rw-rw-r--  2.0 unx      537 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/ret_cte_os_v4_00.py
+-rw-rw-r--  2.0 unx     6178 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/cons_sit_cte_tipos_basico_v4_00.py
+-rw-rw-r--  2.0 unx     1676 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_canc_iecte_v4_00.py
+-rw-rw-r--  2.0 unx      561 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/cons_sit_cte_v4_00.py
+-rw-rw-r--  2.0 unx     1684 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_canc_cecte_v4_00.py
+-rw-rw-r--  2.0 unx      576 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/inut_cte_v4_00.py
+-rw-rw-r--  2.0 unx    14185 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/inut_cte_tipos_basico_v4_00.py
+-rw-rw-r--  2.0 unx     2313 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/proc_cte_os_v4_00.py
+-rw-rw-r--  2.0 unx      475 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/gtve_v4_00.py
+-rw-rw-r--  2.0 unx      507 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_simp_v4_00.py
+-rw-rw-r--  2.0 unx     8880 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_modal_ferroviario_v4_00.py
+-rw-rw-r--  2.0 unx    10485 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_modal_aereo_v4_00.py
+-rw-rw-r--  2.0 unx     1773 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_prest_desacordo_v4_00.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/cte/schemas/v4_0/
+-rw-rw-r--  2.0 unx     4259 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteModalRodoviario_v4.00.xsd
+-rw-rw-r--  2.0 unx   332786 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteTiposBasico_v4.00.xsd
+-rw-rw-r--  2.0 unx    10576 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/evGTV_v4.00.xsd
+-rw-rw-r--  2.0 unx      700 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/retEventoCTe_v4.00.xsd
+-rw-rw-r--  2.0 unx     8583 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteModalFerroviario_v4.00.xsd
+-rw-rw-r--  2.0 unx     6338 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/evCCeCTe_v4.00.xsd
+-rw-rw-r--  2.0 unx      698 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/eventoCTe_v4.00.xsd
+-rw-rw-r--  2.0 unx     2213 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/evRegMultimodal_v4.00.xsd
+-rw-rw-r--  2.0 unx      706 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/retCTeOS_v4.00.xsd
+-rw-rw-r--  2.0 unx      702 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/retGTVe_v4.00.xsd
+-rw-rw-r--  2.0 unx      699 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/retCTe_v4.00.xsd
+-rw-rw-r--  2.0 unx     2075 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/evPrestDesacordo_v4.00.xsd
+-rw-rw-r--  2.0 unx     9313 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/inutCTeTiposBasico_v4.00.xsd
+-rw-rw-r--  2.0 unx      677 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteSimp_v4.00.xsd
+-rw-rw-r--  2.0 unx     5494 b- defN 23-Mar-09 13:51 nfelib-2.0.5/nfelib/cte/schemas/v4_0/evIECTe_v4.00.xsd
+-rw-rw-r--  2.0 unx     1707 b- defN 23-Feb-27 09:00 nfelib-2.0.5/nfelib/cte/schemas/v4_0/evCancPrestDesacordo_v4.00.xsd
+-rw-rw-r--  2.0 unx      734 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/retConsStatServCTe_v4.00.xsd
+-rw-rw-r--  2.0 unx     4469 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/consStatServTiposBasico_v4.00.xsd
+-rw-rw-r--  2.0 unx    11173 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteModalAereo_v4.00.xsd
+-rw-rw-r--  2.0 unx     1673 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/procGTVe_v4.00.xsd
+-rw-rw-r--  2.0 unx     6498 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/evEPECCTe_v4.00.xsd
+-rw-rw-r--  2.0 unx     8005 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteModalRodoviarioOS_v4.00.xsd
+-rw-rw-r--  2.0 unx     1348 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteModalDutoviario_v4.00.xsd
+-rw-rw-r--  2.0 unx    24294 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/tiposGeralCTe_v4.00.xsd
+-rw-rw-r--  2.0 unx      651 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/GTVe_v4.00.xsd
+-rw-rw-r--  2.0 unx     1648 b- defN 23-Mar-09 13:52 nfelib-2.0.5/nfelib/cte/schemas/v4_0/evCancIECTe_v4.00.xsd
+-rw-rw-r--  2.0 unx     4015 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteMultiModal_v4.00.xsd
+-rw-rw-r--  2.0 unx      834 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/retInutCTe_v4.00.xsd
+-rw-rw-r--  2.0 unx      800 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/procEventoCTe_v4.00.xsd
+-rw-rw-r--  2.0 unx     4690 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/evCECTe_v4.00.xsd
+-rw-rw-r--  2.0 unx      741 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/inutCTe_v4.00.xsd
+-rw-rw-r--  2.0 unx    13190 b- defN 23-Apr-28 08:26 nfelib-2.0.5/nfelib/cte/schemas/v4_0/eventoCTeTiposBasico_v4.00.xsd
+-rw-rw-r--  2.0 unx      677 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteOS_v4.00.xsd
+-rw-rw-r--  2.0 unx     4735 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/consSitCTeTiposBasico_v4.00.xsd
+-rw-rw-r--  2.0 unx      722 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/consStatServCTe_v4.00.xsd
+-rw-rw-r--  2.0 unx     1679 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/procCTeOS_v4.00.xsd
+-rw-rw-r--  2.0 unx      722 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/retConsSitCTe_v4.00.xsd
+-rw-rw-r--  2.0 unx      669 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/consSitCTe_v4.00.xsd
+-rw-rw-r--  2.0 unx     7868 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteModalAquaviario_v4.00.xsd
+-rw-rw-r--  2.0 unx      656 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/cte_v4.00.xsd
+-rw-rw-r--  2.0 unx      695 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/procInutCTe_v4.00.xsd
+-rw-rw-r--  2.0 unx      720 b- defN 24-May-08 08:07 nfelib-2.0.5/nfelib/cte/schemas/v4_0/retCTeSimp_v4.00.xsd
+-rw-rw-r--  2.0 unx     1668 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/procCTe_v4.00.xsd
+-rw-rw-r--  2.0 unx     1673 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/evCancCECTe_v4.00.xsd
+-rw-rw-r--  2.0 unx     1516 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/evCancCTe_v4.00.xsd
+-rw-rw-r--  2.0 unx     3749 b- defN 23-Feb-27 11:40 nfelib-2.0.5/nfelib/cte/schemas/v4_0/xmldsig-core-schema_v1.01.xsd
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_evento_generico/bindings/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_evento_generico/schemas/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_generico/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_evento_generico/bindings/v1_0/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_generico/bindings/__init__.py
+-rw-rw-r--  2.0 unx     6770 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_generico/bindings/v1_0/xmldsig_core_schema_v1_01.py
+-rw-rw-r--  2.0 unx      309 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_generico/bindings/v1_0/tipos_basico_v1_03.py
+-rw-rw-r--  2.0 unx     1346 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_generico/bindings/v1_0/__init__.py
+-rw-rw-r--  2.0 unx      540 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_generico/bindings/v1_0/env_evento_v1_00.py
+-rw-rw-r--  2.0 unx      540 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_generico/bindings/v1_0/ret_env_evento_v1_00.py
+-rw-rw-r--  2.0 unx      542 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_generico/bindings/v1_0/proc_evento_nfe_v1_00.py
+-rw-rw-r--  2.0 unx    19324 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_generico/bindings/v1_0/leiaute_evento_v1_00.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_evento_generico/schemas/v1_0/
+-rw-rw-r--  2.0 unx      575 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_generico/schemas/v1_0/envEvento_v1.00.xsd
+-rw-rw-r--  2.0 unx    14282 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_generico/schemas/v1_0/leiauteEvento_v1.00.xsd
+-rw-rw-r--  2.0 unx      572 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_generico/schemas/v1_0/procEventoNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx      569 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_generico/schemas/v1_0/retEnvEvento_v1.00.xsd
+-rw-rw-r--  2.0 unx    30140 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_generico/schemas/v1_0/tiposBasico_v1.03.xsd
+-rw-rw-r--  2.0 unx     3749 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_evento_generico/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_cons/bindings/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_cons/schemas/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_cons/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_cons/bindings/v2_0/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_cons/bindings/__init__.py
+-rw-rw-r--  2.0 unx     6770 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_cons/bindings/v2_0/xmldsig_core_schema_v1_01.py
+-rw-rw-r--  2.0 unx      934 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_cons/bindings/v2_0/tipos_basico_v1_03.py
+-rw-rw-r--  2.0 unx     1504 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_cons/bindings/v2_0/__init__.py
+-rw-rw-r--  2.0 unx      585 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_cons/bindings/v2_0/cons_sit_nfe_v2_01.py
+-rw-rw-r--  2.0 unx    29843 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_cons/bindings/v2_0/leiaute_cons_sit_nfe_v2_01.py
+-rw-rw-r--  2.0 unx      575 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_cons/bindings/v2_0/ret_cons_sit_nfe_v2_01.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe_cons/schemas/v2_0/
+-rw-rw-r--  2.0 unx      655 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_cons/schemas/v2_0/consSitNFe_v2.01.xsd
+-rw-rw-r--  2.0 unx    22200 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_cons/schemas/v2_0/leiauteConsSitNFe_v2.01.xsd
+-rw-rw-r--  2.0 unx    29554 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_cons/schemas/v2_0/tiposBasico_v1.03.xsd
+-rw-rw-r--  2.0 unx     3749 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_cons/schemas/v2_0/xmldsig-core-schema_v1.01.xsd
+-rw-rw-r--  2.0 unx      686 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe_cons/schemas/v2_0/retConsSitNFe_v2.01.xsd
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe/samples/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe/bindings/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe/ws/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe/schemas/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe/samples/v4_0/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteInutNFe/
+-rw-rw-r--  2.0 unx    10647 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476711079516696-nfe.xml
+-rw-rw-r--  2.0 unx     7180 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/42220575277525000178550030000292481295366801-procNFe.xml
+-rw-rw-r--  2.0 unx    37663 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000474491454651420-nfe.xml
+-rw-rw-r--  2.0 unx    14538 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476051695511860-nfe.xml
+-rw-rw-r--  2.0 unx    32177 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476491552806942-nfe.xml
+-rw-rw-r--  2.0 unx     9218 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/41170706117473000150550010000463202612756525-procNFe.xml
+-rw-rw-r--  2.0 unx    68825 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476861118934859-nfe.xml
+-rw-rw-r--  2.0 unx    10834 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/42210775277525000178550030000266631762885493-procNFe.xml
+-rw-rw-r--  2.0 unx     9301 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476781421693968-nfe.xml
+-rw-rw-r--  2.0 unx    12034 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/42211275277525000178550030000276771368212013-procNFe.xml
+-rw-rw-r--  2.0 unx    11802 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/26180875335849000115550010000016871192213331-nfe.xml
+-rw-rw-r--  2.0 unx     9767 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476121675985748-nfe.xml
+-rw-rw-r--  2.0 unx    46079 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000474501597356342-nfe.xml
+-rw-rw-r--  2.0 unx     5549 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/NFe35200159594315000157550010000000012062777161.xml
+-rw-rw-r--  2.0 unx    19459 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000474281920007498-nfe.xml
+-rw-rw-r--  2.0 unx    46216 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000474641681223493-nfe.xml
+-rw-rw-r--  2.0 unx      484 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteInutNFe/41080676472349000430550010000001041671821888-ped-inu.xml
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe/bindings/v4_0/
+-rw-rw-r--  2.0 unx       15 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/bindings/__init__.py
+-rw-rw-r--  2.0 unx    30307 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/bindings/v4_0/leiaute_cons_sit_nfe_v4_00.py
+-rw-rw-r--  2.0 unx      561 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/bindings/v4_0/ret_cons_sit_nfe_v4_00.py
+-rw-rw-r--  2.0 unx      512 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/bindings/v4_0/cons_cad_v2_00.py
+-rw-rw-r--  2.0 unx     6770 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/bindings/v4_0/xmldsig_core_schema_v1_01.py
+-rw-rw-r--  2.0 unx     7598 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/bindings/v4_0/__init__.py
+-rw-rw-r--  2.0 unx      579 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/bindings/v4_0/ret_inut_nfe_v4_00.py
+-rw-rw-r--  2.0 unx      556 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/bindings/v4_0/inut_nfe_v4_00.py
+-rw-rw-r--  2.0 unx      459 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/bindings/v4_0/nfe_v4_00.py
+-rw-rw-r--  2.0 unx      567 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/bindings/v4_0/cons_reci_nfe_v4_00.py
+-rw-rw-r--  2.0 unx     2676 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/bindings/v4_0/tipos_basico_v4_00.py
+-rw-rw-r--  2.0 unx      576 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/bindings/v4_0/ret_cons_stat_serv_v4_00.py
+-rw-rw-r--  2.0 unx    16440 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/bindings/v4_0/leiaute_consulta_cadastro_v2_00.py
+-rw-rw-r--  2.0 unx      552 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/bindings/v4_0/cons_stat_serv_v4_00.py
+-rw-rw-r--  2.0 unx    13133 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/bindings/v4_0/leiaute_inut_nfe_v4_00.py
+-rw-rw-r--  2.0 unx      571 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/bindings/v4_0/cons_sit_nfe_v4_00.py
+-rw-rw-r--  2.0 unx      591 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/bindings/v4_0/ret_cons_reci_nfe_v4_00.py
+-rw-rw-r--  2.0 unx     5962 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/bindings/v4_0/leiaute_cons_stat_serv_v4_00.py
+-rw-rw-r--  2.0 unx      549 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/bindings/v4_0/envi_nfe_v4_00.py
+-rw-rw-r--  2.0 unx      467 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/bindings/v4_0/proc_nfe_v4_00.py
+-rw-rw-r--  2.0 unx      533 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/bindings/v4_0/proc_inut_nfe_v4_00.py
+-rw-rw-r--  2.0 unx      572 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/bindings/v4_0/ret_envi_nfe_v4_00.py
+-rw-rw-r--  2.0 unx   494616 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/bindings/v4_0/leiaute_nfe_v4_00.py
+-rw-rw-r--  2.0 unx      558 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/bindings/v4_0/ret_cons_cad_v2_00.py
+-rw-rw-r--  2.0 unx       26 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/ws/__init__.py
+-rw-rw-r--  2.0 unx     5164 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/ws/edoc_legacy.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-08 11:09 nfelib-2.0.5/nfelib/nfe/schemas/v4_0/
+-rw-rw-r--  2.0 unx     3902 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/schemas/v4_0/leiauteConsStatServ_v4.00.xsd
+-rw-rw-r--  2.0 unx      628 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/schemas/v4_0/retConsReciNFe_v4.00.xsd
+-rw-rw-r--  2.0 unx      595 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/schemas/v4_0/consStatServ_v4.00.xsd
+-rw-rw-r--  2.0 unx      522 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/schemas/v4_0/procNFe_v4.00.xsd
+-rw-rw-r--  2.0 unx      623 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/schemas/v4_0/retInutNFe_v4.00.xsd
+-rw-rw-r--  2.0 unx      579 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/schemas/v4_0/procInutNFe_v4.00.xsd
+-rw-rw-r--  2.0 unx      600 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/schemas/v4_0/consCad_v2.00.xsd
+-rw-rw-r--  2.0 unx    20000 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/schemas/v4_0/leiauteConsSitNFe_v4.00.xsd
+-rw-rw-r--  2.0 unx      522 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/schemas/v4_0/nfe_v4.00.xsd
+-rw-rw-r--  2.0 unx      606 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/schemas/v4_0/retConsCad_v2.00.xsd
+-rw-rw-r--  2.0 unx      610 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/schemas/v4_0/consReciNFe_v4.00.xsd
+-rw-rw-r--  2.0 unx     7801 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/schemas/v4_0/leiauteInutNFe_v4.00.xsd
+-rw-rw-r--  2.0 unx      600 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/schemas/v4_0/enviNFe_v4.00.xsd
+-rw-rw-r--  2.0 unx      606 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/schemas/v4_0/inutNFe_v4.00.xsd
+-rw-rw-r--  2.0 unx    15469 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/schemas/v4_0/leiauteConsultaCadastro_v2.00.xsd
+-rw-rw-r--  2.0 unx      617 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/schemas/v4_0/retEnviNFe_v4.00.xsd
+-rw-rw-r--  2.0 unx      568 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/schemas/v4_0/consSitNFe_v4.00.xsd
+-rw-rw-r--  2.0 unx    21976 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/schemas/v4_0/tiposBasico_v4.00.xsd
+-rw-rw-r--  2.0 unx   334026 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/schemas/v4_0/leiauteNFe_v4.00.xsd
+-rw-rw-r--  2.0 unx      604 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/schemas/v4_0/retConsStatServ_v4.00.xsd
+-rw-rw-r--  2.0 unx    32310 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/schemas/v4_0/tiposBasico_v1.03.xsd
+-rw-rw-r--  2.0 unx      602 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/schemas/v4_0/retConsSitNFe_v4.00.xsd
+-rw-rw-r--  2.0 unx     3747 b- defN 24-Apr-05 08:24 nfelib-2.0.5/nfelib/nfe/schemas/v4_0/xmldsig-core-schema_v1.01.xsd
+702 files, 10554408 bytes uncompressed, 1229836 bytes compressed:  88.4%
```

## zipnote {}

```diff
@@ -1,2344 +1,2107 @@
-Filename: nfelib-2.0.4/
+Filename: nfelib-2.0.5/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib.egg-info/
+Filename: nfelib-2.0.5/nfelib.egg-info/
 Comment: 
 
-Filename: nfelib-2.0.4/tests/
+Filename: nfelib-2.0.5/tests/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/
+Filename: nfelib-2.0.5/nfelib/
 Comment: 
 
-Filename: nfelib-2.0.4/MIT-LICENSE
+Filename: nfelib-2.0.5/MIT-LICENSE
 Comment: 
 
-Filename: nfelib-2.0.4/setup.py
+Filename: nfelib-2.0.5/setup.py
 Comment: 
 
-Filename: nfelib-2.0.4/setup.cfg
+Filename: nfelib-2.0.5/setup.cfg
 Comment: 
 
-Filename: nfelib-2.0.4/README.md
+Filename: nfelib-2.0.5/README.md
 Comment: 
 
-Filename: nfelib-2.0.4/PKG-INFO
+Filename: nfelib-2.0.5/PKG-INFO
 Comment: 
 
-Filename: nfelib-2.0.4/MANIFEST.in
+Filename: nfelib-2.0.5/MANIFEST.in
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib.egg-info/top_level.txt
+Filename: nfelib-2.0.5/nfelib.egg-info/top_level.txt
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib.egg-info/SOURCES.txt
+Filename: nfelib-2.0.5/nfelib.egg-info/SOURCES.txt
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib.egg-info/requires.txt
+Filename: nfelib-2.0.5/nfelib.egg-info/requires.txt
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib.egg-info/dependency_links.txt
+Filename: nfelib-2.0.5/nfelib.egg-info/dependency_links.txt
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib.egg-info/PKG-INFO
+Filename: nfelib-2.0.5/nfelib.egg-info/PKG-INFO
 Comment: 
 
-Filename: nfelib-2.0.4/tests/nfse/
+Filename: nfelib-2.0.5/tests/nfse/
 Comment: 
 
-Filename: nfelib-2.0.4/tests/mdfe/
+Filename: nfelib-2.0.5/tests/mdfe/
 Comment: 
 
-Filename: nfelib-2.0.4/tests/nfe_evento_cce/
+Filename: nfelib-2.0.5/tests/nfe_evento_cce/
 Comment: 
 
-Filename: nfelib-2.0.4/tests/cte/
+Filename: nfelib-2.0.5/tests/cte/
 Comment: 
 
-Filename: nfelib-2.0.4/tests/cce/
+Filename: nfelib-2.0.5/tests/cce/
 Comment: 
 
-Filename: nfelib-2.0.4/tests/nfe/
+Filename: nfelib-2.0.5/tests/nfe/
 Comment: 
 
-Filename: nfelib-2.0.4/tests/fingerprint_out.txt
+Filename: nfelib-2.0.5/tests/test_fingerprint.py
 Comment: 
 
-Filename: nfelib-2.0.4/tests/test_fingerprint.py
+Filename: nfelib-2.0.5/tests/output_nfse.xml
 Comment: 
 
-Filename: nfelib-2.0.4/tests/output_nfse.xml
+Filename: nfelib-2.0.5/tests/output_nfse_pedRegEvento.xml
 Comment: 
 
-Filename: nfelib-2.0.4/tests/output_nfse_pedRegEvento.xml
+Filename: nfelib-2.0.5/tests/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/tests/__init__.py
+Filename: nfelib-2.0.5/tests/output_nfse_dps.xml
 Comment: 
 
-Filename: nfelib-2.0.4/tests/output_nfse_dps.xml
+Filename: nfelib-2.0.5/tests/output_cte.xml
 Comment: 
 
-Filename: nfelib-2.0.4/tests/output_cte.xml
+Filename: nfelib-2.0.5/tests/fingerprint.txt
 Comment: 
 
-Filename: nfelib-2.0.4/tests/fingerprint.txt
+Filename: nfelib-2.0.5/tests/output.xml
 Comment: 
 
-Filename: nfelib-2.0.4/tests/output.xml
+Filename: nfelib-2.0.5/tests/output_nfe_evento_cce.xml
 Comment: 
 
-Filename: nfelib-2.0.4/tests/output_nfe_evento_cce.xml
+Filename: nfelib-2.0.5/tests/output_mdfe.xml
 Comment: 
 
-Filename: nfelib-2.0.4/tests/output_mdfe.xml
+Filename: nfelib-2.0.5/tests/output_nfe_inut.xml
 Comment: 
 
-Filename: nfelib-2.0.4/tests/output_nfe_inut.xml
+Filename: nfelib-2.0.5/tests/output_nfe_leiaute.xml
 Comment: 
 
-Filename: nfelib-2.0.4/tests/output_nfe_leiaute.xml
+Filename: nfelib-2.0.5/tests/input.xml
 Comment: 
 
-Filename: nfelib-2.0.4/tests/input.xml
+Filename: nfelib-2.0.5/tests/test_all.py
 Comment: 
 
-Filename: nfelib-2.0.4/tests/test_all.py
+Filename: nfelib-2.0.5/tests/nfse/test_nfse.py
 Comment: 
 
-Filename: nfelib-2.0.4/tests/nfse/test_nfse.py
+Filename: nfelib-2.0.5/tests/mdfe/test_mdfe.py
 Comment: 
 
-Filename: nfelib-2.0.4/tests/mdfe/test_mdfe.py
+Filename: nfelib-2.0.5/tests/nfe_evento_cce/test_cce.py
 Comment: 
 
-Filename: nfelib-2.0.4/tests/nfe_evento_cce/test_cce.py
+Filename: nfelib-2.0.5/tests/cte/test_cte.py
 Comment: 
 
-Filename: nfelib-2.0.4/tests/cte/test_cte.py
+Filename: nfelib-2.0.5/tests/cce/v1_00/
 Comment: 
 
-Filename: nfelib-2.0.4/tests/cce/v1_00/
+Filename: nfelib-2.0.5/tests/cce/v1_00/leiauteCCe/
 Comment: 
 
-Filename: nfelib-2.0.4/tests/cce/v1_00/leiauteCCe/
+Filename: nfelib-2.0.5/tests/cce/v1_00/leiauteCCe/35180803102452000172550010000476051695511860-01-cce.xml
 Comment: 
 
-Filename: nfelib-2.0.4/tests/cce/v1_00/leiauteCCe/35180803102452000172550010000476051695511860-01-cce.xml
+Filename: nfelib-2.0.5/tests/nfe/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/tests/nfe/__init__.py
+Filename: nfelib-2.0.5/tests/nfe/test_nfe_legacy.py
 Comment: 
 
-Filename: nfelib-2.0.4/tests/nfe/test_nfe_legacy.py
+Filename: nfelib-2.0.5/tests/nfe/test_nfe.py
 Comment: 
 
-Filename: nfelib-2.0.4/tests/nfe/test_nfe.py
+Filename: nfelib-2.0.5/nfelib/nfse/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfse/
+Filename: nfelib-2.0.5/nfelib/v4_00/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/v4_00/
+Filename: nfelib-2.0.5/nfelib/mdfe/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/
+Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_mde/
+Filename: nfelib-2.0.5/nfelib/nfe_insucesso/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_epec/
+Filename: nfelib-2.0.5/nfelib/nfe_epec/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_entrega/
+Filename: nfelib-2.0.5/nfelib/nfe_entrega/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_dist_dfe/
+Filename: nfelib-2.0.5/nfelib/nfe_dist_dfe/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_cancel/
+Filename: nfelib-2.0.5/nfelib/nfe_evento_cancel/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte_dist_dfe/
+Filename: nfelib-2.0.5/nfelib/cte_dist_dfe/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/bpe/
+Filename: nfelib-2.0.5/nfelib/bpe/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe_dist_dfe/
+Filename: nfelib-2.0.5/nfelib/mdfe_dist_dfe/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_cce/
+Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_ator_interessado/
+Filename: nfelib-2.0.5/nfelib/nfe_ator_interessado/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/
+Filename: nfelib-2.0.5/nfelib/cte/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_generico/
+Filename: nfelib-2.0.5/nfelib/nfe_evento_generico/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_cons/
+Filename: nfelib-2.0.5/nfelib/nfe_cons/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe/
+Filename: nfelib-2.0.5/nfelib/nfe/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/odoo/
+Filename: nfelib-2.0.5/nfelib/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/__init__.py
+Filename: nfelib-2.0.5/nfelib/nfse/samples/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfse/samples/
+Filename: nfelib-2.0.5/nfelib/nfse/bindings/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfse/bindings/
+Filename: nfelib-2.0.5/nfelib/nfse/schemas/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfse/schemas/
+Filename: nfelib-2.0.5/nfelib/nfse/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfse/__init__.py
+Filename: nfelib-2.0.5/nfelib/nfse/samples/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfse/samples/v1_0/
+Filename: nfelib-2.0.5/nfelib/nfse/samples/v1_0/ConsultarNFSeRPS-ped-sitnfserps.xml
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfse/samples/v1_0/ConsultarNFSeRPS-ped-sitnfserps.xml
+Filename: nfelib-2.0.5/nfelib/nfse/samples/v1_0/GerarNFSeEnvio-env-loterps.xml
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfse/samples/v1_0/GerarNFSeEnvio-env-loterps.xml
+Filename: nfelib-2.0.5/nfelib/nfse/samples/v1_0/CancelarNFSe-ped-cannfse.xml
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfse/samples/v1_0/CancelarNFSe-ped-cannfse.xml
+Filename: nfelib-2.0.5/nfelib/nfse/samples/v1_0/ConsultarNFSeEnvio-ped-sitnfse.xml
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfse/samples/v1_0/ConsultarNFSeEnvio-ped-sitnfse.xml
+Filename: nfelib-2.0.5/nfelib/nfse/bindings/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfse/bindings/v1_0/
+Filename: nfelib-2.0.5/nfelib/nfse/bindings/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfse/bindings/__init__.py
+Filename: nfelib-2.0.5/nfelib/nfse/bindings/v1_0/ped_reg_evento_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfse/bindings/v1_0/ped_reg_evento_v1_00.py
+Filename: nfelib-2.0.5/nfelib/nfse/bindings/v1_0/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfse/bindings/v1_0/__init__.py
+Filename: nfelib-2.0.5/nfelib/nfse/bindings/v1_0/tipos_eventos_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfse/bindings/v1_0/tipos_eventos_v1_00.py
+Filename: nfelib-2.0.5/nfelib/nfse/bindings/v1_0/nfse_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfse/bindings/v1_0/nfse_v1_00.py
+Filename: nfelib-2.0.5/nfelib/nfse/bindings/v1_0/tipos_complexos_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfse/bindings/v1_0/tipos_complexos_v1_00.py
+Filename: nfelib-2.0.5/nfelib/nfse/bindings/v1_0/dps_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfse/bindings/v1_0/dps_v1_00.py
+Filename: nfelib-2.0.5/nfelib/nfse/bindings/v1_0/tipos_simples_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfse/bindings/v1_0/tipos_simples_v1_00.py
+Filename: nfelib-2.0.5/nfelib/nfse/bindings/v1_0/xmldsig_core_schema_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfse/bindings/v1_0/xmldsig_core_schema_v1_00.py
+Filename: nfelib-2.0.5/nfelib/nfse/bindings/v1_0/evento_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfse/bindings/v1_0/evento_v1_00.py
+Filename: nfelib-2.0.5/nfelib/nfse/schemas/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfse/schemas/v1_0/
+Filename: nfelib-2.0.5/nfelib/nfse/schemas/v1_0/tiposEventos_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfse/schemas/v1_0/tiposEventos_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfse/schemas/v1_0/NFSe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfse/schemas/v1_0/NFSe_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfse/schemas/v1_0/pedRegEvento_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfse/schemas/v1_0/pedRegEvento_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfse/schemas/v1_0/tiposComplexos_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfse/schemas/v1_0/tiposComplexos_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfse/schemas/v1_0/DPS_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfse/schemas/v1_0/DPS_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfse/schemas/v1_0/xmldsig-core-schema_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfse/schemas/v1_0/xmldsig-core-schema_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfse/schemas/v1_0/tiposSimples_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfse/schemas/v1_0/tiposSimples_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfse/schemas/v1_0/evento_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfse/schemas/v1_0/evento_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/v4_00/retConsStatServ.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/v4_00/retConsStatServ.py
+Filename: nfelib-2.0.5/nfelib/v4_00/retEnviNFe.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/v4_00/retEnviNFe.py
+Filename: nfelib-2.0.5/nfelib/v4_00/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/v4_00/__init__.py
+Filename: nfelib-2.0.5/nfelib/v4_00/README.txt
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/v4_00/README.txt
+Filename: nfelib-2.0.5/nfelib/v4_00/retEnvConfRecebto.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/v4_00/retEnvConfRecebto.py
+Filename: nfelib-2.0.5/nfelib/v4_00/retEnvEvento.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/v4_00/retEnvEvento.py
+Filename: nfelib-2.0.5/nfelib/v4_00/leiauteNFe_sub.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/v4_00/leiauteNFe_sub.py
+Filename: nfelib-2.0.5/nfelib/v4_00/retInutNFe.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/v4_00/retInutNFe.py
+Filename: nfelib-2.0.5/nfelib/v4_00/retConsCad.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/v4_00/retConsCad.py
+Filename: nfelib-2.0.5/nfelib/v4_00/distDFeInt.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/v4_00/distDFeInt.py
+Filename: nfelib-2.0.5/nfelib/v4_00/retDistDFeInt.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/v4_00/retDistDFeInt.py
+Filename: nfelib-2.0.5/nfelib/v4_00/retConsReciNFe.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/v4_00/retConsReciNFe.py
+Filename: nfelib-2.0.5/nfelib/v4_00/retEnvCCe.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/v4_00/retEnvCCe.py
+Filename: nfelib-2.0.5/nfelib/v4_00/retEnvEventoCancNFe.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/v4_00/retEnvEventoCancNFe.py
+Filename: nfelib-2.0.5/nfelib/v4_00/retConsSitNFe.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/v4_00/retConsSitNFe.py
+Filename: nfelib-2.0.5/nfelib/mdfe/samples/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/samples/
+Filename: nfelib-2.0.5/nfelib/mdfe/bindings/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/bindings/
+Filename: nfelib-2.0.5/nfelib/mdfe/schemas/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/schemas/
+Filename: nfelib-2.0.5/nfelib/mdfe/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/odoo/
+Filename: nfelib-2.0.5/nfelib/mdfe/samples/v3_0/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/__init__.py
+Filename: nfelib-2.0.5/nfelib/mdfe/samples/v3_0/inclusaoDFe1101154119060611747300015058001000000001111700344401-ped-eve.xml
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/samples/v3_0/
+Filename: nfelib-2.0.5/nfelib/mdfe/samples/v3_0/pagamentoOperacao1101103511031029073900013955001000000001105112804101-ped-eve.xml
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/samples/v3_0/inclusaoDFe1101154119060611747300015058001000000001111700344401-ped-eve.xml
+Filename: nfelib-2.0.5/nfelib/mdfe/samples/v3_0/PagamentoOperacaoMDFe_1101164120039999999999999958001000000999999999999901-ped-eve.xml
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/samples/v3_0/pagamentoOperacao1101103511031029073900013955001000000001105112804101-ped-eve.xml
+Filename: nfelib-2.0.5/nfelib/mdfe/samples/v3_0/26999999999999999999999999999999999999999991-mdfe.xml
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/samples/v3_0/PagamentoOperacaoMDFe_1101164120039999999999999958001000000999999999999901-ped-eve.xml
+Filename: nfelib-2.0.5/nfelib/mdfe/samples/v3_0/41190876676436000167580010000500001000437558-mdfe.xml
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/samples/v3_0/26999999999999999999999999999999999999999991-mdfe.xml
+Filename: nfelib-2.0.5/nfelib/mdfe/samples/v3_0/50170876063965000276580010000011311421039568-mdfe.xml
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/samples/v3_0/41190876676436000167580010000500001000437558-mdfe.xml
+Filename: nfelib-2.0.5/nfelib/mdfe/samples/v3_0/ComPagtoPIX_41210780568835000181580010402005751006005791-procMDFe.xml
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/samples/v3_0/50170876063965000276580010000011311421039568-mdfe.xml
+Filename: nfelib-2.0.5/nfelib/mdfe/samples/v3_0/310000007934162-ped-rec.xml
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/samples/v3_0/ComPagtoPIX_41210780568835000181580010402005751006005791-procMDFe.xml
+Filename: nfelib-2.0.5/nfelib/mdfe/samples/v3_0/cancelameto1101103511031029073900013955001000000001105112804101-ped-eve.xml
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/samples/v3_0/310000007934162-ped-rec.xml
+Filename: nfelib-2.0.5/nfelib/mdfe/samples/v3_0/encerramento1101123511031029073900013955001000000001105112804101-ped-eve.xml
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/samples/v3_0/cancelameto1101103511031029073900013955001000000001105112804101-ped-eve.xml
+Filename: nfelib-2.0.5/nfelib/mdfe/samples/v3_0/inclusaocondutor31131223864838000129580000000000051003000003-ped-eve.xml
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/samples/v3_0/encerramento1101123511031029073900013955001000000001105112804101-ped-eve.xml
+Filename: nfelib-2.0.5/nfelib/mdfe/samples/v3_0/01010101010-ped-cons-mdfe-naoenc.xml
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/samples/v3_0/inclusaocondutor31131223864838000129580000000000051003000003-ped-eve.xml
+Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/samples/v3_0/01010101010-ped-cons-mdfe-naoenc.xml
+Filename: nfelib-2.0.5/nfelib/mdfe/bindings/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/
+Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ret_cons_stat_serv_mdfe_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/bindings/__init__.py
+Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/xmldsig_core_schema_v1_01.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/ret_cons_stat_serv_mdfe_v3_00.py
+Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/cons_stat_serv_tipos_basico_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/xmldsig_core_schema_v1_01.py
+Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/cons_stat_serv_tipos_basico_v3_00.py
+Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/proc_evento_mdfe_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/__init__.py
+Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/cons_sit_mdfe_tipos_basico_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/proc_evento_mdfe_v3_00.py
+Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/mdfe_consulta_dfe_tipos_basico_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/cons_sit_mdfe_tipos_basico_v3_00.py
+Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ret_evento_mdfe_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/mdfe_consulta_dfe_tipos_basico_v3_00.py
+Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/leiaute_dist_mdfe_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/ret_evento_mdfe_v3_00.py
+Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/mdfe_consulta_dfe_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/leiaute_dist_mdfe_v3_00.py
+Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ev_pagto_oper_mdfe_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/mdfe_consulta_dfe_v3_00.py
+Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ret_mdfe_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/ev_pagto_oper_mdfe_v3_00.py
+Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ev_inc_condutor_mdfe_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/ret_mdfe_v3_00.py
+Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/tipos_geral_mdfe_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/ev_inc_condutor_mdfe_v3_00.py
+Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ret_cons_sit_mdfe_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/tipos_geral_mdfe_v3_00.py
+Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ret_cons_reci_mdfe_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/ret_cons_sit_mdfe_v3_00.py
+Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ret_envi_mdfe_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/ret_cons_reci_mdfe_v3_00.py
+Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/envi_mdfe_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/ret_envi_mdfe_v3_00.py
+Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/cons_mdfe_nao_enc_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/envi_mdfe_v3_00.py
+Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/cons_mdfe_nao_enc_tipos_basico_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/cons_mdfe_nao_enc_v3_00.py
+Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ret_dist_mdfe_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/cons_mdfe_nao_enc_tipos_basico_v3_00.py
+Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/evento_mdfe_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/ret_dist_mdfe_v3_00.py
+Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/mdfe_modal_rodoviario_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/evento_mdfe_v3_00.py
+Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/evento_mdfe_tipos_basico_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/mdfe_modal_rodoviario_v3_00.py
+Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ev_canc_mdfe_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/evento_mdfe_tipos_basico_v3_00.py
+Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/mdfe_modal_aquaviario_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/ev_canc_mdfe_v3_00.py
+Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ret_cons_mdfe_nao_enc_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/mdfe_modal_aquaviario_v3_00.py
+Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ret_mdfe_consulta_dfe_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/ret_cons_mdfe_nao_enc_v3_00.py
+Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/dist_mdfe_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/ret_mdfe_consulta_dfe_v3_00.py
+Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/cons_reci_mdfe_tipos_basico_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/dist_mdfe_v3_00.py
+Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/mdfe_modal_ferroviario_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/cons_reci_mdfe_tipos_basico_v3_00.py
+Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ev_inclusao_dfe_mdfe_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/mdfe_modal_ferroviario_v3_00.py
+Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/cons_sit_mdfe_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/ev_inclusao_dfe_mdfe_v3_00.py
+Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/mdfe_tipos_basico_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/cons_sit_mdfe_v3_00.py
+Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/mdfe_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/mdfe_tipos_basico_v3_00.py
+Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ev_enc_mdfe_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/mdfe_v3_00.py
+Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/mdfe_modal_aereo_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/ev_enc_mdfe_v3_00.py
+Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/cons_reci_mdfe_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/mdfe_modal_aereo_v3_00.py
+Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/proc_mdfe_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/cons_reci_mdfe_v3_00.py
+Filename: nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/cons_stat_serv_mdfe_v3_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/proc_mdfe_v3_00.py
+Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/cons_stat_serv_mdfe_v3_00.py
+Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/consReciMDFeTiposBasico_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/
+Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retConsReciMDFe_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/consReciMDFeTiposBasico_v3.00.xsd
+Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retConsMDFeNaoEnc_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/retConsReciMDFe_v3.00.xsd
+Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/consStatServMDFe_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/retConsMDFeNaoEnc_v3.00.xsd
+Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/evIncCondutorMDFe_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/consStatServMDFe_v3.00.xsd
+Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/consStatServTiposBasico_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/evIncCondutorMDFe_v3.00.xsd
+Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retMDFe_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/consStatServTiposBasico_v3.00.xsd
+Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/mdfeModalRodoviario_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/retMDFe_v3.00.xsd
+Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/evCancMDFe_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/mdfeModalRodoviario_v3.00.xsd
+Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/distMDFe_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/evCancMDFe_v3.00.xsd
+Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retMDFeConsultaDFe_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/distMDFe_v3.00.xsd
+Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/mdfeModalAereo_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/retMDFeConsultaDFe_v3.00.xsd
+Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/mdfeModalFerroviario_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/mdfeModalAereo_v3.00.xsd
+Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/eventoMDFe_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/mdfeModalFerroviario_v3.00.xsd
+Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retConsStatServMDFe_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/eventoMDFe_v3.00.xsd
+Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/evPagtoOperMDFe_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/retConsStatServMDFe_v3.00.xsd
+Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retEventoMDFe_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/evPagtoOperMDFe_v3.00.xsd
+Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/consReciMDFe_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/retEventoMDFe_v3.00.xsd
+Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/mdfeConsultaDFe_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/consReciMDFe_v3.00.xsd
+Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/consMDFeNaoEnc_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/mdfeConsultaDFe_v3.00.xsd
+Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/procMDFe_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/consMDFeNaoEnc_v3.00.xsd
+Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/enviMDFe_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/procMDFe_v3.00.xsd
+Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/evInclusaoDFeMDFe_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/enviMDFe_v3.00.xsd
+Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/tiposGeralMDFe_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/evInclusaoDFeMDFe_v3.00.xsd
+Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/mdfeConsultaDFeTiposBasico_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/tiposGeralMDFe_v3.00.xsd
+Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/mdfeTiposBasico_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/mdfeConsultaDFeTiposBasico_v3.00.xsd
+Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/mdfeModalAquaviario_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/mdfeTiposBasico_v3.00.xsd
+Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/mdfe_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/mdfeModalAquaviario_v3.00.xsd
+Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retEnviMDFe_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/mdfe_v3.00.xsd
+Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/consSitMDFe_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/retEnviMDFe_v3.00.xsd
+Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/consSitMDFeTiposBasico_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/consSitMDFe_v3.00.xsd
+Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retConsMDFeNaoEnc_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/consSitMDFeTiposBasico_v3.00.xsd
+Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/leiauteDistMDFe_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/retConsMDFeNaoEnc_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/consMDFeNaoEncTiposBasico_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/leiauteDistMDFe_v3.00.xsd
+Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/xmldsig-core-schema_v1.01.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/consMDFeNaoEncTiposBasico_v3.00.xsd
+Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/eventoMDFeTiposBasico_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/xmldsig-core-schema_v1.01.xsd
+Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/procEventoMDFe_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/eventoMDFeTiposBasico_v3.00.xsd
+Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retDistMDFe_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/procEventoMDFe_v3.00.xsd
+Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retConsSitMDFe_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/retDistMDFe_v3.00.xsd
+Filename: nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/evEncMDFe_v3.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/retConsSitMDFe_v3.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/evEncMDFe_v3.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/
+Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/odoo/__init__.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/ret_cons_stat_serv_mdfe_v3_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/cons_stat_serv_tipos_basico_v3_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/proc_conf_recebto_nfe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/proc_evento_mdfe_v3_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/xmldsig_core_schema_v1_01.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/cons_sit_mdfe_tipos_basico_v3_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/tipos_basico_v1_03.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/mdfe_consulta_dfe_tipos_basico_v3_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/ret_evento_mdfe_v3_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/e210240_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/leiaute_dist_mdfe_v3_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/leiaute_conf_recebto_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/mdfe_consulta_dfe_v3_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/conf_recebto_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/ev_pagto_oper_mdfe_v3_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/ret_env_conf_recebto_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/ret_mdfe_v3_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/env_conf_recebto_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/ev_inc_condutor_mdfe_v3_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/tipos_geral_mdfe_v3_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/leiauteConfRecebto_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/ret_cons_sit_mdfe_v3_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/procConfRecebtoNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/ret_cons_reci_mdfe_v3_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/e210220_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/ret_envi_mdfe_v3_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/e210200_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/envi_mdfe_v3_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/e210240_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/cons_mdfe_nao_enc_v3_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/envConfRecebto_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/cons_mdfe_nao_enc_tipos_basico_v3_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/e210210_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/ret_dist_mdfe_v3_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/confRecebto_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/evento_mdfe_v3_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/tiposBasico_v1.03.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/mdfe_modal_rodoviario_v3_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/retEnvConfRecebto_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/evento_mdfe_tipos_basico_v3_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/ev_canc_mdfe_v3_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_insucesso/bindings/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/mdfe_modal_aquaviario_v3_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_insucesso/schemas/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/ret_cons_mdfe_nao_enc_v3_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_insucesso/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/ret_mdfe_consulta_dfe_v3_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/dist_mdfe_v3_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_insucesso/bindings/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/cons_reci_mdfe_tipos_basico_v3_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/tmp0000.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/mdfe_modal_ferroviario_v3_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/xmldsig_core_schema_v1_01.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/ev_inclusao_dfe_mdfe_v3_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/tipos_basico_v1_03.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/cons_sit_mdfe_v3_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/mdfe_tipos_basico_v3_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/ret_evento_insucesso_nfe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/mdfe_v3_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/env_evento_insucesso_nfe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/ev_enc_mdfe_v3_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/evento_insucesso_nfe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/mdfe_modal_aereo_v3_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/leiaute_evento_insucesso_nfe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/cons_reci_mdfe_v3_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/proc_evento_insucesso_nfe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/proc_mdfe_v3_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe/odoo/v3_0/cons_stat_serv_mdfe_v3_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/envEventoInsucessoNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_mde/bindings/
+Filename: nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/tmp0000.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_mde/schemas/
+Filename: nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/e110192_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_mde/__init__.py
+Filename: nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/retEventoCancInsucessoNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_mde/bindings/v1_0/
+Filename: nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/procEventoInsucessoNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_mde/bindings/__init__.py
+Filename: nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/leiauteEventoCancInsucessoNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_mde/bindings/v1_0/proc_conf_recebto_nfe_v1_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/EventoInsucessoNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_mde/bindings/v1_0/xmldsig_core_schema_v1_01.py
+Filename: nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/retEventoInsucessoNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_mde/bindings/v1_0/tipos_basico_v1_03.py
+Filename: nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/leiauteEventoInsucessoNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_mde/bindings/v1_0/__init__.py
+Filename: nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/e110193_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_mde/bindings/v1_0/e210240_v1_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/EventoCancInsucessoNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_mde/bindings/v1_0/leiaute_conf_recebto_v1_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/tiposBasico_v1.03.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_mde/bindings/v1_0/conf_recebto_v1_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_mde/bindings/v1_0/ret_env_conf_recebto_v1_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/procEventoCancInsucessoNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_mde/bindings/v1_0/env_conf_recebto_v1_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/envEventoCancInsucessoNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_mde/schemas/v1_0/
+Filename: nfelib-2.0.5/nfelib/nfe_epec/bindings/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_mde/schemas/v1_0/leiauteConfRecebto_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_epec/schemas/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_mde/schemas/v1_0/procConfRecebtoNFe_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_epec/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_mde/schemas/v1_0/e210220_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_epec/bindings/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_mde/schemas/v1_0/e210200_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_epec/bindings/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_mde/schemas/v1_0/e210240_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_epec/bindings/v1_0/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_mde/schemas/v1_0/envConfRecebto_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_epec/bindings/v1_0/e110140_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_mde/schemas/v1_0/e210210_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_epec/bindings/v1_0/leiaute_epec_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_mde/schemas/v1_0/confRecebto_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_epec/schemas/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_mde/schemas/v1_0/tiposBasico_v1.03.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_epec/schemas/v1_0/EPEC_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_mde/schemas/v1_0/retEnvConfRecebto_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_epec/schemas/v1_0/e110140_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_mde/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_epec/schemas/v1_0/envEPEC_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_epec/bindings/
+Filename: nfelib-2.0.5/nfelib/nfe_epec/schemas/v1_0/procEPEC_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_epec/schemas/
+Filename: nfelib-2.0.5/nfelib/nfe_epec/schemas/v1_0/leiauteEPEC_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_epec/__init__.py
+Filename: nfelib-2.0.5/nfelib/nfe_epec/schemas/v1_0/tiposBasico_v1.03.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_epec/bindings/v1_0/
+Filename: nfelib-2.0.5/nfelib/nfe_epec/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_epec/bindings/__init__.py
+Filename: nfelib-2.0.5/nfelib/nfe_epec/schemas/v1_0/retEnvEPEC_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_epec/bindings/v1_0/__init__.py
+Filename: nfelib-2.0.5/nfelib/nfe_entrega/bindings/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_epec/bindings/v1_0/e110140_v1_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_entrega/schemas/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_epec/bindings/v1_0/leiaute_epec_v1_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_entrega/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_epec/schemas/v1_0/
+Filename: nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_epec/schemas/v1_0/EPEC_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_entrega/bindings/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_epec/schemas/v1_0/e110140_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/xmldsig_core_schema_v1_01.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_epec/schemas/v1_0/envEPEC_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/tipos_basico_v1_03.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_epec/schemas/v1_0/procEPEC_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_epec/schemas/v1_0/leiauteEPEC_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/evento_entrega_nfe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_epec/schemas/v1_0/tiposBasico_v1.03.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/proc_evento_entrega_nfe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_epec/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/ret_evento_entrega_nfe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_epec/schemas/v1_0/retEnvEPEC_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/leiaute_evento_entrega_nfe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_entrega/bindings/
+Filename: nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/env_evento_entrega_nfe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_entrega/schemas/
+Filename: nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/e110130_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_entrega/__init__.py
+Filename: nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_entrega/bindings/v1_0/
+Filename: nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/envEventoCancEntregaNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_entrega/bindings/__init__.py
+Filename: nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/procEventoEntregaNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_entrega/bindings/v1_0/xmldsig_core_schema_v1_01.py
+Filename: nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/EventoCancEntregaNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_entrega/bindings/v1_0/tipos_basico_v1_03.py
+Filename: nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/retEventoCancEntregaNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_entrega/bindings/v1_0/__init__.py
+Filename: nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/EventoEntregaNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_entrega/bindings/v1_0/evento_entrega_nfe_v1_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/e110130_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_entrega/bindings/v1_0/proc_evento_entrega_nfe_v1_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/leiauteEventoCancEntregaNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_entrega/bindings/v1_0/ret_evento_entrega_nfe_v1_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/leiauteEventoEntregaNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_entrega/bindings/v1_0/leiaute_evento_entrega_nfe_v1_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/envEventoEntregaNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_entrega/bindings/v1_0/env_evento_entrega_nfe_v1_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/tiposBasico_v1.03.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_entrega/bindings/v1_0/e110130_v1_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/retEventoEntregaNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_entrega/schemas/v1_0/
+Filename: nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_entrega/schemas/v1_0/envEventoCancEntregaNFe_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/e110131_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_entrega/schemas/v1_0/procEventoEntregaNFe_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/procEventoCancEntregaNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_entrega/schemas/v1_0/EventoCancEntregaNFe_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_entrega/schemas/v1_0/retEventoCancEntregaNFe_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_dist_dfe/schemas/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_entrega/schemas/v1_0/EventoEntregaNFe_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_dist_dfe/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_entrega/schemas/v1_0/e110130_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_entrega/schemas/v1_0/leiauteEventoCancEntregaNFe_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_entrega/schemas/v1_0/leiauteEventoEntregaNFe_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/v1_0/res_evento_v1_01.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_entrega/schemas/v1_0/envEventoEntregaNFe_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/v1_0/xmldsig_core_schema_v1_01.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_entrega/schemas/v1_0/tiposBasico_v1.03.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/v1_0/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_entrega/schemas/v1_0/retEventoEntregaNFe_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/v1_0/ret_dist_dfe_int_v1_01.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_entrega/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/v1_0/res_nfe_v1_01.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_entrega/schemas/v1_0/e110131_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/v1_0/dist_dfe_int_v1_01.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_entrega/schemas/v1_0/procEventoCancEntregaNFe_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/v1_0/tipos_dist_dfe_v1_01.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_dist_dfe/bindings/
+Filename: nfelib-2.0.5/nfelib/nfe_dist_dfe/schemas/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_dist_dfe/schemas/
+Filename: nfelib-2.0.5/nfelib/nfe_dist_dfe/schemas/v1_0/retDistDFeInt_v1.01.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_dist_dfe/__init__.py
+Filename: nfelib-2.0.5/nfelib/nfe_dist_dfe/schemas/v1_0/tiposDistDFe_v1.01.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_dist_dfe/bindings/v1_0/
+Filename: nfelib-2.0.5/nfelib/nfe_dist_dfe/schemas/v1_0/distDFeInt_v1.01.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_dist_dfe/bindings/__init__.py
+Filename: nfelib-2.0.5/nfelib/nfe_dist_dfe/schemas/v1_0/resEvento_v1.01.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_dist_dfe/bindings/v1_0/res_evento_v1_01.py
+Filename: nfelib-2.0.5/nfelib/nfe_dist_dfe/schemas/v1_0/resNFe_v1.01.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_dist_dfe/bindings/v1_0/xmldsig_core_schema_v1_01.py
+Filename: nfelib-2.0.5/nfelib/nfe_dist_dfe/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_dist_dfe/bindings/v1_0/__init__.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_dist_dfe/bindings/v1_0/ret_dist_dfe_int_v1_01.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_dist_dfe/bindings/v1_0/res_nfe_v1_01.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_cancel/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_dist_dfe/bindings/v1_0/dist_dfe_int_v1_01.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_dist_dfe/bindings/v1_0/tipos_dist_dfe_v1_01.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_dist_dfe/schemas/v1_0/
+Filename: nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/e110111_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_dist_dfe/schemas/v1_0/retDistDFeInt_v1.01.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/ret_env_evento_canc_nfe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_dist_dfe/schemas/v1_0/tiposDistDFe_v1.01.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/xmldsig_core_schema_v1_01.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_dist_dfe/schemas/v1_0/distDFeInt_v1.01.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/tipos_basico_v1_03.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_dist_dfe/schemas/v1_0/resEvento_v1.01.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_dist_dfe/schemas/v1_0/resNFe_v1.01.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/env_evento_canc_nfe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_dist_dfe/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/proc_evento_canc_nfe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_cancel/bindings/
+Filename: nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/leiaute_evento_canc_nfe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_cancel/schemas/
+Filename: nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/evento_canc_nfe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_cancel/__init__.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_cancel/bindings/v1_0/
+Filename: nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/v1_0/envEventoCancNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_cancel/bindings/__init__.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/v1_0/eventoCancNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_cancel/bindings/v1_0/e110111_v1_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/v1_0/leiauteEventoCancNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_cancel/bindings/v1_0/ret_env_evento_canc_nfe_v1_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/v1_0/e110111_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_cancel/bindings/v1_0/xmldsig_core_schema_v1_01.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/v1_0/procEventoCancNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_cancel/bindings/v1_0/tipos_basico_v1_03.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/v1_0/retEnvEventoCancNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_cancel/bindings/v1_0/__init__.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/v1_0/tiposBasico_v1.03.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_cancel/bindings/v1_0/env_evento_canc_nfe_v1_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_cancel/bindings/v1_0/proc_evento_canc_nfe_v1_00.py
+Filename: nfelib-2.0.5/nfelib/cte_dist_dfe/bindings/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_cancel/bindings/v1_0/leiaute_evento_canc_nfe_v1_00.py
+Filename: nfelib-2.0.5/nfelib/cte_dist_dfe/schemas/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_cancel/bindings/v1_0/evento_canc_nfe_v1_00.py
+Filename: nfelib-2.0.5/nfelib/cte_dist_dfe/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_cancel/schemas/v1_0/
+Filename: nfelib-2.0.5/nfelib/cte_dist_dfe/bindings/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_cancel/schemas/v1_0/envEventoCancNFe_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/cte_dist_dfe/bindings/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_cancel/schemas/v1_0/eventoCancNFe_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/cte_dist_dfe/bindings/v1_0/dist_dfe_int_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_cancel/schemas/v1_0/leiauteEventoCancNFe_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/cte_dist_dfe/bindings/v1_0/xmldsig_core_schema_v1_01.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_cancel/schemas/v1_0/e110111_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/cte_dist_dfe/bindings/v1_0/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_cancel/schemas/v1_0/procEventoCancNFe_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/cte_dist_dfe/bindings/v1_0/tipos_dist_dfe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_cancel/schemas/v1_0/retEnvEventoCancNFe_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/cte_dist_dfe/bindings/v1_0/ret_dist_dfe_int_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_cancel/schemas/v1_0/tiposBasico_v1.03.xsd
+Filename: nfelib-2.0.5/nfelib/cte_dist_dfe/schemas/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_cancel/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
+Filename: nfelib-2.0.5/nfelib/cte_dist_dfe/schemas/v1_0/distDFeInt_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte_dist_dfe/bindings/
+Filename: nfelib-2.0.5/nfelib/cte_dist_dfe/schemas/v1_0/retDistDFeInt_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte_dist_dfe/schemas/
+Filename: nfelib-2.0.5/nfelib/cte_dist_dfe/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte_dist_dfe/__init__.py
+Filename: nfelib-2.0.5/nfelib/cte_dist_dfe/schemas/v1_0/tiposDistDFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte_dist_dfe/bindings/v1_0/
+Filename: nfelib-2.0.5/nfelib/bpe/bindings/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte_dist_dfe/bindings/__init__.py
+Filename: nfelib-2.0.5/nfelib/bpe/schemas/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte_dist_dfe/bindings/v1_0/dist_dfe_int_v1_00.py
+Filename: nfelib-2.0.5/nfelib/bpe/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte_dist_dfe/bindings/v1_0/xmldsig_core_schema_v1_01.py
+Filename: nfelib-2.0.5/nfelib/bpe/bindings/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte_dist_dfe/bindings/v1_0/__init__.py
+Filename: nfelib-2.0.5/nfelib/bpe/bindings/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte_dist_dfe/bindings/v1_0/tipos_dist_dfe_v1_00.py
+Filename: nfelib-2.0.5/nfelib/bpe/bindings/v1_0/cons_sit_bpe_tipos_basico_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte_dist_dfe/bindings/v1_0/ret_dist_dfe_int_v1_00.py
+Filename: nfelib-2.0.5/nfelib/bpe/bindings/v1_0/xmldsig_core_schema_v1_01.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte_dist_dfe/schemas/v1_0/
+Filename: nfelib-2.0.5/nfelib/bpe/bindings/v1_0/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte_dist_dfe/schemas/v1_0/distDFeInt_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/bpe/bindings/v1_0/cons_stat_serv_bpe_tipos_basico_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte_dist_dfe/schemas/v1_0/retDistDFeInt_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/bpe/bindings/v1_0/ev_nao_emb_bpe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte_dist_dfe/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
+Filename: nfelib-2.0.5/nfelib/bpe/bindings/v1_0/ev_alteracao_poltrona_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte_dist_dfe/schemas/v1_0/tiposDistDFe_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/bpe/bindings/v1_0/evento_bpe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/bpe/bindings/
+Filename: nfelib-2.0.5/nfelib/bpe/bindings/v1_0/tipos_geral_bpe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/bpe/schemas/
+Filename: nfelib-2.0.5/nfelib/bpe/bindings/v1_0/bpe_tm_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/bpe/__init__.py
+Filename: nfelib-2.0.5/nfelib/bpe/bindings/v1_0/proc_evento_bpe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/bpe/bindings/v1_0/
+Filename: nfelib-2.0.5/nfelib/bpe/bindings/v1_0/ret_evento_bpe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/bpe/bindings/__init__.py
+Filename: nfelib-2.0.5/nfelib/bpe/bindings/v1_0/cons_stat_serv_bpe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/bpe/bindings/v1_0/cons_sit_bpe_tipos_basico_v1_00.py
+Filename: nfelib-2.0.5/nfelib/bpe/bindings/v1_0/bpe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/bpe/bindings/v1_0/xmldsig_core_schema_v1_01.py
+Filename: nfelib-2.0.5/nfelib/bpe/bindings/v1_0/ret_cons_sit_bpe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/bpe/bindings/v1_0/__init__.py
+Filename: nfelib-2.0.5/nfelib/bpe/bindings/v1_0/cons_sit_bpe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/bpe/bindings/v1_0/cons_stat_serv_bpe_tipos_basico_v1_00.py
+Filename: nfelib-2.0.5/nfelib/bpe/bindings/v1_0/proc_bpe_tm_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/bpe/bindings/v1_0/ev_nao_emb_bpe_v1_00.py
+Filename: nfelib-2.0.5/nfelib/bpe/bindings/v1_0/evento_bpe_tipos_basico_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/bpe/bindings/v1_0/ev_alteracao_poltrona_v1_00.py
+Filename: nfelib-2.0.5/nfelib/bpe/bindings/v1_0/ret_bpe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/bpe/bindings/v1_0/evento_bpe_v1_00.py
+Filename: nfelib-2.0.5/nfelib/bpe/bindings/v1_0/ev_excesso_bagagem_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/bpe/bindings/v1_0/tipos_geral_bpe_v1_00.py
+Filename: nfelib-2.0.5/nfelib/bpe/bindings/v1_0/ret_cons_stat_serv_bpe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/bpe/bindings/v1_0/bpe_tm_v1_00.py
+Filename: nfelib-2.0.5/nfelib/bpe/bindings/v1_0/ev_canc_bpe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/bpe/bindings/v1_0/proc_evento_bpe_v1_00.py
+Filename: nfelib-2.0.5/nfelib/bpe/bindings/v1_0/proc_bpe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/bpe/bindings/v1_0/ret_evento_bpe_v1_00.py
+Filename: nfelib-2.0.5/nfelib/bpe/bindings/v1_0/bpe_tipos_basico_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/bpe/bindings/v1_0/cons_stat_serv_bpe_v1_00.py
+Filename: nfelib-2.0.5/nfelib/bpe/schemas/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/bpe/bindings/v1_0/bpe_v1_00.py
+Filename: nfelib-2.0.5/nfelib/bpe/schemas/v1_0/eventoBPe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/bpe/bindings/v1_0/ret_cons_sit_bpe_v1_00.py
+Filename: nfelib-2.0.5/nfelib/bpe/schemas/v1_0/consStatServBPe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/bpe/bindings/v1_0/cons_sit_bpe_v1_00.py
+Filename: nfelib-2.0.5/nfelib/bpe/schemas/v1_0/bpeTiposBasico_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/bpe/bindings/v1_0/proc_bpe_tm_v1_00.py
+Filename: nfelib-2.0.5/nfelib/bpe/schemas/v1_0/retEventoBPe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/bpe/bindings/v1_0/evento_bpe_tipos_basico_v1_00.py
+Filename: nfelib-2.0.5/nfelib/bpe/schemas/v1_0/tiposGeralBPe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/bpe/bindings/v1_0/ret_bpe_v1_00.py
+Filename: nfelib-2.0.5/nfelib/bpe/schemas/v1_0/evCancBPe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/bpe/bindings/v1_0/ev_excesso_bagagem_v1_00.py
+Filename: nfelib-2.0.5/nfelib/bpe/schemas/v1_0/evNaoEmbBPe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/bpe/bindings/v1_0/ret_cons_stat_serv_bpe_v1_00.py
+Filename: nfelib-2.0.5/nfelib/bpe/schemas/v1_0/retConsSitBPe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/bpe/bindings/v1_0/ev_canc_bpe_v1_00.py
+Filename: nfelib-2.0.5/nfelib/bpe/schemas/v1_0/bpe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/bpe/bindings/v1_0/proc_bpe_v1_00.py
+Filename: nfelib-2.0.5/nfelib/bpe/schemas/v1_0/evExcessoBagagem_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/bpe/bindings/v1_0/bpe_tipos_basico_v1_00.py
+Filename: nfelib-2.0.5/nfelib/bpe/schemas/v1_0/retBPe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/bpe/schemas/v1_0/
+Filename: nfelib-2.0.5/nfelib/bpe/schemas/v1_0/eventoBPeTiposBasico_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/bpe/schemas/v1_0/eventoBPe_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/bpe/schemas/v1_0/procBPe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/bpe/schemas/v1_0/consStatServBPe_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/bpe/schemas/v1_0/procBPeTM_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/bpe/schemas/v1_0/bpeTiposBasico_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/bpe/schemas/v1_0/retConsStatServBPe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/bpe/schemas/v1_0/retEventoBPe_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/bpe/schemas/v1_0/evAlteracaoPoltrona_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/bpe/schemas/v1_0/tiposGeralBPe_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/bpe/schemas/v1_0/consSitBPeTiposBasico_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/bpe/schemas/v1_0/evCancBPe_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/bpe/schemas/v1_0/bpeTM_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/bpe/schemas/v1_0/evNaoEmbBPe_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/bpe/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/bpe/schemas/v1_0/retConsSitBPe_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/bpe/schemas/v1_0/procEventoBPe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/bpe/schemas/v1_0/bpe_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/bpe/schemas/v1_0/consSitBPe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/bpe/schemas/v1_0/evExcessoBagagem_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/bpe/schemas/v1_0/consStatServBPeTiposBasico_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/bpe/schemas/v1_0/retBPe_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/mdfe_dist_dfe/bindings/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/bpe/schemas/v1_0/eventoBPeTiposBasico_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/mdfe_dist_dfe/schemas/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/bpe/schemas/v1_0/procBPe_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/mdfe_dist_dfe/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/bpe/schemas/v1_0/procBPeTM_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/mdfe_dist_dfe/bindings/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/bpe/schemas/v1_0/retConsStatServBPe_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/mdfe_dist_dfe/bindings/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/bpe/schemas/v1_0/evAlteracaoPoltrona_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/mdfe_dist_dfe/bindings/v1_0/dist_dfe_int_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/bpe/schemas/v1_0/consSitBPeTiposBasico_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/mdfe_dist_dfe/bindings/v1_0/xmldsig_core_schema_v1_01.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/bpe/schemas/v1_0/bpeTM_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/mdfe_dist_dfe/bindings/v1_0/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/bpe/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
+Filename: nfelib-2.0.5/nfelib/mdfe_dist_dfe/bindings/v1_0/tipos_dist_dfe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/bpe/schemas/v1_0/procEventoBPe_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/mdfe_dist_dfe/bindings/v1_0/tipos_geral_mdfe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/bpe/schemas/v1_0/consSitBPe_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/mdfe_dist_dfe/bindings/v1_0/ret_dist_dfe_int_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/bpe/schemas/v1_0/consStatServBPeTiposBasico_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/mdfe_dist_dfe/schemas/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe_dist_dfe/bindings/
+Filename: nfelib-2.0.5/nfelib/mdfe_dist_dfe/schemas/v1_0/tiposGeralMDFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe_dist_dfe/schemas/
+Filename: nfelib-2.0.5/nfelib/mdfe_dist_dfe/schemas/v1_0/distDFeInt_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe_dist_dfe/__init__.py
+Filename: nfelib-2.0.5/nfelib/mdfe_dist_dfe/schemas/v1_0/retDistDFeInt_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe_dist_dfe/bindings/v1_0/
+Filename: nfelib-2.0.5/nfelib/mdfe_dist_dfe/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe_dist_dfe/bindings/__init__.py
+Filename: nfelib-2.0.5/nfelib/mdfe_dist_dfe/schemas/v1_0/tiposDistDFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe_dist_dfe/bindings/v1_0/dist_dfe_int_v1_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/samples/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe_dist_dfe/bindings/v1_0/xmldsig_core_schema_v1_01.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe_dist_dfe/bindings/v1_0/__init__.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe_dist_dfe/bindings/v1_0/tipos_dist_dfe_v1_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe_dist_dfe/bindings/v1_0/tipos_geral_mdfe_v1_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/samples/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe_dist_dfe/bindings/v1_0/ret_dist_dfe_int_v1_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/samples/v1_0/35180803102452000172550010000476051695511860-01-cce.xml
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe_dist_dfe/schemas/v1_0/
+Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe_dist_dfe/schemas/v1_0/tiposGeralMDFe_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe_dist_dfe/schemas/v1_0/distDFeInt_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/cce_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe_dist_dfe/schemas/v1_0/retDistDFeInt_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/xmldsig_core_schema_v1_01.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe_dist_dfe/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/tipos_basico_v1_03.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/mdfe_dist_dfe/schemas/v1_0/tiposDistDFe_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_cce/samples/
+Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/proc_cce_nfe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_cce/bindings/
+Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/leiaute_cce_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_cce/schemas/
+Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/e110110_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_cce/__init__.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/ret_env_cce_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_cce/samples/v1_0/
+Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/env_cce_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_cce/samples/v1_0/35180803102452000172550010000476051695511860-01-cce.xml
+Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_cce/bindings/v1_0/
+Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/v1_0/leiauteCCe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_cce/bindings/__init__.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/v1_0/CCe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_cce/bindings/v1_0/cce_v1_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/v1_0/procCCeNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_cce/bindings/v1_0/xmldsig_core_schema_v1_01.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/v1_0/e110110_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_cce/bindings/v1_0/tipos_basico_v1_03.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/v1_0/envCCe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_cce/bindings/v1_0/__init__.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/v1_0/tiposBasico_v1.03.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_cce/bindings/v1_0/proc_cce_nfe_v1_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_cce/bindings/v1_0/leiaute_cce_v1_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/v1_0/retEnvCCe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_cce/bindings/v1_0/e110110_v1_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_cce/bindings/v1_0/ret_env_cce_v1_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_cce/bindings/v1_0/env_cce_v1_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_ator_interessado/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_cce/schemas/v1_0/
+Filename: nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_cce/schemas/v1_0/leiauteCCe_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_cce/schemas/v1_0/CCe_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/xmldsig_core_schema_v1_01.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_cce/schemas/v1_0/procCCeNFe_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/tipos_basico_v1_03.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_cce/schemas/v1_0/e110110_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_cce/schemas/v1_0/envCCe_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/ret_env_evento_ator_interessado_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_cce/schemas/v1_0/tiposBasico_v1.03.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/proc_evento_ator_interessado_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_cce/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/mod_110150_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_cce/schemas/v1_0/retEnvCCe_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/evento_ator_interessado_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_ator_interessado/bindings/
+Filename: nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/leiaute_evento_ator_interessado_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_ator_interessado/schemas/
+Filename: nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/env_evento_ator_interessado_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_ator_interessado/__init__.py
+Filename: nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_ator_interessado/bindings/v1_0/
+Filename: nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/v1_0/retEnvEventoAtorInteressado_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_ator_interessado/bindings/__init__.py
+Filename: nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/v1_0/procEventoAtorInteressado_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_ator_interessado/bindings/v1_0/xmldsig_core_schema_v1_01.py
+Filename: nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/v1_0/110150_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_ator_interessado/bindings/v1_0/tipos_basico_v1_03.py
+Filename: nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/v1_0/leiauteEventoAtorInteressado_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_ator_interessado/bindings/v1_0/__init__.py
+Filename: nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/v1_0/envEventoAtorInteressado_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_ator_interessado/bindings/v1_0/ret_env_evento_ator_interessado_v1_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/v1_0/eventoAtorInteressado_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_ator_interessado/bindings/v1_0/proc_evento_ator_interessado_v1_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/v1_0/tiposBasico_v1.03.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_ator_interessado/bindings/v1_0/mod_110150_v1_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_ator_interessado/bindings/v1_0/evento_ator_interessado_v1_00.py
+Filename: nfelib-2.0.5/nfelib/cte/samples/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_ator_interessado/bindings/v1_0/leiaute_evento_ator_interessado_v1_00.py
+Filename: nfelib-2.0.5/nfelib/cte/bindings/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_ator_interessado/bindings/v1_0/env_evento_ator_interessado_v1_00.py
+Filename: nfelib-2.0.5/nfelib/cte/schemas/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_ator_interessado/schemas/v1_0/
+Filename: nfelib-2.0.5/nfelib/cte/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_ator_interessado/schemas/v1_0/retEnvEventoAtorInteressado_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/cte/samples/v4_0/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_ator_interessado/schemas/v1_0/procEventoAtorInteressado_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/cte/samples/v4_0/51160624686092000173570010000000031000000020-cte.XML
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_ator_interessado/schemas/v1_0/110150_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/cte/samples/v4_0/cce35150107565416000104570000000012301000012300-ped-eve.xml
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_ator_interessado/schemas/v1_0/leiauteEventoAtorInteressado_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/cte/samples/v4_0/35190602427026001207570040000522031000522035-cte-multimodal.xml
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_ator_interessado/schemas/v1_0/envEventoAtorInteressado_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/cte/samples/v4_0/35170799999999999999670000000000261309301440-cte-of.xml
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_ator_interessado/schemas/v1_0/eventoAtorInteressado_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/cte/samples/v4_0/43120178408960000182570010000000041000000047-cte.xml
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_ator_interessado/schemas/v1_0/tiposBasico_v1.03.xsd
+Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_ator_interessado/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
+Filename: nfelib-2.0.5/nfelib/cte/bindings/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/samples/
+Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_reg_multimodal_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/bindings/
+Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/ret_cons_stat_serv_cte_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/schemas/
+Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_multi_modal_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/odoo/
+Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_epeccte_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/__init__.py
+Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/xmldsig_core_schema_v1_01.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/samples/v4_0/
+Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/cons_stat_serv_tipos_basico_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/samples/v4_0/51160624686092000173570010000000031000000020-cte.XML
+Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/samples/v4_0/cce35150107565416000104570000000012301000012300-ped-eve.xml
+Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/proc_gtve_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/samples/v4_0/35190602427026001207570040000522031000522035-cte-multimodal.xml
+Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_iecte_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/samples/v4_0/35170799999999999999670000000000261309301440-cte-of.xml
+Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/ret_inut_cte_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/samples/v4_0/43120178408960000182570010000000041000000047-cte.xml
+Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/proc_cte_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/bindings/v4_0/
+Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/proc_inut_cte_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/bindings/__init__.py
+Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_canc_prest_desacordo_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/bindings/v4_0/ev_reg_multimodal_v4_00.py
+Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_modal_rodoviario_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/bindings/v4_0/ret_cons_stat_serv_cte_v4_00.py
+Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/bindings/v4_0/cte_multi_modal_v4_00.py
+Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/ret_cons_sit_cte_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/bindings/v4_0/ev_epeccte_v4_00.py
+Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_cce_cte_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/bindings/v4_0/xmldsig_core_schema_v1_01.py
+Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/evento_cte_tipos_basico_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/bindings/v4_0/cons_stat_serv_tipos_basico_v4_00.py
+Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/tipos_geral_cte_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/bindings/v4_0/__init__.py
+Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_canc_cte_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/bindings/v4_0/proc_gtve_v4_00.py
+Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/ret_gtve_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/bindings/v4_0/ev_iecte_v4_00.py
+Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/ret_cte_simp_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/bindings/v4_0/ret_inut_cte_v4_00.py
+Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_modal_rodoviario_os_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/bindings/v4_0/proc_cte_v4_00.py
+Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/proc_evento_cte_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/bindings/v4_0/proc_inut_cte_v4_00.py
+Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_modal_aquaviario_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/bindings/v4_0/ev_canc_prest_desacordo_v4_00.py
+Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_gtv_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/bindings/v4_0/cte_modal_rodoviario_v4_00.py
+Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_modal_dutoviario_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/bindings/v4_0/cte_v4_00.py
+Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_tipos_basico_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/bindings/v4_0/ret_cons_sit_cte_v4_00.py
+Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/evento_cte_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/bindings/v4_0/ev_cce_cte_v4_00.py
+Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_os_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/bindings/v4_0/evento_cte_tipos_basico_v4_00.py
+Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/ret_evento_cte_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/bindings/v4_0/tipos_geral_cte_v4_00.py
+Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_cecte_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/bindings/v4_0/ev_canc_cte_v4_00.py
+Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/ret_cte_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/bindings/v4_0/ret_gtve_v4_00.py
+Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/cons_stat_serv_cte_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/bindings/v4_0/cte_modal_rodoviario_os_v4_00.py
+Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/ret_cte_os_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/bindings/v4_0/proc_evento_cte_v4_00.py
+Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/cons_sit_cte_tipos_basico_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/bindings/v4_0/cte_modal_aquaviario_v4_00.py
+Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_canc_iecte_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/bindings/v4_0/ev_gtv_v4_00.py
+Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/cons_sit_cte_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/bindings/v4_0/cte_modal_dutoviario_v4_00.py
+Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_canc_cecte_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/bindings/v4_0/cte_tipos_basico_v4_00.py
+Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/inut_cte_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/bindings/v4_0/evento_cte_v4_00.py
+Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/inut_cte_tipos_basico_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/bindings/v4_0/cte_os_v4_00.py
+Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/proc_cte_os_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/bindings/v4_0/ret_evento_cte_v4_00.py
+Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/gtve_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/bindings/v4_0/ev_cecte_v4_00.py
+Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_simp_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/bindings/v4_0/ret_cte_v4_00.py
+Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_modal_ferroviario_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/bindings/v4_0/cons_stat_serv_cte_v4_00.py
+Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_modal_aereo_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/bindings/v4_0/ret_cte_os_v4_00.py
+Filename: nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_prest_desacordo_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/bindings/v4_0/cons_sit_cte_tipos_basico_v4_00.py
+Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/bindings/v4_0/ev_canc_iecte_v4_00.py
+Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteModalRodoviario_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/bindings/v4_0/cons_sit_cte_v4_00.py
+Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteTiposBasico_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/bindings/v4_0/ev_canc_cecte_v4_00.py
+Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/evGTV_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/bindings/v4_0/inut_cte_v4_00.py
+Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/retEventoCTe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/bindings/v4_0/inut_cte_tipos_basico_v4_00.py
+Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteModalFerroviario_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/bindings/v4_0/proc_cte_os_v4_00.py
+Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/evCCeCTe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/bindings/v4_0/gtve_v4_00.py
+Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/eventoCTe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/bindings/v4_0/cte_modal_ferroviario_v4_00.py
+Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/evRegMultimodal_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/bindings/v4_0/cte_modal_aereo_v4_00.py
+Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/retCTeOS_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/bindings/v4_0/ev_prest_desacordo_v4_00.py
+Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/retGTVe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/schemas/v4_0/
+Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/retCTe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/schemas/v4_0/cteModalRodoviario_v4.00.xsd
+Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/evPrestDesacordo_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/schemas/v4_0/cteTiposBasico_v4.00.xsd
+Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/inutCTeTiposBasico_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/schemas/v4_0/evGTV_v4.00.xsd
+Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteSimp_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/schemas/v4_0/retEventoCTe_v4.00.xsd
+Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/evIECTe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/schemas/v4_0/cteModalFerroviario_v4.00.xsd
+Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/evCancPrestDesacordo_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/schemas/v4_0/evCCeCTe_v4.00.xsd
+Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/retConsStatServCTe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/schemas/v4_0/eventoCTe_v4.00.xsd
+Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/consStatServTiposBasico_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/schemas/v4_0/evRegMultimodal_v4.00.xsd
+Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteModalAereo_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/schemas/v4_0/retCTeOS_v4.00.xsd
+Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/procGTVe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/schemas/v4_0/retGTVe_v4.00.xsd
+Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/evEPECCTe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/schemas/v4_0/retCTe_v4.00.xsd
+Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteModalRodoviarioOS_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/schemas/v4_0/evPrestDesacordo_v4.00.xsd
+Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteModalDutoviario_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/schemas/v4_0/inutCTeTiposBasico_v4.00.xsd
+Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/tiposGeralCTe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/schemas/v4_0/evIECTe_v4.00.xsd
+Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/GTVe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/schemas/v4_0/evCancPrestDesacordo_v4.00.xsd
+Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/evCancIECTe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/schemas/v4_0/retConsStatServCTe_v4.00.xsd
+Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteMultiModal_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/schemas/v4_0/consStatServTiposBasico_v4.00.xsd
+Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/retInutCTe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/schemas/v4_0/cteModalAereo_v4.00.xsd
+Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/procEventoCTe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/schemas/v4_0/procGTVe_v4.00.xsd
+Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/evCECTe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/schemas/v4_0/evEPECCTe_v4.00.xsd
+Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/inutCTe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/schemas/v4_0/cteModalRodoviarioOS_v4.00.xsd
+Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/eventoCTeTiposBasico_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/schemas/v4_0/cteModalDutoviario_v4.00.xsd
+Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteOS_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/schemas/v4_0/tiposGeralCTe_v4.00.xsd
+Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/consSitCTeTiposBasico_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/schemas/v4_0/GTVe_v4.00.xsd
+Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/consStatServCTe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/schemas/v4_0/evCancIECTe_v4.00.xsd
+Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/procCTeOS_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/schemas/v4_0/cteMultiModal_v4.00.xsd
+Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/retConsSitCTe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/schemas/v4_0/retInutCTe_v4.00.xsd
+Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/consSitCTe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/schemas/v4_0/procEventoCTe_v4.00.xsd
+Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteModalAquaviario_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/schemas/v4_0/evCECTe_v4.00.xsd
+Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/cte_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/schemas/v4_0/inutCTe_v4.00.xsd
+Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/procInutCTe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/schemas/v4_0/eventoCTeTiposBasico_v4.00.xsd
+Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/retCTeSimp_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/schemas/v4_0/cteOS_v4.00.xsd
+Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/procCTe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/schemas/v4_0/consSitCTeTiposBasico_v4.00.xsd
+Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/evCancCECTe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/schemas/v4_0/consStatServCTe_v4.00.xsd
+Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/evCancCTe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/schemas/v4_0/procCTeOS_v4.00.xsd
+Filename: nfelib-2.0.5/nfelib/cte/schemas/v4_0/xmldsig-core-schema_v1.01.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/schemas/v4_0/retConsSitCTe_v4.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_evento_generico/bindings/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/schemas/v4_0/consSitCTe_v4.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_evento_generico/schemas/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/schemas/v4_0/cteModalAquaviario_v4.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_evento_generico/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/schemas/v4_0/cte_v4.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_evento_generico/bindings/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/schemas/v4_0/procInutCTe_v4.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_evento_generico/bindings/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/schemas/v4_0/procCTe_v4.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_evento_generico/bindings/v1_0/xmldsig_core_schema_v1_01.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/schemas/v4_0/evCancCECTe_v4.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_evento_generico/bindings/v1_0/tipos_basico_v1_03.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/schemas/v4_0/evCancCTe_v4.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_evento_generico/bindings/v1_0/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/schemas/v4_0/xmldsig-core-schema_v1.01.xsd
+Filename: nfelib-2.0.5/nfelib/nfe_evento_generico/bindings/v1_0/env_evento_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/odoo/v4_0/
+Filename: nfelib-2.0.5/nfelib/nfe_evento_generico/bindings/v1_0/ret_env_evento_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/odoo/__init__.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_generico/bindings/v1_0/proc_evento_nfe_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/odoo/v4_0/ev_reg_multimodal_v4_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_generico/bindings/v1_0/leiaute_evento_v1_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/odoo/v4_0/ret_cons_stat_serv_cte_v4_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_generico/schemas/v1_0/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/odoo/v4_0/cte_multi_modal_v4_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_generico/schemas/v1_0/envEvento_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/odoo/v4_0/ev_epeccte_v4_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_generico/schemas/v1_0/leiauteEvento_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/odoo/v4_0/cons_stat_serv_tipos_basico_v4_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_generico/schemas/v1_0/procEventoNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/odoo/v4_0/proc_gtve_v4_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_generico/schemas/v1_0/retEnvEvento_v1.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/odoo/v4_0/ev_iecte_v4_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_generico/schemas/v1_0/tiposBasico_v1.03.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/odoo/v4_0/ret_inut_cte_v4_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_evento_generico/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/odoo/v4_0/proc_cte_v4_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_cons/bindings/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/odoo/v4_0/proc_inut_cte_v4_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_cons/schemas/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/odoo/v4_0/ev_canc_prest_desacordo_v4_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_cons/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/odoo/v4_0/cte_modal_rodoviario_v4_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_cons/bindings/v2_0/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/odoo/v4_0/cte_v4_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_cons/bindings/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/odoo/v4_0/ret_cons_sit_cte_v4_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_cons/bindings/v2_0/xmldsig_core_schema_v1_01.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/odoo/v4_0/ev_cce_cte_v4_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_cons/bindings/v2_0/tipos_basico_v1_03.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/odoo/v4_0/evento_cte_tipos_basico_v4_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_cons/bindings/v2_0/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/odoo/v4_0/tipos_geral_cte_v4_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_cons/bindings/v2_0/cons_sit_nfe_v2_01.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/odoo/v4_0/ev_canc_cte_v4_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_cons/bindings/v2_0/leiaute_cons_sit_nfe_v2_01.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/odoo/v4_0/ret_gtve_v4_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_cons/bindings/v2_0/ret_cons_sit_nfe_v2_01.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/odoo/v4_0/cte_modal_rodoviario_os_v4_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_cons/schemas/v2_0/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/odoo/v4_0/proc_evento_cte_v4_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_cons/schemas/v2_0/consSitNFe_v2.01.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/odoo/v4_0/cte_modal_aquaviario_v4_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_cons/schemas/v2_0/leiauteConsSitNFe_v2.01.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/odoo/v4_0/ev_gtv_v4_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_cons/schemas/v2_0/tiposBasico_v1.03.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/odoo/v4_0/cte_modal_dutoviario_v4_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_cons/schemas/v2_0/xmldsig-core-schema_v1.01.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/odoo/v4_0/cte_tipos_basico_v4_00.py
+Filename: nfelib-2.0.5/nfelib/nfe_cons/schemas/v2_0/retConsSitNFe_v2.01.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/odoo/v4_0/evento_cte_v4_00.py
+Filename: nfelib-2.0.5/nfelib/nfe/samples/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/odoo/v4_0/cte_os_v4_00.py
+Filename: nfelib-2.0.5/nfelib/nfe/bindings/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/odoo/v4_0/ret_evento_cte_v4_00.py
+Filename: nfelib-2.0.5/nfelib/nfe/ws/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/odoo/v4_0/ev_cecte_v4_00.py
+Filename: nfelib-2.0.5/nfelib/nfe/schemas/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/odoo/v4_0/ret_cte_v4_00.py
+Filename: nfelib-2.0.5/nfelib/nfe/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/odoo/v4_0/cons_stat_serv_cte_v4_00.py
+Filename: nfelib-2.0.5/nfelib/nfe/samples/v4_0/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/odoo/v4_0/ret_cte_os_v4_00.py
+Filename: nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/odoo/v4_0/cons_sit_cte_tipos_basico_v4_00.py
+Filename: nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteInutNFe/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/odoo/v4_0/ev_canc_iecte_v4_00.py
+Filename: nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476711079516696-nfe.xml
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/odoo/v4_0/cons_sit_cte_v4_00.py
+Filename: nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/42220575277525000178550030000292481295366801-procNFe.xml
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/odoo/v4_0/ev_canc_cecte_v4_00.py
+Filename: nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000474491454651420-nfe.xml
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/odoo/v4_0/inut_cte_v4_00.py
+Filename: nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476051695511860-nfe.xml
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/odoo/v4_0/inut_cte_tipos_basico_v4_00.py
+Filename: nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476491552806942-nfe.xml
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/odoo/v4_0/proc_cte_os_v4_00.py
+Filename: nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/41170706117473000150550010000463202612756525-procNFe.xml
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/odoo/v4_0/gtve_v4_00.py
+Filename: nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476861118934859-nfe.xml
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/odoo/v4_0/cte_modal_ferroviario_v4_00.py
+Filename: nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/42210775277525000178550030000266631762885493-procNFe.xml
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/odoo/v4_0/cte_modal_aereo_v4_00.py
+Filename: nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476781421693968-nfe.xml
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/cte/odoo/v4_0/ev_prest_desacordo_v4_00.py
+Filename: nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/42211275277525000178550030000276771368212013-procNFe.xml
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_generico/bindings/
+Filename: nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/26180875335849000115550010000016871192213331-nfe.xml
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_generico/schemas/
+Filename: nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476121675985748-nfe.xml
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_generico/__init__.py
+Filename: nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000474501597356342-nfe.xml
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_generico/bindings/v1_0/
+Filename: nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/NFe35200159594315000157550010000000012062777161.xml
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_generico/bindings/__init__.py
+Filename: nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000474281920007498-nfe.xml
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_generico/bindings/v1_0/xmldsig_core_schema_v1_01.py
+Filename: nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000474641681223493-nfe.xml
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_generico/bindings/v1_0/tipos_basico_v1_03.py
+Filename: nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteInutNFe/41080676472349000430550010000001041671821888-ped-inu.xml
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_generico/bindings/v1_0/__init__.py
+Filename: nfelib-2.0.5/nfelib/nfe/bindings/v4_0/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_generico/bindings/v1_0/env_evento_v1_00.py
+Filename: nfelib-2.0.5/nfelib/nfe/bindings/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_generico/bindings/v1_0/ret_env_evento_v1_00.py
+Filename: nfelib-2.0.5/nfelib/nfe/bindings/v4_0/leiaute_cons_sit_nfe_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_generico/bindings/v1_0/proc_evento_nfe_v1_00.py
+Filename: nfelib-2.0.5/nfelib/nfe/bindings/v4_0/ret_cons_sit_nfe_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_generico/bindings/v1_0/leiaute_evento_v1_00.py
+Filename: nfelib-2.0.5/nfelib/nfe/bindings/v4_0/cons_cad_v2_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_generico/schemas/v1_0/
+Filename: nfelib-2.0.5/nfelib/nfe/bindings/v4_0/xmldsig_core_schema_v1_01.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_generico/schemas/v1_0/envEvento_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfe/bindings/v4_0/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_generico/schemas/v1_0/leiauteEvento_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfe/bindings/v4_0/ret_inut_nfe_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_generico/schemas/v1_0/procEventoNFe_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfe/bindings/v4_0/inut_nfe_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_generico/schemas/v1_0/retEnvEvento_v1.00.xsd
+Filename: nfelib-2.0.5/nfelib/nfe/bindings/v4_0/nfe_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_generico/schemas/v1_0/tiposBasico_v1.03.xsd
+Filename: nfelib-2.0.5/nfelib/nfe/bindings/v4_0/cons_reci_nfe_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_evento_generico/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
+Filename: nfelib-2.0.5/nfelib/nfe/bindings/v4_0/tipos_basico_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_cons/bindings/
+Filename: nfelib-2.0.5/nfelib/nfe/bindings/v4_0/ret_cons_stat_serv_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_cons/schemas/
+Filename: nfelib-2.0.5/nfelib/nfe/bindings/v4_0/leiaute_consulta_cadastro_v2_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_cons/__init__.py
+Filename: nfelib-2.0.5/nfelib/nfe/bindings/v4_0/cons_stat_serv_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_cons/bindings/v2_0/
+Filename: nfelib-2.0.5/nfelib/nfe/bindings/v4_0/leiaute_inut_nfe_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_cons/bindings/__init__.py
+Filename: nfelib-2.0.5/nfelib/nfe/bindings/v4_0/cons_sit_nfe_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_cons/bindings/v2_0/xmldsig_core_schema_v1_01.py
+Filename: nfelib-2.0.5/nfelib/nfe/bindings/v4_0/ret_cons_reci_nfe_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_cons/bindings/v2_0/tipos_basico_v1_03.py
+Filename: nfelib-2.0.5/nfelib/nfe/bindings/v4_0/leiaute_cons_stat_serv_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_cons/bindings/v2_0/__init__.py
+Filename: nfelib-2.0.5/nfelib/nfe/bindings/v4_0/envi_nfe_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_cons/bindings/v2_0/cons_sit_nfe_v2_01.py
+Filename: nfelib-2.0.5/nfelib/nfe/bindings/v4_0/proc_nfe_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_cons/bindings/v2_0/leiaute_cons_sit_nfe_v2_01.py
+Filename: nfelib-2.0.5/nfelib/nfe/bindings/v4_0/proc_inut_nfe_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_cons/bindings/v2_0/ret_cons_sit_nfe_v2_01.py
+Filename: nfelib-2.0.5/nfelib/nfe/bindings/v4_0/ret_envi_nfe_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_cons/schemas/v2_0/
+Filename: nfelib-2.0.5/nfelib/nfe/bindings/v4_0/leiaute_nfe_v4_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_cons/schemas/v2_0/consSitNFe_v2.01.xsd
+Filename: nfelib-2.0.5/nfelib/nfe/bindings/v4_0/ret_cons_cad_v2_00.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_cons/schemas/v2_0/leiauteConsSitNFe_v2.01.xsd
+Filename: nfelib-2.0.5/nfelib/nfe/ws/__init__.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_cons/schemas/v2_0/tiposBasico_v1.03.xsd
+Filename: nfelib-2.0.5/nfelib/nfe/ws/edoc_legacy.py
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_cons/schemas/v2_0/xmldsig-core-schema_v1.01.xsd
+Filename: nfelib-2.0.5/nfelib/nfe/schemas/v4_0/
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe_cons/schemas/v2_0/retConsSitNFe_v2.01.xsd
+Filename: nfelib-2.0.5/nfelib/nfe/schemas/v4_0/leiauteConsStatServ_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe/samples/
+Filename: nfelib-2.0.5/nfelib/nfe/schemas/v4_0/retConsReciNFe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe/bindings/
+Filename: nfelib-2.0.5/nfelib/nfe/schemas/v4_0/consStatServ_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe/ws/
+Filename: nfelib-2.0.5/nfelib/nfe/schemas/v4_0/procNFe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe/schemas/
+Filename: nfelib-2.0.5/nfelib/nfe/schemas/v4_0/retInutNFe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe/__init__.py
+Filename: nfelib-2.0.5/nfelib/nfe/schemas/v4_0/procInutNFe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe/samples/v4_0/
+Filename: nfelib-2.0.5/nfelib/nfe/schemas/v4_0/consCad_v2.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteNFe/
+Filename: nfelib-2.0.5/nfelib/nfe/schemas/v4_0/leiauteConsSitNFe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteInutNFe/
+Filename: nfelib-2.0.5/nfelib/nfe/schemas/v4_0/nfe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476711079516696-nfe.xml
+Filename: nfelib-2.0.5/nfelib/nfe/schemas/v4_0/retConsCad_v2.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteNFe/42220575277525000178550030000292481295366801-procNFe.xml
+Filename: nfelib-2.0.5/nfelib/nfe/schemas/v4_0/consReciNFe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000474491454651420-nfe.xml
+Filename: nfelib-2.0.5/nfelib/nfe/schemas/v4_0/leiauteInutNFe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476051695511860-nfe.xml
+Filename: nfelib-2.0.5/nfelib/nfe/schemas/v4_0/enviNFe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476491552806942-nfe.xml
+Filename: nfelib-2.0.5/nfelib/nfe/schemas/v4_0/inutNFe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteNFe/41170706117473000150550010000463202612756525-procNFe.xml
+Filename: nfelib-2.0.5/nfelib/nfe/schemas/v4_0/leiauteConsultaCadastro_v2.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476861118934859-nfe.xml
+Filename: nfelib-2.0.5/nfelib/nfe/schemas/v4_0/retEnviNFe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteNFe/42210775277525000178550030000266631762885493-procNFe.xml
+Filename: nfelib-2.0.5/nfelib/nfe/schemas/v4_0/consSitNFe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476781421693968-nfe.xml
+Filename: nfelib-2.0.5/nfelib/nfe/schemas/v4_0/tiposBasico_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteNFe/42211275277525000178550030000276771368212013-procNFe.xml
+Filename: nfelib-2.0.5/nfelib/nfe/schemas/v4_0/leiauteNFe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteNFe/26180875335849000115550010000016871192213331-nfe.xml
+Filename: nfelib-2.0.5/nfelib/nfe/schemas/v4_0/retConsStatServ_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476121675985748-nfe.xml
+Filename: nfelib-2.0.5/nfelib/nfe/schemas/v4_0/tiposBasico_v1.03.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000474501597356342-nfe.xml
+Filename: nfelib-2.0.5/nfelib/nfe/schemas/v4_0/retConsSitNFe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteNFe/NFe35200159594315000157550010000000012062777161.xml
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000474281920007498-nfe.xml
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000474641681223493-nfe.xml
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteInutNFe/41080676472349000430550010000001041671821888-ped-inu.xml
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/bindings/v4_0/
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/bindings/__init__.py
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/bindings/v4_0/leiaute_cons_sit_nfe_v4_00.py
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/bindings/v4_0/ret_cons_sit_nfe_v4_00.py
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/bindings/v4_0/cons_cad_v2_00.py
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/bindings/v4_0/xmldsig_core_schema_v1_01.py
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/bindings/v4_0/__init__.py
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/bindings/v4_0/ret_inut_nfe_v4_00.py
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/bindings/v4_0/inut_nfe_v4_00.py
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/bindings/v4_0/nfe_v4_00.py
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/bindings/v4_0/cons_reci_nfe_v4_00.py
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/bindings/v4_0/tipos_basico_v4_00.py
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/bindings/v4_0/ret_cons_stat_serv_v4_00.py
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/bindings/v4_0/leiaute_consulta_cadastro_v2_00.py
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/bindings/v4_0/cons_stat_serv_v4_00.py
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/bindings/v4_0/leiaute_inut_nfe_v4_00.py
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/bindings/v4_0/cons_sit_nfe_v4_00.py
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/bindings/v4_0/ret_cons_reci_nfe_v4_00.py
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/bindings/v4_0/leiaute_cons_stat_serv_v4_00.py
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/bindings/v4_0/envi_nfe_v4_00.py
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/bindings/v4_0/proc_nfe_v4_00.py
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/bindings/v4_0/proc_inut_nfe_v4_00.py
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/bindings/v4_0/ret_envi_nfe_v4_00.py
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/bindings/v4_0/leiaute_nfe_v4_00.py
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/bindings/v4_0/ret_cons_cad_v2_00.py
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/ws/__init__.py
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/ws/edoc_legacy.py
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/schemas/v4_0/
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/schemas/v4_0/leiauteConsStatServ_v4.00.xsd
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/schemas/v4_0/retConsReciNFe_v4.00.xsd
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/schemas/v4_0/consStatServ_v4.00.xsd
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/schemas/v4_0/procNFe_v4.00.xsd
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/schemas/v4_0/retInutNFe_v4.00.xsd
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/schemas/v4_0/procInutNFe_v4.00.xsd
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/schemas/v4_0/consCad_v2.00.xsd
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/schemas/v4_0/leiauteConsSitNFe_v4.00.xsd
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/schemas/v4_0/nfe_v4.00.xsd
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/schemas/v4_0/retConsCad_v2.00.xsd
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/schemas/v4_0/consReciNFe_v4.00.xsd
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/schemas/v4_0/leiauteInutNFe_v4.00.xsd
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/schemas/v4_0/enviNFe_v4.00.xsd
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/schemas/v4_0/inutNFe_v4.00.xsd
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/schemas/v4_0/leiauteConsultaCadastro_v2.00.xsd
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/schemas/v4_0/retEnviNFe_v4.00.xsd
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/schemas/v4_0/consSitNFe_v4.00.xsd
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/schemas/v4_0/tiposBasico_v4.00.xsd
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/schemas/v4_0/leiauteNFe_v4.00.xsd
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/schemas/v4_0/retConsStatServ_v4.00.xsd
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/schemas/v4_0/tiposBasico_v1.03.xsd
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/schemas/v4_0/retConsSitNFe_v4.00.xsd
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/nfe/schemas/v4_0/xmldsig-core-schema_v1.01.xsd
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/odoo/nfe/
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/odoo/__init__.py
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/odoo/nfe/v4_0/
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/odoo/nfe/__init__.py
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/odoo/nfe/v4_0/leiaute_cons_sit_nfe_v4_00.py
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/odoo/nfe/v4_0/ret_cons_sit_nfe_v4_00.py
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/odoo/nfe/v4_0/cons_cad_v2_00.py
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/odoo/nfe/v4_0/ret_inut_nfe_v4_00.py
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/odoo/nfe/v4_0/inut_nfe_v4_00.py
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/odoo/nfe/v4_0/nfe_v4_00.py
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/odoo/nfe/v4_0/cons_reci_nfe_v4_00.py
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/odoo/nfe/v4_0/tipos_basico_v4_00.py
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/odoo/nfe/v4_0/ret_cons_stat_serv_v4_00.py
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/odoo/nfe/v4_0/leiaute_consulta_cadastro_v2_00.py
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/odoo/nfe/v4_0/cons_stat_serv_v4_00.py
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/odoo/nfe/v4_0/leiaute_inut_nfe_v4_00.py
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/odoo/nfe/v4_0/cons_sit_nfe_v4_00.py
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/odoo/nfe/v4_0/ret_cons_reci_nfe_v4_00.py
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/odoo/nfe/v4_0/leiaute_cons_stat_serv_v4_00.py
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/odoo/nfe/v4_0/envi_nfe_v4_00.py
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/odoo/nfe/v4_0/proc_nfe_v4_00.py
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/odoo/nfe/v4_0/proc_inut_nfe_v4_00.py
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/odoo/nfe/v4_0/ret_envi_nfe_v4_00.py
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/odoo/nfe/v4_0/leiaute_nfe_v4_00.py
-Comment: 
-
-Filename: nfelib-2.0.4/nfelib/odoo/nfe/v4_0/ret_cons_cad_v2_00.py
+Filename: nfelib-2.0.5/nfelib/nfe/schemas/v4_0/xmldsig-core-schema_v1.01.xsd
 Comment: 
 
 Zip file comment:
```

## Comparing `nfelib-2.0.4/MIT-LICENSE` & `nfelib-2.0.5/MIT-LICENSE`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/setup.cfg` & `nfelib-2.0.5/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nfelib
-version = 2.0.4
+version = 2.0.5
 description = nfelib: electronic invoicing library for Brazil
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/akretion/nfelib
 author = Raphaël Valyi
 author_email = "raphael.valyi@akretion.com.br"
 license = MIT
@@ -40,14 +40,16 @@
 test = 
 	xmldiff
 	pytest
 	pytest-cov
 	tox
 	requests
 	beautifulsoup4
+	erpbrasil.assinatura
+	brazilfiscalreport
 
 [flake8]
 exclude = tests/*
 max-line-length = 88
 ignore = W503,ANN101,ANN102,E203
 
 [doc8]
```

## Comparing `nfelib-2.0.4/README.md` & `nfelib-2.0.5/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -54,14 +54,36 @@
 Nfe(infNFe=Tnfe.InfNfe(ide=None, emit=Tnfe.InfNfe.Emit(CNPJ='59594315000157', CPF=None, xNome='Minha Empresa', xFant=None, enderEmit=None, IE=None, IEST=None, IM=None, CNAE=None, CRT=None), avulsa=None, dest=None, retirada=None, entrega=None, autXML=[], det=[], total=None, transp=None, cobr=None, pag=None, infIntermed=None, infAdic=None, exporta=None, compra=None, cana=None, infRespTec=None, infSolicNFF=None, versao=None, Id=None), infNFeSupl=None, signature=None)
 >>> 
 >>> # Validar o XML de uma nota:
 >>> nfe.validate_xml()
 ["Element '{http://www.portalfiscal.inf.br/nfe}infNFe': The attribute 'versao' is required but missing.", "Element '{http://www.portalfiscal.inf.br/nfe}infNFe': The attribute 'Id' is required but missing." [...]
 ```
 
+Assinar o XML de uma nota usando a lib [erpbrasil.assinatura](https://github.com/erpbrasil/erpbrasil.assinatura) (funciona com os outros documentos eletrônicos também)
+```
+>>> # Assinar o XML de uma nota:
+>>> with open(path_to_your_pkcs12_certificate, "rb") as pkcs12_buffer:
+    pkcs12_data = pkcs12_buffer.read()
+>>> signed_xml = nfe.sign_xml(xml, pkcs12_data, cert_password, nfe.NFe.infNFe.Id)
+```
+
+Imprimir o DANFE usando a lib [BrazilFiscalReport](https://github.com/Engenere/BrazilFiscalReport) ou a lib [erpbrasil.edoc.pdf](https://github.com/erpbrasil/erpbrasil.edoc.pdf) (futuramente BrazilFiscalReport deve imprimir o pdf de outros documentos eletrônicos também; erpbrasil.edoc.pdf é uma lib mais 'legacy')
+```
+>>> # Imprimir o pdf de uma nota usando BrazilFiscalReport:
+>>> pdf_bytes = nfe.to_pdf()
+>>> # Imprimir o pdf de uma nota usando erpbrasil.edoc.pdf:
+>>> pdf_bytes = nfe.to_pdf(engine="erpbrasil.edoc.pdf")
+>>> # Ou então para imprimir e assinar junto:
+>>> pdf_bytes = nfe.to_pdf(
+    pkcs12_data=cert_data,
+    pkcs12_password=cert_password,
+    doc_id=nfe.NFe.infNFe.Id,
+    )
+```
+
 **NFS-e padrão nacional**
 ```python
 >>> # Ler uma NFS-e:
 >>>> from nfelib.nfse.bindings.v1_0.nfse_v1_00 import Nfse
 >>> nfse = Nfse.from_path("alguma_nfse.xml")
 >>>
 >>> # Serializar uma NFS-e:
```

### html2text {}

```diff
@@ -38,17 +38,32 @@
 avulsa=None, dest=None, retirada=None, entrega=None, autXML=[], det=[],
 total=None, transp=None, cobr=None, pag=None, infIntermed=None, infAdic=None,
 exporta=None, compra=None, cana=None, infRespTec=None, infSolicNFF=None,
 versao=None, Id=None), infNFeSupl=None, signature=None) >>> >>> # Validar o XML
 de uma nota: >>> nfe.validate_xml() ["Element '{http://www.portalfiscal.inf.br/
 nfe}infNFe': The attribute 'versao' is required but missing.", "Element '{http:
 //www.portalfiscal.inf.br/nfe}infNFe': The attribute 'Id' is required but
-missing." [...] ``` **NFS-e padrÃ£o nacional** ```python >>> # Ler uma NFS-e:
->>>> from nfelib.nfse.bindings.v1_0.nfse_v1_00 import Nfse >>> nfse =
-Nfse.from_path("alguma_nfse.xml") >>> >>> # Serializar uma NFS-e: >>>
+missing." [...] ``` Assinar o XML de uma nota usando a lib
+[erpbrasil.assinatura](https://github.com/erpbrasil/erpbrasil.assinatura)
+(funciona com os outros documentos eletrÃ´nicos tambÃ©m) ``` >>> # Assinar o
+XML de uma nota: >>> with open(path_to_your_pkcs12_certificate, "rb") as
+pkcs12_buffer: pkcs12_data = pkcs12_buffer.read() >>> signed_xml = nfe.sign_xml
+(xml, pkcs12_data, cert_password, nfe.NFe.infNFe.Id) ``` Imprimir o DANFE
+usando a lib [BrazilFiscalReport](https://github.com/Engenere/
+BrazilFiscalReport) ou a lib [erpbrasil.edoc.pdf](https://github.com/erpbrasil/
+erpbrasil.edoc.pdf) (futuramente BrazilFiscalReport deve imprimir o pdf de
+outros documentos eletrÃ´nicos tambÃ©m; erpbrasil.edoc.pdf Ã© uma lib mais
+'legacy') ``` >>> # Imprimir o pdf de uma nota usando BrazilFiscalReport: >>>
+pdf_bytes = nfe.to_pdf() >>> # Imprimir o pdf de uma nota usando
+erpbrasil.edoc.pdf: >>> pdf_bytes = nfe.to_pdf(engine="erpbrasil.edoc.pdf") >>>
+# Ou entÃ£o para imprimir e assinar junto: >>> pdf_bytes = nfe.to_pdf
+( pkcs12_data=cert_data, pkcs12_password=cert_password,
+doc_id=nfe.NFe.infNFe.Id, ) ``` **NFS-e padrÃ£o nacional** ```python >>> # Ler
+uma NFS-e: >>>> from nfelib.nfse.bindings.v1_0.nfse_v1_00 import Nfse >>> nfse
+= Nfse.from_path("alguma_nfse.xml") >>> >>> # Serializar uma NFS-e: >>>
 nfse.to_xml() >>> # Ler uma DPS: >>>> from nfelib.nfse.bindings.v1_0.dps_v1_00
 import Dps >>> dps = Nfse.from_path("nfelib/nfse/samples/v1_0/GerarNFSeEnvio-
 env-loterps.xml") >>> >>> # Serializar uma DPS: >>> dps.to_xml() ``` **MDF-e**
 ```python >>> # Ler um MDF-e: >>>> from nfelib.mdfe.bindings.v3_0.mdfe_v3_00
 import Mdfe >>> mdfe = Mdfe.from_path("nfelib/mdfe/samples/v3_0/
 ComPagtoPIX_41210780568835000181580010402005751006005791-procMDFe.xml") >>> >>>
 # Serializar um MDF-e: >>> mdfe.to_xml() ``` **CT-e** ```python >>> # Ler um
```

## Comparing `nfelib-2.0.4/PKG-INFO` & `nfelib-2.0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nfelib
-Version: 2.0.4
+Version: 2.0.5
 Summary: nfelib: electronic invoicing library for Brazil
 Home-page: https://github.com/akretion/nfelib
 Author: Raphaël Valyi
 Author-email: "raphael.valyi@akretion.com.br"
 License: MIT
 Project-URL: Source, https://github.com/akretion/nfelib
 Keywords: e-invoicing,NFe,ERP,Odoo,NFSe,CTe,MDFe,BPe
@@ -84,14 +84,36 @@
 Nfe(infNFe=Tnfe.InfNfe(ide=None, emit=Tnfe.InfNfe.Emit(CNPJ='59594315000157', CPF=None, xNome='Minha Empresa', xFant=None, enderEmit=None, IE=None, IEST=None, IM=None, CNAE=None, CRT=None), avulsa=None, dest=None, retirada=None, entrega=None, autXML=[], det=[], total=None, transp=None, cobr=None, pag=None, infIntermed=None, infAdic=None, exporta=None, compra=None, cana=None, infRespTec=None, infSolicNFF=None, versao=None, Id=None), infNFeSupl=None, signature=None)
 >>> 
 >>> # Validar o XML de uma nota:
 >>> nfe.validate_xml()
 ["Element '{http://www.portalfiscal.inf.br/nfe}infNFe': The attribute 'versao' is required but missing.", "Element '{http://www.portalfiscal.inf.br/nfe}infNFe': The attribute 'Id' is required but missing." [...]
 ```
 
+Assinar o XML de uma nota usando a lib [erpbrasil.assinatura](https://github.com/erpbrasil/erpbrasil.assinatura) (funciona com os outros documentos eletrônicos também)
+```
+>>> # Assinar o XML de uma nota:
+>>> with open(path_to_your_pkcs12_certificate, "rb") as pkcs12_buffer:
+    pkcs12_data = pkcs12_buffer.read()
+>>> signed_xml = nfe.sign_xml(xml, pkcs12_data, cert_password, nfe.NFe.infNFe.Id)
+```
+
+Imprimir o DANFE usando a lib [BrazilFiscalReport](https://github.com/Engenere/BrazilFiscalReport) ou a lib [erpbrasil.edoc.pdf](https://github.com/erpbrasil/erpbrasil.edoc.pdf) (futuramente BrazilFiscalReport deve imprimir o pdf de outros documentos eletrônicos também; erpbrasil.edoc.pdf é uma lib mais 'legacy')
+```
+>>> # Imprimir o pdf de uma nota usando BrazilFiscalReport:
+>>> pdf_bytes = nfe.to_pdf()
+>>> # Imprimir o pdf de uma nota usando erpbrasil.edoc.pdf:
+>>> pdf_bytes = nfe.to_pdf(engine="erpbrasil.edoc.pdf")
+>>> # Ou então para imprimir e assinar junto:
+>>> pdf_bytes = nfe.to_pdf(
+    pkcs12_data=cert_data,
+    pkcs12_password=cert_password,
+    doc_id=nfe.NFe.infNFe.Id,
+    )
+```
+
 **NFS-e padrão nacional**
 ```python
 >>> # Ler uma NFS-e:
 >>>> from nfelib.nfse.bindings.v1_0.nfse_v1_00 import Nfse
 >>> nfse = Nfse.from_path("alguma_nfse.xml")
 >>>
 >>> # Serializar uma NFS-e:
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nfelib Version: 2.0.4 Summary: nfelib: electronic
+Metadata-Version: 2.1 Name: nfelib Version: 2.0.5 Summary: nfelib: electronic
 invoicing library for Brazil Home-page: https://github.com/akretion/nfelib
 Author: RaphaÃ«l Valyi Author-email: "raphael.valyi@akretion.com.br" License:
 MIT Project-URL: Source, https://github.com/akretion/nfelib Keywords: e-
 invoicing,NFe,ERP,Odoo,NFSe,CTe,MDFe,BPe Platform: UNKNOWN Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python Classifier: Programming Language :: Python :: 3 Classifier:
@@ -54,17 +54,32 @@
 avulsa=None, dest=None, retirada=None, entrega=None, autXML=[], det=[],
 total=None, transp=None, cobr=None, pag=None, infIntermed=None, infAdic=None,
 exporta=None, compra=None, cana=None, infRespTec=None, infSolicNFF=None,
 versao=None, Id=None), infNFeSupl=None, signature=None) >>> >>> # Validar o XML
 de uma nota: >>> nfe.validate_xml() ["Element '{http://www.portalfiscal.inf.br/
 nfe}infNFe': The attribute 'versao' is required but missing.", "Element '{http:
 //www.portalfiscal.inf.br/nfe}infNFe': The attribute 'Id' is required but
-missing." [...] ``` **NFS-e padrÃ£o nacional** ```python >>> # Ler uma NFS-e:
->>>> from nfelib.nfse.bindings.v1_0.nfse_v1_00 import Nfse >>> nfse =
-Nfse.from_path("alguma_nfse.xml") >>> >>> # Serializar uma NFS-e: >>>
+missing." [...] ``` Assinar o XML de uma nota usando a lib
+[erpbrasil.assinatura](https://github.com/erpbrasil/erpbrasil.assinatura)
+(funciona com os outros documentos eletrÃ´nicos tambÃ©m) ``` >>> # Assinar o
+XML de uma nota: >>> with open(path_to_your_pkcs12_certificate, "rb") as
+pkcs12_buffer: pkcs12_data = pkcs12_buffer.read() >>> signed_xml = nfe.sign_xml
+(xml, pkcs12_data, cert_password, nfe.NFe.infNFe.Id) ``` Imprimir o DANFE
+usando a lib [BrazilFiscalReport](https://github.com/Engenere/
+BrazilFiscalReport) ou a lib [erpbrasil.edoc.pdf](https://github.com/erpbrasil/
+erpbrasil.edoc.pdf) (futuramente BrazilFiscalReport deve imprimir o pdf de
+outros documentos eletrÃ´nicos tambÃ©m; erpbrasil.edoc.pdf Ã© uma lib mais
+'legacy') ``` >>> # Imprimir o pdf de uma nota usando BrazilFiscalReport: >>>
+pdf_bytes = nfe.to_pdf() >>> # Imprimir o pdf de uma nota usando
+erpbrasil.edoc.pdf: >>> pdf_bytes = nfe.to_pdf(engine="erpbrasil.edoc.pdf") >>>
+# Ou entÃ£o para imprimir e assinar junto: >>> pdf_bytes = nfe.to_pdf
+( pkcs12_data=cert_data, pkcs12_password=cert_password,
+doc_id=nfe.NFe.infNFe.Id, ) ``` **NFS-e padrÃ£o nacional** ```python >>> # Ler
+uma NFS-e: >>>> from nfelib.nfse.bindings.v1_0.nfse_v1_00 import Nfse >>> nfse
+= Nfse.from_path("alguma_nfse.xml") >>> >>> # Serializar uma NFS-e: >>>
 nfse.to_xml() >>> # Ler uma DPS: >>>> from nfelib.nfse.bindings.v1_0.dps_v1_00
 import Dps >>> dps = Nfse.from_path("nfelib/nfse/samples/v1_0/GerarNFSeEnvio-
 env-loterps.xml") >>> >>> # Serializar uma DPS: >>> dps.to_xml() ``` **MDF-e**
 ```python >>> # Ler um MDF-e: >>>> from nfelib.mdfe.bindings.v3_0.mdfe_v3_00
 import Mdfe >>> mdfe = Mdfe.from_path("nfelib/mdfe/samples/v3_0/
 ComPagtoPIX_41210780568835000181580010402005751006005791-procMDFe.xml") >>> >>>
 # Serializar um MDF-e: >>> mdfe.to_xml() ``` **CT-e** ```python >>> # Ler um
```

## Comparing `nfelib-2.0.4/nfelib.egg-info/SOURCES.txt` & `nfelib-2.0.5/nfelib.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -67,14 +67,15 @@
 nfelib/cte/bindings/v4_0/cte_modal_aquaviario_v4_00.py
 nfelib/cte/bindings/v4_0/cte_modal_dutoviario_v4_00.py
 nfelib/cte/bindings/v4_0/cte_modal_ferroviario_v4_00.py
 nfelib/cte/bindings/v4_0/cte_modal_rodoviario_os_v4_00.py
 nfelib/cte/bindings/v4_0/cte_modal_rodoviario_v4_00.py
 nfelib/cte/bindings/v4_0/cte_multi_modal_v4_00.py
 nfelib/cte/bindings/v4_0/cte_os_v4_00.py
+nfelib/cte/bindings/v4_0/cte_simp_v4_00.py
 nfelib/cte/bindings/v4_0/cte_tipos_basico_v4_00.py
 nfelib/cte/bindings/v4_0/cte_v4_00.py
 nfelib/cte/bindings/v4_0/ev_canc_cecte_v4_00.py
 nfelib/cte/bindings/v4_0/ev_canc_cte_v4_00.py
 nfelib/cte/bindings/v4_0/ev_canc_iecte_v4_00.py
 nfelib/cte/bindings/v4_0/ev_canc_prest_desacordo_v4_00.py
 nfelib/cte/bindings/v4_0/ev_cce_cte_v4_00.py
@@ -93,64 +94,21 @@
 nfelib/cte/bindings/v4_0/proc_cte_v4_00.py
 nfelib/cte/bindings/v4_0/proc_evento_cte_v4_00.py
 nfelib/cte/bindings/v4_0/proc_gtve_v4_00.py
 nfelib/cte/bindings/v4_0/proc_inut_cte_v4_00.py
 nfelib/cte/bindings/v4_0/ret_cons_sit_cte_v4_00.py
 nfelib/cte/bindings/v4_0/ret_cons_stat_serv_cte_v4_00.py
 nfelib/cte/bindings/v4_0/ret_cte_os_v4_00.py
+nfelib/cte/bindings/v4_0/ret_cte_simp_v4_00.py
 nfelib/cte/bindings/v4_0/ret_cte_v4_00.py
 nfelib/cte/bindings/v4_0/ret_evento_cte_v4_00.py
 nfelib/cte/bindings/v4_0/ret_gtve_v4_00.py
 nfelib/cte/bindings/v4_0/ret_inut_cte_v4_00.py
 nfelib/cte/bindings/v4_0/tipos_geral_cte_v4_00.py
 nfelib/cte/bindings/v4_0/xmldsig_core_schema_v1_01.py
-nfelib/cte/odoo/__init__.py
-nfelib/cte/odoo/v4_0/cons_sit_cte_tipos_basico_v4_00.py
-nfelib/cte/odoo/v4_0/cons_sit_cte_v4_00.py
-nfelib/cte/odoo/v4_0/cons_stat_serv_cte_v4_00.py
-nfelib/cte/odoo/v4_0/cons_stat_serv_tipos_basico_v4_00.py
-nfelib/cte/odoo/v4_0/cte_modal_aereo_v4_00.py
-nfelib/cte/odoo/v4_0/cte_modal_aquaviario_v4_00.py
-nfelib/cte/odoo/v4_0/cte_modal_dutoviario_v4_00.py
-nfelib/cte/odoo/v4_0/cte_modal_ferroviario_v4_00.py
-nfelib/cte/odoo/v4_0/cte_modal_rodoviario_os_v4_00.py
-nfelib/cte/odoo/v4_0/cte_modal_rodoviario_v4_00.py
-nfelib/cte/odoo/v4_0/cte_multi_modal_v4_00.py
-nfelib/cte/odoo/v4_0/cte_os_v4_00.py
-nfelib/cte/odoo/v4_0/cte_tipos_basico_v4_00.py
-nfelib/cte/odoo/v4_0/cte_v4_00.py
-nfelib/cte/odoo/v4_0/ev_canc_cecte_v4_00.py
-nfelib/cte/odoo/v4_0/ev_canc_cte_v4_00.py
-nfelib/cte/odoo/v4_0/ev_canc_iecte_v4_00.py
-nfelib/cte/odoo/v4_0/ev_canc_prest_desacordo_v4_00.py
-nfelib/cte/odoo/v4_0/ev_cce_cte_v4_00.py
-nfelib/cte/odoo/v4_0/ev_cecte_v4_00.py
-nfelib/cte/odoo/v4_0/ev_epeccte_v4_00.py
-nfelib/cte/odoo/v4_0/ev_gtv_v4_00.py
-nfelib/cte/odoo/v4_0/ev_iecte_v4_00.py
-nfelib/cte/odoo/v4_0/ev_prest_desacordo_v4_00.py
-nfelib/cte/odoo/v4_0/ev_reg_multimodal_v4_00.py
-nfelib/cte/odoo/v4_0/evento_cte_tipos_basico_v4_00.py
-nfelib/cte/odoo/v4_0/evento_cte_v4_00.py
-nfelib/cte/odoo/v4_0/gtve_v4_00.py
-nfelib/cte/odoo/v4_0/inut_cte_tipos_basico_v4_00.py
-nfelib/cte/odoo/v4_0/inut_cte_v4_00.py
-nfelib/cte/odoo/v4_0/proc_cte_os_v4_00.py
-nfelib/cte/odoo/v4_0/proc_cte_v4_00.py
-nfelib/cte/odoo/v4_0/proc_evento_cte_v4_00.py
-nfelib/cte/odoo/v4_0/proc_gtve_v4_00.py
-nfelib/cte/odoo/v4_0/proc_inut_cte_v4_00.py
-nfelib/cte/odoo/v4_0/ret_cons_sit_cte_v4_00.py
-nfelib/cte/odoo/v4_0/ret_cons_stat_serv_cte_v4_00.py
-nfelib/cte/odoo/v4_0/ret_cte_os_v4_00.py
-nfelib/cte/odoo/v4_0/ret_cte_v4_00.py
-nfelib/cte/odoo/v4_0/ret_evento_cte_v4_00.py
-nfelib/cte/odoo/v4_0/ret_gtve_v4_00.py
-nfelib/cte/odoo/v4_0/ret_inut_cte_v4_00.py
-nfelib/cte/odoo/v4_0/tipos_geral_cte_v4_00.py
 nfelib/cte/samples/v4_0/35170799999999999999670000000000261309301440-cte-of.xml
 nfelib/cte/samples/v4_0/35190602427026001207570040000522031000522035-cte-multimodal.xml
 nfelib/cte/samples/v4_0/43120178408960000182570010000000041000000047-cte.xml
 nfelib/cte/samples/v4_0/51160624686092000173570010000000031000000020-cte.XML
 nfelib/cte/samples/v4_0/cce35150107565416000104570000000012301000012300-ped-eve.xml
 nfelib/cte/schemas/v4_0/GTVe_v4.00.xsd
 nfelib/cte/schemas/v4_0/consSitCTeTiposBasico_v4.00.xsd
@@ -161,14 +119,15 @@
 nfelib/cte/schemas/v4_0/cteModalAquaviario_v4.00.xsd
 nfelib/cte/schemas/v4_0/cteModalDutoviario_v4.00.xsd
 nfelib/cte/schemas/v4_0/cteModalFerroviario_v4.00.xsd
 nfelib/cte/schemas/v4_0/cteModalRodoviarioOS_v4.00.xsd
 nfelib/cte/schemas/v4_0/cteModalRodoviario_v4.00.xsd
 nfelib/cte/schemas/v4_0/cteMultiModal_v4.00.xsd
 nfelib/cte/schemas/v4_0/cteOS_v4.00.xsd
+nfelib/cte/schemas/v4_0/cteSimp_v4.00.xsd
 nfelib/cte/schemas/v4_0/cteTiposBasico_v4.00.xsd
 nfelib/cte/schemas/v4_0/cte_v4.00.xsd
 nfelib/cte/schemas/v4_0/evCCeCTe_v4.00.xsd
 nfelib/cte/schemas/v4_0/evCECTe_v4.00.xsd
 nfelib/cte/schemas/v4_0/evCancCECTe_v4.00.xsd
 nfelib/cte/schemas/v4_0/evCancCTe_v4.00.xsd
 nfelib/cte/schemas/v4_0/evCancIECTe_v4.00.xsd
@@ -184,14 +143,15 @@
 nfelib/cte/schemas/v4_0/inutCTe_v4.00.xsd
 nfelib/cte/schemas/v4_0/procCTeOS_v4.00.xsd
 nfelib/cte/schemas/v4_0/procCTe_v4.00.xsd
 nfelib/cte/schemas/v4_0/procEventoCTe_v4.00.xsd
 nfelib/cte/schemas/v4_0/procGTVe_v4.00.xsd
 nfelib/cte/schemas/v4_0/procInutCTe_v4.00.xsd
 nfelib/cte/schemas/v4_0/retCTeOS_v4.00.xsd
+nfelib/cte/schemas/v4_0/retCTeSimp_v4.00.xsd
 nfelib/cte/schemas/v4_0/retCTe_v4.00.xsd
 nfelib/cte/schemas/v4_0/retConsSitCTe_v4.00.xsd
 nfelib/cte/schemas/v4_0/retConsStatServCTe_v4.00.xsd
 nfelib/cte/schemas/v4_0/retEventoCTe_v4.00.xsd
 nfelib/cte/schemas/v4_0/retGTVe_v4.00.xsd
 nfelib/cte/schemas/v4_0/retInutCTe_v4.00.xsd
 nfelib/cte/schemas/v4_0/tiposGeralCTe_v4.00.xsd
@@ -245,53 +205,14 @@
 nfelib/mdfe/bindings/v3_0/ret_dist_mdfe_v3_00.py
 nfelib/mdfe/bindings/v3_0/ret_envi_mdfe_v3_00.py
 nfelib/mdfe/bindings/v3_0/ret_evento_mdfe_v3_00.py
 nfelib/mdfe/bindings/v3_0/ret_mdfe_consulta_dfe_v3_00.py
 nfelib/mdfe/bindings/v3_0/ret_mdfe_v3_00.py
 nfelib/mdfe/bindings/v3_0/tipos_geral_mdfe_v3_00.py
 nfelib/mdfe/bindings/v3_0/xmldsig_core_schema_v1_01.py
-nfelib/mdfe/odoo/__init__.py
-nfelib/mdfe/odoo/v3_0/cons_mdfe_nao_enc_tipos_basico_v3_00.py
-nfelib/mdfe/odoo/v3_0/cons_mdfe_nao_enc_v3_00.py
-nfelib/mdfe/odoo/v3_0/cons_reci_mdfe_tipos_basico_v3_00.py
-nfelib/mdfe/odoo/v3_0/cons_reci_mdfe_v3_00.py
-nfelib/mdfe/odoo/v3_0/cons_sit_mdfe_tipos_basico_v3_00.py
-nfelib/mdfe/odoo/v3_0/cons_sit_mdfe_v3_00.py
-nfelib/mdfe/odoo/v3_0/cons_stat_serv_mdfe_v3_00.py
-nfelib/mdfe/odoo/v3_0/cons_stat_serv_tipos_basico_v3_00.py
-nfelib/mdfe/odoo/v3_0/dist_mdfe_v3_00.py
-nfelib/mdfe/odoo/v3_0/envi_mdfe_v3_00.py
-nfelib/mdfe/odoo/v3_0/ev_canc_mdfe_v3_00.py
-nfelib/mdfe/odoo/v3_0/ev_enc_mdfe_v3_00.py
-nfelib/mdfe/odoo/v3_0/ev_inc_condutor_mdfe_v3_00.py
-nfelib/mdfe/odoo/v3_0/ev_inclusao_dfe_mdfe_v3_00.py
-nfelib/mdfe/odoo/v3_0/ev_pagto_oper_mdfe_v3_00.py
-nfelib/mdfe/odoo/v3_0/evento_mdfe_tipos_basico_v3_00.py
-nfelib/mdfe/odoo/v3_0/evento_mdfe_v3_00.py
-nfelib/mdfe/odoo/v3_0/leiaute_dist_mdfe_v3_00.py
-nfelib/mdfe/odoo/v3_0/mdfe_consulta_dfe_tipos_basico_v3_00.py
-nfelib/mdfe/odoo/v3_0/mdfe_consulta_dfe_v3_00.py
-nfelib/mdfe/odoo/v3_0/mdfe_modal_aereo_v3_00.py
-nfelib/mdfe/odoo/v3_0/mdfe_modal_aquaviario_v3_00.py
-nfelib/mdfe/odoo/v3_0/mdfe_modal_ferroviario_v3_00.py
-nfelib/mdfe/odoo/v3_0/mdfe_modal_rodoviario_v3_00.py
-nfelib/mdfe/odoo/v3_0/mdfe_tipos_basico_v3_00.py
-nfelib/mdfe/odoo/v3_0/mdfe_v3_00.py
-nfelib/mdfe/odoo/v3_0/proc_evento_mdfe_v3_00.py
-nfelib/mdfe/odoo/v3_0/proc_mdfe_v3_00.py
-nfelib/mdfe/odoo/v3_0/ret_cons_mdfe_nao_enc_v3_00.py
-nfelib/mdfe/odoo/v3_0/ret_cons_reci_mdfe_v3_00.py
-nfelib/mdfe/odoo/v3_0/ret_cons_sit_mdfe_v3_00.py
-nfelib/mdfe/odoo/v3_0/ret_cons_stat_serv_mdfe_v3_00.py
-nfelib/mdfe/odoo/v3_0/ret_dist_mdfe_v3_00.py
-nfelib/mdfe/odoo/v3_0/ret_envi_mdfe_v3_00.py
-nfelib/mdfe/odoo/v3_0/ret_evento_mdfe_v3_00.py
-nfelib/mdfe/odoo/v3_0/ret_mdfe_consulta_dfe_v3_00.py
-nfelib/mdfe/odoo/v3_0/ret_mdfe_v3_00.py
-nfelib/mdfe/odoo/v3_0/tipos_geral_mdfe_v3_00.py
 nfelib/mdfe/samples/v3_0/01010101010-ped-cons-mdfe-naoenc.xml
 nfelib/mdfe/samples/v3_0/26999999999999999999999999999999999999999991-mdfe.xml
 nfelib/mdfe/samples/v3_0/310000007934162-ped-rec.xml
 nfelib/mdfe/samples/v3_0/41190876676436000167580010000500001000437558-mdfe.xml
 nfelib/mdfe/samples/v3_0/50170876063965000276580010000011311421039568-mdfe.xml
 nfelib/mdfe/samples/v3_0/ComPagtoPIX_41210780568835000181580010402005751006005791-procMDFe.xml
 nfelib/mdfe/samples/v3_0/PagamentoOperacaoMDFe_1101164120039999999999999958001000000999999999999901-ped-eve.xml
@@ -577,14 +498,40 @@
 nfelib/nfe_evento_mde/schemas/v1_0/e210240_v1.00.xsd
 nfelib/nfe_evento_mde/schemas/v1_0/envConfRecebto_v1.00.xsd
 nfelib/nfe_evento_mde/schemas/v1_0/leiauteConfRecebto_v1.00.xsd
 nfelib/nfe_evento_mde/schemas/v1_0/procConfRecebtoNFe_v1.00.xsd
 nfelib/nfe_evento_mde/schemas/v1_0/retEnvConfRecebto_v1.00.xsd
 nfelib/nfe_evento_mde/schemas/v1_0/tiposBasico_v1.03.xsd
 nfelib/nfe_evento_mde/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
+nfelib/nfe_insucesso/__init__.py
+nfelib/nfe_insucesso/bindings/__init__.py
+nfelib/nfe_insucesso/bindings/v1_0/__init__.py
+nfelib/nfe_insucesso/bindings/v1_0/env_evento_insucesso_nfe_v1_00.py
+nfelib/nfe_insucesso/bindings/v1_0/evento_insucesso_nfe_v1_00.py
+nfelib/nfe_insucesso/bindings/v1_0/leiaute_evento_insucesso_nfe_v1_00.py
+nfelib/nfe_insucesso/bindings/v1_0/proc_evento_insucesso_nfe_v1_00.py
+nfelib/nfe_insucesso/bindings/v1_0/ret_evento_insucesso_nfe_v1_00.py
+nfelib/nfe_insucesso/bindings/v1_0/tipos_basico_v1_03.py
+nfelib/nfe_insucesso/bindings/v1_0/tmp0000.py
+nfelib/nfe_insucesso/bindings/v1_0/xmldsig_core_schema_v1_01.py
+nfelib/nfe_insucesso/schemas/v1_0/EventoCancInsucessoNFe_v1.00.xsd
+nfelib/nfe_insucesso/schemas/v1_0/EventoInsucessoNFe_v1.00.xsd
+nfelib/nfe_insucesso/schemas/v1_0/e110192_v1.00.xsd
+nfelib/nfe_insucesso/schemas/v1_0/e110193_v1.00.xsd
+nfelib/nfe_insucesso/schemas/v1_0/envEventoCancInsucessoNFe_v1.00.xsd
+nfelib/nfe_insucesso/schemas/v1_0/envEventoInsucessoNFe_v1.00.xsd
+nfelib/nfe_insucesso/schemas/v1_0/leiauteEventoCancInsucessoNFe_v1.00.xsd
+nfelib/nfe_insucesso/schemas/v1_0/leiauteEventoInsucessoNFe_v1.00.xsd
+nfelib/nfe_insucesso/schemas/v1_0/procEventoCancInsucessoNFe_v1.00.xsd
+nfelib/nfe_insucesso/schemas/v1_0/procEventoInsucessoNFe_v1.00.xsd
+nfelib/nfe_insucesso/schemas/v1_0/retEventoCancInsucessoNFe_v1.00.xsd
+nfelib/nfe_insucesso/schemas/v1_0/retEventoInsucessoNFe_v1.00.xsd
+nfelib/nfe_insucesso/schemas/v1_0/tiposBasico_v1.03.xsd
+nfelib/nfe_insucesso/schemas/v1_0/tmp0000.xsd
+nfelib/nfe_insucesso/schemas/v1_0/xmldsig-core-schema_v1.01.xsd
 nfelib/nfse/__init__.py
 nfelib/nfse/bindings/__init__.py
 nfelib/nfse/bindings/v1_0/__init__.py
 nfelib/nfse/bindings/v1_0/dps_v1_00.py
 nfelib/nfse/bindings/v1_0/evento_v1_00.py
 nfelib/nfse/bindings/v1_0/nfse_v1_00.py
 nfelib/nfse/bindings/v1_0/ped_reg_evento_v1_00.py
@@ -600,37 +547,14 @@
 nfelib/nfse/schemas/v1_0/NFSe_v1.00.xsd
 nfelib/nfse/schemas/v1_0/evento_v1.00.xsd
 nfelib/nfse/schemas/v1_0/pedRegEvento_v1.00.xsd
 nfelib/nfse/schemas/v1_0/tiposComplexos_v1.00.xsd
 nfelib/nfse/schemas/v1_0/tiposEventos_v1.00.xsd
 nfelib/nfse/schemas/v1_0/tiposSimples_v1.00.xsd
 nfelib/nfse/schemas/v1_0/xmldsig-core-schema_v1.00.xsd
-nfelib/odoo/__init__.py
-nfelib/odoo/nfe/__init__.py
-nfelib/odoo/nfe/v4_0/cons_cad_v2_00.py
-nfelib/odoo/nfe/v4_0/cons_reci_nfe_v4_00.py
-nfelib/odoo/nfe/v4_0/cons_sit_nfe_v4_00.py
-nfelib/odoo/nfe/v4_0/cons_stat_serv_v4_00.py
-nfelib/odoo/nfe/v4_0/envi_nfe_v4_00.py
-nfelib/odoo/nfe/v4_0/inut_nfe_v4_00.py
-nfelib/odoo/nfe/v4_0/leiaute_cons_sit_nfe_v4_00.py
-nfelib/odoo/nfe/v4_0/leiaute_cons_stat_serv_v4_00.py
-nfelib/odoo/nfe/v4_0/leiaute_consulta_cadastro_v2_00.py
-nfelib/odoo/nfe/v4_0/leiaute_inut_nfe_v4_00.py
-nfelib/odoo/nfe/v4_0/leiaute_nfe_v4_00.py
-nfelib/odoo/nfe/v4_0/nfe_v4_00.py
-nfelib/odoo/nfe/v4_0/proc_inut_nfe_v4_00.py
-nfelib/odoo/nfe/v4_0/proc_nfe_v4_00.py
-nfelib/odoo/nfe/v4_0/ret_cons_cad_v2_00.py
-nfelib/odoo/nfe/v4_0/ret_cons_reci_nfe_v4_00.py
-nfelib/odoo/nfe/v4_0/ret_cons_sit_nfe_v4_00.py
-nfelib/odoo/nfe/v4_0/ret_cons_stat_serv_v4_00.py
-nfelib/odoo/nfe/v4_0/ret_envi_nfe_v4_00.py
-nfelib/odoo/nfe/v4_0/ret_inut_nfe_v4_00.py
-nfelib/odoo/nfe/v4_0/tipos_basico_v4_00.py
 nfelib/v4_00/README.txt
 nfelib/v4_00/__init__.py
 nfelib/v4_00/distDFeInt.py
 nfelib/v4_00/leiauteNFe_sub.py
 nfelib/v4_00/retConsCad.py
 nfelib/v4_00/retConsReciNFe.py
 nfelib/v4_00/retConsSitNFe.py
@@ -640,15 +564,14 @@
 nfelib/v4_00/retEnvConfRecebto.py
 nfelib/v4_00/retEnvEvento.py
 nfelib/v4_00/retEnvEventoCancNFe.py
 nfelib/v4_00/retEnviNFe.py
 nfelib/v4_00/retInutNFe.py
 tests/__init__.py
 tests/fingerprint.txt
-tests/fingerprint_out.txt
 tests/input.xml
 tests/output.xml
 tests/output_cte.xml
 tests/output_mdfe.xml
 tests/output_nfe_evento_cce.xml
 tests/output_nfe_inut.xml
 tests/output_nfe_leiaute.xml
```

## Comparing `nfelib-2.0.4/nfelib.egg-info/PKG-INFO` & `nfelib-2.0.5/nfelib.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nfelib
-Version: 2.0.4
+Version: 2.0.5
 Summary: nfelib: electronic invoicing library for Brazil
 Home-page: https://github.com/akretion/nfelib
 Author: Raphaël Valyi
 Author-email: "raphael.valyi@akretion.com.br"
 License: MIT
 Project-URL: Source, https://github.com/akretion/nfelib
 Keywords: e-invoicing,NFe,ERP,Odoo,NFSe,CTe,MDFe,BPe
@@ -84,14 +84,36 @@
 Nfe(infNFe=Tnfe.InfNfe(ide=None, emit=Tnfe.InfNfe.Emit(CNPJ='59594315000157', CPF=None, xNome='Minha Empresa', xFant=None, enderEmit=None, IE=None, IEST=None, IM=None, CNAE=None, CRT=None), avulsa=None, dest=None, retirada=None, entrega=None, autXML=[], det=[], total=None, transp=None, cobr=None, pag=None, infIntermed=None, infAdic=None, exporta=None, compra=None, cana=None, infRespTec=None, infSolicNFF=None, versao=None, Id=None), infNFeSupl=None, signature=None)
 >>> 
 >>> # Validar o XML de uma nota:
 >>> nfe.validate_xml()
 ["Element '{http://www.portalfiscal.inf.br/nfe}infNFe': The attribute 'versao' is required but missing.", "Element '{http://www.portalfiscal.inf.br/nfe}infNFe': The attribute 'Id' is required but missing." [...]
 ```
 
+Assinar o XML de uma nota usando a lib [erpbrasil.assinatura](https://github.com/erpbrasil/erpbrasil.assinatura) (funciona com os outros documentos eletrônicos também)
+```
+>>> # Assinar o XML de uma nota:
+>>> with open(path_to_your_pkcs12_certificate, "rb") as pkcs12_buffer:
+    pkcs12_data = pkcs12_buffer.read()
+>>> signed_xml = nfe.sign_xml(xml, pkcs12_data, cert_password, nfe.NFe.infNFe.Id)
+```
+
+Imprimir o DANFE usando a lib [BrazilFiscalReport](https://github.com/Engenere/BrazilFiscalReport) ou a lib [erpbrasil.edoc.pdf](https://github.com/erpbrasil/erpbrasil.edoc.pdf) (futuramente BrazilFiscalReport deve imprimir o pdf de outros documentos eletrônicos também; erpbrasil.edoc.pdf é uma lib mais 'legacy')
+```
+>>> # Imprimir o pdf de uma nota usando BrazilFiscalReport:
+>>> pdf_bytes = nfe.to_pdf()
+>>> # Imprimir o pdf de uma nota usando erpbrasil.edoc.pdf:
+>>> pdf_bytes = nfe.to_pdf(engine="erpbrasil.edoc.pdf")
+>>> # Ou então para imprimir e assinar junto:
+>>> pdf_bytes = nfe.to_pdf(
+    pkcs12_data=cert_data,
+    pkcs12_password=cert_password,
+    doc_id=nfe.NFe.infNFe.Id,
+    )
+```
+
 **NFS-e padrão nacional**
 ```python
 >>> # Ler uma NFS-e:
 >>>> from nfelib.nfse.bindings.v1_0.nfse_v1_00 import Nfse
 >>> nfse = Nfse.from_path("alguma_nfse.xml")
 >>>
 >>> # Serializar uma NFS-e:
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nfelib Version: 2.0.4 Summary: nfelib: electronic
+Metadata-Version: 2.1 Name: nfelib Version: 2.0.5 Summary: nfelib: electronic
 invoicing library for Brazil Home-page: https://github.com/akretion/nfelib
 Author: RaphaÃ«l Valyi Author-email: "raphael.valyi@akretion.com.br" License:
 MIT Project-URL: Source, https://github.com/akretion/nfelib Keywords: e-
 invoicing,NFe,ERP,Odoo,NFSe,CTe,MDFe,BPe Platform: UNKNOWN Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python Classifier: Programming Language :: Python :: 3 Classifier:
@@ -54,17 +54,32 @@
 avulsa=None, dest=None, retirada=None, entrega=None, autXML=[], det=[],
 total=None, transp=None, cobr=None, pag=None, infIntermed=None, infAdic=None,
 exporta=None, compra=None, cana=None, infRespTec=None, infSolicNFF=None,
 versao=None, Id=None), infNFeSupl=None, signature=None) >>> >>> # Validar o XML
 de uma nota: >>> nfe.validate_xml() ["Element '{http://www.portalfiscal.inf.br/
 nfe}infNFe': The attribute 'versao' is required but missing.", "Element '{http:
 //www.portalfiscal.inf.br/nfe}infNFe': The attribute 'Id' is required but
-missing." [...] ``` **NFS-e padrÃ£o nacional** ```python >>> # Ler uma NFS-e:
->>>> from nfelib.nfse.bindings.v1_0.nfse_v1_00 import Nfse >>> nfse =
-Nfse.from_path("alguma_nfse.xml") >>> >>> # Serializar uma NFS-e: >>>
+missing." [...] ``` Assinar o XML de uma nota usando a lib
+[erpbrasil.assinatura](https://github.com/erpbrasil/erpbrasil.assinatura)
+(funciona com os outros documentos eletrÃ´nicos tambÃ©m) ``` >>> # Assinar o
+XML de uma nota: >>> with open(path_to_your_pkcs12_certificate, "rb") as
+pkcs12_buffer: pkcs12_data = pkcs12_buffer.read() >>> signed_xml = nfe.sign_xml
+(xml, pkcs12_data, cert_password, nfe.NFe.infNFe.Id) ``` Imprimir o DANFE
+usando a lib [BrazilFiscalReport](https://github.com/Engenere/
+BrazilFiscalReport) ou a lib [erpbrasil.edoc.pdf](https://github.com/erpbrasil/
+erpbrasil.edoc.pdf) (futuramente BrazilFiscalReport deve imprimir o pdf de
+outros documentos eletrÃ´nicos tambÃ©m; erpbrasil.edoc.pdf Ã© uma lib mais
+'legacy') ``` >>> # Imprimir o pdf de uma nota usando BrazilFiscalReport: >>>
+pdf_bytes = nfe.to_pdf() >>> # Imprimir o pdf de uma nota usando
+erpbrasil.edoc.pdf: >>> pdf_bytes = nfe.to_pdf(engine="erpbrasil.edoc.pdf") >>>
+# Ou entÃ£o para imprimir e assinar junto: >>> pdf_bytes = nfe.to_pdf
+( pkcs12_data=cert_data, pkcs12_password=cert_password,
+doc_id=nfe.NFe.infNFe.Id, ) ``` **NFS-e padrÃ£o nacional** ```python >>> # Ler
+uma NFS-e: >>>> from nfelib.nfse.bindings.v1_0.nfse_v1_00 import Nfse >>> nfse
+= Nfse.from_path("alguma_nfse.xml") >>> >>> # Serializar uma NFS-e: >>>
 nfse.to_xml() >>> # Ler uma DPS: >>>> from nfelib.nfse.bindings.v1_0.dps_v1_00
 import Dps >>> dps = Nfse.from_path("nfelib/nfse/samples/v1_0/GerarNFSeEnvio-
 env-loterps.xml") >>> >>> # Serializar uma DPS: >>> dps.to_xml() ``` **MDF-e**
 ```python >>> # Ler um MDF-e: >>>> from nfelib.mdfe.bindings.v3_0.mdfe_v3_00
 import Mdfe >>> mdfe = Mdfe.from_path("nfelib/mdfe/samples/v3_0/
 ComPagtoPIX_41210780568835000181580010402005751006005791-procMDFe.xml") >>> >>>
 # Serializar um MDF-e: >>> mdfe.to_xml() ``` **CT-e** ```python >>> # Ler um
```

## Comparing `nfelib-2.0.4/tests/test_fingerprint.py` & `nfelib-2.0.5/tests/test_fingerprint.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/tests/output_nfse.xml` & `nfelib-2.0.5/tests/output_nfse.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/tests/output_nfse_pedRegEvento.xml` & `nfelib-2.0.5/tests/output_nfse_pedRegEvento.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/tests/output_nfse_dps.xml` & `nfelib-2.0.5/tests/output_nfse_dps.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/tests/output_cte.xml` & `nfelib-2.0.5/tests/output_cte.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/tests/output.xml` & `nfelib-2.0.5/tests/output.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/tests/output_nfe_evento_cce.xml` & `nfelib-2.0.5/tests/output_nfe_evento_cce.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/tests/output_nfe_leiaute.xml` & `nfelib-2.0.5/tests/output_nfe_leiaute.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/tests/input.xml` & `nfelib-2.0.5/tests/input.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/tests/test_all.py` & `nfelib-2.0.5/tests/test_all.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/tests/nfse/test_nfse.py` & `nfelib-2.0.5/tests/nfse/test_nfse.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/tests/mdfe/test_mdfe.py` & `nfelib-2.0.5/tests/mdfe/test_mdfe.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/tests/nfe_evento_cce/test_cce.py` & `nfelib-2.0.5/tests/nfe_evento_cce/test_cce.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/tests/cte/test_cte.py` & `nfelib-2.0.5/tests/cte/test_cte.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/tests/cce/v1_00/leiauteCCe/35180803102452000172550010000476051695511860-01-cce.xml` & `nfelib-2.0.5/tests/cce/v1_00/leiauteCCe/35180803102452000172550010000476051695511860-01-cce.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/tests/nfe/test_nfe_legacy.py` & `nfelib-2.0.5/tests/nfe/test_nfe_legacy.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/tests/nfe/test_nfe.py` & `nfelib-2.0.5/tests/nfe/test_nfe.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,144 +1,186 @@
 # Copyright (C) 2019 - TODAY Raphaël Valyi - Akretion
 
 import os
 from pathlib import Path
+from unittest import TestCase
 
-from xmldiff import main
-from xsdata.formats.dataclass.parsers import XmlParser
-from xsdata.formats.dataclass.serializers import XmlSerializer
-from xsdata.formats.dataclass.serializers.config import SerializerConfig
-
-from nfelib.nfe.bindings.v4_0 import leiaute_nfe_v4_00
 from nfelib.nfe.bindings.v4_0.leiaute_cons_sit_nfe_v4_00 import TconsSitNfe
 from nfelib.nfe.bindings.v4_0.leiaute_cons_stat_serv_v4_00 import TconsStatServ
 from nfelib.nfe.bindings.v4_0.leiaute_nfe_v4_00 import Tnfe
 from nfelib.nfe.bindings.v4_0.nfe_v4_00 import Nfe
 from nfelib.nfe_dist_dfe.bindings.v1_0.dist_dfe_int_v1_01 import DistDfeInt
 from nfelib.nfe_evento_generico.bindings.v1_0.leiaute_evento_v1_00 import TenvEvento
+from xmldiff import main
+from xsdata.formats.dataclass.parsers import XmlParser
+from xsdata.formats.dataclass.serializers import XmlSerializer
+from xsdata.formats.dataclass.serializers.config import SerializerConfig
+
 
+class ClientTests(TestCase):
+    def test_patched_xsdata_for_ipi(self):
+        # o xsdata precisa de uma linha de patch para funcionar legal para a NFe
+        # (de forma simples/backward compatible no Odoo)
+        # uma alternativa seria usar a opção --compound-fields do xsdata mas
+        # deixaria o uso mais complexo no Odoo de forma desnecessaria. A gestão dos campos
+        # compostos/compound esta sendo retrabalhada no xsdata de qualquer forma.
+        # Enfim hoje o mais simples é aplicar um patch de uma linha no xsdata.
+        # Se vc instalar o pacote xsdata-odoo e fizer export XSD_SCHEMA=nfe,
+        # o xsdata-odoo aplica esse monkey patch para você.
+        # ver detalhes aqui: https://github.com/akretion/nfelib/issues/40
+        assert (
+            str(Tnfe.InfNfe.Det.Imposto().__annotations__["IPI"]).startswith(
+                "typing.Optional"
+            )
+            # Python < 3.9:
+            or str(Tnfe.InfNfe.Det.Imposto().__annotations__["IPI"])
+            == "typing.Union[nfelib.nfe.bindings.v4_0.leiaute_nfe_v4_00.Tipi, NoneType]"
+        )
 
-def test_patched_xsdata_for_ipi():
-    # o xsdata precisa de uma linha de patch para funcionar legal para a NFe
-    # (de forma simples/backward compatible no Odoo)
-    # uma alternativa seria usar a opção --compound-fields do xsdata mas
-    # deixaria o uso mais complexo no Odoo de forma desnecessaria. A gestão dos campos
-    # compostos/compound esta sendo retrabalhada no xsdata de qualquer forma.
-    # Enfim hoje o mais simples é aplicar um patch de uma linha no xsdata.
-    # Se vc instalar o pacote xsdata-odoo e fizer export XSD_SCHEMA=nfe,
-    # o xsdata-odoo aplica esse monkey patch para você.
-    # ver detalhes aqui: https://github.com/akretion/nfelib/issues/40
-    assert (
-        str(Tnfe.InfNfe.Det.Imposto().__annotations__["IPI"]).startswith(
-            "typing.Optional"
-        )
-        # Python < 3.9:
-        or str(Tnfe.InfNfe.Det.Imposto().__annotations__["IPI"])
-        == "typing.Union[nfelib.nfe.bindings.v4_0.leiaute_nfe_v4_00.Tipi, NoneType]"
-    )
-
-
-def test_in_out_leiauteNFe():
-    path = os.path.join("nfelib", "nfe", "samples", "v4_0", "leiauteNFe")
-    for filename in os.listdir(path):
+    def test_sign(self):
+        path = os.path.join("nfelib", "nfe", "samples", "v4_0", "leiauteNFe")
+        filename = "42210775277525000178550030000266631762885493-procNFe.xml"
         input_file = os.path.join(path, filename)
         parser = XmlParser()
-        obj = parser.from_path(Path(input_file))
-        serializer = XmlSerializer(config=SerializerConfig(pretty_print=True))
+        nfe = parser.from_path(Path(input_file))
+        serializer = XmlSerializer(config=SerializerConfig(pretty_print=False))
         xml = serializer.render(
-            obj=obj, ns_map={None: "http://www.portalfiscal.inf.br/nfe"}
+            obj=nfe, ns_map={None: "http://www.portalfiscal.inf.br/nfe"}
         )
-        # agora podemos trabalhar em cima do objeto e fazer operaçoes como:
-        #        obj.infNFe.emit.CNPJ
-
-        output_file = "tests/output_nfe_leiaute.xml"
-        with open(output_file, "w") as f:
-            f.write(xml)
+        self.assertNotIn("<X509Certificate>", xml)
+        valid = (True,)
+        cert_password = "123456"
+        issuer = "EMISSOR A TESTE"
+        country = "BR"
+        subject = "CERTIFICADO VALIDO TESTE"
+        from erpbrasil.assinatura import misc
 
-        diff = main.diff_files(input_file, output_file)
-        assert len(diff) == 0
-        if len(diff) != 0:
-            break
+        cert_data = misc.create_fake_certificate_file(
+            valid, cert_password, issuer, country, subject
+        )
+        signed_xml = nfe.sign_xml(xml, cert_data, cert_password, nfe.NFe.infNFe.Id)
+        self.assertIn("<X509Certificate>", signed_xml)
 
+        # this was an attempt to keep the signature inside the
+        # binding before serializing it again. But at the moment it fails
+        # because xsdata will serialize the Signature elements with their namespaces.
+        # signed_nfe = nfe.sign(cert_data, cert_password, nfe.NFe.infNFe.Id)
+        # signed_xml2 = signed_nfe.to_xml(pretty_print=False)
+        # self.assertEqual(signed_xml, signed_xml2)
+
+        pdf_bytes = nfe.to_pdf(
+            pkcs12_data=cert_data,
+            pkcs12_password=cert_password,
+            doc_id=nfe.NFe.infNFe.Id,
+        )
+        self.assertEqual(type(pdf_bytes), bytes)
 
-def test_in_out_leiauteInutNFe():
-    path = os.path.join("nfelib", "nfe", "samples", "v4_0", "leiauteInutNFe")
-    for filename in os.listdir(path):
+    def test_pdf(self):
+        path = os.path.join("nfelib", "nfe", "samples", "v4_0", "leiauteNFe")
+        filename = "42210775277525000178550030000266631762885493-procNFe.xml"
         input_file = os.path.join(path, filename)
         parser = XmlParser()
-        obj = parser.from_path(Path(input_file))
+        nfe = parser.from_path(Path(input_file))
+        pdf_bytes = nfe.to_pdf()
+        self.assertEqual(type(pdf_bytes), bytes)
+
+    def test_in_out_leiauteNFe(self):
+        path = os.path.join("nfelib", "nfe", "samples", "v4_0", "leiauteNFe")
+        for filename in os.listdir(path):
+            input_file = os.path.join(path, filename)
+            parser = XmlParser()
+            obj = parser.from_path(Path(input_file))
+            serializer = XmlSerializer(config=SerializerConfig(pretty_print=True))
+            xml = serializer.render(
+                obj=obj, ns_map={None: "http://www.portalfiscal.inf.br/nfe"}
+            )
+            # agora podemos trabalhar em cima do objeto e fazer operaçoes como:
+            #        obj.infNFe.emit.CNPJ
+
+            output_file = "tests/output_nfe_leiaute.xml"
+            with open(output_file, "w") as f:
+                f.write(xml)
+
+            diff = main.diff_files(input_file, output_file)
+            assert len(diff) == 0
+            if len(diff) != 0:
+                break
+
+    def test_in_out_leiauteInutNFe(self):
+        path = os.path.join("nfelib", "nfe", "samples", "v4_0", "leiauteInutNFe")
+        for filename in os.listdir(path):
+            input_file = os.path.join(path, filename)
+            parser = XmlParser()
+            obj = parser.from_path(Path(input_file))
+            serializer = XmlSerializer(config=SerializerConfig(pretty_print=True))
+            xml = serializer.render(
+                obj=obj, ns_map={None: "http://www.portalfiscal.inf.br/nfe"}
+            )
+
+            output_file = "tests/output_nfe_inut.xml"
+            with open(output_file, "w") as f:
+                f.write(xml)
+
+            diff = main.diff_files(input_file, output_file)
+            assert len(diff) == 0
+
+    def test_stat(self):
+        obj = TconsStatServ(
+            versao="4.00",
+            tpAmb="1",
+            cUF="12",
+            xServ="STATUS",
+        )
         serializer = XmlSerializer(config=SerializerConfig(pretty_print=True))
-        xml = serializer.render(
-            obj=obj, ns_map={None: "http://www.portalfiscal.inf.br/nfe"}
+        serializer.render(obj=obj)
+
+    def test_cons_sit(self):
+        obj = TconsSitNfe(
+            versao="4.00",
+            tpAmb="1",
+            xServ="CONSULTAR",
+            chNFe="NFe35180803102452000172550010000474641681223493",
         )
+        serializer = XmlSerializer(config=SerializerConfig(pretty_print=True))
+        serializer.render(obj=obj)
 
-        output_file = "tests/output_nfe_inut.xml"
-        with open(output_file, "w") as f:
-            f.write(xml)
-
-        diff = main.diff_files(input_file, output_file)
-        assert len(diff) == 0
-
-
-def test_stat():
-    obj = TconsStatServ(
-        versao="4.00",
-        tpAmb="1",
-        cUF="12",
-        xServ="STATUS",
-    )
-    serializer = XmlSerializer(config=SerializerConfig(pretty_print=True))
-    xml = serializer.render(obj=obj)
-
-
-def test_cons_sit():
-    obj = TconsSitNfe(
-        versao="4.00",
-        tpAmb="1",
-        xServ="CONSULTAR",
-        chNFe="NFe35180803102452000172550010000474641681223493",
-    )
-    serializer = XmlSerializer(config=SerializerConfig(pretty_print=True))
-    xml = serializer.render(obj=obj)
-
-
-def test_distDFe():
-    obj = DistDfeInt(
-        versao="4.00",
-        tpAmb="1",
-        cUFAutor="SP",
-        distNSU=DistDfeInt.DistNsu(
-            ultNSU="35180803102452000172550010000474641681223493"
-        ),
-        consNSU=DistDfeInt.ConsNsu(NSU="35180803102452000172550010000474641681223493"),
-    )
-    serializer = XmlSerializer(config=SerializerConfig(pretty_print=True))
-    xml = serializer.render(obj=obj)
-
-
-def test_evento_generico():
-    obj = TenvEvento(versao="1.00", idLote="42")
-    serializer = XmlSerializer(config=SerializerConfig(pretty_print=True))
-    xml = serializer.render(obj=obj)
-
-
-def test_validator():
-    path = os.path.join(
-        "nfelib",
-        "nfe",
-        "samples",
-        "v4_0",
-        "leiauteNFe",
-        "NFe35200159594315000157550010000000012062777161.xml",
-    )
-    parser = XmlParser()
-    nfe_proc = parser.from_path(Path(path))
-    assert (
-        len(Nfe(infNFe=nfe_proc.NFe.infNFe).validate_xml()) == 3
-    )  # (we know this file has 3 schema errors)
+    def test_distDFe(self):
+        obj = DistDfeInt(
+            versao="4.00",
+            tpAmb="1",
+            cUFAutor="SP",
+            distNSU=DistDfeInt.DistNsu(
+                ultNSU="35180803102452000172550010000474641681223493"
+            ),
+            consNSU=DistDfeInt.ConsNsu(
+                NSU="35180803102452000172550010000474641681223493"
+            ),
+        )
+        serializer = XmlSerializer(config=SerializerConfig(pretty_print=True))
+        serializer.render(obj=obj)
+
+    def test_evento_generico(self):
+        obj = TenvEvento(versao="1.00", idLote="42")
+        serializer = XmlSerializer(config=SerializerConfig(pretty_print=True))
+        serializer.render(obj=obj)
+
+    def test_validator(self):
+        path = os.path.join(
+            "nfelib",
+            "nfe",
+            "samples",
+            "v4_0",
+            "leiauteNFe",
+            "NFe35200159594315000157550010000000012062777161.xml",
+        )
+        parser = XmlParser()
+        nfe_proc = parser.from_path(Path(path))
+        assert (
+            len(Nfe(infNFe=nfe_proc.NFe.infNFe).validate_xml()) == 3
+        )  # (we know this file has 3 schema errors)
 
 
 # def test_evento_cancelamento():
 #     retEnvEventoCancNFe.TEvento()
 #     retEnvEventoCancNFe.infEventoType()
 #     retEnvEventoCancNFe.detEventoType()
```

## Comparing `nfelib-2.0.4/nfelib/nfse/samples/v1_0/ConsultarNFSeRPS-ped-sitnfserps.xml` & `nfelib-2.0.5/nfelib/nfse/samples/v1_0/ConsultarNFSeRPS-ped-sitnfserps.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfse/samples/v1_0/GerarNFSeEnvio-env-loterps.xml` & `nfelib-2.0.5/nfelib/nfse/samples/v1_0/GerarNFSeEnvio-env-loterps.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfse/samples/v1_0/CancelarNFSe-ped-cannfse.xml` & `nfelib-2.0.5/nfelib/nfse/samples/v1_0/CancelarNFSe-ped-cannfse.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfse/samples/v1_0/ConsultarNFSeEnvio-ped-sitnfse.xml` & `nfelib-2.0.5/nfelib/nfse/samples/v1_0/ConsultarNFSeEnvio-ped-sitnfse.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfse/bindings/v1_0/__init__.py` & `nfelib-2.0.5/nfelib/nfse/bindings/v1_0/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""This file was generated by xsdata, v24.2.1, on 2024-03-11 16:13:50
+
+Generator: DataclassGenerator
+See: https://xsdata.readthedocs.io/
+"""
 from nfelib.nfse.bindings.v1_0.dps_v1_00 import Dps
 from nfelib.nfse.bindings.v1_0.evento_v1_00 import Evento
 from nfelib.nfse.bindings.v1_0.nfse_v1_00 import Nfse
 from nfelib.nfse.bindings.v1_0.ped_reg_evento_v1_00 import PedRegEvento
 from nfelib.nfse.bindings.v1_0.tipos_complexos_v1_00 import (
     TcatvEvento,
     TcbeneficioMunicipal,
```

## Comparing `nfelib-2.0.4/nfelib/nfse/bindings/v1_0/tipos_eventos_v1_00.py` & `nfelib-2.0.5/nfelib/nfse/bindings/v1_0/tipos_eventos_v1_00.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,15 @@
+"""This file was generated by xsdata, v24.2.1, on 2024-03-11 16:13:50
+
+Generator: DataclassGenerator
+See: https://xsdata.readthedocs.io/
+"""
 from dataclasses import dataclass, field
 from enum import Enum
+from nfelib import CommonMixin
 from typing import List, Optional
 from nfelib.nfse.bindings.v1_0.tipos_simples_v1_00 import (
     TsambGeradorEvt,
     TscodJustAnaliseFiscalCanc,
     TscodJustAnaliseFiscalCancDef,
     TscodJustAnaliseFiscalCancIndef,
     TscodJustCanc,
@@ -14,78 +20,87 @@
 )
 from nfelib.nfse.bindings.v1_0.xmldsig_core_schema_v1_00 import Signature
 
 __NAMESPACE__ = "http://www.sped.fazenda.gov.br/nfse"
 
 
 @dataclass
-class TcinfoEventoAnulacaoRejeicao:
+class TcinfoEventoAnulacaoRejeicao(CommonMixin):
     """
     :ivar CPFAgTrib: CPF do agente da administração tributária municipal
         que efetuou o anulação da manifestação de rejeição da NFS-e.
     :ivar idEvManifRej: Referência ao Id da "Manifestação de rejeição da
         NFS-e" que originou o presente evento de anulação.
     :ivar xMotivo: Descrição para explicitar o motivo da anluação
     """
+
     class Meta:
         name = "TCInfoEventoAnulacaoRejeicao"
 
     CPFAgTrib: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "max_length": 11,
             "white_space": "preserve",
             "pattern": r"[0-9]{11}",
-        }
+        },
     )
     idEvManifRej: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "white_space": "preserve",
             "pattern": r"[0-9]{59}",
-        }
+        },
     )
     xMotivo: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "min_length": 15,
             "max_length": 255,
             "white_space": "preserve",
             "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
-        }
+        },
     )
 
 
 class Te101101XDesc(Enum):
     CANCELAMENTO_DE_NFS_E = "Cancelamento de NFS-e"
 
 
 class Te101103XDesc(Enum):
-    SOLICITACAO_DE_ANALISE_FISCAL_PARA_CANCELAMENTO_DE_NFS_E = "Solicitacao de Analise Fiscal para Cancelamento de NFS-e"
+    SOLICITACAO_DE_ANALISE_FISCAL_PARA_CANCELAMENTO_DE_NFS_E = (
+        "Solicitacao de Analise Fiscal para Cancelamento de NFS-e"
+    )
 
 
 class Te105102XDesc(Enum):
-    CANCELAMENTO_DE_NFS_E_POR_SUBSTITUICAO = "Cancelamento de NFS-e por Substituicao"
+    CANCELAMENTO_DE_NFS_E_POR_SUBSTITUICAO = (
+        "Cancelamento de NFS-e por Substituicao"
+    )
 
 
 class Te105104XDesc(Enum):
-    CANCELAMENTO_DE_NFS_E_DEFERIDO_POR_AN_LISE_FISCAL = "Cancelamento de NFS-e Deferido por Análise Fiscal"
+    CANCELAMENTO_DE_NFS_E_DEFERIDO_POR_AN_LISE_FISCAL = (
+        "Cancelamento de NFS-e Deferido por Análise Fiscal"
+    )
 
 
 class Te105105XDesc(Enum):
-    CANCELAMENTO_DE_NFS_E_INDEFERIDO_POR_AN_LISE_FISCAL = "Cancelamento de NFS-e Indeferido por Análise Fiscal"
+    CANCELAMENTO_DE_NFS_E_INDEFERIDO_POR_AN_LISE_FISCAL = (
+        "Cancelamento de NFS-e Indeferido por Análise Fiscal"
+    )
 
 
 class Te202201XDesc(Enum):
     CONFIRMA_O_DO_PRESTADOR = "Confirmação do Prestador"
 
 
 class Te202205XDesc(Enum):
@@ -125,284 +140,290 @@
 
 
 class Te305103XDesc(Enum):
     DESBLOQUEIO_DE_NFS_E_POR_OF_CIO = "Desbloqueio de NFS-e por Ofício"
 
 
 @dataclass
-class TcinfoEventoRejeicao:
+class TcinfoEventoRejeicao(CommonMixin):
     """
     :ivar cMotivo: Motivo da Rejeição da NFS-e: 1 - NFS-e em
         duplicidade; 2 - NFS-e já emitida pelo tomador; 3 - Não
         ocorrência do fato gerador; 4 - Erro quanto a responsabilidade
         tributária; 5 - Erro quanto ao valor do serviço, valor das
         deduções ou serviço prestado ou data do fato gerador; 9 -
         Outros;
     :ivar xMotivo: Descrição para explicitar o motivo indicado neste
         evento
     """
+
     class Meta:
         name = "TCInfoEventoRejeicao"
 
     cMotivo: Optional[TscodMotivoRejeicao] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
     xMotivo: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "min_length": 15,
             "max_length": 255,
             "white_space": "preserve",
             "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
-        }
+        },
     )
 
 
 @dataclass
-class TclistaEventos:
+class TclistaEventos(CommonMixin):
     """
     :ivar codEvento: Grupo de informações de documento utilizado para
         Dedução/Redução do valor do serviço
     """
+
     class Meta:
         name = "TCListaEventos"
 
     codEvento: List[TscodigoEventoNfse] = field(
         default_factory=list,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "min_occurs": 1,
             "max_occurs": 9,
-        }
+        },
     )
 
 
 @dataclass
-class Te101101:
+class Te101101(CommonMixin):
     """
     :ivar xDesc: Descrição do Evento: Descrição do evento: "Cancelamento
         de NFS-e".
     :ivar cMotivo: Código de justificativa de cancelamento
     :ivar xMotivo: Descrição para explicitar o motivo indicado neste
         evento
     """
+
     class Meta:
         name = "TE101101"
 
     xDesc: Optional[Te101101XDesc] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "white_space": "preserve",
-        }
+        },
     )
     cMotivo: Optional[TscodJustCanc] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
     xMotivo: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "min_length": 15,
             "max_length": 255,
             "white_space": "preserve",
             "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
-        }
+        },
     )
 
 
 @dataclass
-class Te101103:
+class Te101103(CommonMixin):
     """
     :ivar xDesc: Descrição do evento: "Solicitação de Análise Fiscal
         para Cancelamento de NFS-e"
     :ivar cMotivo: Código do motivo da solicitação de análise fiscal
         para cancelamento de NFS-e:
     :ivar xMotivo: Descrição para explicitar o motivo indicado neste
         evento
     """
+
     class Meta:
         name = "TE101103"
 
     xDesc: Optional[Te101103XDesc] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "white_space": "preserve",
-        }
+        },
     )
     cMotivo: Optional[TscodJustAnaliseFiscalCanc] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
     xMotivo: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "min_length": 15,
             "max_length": 255,
             "white_space": "preserve",
             "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
-        }
+        },
     )
 
 
 @dataclass
-class Te105102:
+class Te105102(CommonMixin):
     """
     :ivar xDesc: Descrição do Evento: Descrição do evento: "Cancelamento
         de NFS-e por Substituição".
     :ivar cMotivo: Código de justificativa de cancelamento substituição
     :ivar xMotivo: Descrição para explicitar o motivo indicado neste
         evento
     :ivar chSubstituta: Chave de Acesso da NFS-e substituta.
     """
+
     class Meta:
         name = "TE105102"
 
     xDesc: Optional[Te105102XDesc] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "white_space": "preserve",
-        }
+        },
     )
     cMotivo: Optional[TscodJustSubst] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
     xMotivo: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "min_length": 15,
             "max_length": 255,
             "white_space": "preserve",
             "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
-        }
+        },
     )
     chSubstituta: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "max_length": 50,
             "white_space": "preserve",
             "pattern": r"[0-9]{50}",
-        }
+        },
     )
 
 
 @dataclass
-class Te105104:
+class Te105104(CommonMixin):
     """
     :ivar xDesc: Descrição do evento: "Cancelamento de NFS-e Deferido
         por Análise Fiscal"
     :ivar CPFAgTrib: CPF do agente da administração tributária municipal
         que efetuou o deferimento da  solicitação de análise fiscal para
         cancelamento de NFS-e.
     :ivar nProcAdm: Número do processo administrativo municipal
         vinculado à solicitação de análise fiscal para cancelamento de
         NFS-e.
     :ivar cMotivo: Resposta da solicitação de análise fiscal para
         cancelamento de NFS-e: 1 - Cancelamento de NFS-e Deferido.
     :ivar xMotivo: Descrição para explicitar o motivo indicado neste
         evento
     """
+
     class Meta:
         name = "TE105104"
 
     xDesc: Optional[Te105104XDesc] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "white_space": "preserve",
-        }
+        },
     )
     CPFAgTrib: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "max_length": 11,
             "white_space": "preserve",
             "pattern": r"[0-9]{11}",
-        }
+        },
     )
     nProcAdm: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "min_length": 1,
             "max_length": 30,
             "white_space": "preserve",
             "pattern": r"[0-9]{1,30}",
-        }
+        },
     )
     cMotivo: Optional[TscodJustAnaliseFiscalCancDef] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
     xMotivo: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "min_length": 15,
             "max_length": 255,
             "white_space": "preserve",
             "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
-        }
+        },
     )
 
 
 @dataclass
-class Te105105:
+class Te105105(CommonMixin):
     """
     :ivar xDesc: Descrição do evento: "Cancelamento de NFS-e Indeferido
         por Análise Fiscal".
     :ivar CPFAgTrib: CPF do agente da administração tributária municipal
         que efetuou o indeferimento da solicitação de análise fiscal
         para cancelamento de NFS-e.
     :ivar nProcAdm: Número do processo administrativo municipal
@@ -410,421 +431,433 @@
         NFS-e.
     :ivar cMotivo: Resposta da solicitação de análise fiscal para
         cancelamento de NFS-e: 1 - Cancelamento de NFS-e Indeferido; 2 -
         Cancelamento de NFS-e Indeferido Sem Análise de Mérito.
     :ivar xMotivo: Descrição para explicitar o motivo indicado neste
         evento
     """
+
     class Meta:
         name = "TE105105"
 
     xDesc: Optional[Te105105XDesc] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "white_space": "preserve",
-        }
+        },
     )
     CPFAgTrib: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "max_length": 11,
             "white_space": "preserve",
             "pattern": r"[0-9]{11}",
-        }
+        },
     )
     nProcAdm: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "min_length": 1,
             "max_length": 30,
             "white_space": "preserve",
             "pattern": r"[0-9]{1,30}",
-        }
+        },
     )
     cMotivo: Optional[TscodJustAnaliseFiscalCancIndef] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
     xMotivo: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "min_length": 15,
             "max_length": 255,
             "white_space": "preserve",
             "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
-        }
+        },
     )
 
 
 @dataclass
-class Te202201:
+class Te202201(CommonMixin):
     """
     :ivar xDesc: Descrição do evento: "Confirmação do Prestador".
     """
+
     class Meta:
         name = "TE202201"
 
     xDesc: Optional[Te202201XDesc] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "white_space": "preserve",
-        }
+        },
     )
 
 
 @dataclass
-class Te203202:
+class Te203202(CommonMixin):
     """
     :ivar xDesc: Descrição do evento: "Confirmação do Tomador".
     """
+
     class Meta:
         name = "TE203202"
 
     xDesc: Optional[Te203202XDesc] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "white_space": "preserve",
-        }
+        },
     )
 
 
 @dataclass
-class Te204203:
+class Te204203(CommonMixin):
     """
     :ivar xDesc: Descrição do evento: "Confirmação do Intermediário".
     """
+
     class Meta:
         name = "TE204203"
 
     xDesc: Optional[Te204203XDesc] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "white_space": "preserve",
-        }
+        },
     )
 
 
 @dataclass
-class Te205204:
+class Te205204(CommonMixin):
     """
     :ivar xDesc: Descrição do evento: "Confirmação Tácita".
     """
+
     class Meta:
         name = "TE205204"
 
     xDesc: Optional[Te205204XDesc] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "white_space": "preserve",
-        }
+        },
     )
 
 
 @dataclass
-class Te205208:
+class Te205208(CommonMixin):
     """
     :ivar xDesc: Descrição do evento: "Anulação da Rejeição".
     :ivar infAnRej:
     """
+
     class Meta:
         name = "TE205208"
 
     xDesc: Optional[Te205208XDesc] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "white_space": "preserve",
-        }
+        },
     )
     infAnRej: Optional[TcinfoEventoAnulacaoRejeicao] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
 
 
 @dataclass
-class Te305101:
+class Te305101(CommonMixin):
     """
     :ivar xDesc: Descrição do evento: "Cancelamento de NFS-e por
         Ofício".
     :ivar CPFAgTrib: CPF do agente da administração tributária municipal
         que efetuou o cancelamento por ofício de NFS-e.
     :ivar nProcAdm: Número do processo administrativo municipal
         vinculado ao cancelamento de NFS-e por ofício.
     :ivar xProcAdm: Descrição para explicitar o motivo indicado neste
         evento.
     """
+
     class Meta:
         name = "TE305101"
 
     xDesc: Optional[Te305101XDesc] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "white_space": "preserve",
-        }
+        },
     )
     CPFAgTrib: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "max_length": 11,
             "white_space": "preserve",
             "pattern": r"[0-9]{11}",
-        }
+        },
     )
     nProcAdm: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "min_length": 1,
             "max_length": 30,
             "white_space": "preserve",
             "pattern": r"[0-9]{1,30}",
-        }
+        },
     )
     xProcAdm: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "min_length": 15,
             "max_length": 255,
             "white_space": "preserve",
             "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
-        }
+        },
     )
 
 
 @dataclass
-class Te305102:
+class Te305102(CommonMixin):
     """
     :ivar xDesc: Descrição do evento: "Bloqueio de NFS-e por Ofício".
     :ivar CPFAgTrib: CPF do agente da administração tributária municipal
         que efetuou o cancelamento por ofício de NFS-e.
     :ivar xMotivo: Descrição para explicitar o motivo indicado neste
         evento
     :ivar codEvento: Descrição para explicitar o motivo indicado neste
         evento
     """
+
     class Meta:
         name = "TE305102"
 
     xDesc: Optional[Te305102XDesc] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "white_space": "preserve",
-        }
+        },
     )
     CPFAgTrib: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "max_length": 11,
             "white_space": "preserve",
             "pattern": r"[0-9]{11}",
-        }
+        },
     )
     xMotivo: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "min_length": 15,
             "max_length": 255,
             "white_space": "preserve",
             "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
-        }
+        },
     )
     codEvento: Optional[TscodigoEventoNfse] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
 
 
 @dataclass
-class Te305103:
+class Te305103(CommonMixin):
     """
     :ivar xDesc: Descrição do evento: "Desbloqueio de NFS-e por Ofício".
     :ivar CPFAgTrib: CPF do agente da administração tributária municipal
         que efetuou o cancelamento por ofício de NFS-e.
     :ivar idBloqOfic: Referência ao Id da "Manifestação de rejeição da
         NFS-e" que originou o presente evento de anulação.
     """
+
     class Meta:
         name = "TE305103"
 
     xDesc: Optional[Te305103XDesc] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "white_space": "preserve",
-        }
+        },
     )
     CPFAgTrib: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "max_length": 11,
             "white_space": "preserve",
             "pattern": r"[0-9]{11}",
-        }
+        },
     )
     idBloqOfic: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "white_space": "preserve",
             "pattern": r"[0-9]{59}",
-        }
+        },
     )
 
 
 @dataclass
-class Te202205:
+class Te202205(CommonMixin):
     """
     :ivar xDesc: Descrição do evento: "Rejeição do Prestador".
     :ivar infRej:
     """
+
     class Meta:
         name = "TE202205"
 
     xDesc: Optional[Te202205XDesc] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "white_space": "preserve",
-        }
+        },
     )
     infRej: Optional[TcinfoEventoRejeicao] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
 
 
 @dataclass
-class Te203206:
+class Te203206(CommonMixin):
     """
     :ivar xDesc: Descrição do evento: "Rejeição do Tomador".
     :ivar infRej:
     """
+
     class Meta:
         name = "TE203206"
 
     xDesc: Optional[Te203206XDesc] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "white_space": "preserve",
-        }
+        },
     )
     infRej: Optional[TcinfoEventoRejeicao] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
 
 
 @dataclass
-class Te204207:
+class Te204207(CommonMixin):
     """
     :ivar xDesc: Descrição do evento: "Rejeição do Intermediário".
     :ivar infRej:
     """
+
     class Meta:
         name = "TE204207"
 
     xDesc: Optional[Te204207XDesc] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "white_space": "preserve",
-        }
+        },
     )
     infRej: Optional[TcinfoEventoRejeicao] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
 
 
 @dataclass
-class TcinfPedReg:
+class TcinfPedReg(CommonMixin):
     """
     :ivar tpAmb: Identificação do Ambiente: 1 - Produção; 2 -
         Homologação
     :ivar verAplic: Versão do aplicativo que gerou o pedido de registro
         de evento.
     :ivar dhEvento: Data e hora do evento no formato AAAA-MM-
         DDThh:mm:ssTZD (UTC - Universal Coordinated Time, onde TZD pode
@@ -854,247 +887,248 @@
     :ivar e204207: Rejeição do Intermediário
     :ivar e205208: Anulação da Rejeição
     :ivar e305101: Cancelamento de NFS-e por Ofício
     :ivar e305102: Bloqueio de NFS-e por Ofício
     :ivar e305103: Desbloqueio de NFS-e por Ofício
     :ivar Id:
     """
+
     class Meta:
         name = "TCInfPedReg"
 
     tpAmb: Optional[TstipoAmbiente] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
     verAplic: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "min_length": 1,
             "max_length": 20,
             "white_space": "preserve",
             "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
-        }
+        },
     )
     dhEvento: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "white_space": "preserve",
             "pattern": r"(((20(([02468][048])|([13579][26]))-02-29))|(20[0-9][0-9])-((((0[1-9])|(1[0-2]))-((0[1-9])|(1\d)|(2[0-8])))|((((0[13578])|(1[02]))-31)|(((0[1,3-9])|(1[0-2]))-(29|30)))))T(20|21|22|23|[0-1]\d):[0-5]\d:[0-5]\d([\-,\+](0[0-9]|10|11):00|([\+](12):00))",
-        }
+        },
     )
     CNPJAutor: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "max_length": 14,
             "white_space": "preserve",
             "pattern": r"[0-9]{14}",
-        }
+        },
     )
     CPFAutor: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "max_length": 11,
             "white_space": "preserve",
             "pattern": r"[0-9]{11}",
-        }
+        },
     )
     chNFSe: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "max_length": 50,
             "white_space": "preserve",
             "pattern": r"[0-9]{50}",
-        }
+        },
     )
     nPedRegEvento: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "max_length": 3,
             "white_space": "preserve",
             "pattern": r"[0-9]{1}[0-9]{0,2}",
-        }
+        },
     )
     e101101: Optional[Te101101] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
-        }
+        },
     )
     e105102: Optional[Te105102] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
-        }
+        },
     )
     e101103: Optional[Te101103] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
-        }
+        },
     )
     e105104: Optional[Te105104] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
-        }
+        },
     )
     e105105: Optional[Te105105] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
-        }
+        },
     )
     e202201: Optional[Te202201] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
-        }
+        },
     )
     e203202: Optional[Te203202] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
-        }
+        },
     )
     e204203: Optional[Te204203] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
-        }
+        },
     )
     e205204: Optional[Te205204] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
-        }
+        },
     )
     e202205: Optional[Te202205] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
-        }
+        },
     )
     e203206: Optional[Te203206] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
-        }
+        },
     )
     e204207: Optional[Te204207] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
-        }
+        },
     )
     e205208: Optional[Te205208] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
-        }
+        },
     )
     e305101: Optional[Te305101] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
-        }
+        },
     )
     e305102: Optional[Te305102] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
-        }
+        },
     )
     e305103: Optional[Te305103] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
-        }
+        },
     )
     Id: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "required": True,
             "max_length": 62,
             "white_space": "preserve",
             "pattern": r"PRE[0-9]{59}",
-        }
+        },
     )
 
 
 @dataclass
-class TcpedRegEvt:
+class TcpedRegEvt(CommonMixin):
     class Meta:
         name = "TCPedRegEvt"
 
     infPedReg: Optional[TcinfPedReg] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
     signature: Optional[Signature] = field(
         default=None,
         metadata={
             "name": "Signature",
             "type": "Element",
             "namespace": "http://www.w3.org/2000/09/xmldsig#",
-        }
+        },
     )
     versao: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "required": True,
             "white_space": "preserve",
             "pattern": r"1\.00",
-        }
+        },
     )
 
 
 @dataclass
-class TcinfEvento:
+class TcinfEvento(CommonMixin):
     """
     :ivar verAplic: Versão do aplicativo que gerou o pedido do evento.
     :ivar ambGer: Ambiente gerador do evento
     :ivar nSeqEvento: Sequencial do evento para o mesmo tipo de evento.
         Para maioria dos eventos nSeqEvento=1. Nos casos em que possa
         existir mais de um evento do mesmo tipo o ambiente gerador
         deverá numerar de forma sequencial.
@@ -1102,111 +1136,112 @@
         formato UTC (Universal Coordinated Time): AAAA-MM-
         DDThh:mm:ssTZD"
     :ivar nDFe: Ambiente gerador do evento
     :ivar pedRegEvento: Leiaute do pedido de registro do evento gerado
         pelo autor do evento
     :ivar Id:
     """
+
     class Meta:
         name = "TCInfEvento"
 
     verAplic: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "min_length": 1,
             "max_length": 20,
             "white_space": "preserve",
             "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
-        }
+        },
     )
     ambGer: Optional[TsambGeradorEvt] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
     nSeqEvento: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "max_length": 3,
             "white_space": "preserve",
             "pattern": r"[0-9]{1}[0-9]{0,2}",
-        }
+        },
     )
     dhProc: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "white_space": "preserve",
             "pattern": r"(((20(([02468][048])|([13579][26]))-02-29))|(20[0-9][0-9])-((((0[1-9])|(1[0-2]))-((0[1-9])|(1\d)|(2[0-8])))|((((0[13578])|(1[02]))-31)|(((0[1,3-9])|(1[0-2]))-(29|30)))))T(20|21|22|23|[0-1]\d):[0-5]\d:[0-5]\d([\-,\+](0[0-9]|10|11):00|([\+](12):00))",
-        }
+        },
     )
     nDFe: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "white_space": "preserve",
             "pattern": r"[0-9]{1,13}",
-        }
+        },
     )
     pedRegEvento: Optional[TcpedRegEvt] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
     Id: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "required": True,
             "max_length": 62,
             "white_space": "preserve",
             "pattern": r"EVT[0-9]{59}",
-        }
+        },
     )
 
 
 @dataclass
-class Tcevento:
+class Tcevento(CommonMixin):
     class Meta:
         name = "TCEvento"
 
     infEvento: Optional[TcinfEvento] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
     signature: Optional[Signature] = field(
         default=None,
         metadata={
             "name": "Signature",
             "type": "Element",
             "namespace": "http://www.w3.org/2000/09/xmldsig#",
             "required": True,
-        }
+        },
     )
     versao: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "required": True,
             "white_space": "preserve",
             "pattern": r"1\.00",
-        }
+        },
     )
```

## Comparing `nfelib-2.0.4/nfelib/nfse/bindings/v1_0/tipos_complexos_v1_00.py` & `nfelib-2.0.5/nfelib/nfse/bindings/v1_0/tipos_complexos_v1_00.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,14 @@
+"""This file was generated by xsdata, v24.2.1, on 2024-03-11 16:13:50
+
+Generator: DataclassGenerator
+See: https://xsdata.readthedocs.io/
+"""
 from dataclasses import dataclass, field
+from nfelib import CommonMixin
 from typing import List, Optional
 from xsdata.models.datatype import XmlDate
 from nfelib.nfse.bindings.v1_0.tipos_simples_v1_00 import (
     TcobjetoLocacao,
     TsambGeradorNfse,
     TscategVeic,
     TscategoriaServico,
@@ -37,609 +43,621 @@
 )
 from nfelib.nfse.bindings.v1_0.xmldsig_core_schema_v1_00 import Signature
 
 __NAMESPACE__ = "http://www.sped.fazenda.gov.br/nfse"
 
 
 @dataclass
-class Tccserv:
+class Tccserv(CommonMixin):
     """
     :ivar cTribNac: Código de tributação nacional do ISSQN: Regra de
         formação - 6 dígitos numéricos sendo: 2 para Item (LC 116/2003),
         2 para Subitem (LC 116/2003) e 2 para Desdobro Nacional
     :ivar cTribMun: Código de tributação municipal do ISSQN
     :ivar xDescServ: Descrição completa do serviço prestado
     :ivar cNBS: Código NBS (Nomenclatura Brasileira de Serviços,
         Intangíveis e outras Operações que produzam Variações no
         Patrimônio) correspondente ao serviço prestado
     :ivar cIntContrib: Código interno do contribuinte
     """
+
     class Meta:
         name = "TCCServ"
 
     cTribNac: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "white_space": "preserve",
             "pattern": r"[0-9]{6}",
-        }
+        },
     )
     cTribMun: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "white_space": "preserve",
             "pattern": r"[0-9]{3}",
-        }
+        },
     )
     xDescServ: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "min_length": 1,
             "max_length": 2000,
             "white_space": "preserve",
             "pattern": r"[\s\S!-ÿ]{1}[\s\S -ÿ]{0,}[\s\S!-ÿ]{1}|[\s\S!-ÿ]{1}",
-        }
+        },
     )
     cNBS: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "white_space": "preserve",
             "pattern": r"[0-9]{9}",
-        }
+        },
     )
     cIntContrib: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "min_length": 1,
             "max_length": 20,
             "white_space": "preserve",
             "pattern": r"[a-zA-Z0-9]{1,20}",
-        }
+        },
     )
 
 
 @dataclass
-class TcdocNfnfs:
+class TcdocNfnfs(CommonMixin):
     """
     :ivar nNFS: Número da Nota Fiscal NF ou NFS
     :ivar modNFS: Modelo da Nota Fiscal NF ou NFS
     :ivar serieNFS: Série Nota Fiscal NF ou NFS
     """
+
     class Meta:
         name = "TCDocNFNFS"
 
     nNFS: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "max_length": 7,
             "white_space": "preserve",
             "pattern": r"[0-9]{7}",
-        }
+        },
     )
     modNFS: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "max_length": 15,
             "white_space": "preserve",
             "pattern": r"[0-9]{15}",
-        }
+        },
     )
     serieNFS: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "min_length": 1,
             "max_length": 15,
             "white_space": "preserve",
             "pattern": r"[a-zA-Z0-9]{1,15}",
-        }
+        },
     )
 
 
 @dataclass
-class TcdocOutNfse:
+class TcdocOutNfse(CommonMixin):
     """
     :ivar cMunNFSeMun: Código Município emissor da nota eletrônica
         municipal (Tabela do IBGE)
     :ivar nNFSeMun: Número da nota eletrônica municipal
     :ivar cVerifNFSeMun: Código de Verificação da nota eletrônica
         municipal
     """
+
     class Meta:
         name = "TCDocOutNFSe"
 
     cMunNFSeMun: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "white_space": "preserve",
             "pattern": r"[0-9]{7}",
-        }
+        },
     )
     nNFSeMun: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "max_length": 15,
             "white_space": "preserve",
             "pattern": r"[0-9]{15}",
-        }
+        },
     )
     cVerifNFSeMun: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "min_length": 1,
             "max_length": 9,
             "white_space": "preserve",
             "pattern": r"[a-zA-Z0-9]{1,9}",
-        }
+        },
     )
 
 
 @dataclass
-class TcenderExt:
+class TcenderExt(CommonMixin):
     """
     :ivar cPais: Código do país (Tabela de Países ISO)
     :ivar cEndPost: Código alfanumérico do Endereçamento Postal no
         exterior do prestador do serviço.
     :ivar xCidade: Nome da cidade no exterior do prestador do serviço.
     :ivar xEstProvReg: Estado, província ou região da cidade no exterior
         do prestador do serviço.
     """
+
     class Meta:
         name = "TCEnderExt"
 
     cPais: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "white_space": "preserve",
             "pattern": r"[A-Z]{2}",
-        }
+        },
     )
     cEndPost: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "min_length": 1,
             "max_length": 11,
             "white_space": "preserve",
-        }
+        },
     )
     xCidade: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "min_length": 1,
             "max_length": 60,
             "white_space": "preserve",
-        }
+        },
     )
     xEstProvReg: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "min_length": 1,
             "max_length": 60,
             "white_space": "preserve",
-        }
+        },
     )
 
 
 @dataclass
-class TcenderExtSimples:
+class TcenderExtSimples(CommonMixin):
     """
     :ivar cEndPost: Código alfanumérico do Endereçamento Postal no
         exterior do prestador do serviço.
     :ivar xCidade: Nome da cidade no exterior do prestador do serviço.
     :ivar xEstProvReg: Estado, província ou região da cidade no exterior
         do prestador do serviço.
     """
+
     class Meta:
         name = "TCEnderExtSimples"
 
     cEndPost: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "min_length": 1,
             "max_length": 11,
             "white_space": "preserve",
-        }
+        },
     )
     xCidade: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "min_length": 1,
             "max_length": 60,
             "white_space": "preserve",
-        }
+        },
     )
     xEstProvReg: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "min_length": 1,
             "max_length": 60,
             "white_space": "preserve",
-        }
+        },
     )
 
 
 @dataclass
-class TcenderNac:
+class TcenderNac(CommonMixin):
     """
     :ivar cMun: Código do município, conforme Tabela do IBGE
     :ivar CEP: Número do CEP
     """
+
     class Meta:
         name = "TCEnderNac"
 
     cMun: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "white_space": "preserve",
             "pattern": r"[0-9]{7}",
-        }
+        },
     )
     CEP: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "white_space": "preserve",
             "pattern": r"[0-9]{8}",
-        }
+        },
     )
 
 
 @dataclass
-class TcenderObraEvento:
+class TcenderObraEvento(CommonMixin):
     """
     :ivar cEndPost: Código de endereçamento postal
     :ivar xLgr: Tipo e nome do logradouro da localização do imóvel
     :ivar nro: Número do imóvel
     :ivar xCpl: Complemento do endereço
     :ivar xBairro: Bairro
     :ivar xCidade: Cidade
     :ivar xEstProvReg: Estado, província ou região
     """
+
     class Meta:
         name = "TCEnderObraEvento"
 
     cEndPost: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "min_length": 1,
             "max_length": 11,
             "white_space": "preserve",
-        }
+        },
     )
     xLgr: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "min_length": 1,
             "max_length": 255,
             "white_space": "preserve",
             "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
-        }
+        },
     )
     nro: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "min_length": 1,
             "max_length": 60,
             "white_space": "preserve",
             "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
-        }
+        },
     )
     xCpl: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "min_length": 1,
             "max_length": 156,
             "white_space": "preserve",
             "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
-        }
+        },
     )
     xBairro: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "min_length": 1,
             "max_length": 60,
             "white_space": "preserve",
             "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
-        }
+        },
     )
     xCidade: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "min_length": 1,
             "max_length": 60,
             "white_space": "preserve",
-        }
+        },
     )
     xEstProvReg: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "min_length": 1,
             "max_length": 60,
             "white_space": "preserve",
-        }
+        },
     )
 
 
 @dataclass
-class TcinfoCompl:
+class TcinfoCompl(CommonMixin):
     """
     :ivar idDocTec: Identificador de Documento de Responsabilidade
         Técnica: ART, RRT, DRT, Outros.
     :ivar docRef: Chave da nota, número identificador da nota, número do
         contrato ou outro identificador de documento emitido pelo
         prestador de serviços, que subsidia a emissão dessa nota pelo
         tomador do serviço ou intermediário (preenchimento obrigatório
         caso a nota esteja sendo emitida pelo Tomador ou intermediário
         do serviço).
     :ivar xInfComp: Informações complementares
     """
+
     class Meta:
         name = "TCInfoCompl"
 
     idDocTec: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "min_length": 1,
             "max_length": 40,
             "white_space": "preserve",
-        }
+        },
     )
     docRef: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "min_length": 1,
             "max_length": 255,
             "white_space": "preserve",
             "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
-        }
+        },
     )
     xInfComp: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "min_length": 1,
             "max_length": 2000,
             "white_space": "preserve",
             "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
-        }
+        },
     )
 
 
 @dataclass
-class TctribTotalMonet:
+class TctribTotalMonet(CommonMixin):
     """
     :ivar vTotTribFed: Valor monetário total aproximado dos tributos
         federais (R$).
     :ivar vTotTribEst: Valor monetário total aproximado dos tributos
         estaduais (R$).
     :ivar vTotTribMun: Valor monetário total aproximado dos tributos
         municipais (R$).
     """
+
     class Meta:
         name = "TCTribTotalMonet"
 
     vTotTribFed: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "white_space": "preserve",
             "pattern": r"0|0\.[0-9]{2}|[1-9]{1}[0-9]{0,14}(\.[0-9]{2})?",
-        }
+        },
     )
     vTotTribEst: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "white_space": "preserve",
             "pattern": r"0|0\.[0-9]{2}|[1-9]{1}[0-9]{0,14}(\.[0-9]{2})?",
-        }
+        },
     )
     vTotTribMun: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "white_space": "preserve",
             "pattern": r"0|0\.[0-9]{2}|[1-9]{1}[0-9]{0,14}(\.[0-9]{2})?",
-        }
+        },
     )
 
 
 @dataclass
-class TctribTotalPercent:
+class TctribTotalPercent(CommonMixin):
     """
     :ivar pTotTribFed: Valor percentual total aproximado dos tributos
         federais (%).
     :ivar pTotTribEst: Valor percentual total aproximado dos tributos
         estaduais (%).
     :ivar pTotTribMun: Valor percentual total aproximado dos tributos
         municipais (%).
     """
+
     class Meta:
         name = "TCTribTotalPercent"
 
     pTotTribFed: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "white_space": "preserve",
             "pattern": r"0|0\.[0-9]{2}|[1-9]{1}[0-9]{0,2}(\.[0-9]{2})?",
-        }
+        },
     )
     pTotTribEst: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "white_space": "preserve",
             "pattern": r"0|0\.[0-9]{2}|[1-9]{1}[0-9]{0,2}(\.[0-9]{2})?",
-        }
+        },
     )
     pTotTribMun: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "white_space": "preserve",
             "pattern": r"0|0\.[0-9]{2}|[1-9]{1}[0-9]{0,2}(\.[0-9]{2})?",
-        }
+        },
     )
 
 
 @dataclass
-class TcvdescCondIncond:
+class TcvdescCondIncond(CommonMixin):
     """
     :ivar vDescIncond: Valor monetário do desconto incondicionado (R$)
     :ivar vDescCond: Valor monetário do desconto condicionado (R$)
     """
+
     class Meta:
         name = "TCVDescCondIncond"
 
     vDescIncond: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "white_space": "preserve",
             "pattern": r"0|0\.[0-9]{2}|[1-9]{1}[0-9]{0,14}(\.[0-9]{2})?",
-        }
+        },
     )
     vDescCond: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "white_space": "preserve",
             "pattern": r"0|0\.[0-9]{2}|[1-9]{1}[0-9]{0,14}(\.[0-9]{2})?",
-        }
+        },
     )
 
 
 @dataclass
-class TcvservPrest:
+class TcvservPrest(CommonMixin):
     """
     :ivar vReceb: Valor monetário recebido pelo intermediário do serviço
         (R$)
     :ivar vServ: Valor dos serviços em R$
     """
+
     class Meta:
         name = "TCVServPrest"
 
     vReceb: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "white_space": "preserve",
             "pattern": r"0|0\.[0-9]{2}|[1-9]{1}[0-9]{0,14}(\.[0-9]{2})?",
-        }
+        },
     )
     vServ: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "white_space": "preserve",
             "pattern": r"0|0\.[0-9]{2}|[1-9]{1}[0-9]{0,14}(\.[0-9]{2})?",
-        }
+        },
     )
 
 
 @dataclass
-class TcvaloresNfse:
+class TcvaloresNfse(CommonMixin):
     """
     :ivar vCalcDR: Valor monetário (R$) de dedução/redução da base de
         cálculo (BC) do ISSQN.
     :ivar tpBM: Tipo de Benefício Municipal (BM)
     :ivar vCalcBM: Valor monetário (R$) do percentual de redução da base
         de cálculo (BC) do ISSQN devido a um benefício municipal (BM).
     :ivar vBC: Valor monetário (R$) do percentual de redução da base de
@@ -654,107 +672,108 @@
     :ivar vLiq: Valor líquido = Valor do serviço - Desconto condicionado
         - Desconto incondicionado - Valores retidos (CP, IRRF, CSLL)* -
         Valores, se retidos (ISSQN, PIS, COFINS)** Valor Líquido (R$) =
         vServ – vDescIncond – vDescCond – (vRetCP + vRetIRRF +
         vRetCSLL)* – (vISSQN - vPIS + vCOFINS)**
     :ivar xOutInf: Uso da Administração Tributária Municipal.
     """
+
     class Meta:
         name = "TCValoresNFSe"
 
     vCalcDR: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "white_space": "preserve",
             "pattern": r"0|0\.[0-9]{2}|[1-9]{1}[0-9]{0,14}(\.[0-9]{2})?",
-        }
+        },
     )
     tpBM: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "min_length": 1,
             "max_length": 40,
             "white_space": "preserve",
             "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
-        }
+        },
     )
     vCalcBM: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "white_space": "preserve",
             "pattern": r"0|0\.[0-9]{2}|[1-9]{1}[0-9]{0,14}(\.[0-9]{2})?",
-        }
+        },
     )
     vBC: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "white_space": "preserve",
             "pattern": r"0|0\.[0-9]{2}|[1-9]{1}[0-9]{0,14}(\.[0-9]{2})?",
-        }
+        },
     )
     pAliqAplic: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "white_space": "preserve",
             "pattern": r"0|[0-9]{1}(\.[0-9]{2})?",
-        }
+        },
     )
     vISSQN: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "white_space": "preserve",
             "pattern": r"0|0\.[0-9]{2}|[1-9]{1}[0-9]{0,14}(\.[0-9]{2})?",
-        }
+        },
     )
     vTotalRet: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "white_space": "preserve",
             "pattern": r"0|0\.[0-9]{2}|[1-9]{1}[0-9]{0,14}(\.[0-9]{2})?",
-        }
+        },
     )
     vLiq: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "white_space": "preserve",
             "pattern": r"0|0\.[0-9]{2}|[1-9]{1}[0-9]{0,14}(\.[0-9]{2})?",
-        }
+        },
     )
     xOutInf: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "min_length": 1,
             "max_length": 2000,
             "white_space": "preserve",
             "pattern": r"[\s\S!-ÿ]{1}[\s\S -ÿ]{0,}[\s\S!-ÿ]{1}|[\s\S!-ÿ]{1}",
-        }
+        },
     )
 
 
 @dataclass
-class TcbeneficioMunicipal:
+class TcbeneficioMunicipal(CommonMixin):
     """
     :ivar tpBM: Identificação da Lei parametrizada pelo município que
         define o benefício. Trata-se de um identificador único que foi
         gerado pelo Sistema Nacional no momento em que o município de
         incidência do ISSQN incluiu o benefício no sistema. Tem a
         seguinte regra de formação: 7 dígitos com o código IBGE do
         município + 4 dígitos com número sequencial. Deve ser obtido da
@@ -764,56 +783,57 @@
     :ivar vRedBCBM: Valor monetário informado pelo emitente para redução
         da base de cálculo (BC) do ISSQN devido a um Benefício Municipal
         (BM).
     :ivar pRedBCBM: Valor percentual informado pelo emitente para
         redução da base de cálculo (BC) do ISSQN devido a um Benefício
         Municipal (BM).
     """
+
     class Meta:
         name = "TCBeneficioMunicipal"
 
     tpBM: Optional[TsopTipoBm] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
     nBM: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "pattern": r"[0-9]{14}",
-        }
+        },
     )
     vRedBCBM: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "white_space": "preserve",
             "pattern": r"0|0\.[0-9]{2}|[1-9]{1}[0-9]{0,14}(\.[0-9]{2})?",
-        }
+        },
     )
     pRedBCBM: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "white_space": "preserve",
             "pattern": r"0|0\.[0-9]{2}|[1-9]{1}[0-9]{0,2}(\.[0-9]{2})?",
-        }
+        },
     )
 
 
 @dataclass
-class TccomExterior:
+class TccomExterior(CommonMixin):
     """
     :ivar mdPrestacao: Modo de Prestação: 0 - Desconhecido (tipo não
         informado na nota de origem); 1 - Transfronteiriço; 2 - Consumo
         no Brasil; 3 - Presença Comercial no Exterior; 4 - Movimento
         Temporário de Pessoas Físicas;
     :ivar vincPrest: Vínculo entre as partes no negócio: 0 - Sem vínculo
         com o tomador/ Prestador 1 - Controlada; 2 - Controladora; 3 -
@@ -856,391 +876,396 @@
     :ivar nDI: Número da Declaração de Importação (DI/DSI/DA/DRI-E)
         averbado
     :ivar nRE: Número do Registro de Exportação (RE) averbado
     :ivar mdic: Compartilhar as informações da NFS-e gerada a partir
         desta DPS com a Secretaria de Comércio Exterior: 0 - Não enviar
         para o MDIC; 1 - Enviar para o MDIC;
     """
+
     class Meta:
         name = "TCComExterior"
 
     mdPrestacao: Optional[TsmodoPrestacao] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
     vincPrest: Optional[TsvincPrest] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
     tpMoeda: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "max_length": 3,
             "white_space": "preserve",
             "pattern": r"[0-9]{3}",
-        }
+        },
     )
     vServMoeda: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "white_space": "preserve",
             "pattern": r"0|0\.[0-9]{2}|[1-9]{1}[0-9]{0,14}(\.[0-9]{2})?",
-        }
+        },
     )
     mecAFComexP: Optional[TsmecAfcomExPrest] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
     mecAFComexT: Optional[TsmecAfcomExToma] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
     movTempBens: Optional[TsmovTempBens] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
     nDI: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "min_length": 1,
             "max_length": 12,
             "white_space": "preserve",
             "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
-        }
+        },
     )
     nRE: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "min_length": 1,
             "max_length": 12,
             "white_space": "preserve",
             "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
-        }
+        },
     )
     mdic: Optional[TsenvMdic] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
 
 
 @dataclass
-class Tcendereco:
+class Tcendereco(CommonMixin):
     """
     :ivar endNac: Grupo de informações específicas de endereço nacional
     :ivar endExt: Grupo de informações específicas de endereço no
         exterior
     :ivar xLgr: Tipo e nome do logradouro da localização do imóvel
     :ivar nro: Número do imóvel
     :ivar xCpl: Complemento do endereço
     :ivar xBairro: Bairro
     """
+
     class Meta:
         name = "TCEndereco"
 
     endNac: Optional[TcenderNac] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
-        }
+        },
     )
     endExt: Optional[TcenderExt] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
-        }
+        },
     )
     xLgr: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "min_length": 1,
             "max_length": 255,
             "white_space": "preserve",
             "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
-        }
+        },
     )
     nro: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "min_length": 1,
             "max_length": 60,
             "white_space": "preserve",
             "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
-        }
+        },
     )
     xCpl: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "min_length": 1,
             "max_length": 156,
             "white_space": "preserve",
             "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
-        }
+        },
     )
     xBairro: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "min_length": 1,
             "max_length": 60,
             "white_space": "preserve",
             "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
-        }
+        },
     )
 
 
 @dataclass
-class TcenderecoEmitente:
+class TcenderecoEmitente(CommonMixin):
     """
     :ivar xLgr: Tipo e nome do logradouro da localização do imóvel
     :ivar nro: Número do imóvel
     :ivar xCpl: Complemento do endereço
     :ivar xBairro: Bairro
     :ivar cMun: Código do município, conforme Tabela do IBGE
     :ivar UF: Sigla da unidade da federação do município do endereço do
         emitente.
     :ivar CEP: Número do CEP
     """
+
     class Meta:
         name = "TCEnderecoEmitente"
 
     xLgr: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "min_length": 1,
             "max_length": 255,
             "white_space": "preserve",
             "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
-        }
+        },
     )
     nro: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "min_length": 1,
             "max_length": 60,
             "white_space": "preserve",
             "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
-        }
+        },
     )
     xCpl: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "min_length": 1,
             "max_length": 156,
             "white_space": "preserve",
             "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
-        }
+        },
     )
     xBairro: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "min_length": 1,
             "max_length": 60,
             "white_space": "preserve",
             "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
-        }
+        },
     )
     cMun: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "white_space": "preserve",
             "pattern": r"[0-9]{7}",
-        }
+        },
     )
     UF: Optional[Tsuf] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
     CEP: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "white_space": "preserve",
             "pattern": r"[0-9]{8}",
-        }
+        },
     )
 
 
 @dataclass
-class TcenderecoSimples:
+class TcenderecoSimples(CommonMixin):
     """
     :ivar CEP: Número do CEP
     :ivar endExt: Grupo de informações específicas de endereço no
         exterior
     :ivar xLgr: Tipo e nome do logradouro da localização do imóvel
     :ivar nro: Número do imóvel
     :ivar xCpl: Complemento do endereço
     :ivar xBairro: Bairro
     """
+
     class Meta:
         name = "TCEnderecoSimples"
 
     CEP: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "white_space": "preserve",
             "pattern": r"[0-9]{8}",
-        }
+        },
     )
     endExt: Optional[TcenderExtSimples] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
-        }
+        },
     )
     xLgr: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "min_length": 1,
             "max_length": 255,
             "white_space": "preserve",
             "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
-        }
+        },
     )
     nro: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "min_length": 1,
             "max_length": 60,
             "white_space": "preserve",
             "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
-        }
+        },
     )
     xCpl: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "min_length": 1,
             "max_length": 156,
             "white_space": "preserve",
             "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
-        }
+        },
     )
     xBairro: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "min_length": 1,
             "max_length": 60,
             "white_space": "preserve",
             "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
-        }
+        },
     )
 
 
 @dataclass
-class TcexigSuspensa:
+class TcexigSuspensa(CommonMixin):
     """
     :ivar tpSusp: Opção para Exigibilidade Suspensa: 1 - Exigibilidade
         Suspensa por Decisão Judicial; 2 - Exigibilidade Suspensa por
         Processo Administrativo;
     :ivar nProcesso: Número do processo judicial ou administrativo de
         suspensão da exigibilidade
     """
+
     class Meta:
         name = "TCExigSuspensa"
 
     tpSusp: Optional[TsopExigSuspensa] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
     nProcesso: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "pattern": r"[0-9]{30}",
-        }
+        },
     )
 
 
 @dataclass
-class TcexploracaoRodoviaria:
+class TcexploracaoRodoviaria(CommonMixin):
     """
     :ivar categVeic: Categorias de veículos para cobrança: 00 -
         Categoria de Veículos (tipo não informado na nota de origem); 01
         - Automóvel, caminhonete e furgão; 02 - Caminhão leve, ônibus,
         caminhão trator e furgão; 03 - Automóvel e caminhonete com
         semireboque; 04 - Caminhão, caminhão-trator, caminhão-trator com
         semi-reboque e ônibus; 05 - Automóvel e caminhonete com reboque;
@@ -1254,184 +1279,187 @@
     :ivar sentido: Placa do veículo
     :ivar placa: Placa do veículo
     :ivar codAcessoPed: Código de acesso gerado automaticamente pelo
         sistema emissor da concessionária.
     :ivar codContrato: Código de contrato gerado automaticamente pelo
         sistema nacional no cadastro da concessionária.
     """
+
     class Meta:
         name = "TCExploracaoRodoviaria"
 
     categVeic: Optional[TscategVeic] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
     nEixos: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "white_space": "preserve",
             "pattern": r"[0-9]{1,2}",
-        }
+        },
     )
     rodagem: Optional[Tsrodagem] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
     sentido: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "white_space": "preserve",
             "pattern": r"[0-9]{1,3}",
-        }
+        },
     )
     placa: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "white_space": "preserve",
             "pattern": r"[A-Z]{2,3}[0-9]{4}|[A-Z]{3,4}[0-9]{3}",
-        }
+        },
     )
     codAcessoPed: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "white_space": "preserve",
             "pattern": r"[a-zA-Z0-9]{10}",
-        }
+        },
     )
     codContrato: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "white_space": "preserve",
             "pattern": r"[a-zA-Z0-9]{4}",
-        }
+        },
     )
 
 
 @dataclass
-class TclocPrest:
+class TclocPrest(CommonMixin):
     """
     :ivar cLocPrestacao: Código do município onde o serviço foi prestado
         (tabela do IBGE)
     :ivar cPaisPrestacao: Código do país onde o serviço foi prestado
         (Tabela de Países ISO)
     :ivar opConsumServ: Opção para que o emitente informe onde ocorreu o
         consumo do serviço prestado. 0 - Consumo do serviço prestado
         ocorrido no município do local da prestação; 1 - Consumo do
         serviço prestado ocorrido ocorrido no exterior ;
     """
+
     class Meta:
         name = "TCLocPrest"
 
     cLocPrestacao: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "white_space": "preserve",
             "pattern": r"[0-9]{7}",
-        }
+        },
     )
     cPaisPrestacao: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "white_space": "preserve",
             "pattern": r"[A-Z]{2}",
-        }
+        },
     )
     opConsumServ: Optional[TsopConsumServ] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
-        }
+        },
     )
 
 
 @dataclass
-class TclocacaoSublocacao:
+class TclocacaoSublocacao(CommonMixin):
     """
     :ivar categ: Categoria do serviço
     :ivar objeto: Tipo de objetos da locação, sublocação, arrendamento,
         direito de passagem ou permissão de uso
     :ivar extensao: Extensão total da ferrovia, rodovia, cabos, dutos ou
         condutos
     :ivar nPostes: Número total de postes
     """
+
     class Meta:
         name = "TCLocacaoSublocacao"
 
     categ: Optional[TscategoriaServico] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
     objeto: Optional[TcobjetoLocacao] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
     extensao: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "min_length": 1,
             "max_length": 5,
             "white_space": "preserve",
             "pattern": r"[0-9]{1,5}",
-        }
+        },
     )
     nPostes: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "min_length": 1,
             "max_length": 6,
             "white_space": "preserve",
             "pattern": r"[0-9]{1,6}",
-        }
+        },
     )
 
 
 @dataclass
-class TcregTrib:
+class TcregTrib(CommonMixin):
     """
     :ivar opSimpNac: Situação perante o Simples Nacional: 1 - Não
         Optante; 2 - Optante - Microempreendedor Individual (MEI); 3 -
         Optante - Microempresa ou Empresa de Pequeno Porte (ME/EPP);
     :ivar regApTribSN: Opção para que o contribuinte optante pelo
         Simples Nacional ME/EPP (opSimpNac = 3) possa indicar, ao emitir
         o documento fiscal, em qual regime de apuração os tributos
@@ -1444,92 +1472,94 @@
         fora do SN conforme respectivas legilações federal e municipal
         de cada tributo;
     :ivar regEspTrib: Tipos de Regimes Especiais de Tributação: 0 -
         Nenhum; 1 - Ato Cooperado (Cooperativa); 2 - Estimativa; 3 -
         Microempresa Municipal; 4 - Notário ou Registrador; 5 -
         Profissional Autônomo; 6 - Sociedade de Profissionais;
     """
+
     class Meta:
         name = "TCRegTrib"
 
     opSimpNac: Optional[TsopSimpNac] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
     regApTribSN: Optional[TsregimeApuracaoSimpNac] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
-        }
+        },
     )
     regEspTrib: Optional[TsregEspTrib] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
 
 
 @dataclass
-class Tcsubstituicao:
+class Tcsubstituicao(CommonMixin):
     """
     :ivar chSubstda: Chave de acesso da NFS-e a ser substituída
     :ivar cMotivo: Código de justificativa para substituição de NFS-e:
         01 - Desenquadramento de NFS-e do Simples Nacional; 02 -
         Enquadramento de NFS-e no Simples Nacional; 03 - Inclusão
         Retroativa de Imunidade/Isenção para NFS-e; 04 - Exclusão
         Retroativa de Imunidade/Isenção para NFS-e; 05 - Rejeição de
         NFS-e pelo tomador ou pelo intermediário se responsável pelo
         recolhimento do tributo; 99 - Outros;
     :ivar xMotivo: Descrição do motivo da substituição da NFS-e
     """
+
     class Meta:
         name = "TCSubstituicao"
 
     chSubstda: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "max_length": 50,
             "white_space": "preserve",
             "pattern": r"[0-9]{50}",
-        }
+        },
     )
     cMotivo: Optional[TscodJustSubst] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
     xMotivo: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "min_length": 15,
             "max_length": 255,
             "white_space": "preserve",
             "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
-        }
+        },
     )
 
 
 @dataclass
-class TctribOutrosPisCofins:
+class TctribOutrosPisCofins(CommonMixin):
     """
     :ivar CST: Código de Situação Tributária do PIS/COFINS (CST): 00 -
         Nenhum; 01 - Operação Tributável com Alíquota Básica; 02 -
         Operação Tributável com Alíquota Diferenciada; 03 - Operação
         Tributável com Alíquota por Unidade de Medida de Produto; 04 -
         Operação Tributável monofásica - Revenda a Alíquota Zero; 05 -
         Operação Tributável por Substituição Tributária; 06 - Operação
@@ -1540,336 +1570,341 @@
     :ivar pAliqPis: Valor da Alíquota do PIS (%).
     :ivar pAliqCofins: Valor da Alíquota da COFINS (%).
     :ivar vPis: Valor monetário do PIS (R$).
     :ivar vCofins: Valor monetário do COFINS (R$).
     :ivar tpRetPisCofins: Tipo de retencao do Pis/Cofins: 1 - Retido; 2
         - Não Retido;
     """
+
     class Meta:
         name = "TCTribOutrosPisCofins"
 
     CST: Optional[TstipoCst] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
     vBCPisCofins: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "white_space": "preserve",
             "pattern": r"0|0\.[0-9]{2}|[1-9]{1}[0-9]{0,14}(\.[0-9]{2})?",
-        }
+        },
     )
     pAliqPis: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "white_space": "preserve",
             "pattern": r"0|0\.[0-9]{2}|[1-9]{1}[0-9]{0,1}(\.[0-9]{2})?",
-        }
+        },
     )
     pAliqCofins: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "white_space": "preserve",
             "pattern": r"0|0\.[0-9]{2}|[1-9]{1}[0-9]{0,1}(\.[0-9]{2})?",
-        }
+        },
     )
     vPis: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "white_space": "preserve",
             "pattern": r"0|0\.[0-9]{2}|[1-9]{1}[0-9]{0,14}(\.[0-9]{2})?",
-        }
+        },
     )
     vCofins: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "white_space": "preserve",
             "pattern": r"0|0\.[0-9]{2}|[1-9]{1}[0-9]{0,14}(\.[0-9]{2})?",
-        }
+        },
     )
     tpRetPisCofins: Optional[TstipoRetPiscofins] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
-        }
+        },
     )
 
 
 @dataclass
-class TctribTotal:
+class TctribTotal(CommonMixin):
     """
     :ivar vTotTrib: Valor monetário total aproximado dos tributos, em
         conformidade com o artigo 1o da Lei no 12.741/2012
     :ivar pTotTrib: Valor percentual total aproximado dos tributos, em
         conformidade com o artigo 1o da Lei no 12.741/2012
     :ivar indTotTrib: Indicador de informação de valor total de
         tributos. Possui valor fixo igual a zero (indTotTrib=0). Não
         informar nenhum valor estimado para os Tributos (Decreto
         8.264/2014). 0 - Não;
     :ivar pTotTribSN: Valor percentual aproximado do total dos tributos
         da alíquota do Simples Nacional (%)
     """
+
     class Meta:
         name = "TCTribTotal"
 
     vTotTrib: Optional[TctribTotalMonet] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
-        }
+        },
     )
     pTotTrib: Optional[TctribTotalPercent] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
-        }
+        },
     )
     indTotTrib: Optional[TstipoIndTotTrib] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
-        }
+        },
     )
     pTotTribSN: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "white_space": "preserve",
             "pattern": r"0|0\.[0-9]{2}|[1-9]{1}[0-9]{0,1}(\.[0-9]{2})?",
-        }
+        },
     )
 
 
 @dataclass
-class TcatvEvento:
+class TcatvEvento(CommonMixin):
     """
     :ivar desc: Descrição do evento Artístico, Cultural, Esportivo, etc
     :ivar dtIni: Data de início da atividade de evento. Ano, Mês e Dia
         (AAAA-MM-DD)
     :ivar dtFim: Data de fim da atividade de evento. Ano, Mês e Dia
         (AAAA-MM-DD)
     :ivar id: Identificação da Atividade de Evento (código identificador
         de evento determinado pela Administração Tributária Municipal)
     :ivar end: Grupo de informações relativas ao endereço da atividade,
         evento ou local do serviço prestado
     """
+
     class Meta:
         name = "TCAtvEvento"
 
     desc: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "min_length": 1,
             "max_length": 255,
             "white_space": "preserve",
             "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
-        }
+        },
     )
     dtIni: Optional[XmlDate] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
     dtFim: Optional[XmlDate] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
     id: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "min_length": 1,
             "max_length": 30,
             "white_space": "preserve",
-        }
+        },
     )
     end: Optional[TcenderecoSimples] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
-        }
+        },
     )
 
 
 @dataclass
-class Tcemitente:
+class Tcemitente(CommonMixin):
     """
     :ivar CNPJ: Número do CNPJ do emitente da NFS-e.
     :ivar CPF: Número do CPF do emitente da NFS-e.
     :ivar IM: Número da inscrição municipal
     :ivar xNome: Nome / Razão Social do emitente.
     :ivar xFant: Nome / Fantasia do emitente.
     :ivar enderNac: Grupo de informações do endereço nacional do
         Emitente da NFS-e
     :ivar fone: Número do telefone do emitente. (Preencher com o Código
         DDD + número do telefone. Nas operações com exterior é permitido
         informar o código do país + código da localidade + número do
         telefone)
     :ivar email: E-mail do emitente.
     """
+
     class Meta:
         name = "TCEmitente"
 
     CNPJ: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "max_length": 14,
             "white_space": "preserve",
             "pattern": r"[0-9]{14}",
-        }
+        },
     )
     CPF: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "max_length": 11,
             "white_space": "preserve",
             "pattern": r"[0-9]{11}",
-        }
+        },
     )
     IM: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "min_length": 1,
             "max_length": 15,
             "white_space": "preserve",
-        }
+        },
     )
     xNome: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "min_length": 1,
             "max_length": 300,
             "white_space": "preserve",
-        }
+        },
     )
     xFant: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "min_length": 1,
             "max_length": 150,
             "white_space": "preserve",
-        }
+        },
     )
     enderNac: Optional[TcenderecoEmitente] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
     fone: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "white_space": "preserve",
             "pattern": r"[0-9]{6,20}",
-        }
+        },
     )
     email: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "min_length": 1,
             "max_length": 80,
             "white_space": "preserve",
             "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
-        }
+        },
     )
 
 
 @dataclass
-class TcinfoObra:
+class TcinfoObra(CommonMixin):
     """
     :ivar cObra: Número de identificação da obra. Cadastro Nacional de
         Obras (CNO) ou Cadastro Específico do INSS (CEI).
     :ivar inscImobFisc: Inscrição imobiliária fiscal (código fornecido
         pela Prefeitura Municipal para a identificação da obra ou para
         fins de recolhimento do IPTU)
     :ivar end: Grupo de informações do endereço da obra do serviço
         prestado
     """
+
     class Meta:
         name = "TCInfoObra"
 
     cObra: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "min_length": 1,
             "max_length": 30,
             "white_space": "preserve",
-        }
+        },
     )
     inscImobFisc: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "min_length": 1,
             "max_length": 30,
             "white_space": "preserve",
-        }
+        },
     )
     end: Optional[TcenderecoSimples] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
-        }
+        },
     )
 
 
 @dataclass
-class TcinfoPessoa:
+class TcinfoPessoa(CommonMixin):
     """Informações das pessoas envolvidas na NFS-e.
 
     Pode ser o tomador, o intermediário ou o fornecedor
     (dedução/redução)
 
     :ivar CNPJ: Número do CNPJ
     :ivar CPF: Número do CPF
@@ -1885,116 +1920,117 @@
     :ivar end: Dados de endereço
     :ivar fone: Número do telefone do prestador: Preencher com o Código
         DDD + número do telefone. Nas operações com exterior é permitido
         informar o código do país + código da localidade + número do
         telefone)
     :ivar email: E-mail
     """
+
     class Meta:
         name = "TCInfoPessoa"
 
     CNPJ: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "max_length": 14,
             "white_space": "preserve",
             "pattern": r"[0-9]{14}",
-        }
+        },
     )
     CPF: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "max_length": 11,
             "white_space": "preserve",
             "pattern": r"[0-9]{11}",
-        }
+        },
     )
     NIF: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "min_length": 1,
             "max_length": 40,
             "white_space": "preserve",
-        }
+        },
     )
     cNaoNIF: Optional[TscodNaoNif] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
-        }
+        },
     )
     CAEPF: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "max_length": 14,
             "white_space": "preserve",
             "pattern": r"[0-9]{14}",
-        }
+        },
     )
     IM: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "min_length": 1,
             "max_length": 15,
             "white_space": "preserve",
-        }
+        },
     )
     xNome: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "min_length": 1,
             "max_length": 300,
             "white_space": "preserve",
-        }
+        },
     )
     end: Optional[Tcendereco] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
-        }
+        },
     )
     fone: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "white_space": "preserve",
             "pattern": r"[0-9]{6,20}",
-        }
+        },
     )
     email: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "min_length": 1,
             "max_length": 80,
             "white_space": "preserve",
             "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
-        }
+        },
     )
 
 
 @dataclass
-class TcinfoPrestador:
+class TcinfoPrestador(CommonMixin):
     """Informações do prestador da NFS-e.
 
     Difere das demais pessoas por causa das informações de regimes de
     tributação
 
     :ivar CNPJ: Número do CNPJ
     :ivar CPF: Número do CPF
@@ -2011,123 +2047,124 @@
         DDD + número do telefone. Nas operações com exterior é permitido
         informar o código do país + código da localidade + número do
         telefone)
     :ivar email: E-mail
     :ivar regTrib: Grupo de informações relativas aos regimes de
         tributação do prestador de serviços
     """
+
     class Meta:
         name = "TCInfoPrestador"
 
     CNPJ: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "max_length": 14,
             "white_space": "preserve",
             "pattern": r"[0-9]{14}",
-        }
+        },
     )
     CPF: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "max_length": 11,
             "white_space": "preserve",
             "pattern": r"[0-9]{11}",
-        }
+        },
     )
     NIF: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "min_length": 1,
             "max_length": 40,
             "white_space": "preserve",
-        }
+        },
     )
     cNaoNIF: Optional[TscodNaoNif] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
-        }
+        },
     )
     CAEPF: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "max_length": 14,
             "white_space": "preserve",
             "pattern": r"[0-9]{14}",
-        }
+        },
     )
     IM: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "min_length": 1,
             "max_length": 15,
             "white_space": "preserve",
-        }
+        },
     )
     xNome: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "min_length": 1,
             "max_length": 300,
             "white_space": "preserve",
-        }
+        },
     )
     end: Optional[Tcendereco] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
-        }
+        },
     )
     fone: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "white_space": "preserve",
             "pattern": r"[0-9]{6,20}",
-        }
+        },
     )
     email: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "min_length": 1,
             "max_length": 80,
             "white_space": "preserve",
             "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
-        }
+        },
     )
     regTrib: Optional[TcregTrib] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
 
 
 @dataclass
-class TctribMunicipal:
+class TctribMunicipal(CommonMixin):
     """
     :ivar tribISSQN: Tributação do ISSQN sobre o serviço prestado: 1 -
         Operação tributável; 2 - Exportação de serviço; 3 - Não
         Incidência; 4 - Imunidade;
     :ivar cPaisResult: Código do país onde se verficou o resultado da
         prestação do serviço para o caso de Exportação de
         Serviço.(Tabela de Países ISO)
@@ -2152,123 +2189,125 @@
         alíquota estará parametrizada e, portanto, será fornecida pelo
         sistema. Se o município de incidência não pertence ao Sistema
         Nacional NFS-e a alíquota não estará parametrizada e, por isso,
         deverá ser fornecida pelo emitente.
     :ivar tpRetISSQN: Tipo de retencao do ISSQN: 1 - Não Retido; 2 -
         Retido pelo Tomador; 3 - Retido pelo Intermediario;
     """
+
     class Meta:
         name = "TCTribMunicipal"
 
     tribISSQN: Optional[TstribIssqn] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
     cPaisResult: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "white_space": "preserve",
             "pattern": r"[A-Z]{2}",
-        }
+        },
     )
     BM: Optional[TcbeneficioMunicipal] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
-        }
+        },
     )
     exigSusp: Optional[TcexigSuspensa] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
-        }
+        },
     )
     tpImunidade: Optional[TstipoImunidadeIssqn] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
-        }
+        },
     )
     pAliq: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "white_space": "preserve",
             "pattern": r"0|[0-9]{1}(\.[0-9]{2})?",
-        }
+        },
     )
     tpRetISSQN: Optional[TstipoRetIssqn] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
 
 
 @dataclass
-class TctribNacional:
+class TctribNacional(CommonMixin):
     """
     :ivar piscofins: Grupo de informações dos tributos PIS/COFINS
     :ivar vRetCP: Valor monetário do CP(R$).
     :ivar vRetIRRF: Valor monetário do IRRF (R$).
     :ivar vRetCSLL: Valor monetário do CSLL (R$).
     """
+
     class Meta:
         name = "TCTribNacional"
 
     piscofins: Optional[TctribOutrosPisCofins] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
-        }
+        },
     )
     vRetCP: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "white_space": "preserve",
             "pattern": r"0|0\.[0-9]{2}|[1-9]{1}[0-9]{0,14}(\.[0-9]{2})?",
-        }
+        },
     )
     vRetIRRF: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "white_space": "preserve",
             "pattern": r"0|0\.[0-9]{2}|[1-9]{1}[0-9]{0,14}(\.[0-9]{2})?",
-        }
+        },
     )
     vRetCSLL: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "white_space": "preserve",
             "pattern": r"0|0\.[0-9]{2}|[1-9]{1}[0-9]{0,14}(\.[0-9]{2})?",
-        }
+        },
     )
 
 
 @dataclass
-class TcdocDedRed:
+class TcdocDedRed(CommonMixin):
     """
     :ivar chNFSe: Chave de Acesso da NFS-e (Padrão Nacional)
     :ivar chNFe: Chave de Acesso da NF-e
     :ivar NFSeMun: Grupo de informações de Outras NFS-e (Padrão anterior
         de NFS-e)
     :ivar NFNFS: Grupo de informações de NF ou NFS (Modelo não
         eletrônico)
@@ -2289,169 +2328,171 @@
     :ivar vDeducaoReducao: Valor monetário utilizado para
         dedução/redução do valor do serviço da NFS-e que está sendo
         emitida (R$). Deve ser menor ou igual ao valor
         deduzível/redutível (vDedutivelRedutivel).
     :ivar fornec: Grupo de informações do Fornecedor em Deduções de
         Serviços
     """
+
     class Meta:
         name = "TCDocDedRed"
 
     chNFSe: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "max_length": 50,
             "white_space": "preserve",
             "pattern": r"[0-9]{50}",
-        }
+        },
     )
     chNFe: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "max_length": 44,
             "white_space": "preserve",
             "pattern": r"[0-9]{44}",
-        }
+        },
     )
     NFSeMun: Optional[TcdocOutNfse] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
-        }
+        },
     )
     NFNFS: Optional[TcdocNfnfs] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
-        }
+        },
     )
     nDocFisc: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "min_length": 1,
             "max_length": 255,
             "white_space": "preserve",
             "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
-        }
+        },
     )
     nDoc: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "min_length": 1,
             "max_length": 255,
             "white_space": "preserve",
             "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
-        }
+        },
     )
     tpDedRed: Optional[TsideDedRed] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
     xDescOutDed: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "min_length": 1,
             "max_length": 150,
             "white_space": "preserve",
             "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
-        }
+        },
     )
     dtEmiDoc: Optional[XmlDate] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
     vDedutivelRedutivel: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "white_space": "preserve",
             "pattern": r"0|0\.[0-9]{2}|[1-9]{1}[0-9]{0,14}(\.[0-9]{2})?",
-        }
+        },
     )
     vDeducaoReducao: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "white_space": "preserve",
             "pattern": r"0|0\.[0-9]{2}|[1-9]{1}[0-9]{0,14}(\.[0-9]{2})?",
-        }
+        },
     )
     fornec: Optional[TcinfoPessoa] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
-        }
+        },
     )
 
 
 @dataclass
-class TcinfoTributacao:
+class TcinfoTributacao(CommonMixin):
     """
     :ivar tribMun: Grupo de informações relacionados ao Imposto Sobre
         Serviços de Qualquer Natureza - ISSQN
     :ivar tribNac: Grupo de informações de outros tributos relacionados
         ao serviço prestado
     :ivar totTrib: Grupo de informações para totais aproximados dos
         tributos relacionados ao serviço prestado
     """
+
     class Meta:
         name = "TCInfoTributacao"
 
     tribMun: Optional[TctribMunicipal] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
     tribNac: Optional[TctribNacional] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
-        }
+        },
     )
     totTrib: Optional[TctribTotal] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
 
 
 @dataclass
-class Tcserv:
+class Tcserv(CommonMixin):
     """
     :ivar locPrest: Grupo de informações relativas ao local da prestação
         do serviço
     :ivar cServ: Grupo de informações relativas ao código do serviço
         prestado
     :ivar comExt: Grupo de informações relativas à exportação/importação
         de serviço prestado
@@ -2461,186 +2502,190 @@
         postes, cabos, dutos e condutos de qualquer natureza
     :ivar obra: Grupo de informações do DPS relativas à serviço de obra
     :ivar atvEvento: Grupo de informações do DPS relativas à Evento
     :ivar explRod: Grupo de informações relativas a pedágio
     :ivar infoCompl: Grupo de informações complementares disponível para
         todos os serviços prestados
     """
+
     class Meta:
         name = "TCServ"
 
     locPrest: Optional[TclocPrest] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
     cServ: Optional[Tccserv] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
     comExt: Optional[TccomExterior] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
-        }
+        },
     )
     lsadppu: Optional[TclocacaoSublocacao] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
-        }
+        },
     )
     obra: Optional[TcinfoObra] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
-        }
+        },
     )
     atvEvento: Optional[TcatvEvento] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
-        }
+        },
     )
     explRod: Optional[TcexploracaoRodoviaria] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
-        }
+        },
     )
     infoCompl: Optional[TcinfoCompl] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
-        }
+        },
     )
 
 
 @dataclass
-class TclistaDocDedRed:
+class TclistaDocDedRed(CommonMixin):
     """
     :ivar docDedRed: Grupo de informações de documento utilizado para
         Dedução/Redução do valor do serviço
     """
+
     class Meta:
         name = "TCListaDocDedRed"
 
     docDedRed: List[TcdocDedRed] = field(
         default_factory=list,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "min_occurs": 1,
             "max_occurs": 1000,
-        }
+        },
     )
 
 
 @dataclass
-class TcinfoDedRed:
+class TcinfoDedRed(CommonMixin):
     """
     :ivar pDR: Valor percentual padrão para dedução/redução do valor do
         serviço
     :ivar vDR: Valor monetário padrão para dedução/redução do valor do
         serviço
     :ivar documentos: Grupo de informações de documento utilizado para
         Dedução/Redução do valor do serviço
     """
+
     class Meta:
         name = "TCInfoDedRed"
 
     pDR: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "white_space": "preserve",
             "pattern": r"0|0\.[0-9]{2}|[1-9]{1}[0-9]{0,2}(\.[0-9]{2})?",
-        }
+        },
     )
     vDR: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "white_space": "preserve",
             "pattern": r"0|0\.[0-9]{2}|[1-9]{1}[0-9]{0,14}(\.[0-9]{2})?",
-        }
+        },
     )
     documentos: Optional[TclistaDocDedRed] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
-        }
+        },
     )
 
 
 @dataclass
-class TcinfoValores:
+class TcinfoValores(CommonMixin):
     """
     :ivar vServPrest: Grupo de informações relativas aos valores do
         serviço prestado
     :ivar vDescCondIncond: Grupo de informações relativas aos descontos
         condicionados e incondicionados
     :ivar vDedRed: Grupo de informações relativas ao valores para
         dedução/redução do valor da base de cálculo (valor do serviço)
     :ivar trib: Grupo de informações relacionados aos tributos
         relacionados ao serviço prestado
     """
+
     class Meta:
         name = "TCInfoValores"
 
     vServPrest: Optional[TcvservPrest] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
     vDescCondIncond: Optional[TcvdescCondIncond] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
-        }
+        },
     )
     vDedRed: Optional[TcinfoDedRed] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
-        }
+        },
     )
     trib: Optional[TcinfoTributacao] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
 
 
 @dataclass
-class TcinfDps:
+class TcinfDps(CommonMixin):
     """
     :ivar tpAmb: Identificação do Ambiente: 1 - Produção; 2 -
         Homologação
     :ivar dhEmi: Data e hora da emissão do DPS. Data e hora no formato
         UTC (Universal Coordinated Time): AAAA-MM-DDThh:mm:ssTZD
     :ivar verAplic: Versão do aplicativo que gerou o DPS
     :ivar serie: Número do equipamento emissor do DPS ou série do DPS
@@ -2671,188 +2716,189 @@
         de Serviços
     :ivar serv: Grupo de informações do DPS relativas ao Serviço
         Prestado
     :ivar valores: Grupo de informações relativas à valores do serviço
         prestado
     :ivar Id:
     """
+
     class Meta:
         name = "TCInfDPS"
 
     tpAmb: Optional[TstipoAmbiente] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
     dhEmi: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "white_space": "preserve",
             "pattern": r"(((20(([02468][048])|([13579][26]))-02-29))|(20[0-9][0-9])-((((0[1-9])|(1[0-2]))-((0[1-9])|(1\d)|(2[0-8])))|((((0[13578])|(1[02]))-31)|(((0[1,3-9])|(1[0-2]))-(29|30)))))T(20|21|22|23|[0-1]\d):[0-5]\d:[0-5]\d([\-,\+](0[0-9]|10|11):00|([\+](12):00))",
-        }
+        },
     )
     verAplic: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "min_length": 1,
             "max_length": 20,
             "white_space": "preserve",
             "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
-        }
+        },
     )
     serie: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "min_length": 1,
             "max_length": 5,
             "white_space": "preserve",
-        }
+        },
     )
     nDPS: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "max_length": 15,
             "white_space": "preserve",
             "pattern": r"[1-9]{1}[0-9]{0,14}",
-        }
+        },
     )
     dCompet: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "white_space": "preserve",
             "pattern": r"(((20(([02468][048])|([13579][26]))-02-29))|(20[0-9][0-9])-((((0[1-9])|(1[0-2]))-((0[1-9])|(1\d)|(2[0-8])))|((((0[13578])|(1[02]))-31)|(((0[1,3-9])|(1[0-2]))-(29|30)))))",
-        }
+        },
     )
     tpEmit: Optional[TsemitenteDps] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
     cLocEmi: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "white_space": "preserve",
             "pattern": r"[0-9]{7}",
-        }
+        },
     )
     subst: Optional[Tcsubstituicao] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
-        }
+        },
     )
     prest: Optional[TcinfoPrestador] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
     toma: Optional[TcinfoPessoa] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
-        }
+        },
     )
     interm: Optional[TcinfoPessoa] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
-        }
+        },
     )
     serv: Optional[Tcserv] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
     valores: Optional[TcinfoValores] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
     Id: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "required": True,
             "max_length": 45,
             "white_space": "preserve",
             "pattern": r"DPS[0-9]{42}",
-        }
+        },
     )
 
 
 @dataclass
-class Tcdps:
+class Tcdps(CommonMixin):
     class Meta:
         name = "TCDPS"
 
     infDPS: Optional[TcinfDps] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
     signature: Optional[Signature] = field(
         default=None,
         metadata={
             "name": "Signature",
             "type": "Element",
             "namespace": "http://www.w3.org/2000/09/xmldsig#",
-        }
+        },
     )
     versao: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "required": True,
             "white_space": "preserve",
             "pattern": r"1\.00",
-        }
+        },
     )
 
 
 @dataclass
-class TcinfNfse:
+class TcinfNfse(CommonMixin):
     """
     :ivar xLocEmi: Descrição do código do IBGE do município emissor da
         NFS-e.
     :ivar xLocPrestacao: Descrição do local da prestação do serviço.
     :ivar nNFSe: Número sequencial por tipo de emitente da NFS-e. A
         Sefin Nacional NFS-e irá gerar o número da NFS-e de forma
         sequencial por emitente. Por se tratar de um ambiente altamente
@@ -2894,231 +2940,232 @@
         gerador de DFSe do múnicípio.
     :ivar emit: Grupo de informações da DPS relativas ao emitente da
         NFS-e
     :ivar valores: Grupo de valores referentes ao Serviço Prestado
     :ivar DPS: Grupo de informações da DPS relativas ao serviço prestado
     :ivar Id:
     """
+
     class Meta:
         name = "TCInfNFSe"
 
     xLocEmi: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "min_length": 1,
             "max_length": 150,
             "white_space": "preserve",
             "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
-        }
+        },
     )
     xLocPrestacao: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "min_length": 1,
             "max_length": 150,
             "white_space": "preserve",
             "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
-        }
+        },
     )
     nNFSe: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "max_length": 13,
             "white_space": "preserve",
             "pattern": r"[1-9]{1}[0-9]{0,12}",
-        }
+        },
     )
     cLocIncid: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "white_space": "preserve",
             "pattern": r"[0-9]{7}",
-        }
+        },
     )
     xLocIncid: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "min_length": 1,
             "max_length": 150,
             "white_space": "preserve",
             "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
-        }
+        },
     )
     xTribNac: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "min_length": 1,
             "max_length": 600,
             "white_space": "preserve",
             "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
-        }
+        },
     )
     xTribMun: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "min_length": 1,
             "max_length": 600,
             "white_space": "preserve",
             "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
-        }
+        },
     )
     xNBS: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "min_length": 1,
             "max_length": 600,
             "white_space": "preserve",
             "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
-        }
+        },
     )
     verAplic: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "min_length": 1,
             "max_length": 20,
             "white_space": "preserve",
             "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
-        }
+        },
     )
     ambGer: Optional[TsambGeradorNfse] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
     tpEmis: Optional[TstipoEmissao] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
     procEmi: Optional[TsprocEmissao] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
     cStat: Optional[Tstat] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
     dhProc: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "white_space": "preserve",
             "pattern": r"(((20(([02468][048])|([13579][26]))-02-29))|(20[0-9][0-9])-((((0[1-9])|(1[0-2]))-((0[1-9])|(1\d)|(2[0-8])))|((((0[13578])|(1[02]))-31)|(((0[1,3-9])|(1[0-2]))-(29|30)))))T(20|21|22|23|[0-1]\d):[0-5]\d:[0-5]\d([\-,\+](0[0-9]|10|11):00|([\+](12):00))",
-        }
+        },
     )
     nDFSe: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
             "max_length": 13,
             "white_space": "preserve",
             "pattern": r"[1-9]{1}[0-9]{0,12}",
-        }
+        },
     )
     emit: Optional[Tcemitente] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
     valores: Optional[TcvaloresNfse] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
     DPS: Optional[Tcdps] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
     Id: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "required": True,
             "max_length": 53,
             "white_space": "preserve",
             "pattern": r"NFS[0-9]{50}",
-        }
+        },
     )
 
 
 @dataclass
-class Tcnfse:
+class Tcnfse(CommonMixin):
     class Meta:
         name = "TCNFSe"
 
     infNFSe: Optional[TcinfNfse] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.sped.fazenda.gov.br/nfse",
             "required": True,
-        }
+        },
     )
     signature: Optional[Signature] = field(
         default=None,
         metadata={
             "name": "Signature",
             "type": "Element",
             "namespace": "http://www.w3.org/2000/09/xmldsig#",
             "required": True,
-        }
+        },
     )
     versao: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "required": True,
             "white_space": "preserve",
             "pattern": r"1\.00",
-        }
+        },
     )
```

## Comparing `nfelib-2.0.4/nfelib/nfse/bindings/v1_0/tipos_simples_v1_00.py` & `nfelib-2.0.5/nfelib/nfse/bindings/v1_0/tipos_simples_v1_00.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,29 @@
+"""This file was generated by xsdata, v24.2.1, on 2024-03-11 16:13:50
+
+Generator: DataclassGenerator
+See: https://xsdata.readthedocs.io/
+"""
 from enum import Enum
 
 __NAMESPACE__ = "http://www.sped.fazenda.gov.br/nfse"
 
 
 class TcobjetoLocacao(Enum):
-    """Tipo de objetos da locação, sublocação, arrendamento, direito de
-    passagem ou permissão de uso:
+    """Tipo de objetos da locação, sublocação, arrendamento, direito de passagem ou
+    permissão de uso:
 
     1 - Ferrovia;
     2 - Rodovia;
     3 - Postes;
     4 - Cabos;
     5 - Dutos;
     6 - Condutos de qualquer natureza;
     """
+
     VALUE_1 = "1"
     VALUE_2 = "2"
     VALUE_3 = "3"
     VALUE_4 = "4"
     VALUE_5 = "5"
     VALUE_6 = "6"
 
@@ -25,25 +31,27 @@
 class TsambGeradorEvt(Enum):
     """Tipo Ambiente gerador do evento:
 
     1- Prefeitura;
     2- Sefin Nacional;
     3- Ambiente Nacional.
     """
+
     VALUE_1 = "1"
     VALUE_2 = "2"
     VALUE_3 = "3"
 
 
 class TsambGeradorNfse(Enum):
     """Tipo Ambiente Gerador de NFS-e:
 
     1 - Prefeitura;
     2 - Sistema Nacional da NFS-e;
     """
+
     VALUE_1 = "1"
     VALUE_2 = "2"
 
 
 class TscategVeic(Enum):
     """Categorias de veículos para cobrança:
 
@@ -56,14 +64,15 @@
     06 - Caminhão com reboque e caminhãotrator com semi-reboque;
     07 - Caminhão com reboque e caminhãotrator com semi-reboque;
     08 - Caminhão com reboque e caminhãotrator com semi-reboque;
     09 - Motocicletas, motonetas e bicicletas motorizadas;
     10 - Veículo especial;
     11 - Veículo Isento;
     """
+
     VALUE_00 = "00"
     VALUE_01 = "01"
     VALUE_02 = "02"
     VALUE_03 = "03"
     VALUE_04 = "04"
     VALUE_05 = "05"
     VALUE_06 = "06"
@@ -79,14 +88,15 @@
 
     1 - Locação;
     2 - Sublocação;
     3 - Arrendamento;
     4 - Direito de passagem;
     5 - Permissão de uso;
     """
+
     VALUE_1 = "1"
     VALUE_2 = "2"
     VALUE_3 = "3"
     VALUE_4 = "4"
     VALUE_5 = "5"
 
 
@@ -94,46 +104,48 @@
     """Código do motivo da solicitação de análise fiscal para cancelamento de
     NFS-e:
 
     1 - Erro na Emissão;
     2 - Serviço não Prestado;
     3 - Outros.
     """
+
     VALUE_1 = "1"
     VALUE_2 = "2"
     VALUE_9 = "9"
 
 
 class TscodJustAnaliseFiscalCancDef(Enum):
-    """Resposta da análise da solicitação do cancelamento extemporâneo de
-    NFS-e:
+    """Resposta da análise da solicitação do cancelamento extemporâneo de NFS-e:
 
     1 - Cancelamento Extemporâneo Deferido.
     """
+
     VALUE_1 = "1"
 
 
 class TscodJustAnaliseFiscalCancIndef(Enum):
-    """Resposta da análise da solicitação do cancelamento extemporâneo de
-    NFS-e:
+    """Resposta da análise da solicitação do cancelamento extemporâneo de NFS-e:
 
     1 - Cancelamento Extemporâneo Indeferido;
     2 - Cancelamento Extemporâneo Indeferido Sem Análise de Mérito.
     """
+
     VALUE_1 = "1"
     VALUE_2 = "2"
 
 
 class TscodJustCanc(Enum):
     """Código de justificativa de cancelamento:
 
     1 - Erro na Emissão;
     2 - Serviço não Prestado;
     9 - Outros;
     """
+
     VALUE_1 = "1"
     VALUE_2 = "2"
     VALUE_9 = "9"
 
 
 class TscodJustSubst(Enum):
     """Código de justificativa para substituição de NFS-e:
@@ -141,14 +153,15 @@
     01 - Desenquadramento de NFS-e do Simples Nacional;
     02 - Enquadramento de NFS-e no Simples Nacional;
     03 - Inclusão Retroativa de Imunidade/Isenção para NFS-e;
     04 - Exclusão Retroativa de Imunidade/Isenção para NFS-e;
     05 - Rejeição de NFS-e pelo tomador ou pelo intermediário se responsável pelo recolhimento do tributo;
     99 - Outros;
     """
+
     VALUE_01 = "01"
     VALUE_02 = "02"
     VALUE_03 = "03"
     VALUE_04 = "04"
     VALUE_05 = "05"
     VALUE_99 = "99"
 
@@ -159,14 +172,15 @@
     1 - NFS-e em duplicidade;
     2 - NFS-e já emitida pelo tomador;
     3 - Não ocorrência do fato gerador;
     4 - Erro quanto a responsabilidade tributária;
     5 - Erro quanto ao valor do serviço, valor das deduções ou serviço prestado ou data do fato gerador;
     9 - Outros;
     """
+
     VALUE_1 = "1"
     VALUE_2 = "2"
     VALUE_3 = "3"
     VALUE_4 = "4"
     VALUE_5 = "5"
     VALUE_9 = "9"
 
@@ -174,23 +188,25 @@
 class TscodNaoNif(Enum):
     """Motivo para não informação do NIF:
 
     0 - Não informado na nota de origem;
     1 - Dispensado do NIF;
     2 - Não exigência do NIF;
     """
+
     VALUE_0 = "0"
     VALUE_1 = "1"
     VALUE_2 = "2"
 
 
 class TscodigoEventoNfse(Enum):
     """
     Código de evento da NFS-e.
     """
+
     E101101 = "e101101"
     E105102 = "e105102"
     E105104 = "e105104"
     E105105 = "e105105"
     E305101 = "e305101"
     E907202 = "e907202"
     E967203 = "e967203"
@@ -199,77 +215,81 @@
 class TsemitenteDps(Enum):
     """Emitente da DPS:
 
     1 - Prestador
     2 - Tomador
     3 - Intermediário
     """
+
     VALUE_1 = "1"
     VALUE_2 = "2"
     VALUE_3 = "3"
 
 
 class TsenvMdic(Enum):
     """Compartilhar as informações da NFS-e gerada a partir desta DPS com a
     Secretaria de Comércio Exterior:
 
     0 - Não enviar para o MDIC;
     1 - Enviar para o MDIC;
     """
+
     VALUE_0 = "0"
     VALUE_1 = "1"
 
 
 class TsideDedRed(Enum):
     """Identificação da Dedução/Redução:
 
     1 – Alimentação e bebidas/frigobar; 2 – Materiais; 3 – Produção
     externa; 4 – Reembolso de despesas; 5 – Repasse consorciado; 6 –
     Repasse plano de saúde; 7 – Serviços; 8 – Subempreitada de mão de
     obra; 99 – Outras deduções;
     """
+
     VALUE_1 = "1"
     VALUE_2 = "2"
     VALUE_3 = "3"
     VALUE_4 = "4"
     VALUE_5 = "5"
     VALUE_6 = "6"
     VALUE_7 = "7"
     VALUE_8 = "8"
     VALUE_99 = "99"
 
 
 class TsmecAfcomExPrest(Enum):
-    """Mecanismo de apoio/fomento ao Comércio Exterior utilizado pelo prestador
-    do serviço:
+    """Mecanismo de apoio/fomento ao Comércio Exterior utilizado pelo prestador do
+    serviço:
 
     00 - Desconhecido (tipo não informado na nota de origem);
     01 - Nenhum;
     02 - ACC - Adiantamento sobre Contrato de Câmbio – Redução a Zero do IR e do IOF;
     03 - ACE – Adiantamento sobre Cambiais Entregues - Redução a Zero do IR e do IOF;
     04 - BNDES-Exim Pós-Embarque – Serviços;
     05 - BNDES-Exim Pré-Embarque - Serviços;
     06 - FGE - Fundo de Garantia à Exportação;
     07 - PROEX - EQUALIZAÇÃO
     08 - PROEX - Financiamento;
     """
+
     VALUE_00 = "00"
     VALUE_01 = "01"
     VALUE_02 = "02"
     VALUE_03 = "03"
     VALUE_04 = "04"
     VALUE_05 = "05"
     VALUE_06 = "06"
     VALUE_07 = "07"
     VALUE_08 = "08"
 
 
 class TsmecAfcomExToma(Enum):
-    """Mecanismo de apoio/fomento ao Comércio Exterior utilizado pelo tomador
-    do serviço:
+    """Mecanismo de apoio/fomento ao Comércio Exterior utilizado pelo tomador do
+    serviço:
 
     00 - Desconhecido (tipo não informado na nota de origem);
     01 - Nenhum;
     02 - Adm. Pública e Repr. Internacional;
     03 - Alugueis e Arrend. Mercantil de maquinas, equip., embarc. e aeronaves;
     04 - Arrendamento Mercantil de aeronave para empresa de transporte aéreo público;
     05 - Comissão a agentes externos na exportação;
@@ -291,14 +311,15 @@
     21 - REPES;
     22 - RETAERO;
     23 - RETID;
     24 - Royalties, Assistência Técnica, Científica e Assemelhados;
     25 - Serviços de avaliação da conformidade vinculados aos Acordos da OMC;
     26 - ZPE;
     """
+
     VALUE_00 = "00"
     VALUE_01 = "01"
     VALUE_02 = "02"
     VALUE_03 = "03"
     VALUE_04 = "04"
     VALUE_05 = "05"
     VALUE_06 = "06"
@@ -329,14 +350,15 @@
 
     0 - Desconhecido (tipo não informado na nota de origem);
     1 - Transfronteiriço;
     2 - Consumo no Brasil;
     3 - Presença Comercial no Exterior;
     4 - Movimento Temporário de Pessoas Físicas;
     """
+
     VALUE_0 = "0"
     VALUE_1 = "1"
     VALUE_2 = "2"
     VALUE_3 = "3"
     VALUE_4 = "4"
 
 
@@ -344,72 +366,78 @@
     """Operação está vinculada à Movimentação Temporária de Bens:
 
     0 - Desconhecido (tipo não informado na nota de origem);
     1 - Não
     2 - Vinculada - Declaração de Importação
     3 - Vinculada - Declaração de Exportação
     """
+
     VALUE_0 = "0"
     VALUE_1 = "1"
     VALUE_2 = "2"
     VALUE_3 = "3"
 
 
 class TsopConsumServ(Enum):
     """Opção para que o emitente informe onde ocorreu o consumo do serviço
     prestado.
 
     0 - Consumo do serviço prestado ocorrido no município do local da prestação;
     1 - Consumo do serviço prestado ocorrido ocorrido no exterior ;
     """
+
     VALUE_0 = "0"
     VALUE_1 = "1"
 
 
 class TsopExigSuspensa(Enum):
     """Opção para Exigibilidade Suspensa:
 
     1 - Exigibilidade Suspensa por Decisão Judicial;
     2 - Exigibilidade Suspensa por Processo Administrativo;
     """
+
     VALUE_1 = "1"
     VALUE_2 = "2"
 
 
 class TsopSimpNac(Enum):
     """Situação perante o Simples Nacional:
 
     1 - Não Optante;
     2 - Optante - Microempreendedor Individual (MEI);
     3 - Optante - Microempresa ou Empresa de Pequeno Porte (ME/EPP);
     """
+
     VALUE_1 = "1"
     VALUE_2 = "2"
     VALUE_3 = "3"
 
 
 class TsopTipoBm(Enum):
     """Tipo do Benefício Municipal:
 
     1 - Alíquota Diferenciada;
     2 - Redução da BC;
     3 - Isenção;
     """
+
     VALUE_1 = "1"
     VALUE_2 = "2"
     VALUE_3 = "3"
 
 
 class TsprocEmissao(Enum):
     """Processo de Emissão da DPS:
 
     1 - Emissão com aplicativo do contribuinte (via Web Service);
     2 - Emissão com aplicativo disponibilizado pelo fisco (Web);
     3 - Emissão com aplicativo disponibilizado pelo fisco (App);
     """
+
     VALUE_1 = "1"
     VALUE_2 = "2"
     VALUE_3 = "3"
 
 
 class TsregEspTrib(Enum):
     """Tipos de Regimes Especiais de Tributação:
@@ -418,45 +446,49 @@
     1 - Ato Cooperado (Cooperativa);
     2 - Estimativa;
     3 - Microempresa Municipal;
     4 - Notário ou Registrador;
     5 - Profissional Autônomo;
     6 - Sociedade de Profissionais;
     """
+
     VALUE_0 = "0"
     VALUE_1 = "1"
     VALUE_2 = "2"
     VALUE_3 = "3"
     VALUE_4 = "4"
     VALUE_5 = "5"
     VALUE_6 = "6"
 
 
 class TsregimeApuracaoSimpNac(Enum):
     """Opção para que o contribuinte optante pelo Simples Nacional ME/EPP (opSimpNac = 3) possa indicar, ao emitir o documento fiscal, em qual regime de apuração os tributos federais e municipal estão inseridos, caso tenha ultrapassado algum sublimite ou limite definido para o Simples Nacional.
     1 – Regime de apuração dos tributos federais e municipal pelo SN;
     2 – Regime de apuração dos tributos federais pelo SN e ISSQN  por fora do SN conforme respectiva legislação municipal do tributo;
     3 – Regime de apuração dos tributos federais e municipal por fora do SN conforme respectivas legilações federal e municipal de cada tributo;"""
+
     VALUE_1 = "1"
     VALUE_2 = "2"
     VALUE_3 = "3"
 
 
 class Tsrodagem(Enum):
     """Tipo de rodagem:
 
     1 - Simples;
     2 - Dupla;
     """
+
     VALUE_1 = "1"
     VALUE_2 = "2"
 
 
 class TstipoAmbiente(Enum):
     """Tipos de ambiente do Sistema Nacional NFS-e: 1 - Produção; 2 - Homologação;"""
+
     VALUE_1 = "1"
     VALUE_2 = "2"
 
 
 class TstipoCst(Enum):
     """Código de Situação Tributária do PIS/COFINS (CST):
 
@@ -467,14 +499,15 @@
     04 - Operação Tributável monofásica - Revenda a Alíquota Zero;
     05 - Operação Tributável por Substituição Tributária;
     06 - Operação Tributável a Alíquota Zero;
     07 - Operação Tributável da Contribuição;
     08 - Operação sem Incidência da Contribuição;
     09 - Operação com Suspensão da Contribuição;
     """
+
     VALUE_00 = "00"
     VALUE_01 = "01"
     VALUE_02 = "02"
     VALUE_03 = "03"
     VALUE_04 = "04"
     VALUE_05 = "05"
     VALUE_06 = "06"
@@ -485,87 +518,94 @@
 
 class TstipoEmissao(Enum):
     """Tipo de emissão da NFS-e:
 
     1 - Emissão normal no modelo da NFS-e Nacional;
     2 - Emissão original em leiaute próprio do município com transcrição para o modelo da NFS-e Nacional.
     """
+
     VALUE_1 = "1"
     VALUE_2 = "2"
 
 
 class TstipoImunidadeIssqn(Enum):
     """Identificação da Imunidade do ISSQN – somente para o caso de Imunidade.
-    Tipos de Imunidades:
 
+    Tipos de Imunidades:
     0 - Imunidade (tipo não informado na nota de origem);
     1 - Patrimônio, renda ou serviços, uns dos outros (CF88, Art 150, VI, a);
     2 - Templos de qualquer culto (CF88, Art 150, VI, b);
     3 - Patrimônio, renda ou serviços dos partidos políticos, inclusive suas fundações, das entidades sindicais dos trabalhadores, das instituições de        educação e de assistência social, sem fins lucrativos, atendidos os requisitos da lei (CF88, Art 150, VI, c);
     4 - Livros, jornais, periódicos e o papel destinado a sua impressão (CF88, Art 150, VI, d);
     5 - Fonogramas e videofonogramas musicais produzidos no Brasil contendo obras musicais ou literomusicais de autores brasileiros e/ou obras em geral interpretadas por artistas brasileiros bem como os suportes materiais ou arquivos digitais que os contenham, salvo na etapa de replicação industrial de mídias ópticas de leitura a laser.   (CF88, Art 150, VI, e);
     """
+
     VALUE_0 = "0"
     VALUE_1 = "1"
     VALUE_2 = "2"
     VALUE_3 = "3"
     VALUE_4 = "4"
     VALUE_5 = "5"
 
 
 class TstipoIndTotTrib(Enum):
-    """Indicador de informação de valor total de tributos. Possui valor fixo
-    igual a zero (indTotTrib=0). Não informar nenhum valor estimado para os
-    Tributos (Decreto 8.264/2014).
+    """Indicador de informação de valor total de tributos. Possui valor fixo igual
+    a zero (indTotTrib=0).
 
+    Não informar nenhum valor estimado para os Tributos (Decreto 8.264/2014).
     0 - Não;
     """
+
     VALUE_0 = "0"
 
 
 class TstipoRetIssqn(Enum):
     """Tipo de retencao do ISSQN:
 
     1 - Não Retido;
     2 - Retido pelo Tomador;
     3 - Retido pelo Intermediario;
     """
+
     VALUE_1 = "1"
     VALUE_2 = "2"
     VALUE_3 = "3"
 
 
 class TstipoRetPiscofins(Enum):
     """Tipo de retencao do Pis/Cofins:
 
     1 - Retido;
     2 - Não Retido;
     """
+
     VALUE_1 = "1"
     VALUE_2 = "2"
 
 
 class TstribIssqn(Enum):
     """Tributação do ISSQN sobre o serviço prestado:
 
     1 - Operação tributável;
     2 - Exportação de serviço;
     3 - Não Incidência;
     4 - Imunidade;
     """
+
     VALUE_1 = "1"
     VALUE_2 = "2"
     VALUE_3 = "3"
     VALUE_4 = "4"
 
 
 class Tsuf(Enum):
     """
     Tipo Sigla da UF.
     """
+
     AC = "AC"
     AL = "AL"
     AM = "AM"
     AP = "AP"
     BA = "BA"
     CE = "CE"
     DF = "DF"
@@ -598,24 +638,26 @@
     1 - Controlada;
     2 - Controladora;
     3 - Coligada;
     4 - Matriz;
     5 - Filial ou sucursal;
     6 - Outro vínculo;
     """
+
     VALUE_1 = "1"
     VALUE_2 = "2"
     VALUE_3 = "3"
     VALUE_4 = "4"
     VALUE_5 = "5"
     VALUE_6 = "6"
 
 
 class Tstat(Enum):
     """100 - NFS-e Gerada;
     101 - NFS-e de Substituição Gerada;
     102 - NFS-e de Decisão Judicial;
     103 - NFS-e Avulsa;" """
+
     VALUE_100 = "100"
     VALUE_101 = "101"
     VALUE_102 = "102"
     VALUE_103 = "103"
```

## Comparing `nfelib-2.0.4/nfelib/nfse/bindings/v1_0/xmldsig_core_schema_v1_00.py` & `nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/xmldsig_core_schema_v1_01.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,256 +1,269 @@
+"""This file was generated by xsdata, v24.4, on 2024-05-08 08:25:46
+
+Generator: DataclassGenerator
+See: https://xsdata.readthedocs.io/
+"""
 from dataclasses import dataclass, field
 from enum import Enum
 from typing import List, Optional
 
+from nfelib import CommonMixin
+
 __NAMESPACE__ = "http://www.w3.org/2000/09/xmldsig#"
 
 
 @dataclass
-class SignatureValueType:
+class SignatureValueType(CommonMixin):
     value: Optional[bytes] = field(
         default=None,
         metadata={
             "required": True,
             "format": "base64",
-        }
+        },
     )
     Id: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-        }
+        },
     )
 
 
 class TtransformUri(Enum):
-    HTTP_WWW_W3_ORG_2000_09_XMLDSIG_ENVELOPED_SIGNATURE = "http://www.w3.org/2000/09/xmldsig#enveloped-signature"
-    HTTP_WWW_W3_ORG_TR_2001_REC_XML_C14N_20010315 = "http://www.w3.org/TR/2001/REC-xml-c14n-20010315"
+    HTTP_WWW_W3_ORG_2000_09_XMLDSIG_ENVELOPED_SIGNATURE = (
+        "http://www.w3.org/2000/09/xmldsig#enveloped-signature"
+    )
+    HTTP_WWW_W3_ORG_TR_2001_REC_XML_C14N_20010315 = (
+        "http://www.w3.org/TR/2001/REC-xml-c14n-20010315"
+    )
 
 
 @dataclass
-class X509DataType:
+class X509DataType(CommonMixin):
     X509Certificate: Optional[bytes] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.w3.org/2000/09/xmldsig#",
             "required": True,
             "format": "base64",
-        }
+        },
     )
 
 
 @dataclass
-class KeyInfoType:
+class KeyInfoType(CommonMixin):
     X509Data: Optional[X509DataType] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "http://www.w3.org/2000/09/xmldsig#",
             "required": True,
-        }
+        },
     )
     Id: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-        }
+        },
     )
 
 
 @dataclass
-class TransformType:
+class TransformType(CommonMixin):
     XPath: List[str] = field(
         default_factory=list,
         metadata={
             "type": "Element",
             "namespace": "http://www.w3.org/2000/09/xmldsig#",
-        }
+        },
     )
     Algorithm: Optional[TtransformUri] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "required": True,
-        }
+        },
     )
 
 
 @dataclass
-class TransformsType:
+class TransformsType(CommonMixin):
     transform: List[TransformType] = field(
         default_factory=list,
         metadata={
             "name": "Transform",
             "type": "Element",
             "namespace": "http://www.w3.org/2000/09/xmldsig#",
             "min_occurs": 2,
             "max_occurs": 2,
-        }
+        },
     )
 
 
 @dataclass
-class ReferenceType:
+class ReferenceType(CommonMixin):
     transforms: Optional[TransformsType] = field(
         default=None,
         metadata={
             "name": "Transforms",
             "type": "Element",
             "namespace": "http://www.w3.org/2000/09/xmldsig#",
             "required": True,
-        }
+        },
     )
     digestMethod: Optional["ReferenceType.DigestMethod"] = field(
         default=None,
         metadata={
             "name": "DigestMethod",
             "type": "Element",
             "namespace": "http://www.w3.org/2000/09/xmldsig#",
             "required": True,
-        }
+        },
     )
     digestValue: Optional[bytes] = field(
         default=None,
         metadata={
             "name": "DigestValue",
             "type": "Element",
             "namespace": "http://www.w3.org/2000/09/xmldsig#",
             "required": True,
             "format": "base64",
-        }
+        },
     )
     Id: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-        }
+        },
     )
     URI: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "required": True,
             "min_length": 2,
-        }
+        },
     )
     Type_value: Optional[str] = field(
         default=None,
         metadata={
             "name": "Type",
             "type": "Attribute",
-        }
+        },
     )
 
     @dataclass
-    class DigestMethod:
+    class DigestMethod(CommonMixin):
         Algorithm: str = field(
             init=False,
             default="http://www.w3.org/2000/09/xmldsig#sha1",
             metadata={
                 "type": "Attribute",
                 "required": True,
-            }
+            },
         )
 
 
 @dataclass
-class SignedInfoType:
-    canonicalizationMethod: Optional["SignedInfoType.CanonicalizationMethod"] = field(
+class SignedInfoType(CommonMixin):
+    canonicalizationMethod: Optional[
+        "SignedInfoType.CanonicalizationMethod"
+    ] = field(
         default=None,
         metadata={
             "name": "CanonicalizationMethod",
             "type": "Element",
             "namespace": "http://www.w3.org/2000/09/xmldsig#",
             "required": True,
-        }
+        },
     )
     signatureMethod: Optional["SignedInfoType.SignatureMethod"] = field(
         default=None,
         metadata={
             "name": "SignatureMethod",
             "type": "Element",
             "namespace": "http://www.w3.org/2000/09/xmldsig#",
             "required": True,
-        }
+        },
     )
     reference: Optional[ReferenceType] = field(
         default=None,
         metadata={
             "name": "Reference",
             "type": "Element",
             "namespace": "http://www.w3.org/2000/09/xmldsig#",
             "required": True,
-        }
+        },
     )
     Id: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-        }
+        },
     )
 
     @dataclass
-    class CanonicalizationMethod:
+    class CanonicalizationMethod(CommonMixin):
         Algorithm: str = field(
             init=False,
             default="http://www.w3.org/TR/2001/REC-xml-c14n-20010315",
             metadata={
                 "type": "Attribute",
                 "required": True,
-            }
+            },
         )
 
     @dataclass
-    class SignatureMethod:
+    class SignatureMethod(CommonMixin):
         Algorithm: str = field(
             init=False,
             default="http://www.w3.org/2000/09/xmldsig#rsa-sha1",
             metadata={
                 "type": "Attribute",
                 "required": True,
-            }
+            },
         )
 
 
 @dataclass
-class SignatureType:
+class SignatureType(CommonMixin):
     signedInfo: Optional[SignedInfoType] = field(
         default=None,
         metadata={
             "name": "SignedInfo",
             "type": "Element",
             "namespace": "http://www.w3.org/2000/09/xmldsig#",
             "required": True,
-        }
+        },
     )
     signatureValue: Optional[SignatureValueType] = field(
         default=None,
         metadata={
             "name": "SignatureValue",
             "type": "Element",
             "namespace": "http://www.w3.org/2000/09/xmldsig#",
             "required": True,
-        }
+        },
     )
     keyInfo: Optional[KeyInfoType] = field(
         default=None,
         metadata={
             "name": "KeyInfo",
             "type": "Element",
             "namespace": "http://www.w3.org/2000/09/xmldsig#",
             "required": True,
-        }
+        },
     )
     Id: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-        }
+        },
     )
 
 
 @dataclass
 class Signature(SignatureType):
     class Meta:
         namespace = "http://www.w3.org/2000/09/xmldsig#"
```

## Comparing `nfelib-2.0.4/nfelib/nfse/schemas/v1_0/tiposEventos_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfse/schemas/v1_0/tiposEventos_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfse/schemas/v1_0/NFSe_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfse/schemas/v1_0/NFSe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfse/schemas/v1_0/pedRegEvento_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfse/schemas/v1_0/pedRegEvento_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfse/schemas/v1_0/tiposComplexos_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfse/schemas/v1_0/tiposComplexos_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfse/schemas/v1_0/DPS_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfse/schemas/v1_0/DPS_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfse/schemas/v1_0/xmldsig-core-schema_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfse/schemas/v1_0/xmldsig-core-schema_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfse/schemas/v1_0/tiposSimples_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfse/schemas/v1_0/tiposSimples_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfse/schemas/v1_0/evento_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfse/schemas/v1_0/evento_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/v4_00/retConsStatServ.py` & `nfelib-2.0.5/nfelib/v4_00/retConsStatServ.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/v4_00/retEnviNFe.py` & `nfelib-2.0.5/nfelib/v4_00/retEnviNFe.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/v4_00/retEnvConfRecebto.py` & `nfelib-2.0.5/nfelib/v4_00/retEnvConfRecebto.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/v4_00/retEnvEvento.py` & `nfelib-2.0.5/nfelib/v4_00/retEnvEvento.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/v4_00/leiauteNFe_sub.py` & `nfelib-2.0.5/nfelib/v4_00/leiauteNFe_sub.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,30 @@
 # Copyright (C) 2019 - TODAY Raphaël Valyi - Akretion
 
 import sys
 import os
 from lxml import etree as etree_
+import warnings
 
 sys.path.append(os.path.dirname(__file__))
 import retEnviNFe as supermod
 
 
+warnings.warn(
+    (
+        "These nfelib 1.x bindings (nfelib.v4_00; generated with GenerateDS) "
+        "are deprecated and will be removed after 01/06/2024. "
+        "\nYou should use the nfelib 2.x xsdata bindings in nfelib.nfe.bindings "
+        "instead.\nYou can learn about the migration process here: "
+        "https://github.com/akretion/nfelib/issues/59"
+    ),
+    DeprecationWarning,
+)
+
+
 def parsexml_(infile, parser=None, keep_signature=False, **kwargs):
     "accepts both NFe and nfeProc documents"
 
     if not parser:
         # Use the lxml ElementTree compatible parser so that, e.g.,
         # we ignore comments.
         parser = etree_.ETCompatXMLParser()
```

## Comparing `nfelib-2.0.4/nfelib/v4_00/retInutNFe.py` & `nfelib-2.0.5/nfelib/v4_00/retInutNFe.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/v4_00/retConsCad.py` & `nfelib-2.0.5/nfelib/v4_00/retConsCad.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/v4_00/distDFeInt.py` & `nfelib-2.0.5/nfelib/v4_00/distDFeInt.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/v4_00/retDistDFeInt.py` & `nfelib-2.0.5/nfelib/v4_00/retDistDFeInt.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/v4_00/retConsReciNFe.py` & `nfelib-2.0.5/nfelib/v4_00/retConsReciNFe.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/v4_00/retEnvCCe.py` & `nfelib-2.0.5/nfelib/v4_00/retEnvCCe.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/v4_00/retEnvEventoCancNFe.py` & `nfelib-2.0.5/nfelib/v4_00/retEnvEventoCancNFe.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/v4_00/retConsSitNFe.py` & `nfelib-2.0.5/nfelib/v4_00/retConsSitNFe.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/samples/v3_0/inclusaoDFe1101154119060611747300015058001000000001111700344401-ped-eve.xml` & `nfelib-2.0.5/nfelib/mdfe/samples/v3_0/inclusaoDFe1101154119060611747300015058001000000001111700344401-ped-eve.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/samples/v3_0/pagamentoOperacao1101103511031029073900013955001000000001105112804101-ped-eve.xml` & `nfelib-2.0.5/nfelib/mdfe/samples/v3_0/pagamentoOperacao1101103511031029073900013955001000000001105112804101-ped-eve.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/samples/v3_0/PagamentoOperacaoMDFe_1101164120039999999999999958001000000999999999999901-ped-eve.xml` & `nfelib-2.0.5/nfelib/mdfe/samples/v3_0/PagamentoOperacaoMDFe_1101164120039999999999999958001000000999999999999901-ped-eve.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/samples/v3_0/26999999999999999999999999999999999999999991-mdfe.xml` & `nfelib-2.0.5/nfelib/mdfe/samples/v3_0/26999999999999999999999999999999999999999991-mdfe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/samples/v3_0/41190876676436000167580010000500001000437558-mdfe.xml` & `nfelib-2.0.5/nfelib/mdfe/samples/v3_0/41190876676436000167580010000500001000437558-mdfe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/samples/v3_0/50170876063965000276580010000011311421039568-mdfe.xml` & `nfelib-2.0.5/nfelib/mdfe/samples/v3_0/50170876063965000276580010000011311421039568-mdfe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/samples/v3_0/ComPagtoPIX_41210780568835000181580010402005751006005791-procMDFe.xml` & `nfelib-2.0.5/nfelib/mdfe/samples/v3_0/ComPagtoPIX_41210780568835000181580010402005751006005791-procMDFe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/samples/v3_0/cancelameto1101103511031029073900013955001000000001105112804101-ped-eve.xml` & `nfelib-2.0.5/nfelib/mdfe/samples/v3_0/cancelameto1101103511031029073900013955001000000001105112804101-ped-eve.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/samples/v3_0/encerramento1101123511031029073900013955001000000001105112804101-ped-eve.xml` & `nfelib-2.0.5/nfelib/mdfe/samples/v3_0/encerramento1101123511031029073900013955001000000001105112804101-ped-eve.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/samples/v3_0/inclusaocondutor31131223864838000129580000000000051003000003-ped-eve.xml` & `nfelib-2.0.5/nfelib/mdfe/samples/v3_0/inclusaocondutor31131223864838000129580000000000051003000003-ped-eve.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/ret_cons_stat_serv_mdfe_v3_00.py` & `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ret_cons_stat_serv_mdfe_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/xmldsig_core_schema_v1_01.py` & `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/xmldsig_core_schema_v1_01.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/cons_stat_serv_tipos_basico_v3_00.py` & `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/cons_stat_serv_tipos_basico_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/__init__.py` & `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/__init__.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/proc_evento_mdfe_v3_00.py` & `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/proc_evento_mdfe_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/cons_sit_mdfe_tipos_basico_v3_00.py` & `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/cons_sit_mdfe_tipos_basico_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/mdfe_consulta_dfe_tipos_basico_v3_00.py` & `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/mdfe_consulta_dfe_tipos_basico_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/ret_evento_mdfe_v3_00.py` & `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ret_evento_mdfe_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/leiaute_dist_mdfe_v3_00.py` & `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/leiaute_dist_mdfe_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/mdfe_consulta_dfe_v3_00.py` & `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/mdfe_consulta_dfe_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/ev_pagto_oper_mdfe_v3_00.py` & `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ev_pagto_oper_mdfe_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/ev_inc_condutor_mdfe_v3_00.py` & `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ev_inc_condutor_mdfe_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/tipos_geral_mdfe_v3_00.py` & `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/tipos_geral_mdfe_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/ret_cons_sit_mdfe_v3_00.py` & `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ret_cons_sit_mdfe_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/ret_cons_reci_mdfe_v3_00.py` & `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ret_cons_reci_mdfe_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/ret_envi_mdfe_v3_00.py` & `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ret_envi_mdfe_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/envi_mdfe_v3_00.py` & `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/envi_mdfe_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/cons_mdfe_nao_enc_v3_00.py` & `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/cons_mdfe_nao_enc_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/cons_mdfe_nao_enc_tipos_basico_v3_00.py` & `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/cons_mdfe_nao_enc_tipos_basico_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/ret_dist_mdfe_v3_00.py` & `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ret_dist_mdfe_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/evento_mdfe_v3_00.py` & `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/evento_mdfe_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/mdfe_modal_rodoviario_v3_00.py` & `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/mdfe_modal_rodoviario_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/evento_mdfe_tipos_basico_v3_00.py` & `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/evento_mdfe_tipos_basico_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/ev_canc_mdfe_v3_00.py` & `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ev_canc_mdfe_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/mdfe_modal_aquaviario_v3_00.py` & `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/mdfe_modal_aquaviario_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/ret_cons_mdfe_nao_enc_v3_00.py` & `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ret_cons_mdfe_nao_enc_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/ret_mdfe_consulta_dfe_v3_00.py` & `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ret_mdfe_consulta_dfe_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/dist_mdfe_v3_00.py` & `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/dist_mdfe_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/cons_reci_mdfe_tipos_basico_v3_00.py` & `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/cons_reci_mdfe_tipos_basico_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/mdfe_modal_ferroviario_v3_00.py` & `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/mdfe_modal_ferroviario_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/ev_inclusao_dfe_mdfe_v3_00.py` & `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ev_inclusao_dfe_mdfe_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/cons_sit_mdfe_v3_00.py` & `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/cons_sit_mdfe_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/mdfe_tipos_basico_v3_00.py` & `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/mdfe_tipos_basico_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/ev_enc_mdfe_v3_00.py` & `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/ev_enc_mdfe_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/mdfe_modal_aereo_v3_00.py` & `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/mdfe_modal_aereo_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/cons_reci_mdfe_v3_00.py` & `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/cons_reci_mdfe_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/proc_mdfe_v3_00.py` & `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/proc_mdfe_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/bindings/v3_0/cons_stat_serv_mdfe_v3_00.py` & `nfelib-2.0.5/nfelib/mdfe/bindings/v3_0/cons_stat_serv_mdfe_v3_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/consReciMDFeTiposBasico_v3.00.xsd` & `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/consReciMDFeTiposBasico_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/retConsReciMDFe_v3.00.xsd` & `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retConsReciMDFe_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/retConsMDFeNaoEnc_v3.00.xsd` & `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retConsMDFeNaoEnc_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/consStatServMDFe_v3.00.xsd` & `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/consStatServMDFe_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/evIncCondutorMDFe_v3.00.xsd` & `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/evIncCondutorMDFe_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/consStatServTiposBasico_v3.00.xsd` & `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/consStatServTiposBasico_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/retMDFe_v3.00.xsd` & `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retMDFe_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/mdfeModalRodoviario_v3.00.xsd` & `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/mdfeModalRodoviario_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/evCancMDFe_v3.00.xsd` & `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/evCancMDFe_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/distMDFe_v3.00.xsd` & `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/distMDFe_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/retMDFeConsultaDFe_v3.00.xsd` & `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retMDFeConsultaDFe_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/mdfeModalAereo_v3.00.xsd` & `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/mdfeModalAereo_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/mdfeModalFerroviario_v3.00.xsd` & `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/mdfeModalFerroviario_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/eventoMDFe_v3.00.xsd` & `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/eventoMDFe_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/retConsStatServMDFe_v3.00.xsd` & `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retConsStatServMDFe_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/evPagtoOperMDFe_v3.00.xsd` & `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/evPagtoOperMDFe_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/retEventoMDFe_v3.00.xsd` & `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retEventoMDFe_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/consReciMDFe_v3.00.xsd` & `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/consReciMDFe_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/mdfeConsultaDFe_v3.00.xsd` & `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/mdfeConsultaDFe_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/consMDFeNaoEnc_v3.00.xsd` & `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/consMDFeNaoEnc_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/procMDFe_v3.00.xsd` & `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/procMDFe_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/enviMDFe_v3.00.xsd` & `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/enviMDFe_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/evInclusaoDFeMDFe_v3.00.xsd` & `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/evInclusaoDFeMDFe_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/tiposGeralMDFe_v3.00.xsd` & `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/tiposGeralMDFe_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/mdfeConsultaDFeTiposBasico_v3.00.xsd` & `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/mdfeConsultaDFeTiposBasico_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/mdfeTiposBasico_v3.00.xsd` & `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/mdfeTiposBasico_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/mdfeModalAquaviario_v3.00.xsd` & `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/mdfeModalAquaviario_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/mdfe_v3.00.xsd` & `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/mdfe_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/retEnviMDFe_v3.00.xsd` & `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retEnviMDFe_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/consSitMDFe_v3.00.xsd` & `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/consSitMDFe_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/consSitMDFeTiposBasico_v3.00.xsd` & `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/consSitMDFeTiposBasico_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/retConsMDFeNaoEnc_v1.00.xsd` & `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retConsMDFeNaoEnc_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/leiauteDistMDFe_v3.00.xsd` & `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/leiauteDistMDFe_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/consMDFeNaoEncTiposBasico_v3.00.xsd` & `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/consMDFeNaoEncTiposBasico_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/xmldsig-core-schema_v1.01.xsd` & `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/xmldsig-core-schema_v1.01.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/eventoMDFeTiposBasico_v3.00.xsd` & `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/eventoMDFeTiposBasico_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/procEventoMDFe_v3.00.xsd` & `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/procEventoMDFe_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/retDistMDFe_v3.00.xsd` & `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retDistMDFe_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/retConsSitMDFe_v3.00.xsd` & `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/retConsSitMDFe_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe/schemas/v3_0/evEncMDFe_v3.00.xsd` & `nfelib-2.0.5/nfelib/mdfe/schemas/v3_0/evEncMDFe_v3.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_mde/bindings/v1_0/proc_conf_recebto_nfe_v1_00.py` & `nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/proc_conf_recebto_nfe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_mde/bindings/v1_0/xmldsig_core_schema_v1_01.py` & `nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/xmldsig_core_schema_v1_01.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_mde/bindings/v1_0/__init__.py` & `nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/__init__.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_mde/bindings/v1_0/e210240_v1_00.py` & `nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/e210240_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_mde/bindings/v1_0/leiaute_conf_recebto_v1_00.py` & `nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/leiaute_conf_recebto_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_mde/bindings/v1_0/conf_recebto_v1_00.py` & `nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/conf_recebto_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_mde/bindings/v1_0/ret_env_conf_recebto_v1_00.py` & `nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/ret_env_conf_recebto_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_mde/bindings/v1_0/env_conf_recebto_v1_00.py` & `nfelib-2.0.5/nfelib/nfe_evento_mde/bindings/v1_0/env_conf_recebto_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_mde/schemas/v1_0/leiauteConfRecebto_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/leiauteConfRecebto_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_mde/schemas/v1_0/procConfRecebtoNFe_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/procConfRecebtoNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_mde/schemas/v1_0/e210220_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/e210220_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_mde/schemas/v1_0/e210200_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/e210200_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_mde/schemas/v1_0/e210240_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/e210240_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_mde/schemas/v1_0/envConfRecebto_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/envConfRecebto_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_mde/schemas/v1_0/e210210_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/e210210_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_mde/schemas/v1_0/confRecebto_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/confRecebto_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_mde/schemas/v1_0/tiposBasico_v1.03.xsd` & `nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/tiposBasico_v1.03.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_mde/schemas/v1_0/retEnvConfRecebto_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/retEnvConfRecebto_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_mde/schemas/v1_0/xmldsig-core-schema_v1.01.xsd` & `nfelib-2.0.5/nfelib/nfe_evento_mde/schemas/v1_0/xmldsig-core-schema_v1.01.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_epec/bindings/v1_0/__init__.py` & `nfelib-2.0.5/nfelib/nfe_epec/bindings/v1_0/__init__.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_epec/bindings/v1_0/e110140_v1_00.py` & `nfelib-2.0.5/nfelib/nfe_epec/bindings/v1_0/e110140_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_epec/bindings/v1_0/leiaute_epec_v1_00.py` & `nfelib-2.0.5/nfelib/nfe_epec/bindings/v1_0/leiaute_epec_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_epec/schemas/v1_0/EPEC_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfe_epec/schemas/v1_0/EPEC_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_epec/schemas/v1_0/e110140_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfe_epec/schemas/v1_0/e110140_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_epec/schemas/v1_0/envEPEC_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfe_epec/schemas/v1_0/envEPEC_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_epec/schemas/v1_0/procEPEC_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfe_epec/schemas/v1_0/procEPEC_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_epec/schemas/v1_0/leiauteEPEC_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfe_epec/schemas/v1_0/leiauteEPEC_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_epec/schemas/v1_0/tiposBasico_v1.03.xsd` & `nfelib-2.0.5/nfelib/nfe_epec/schemas/v1_0/tiposBasico_v1.03.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_epec/schemas/v1_0/xmldsig-core-schema_v1.01.xsd` & `nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/xmldsig-core-schema_v1.01.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_epec/schemas/v1_0/retEnvEPEC_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfe_epec/schemas/v1_0/retEnvEPEC_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_entrega/bindings/v1_0/xmldsig_core_schema_v1_01.py` & `nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/xmldsig_core_schema_v1_01.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_entrega/bindings/v1_0/tipos_basico_v1_03.py` & `nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/tipos_basico_v1_03.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_entrega/bindings/v1_0/__init__.py` & `nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/__init__.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_entrega/bindings/v1_0/evento_entrega_nfe_v1_00.py` & `nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/evento_entrega_nfe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_entrega/bindings/v1_0/proc_evento_entrega_nfe_v1_00.py` & `nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/proc_evento_entrega_nfe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_entrega/bindings/v1_0/ret_evento_entrega_nfe_v1_00.py` & `nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/ret_evento_entrega_nfe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_entrega/bindings/v1_0/leiaute_evento_entrega_nfe_v1_00.py` & `nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/leiaute_evento_entrega_nfe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_entrega/bindings/v1_0/env_evento_entrega_nfe_v1_00.py` & `nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/env_evento_entrega_nfe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_entrega/bindings/v1_0/e110130_v1_00.py` & `nfelib-2.0.5/nfelib/nfe_entrega/bindings/v1_0/e110130_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_entrega/schemas/v1_0/envEventoCancEntregaNFe_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/envEventoCancEntregaNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_entrega/schemas/v1_0/procEventoEntregaNFe_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/procEventoEntregaNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_entrega/schemas/v1_0/EventoCancEntregaNFe_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/EventoCancEntregaNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_entrega/schemas/v1_0/retEventoCancEntregaNFe_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/retEventoCancEntregaNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_entrega/schemas/v1_0/EventoEntregaNFe_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/EventoEntregaNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_entrega/schemas/v1_0/e110130_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/e110130_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_entrega/schemas/v1_0/leiauteEventoCancEntregaNFe_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/leiauteEventoCancEntregaNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_entrega/schemas/v1_0/leiauteEventoEntregaNFe_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/leiauteEventoEntregaNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_entrega/schemas/v1_0/envEventoEntregaNFe_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/envEventoEntregaNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_entrega/schemas/v1_0/tiposBasico_v1.03.xsd` & `nfelib-2.0.5/nfelib/nfe_insucesso/schemas/v1_0/tiposBasico_v1.03.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_entrega/schemas/v1_0/retEventoEntregaNFe_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/retEventoEntregaNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_entrega/schemas/v1_0/xmldsig-core-schema_v1.01.xsd` & `nfelib-2.0.5/nfelib/nfe_epec/schemas/v1_0/xmldsig-core-schema_v1.01.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_entrega/schemas/v1_0/e110131_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/e110131_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_entrega/schemas/v1_0/procEventoCancEntregaNFe_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/procEventoCancEntregaNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_dist_dfe/bindings/v1_0/res_evento_v1_01.py` & `nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/v1_0/res_evento_v1_01.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_dist_dfe/bindings/v1_0/xmldsig_core_schema_v1_01.py` & `nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/v1_0/xmldsig_core_schema_v1_01.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_dist_dfe/bindings/v1_0/__init__.py` & `nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/v1_0/__init__.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_dist_dfe/bindings/v1_0/ret_dist_dfe_int_v1_01.py` & `nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/v1_0/ret_dist_dfe_int_v1_01.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_dist_dfe/bindings/v1_0/res_nfe_v1_01.py` & `nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/v1_0/res_nfe_v1_01.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_dist_dfe/bindings/v1_0/dist_dfe_int_v1_01.py` & `nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/v1_0/dist_dfe_int_v1_01.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_dist_dfe/bindings/v1_0/tipos_dist_dfe_v1_01.py` & `nfelib-2.0.5/nfelib/nfe_dist_dfe/bindings/v1_0/tipos_dist_dfe_v1_01.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_dist_dfe/schemas/v1_0/retDistDFeInt_v1.01.xsd` & `nfelib-2.0.5/nfelib/nfe_dist_dfe/schemas/v1_0/retDistDFeInt_v1.01.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_dist_dfe/schemas/v1_0/tiposDistDFe_v1.01.xsd` & `nfelib-2.0.5/nfelib/nfe_dist_dfe/schemas/v1_0/tiposDistDFe_v1.01.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_dist_dfe/schemas/v1_0/distDFeInt_v1.01.xsd` & `nfelib-2.0.5/nfelib/nfe_dist_dfe/schemas/v1_0/distDFeInt_v1.01.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_dist_dfe/schemas/v1_0/resEvento_v1.01.xsd` & `nfelib-2.0.5/nfelib/nfe_dist_dfe/schemas/v1_0/resEvento_v1.01.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_dist_dfe/schemas/v1_0/resNFe_v1.01.xsd` & `nfelib-2.0.5/nfelib/nfe_dist_dfe/schemas/v1_0/resNFe_v1.01.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_dist_dfe/schemas/v1_0/xmldsig-core-schema_v1.01.xsd` & `nfelib-2.0.5/nfelib/nfe_dist_dfe/schemas/v1_0/xmldsig-core-schema_v1.01.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_cancel/bindings/v1_0/e110111_v1_00.py` & `nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/e110111_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_cancel/bindings/v1_0/ret_env_evento_canc_nfe_v1_00.py` & `nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/ret_env_evento_canc_nfe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_cancel/bindings/v1_0/xmldsig_core_schema_v1_01.py` & `nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/xmldsig_core_schema_v1_01.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_cancel/bindings/v1_0/tipos_basico_v1_03.py` & `nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/tipos_basico_v1_03.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_cancel/bindings/v1_0/__init__.py` & `nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/__init__.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_cancel/bindings/v1_0/env_evento_canc_nfe_v1_00.py` & `nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/env_evento_canc_nfe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_cancel/bindings/v1_0/proc_evento_canc_nfe_v1_00.py` & `nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/proc_evento_canc_nfe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_cancel/bindings/v1_0/leiaute_evento_canc_nfe_v1_00.py` & `nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/leiaute_evento_canc_nfe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_cancel/bindings/v1_0/evento_canc_nfe_v1_00.py` & `nfelib-2.0.5/nfelib/nfe_evento_cancel/bindings/v1_0/evento_canc_nfe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_cancel/schemas/v1_0/envEventoCancNFe_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/v1_0/envEventoCancNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_cancel/schemas/v1_0/eventoCancNFe_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/v1_0/eventoCancNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_cancel/schemas/v1_0/leiauteEventoCancNFe_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/v1_0/leiauteEventoCancNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_cancel/schemas/v1_0/e110111_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/v1_0/e110111_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_cancel/schemas/v1_0/procEventoCancNFe_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/v1_0/procEventoCancNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_cancel/schemas/v1_0/retEnvEventoCancNFe_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/v1_0/retEnvEventoCancNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_cancel/schemas/v1_0/tiposBasico_v1.03.xsd` & `nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/v1_0/tiposBasico_v1.03.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_cancel/schemas/v1_0/xmldsig-core-schema_v1.01.xsd` & `nfelib-2.0.5/nfelib/nfe_entrega/schemas/v1_0/xmldsig-core-schema_v1.01.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte_dist_dfe/bindings/v1_0/dist_dfe_int_v1_00.py` & `nfelib-2.0.5/nfelib/cte_dist_dfe/bindings/v1_0/dist_dfe_int_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte_dist_dfe/bindings/v1_0/xmldsig_core_schema_v1_01.py` & `nfelib-2.0.5/nfelib/cte_dist_dfe/bindings/v1_0/xmldsig_core_schema_v1_01.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte_dist_dfe/bindings/v1_0/__init__.py` & `nfelib-2.0.5/nfelib/cte_dist_dfe/bindings/v1_0/__init__.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte_dist_dfe/bindings/v1_0/tipos_dist_dfe_v1_00.py` & `nfelib-2.0.5/nfelib/cte_dist_dfe/bindings/v1_0/tipos_dist_dfe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte_dist_dfe/bindings/v1_0/ret_dist_dfe_int_v1_00.py` & `nfelib-2.0.5/nfelib/cte_dist_dfe/bindings/v1_0/ret_dist_dfe_int_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte_dist_dfe/schemas/v1_0/distDFeInt_v1.00.xsd` & `nfelib-2.0.5/nfelib/cte_dist_dfe/schemas/v1_0/distDFeInt_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte_dist_dfe/schemas/v1_0/retDistDFeInt_v1.00.xsd` & `nfelib-2.0.5/nfelib/cte_dist_dfe/schemas/v1_0/retDistDFeInt_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte_dist_dfe/schemas/v1_0/xmldsig-core-schema_v1.01.xsd` & `nfelib-2.0.5/nfelib/cte_dist_dfe/schemas/v1_0/xmldsig-core-schema_v1.01.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte_dist_dfe/schemas/v1_0/tiposDistDFe_v1.00.xsd` & `nfelib-2.0.5/nfelib/cte_dist_dfe/schemas/v1_0/tiposDistDFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/bpe/bindings/v1_0/cons_sit_bpe_tipos_basico_v1_00.py` & `nfelib-2.0.5/nfelib/bpe/bindings/v1_0/cons_sit_bpe_tipos_basico_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/bpe/bindings/v1_0/xmldsig_core_schema_v1_01.py` & `nfelib-2.0.5/nfelib/bpe/bindings/v1_0/xmldsig_core_schema_v1_01.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/bpe/bindings/v1_0/__init__.py` & `nfelib-2.0.5/nfelib/bpe/bindings/v1_0/__init__.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/bpe/bindings/v1_0/cons_stat_serv_bpe_tipos_basico_v1_00.py` & `nfelib-2.0.5/nfelib/bpe/bindings/v1_0/cons_stat_serv_bpe_tipos_basico_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/bpe/bindings/v1_0/ev_nao_emb_bpe_v1_00.py` & `nfelib-2.0.5/nfelib/bpe/bindings/v1_0/ev_nao_emb_bpe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/bpe/bindings/v1_0/ev_alteracao_poltrona_v1_00.py` & `nfelib-2.0.5/nfelib/bpe/bindings/v1_0/ev_alteracao_poltrona_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/bpe/bindings/v1_0/evento_bpe_v1_00.py` & `nfelib-2.0.5/nfelib/bpe/bindings/v1_0/evento_bpe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/bpe/bindings/v1_0/tipos_geral_bpe_v1_00.py` & `nfelib-2.0.5/nfelib/bpe/bindings/v1_0/tipos_geral_bpe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/bpe/bindings/v1_0/proc_evento_bpe_v1_00.py` & `nfelib-2.0.5/nfelib/bpe/bindings/v1_0/proc_evento_bpe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/bpe/bindings/v1_0/ret_evento_bpe_v1_00.py` & `nfelib-2.0.5/nfelib/bpe/bindings/v1_0/ret_evento_bpe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/bpe/bindings/v1_0/cons_stat_serv_bpe_v1_00.py` & `nfelib-2.0.5/nfelib/bpe/bindings/v1_0/cons_stat_serv_bpe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/bpe/bindings/v1_0/ret_cons_sit_bpe_v1_00.py` & `nfelib-2.0.5/nfelib/bpe/bindings/v1_0/ret_cons_sit_bpe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/bpe/bindings/v1_0/cons_sit_bpe_v1_00.py` & `nfelib-2.0.5/nfelib/bpe/bindings/v1_0/cons_sit_bpe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/bpe/bindings/v1_0/proc_bpe_tm_v1_00.py` & `nfelib-2.0.5/nfelib/bpe/bindings/v1_0/proc_bpe_tm_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/bpe/bindings/v1_0/evento_bpe_tipos_basico_v1_00.py` & `nfelib-2.0.5/nfelib/bpe/bindings/v1_0/evento_bpe_tipos_basico_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/bpe/bindings/v1_0/ev_excesso_bagagem_v1_00.py` & `nfelib-2.0.5/nfelib/bpe/bindings/v1_0/ev_excesso_bagagem_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/bpe/bindings/v1_0/ret_cons_stat_serv_bpe_v1_00.py` & `nfelib-2.0.5/nfelib/bpe/bindings/v1_0/ret_cons_stat_serv_bpe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/bpe/bindings/v1_0/ev_canc_bpe_v1_00.py` & `nfelib-2.0.5/nfelib/bpe/bindings/v1_0/ev_canc_bpe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/bpe/bindings/v1_0/proc_bpe_v1_00.py` & `nfelib-2.0.5/nfelib/bpe/bindings/v1_0/proc_bpe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/bpe/bindings/v1_0/bpe_tipos_basico_v1_00.py` & `nfelib-2.0.5/nfelib/bpe/bindings/v1_0/bpe_tipos_basico_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/bpe/schemas/v1_0/eventoBPe_v1.00.xsd` & `nfelib-2.0.5/nfelib/bpe/schemas/v1_0/eventoBPe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/bpe/schemas/v1_0/consStatServBPe_v1.00.xsd` & `nfelib-2.0.5/nfelib/bpe/schemas/v1_0/consStatServBPe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/bpe/schemas/v1_0/bpeTiposBasico_v1.00.xsd` & `nfelib-2.0.5/nfelib/bpe/schemas/v1_0/bpeTiposBasico_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/bpe/schemas/v1_0/retEventoBPe_v1.00.xsd` & `nfelib-2.0.5/nfelib/bpe/schemas/v1_0/retEventoBPe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/bpe/schemas/v1_0/tiposGeralBPe_v1.00.xsd` & `nfelib-2.0.5/nfelib/bpe/schemas/v1_0/tiposGeralBPe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/bpe/schemas/v1_0/evCancBPe_v1.00.xsd` & `nfelib-2.0.5/nfelib/bpe/schemas/v1_0/evCancBPe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/bpe/schemas/v1_0/evNaoEmbBPe_v1.00.xsd` & `nfelib-2.0.5/nfelib/bpe/schemas/v1_0/evNaoEmbBPe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/bpe/schemas/v1_0/retConsSitBPe_v1.00.xsd` & `nfelib-2.0.5/nfelib/bpe/schemas/v1_0/retConsSitBPe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/bpe/schemas/v1_0/bpe_v1.00.xsd` & `nfelib-2.0.5/nfelib/bpe/schemas/v1_0/bpe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/bpe/schemas/v1_0/evExcessoBagagem_v1.00.xsd` & `nfelib-2.0.5/nfelib/bpe/schemas/v1_0/evExcessoBagagem_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/bpe/schemas/v1_0/retBPe_v1.00.xsd` & `nfelib-2.0.5/nfelib/bpe/schemas/v1_0/retBPe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/bpe/schemas/v1_0/eventoBPeTiposBasico_v1.00.xsd` & `nfelib-2.0.5/nfelib/bpe/schemas/v1_0/eventoBPeTiposBasico_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/bpe/schemas/v1_0/procBPe_v1.00.xsd` & `nfelib-2.0.5/nfelib/bpe/schemas/v1_0/procBPe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/bpe/schemas/v1_0/procBPeTM_v1.00.xsd` & `nfelib-2.0.5/nfelib/bpe/schemas/v1_0/procBPeTM_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/bpe/schemas/v1_0/retConsStatServBPe_v1.00.xsd` & `nfelib-2.0.5/nfelib/bpe/schemas/v1_0/retConsStatServBPe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/bpe/schemas/v1_0/evAlteracaoPoltrona_v1.00.xsd` & `nfelib-2.0.5/nfelib/bpe/schemas/v1_0/evAlteracaoPoltrona_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/bpe/schemas/v1_0/consSitBPeTiposBasico_v1.00.xsd` & `nfelib-2.0.5/nfelib/bpe/schemas/v1_0/consSitBPeTiposBasico_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/bpe/schemas/v1_0/bpeTM_v1.00.xsd` & `nfelib-2.0.5/nfelib/bpe/schemas/v1_0/bpeTM_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/bpe/schemas/v1_0/xmldsig-core-schema_v1.01.xsd` & `nfelib-2.0.5/nfelib/nfe_evento_cancel/schemas/v1_0/xmldsig-core-schema_v1.01.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/bpe/schemas/v1_0/procEventoBPe_v1.00.xsd` & `nfelib-2.0.5/nfelib/bpe/schemas/v1_0/procEventoBPe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/bpe/schemas/v1_0/consSitBPe_v1.00.xsd` & `nfelib-2.0.5/nfelib/bpe/schemas/v1_0/consSitBPe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/bpe/schemas/v1_0/consStatServBPeTiposBasico_v1.00.xsd` & `nfelib-2.0.5/nfelib/bpe/schemas/v1_0/consStatServBPeTiposBasico_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe_dist_dfe/bindings/v1_0/dist_dfe_int_v1_00.py` & `nfelib-2.0.5/nfelib/mdfe_dist_dfe/bindings/v1_0/dist_dfe_int_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe_dist_dfe/bindings/v1_0/xmldsig_core_schema_v1_01.py` & `nfelib-2.0.5/nfelib/mdfe_dist_dfe/bindings/v1_0/xmldsig_core_schema_v1_01.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe_dist_dfe/bindings/v1_0/__init__.py` & `nfelib-2.0.5/nfelib/mdfe_dist_dfe/bindings/v1_0/__init__.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe_dist_dfe/bindings/v1_0/ret_dist_dfe_int_v1_00.py` & `nfelib-2.0.5/nfelib/mdfe_dist_dfe/bindings/v1_0/ret_dist_dfe_int_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe_dist_dfe/schemas/v1_0/tiposGeralMDFe_v1.00.xsd` & `nfelib-2.0.5/nfelib/mdfe_dist_dfe/schemas/v1_0/tiposGeralMDFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe_dist_dfe/schemas/v1_0/distDFeInt_v1.00.xsd` & `nfelib-2.0.5/nfelib/mdfe_dist_dfe/schemas/v1_0/distDFeInt_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe_dist_dfe/schemas/v1_0/retDistDFeInt_v1.00.xsd` & `nfelib-2.0.5/nfelib/mdfe_dist_dfe/schemas/v1_0/retDistDFeInt_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe_dist_dfe/schemas/v1_0/xmldsig-core-schema_v1.01.xsd` & `nfelib-2.0.5/nfelib/mdfe_dist_dfe/schemas/v1_0/xmldsig-core-schema_v1.01.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/mdfe_dist_dfe/schemas/v1_0/tiposDistDFe_v1.00.xsd` & `nfelib-2.0.5/nfelib/mdfe_dist_dfe/schemas/v1_0/tiposDistDFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_cce/samples/v1_0/35180803102452000172550010000476051695511860-01-cce.xml` & `nfelib-2.0.5/nfelib/nfe_evento_cce/samples/v1_0/35180803102452000172550010000476051695511860-01-cce.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_cce/bindings/v1_0/cce_v1_00.py` & `nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/cce_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_cce/bindings/v1_0/xmldsig_core_schema_v1_01.py` & `nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/xmldsig_core_schema_v1_01.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_cce/bindings/v1_0/__init__.py` & `nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/__init__.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_cce/bindings/v1_0/proc_cce_nfe_v1_00.py` & `nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/proc_cce_nfe_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_cce/bindings/v1_0/leiaute_cce_v1_00.py` & `nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/leiaute_cce_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_cce/bindings/v1_0/e110110_v1_00.py` & `nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/e110110_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_cce/bindings/v1_0/ret_env_cce_v1_00.py` & `nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/ret_env_cce_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_cce/bindings/v1_0/env_cce_v1_00.py` & `nfelib-2.0.5/nfelib/nfe_evento_cce/bindings/v1_0/env_cce_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_cce/schemas/v1_0/leiauteCCe_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/v1_0/leiauteCCe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_cce/schemas/v1_0/CCe_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/v1_0/CCe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_cce/schemas/v1_0/procCCeNFe_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/v1_0/procCCeNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_cce/schemas/v1_0/e110110_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/v1_0/e110110_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_cce/schemas/v1_0/envCCe_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/v1_0/envCCe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_cce/schemas/v1_0/tiposBasico_v1.03.xsd` & `nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/v1_0/tiposBasico_v1.03.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_cce/schemas/v1_0/xmldsig-core-schema_v1.01.xsd` & `nfelib-2.0.5/nfelib/bpe/schemas/v1_0/xmldsig-core-schema_v1.01.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_cce/schemas/v1_0/retEnvCCe_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/v1_0/retEnvCCe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_ator_interessado/bindings/v1_0/xmldsig_core_schema_v1_01.py` & `nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/xmldsig_core_schema_v1_01.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_ator_interessado/bindings/v1_0/tipos_basico_v1_03.py` & `nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/tipos_basico_v1_03.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_ator_interessado/bindings/v1_0/__init__.py` & `nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/__init__.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_ator_interessado/bindings/v1_0/ret_env_evento_ator_interessado_v1_00.py` & `nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/ret_env_evento_ator_interessado_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_ator_interessado/bindings/v1_0/proc_evento_ator_interessado_v1_00.py` & `nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/proc_evento_ator_interessado_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_ator_interessado/bindings/v1_0/mod_110150_v1_00.py` & `nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/mod_110150_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_ator_interessado/bindings/v1_0/evento_ator_interessado_v1_00.py` & `nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/evento_ator_interessado_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_ator_interessado/bindings/v1_0/leiaute_evento_ator_interessado_v1_00.py` & `nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/leiaute_evento_ator_interessado_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_ator_interessado/bindings/v1_0/env_evento_ator_interessado_v1_00.py` & `nfelib-2.0.5/nfelib/nfe_ator_interessado/bindings/v1_0/env_evento_ator_interessado_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_ator_interessado/schemas/v1_0/retEnvEventoAtorInteressado_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/v1_0/retEnvEventoAtorInteressado_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_ator_interessado/schemas/v1_0/procEventoAtorInteressado_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/v1_0/procEventoAtorInteressado_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_ator_interessado/schemas/v1_0/110150_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/v1_0/110150_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_ator_interessado/schemas/v1_0/leiauteEventoAtorInteressado_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/v1_0/leiauteEventoAtorInteressado_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_ator_interessado/schemas/v1_0/envEventoAtorInteressado_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/v1_0/envEventoAtorInteressado_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_ator_interessado/schemas/v1_0/eventoAtorInteressado_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/v1_0/eventoAtorInteressado_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_ator_interessado/schemas/v1_0/tiposBasico_v1.03.xsd` & `nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/v1_0/tiposBasico_v1.03.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_ator_interessado/schemas/v1_0/xmldsig-core-schema_v1.01.xsd` & `nfelib-2.0.5/nfelib/nfe_evento_cce/schemas/v1_0/xmldsig-core-schema_v1.01.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte/samples/v4_0/51160624686092000173570010000000031000000020-cte.XML` & `nfelib-2.0.5/nfelib/cte/samples/v4_0/51160624686092000173570010000000031000000020-cte.XML`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte/samples/v4_0/cce35150107565416000104570000000012301000012300-ped-eve.xml` & `nfelib-2.0.5/nfelib/cte/samples/v4_0/cce35150107565416000104570000000012301000012300-ped-eve.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte/samples/v4_0/35190602427026001207570040000522031000522035-cte-multimodal.xml` & `nfelib-2.0.5/nfelib/cte/samples/v4_0/35190602427026001207570040000522031000522035-cte-multimodal.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte/samples/v4_0/35170799999999999999670000000000261309301440-cte-of.xml` & `nfelib-2.0.5/nfelib/cte/samples/v4_0/35170799999999999999670000000000261309301440-cte-of.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte/samples/v4_0/43120178408960000182570010000000041000000047-cte.xml` & `nfelib-2.0.5/nfelib/cte/samples/v4_0/43120178408960000182570010000000041000000047-cte.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte/bindings/v4_0/ev_reg_multimodal_v4_00.py` & `nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_reg_multimodal_v4_00.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:16:35
+"""This file was generated by xsdata, v24.4, on 2024-04-08 21:52:20
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass, field
 from enum import Enum
-from nfelib import CommonMixin
 from typing import Optional
 
+from nfelib import CommonMixin
+
 __NAMESPACE__ = "http://www.portalfiscal.inf.br/cte"
 
 
 class EvRegMultimodalDescEvento(Enum):
     REGISTRO_MULTIMODAL = "Registro Multimodal"
```

## Comparing `nfelib-2.0.4/nfelib/cte/bindings/v4_0/ret_cons_stat_serv_cte_v4_00.py` & `nfelib-2.0.5/nfelib/cte/bindings/v4_0/ret_cons_stat_serv_cte_v4_00.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:16:35
+"""This file was generated by xsdata, v24.4, on 2024-04-08 21:52:20
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass
+
 from nfelib.cte.bindings.v4_0.cons_stat_serv_tipos_basico_v4_00 import (
     TretConsStatServ,
 )
 
 __NAMESPACE__ = "http://www.portalfiscal.inf.br/cte"
```

## Comparing `nfelib-2.0.4/nfelib/cte/bindings/v4_0/cte_multi_modal_v4_00.py` & `nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_multi_modal_v4_00.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:16:35
+"""This file was generated by xsdata, v24.4, on 2024-04-08 21:52:20
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass, field
 from enum import Enum
-from nfelib import CommonMixin
 from typing import Optional
 
+from nfelib import CommonMixin
+
 __NAMESPACE__ = "http://www.portalfiscal.inf.br/cte"
 
 
 class MultimodalIndNegociavel(Enum):
     VALUE_0 = "0"
     VALUE_1 = "1"
```

## Comparing `nfelib-2.0.4/nfelib/cte/bindings/v4_0/ev_epeccte_v4_00.py` & `nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_epeccte_v4_00.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:16:35
+"""This file was generated by xsdata, v24.4, on 2024-04-08 21:52:20
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass, field
 from enum import Enum
-from nfelib import CommonMixin
 from typing import Optional
+
+from nfelib import CommonMixin
 from nfelib.cte.bindings.v4_0.cte_tipos_basico_v4_00 import Toma4Toma
 from nfelib.cte.bindings.v4_0.evento_cte_tipos_basico_v4_00 import TmodTransp
 from nfelib.cte.bindings.v4_0.tipos_geral_cte_v4_00 import Tuf
 
 __NAMESPACE__ = "http://www.portalfiscal.inf.br/cte"
```

## Comparing `nfelib-2.0.4/nfelib/cte/bindings/v4_0/xmldsig_core_schema_v1_01.py` & `nfelib-2.0.5/nfelib/nfe_evento_generico/bindings/v1_0/xmldsig_core_schema_v1_01.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:16:35
+"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:16:22
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass, field
 from enum import Enum
 from nfelib import CommonMixin
```

## Comparing `nfelib-2.0.4/nfelib/cte/bindings/v4_0/cons_stat_serv_tipos_basico_v4_00.py` & `nfelib-2.0.5/nfelib/cte/bindings/v4_0/cons_stat_serv_tipos_basico_v4_00.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:16:35
+"""This file was generated by xsdata, v24.4, on 2024-04-08 21:52:20
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass, field
-from nfelib import CommonMixin
 from typing import Optional
+
+from nfelib import CommonMixin
 from nfelib.cte.bindings.v4_0.tipos_geral_cte_v4_00 import (
     Tamb,
     TcodUfIbge,
 )
 
 __NAMESPACE__ = "http://www.portalfiscal.inf.br/cte"
```

## Comparing `nfelib-2.0.4/nfelib/cte/bindings/v4_0/__init__.py` & `nfelib-2.0.5/nfelib/cte/bindings/v4_0/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:16:35
+"""This file was generated by xsdata, v24.4, on 2024-04-08 21:52:20
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from nfelib.cte.bindings.v4_0.cons_sit_cte_tipos_basico_v4_00 import (
-    TconsSitCte,
-    TretConsSitCte,
     ProcEventoCteVersao,
     ProtCteVersao,
+    TconsSitCte,
+    TretConsSitCte,
 )
 from nfelib.cte.bindings.v4_0.cons_sit_cte_v4_00 import ConsSitCte
 from nfelib.cte.bindings.v4_0.cons_stat_serv_cte_v4_00 import ConsStatServCte
 from nfelib.cte.bindings.v4_0.cons_stat_serv_tipos_basico_v4_00 import (
     TconsStatServ,
     TretConsStatServ,
 )
@@ -23,90 +23,98 @@
 from nfelib.cte.bindings.v4_0.cte_modal_aquaviario_v4_00 import (
     Aquav,
     AquavDirec,
     AquavTpNav,
 )
 from nfelib.cte.bindings.v4_0.cte_modal_dutoviario_v4_00 import Duto
 from nfelib.cte.bindings.v4_0.cte_modal_ferroviario_v4_00 import (
-    TenderFer,
     Ferrov,
     FerrovTpTraf,
+    TenderFer,
     TrafMutFerrEmi,
     TrafMutRespFat,
 )
 from nfelib.cte.bindings.v4_0.cte_modal_rodoviario_os_v4_00 import (
     InfFretamentoTpFretamento,
     PropTpProp,
     RodoOs,
 )
 from nfelib.cte.bindings.v4_0.cte_modal_rodoviario_v4_00 import Rodo
 from nfelib.cte.bindings.v4_0.cte_multi_modal_v4_00 import (
     Multimodal,
     MultimodalIndNegociavel,
 )
 from nfelib.cte.bindings.v4_0.cte_os_v4_00 import CteOs
+from nfelib.cte.bindings.v4_0.cte_simp_v4_00 import CteSimp
 from nfelib.cte.bindings.v4_0.cte_tipos_basico_v4_00 import (
+    ComDataTpPer,
+    ComHoraTpHor,
     CompTpComp,
     Icms00Cst,
     Icms20Cst,
     Icms45Cst,
     Icms60Cst,
     Icms90Cst,
     IcmsoutraUfCst,
     IcmssnCst,
     IcmssnIndSn,
+    IdeIndGlobalizado,
+    IdeIndIetoma,
+    IdeModal,
+    IdeRetira,
+    IdeTpEmis,
+    IdeTpImp,
+    IdeTpServ,
+    InfCteSubIndAlteraToma,
+    InfDocAntTpPrest,
+    InfEspecieTpEspecie,
+    InfEspecieTpNumerario,
+    InfOutrosTpDoc,
+    InfQCUnid,
+    InfQTpMed,
+    NoInterTpHor,
+    NoPeriodoTpPer,
+    SegRespSeg,
+    SemDataTpPer,
+    SemHoraTpHor,
     Tcrt,
     Tcte,
     TcteOs,
+    TcteSimp,
     TdocAssoc,
-    TendOrg,
-    TendReEnt,
     TendeEmi,
     Tendereco,
     Tendernac,
+    TendOrg,
+    TendReEnt,
     TfinCte,
+    TfinCteSimp,
     TfinGtve,
     Tgtve,
     Timp,
     TimpOs,
     Tlocal,
     TmodTranspOs,
+    TmodTranspSimp,
+    Toma3Toma,
+    Toma4Toma,
+    TomaIndIetoma,
+    TomaTerceiroToma,
+    TomaToma,
     TprocEmi,
     TprotCte,
     TprotCteOs,
     TprotGtve,
     TrespTec,
     TretCte,
     TretCteOs,
+    TretCteSimp,
     TretGtve,
-    TunidCarga,
     TunidadeTransp,
-    ComDataTpPer,
-    ComHoraTpHor,
-    IdeIndGlobalizado,
-    IdeIndIetoma,
-    IdeModal,
-    IdeRetira,
-    IdeTpEmis,
-    IdeTpImp,
-    IdeTpServ,
-    InfCteSubIndAlteraToma,
-    InfEspecieTpEspecie,
-    InfEspecieTpNumerario,
-    InfOutrosTpDoc,
-    InfQCUnid,
-    NoInterTpHor,
-    NoPeriodoTpPer,
-    SegRespSeg,
-    SemDataTpPer,
-    SemHoraTpHor,
-    Toma3Toma,
-    Toma4Toma,
-    TomaTerceiroToma,
-    TomaToma,
+    TunidCarga,
 )
 from nfelib.cte.bindings.v4_0.cte_v4_00 import Cte
 from nfelib.cte.bindings.v4_0.ev_canc_cecte_v4_00 import (
     EvCancCecte,
     EvCancCecteDescEvento,
 )
 from nfelib.cte.bindings.v4_0.ev_canc_cte_v4_00 import (
@@ -173,43 +181,44 @@
 from nfelib.cte.bindings.v4_0.proc_gtve_v4_00 import GtveProc
 from nfelib.cte.bindings.v4_0.proc_inut_cte_v4_00 import ProcInutCte
 from nfelib.cte.bindings.v4_0.ret_cons_sit_cte_v4_00 import RetConsSitCte
 from nfelib.cte.bindings.v4_0.ret_cons_stat_serv_cte_v4_00 import (
     RetConsStatServCte,
 )
 from nfelib.cte.bindings.v4_0.ret_cte_os_v4_00 import RetCteOs
+from nfelib.cte.bindings.v4_0.ret_cte_simp_v4_00 import RetCteSimp
 from nfelib.cte.bindings.v4_0.ret_cte_v4_00 import RetCte
 from nfelib.cte.bindings.v4_0.ret_evento_cte_v4_00 import RetEventoCte
 from nfelib.cte.bindings.v4_0.ret_gtve_v4_00 import RetGtve
 from nfelib.cte.bindings.v4_0.ret_inut_cte_v4_00 import RetInutCte
 from nfelib.cte.bindings.v4_0.tipos_geral_cte_v4_00 import (
     Tamb,
-    TcorgaoIbge,
     TcodUfIbge,
+    TcorgaoIbge,
     TmodCt,
-    TmodCtos,
     TmodCtCargaOs,
+    TmodCtos,
     TmodGtve,
     TmodNf,
     TrsakeyValueType,
-    TufSemEx,
-    Tuf,
     TtipoUnidCarga,
     TtipoUnidTransp,
+    Tuf,
+    TufSemEx,
 )
 from nfelib.cte.bindings.v4_0.xmldsig_core_schema_v1_01 import (
     KeyInfoType,
     ReferenceType,
     Signature,
     SignatureType,
     SignatureValueType,
     SignedInfoType,
-    TtransformUri,
-    TransformType,
     TransformsType,
+    TransformType,
+    TtransformUri,
     X509DataType,
 )
 
 __all__ = [
     "TconsSitCte",
     "TretConsSitCte",
     "ProcEventoCteVersao",
@@ -233,71 +242,79 @@
     "InfFretamentoTpFretamento",
     "PropTpProp",
     "RodoOs",
     "Rodo",
     "Multimodal",
     "MultimodalIndNegociavel",
     "CteOs",
+    "CteSimp",
     "CompTpComp",
     "Icms00Cst",
     "Icms20Cst",
     "Icms45Cst",
     "Icms60Cst",
     "Icms90Cst",
     "IcmsoutraUfCst",
     "IcmssnCst",
     "IcmssnIndSn",
     "Tcrt",
     "Tcte",
     "TcteOs",
+    "TcteSimp",
     "TdocAssoc",
     "TendOrg",
     "TendReEnt",
     "TendeEmi",
     "Tendereco",
     "Tendernac",
     "TfinCte",
+    "TfinCteSimp",
     "TfinGtve",
     "Tgtve",
     "Timp",
     "TimpOs",
     "Tlocal",
     "TmodTranspOs",
+    "TmodTranspSimp",
     "TprocEmi",
     "TprotCte",
     "TprotCteOs",
     "TprotGtve",
     "TrespTec",
     "TretCte",
     "TretCteOs",
+    "TretCteSimp",
     "TretGtve",
     "TunidCarga",
     "TunidadeTransp",
     "ComDataTpPer",
     "ComHoraTpHor",
     "IdeIndGlobalizado",
     "IdeIndIetoma",
     "IdeModal",
     "IdeRetira",
     "IdeTpEmis",
     "IdeTpImp",
     "IdeTpServ",
     "InfCteSubIndAlteraToma",
+    "InfDocAntTpPrest",
     "InfEspecieTpEspecie",
     "InfEspecieTpNumerario",
     "InfOutrosTpDoc",
     "InfQCUnid",
+    "InfQTpMed",
     "NoInterTpHor",
     "NoPeriodoTpPer",
     "SegRespSeg",
     "SemDataTpPer",
     "SemHoraTpHor",
     "Toma3Toma",
     "Toma4Toma",
     "TomaTerceiroToma",
+    "TomaIndIetoma",
     "TomaToma",
     "Cte",
     "EvCancCecte",
     "EvCancCecteDescEvento",
     "EvCancCte",
     "EvCancCteDescEvento",
     "EvCancIecte",
@@ -336,14 +353,15 @@
     "CteProc",
     "ProcEventoCte",
     "GtveProc",
     "ProcInutCte",
     "RetConsSitCte",
     "RetConsStatServCte",
     "RetCteOs",
+    "RetCteSimp",
     "RetCte",
     "RetEventoCte",
     "RetGtve",
     "RetInutCte",
     "Tamb",
     "TcorgaoIbge",
     "TcodUfIbge",
```

## Comparing `nfelib-2.0.4/nfelib/cte/bindings/v4_0/proc_gtve_v4_00.py` & `nfelib-2.0.5/nfelib/cte/bindings/v4_0/proc_gtve_v4_00.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:16:35
+"""This file was generated by xsdata, v24.4, on 2024-04-08 21:52:20
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass, field
-from nfelib import CommonMixin
 from typing import Optional
+
+from nfelib import CommonMixin
 from nfelib.cte.bindings.v4_0.cte_tipos_basico_v4_00 import (
     Tgtve,
     TprotGtve,
 )
 
 __NAMESPACE__ = "http://www.portalfiscal.inf.br/cte"
```

## Comparing `nfelib-2.0.4/nfelib/cte/bindings/v4_0/ev_iecte_v4_00.py` & `nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_iecte_v4_00.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:16:35
+"""This file was generated by xsdata, v24.4, on 2024-04-08 21:52:20
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass, field
 from enum import Enum
-from nfelib import CommonMixin
 from typing import List, Optional
 
+from nfelib import CommonMixin
+
 __NAMESPACE__ = "http://www.portalfiscal.inf.br/cte"
 
 
 class EvIecteDescEvento(Enum):
     INSUCESSO_NA_ENTREGA_DO_CT_E = "Insucesso na Entrega do CT-e"
```

## Comparing `nfelib-2.0.4/nfelib/cte/bindings/v4_0/ret_inut_cte_v4_00.py` & `nfelib-2.0.5/nfelib/nfe/bindings/v4_0/ret_cons_stat_serv_v4_00.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:16:35
+"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:31:20
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass
-from nfelib.cte.bindings.v4_0.inut_cte_tipos_basico_v4_00 import TretInutCte
+from nfelib.nfe.bindings.v4_0.leiaute_cons_stat_serv_v4_00 import (
+    TretConsStatServ,
+)
 
-__NAMESPACE__ = "http://www.portalfiscal.inf.br/cte"
+__NAMESPACE__ = "http://www.portalfiscal.inf.br/nfe"
 
 
 @dataclass
-class RetInutCte(TretInutCte):
+class RetConsStatServ(TretConsStatServ):
     """
-    Schema XML de validação do retorno do Pedido de Inutilização de Numeração do
-    CT-e.
+    Schema XML de validação do Resultado da Consulta do Status do Serviço.
     """
 
     class Meta:
-        name = "retInutCTe"
-        namespace = "http://www.portalfiscal.inf.br/cte"
+        name = "retConsStatServ"
+        namespace = "http://www.portalfiscal.inf.br/nfe"
```

## Comparing `nfelib-2.0.4/nfelib/cte/bindings/v4_0/proc_cte_v4_00.py` & `nfelib-2.0.5/nfelib/cte/bindings/v4_0/proc_cte_v4_00.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:16:35
+"""This file was generated by xsdata, v24.4, on 2024-04-08 21:52:20
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass, field
-from nfelib import CommonMixin
 from typing import Optional
+
+from nfelib import CommonMixin
 from nfelib.cte.bindings.v4_0.cte_tipos_basico_v4_00 import (
     Tcte,
     TprotCte,
 )
 
 __NAMESPACE__ = "http://www.portalfiscal.inf.br/cte"
```

## Comparing `nfelib-2.0.4/nfelib/cte/bindings/v4_0/proc_inut_cte_v4_00.py` & `nfelib-2.0.5/nfelib/nfe/bindings/v4_0/proc_inut_nfe_v4_00.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:16:35
+"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:31:20
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass
-from nfelib.cte.bindings.v4_0.inut_cte_tipos_basico_v4_00 import TprocInutCte
+from nfelib.nfe.bindings.v4_0.leiaute_inut_nfe_v4_00 import TprocInutNfe
 
-__NAMESPACE__ = "http://www.portalfiscal.inf.br/cte"
+__NAMESPACE__ = "http://www.portalfiscal.inf.br/nfe"
 
 
 @dataclass
-class ProcInutCte(TprocInutCte):
+class ProcInutNfe(TprocInutNfe):
     """
-    Pedido de inutilzação de numeração de CT-e processado.
+    Pedido de inutilização de númeração de  NF-e processado.
     """
 
     class Meta:
-        name = "procInutCTe"
-        namespace = "http://www.portalfiscal.inf.br/cte"
+        name = "ProcInutNFe"
+        namespace = "http://www.portalfiscal.inf.br/nfe"
```

## Comparing `nfelib-2.0.4/nfelib/cte/bindings/v4_0/ev_canc_prest_desacordo_v4_00.py` & `nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_prest_desacordo_v4_00.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,56 +1,64 @@
-"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:16:35
+"""This file was generated by xsdata, v24.4, on 2024-04-08 21:52:20
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass, field
 from enum import Enum
-from nfelib import CommonMixin
 from typing import Optional
 
+from nfelib import CommonMixin
+
 __NAMESPACE__ = "http://www.portalfiscal.inf.br/cte"
 
 
-class EvCancPrestDesacordoDescEvento(Enum):
-    CANCELAMENTO_PRESTA_O_DO_SERVI_O_EM_DESACORDO = (
-        "Cancelamento Prestação do Serviço em Desacordo"
-    )
-    CANCELAMENTO_PRESTACAO_DO_SERVICO_EM_DESACORDO = (
-        "Cancelamento Prestacao do Servico em Desacordo"
-    )
+class EvPrestDesacordoDescEvento(Enum):
+    PRESTA_O_DO_SERVI_O_EM_DESACORDO = "Prestação do Serviço em Desacordo"
+    PRESTACAO_DO_SERVICO_EM_DESACORDO = "Prestacao do Servico em Desacordo"
+
+
+class EvPrestDesacordoIndDesacordoOper(Enum):
+    VALUE_1 = "1"
 
 
 @dataclass
-class EvCancPrestDesacordo(CommonMixin):
+class EvPrestDesacordo(CommonMixin):
     """
-    Schema XML de validação do evento Cancelamento Prestação do Serviço em
-    Desacordo 610111.
+    Schema XML de validação do evento Prestação do Serviço em Desacordo 610110.
 
-    :ivar descEvento: Descrição do Evento - “Cancelamento Prestação do
-        Serviço em Desacordo”
-    :ivar nProtEvPrestDes: Protocolo do evento que será cancelado
-        Informar o número do protocolo de autorização do evento de
-        prestação de serviço em desacordo que será cancelado
+    :ivar descEvento: Descrição do Evento - “Prestação do Serviço em
+        Desacordo”
+    :ivar indDesacordoOper: Indicador de operação em desacordo
+    :ivar xObs: Observações do tomador
     """
 
     class Meta:
-        name = "evCancPrestDesacordo"
+        name = "evPrestDesacordo"
         namespace = "http://www.portalfiscal.inf.br/cte"
 
-    descEvento: Optional[EvCancPrestDesacordoDescEvento] = field(
+    descEvento: Optional[EvPrestDesacordoDescEvento] = field(
         default=None,
         metadata={
             "type": "Element",
             "required": True,
             "white_space": "preserve",
         },
     )
-    nProtEvPrestDes: Optional[str] = field(
+    indDesacordoOper: Optional[EvPrestDesacordoIndDesacordoOper] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+            "required": True,
+        },
+    )
+    xObs: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "required": True,
+            "min_length": 15,
+            "max_length": 255,
             "white_space": "preserve",
-            "pattern": r"[0-9]{15}",
+            "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
         },
     )
```

## Comparing `nfelib-2.0.4/nfelib/cte/bindings/v4_0/cte_modal_rodoviario_v4_00.py` & `nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_modal_rodoviario_v4_00.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:16:35
+"""This file was generated by xsdata, v24.4, on 2024-04-08 21:52:20
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass, field
-from nfelib import CommonMixin
 from typing import List, Optional
+
+from nfelib import CommonMixin
 from nfelib.cte.bindings.v4_0.tipos_geral_cte_v4_00 import Tuf
 
 __NAMESPACE__ = "http://www.portalfiscal.inf.br/cte"
 
 
 @dataclass
 class Rodo(CommonMixin):
```

## Comparing `nfelib-2.0.4/nfelib/cte/bindings/v4_0/ret_cons_sit_cte_v4_00.py` & `nfelib-2.0.5/nfelib/nfe/bindings/v4_0/ret_cons_sit_nfe_v4_00.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:16:35
+"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:31:20
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass
-from nfelib.cte.bindings.v4_0.cons_sit_cte_tipos_basico_v4_00 import (
-    TretConsSitCte,
-)
+from nfelib.nfe.bindings.v4_0.leiaute_cons_sit_nfe_v4_00 import TretConsSitNfe
 
-__NAMESPACE__ = "http://www.portalfiscal.inf.br/cte"
+__NAMESPACE__ = "http://www.portalfiscal.inf.br/nfe"
 
 
 @dataclass
-class RetConsSitCte(TretConsSitCte):
+class RetConsSitNfe(TretConsSitNfe):
     """
-    Schema XML de validação do retorno da consulta da situação atual do CT-e.
+    Schema XML de validação do retorno da consulta da situação atual da NF-e.
     """
 
     class Meta:
-        name = "retConsSitCTe"
-        namespace = "http://www.portalfiscal.inf.br/cte"
+        name = "retConsSitNFe"
+        namespace = "http://www.portalfiscal.inf.br/nfe"
```

## Comparing `nfelib-2.0.4/nfelib/cte/bindings/v4_0/ev_cce_cte_v4_00.py` & `nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_cce_cte_v4_00.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:16:35
+"""This file was generated by xsdata, v24.4, on 2024-04-08 21:52:20
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass, field
 from enum import Enum
-from nfelib import CommonMixin
 from typing import List, Optional
 
+from nfelib import CommonMixin
+
 __NAMESPACE__ = "http://www.portalfiscal.inf.br/cte"
 
 
 class EvCceCteDescEvento(Enum):
     CARTA_DE_CORRE_O = "Carta de Correção"
     CARTA_DE_CORRECAO = "Carta de Correcao"
```

## Comparing `nfelib-2.0.4/nfelib/cte/bindings/v4_0/evento_cte_tipos_basico_v4_00.py` & `nfelib-2.0.5/nfelib/cte/bindings/v4_0/evento_cte_tipos_basico_v4_00.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:16:35
+"""This file was generated by xsdata, v24.4, on 2024-04-08 21:52:20
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass, field
 from enum import Enum
-from nfelib import CommonMixin
 from typing import Optional
+
+from nfelib import CommonMixin
 from nfelib.cte.bindings.v4_0.tipos_geral_cte_v4_00 import (
     Tamb,
     TcorgaoIbge,
     TrsakeyValueType,
 )
 from nfelib.cte.bindings.v4_0.xmldsig_core_schema_v1_01 import Signature
```

## Comparing `nfelib-2.0.4/nfelib/cte/bindings/v4_0/tipos_geral_cte_v4_00.py` & `nfelib-2.0.5/nfelib/cte/bindings/v4_0/tipos_geral_cte_v4_00.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:16:35
+"""This file was generated by xsdata, v24.4, on 2024-04-08 21:52:20
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass, field
 from enum import Enum
-from nfelib import CommonMixin
 from typing import Optional
 
+from nfelib import CommonMixin
+
 __NAMESPACE__ = "http://www.portalfiscal.inf.br/cte"
 
 
 class Tamb(Enum):
     """
     Tipo Ambiente.
     """
```

## Comparing `nfelib-2.0.4/nfelib/cte/bindings/v4_0/ev_canc_cte_v4_00.py` & `nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_canc_cte_v4_00.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:16:35
+"""This file was generated by xsdata, v24.4, on 2024-04-08 21:52:20
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass, field
 from enum import Enum
-from nfelib import CommonMixin
 from typing import Optional
 
+from nfelib import CommonMixin
+
 __NAMESPACE__ = "http://www.portalfiscal.inf.br/cte"
 
 
 class EvCancCteDescEvento(Enum):
     CANCELAMENTO = "Cancelamento"
```

## Comparing `nfelib-2.0.4/nfelib/cte/bindings/v4_0/ret_gtve_v4_00.py` & `nfelib-2.0.5/nfelib/cte/bindings/v4_0/ret_gtve_v4_00.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:16:35
+"""This file was generated by xsdata, v24.4, on 2024-04-08 21:52:20
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass
+
 from nfelib.cte.bindings.v4_0.cte_tipos_basico_v4_00 import TretGtve
 
 __NAMESPACE__ = "http://www.portalfiscal.inf.br/cte"
 
 
 @dataclass
 class RetGtve(TretGtve):
```

## Comparing `nfelib-2.0.4/nfelib/cte/bindings/v4_0/cte_modal_rodoviario_os_v4_00.py` & `nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_modal_rodoviario_os_v4_00.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:16:35
+"""This file was generated by xsdata, v24.4, on 2024-04-08 21:52:20
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass, field
 from enum import Enum
-from nfelib import CommonMixin
 from typing import Optional
+
+from nfelib import CommonMixin
 from nfelib.cte.bindings.v4_0.tipos_geral_cte_v4_00 import Tuf
 
 __NAMESPACE__ = "http://www.portalfiscal.inf.br/cte"
 
 
 class InfFretamentoTpFretamento(Enum):
     VALUE_1 = "1"
```

## Comparing `nfelib-2.0.4/nfelib/cte/bindings/v4_0/proc_evento_cte_v4_00.py` & `nfelib-2.0.5/nfelib/cte/bindings/v4_0/proc_evento_cte_v4_00.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:16:35
+"""This file was generated by xsdata, v24.4, on 2024-04-08 21:52:20
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass
+
 from nfelib.cte.bindings.v4_0.evento_cte_tipos_basico_v4_00 import TprocEvento
 
 __NAMESPACE__ = "http://www.portalfiscal.inf.br/cte"
 
 
 @dataclass
 class ProcEventoCte(TprocEvento):
```

## Comparing `nfelib-2.0.4/nfelib/cte/bindings/v4_0/cte_modal_aquaviario_v4_00.py` & `nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_modal_aquaviario_v4_00.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:16:35
+"""This file was generated by xsdata, v24.4, on 2024-04-08 21:52:20
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass, field
 from enum import Enum
-from nfelib import CommonMixin
 from typing import List, Optional
 
+from nfelib import CommonMixin
+
 __NAMESPACE__ = "http://www.portalfiscal.inf.br/cte"
 
 
 class AquavDirec(Enum):
     N = "N"
     S = "S"
     L = "L"
```

## Comparing `nfelib-2.0.4/nfelib/cte/bindings/v4_0/ev_gtv_v4_00.py` & `nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_gtv_v4_00.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:16:35
+"""This file was generated by xsdata, v24.4, on 2024-04-08 21:52:20
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass, field
 from enum import Enum
-from nfelib import CommonMixin
 from typing import List, Optional
+
+from nfelib import CommonMixin
 from nfelib.cte.bindings.v4_0.cte_tipos_basico_v4_00 import InfEspecieTpEspecie
 from nfelib.cte.bindings.v4_0.tipos_geral_cte_v4_00 import Tuf
 
 __NAMESPACE__ = "http://www.portalfiscal.inf.br/cte"
 
 
 class EvGtvDescEvento(Enum):
```

## Comparing `nfelib-2.0.4/nfelib/cte/bindings/v4_0/cte_modal_dutoviario_v4_00.py` & `nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_modal_dutoviario_v4_00.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:16:35
+"""This file was generated by xsdata, v24.4, on 2024-04-08 21:52:20
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass, field
-from nfelib import CommonMixin
 from typing import Optional
 
+from nfelib import CommonMixin
+
 __NAMESPACE__ = "http://www.portalfiscal.inf.br/cte"
 
 
 @dataclass
 class Duto(CommonMixin):
     """
     Informações do modal Dutoviário.
```

## Comparing `nfelib-2.0.4/nfelib/cte/bindings/v4_0/cte_tipos_basico_v4_00.py` & `nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_tipos_basico_v4_00.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:16:35
+"""This file was generated by xsdata, v24.4, on 2024-04-08 21:52:20
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass, field
 from enum import Enum
-from nfelib import CommonMixin
 from typing import List, Optional
+
+from nfelib import CommonMixin
 from nfelib.cte.bindings.v4_0.evento_cte_tipos_basico_v4_00 import TmodTransp
 from nfelib.cte.bindings.v4_0.tipos_geral_cte_v4_00 import (
     Tamb,
     TcodUfIbge,
     TmodCt,
     TmodCtos,
     TmodGtve,
     TmodNf,
     TrsakeyValueType,
-    TufSemEx,
-    Tuf,
     TtipoUnidCarga,
     TtipoUnidTransp,
+    Tuf,
+    TufSemEx,
 )
 from nfelib.cte.bindings.v4_0.xmldsig_core_schema_v1_01 import Signature
 
 __NAMESPACE__ = "http://www.portalfiscal.inf.br/cte"
 
 
 class CompTpComp(Enum):
@@ -100,14 +101,23 @@
     """
 
     VALUE_0 = "0"
     VALUE_1 = "1"
     VALUE_3 = "3"
 
 
+class TfinCteSimp(Enum):
+    """
+    Tipos Finalidade de CT-e Simplificado.
+    """
+
+    VALUE_4 = "4"
+    VALUE_5 = "5"
+
+
 class TfinGtve(Enum):
     """
     Tipo Finalidade da GTV-e.
     """
 
     VALUE_4 = "4"
 
@@ -119,14 +129,24 @@
 
     VALUE_01 = "01"
     VALUE_02 = "02"
     VALUE_03 = "03"
     VALUE_04 = "04"
 
 
+class TmodTranspSimp(Enum):
+    """
+    Tipo Modal transporte do CTe Simplificado.
+    """
+
+    VALUE_01 = "01"
+    VALUE_02 = "02"
+    VALUE_03 = "03"
+
+
 class TprocEmi(Enum):
     """
     Tipo processo de emissão do CT-e.
     """
 
     VALUE_0 = "0"
     VALUE_3 = "3"
@@ -271,14 +291,19 @@
     VALUE_9 = "9"
 
 
 class InfCteSubIndAlteraToma(Enum):
     VALUE_1 = "1"
 
 
+class InfDocAntTpPrest(Enum):
+    VALUE_1 = "1"
+    VALUE_2 = "2"
+
+
 class InfEspecieTpEspecie(Enum):
     VALUE_1 = "1"
     VALUE_2 = "2"
     VALUE_3 = "3"
     VALUE_4 = "4"
 
 
@@ -300,14 +325,34 @@
     VALUE_01 = "01"
     VALUE_02 = "02"
     VALUE_03 = "03"
     VALUE_04 = "04"
     VALUE_05 = "05"
 
 
+class InfQTpMed(Enum):
+    VALUE_00 = "00"
+    VALUE_01 = "01"
+    VALUE_02 = "02"
+    VALUE_03 = "03"
+    VALUE_04 = "04"
+    VALUE_05 = "05"
+    VALUE_06 = "06"
+    VALUE_07 = "07"
+    VALUE_08 = "08"
+    VALUE_09 = "09"
+    VALUE_10 = "10"
+    VALUE_11 = "11"
+    VALUE_12 = "12"
+    VALUE_13 = "13"
+    VALUE_14 = "14"
+    VALUE_15 = "15"
+    VALUE_99 = "99"
+
+
 class NoInterTpHor(Enum):
     VALUE_4 = "4"
 
 
 class NoPeriodoTpPer(Enum):
     VALUE_4 = "4"
 
@@ -336,14 +381,20 @@
     VALUE_4 = "4"
 
 
 class TomaTerceiroToma(Enum):
     VALUE_4 = "4"
 
 
+class TomaIndIetoma(Enum):
+    VALUE_1 = "1"
+    VALUE_2 = "2"
+    VALUE_9 = "9"
+
+
 class TomaToma(Enum):
     VALUE_0 = "0"
     VALUE_1 = "1"
 
 
 @dataclass
 class TendOrg(CommonMixin):
@@ -5658,14 +5709,100 @@
             "white_space": "preserve",
             "pattern": r"4\.00",
         },
     )
 
 
 @dataclass
+class TretCteSimp(CommonMixin):
+    """
+    Tipo Retorno do Pedido de Autorização de CT-e Simplificado (Modelo 57)
+
+    :ivar tpAmb: Identificação do Ambiente: 1 - Produção 2 - Homologação
+    :ivar cUF: Identificação da UF
+    :ivar verAplic: Versão do Aplicativo que processou a CT-e
+    :ivar cStat: código do status do retorno da consulta.
+    :ivar xMotivo: Descrição literal do status do do retorno da
+        consulta.
+    :ivar protCTe: Reposta ao processamento do CT-e
+    :ivar versao:
+    """
+
+    class Meta:
+        name = "TRetCTeSimp"
+
+    tpAmb: Optional[Tamb] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+            "namespace": "http://www.portalfiscal.inf.br/cte",
+            "required": True,
+        },
+    )
+    cUF: Optional[TcodUfIbge] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+            "namespace": "http://www.portalfiscal.inf.br/cte",
+            "required": True,
+        },
+    )
+    verAplic: Optional[str] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+            "namespace": "http://www.portalfiscal.inf.br/cte",
+            "required": True,
+            "min_length": 1,
+            "max_length": 20,
+            "white_space": "preserve",
+            "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
+        },
+    )
+    cStat: Optional[str] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+            "namespace": "http://www.portalfiscal.inf.br/cte",
+            "required": True,
+            "white_space": "preserve",
+            "pattern": r"[0-9]{3}",
+        },
+    )
+    xMotivo: Optional[str] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+            "namespace": "http://www.portalfiscal.inf.br/cte",
+            "required": True,
+            "min_length": 1,
+            "max_length": 255,
+            "white_space": "preserve",
+            "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
+        },
+    )
+    protCTe: Optional[TprotCte] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+            "namespace": "http://www.portalfiscal.inf.br/cte",
+        },
+    )
+    versao: Optional[str] = field(
+        default=None,
+        metadata={
+            "type": "Attribute",
+            "required": True,
+            "white_space": "preserve",
+            "pattern": r"4\.00",
+        },
+    )
+
+
+@dataclass
 class TretGtve(CommonMixin):
     """
     Tipo Retorno do Pedido de Autorização de GTV-e (Modelo 64)
 
     :ivar tpAmb: Identificação do Ambiente: 1 - Produção 2 - Homologação
     :ivar cUF: Identificação da UF
     :ivar verAplic: Versão do Aplicativo que processou a GTV-e
@@ -6086,16 +6223,16 @@
                 documento foi transmitido) Informar PAIS/Municipio para
                 as operações com o exterior.
             :ivar UFEnv: Sigla da UF de envio do CT-e (de onde o
                 documento foi transmitido) Informar 'EX' para operações
                 com o exterior.
             :ivar modal: Modal Preencher com:01-Rodoviário;
                 02-Aéreo;03-Aquaviário;04-Ferroviário;05-Dutoviário;06-Multimodal;
-            :ivar tpServ: Tipo do Serviço Preencher com: 0 - Normal;1 -
-                Subcontratação; 2 - Redespacho;3 - Redespacho
+            :ivar tpServ: Tipo do Serviço Preencher com: 0 - Normal; 1 -
+                Subcontratação; 2 - Redespacho; 3 - Redespacho
                 Intermediário; 4 - Serviço Vinculado a Multimodal
             :ivar cMunIni: Código do Município de início da prestação
                 Utilizar a tabela do IBGE. Informar 9999999 para
                 operações com o exterior.
             :ivar xMunIni: Nome do Município do início da prestação
                 Informar 'EXTERIOR' para operações com o exterior.
             :ivar UFIni: UF do início da prestação Informar 'EX' para
@@ -9037,14 +9174,1846 @@
 
     @dataclass
     class InfCteSupl(CommonMixin):
         """
         :ivar qrCodCTe: Texto com o QR-Code impresso no DACTE
         """
 
+        qrCodCTe: Optional[str] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+                "namespace": "http://www.portalfiscal.inf.br/cte",
+                "required": True,
+                "min_length": 50,
+                "max_length": 1000,
+                "white_space": "preserve",
+                "pattern": r"((HTTPS?|https?)://.*\?chCTe=[0-9]{44}&tpAmb=[1-2](&sign=[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1})?)",
+            },
+        )
+
+
+@dataclass
+class TcteSimp(CommonMixin):
+    """Tipo Conhecimento de Transporte Eletrônico (Modelo 57) - Modelo Simplificado
+
+    :ivar infCte: Informações do CT-e
+    :ivar infCTeSupl: Informações suplementares do CT-e
+    :ivar signature:
+    """
+
+    class Meta:
+        name = "TCTeSimp"
+
+    infCte: Optional["TcteSimp.InfCte"] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+            "namespace": "http://www.portalfiscal.inf.br/cte",
+            "required": True,
+        },
+    )
+    infCTeSupl: Optional["TcteSimp.InfCteSupl"] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+            "namespace": "http://www.portalfiscal.inf.br/cte",
+        },
+    )
+    signature: Optional[Signature] = field(
+        default=None,
+        metadata={
+            "name": "Signature",
+            "type": "Element",
+            "namespace": "http://www.w3.org/2000/09/xmldsig#",
+            "required": True,
+        },
+    )
+
+    @dataclass
+    class InfCte(CommonMixin):
+        """
+        :ivar ide: Identificação do CT-e
+        :ivar compl: Dados complementares do CT-e para fins operacionais
+            ou comerciais
+        :ivar emit: Identificação do Emitente do CT-e
+        :ivar toma: Identificação do tomador do serviço no CT-e
+        :ivar infCarga: Informações da Carga do CT-e
+        :ivar det: Detalhamento das entregas / prestações do CTe
+            Simplificado
+        :ivar infModal: Informações do modal
+        :ivar cobr: Dados da cobrança do CT-e
+        :ivar infCteSub: Informações do CT-e de substituição
+        :ivar imp: Informações relativas aos Impostos
+        :ivar total: Valores Totais do CTe
+        :ivar autXML: Autorizados para download do XML do DF-e Informar
+            CNPJ ou CPF. Preencher os zeros não significativos.
+        :ivar infRespTec: Informações do Responsável Técnico pela
+            emissão do DF-e
+        :ivar infSolicNFF: Grupo de informações do pedido de emissão da
+            Nota Fiscal Fácil
+        :ivar infPAA: Grupo de Informação do Provedor de Assinatura e
+            Autorização
+        :ivar versao: Versão do leiaute Ex: "4.00"
+        :ivar Id: Identificador da tag a ser assinada Informar a chave
+            de acesso do CT-e e precedida do literal "CTe"
+        """
+
+        ide: Optional["TcteSimp.InfCte.Ide"] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+                "namespace": "http://www.portalfiscal.inf.br/cte",
+                "required": True,
+            },
+        )
+        compl: Optional["TcteSimp.InfCte.Compl"] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+                "namespace": "http://www.portalfiscal.inf.br/cte",
+            },
+        )
+        emit: Optional["TcteSimp.InfCte.Emit"] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+                "namespace": "http://www.portalfiscal.inf.br/cte",
+                "required": True,
+            },
+        )
+        toma: Optional["TcteSimp.InfCte.Toma"] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+                "namespace": "http://www.portalfiscal.inf.br/cte",
+                "required": True,
+            },
+        )
+        infCarga: Optional["TcteSimp.InfCte.InfCarga"] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+                "namespace": "http://www.portalfiscal.inf.br/cte",
+                "required": True,
+            },
+        )
+        det: List["TcteSimp.InfCte.Det"] = field(
+            default_factory=list,
+            metadata={
+                "type": "Element",
+                "namespace": "http://www.portalfiscal.inf.br/cte",
+                "min_occurs": 1,
+                "max_occurs": 999,
+            },
+        )
+        infModal: Optional["TcteSimp.InfCte.InfModal"] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+                "namespace": "http://www.portalfiscal.inf.br/cte",
+                "required": True,
+            },
+        )
+        cobr: Optional["TcteSimp.InfCte.Cobr"] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+                "namespace": "http://www.portalfiscal.inf.br/cte",
+            },
+        )
+        infCteSub: Optional["TcteSimp.InfCte.InfCteSub"] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+                "namespace": "http://www.portalfiscal.inf.br/cte",
+            },
+        )
+        imp: Optional["TcteSimp.InfCte.Imp"] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+                "namespace": "http://www.portalfiscal.inf.br/cte",
+                "required": True,
+            },
+        )
+        total: Optional["TcteSimp.InfCte.Total"] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+                "namespace": "http://www.portalfiscal.inf.br/cte",
+                "required": True,
+            },
+        )
+        autXML: List["TcteSimp.InfCte.AutXml"] = field(
+            default_factory=list,
+            metadata={
+                "type": "Element",
+                "namespace": "http://www.portalfiscal.inf.br/cte",
+                "max_occurs": 10,
+            },
+        )
+        infRespTec: Optional[TrespTec] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+                "namespace": "http://www.portalfiscal.inf.br/cte",
+            },
+        )
+        infSolicNFF: Optional["TcteSimp.InfCte.InfSolicNff"] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+                "namespace": "http://www.portalfiscal.inf.br/cte",
+            },
+        )
+        infPAA: Optional["TcteSimp.InfCte.InfPaa"] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+                "namespace": "http://www.portalfiscal.inf.br/cte",
+            },
+        )
+        versao: Optional[str] = field(
+            default=None,
+            metadata={
+                "type": "Attribute",
+                "required": True,
+                "white_space": "preserve",
+                "pattern": r"4\.00",
+            },
+        )
+        Id: Optional[str] = field(
+            default=None,
+            metadata={
+                "type": "Attribute",
+                "required": True,
+                "pattern": r"CTe[0-9]{44}",
+            },
+        )
+
+        @dataclass
+        class Ide(CommonMixin):
+            """
+            :ivar cUF: Código da UF do emitente do CT-e. Utilizar a
+                Tabela do IBGE.
+            :ivar cCT: Código numérico que compõe a Chave de Acesso.
+                Número aleatório gerado pelo emitente para cada CT-e,
+                com o objetivo de evitar acessos indevidos ao documento.
+            :ivar CFOP: Código Fiscal de Operações e Prestações
+            :ivar natOp: Natureza da Operação
+            :ivar mod: Modelo do documento fiscal Utilizar o código 57
+                para identificação do CT-e, emitido em substituição aos
+                modelos de conhecimentos em papel.
+            :ivar serie: Série do CT-e Preencher com "0" no caso de
+                série única
+            :ivar nCT: Número do CT-e
+            :ivar dhEmi: Data e hora de emissão do CT-e Formato AAAA-MM-
+                DDTHH:MM:DD TZD
+            :ivar tpImp: Formato de impressão do DACTE Preencher com: 1
+                - Retrato; 2 - Paisagem.
+            :ivar tpEmis: Forma de emissão do CT-e Preencher com: 1 -
+                Normal; 3 - Regime Especial NFF; 4 - EPEC pela SVC; 7 -
+                Autorização pela SVC-RS; 8 - Autorização pela SVC-SP
+            :ivar cDV: Digito Verificador da chave de acesso do CT-e
+                Informar o dígito  de controle da chave de acesso do
+                CT-e, que deve ser calculado com a aplicação do
+                algoritmo módulo 11 (base 2,9) da chave de acesso.
+            :ivar tpAmb: Tipo do Ambiente Preencher com:1 - Produção; 2
+                - Homologação.
+            :ivar tpCTe: Tipo do CT-e Simplificado Preencher com: 4 -
+                CTe Simplificado 5 - Substituição CTe Simplificado
+            :ivar procEmi: Identificador do processo de emissão do CT-e
+                Preencher com: 0 - emissão de CT-e com aplicativo do
+                contribuinte; 3- emissão CT-e pelo contribuinte com
+                aplicativo fornecido pelo SEBRAE.
+            :ivar verProc: Versão do processo de emissão Informar a
+                versão do aplicativo emissor de CT-e.
+            :ivar cMunEnv: Código do Município de envio do CT-e (de onde
+                o documento foi transmitido) Utilizar a tabela do IBGE.
+                Informar 9999999 para as operações com o exterior.
+            :ivar xMunEnv: Nome do Município de envio do CT-e (de onde o
+                documento foi transmitido) Informar PAIS/Municipio para
+                as operações com o exterior.
+            :ivar UFEnv: Sigla da UF de envio do CT-e (de onde o
+                documento foi transmitido) Informar 'EX' para operações
+                com o exterior.
+            :ivar modal: Modal Preencher com: 01-Rodoviário 02-Aéreo
+                03-Aquaviário
+            :ivar tpServ: Tipo do Serviço Preencher com: 0 - Normal; 1 -
+                Subcontratação; 2 - Redespacho;
+            :ivar UFIni: UF do início da prestação Informar 'EX' para
+                operações com o exterior.
+            :ivar UFFim: UF do término da prestação Informar 'EX' para
+                operações com o exterior.
+            :ivar retira: Indicador se o Recebedor retira no Aeroporto,
+                Filial, Porto ou Estação de Destino? Preencher com: 0 -
+                sim; 1 - não
+            :ivar xDetRetira: Detalhes do retira
+            :ivar dhCont: Data e Hora da entrada em contingência
+                Informar a data e hora no formato AAAA-MM-DDTHH:MM:SS
+            :ivar xJust: Justificativa da entrada em contingência
+            """
+
+            cUF: Optional[TcodUfIbge] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "required": True,
+                },
+            )
+            cCT: Optional[str] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "required": True,
+                    "white_space": "preserve",
+                    "pattern": r"[0-9]{8}",
+                },
+            )
+            CFOP: Optional[str] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "required": True,
+                    "white_space": "preserve",
+                    "pattern": r"[123567][0-9]([0-9][1-9]|[1-9][0-9])",
+                },
+            )
+            natOp: Optional[str] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "required": True,
+                    "min_length": 1,
+                    "max_length": 60,
+                    "white_space": "preserve",
+                    "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
+                },
+            )
+            mod: Optional[TmodCt] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "required": True,
+                },
+            )
+            serie: Optional[str] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "required": True,
+                    "white_space": "preserve",
+                    "pattern": r"0|[1-9]{1}[0-9]{0,2}",
+                },
+            )
+            nCT: Optional[str] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "required": True,
+                    "white_space": "preserve",
+                    "pattern": r"[1-9]{1}[0-9]{0,8}",
+                },
+            )
+            dhEmi: Optional[str] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "required": True,
+                    "white_space": "preserve",
+                    "pattern": r"(((20(([02468][048])|([13579][26]))-02-29))|(20[0-9][0-9])-((((0[1-9])|(1[0-2]))-((0[1-9])|(1\d)|(2[0-8])))|((((0[13578])|(1[02]))-31)|(((0[1,3-9])|(1[0-2]))-(29|30)))))T(20|21|22|23|[0-1]\d):[0-5]\d:[0-5]\d([\-,\+](0[0-9]|10|11):00|([\+](12):00))",
+                },
+            )
+            tpImp: Optional[IdeTpImp] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "required": True,
+                    "white_space": "preserve",
+                },
+            )
+            tpEmis: Optional[IdeTpEmis] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "required": True,
+                    "white_space": "preserve",
+                },
+            )
+            cDV: Optional[str] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "required": True,
+                    "white_space": "preserve",
+                    "pattern": r"[0-9]{1}",
+                },
+            )
+            tpAmb: Optional[Tamb] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "required": True,
+                },
+            )
+            tpCTe: Optional[TfinCteSimp] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "required": True,
+                },
+            )
+            procEmi: Optional[TprocEmi] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "required": True,
+                },
+            )
+            verProc: Optional[str] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "required": True,
+                    "min_length": 1,
+                    "max_length": 20,
+                    "white_space": "preserve",
+                    "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
+                },
+            )
+            cMunEnv: Optional[str] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "required": True,
+                    "white_space": "preserve",
+                    "pattern": r"[0-9]{7}",
+                },
+            )
+            xMunEnv: Optional[str] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "required": True,
+                    "min_length": 2,
+                    "max_length": 60,
+                    "white_space": "preserve",
+                    "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
+                },
+            )
+            UFEnv: Optional[Tuf] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "required": True,
+                },
+            )
+            modal: Optional[TmodTranspSimp] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "required": True,
+                },
+            )
+            tpServ: Optional[IdeTpServ] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "required": True,
+                    "white_space": "preserve",
+                },
+            )
+            UFIni: Optional[Tuf] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "required": True,
+                },
+            )
+            UFFim: Optional[Tuf] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "required": True,
+                },
+            )
+            retira: Optional[IdeRetira] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "required": True,
+                    "white_space": "preserve",
+                },
+            )
+            xDetRetira: Optional[str] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "min_length": 1,
+                    "max_length": 160,
+                    "white_space": "preserve",
+                    "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
+                },
+            )
+            dhCont: Optional[str] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "white_space": "preserve",
+                    "pattern": r"(((20(([02468][048])|([13579][26]))-02-29))|(20[0-9][0-9])-((((0[1-9])|(1[0-2]))-((0[1-9])|(1\d)|(2[0-8])))|((((0[13578])|(1[02]))-31)|(((0[1,3-9])|(1[0-2]))-(29|30)))))T(20|21|22|23|[0-1]\d):[0-5]\d:[0-5]\d([\-,\+](0[0-9]|10|11):00|([\+](12):00))",
+                },
+            )
+            xJust: Optional[str] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "min_length": 15,
+                    "max_length": 256,
+                    "white_space": "preserve",
+                    "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
+                },
+            )
+
+        @dataclass
+        class Compl(CommonMixin):
+            """
+            :ivar xCaracAd: Característica adicional do transporte Texto
+                livre: REENTREGA; DEVOLUÇÃO; REFATURAMENTO; etc
+            :ivar xCaracSer: Característica adicional do serviço Texto
+                livre: ENTREGA EXPRESSA; LOGÍSTICA REVERSA;
+                CONVENCIONAL; EMERGENCIAL; etc
+            :ivar fluxo: Previsão do fluxo da carga Preenchimento
+                obrigatório para o modal aéreo.
+            :ivar xObs: Observações Gerais
+            :ivar obsCont: Campo de uso livre do contribuinte Informar o
+                nome do campo no atributo xCampo e o conteúdo do campo
+                no XTexto
+            :ivar obsFisco: Campo de uso livre do contribuinte Informar
+                o nome do campo no atributo xCampo e o conteúdo do campo
+                no XTexto
+            """
+
+            xCaracAd: Optional[str] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "min_length": 1,
+                    "max_length": 15,
+                    "white_space": "preserve",
+                    "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
+                },
+            )
+            xCaracSer: Optional[str] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "min_length": 1,
+                    "max_length": 30,
+                    "white_space": "preserve",
+                    "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
+                },
+            )
+            fluxo: Optional["TcteSimp.InfCte.Compl.Fluxo"] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                },
+            )
+            xObs: Optional[str] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "min_length": 1,
+                    "max_length": 2000,
+                    "white_space": "preserve",
+                    "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
+                },
+            )
+            obsCont: List["TcteSimp.InfCte.Compl.ObsCont"] = field(
+                default_factory=list,
+                metadata={
+                    "name": "ObsCont",
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "max_occurs": 10,
+                },
+            )
+            obsFisco: List["TcteSimp.InfCte.Compl.ObsFisco"] = field(
+                default_factory=list,
+                metadata={
+                    "name": "ObsFisco",
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "max_occurs": 10,
+                },
+            )
+
+            @dataclass
+            class Fluxo(CommonMixin):
+                """
+                :ivar xOrig: Sigla ou código interno da
+                    Filial/Porto/Estação/ Aeroporto de Origem
+                    Observações para o modal aéreo: - Preenchimento
+                    obrigatório para o modal aéreo. - O código de três
+                    letras IATA do aeroporto de partida deverá ser
+                    incluído como primeira anotação. Quando não for
+                    possível, utilizar a sigla OACI.
+                :ivar pass_value:
+                :ivar xDest: Sigla ou código interno da
+                    Filial/Porto/Estação/Aeroporto de Destino
+                    Observações para o modal aéreo: - Preenchimento
+                    obrigatório para o modal aéreo. - Deverá ser
+                    incluído o código de três letras IATA do aeroporto
+                    de destino. Quando não for possível, utilizar a
+                    sigla OACI.
+                :ivar xRota: Código da Rota de Entrega
+                """
+
+                xOrig: Optional[str] = field(
+                    default=None,
+                    metadata={
+                        "type": "Element",
+                        "namespace": "http://www.portalfiscal.inf.br/cte",
+                        "min_length": 1,
+                        "max_length": 60,
+                        "white_space": "preserve",
+                        "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
+                    },
+                )
+                pass_value: List["TcteSimp.InfCte.Compl.Fluxo.Pass"] = field(
+                    default_factory=list,
+                    metadata={
+                        "name": "pass",
+                        "type": "Element",
+                        "namespace": "http://www.portalfiscal.inf.br/cte",
+                    },
+                )
+                xDest: Optional[str] = field(
+                    default=None,
+                    metadata={
+                        "type": "Element",
+                        "namespace": "http://www.portalfiscal.inf.br/cte",
+                        "min_length": 1,
+                        "max_length": 60,
+                        "white_space": "preserve",
+                        "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
+                    },
+                )
+                xRota: Optional[str] = field(
+                    default=None,
+                    metadata={
+                        "type": "Element",
+                        "namespace": "http://www.portalfiscal.inf.br/cte",
+                        "min_length": 1,
+                        "max_length": 10,
+                        "white_space": "preserve",
+                        "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
+                    },
+                )
+
+                @dataclass
+                class Pass(CommonMixin):
+                    """
+                    :ivar xPass: Sigla ou código interno da
+                        Filial/Porto/Estação/Aeroporto de Passagem
+                        Observação para o modal aéreo: - O código de
+                        três letras IATA, referente ao aeroporto de
+                        transferência, deverá ser incluído, quando for o
+                        caso. Quando não for possível,  utilizar a sigla
+                        OACI. Qualquer solicitação de itinerário deverá
+                        ser incluída.
+                    """
+
+                    xPass: Optional[str] = field(
+                        default=None,
+                        metadata={
+                            "type": "Element",
+                            "namespace": "http://www.portalfiscal.inf.br/cte",
+                            "min_length": 1,
+                            "max_length": 15,
+                            "white_space": "preserve",
+                            "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
+                        },
+                    )
+
+            @dataclass
+            class ObsCont(CommonMixin):
+                """
+                :ivar xTexto: Conteúdo do campo
+                :ivar xCampo: Identificação do campo
+                """
+
+                xTexto: Optional[str] = field(
+                    default=None,
+                    metadata={
+                        "type": "Element",
+                        "namespace": "http://www.portalfiscal.inf.br/cte",
+                        "required": True,
+                        "min_length": 1,
+                        "max_length": 160,
+                        "white_space": "preserve",
+                        "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
+                    },
+                )
+                xCampo: Optional[str] = field(
+                    default=None,
+                    metadata={
+                        "type": "Attribute",
+                        "required": True,
+                        "min_length": 1,
+                        "max_length": 20,
+                        "white_space": "preserve",
+                        "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
+                    },
+                )
+
+            @dataclass
+            class ObsFisco(CommonMixin):
+                """
+                :ivar xTexto: Conteúdo do campo
+                :ivar xCampo: Identificação do campo
+                """
+
+                xTexto: Optional[str] = field(
+                    default=None,
+                    metadata={
+                        "type": "Element",
+                        "namespace": "http://www.portalfiscal.inf.br/cte",
+                        "required": True,
+                        "min_length": 1,
+                        "max_length": 60,
+                        "white_space": "preserve",
+                        "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
+                    },
+                )
+                xCampo: Optional[str] = field(
+                    default=None,
+                    metadata={
+                        "type": "Attribute",
+                        "required": True,
+                        "min_length": 1,
+                        "max_length": 20,
+                        "white_space": "preserve",
+                        "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
+                    },
+                )
+
+        @dataclass
+        class Emit(CommonMixin):
+            """
+            :ivar CNPJ: CNPJ do emitente Informar zeros não
+                significativos
+            :ivar CPF: CPF do emitente Informar zeros não
+                significativos. Usar com série específica 920-969 para
+                emitente pessoa física com inscrição estadual
+            :ivar IE: Inscrição Estadual do Emitente A IE do emitente
+                somente ficará sem informação para o caso do Regime
+                Especial da NFF (tpEmis=3)
+            :ivar IEST: Inscrição Estadual do Substituto Tributário
+            :ivar xNome: Razão social ou Nome do emitente
+            :ivar xFant: Nome fantasia
+            :ivar enderEmit: Endereço do emitente
+            :ivar CRT: Código do Regime Tributário Informar: 1=Simples
+                Nacional; 2=Simples Nacional, excesso sublimite de
+                receita bruta; 3=Regime Normal. 4=Simples Nacional -
+                Microempreendedor Individual – MEI.
+            """
+
+            CNPJ: Optional[str] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "white_space": "preserve",
+                    "pattern": r"[0-9]{14}",
+                },
+            )
+            CPF: Optional[str] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "white_space": "preserve",
+                    "pattern": r"[0-9]{11}",
+                },
+            )
+            IE: Optional[str] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "max_length": 14,
+                    "white_space": "preserve",
+                    "pattern": r"[0-9]{2,14}",
+                },
+            )
+            IEST: Optional[str] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "max_length": 14,
+                    "white_space": "preserve",
+                    "pattern": r"[0-9]{2,14}",
+                },
+            )
+            xNome: Optional[str] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "required": True,
+                    "min_length": 2,
+                    "max_length": 60,
+                    "white_space": "preserve",
+                    "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
+                },
+            )
+            xFant: Optional[str] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "min_length": 2,
+                    "max_length": 60,
+                    "white_space": "preserve",
+                    "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
+                },
+            )
+            enderEmit: Optional[TendeEmi] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "required": True,
+                },
+            )
+            CRT: Optional[Tcrt] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "required": True,
+                },
+            )
+
+        @dataclass
+        class Toma(CommonMixin):
+            """
+            :ivar toma: Tomador do Serviço Preencher com: 0-Remetente;
+                1-Expedidor; 2-Recebedor; 3-Destinatário 4-Terceiro
+            :ivar indIEToma: Indicador do papel do tomador na prestação
+                do serviço: 1 – Contribuinte ICMS; 2 – Contribuinte
+                isento de inscrição; 9 – Não Contribuinte Aplica-se ao
+                tomador que for indicado no toma3 ou toma4
+            :ivar CNPJ: Número do CNPJ Em caso de empresa não
+                estabelecida no Brasil, será informado o CNPJ com zeros.
+                Informar os zeros não significativos.
+            :ivar CPF: Número do CPF Informar os zeros não
+                significativos.
+            :ivar IE: Inscrição Estadual Informar a IE do tomador ou
+                ISENTO se tomador é contribuinte do ICMS isento de
+                inscrição no cadastro de contribuintes do ICMS. Caso o
+                tomador não seja contribuinte do ICMS não informar o
+                conteúdo.
+            :ivar xNome: Razão Social ou Nome
+            :ivar ISUF: Inscrição na SUFRAMA (Obrigatório nas operações
+                com as áreas com benefícios de incentivos fiscais sob
+                controle da SUFRAMA)
+            :ivar fone: Telefone
+            :ivar enderToma: Dados do endereço
+            :ivar email: Endereço de email
+            """
+
+            toma: Optional[TomaToma] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "required": True,
+                    "white_space": "preserve",
+                },
+            )
+            indIEToma: Optional[TomaIndIetoma] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "required": True,
+                    "white_space": "preserve",
+                },
+            )
+            CNPJ: Optional[str] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "white_space": "preserve",
+                    "pattern": r"[0-9]{0}|[0-9]{14}",
+                },
+            )
+            CPF: Optional[str] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "white_space": "preserve",
+                    "pattern": r"[0-9]{11}",
+                },
+            )
+            IE: Optional[str] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "max_length": 14,
+                    "white_space": "preserve",
+                    "pattern": r"[0-9]{0,14}|ISENTO",
+                },
+            )
+            xNome: Optional[str] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "required": True,
+                    "min_length": 2,
+                    "max_length": 60,
+                    "white_space": "preserve",
+                    "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
+                },
+            )
+            ISUF: Optional[str] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "white_space": "preserve",
+                    "pattern": r"[0-9]{8,9}",
+                },
+            )
+            fone: Optional[str] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "white_space": "preserve",
+                    "pattern": r"[0-9]{6,14}",
+                },
+            )
+            enderToma: Optional[Tendereco] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "required": True,
+                },
+            )
+            email: Optional[str] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "min_length": 1,
+                    "max_length": 60,
+                    "white_space": "preserve",
+                    "pattern": r"[^@]+@[^\.]+\..+",
+                },
+            )
+
+        @dataclass
+        class InfCarga(CommonMixin):
+            """
+            :ivar vCarga: Valor total da carga
+            :ivar proPred: Produto predominante Informar a descrição do
+                produto predominante
+            :ivar xOutCat: Outras características da carga "FRIA",
+                "GRANEL", "REFRIGERADA", "Medidas: 12X12X12"
+            :ivar infQ: Informações de quantidades da Carga do CT-e Para
+                o Aéreo é obrigatório o preenchimento desse campo da
+                seguinte forma. 1 - Peso Bruto, sempre em quilogramas
+                (obrigatório); 2 - Peso Cubado; sempre em quilogramas; 3
+                - Quantidade de volumes, sempre em unidades
+                (obrigatório); 4 - Cubagem, sempre em metros cúbicos
+                (obrigatório apenas quando for impossível preencher as
+                dimensões da(s) embalagem(ens) na tag xDime do leiaute
+                do Aéreo).
+            :ivar vCargaAverb: Valor da Carga para efeito de averbação
+                Normalmente igual ao valor declarado da mercadoria,
+                diferente por exemplo, quando a mercadoria transportada
+                é isenta de tributos nacionais para exportação, onde é
+                preciso averbar um valor maior, pois no caso de
+                indenização, o valor a ser pago será maior
+            """
+
+            vCarga: Optional[str] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "required": True,
+                    "white_space": "preserve",
+                    "pattern": r"0|0\.[0-9]{2}|[1-9]{1}[0-9]{0,12}(\.[0-9]{2})?",
+                },
+            )
+            proPred: Optional[str] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "required": True,
+                    "min_length": 1,
+                    "max_length": 60,
+                    "white_space": "preserve",
+                    "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
+                },
+            )
+            xOutCat: Optional[str] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "min_length": 1,
+                    "max_length": 30,
+                    "white_space": "preserve",
+                    "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
+                },
+            )
+            infQ: List["TcteSimp.InfCte.InfCarga.InfQ"] = field(
+                default_factory=list,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "min_occurs": 1,
+                },
+            )
+            vCargaAverb: Optional[str] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "white_space": "preserve",
+                    "pattern": r"0\.[0-9]{1}[1-9]{1}|0\.[1-9]{1}[0-9]{1}|[1-9]{1}[0-9]{0,12}(\.[0-9]{2})?",
+                },
+            )
+
+            @dataclass
+            class InfQ(CommonMixin):
+                """
+                :ivar cUnid: Código da Unidade de Medida Preencher com:
+                    00-M3; 01-KG; 02-TON; 03-UNIDADE; 04-LITROS;
+                    05-MMBTU
+                :ivar tpMed: Tipo da Medida Informar com: 00-Cubagem da
+                    NF-e 01-Cubagem Aferida pelo Transportador 02-Peso
+                    Bruto da NF-e 03-Peso Bruto Aferido pelo
+                    Transportador 04-Peso Cubado 05-Peso Base do Cálculo
+                    do Frete 06-Peso para uso Operacional 07-Caixas
+                    08-Paletes 09-Sacas 10-Containers 11-Rolos
+                    12-Bombonas 13-Latas 14-Litragem 15-Milhão de BTU
+                    (British Thermal Units) 99-Outros
+                :ivar qCarga: Quantidade
+                """
+
+                cUnid: Optional[InfQCUnid] = field(
+                    default=None,
+                    metadata={
+                        "type": "Element",
+                        "namespace": "http://www.portalfiscal.inf.br/cte",
+                        "required": True,
+                        "white_space": "preserve",
+                    },
+                )
+                tpMed: Optional[InfQTpMed] = field(
+                    default=None,
+                    metadata={
+                        "type": "Element",
+                        "namespace": "http://www.portalfiscal.inf.br/cte",
+                        "required": True,
+                    },
+                )
+                qCarga: Optional[str] = field(
+                    default=None,
+                    metadata={
+                        "type": "Element",
+                        "namespace": "http://www.portalfiscal.inf.br/cte",
+                        "required": True,
+                        "white_space": "preserve",
+                        "pattern": r"0|0\.[0-9]{4}|[1-9]{1}[0-9]{0,10}(\.[0-9]{4})?",
+                    },
+                )
+
+        @dataclass
+        class Det(CommonMixin):
+            """
+            :ivar cMunIni: Código do Município de início da prestação
+                Utilizar a tabela do IBGE. Informar 9999999 para
+                operações com o exterior.
+            :ivar xMunIni: Nome do Município do início da prestação
+                Informar 'EXTERIOR' para operações com o exterior.
+            :ivar cMunFim: Código do Município de término da prestação
+                Utilizar a tabela do IBGE. Informar 9999999 para
+                operações com o exterior.
+            :ivar xMunFim: Nome do Município do término da prestação
+                Informar 'EXTERIOR' para operações com o exterior.
+            :ivar vPrest: Valorl da Prestação do Serviço Pode conter
+                zeros quando o CT-e for de complemento de ICMS
+            :ivar vRec: Valor a Receber
+            :ivar comp: Componentes do Valor da Prestação
+            :ivar infNFe: Informações das NF-e
+            :ivar infDocAnt: Documentos anteriores
+            :ivar nItem: Número identificador do item agrupador da
+                prestação
+            """
+
+            cMunIni: Optional[str] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "required": True,
+                    "white_space": "preserve",
+                    "pattern": r"[0-9]{7}",
+                },
+            )
+            xMunIni: Optional[str] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "required": True,
+                    "min_length": 2,
+                    "max_length": 60,
+                    "white_space": "preserve",
+                    "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
+                },
+            )
+            cMunFim: Optional[str] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "required": True,
+                    "white_space": "preserve",
+                    "pattern": r"[0-9]{7}",
+                },
+            )
+            xMunFim: Optional[str] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "required": True,
+                    "min_length": 2,
+                    "max_length": 60,
+                    "white_space": "preserve",
+                    "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
+                },
+            )
+            vPrest: Optional[str] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "required": True,
+                    "white_space": "preserve",
+                    "pattern": r"0|0\.[0-9]{2}|[1-9]{1}[0-9]{0,12}(\.[0-9]{2})?",
+                },
+            )
+            vRec: Optional[str] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "required": True,
+                    "white_space": "preserve",
+                    "pattern": r"0|0\.[0-9]{2}|[1-9]{1}[0-9]{0,12}(\.[0-9]{2})?",
+                },
+            )
+            comp: List["TcteSimp.InfCte.Det.Comp"] = field(
+                default_factory=list,
+                metadata={
+                    "name": "Comp",
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                },
+            )
+            infNFe: List["TcteSimp.InfCte.Det.InfNfe"] = field(
+                default_factory=list,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                },
+            )
+            infDocAnt: List["TcteSimp.InfCte.Det.InfDocAnt"] = field(
+                default_factory=list,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                },
+            )
+            nItem: Optional[str] = field(
+                default=None,
+                metadata={
+                    "type": "Attribute",
+                    "required": True,
+                    "white_space": "preserve",
+                    "pattern": r"[1-9]{1}[0-9]{0,1}|[1-8]{1}[0-9]{2}|[9]{1}[0-8]{1}[0-9]{1}|[9]{1}[9]{1}[0]{1}",
+                },
+            )
+
+            @dataclass
+            class Comp(CommonMixin):
+                """
+                :ivar xNome: Nome do componente Exxemplos: FRETE PESO,
+                    FRETE VALOR, SEC/CAT, ADEME, AGENDAMENTO, etc
+                :ivar vComp: Valor do componente
+                """
+
+                xNome: Optional[str] = field(
+                    default=None,
+                    metadata={
+                        "type": "Element",
+                        "namespace": "http://www.portalfiscal.inf.br/cte",
+                        "required": True,
+                        "min_length": 1,
+                        "max_length": 15,
+                        "white_space": "preserve",
+                        "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
+                    },
+                )
+                vComp: Optional[str] = field(
+                    default=None,
+                    metadata={
+                        "type": "Element",
+                        "namespace": "http://www.portalfiscal.inf.br/cte",
+                        "required": True,
+                        "white_space": "preserve",
+                        "pattern": r"0|0\.[0-9]{2}|[1-9]{1}[0-9]{0,12}(\.[0-9]{2})?",
+                    },
+                )
+
+            @dataclass
+            class InfNfe(CommonMixin):
+                """
+                :ivar chNFe: Chave de acesso da NF-e
+                :ivar PIN: PIN SUFRAMA PIN atribuído pela SUFRAMA para a
+                    operação.
+                :ivar dPrev: Data prevista de entrega Formato AAAA-MM-DD
+                :ivar infUnidCarga: Informações das Unidades de Carga
+                    (Containeres/ULD/Outros) Dispositivo de carga
+                    utilizada (Unit Load Device - ULD) significa todo
+                    tipo de contêiner de carga, vagão, contêiner de
+                    avião, palete de aeronave com rede ou palete de
+                    aeronave com rede sobre um iglu.
+                :ivar infUnidTransp: Informações das Unidades de
+                    Transporte (Carreta/Reboque/Vagão) Deve ser
+                    preenchido com as informações das unidades de
+                    transporte utilizadas.
+                """
+
+                chNFe: Optional[str] = field(
+                    default=None,
+                    metadata={
+                        "type": "Element",
+                        "namespace": "http://www.portalfiscal.inf.br/cte",
+                        "required": True,
+                        "max_length": 44,
+                        "white_space": "preserve",
+                        "pattern": r"[0-9]{44}",
+                    },
+                )
+                PIN: Optional[str] = field(
+                    default=None,
+                    metadata={
+                        "type": "Element",
+                        "namespace": "http://www.portalfiscal.inf.br/cte",
+                        "min_length": 2,
+                        "max_length": 9,
+                        "white_space": "preserve",
+                        "pattern": r"[1-9]{1}[0-9]{1,8}",
+                    },
+                )
+                dPrev: Optional[str] = field(
+                    default=None,
+                    metadata={
+                        "type": "Element",
+                        "namespace": "http://www.portalfiscal.inf.br/cte",
+                        "white_space": "preserve",
+                        "pattern": r"(((20(([02468][048])|([13579][26]))-02-29))|(20[0-9][0-9])-((((0[1-9])|(1[0-2]))-((0[1-9])|(1\d)|(2[0-8])))|((((0[13578])|(1[02]))-31)|(((0[1,3-9])|(1[0-2]))-(29|30)))))",
+                    },
+                )
+                infUnidCarga: List[TunidCarga] = field(
+                    default_factory=list,
+                    metadata={
+                        "type": "Element",
+                        "namespace": "http://www.portalfiscal.inf.br/cte",
+                    },
+                )
+                infUnidTransp: List[TunidadeTransp] = field(
+                    default_factory=list,
+                    metadata={
+                        "type": "Element",
+                        "namespace": "http://www.portalfiscal.inf.br/cte",
+                    },
+                )
+
+            @dataclass
+            class InfDocAnt(CommonMixin):
+                """
+                :ivar chCTe: Chave de acesso do CT-e
+                :ivar tpPrest: indica se a prestação é total ou parcial
+                    em relação as notas do documento anterior Preencher
+                    com: 1 - Total 2 - Parcial
+                :ivar infNFeTranspParcial:
+                """
+
+                chCTe: Optional[str] = field(
+                    default=None,
+                    metadata={
+                        "type": "Element",
+                        "namespace": "http://www.portalfiscal.inf.br/cte",
+                        "required": True,
+                        "max_length": 44,
+                        "white_space": "preserve",
+                        "pattern": r"[0-9]{44}",
+                    },
+                )
+                tpPrest: Optional[InfDocAntTpPrest] = field(
+                    default=None,
+                    metadata={
+                        "type": "Element",
+                        "namespace": "http://www.portalfiscal.inf.br/cte",
+                        "required": True,
+                        "white_space": "preserve",
+                    },
+                )
+                infNFeTranspParcial: List[
+                    "TcteSimp.InfCte.Det.InfDocAnt.InfNfeTranspParcial"
+                ] = field(
+                    default_factory=list,
+                    metadata={
+                        "type": "Element",
+                        "namespace": "http://www.portalfiscal.inf.br/cte",
+                    },
+                )
+
+                @dataclass
+                class InfNfeTranspParcial(CommonMixin):
+                    """
+                    :ivar chNFe: Chave de acesso da NF-e Informando o
+                        tpPrest com “2 – Parcial” deve-se informar as
+                        chaves de acesso das NF-e que acobertam a carga
+                        transportada.
+                    """
+
+                    chNFe: Optional[str] = field(
+                        default=None,
+                        metadata={
+                            "type": "Element",
+                            "namespace": "http://www.portalfiscal.inf.br/cte",
+                            "required": True,
+                            "max_length": 44,
+                            "white_space": "preserve",
+                            "pattern": r"[0-9]{44}",
+                        },
+                    )
+
+        @dataclass
+        class InfModal(CommonMixin):
+            """
+            :ivar any_element: XML do modal Insira neste local o XML
+                específico do modal (rodoviário, aéreo, ferroviário,
+                aquaviário ou dutoviário). O elemento do tipo -any-
+                permite estender o documento XML com elementos não
+                especificados pelo schema. Insira neste local - any- o
+                XML específico do modal (rodoviário, aéreo, ferroviário,
+                aquaviário ou dutoviário). A especificação do schema XML
+                para cada modal pode ser encontrada nos arquivos que
+                acompanham este pacote de liberação: Rodoviário - ver
+                arquivo CTeModalRodoviario_v9.99 Aéreo - ver arquivo
+                CTeModalAereo_v9.99 Aquaviário - arquivo
+                CTeModalAquaviario_v9.99 Ferroviário - arquivo
+                CTeModalFerroviario_v9.99 Dutoviário - arquivo
+                CTeModalDutoviario_v9.99 Onde v9.99 é a a designação
+                genérica para a versão do arquivo. Por exemplo, o
+                arquivo para o schema do modal Rodoviário na versão 1.04
+                será denominado "CTeModalRodoviario_v1.04".
+            :ivar versaoModal: Versão do leiaute específico para o Modal
+            """
+
+            any_element: Optional[object] = field(
+                default=None,
+                metadata={
+                    "type": "Wildcard",
+                    "namespace": "##any",
+                    "process_contents": "skip",
+                },
+            )
+            versaoModal: Optional[str] = field(
+                default=None,
+                metadata={
+                    "type": "Attribute",
+                    "required": True,
+                    "white_space": "preserve",
+                    "pattern": r"4\.(0[0-9]|[1-9][0-9])",
+                },
+            )
+
+        @dataclass
+        class Cobr(CommonMixin):
+            """
+            :ivar fat: Dados da fatura
+            :ivar dup: Dados das duplicatas
+            """
+
+            fat: Optional["TcteSimp.InfCte.Cobr.Fat"] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                },
+            )
+            dup: List["TcteSimp.InfCte.Cobr.Dup"] = field(
+                default_factory=list,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                },
+            )
+
+            @dataclass
+            class Fat(CommonMixin):
+                """
+                :ivar nFat: Número da fatura
+                :ivar vOrig: Valor original da fatura
+                :ivar vDesc: Valor do desconto da fatura
+                :ivar vLiq: Valor líquido da fatura
+                """
+
+                nFat: Optional[str] = field(
+                    default=None,
+                    metadata={
+                        "type": "Element",
+                        "namespace": "http://www.portalfiscal.inf.br/cte",
+                        "min_length": 1,
+                        "max_length": 60,
+                        "white_space": "preserve",
+                        "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
+                    },
+                )
+                vOrig: Optional[str] = field(
+                    default=None,
+                    metadata={
+                        "type": "Element",
+                        "namespace": "http://www.portalfiscal.inf.br/cte",
+                        "white_space": "preserve",
+                        "pattern": r"0\.[0-9]{1}[1-9]{1}|0\.[1-9]{1}[0-9]{1}|[1-9]{1}[0-9]{0,12}(\.[0-9]{2})?",
+                    },
+                )
+                vDesc: Optional[str] = field(
+                    default=None,
+                    metadata={
+                        "type": "Element",
+                        "namespace": "http://www.portalfiscal.inf.br/cte",
+                        "white_space": "preserve",
+                        "pattern": r"0\.[0-9]{1}[1-9]{1}|0\.[1-9]{1}[0-9]{1}|[1-9]{1}[0-9]{0,12}(\.[0-9]{2})?",
+                    },
+                )
+                vLiq: Optional[str] = field(
+                    default=None,
+                    metadata={
+                        "type": "Element",
+                        "namespace": "http://www.portalfiscal.inf.br/cte",
+                        "white_space": "preserve",
+                        "pattern": r"0\.[0-9]{1}[1-9]{1}|0\.[1-9]{1}[0-9]{1}|[1-9]{1}[0-9]{0,12}(\.[0-9]{2})?",
+                    },
+                )
+
+            @dataclass
+            class Dup(CommonMixin):
+                """
+                :ivar nDup: Número da duplicata
+                :ivar dVenc: Data de vencimento da duplicata (AAAA-MM-
+                    DD)
+                :ivar vDup: Valor da duplicata
+                """
+
+                nDup: Optional[str] = field(
+                    default=None,
+                    metadata={
+                        "type": "Element",
+                        "namespace": "http://www.portalfiscal.inf.br/cte",
+                        "min_length": 1,
+                        "max_length": 60,
+                        "white_space": "preserve",
+                        "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
+                    },
+                )
+                dVenc: Optional[str] = field(
+                    default=None,
+                    metadata={
+                        "type": "Element",
+                        "namespace": "http://www.portalfiscal.inf.br/cte",
+                        "white_space": "preserve",
+                        "pattern": r"(((20(([02468][048])|([13579][26]))-02-29))|(20[0-9][0-9])-((((0[1-9])|(1[0-2]))-((0[1-9])|(1\d)|(2[0-8])))|((((0[13578])|(1[02]))-31)|(((0[1,3-9])|(1[0-2]))-(29|30)))))",
+                    },
+                )
+                vDup: Optional[str] = field(
+                    default=None,
+                    metadata={
+                        "type": "Element",
+                        "namespace": "http://www.portalfiscal.inf.br/cte",
+                        "white_space": "preserve",
+                        "pattern": r"0\.[0-9]{1}[1-9]{1}|0\.[1-9]{1}[0-9]{1}|[1-9]{1}[0-9]{0,12}(\.[0-9]{2})?",
+                    },
+                )
+
+        @dataclass
+        class InfCteSub(CommonMixin):
+            """
+            :ivar chCte: Chave de acesso do CT-e a ser substituído
+                (original)
+            :ivar indAlteraToma: Indicador de CT-e Alteração de Tomador
+            """
+
+            chCte: Optional[str] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "required": True,
+                    "pattern": r"[0-9]{44}",
+                },
+            )
+            indAlteraToma: Optional[InfCteSubIndAlteraToma] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                },
+            )
+
+        @dataclass
+        class Imp(CommonMixin):
+            """
+            :ivar ICMS: Informações relativas ao ICMS
+            :ivar vTotTrib: Valor Total dos Tributos
+            :ivar infAdFisco: Informações adicionais de interesse do
+                Fisco Norma referenciada, informações complementares,
+                etc
+            :ivar ICMSUFFim: Informações do ICMS de partilha com a UF de
+                término do serviço de transporte na operação
+                interestadual Grupo a ser informado nas prestações
+                interestaduais para consumidor final, não contribuinte
+                do ICMS
+            """
+
+            ICMS: Optional[Timp] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "required": True,
+                },
+            )
+            vTotTrib: Optional[str] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "white_space": "preserve",
+                    "pattern": r"0|0\.[0-9]{2}|[1-9]{1}[0-9]{0,12}(\.[0-9]{2})?",
+                },
+            )
+            infAdFisco: Optional[str] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "min_length": 1,
+                    "max_length": 2000,
+                    "white_space": "preserve",
+                    "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
+                },
+            )
+            ICMSUFFim: Optional["TcteSimp.InfCte.Imp.Icmsuffim"] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                },
+            )
+
+            @dataclass
+            class Icmsuffim(CommonMixin):
+                """
+                :ivar vBCUFFim: Valor da BC do ICMS na UF de término da
+                    prestação do serviço de transporte
+                :ivar pFCPUFFim: Percentual do ICMS relativo ao Fundo de
+                    Combate à pobreza (FCP) na UF de término da
+                    prestação do serviço de transporte Alíquota adotada
+                    nas operações internas na UF do destinatário
+                :ivar pICMSUFFim: Alíquota interna da UF de término da
+                    prestação do serviço de transporte Alíquota adotada
+                    nas operações internas na UF do destinatário
+                :ivar pICMSInter: Alíquota interestadual das UF
+                    envolvidas Alíquota interestadual das UF envolvidas
+                :ivar vFCPUFFim: Valor do ICMS relativo ao Fundo de
+                    Combate á Pobreza (FCP) da UF de término da
+                    prestação
+                :ivar vICMSUFFim: Valor do ICMS de partilha para a UF de
+                    término da prestação do serviço de transporte
+                :ivar vICMSUFIni: Valor do ICMS de partilha para a UF de
+                    início da prestação do serviço de transporte
+                """
+
+                vBCUFFim: Optional[str] = field(
+                    default=None,
+                    metadata={
+                        "type": "Element",
+                        "namespace": "http://www.portalfiscal.inf.br/cte",
+                        "required": True,
+                        "white_space": "preserve",
+                        "pattern": r"0|0\.[0-9]{2}|[1-9]{1}[0-9]{0,12}(\.[0-9]{2})?",
+                    },
+                )
+                pFCPUFFim: Optional[str] = field(
+                    default=None,
+                    metadata={
+                        "type": "Element",
+                        "namespace": "http://www.portalfiscal.inf.br/cte",
+                        "required": True,
+                        "white_space": "preserve",
+                        "pattern": r"0|0\.[0-9]{2}|[1-9]{1}[0-9]{0,2}(\.[0-9]{2})?",
+                    },
+                )
+                pICMSUFFim: Optional[str] = field(
+                    default=None,
+                    metadata={
+                        "type": "Element",
+                        "namespace": "http://www.portalfiscal.inf.br/cte",
+                        "required": True,
+                        "white_space": "preserve",
+                        "pattern": r"0|0\.[0-9]{2}|[1-9]{1}[0-9]{0,2}(\.[0-9]{2})?",
+                    },
+                )
+                pICMSInter: Optional[str] = field(
+                    default=None,
+                    metadata={
+                        "type": "Element",
+                        "namespace": "http://www.portalfiscal.inf.br/cte",
+                        "required": True,
+                        "white_space": "preserve",
+                        "pattern": r"0|0\.[0-9]{2}|[1-9]{1}[0-9]{0,2}(\.[0-9]{2})?",
+                    },
+                )
+                vFCPUFFim: Optional[str] = field(
+                    default=None,
+                    metadata={
+                        "type": "Element",
+                        "namespace": "http://www.portalfiscal.inf.br/cte",
+                        "required": True,
+                        "white_space": "preserve",
+                        "pattern": r"0|0\.[0-9]{2}|[1-9]{1}[0-9]{0,12}(\.[0-9]{2})?",
+                    },
+                )
+                vICMSUFFim: Optional[str] = field(
+                    default=None,
+                    metadata={
+                        "type": "Element",
+                        "namespace": "http://www.portalfiscal.inf.br/cte",
+                        "required": True,
+                        "white_space": "preserve",
+                        "pattern": r"0|0\.[0-9]{2}|[1-9]{1}[0-9]{0,12}(\.[0-9]{2})?",
+                    },
+                )
+                vICMSUFIni: Optional[str] = field(
+                    default=None,
+                    metadata={
+                        "type": "Element",
+                        "namespace": "http://www.portalfiscal.inf.br/cte",
+                        "required": True,
+                        "white_space": "preserve",
+                        "pattern": r"0|0\.[0-9]{2}|[1-9]{1}[0-9]{0,12}(\.[0-9]{2})?",
+                    },
+                )
+
+        @dataclass
+        class Total(CommonMixin):
+            """
+            :ivar vTPrest: Valor Total da Prestação do Serviço Pode
+                conter zeros quando o CT-e for de complemento de ICMS
+            :ivar vTRec: Valor total a Receber
+            """
+
+            vTPrest: Optional[str] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "required": True,
+                    "white_space": "preserve",
+                    "pattern": r"0|0\.[0-9]{2}|[1-9]{1}[0-9]{0,12}(\.[0-9]{2})?",
+                },
+            )
+            vTRec: Optional[str] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "required": True,
+                    "white_space": "preserve",
+                    "pattern": r"0|0\.[0-9]{2}|[1-9]{1}[0-9]{0,12}(\.[0-9]{2})?",
+                },
+            )
+
+        @dataclass
+        class AutXml(CommonMixin):
+            """
+            :ivar CNPJ: CNPJ do autorizado Informar zeros não
+                significativos
+            :ivar CPF: CPF do autorizado Informar zeros não
+                significativos
+            """
+
+            CNPJ: Optional[str] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "white_space": "preserve",
+                    "pattern": r"[0-9]{14}",
+                },
+            )
+            CPF: Optional[str] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "white_space": "preserve",
+                    "pattern": r"[0-9]{11}",
+                },
+            )
+
+        @dataclass
+        class InfSolicNff(CommonMixin):
+            """
+            :ivar xSolic: Solicitação do pedido de emissão da NFF. Será
+                preenchido com a totalidade de campos informados no
+                aplicativo emissor serializado.
+            """
+
+            xSolic: Optional[str] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "required": True,
+                    "min_length": 2,
+                    "max_length": 2000,
+                    "white_space": "preserve",
+                    "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
+                },
+            )
+
+        @dataclass
+        class InfPaa(CommonMixin):
+            """
+            :ivar CNPJPAA: CNPJ do Provedor de Assinatura e Autorização
+            :ivar PAASignature: Assinatura RSA do Emitente para DFe
+                gerados por PAA
+            """
+
+            CNPJPAA: Optional[str] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "required": True,
+                    "white_space": "preserve",
+                    "pattern": r"[0-9]{14}",
+                },
+            )
+            PAASignature: Optional[
+                "TcteSimp.InfCte.InfPaa.Paasignature"
+            ] = field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.portalfiscal.inf.br/cte",
+                    "required": True,
+                },
+            )
+
+            @dataclass
+            class Paasignature(CommonMixin):
+                """
+                :ivar signatureValue: Assinatura digital padrão RSA
+                    Converter o atributo Id do DFe para array de bytes e
+                    assinar com a chave privada do RSA com algoritmo
+                    SHA1 gerando um valor no formato base64.
+                :ivar RSAKeyValue: Chave Publica no padrão XML RSA Key
+                """
+
+                signatureValue: Optional[bytes] = field(
+                    default=None,
+                    metadata={
+                        "name": "SignatureValue",
+                        "type": "Element",
+                        "namespace": "http://www.portalfiscal.inf.br/cte",
+                        "required": True,
+                        "format": "base64",
+                    },
+                )
+                RSAKeyValue: Optional[TrsakeyValueType] = field(
+                    default=None,
+                    metadata={
+                        "type": "Element",
+                        "namespace": "http://www.portalfiscal.inf.br/cte",
+                        "required": True,
+                    },
+                )
+
+    @dataclass
+    class InfCteSupl(CommonMixin):
+        """
+        :ivar qrCodCTe: Texto com o QR-Code impresso no DACTE
+        """
+
         qrCodCTe: Optional[str] = field(
             default=None,
             metadata={
                 "type": "Element",
                 "namespace": "http://www.portalfiscal.inf.br/cte",
                 "required": True,
                 "min_length": 50,
```

## Comparing `nfelib-2.0.4/nfelib/cte/bindings/v4_0/evento_cte_v4_00.py` & `nfelib-2.0.5/nfelib/cte/bindings/v4_0/evento_cte_v4_00.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:16:35
+"""This file was generated by xsdata, v24.4, on 2024-04-08 21:52:20
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass
+
 from nfelib.cte.bindings.v4_0.evento_cte_tipos_basico_v4_00 import Tevento
 
 __NAMESPACE__ = "http://www.portalfiscal.inf.br/cte"
 
 
 @dataclass
 class EventoCte(Tevento):
```

## Comparing `nfelib-2.0.4/nfelib/cte/bindings/v4_0/ret_evento_cte_v4_00.py` & `nfelib-2.0.5/nfelib/cte/bindings/v4_0/ret_evento_cte_v4_00.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:16:35
+"""This file was generated by xsdata, v24.4, on 2024-04-08 21:52:20
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass
+
 from nfelib.cte.bindings.v4_0.evento_cte_tipos_basico_v4_00 import TretEvento
 
 __NAMESPACE__ = "http://www.portalfiscal.inf.br/cte"
 
 
 @dataclass
 class RetEventoCte(TretEvento):
```

## Comparing `nfelib-2.0.4/nfelib/cte/bindings/v4_0/ev_cecte_v4_00.py` & `nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_cecte_v4_00.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:16:35
+"""This file was generated by xsdata, v24.4, on 2024-04-08 21:52:20
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass, field
 from enum import Enum
-from nfelib import CommonMixin
 from typing import List, Optional
 
+from nfelib import CommonMixin
+
 __NAMESPACE__ = "http://www.portalfiscal.inf.br/cte"
 
 
 class EvCecteDescEvento(Enum):
     COMPROVANTE_DE_ENTREGA_DO_CT_E = "Comprovante de Entrega do CT-e"
```

## Comparing `nfelib-2.0.4/nfelib/cte/bindings/v4_0/ret_cte_v4_00.py` & `nfelib-2.0.5/nfelib/cte/bindings/v4_0/ret_cte_os_v4_00.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:16:35
+"""This file was generated by xsdata, v24.4, on 2024-04-08 21:52:20
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass
-from nfelib.cte.bindings.v4_0.cte_tipos_basico_v4_00 import TretCte
+
+from nfelib.cte.bindings.v4_0.cte_tipos_basico_v4_00 import TretCteOs
 
 __NAMESPACE__ = "http://www.portalfiscal.inf.br/cte"
 
 
 @dataclass
-class RetCte(TretCte):
+class RetCteOs(TretCteOs):
     """
-    Schema XML de validação do retorno do recibo de envio do CT-e (Modelo 57)
+    Schema XML de validação do retorno do recibo de envio do CT-e OS (Modelo 67)
     """
 
     class Meta:
-        name = "retCTe"
+        name = "retCTeOS"
         namespace = "http://www.portalfiscal.inf.br/cte"
```

## Comparing `nfelib-2.0.4/nfelib/cte/bindings/v4_0/cons_stat_serv_cte_v4_00.py` & `nfelib-2.0.5/nfelib/cte/bindings/v4_0/cons_stat_serv_cte_v4_00.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:16:35
+"""This file was generated by xsdata, v24.4, on 2024-04-08 21:52:20
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass
+
 from nfelib.cte.bindings.v4_0.cons_stat_serv_tipos_basico_v4_00 import (
     TconsStatServ,
 )
 
 __NAMESPACE__ = "http://www.portalfiscal.inf.br/cte"
```

## Comparing `nfelib-2.0.4/nfelib/cte/bindings/v4_0/ret_cte_os_v4_00.py` & `nfelib-2.0.5/nfelib/nfe_evento_generico/bindings/v1_0/ret_env_evento_v1_00.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:16:35
+"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:16:22
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass
-from nfelib.cte.bindings.v4_0.cte_tipos_basico_v4_00 import TretCteOs
+from nfelib.nfe_evento_generico.bindings.v1_0.leiaute_evento_v1_00 import (
+    TretEnvEvento,
+)
 
-__NAMESPACE__ = "http://www.portalfiscal.inf.br/cte"
+__NAMESPACE__ = "http://www.portalfiscal.inf.br/nfe"
 
 
 @dataclass
-class RetCteOs(TretCteOs):
+class RetEnvEvento(TretEnvEvento):
     """
-    Schema XML de validação do retorno do recibo de envio do CT-e OS (Modelo 67)
+    Schema XML de Retorno da envio do Evento.
     """
 
     class Meta:
-        name = "retCTeOS"
-        namespace = "http://www.portalfiscal.inf.br/cte"
+        name = "retEnvEvento"
+        namespace = "http://www.portalfiscal.inf.br/nfe"
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## Comparing `nfelib-2.0.4/nfelib/cte/bindings/v4_0/cons_sit_cte_tipos_basico_v4_00.py` & `nfelib-2.0.5/nfelib/cte/bindings/v4_0/cons_sit_cte_tipos_basico_v4_00.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:16:35
+"""This file was generated by xsdata, v24.4, on 2024-04-08 21:52:20
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass, field
 from enum import Enum
-from nfelib import CommonMixin
 from typing import List, Optional
+
+from nfelib import CommonMixin
 from nfelib.cte.bindings.v4_0.tipos_geral_cte_v4_00 import (
     Tamb,
     TcodUfIbge,
 )
 
 __NAMESPACE__ = "http://www.portalfiscal.inf.br/cte"
```

## Comparing `nfelib-2.0.4/nfelib/cte/bindings/v4_0/ev_canc_iecte_v4_00.py` & `nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_canc_iecte_v4_00.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:16:35
+"""This file was generated by xsdata, v24.4, on 2024-04-08 21:52:20
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass, field
 from enum import Enum
-from nfelib import CommonMixin
 from typing import Optional
 
+from nfelib import CommonMixin
+
 __NAMESPACE__ = "http://www.portalfiscal.inf.br/cte"
 
 
 class EvCancIecteDescEvento(Enum):
     CANCELAMENTO_DO_INSUCESSO_DE_ENTREGA_DO_CT_E = (
         "Cancelamento do Insucesso de Entrega do CT-e"
     )
```

## Comparing `nfelib-2.0.4/nfelib/cte/bindings/v4_0/cons_sit_cte_v4_00.py` & `nfelib-2.0.5/nfelib/nfe/bindings/v4_0/envi_nfe_v4_00.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:16:35
+"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:31:20
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass
-from nfelib.cte.bindings.v4_0.cons_sit_cte_tipos_basico_v4_00 import (
-    TconsSitCte,
-)
+from nfelib.nfe.bindings.v4_0.leiaute_nfe_v4_00 import TenviNfe
 
-__NAMESPACE__ = "http://www.portalfiscal.inf.br/cte"
+__NAMESPACE__ = "http://www.portalfiscal.inf.br/nfe"
 
 
 @dataclass
-class ConsSitCte(TconsSitCte):
+class EnviNfe(TenviNfe):
     """
-    Schema de validação XML dp Pedido de Consulta da Situação Atual do CT-e.
+    Schema XML de validação do Pedido de Concessão de Autorização da Nota Fiscal
+    Eletrônica.
     """
 
     class Meta:
-        name = "consSitCTe"
-        namespace = "http://www.portalfiscal.inf.br/cte"
+        name = "enviNFe"
+        namespace = "http://www.portalfiscal.inf.br/nfe"
```

## Comparing `nfelib-2.0.4/nfelib/cte/bindings/v4_0/ev_canc_cecte_v4_00.py` & `nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_canc_cecte_v4_00.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:16:35
+"""This file was generated by xsdata, v24.4, on 2024-04-08 21:52:20
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass, field
 from enum import Enum
-from nfelib import CommonMixin
 from typing import Optional
 
+from nfelib import CommonMixin
+
 __NAMESPACE__ = "http://www.portalfiscal.inf.br/cte"
 
 
 class EvCancCecteDescEvento(Enum):
     CANCELAMENTO_DO_COMPROVANTE_DE_ENTREGA_DO_CT_E = (
         "Cancelamento do Comprovante de Entrega do CT-e"
     )
```

## Comparing `nfelib-2.0.4/nfelib/cte/bindings/v4_0/inut_cte_v4_00.py` & `nfelib-2.0.5/nfelib/cte/bindings/v4_0/inut_cte_v4_00.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:16:35
+"""This file was generated by xsdata, v24.4, on 2024-04-08 21:52:20
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass
+
 from nfelib.cte.bindings.v4_0.inut_cte_tipos_basico_v4_00 import TinutCte
 
 __NAMESPACE__ = "http://www.portalfiscal.inf.br/cte"
 
 
 @dataclass
 class InutCte(TinutCte):
```

## Comparing `nfelib-2.0.4/nfelib/cte/bindings/v4_0/inut_cte_tipos_basico_v4_00.py` & `nfelib-2.0.5/nfelib/cte/bindings/v4_0/inut_cte_tipos_basico_v4_00.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:16:35
+"""This file was generated by xsdata, v24.4, on 2024-04-08 21:52:20
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass, field
-from nfelib import CommonMixin
 from typing import Optional
+
+from nfelib import CommonMixin
 from nfelib.cte.bindings.v4_0.tipos_geral_cte_v4_00 import (
     Tamb,
     TcodUfIbge,
     TmodCtCargaOs,
 )
 from nfelib.cte.bindings.v4_0.xmldsig_core_schema_v1_01 import Signature
```

## Comparing `nfelib-2.0.4/nfelib/cte/bindings/v4_0/proc_cte_os_v4_00.py` & `nfelib-2.0.5/nfelib/cte/bindings/v4_0/proc_cte_os_v4_00.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:16:35
+"""This file was generated by xsdata, v24.4, on 2024-04-08 21:52:20
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass, field
-from nfelib import CommonMixin
 from typing import Optional
+
+from nfelib import CommonMixin
 from nfelib.cte.bindings.v4_0.cte_tipos_basico_v4_00 import (
     TcteOs,
     TprotCteOs,
 )
 
 __NAMESPACE__ = "http://www.portalfiscal.inf.br/cte"
```

## Comparing `nfelib-2.0.4/nfelib/cte/bindings/v4_0/cte_modal_ferroviario_v4_00.py` & `nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_modal_ferroviario_v4_00.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:16:35
+"""This file was generated by xsdata, v24.4, on 2024-04-08 21:52:20
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass, field
 from enum import Enum
-from nfelib import CommonMixin
 from typing import List, Optional
+
+from nfelib import CommonMixin
 from nfelib.cte.bindings.v4_0.tipos_geral_cte_v4_00 import Tuf
 
 __NAMESPACE__ = "http://www.portalfiscal.inf.br/cte"
 
 
 class FerrovTpTraf(Enum):
     VALUE_0 = "0"
```

## Comparing `nfelib-2.0.4/nfelib/cte/bindings/v4_0/cte_modal_aereo_v4_00.py` & `nfelib-2.0.5/nfelib/cte/bindings/v4_0/cte_modal_aereo_v4_00.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:16:35
+"""This file was generated by xsdata, v24.4, on 2024-04-08 21:52:20
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass, field
 from enum import Enum
-from nfelib import CommonMixin
 from typing import List, Optional
 
+from nfelib import CommonMixin
+
 __NAMESPACE__ = "http://www.portalfiscal.inf.br/cte"
 
 
 class InfTotApUniAp(Enum):
     VALUE_1 = "1"
     VALUE_2 = "2"
     VALUE_3 = "3"
```

## Comparing `nfelib-2.0.4/nfelib/cte/bindings/v4_0/ev_prest_desacordo_v4_00.py` & `nfelib-2.0.5/nfelib/cte/bindings/v4_0/ev_canc_prest_desacordo_v4_00.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,63 +1,57 @@
-"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:16:35
+"""This file was generated by xsdata, v24.4, on 2024-04-08 21:52:20
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass, field
 from enum import Enum
-from nfelib import CommonMixin
 from typing import Optional
 
-__NAMESPACE__ = "http://www.portalfiscal.inf.br/cte"
-
+from nfelib import CommonMixin
 
-class EvPrestDesacordoDescEvento(Enum):
-    PRESTA_O_DO_SERVI_O_EM_DESACORDO = "Prestação do Serviço em Desacordo"
-    PRESTACAO_DO_SERVICO_EM_DESACORDO = "Prestacao do Servico em Desacordo"
+__NAMESPACE__ = "http://www.portalfiscal.inf.br/cte"
 
 
-class EvPrestDesacordoIndDesacordoOper(Enum):
-    VALUE_1 = "1"
+class EvCancPrestDesacordoDescEvento(Enum):
+    CANCELAMENTO_PRESTA_O_DO_SERVI_O_EM_DESACORDO = (
+        "Cancelamento Prestação do Serviço em Desacordo"
+    )
+    CANCELAMENTO_PRESTACAO_DO_SERVICO_EM_DESACORDO = (
+        "Cancelamento Prestacao do Servico em Desacordo"
+    )
 
 
 @dataclass
-class EvPrestDesacordo(CommonMixin):
+class EvCancPrestDesacordo(CommonMixin):
     """
-    Schema XML de validação do evento Prestação do Serviço em Desacordo 610110.
+    Schema XML de validação do evento Cancelamento Prestação do Serviço em
+    Desacordo 610111.
 
-    :ivar descEvento: Descrição do Evento - “Prestação do Serviço em
-        Desacordo”
-    :ivar indDesacordoOper: Indicador de operação em desacordo
-    :ivar xObs: Observações do tomador
+    :ivar descEvento: Descrição do Evento - “Cancelamento Prestação do
+        Serviço em Desacordo”
+    :ivar nProtEvPrestDes: Protocolo do evento que será cancelado
+        Informar o número do protocolo de autorização do evento de
+        prestação de serviço em desacordo que será cancelado
     """
 
     class Meta:
-        name = "evPrestDesacordo"
+        name = "evCancPrestDesacordo"
         namespace = "http://www.portalfiscal.inf.br/cte"
 
-    descEvento: Optional[EvPrestDesacordoDescEvento] = field(
+    descEvento: Optional[EvCancPrestDesacordoDescEvento] = field(
         default=None,
         metadata={
             "type": "Element",
             "required": True,
             "white_space": "preserve",
         },
     )
-    indDesacordoOper: Optional[EvPrestDesacordoIndDesacordoOper] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-            "required": True,
-        },
-    )
-    xObs: Optional[str] = field(
+    nProtEvPrestDes: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "required": True,
-            "min_length": 15,
-            "max_length": 255,
             "white_space": "preserve",
-            "pattern": r"[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1}",
+            "pattern": r"[0-9]{15}",
         },
     )
```

## Comparing `nfelib-2.0.4/nfelib/cte/schemas/v4_0/cteModalRodoviario_v4.00.xsd` & `nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteModalRodoviario_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte/schemas/v4_0/cteTiposBasico_v4.00.xsd` & `nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteTiposBasico_v4.00.xsd`

 * *Files 7% similar despite different names*

### Comparing `nfelib-2.0.4/nfelib/cte/schemas/v4_0/cteTiposBasico_v4.00.xsd` & `nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteTiposBasico_v4.00.xsd`

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
-<!-- edited with XMLSpy v2008 (http://www.altova.com) by sas.softwares@procergs.rs.gov.br (PROCERGS) -->
+<!-- edited with XMLSpy v2014 rel. 2 (http://www.altova.com) by private (private) -->
 <xs:schema xmlns:ds="http://www.w3.org/2000/09/xmldsig#" xmlns:xs="http://www.w3.org/2001/XMLSchema" xmlns="http://www.portalfiscal.inf.br/cte" targetNamespace="http://www.portalfiscal.inf.br/cte" elementFormDefault="qualified" attributeFormDefault="unqualified">
   <xs:import namespace="http://www.w3.org/2000/09/xmldsig#" schemaLocation="xmldsig-core-schema_v1.01.xsd"/>
   <xs:include schemaLocation="tiposGeralCTe_v4.00.xsd"/>
   <xs:simpleType name="TModTranspGTVe">
     <xs:annotation>
       <xs:documentation>Tipo Modal transporte GTVe</xs:documentation>
     </xs:annotation>
@@ -1186,14 +1186,54 @@
     </xs:sequence>
     <xs:attribute name="versao" use="required">
       <xs:simpleType>
         <xs:restriction base="TVerCTe"/>
       </xs:simpleType>
     </xs:attribute>
   </xs:complexType>
+  <xs:complexType name="TRetCTeSimp">
+    <xs:annotation>
+      <xs:documentation>Tipo Retorno do Pedido de Autorização de CT-e Simplificado (Modelo 57)</xs:documentation>
+    </xs:annotation>
+    <xs:sequence>
+      <xs:element name="tpAmb" type="TAmb">
+        <xs:annotation>
+          <xs:documentation>Identificação do Ambiente:
+1 - Produção
+2 - Homologação</xs:documentation>
+        </xs:annotation>
+      </xs:element>
+      <xs:element name="cUF" type="TCodUfIBGE">
+        <xs:annotation>
+          <xs:documentation>Identificação da UF</xs:documentation>
+        </xs:annotation>
+      </xs:element>
+      <xs:element name="verAplic" type="TVerAplic">
+        <xs:annotation>
+          <xs:documentation>Versão do Aplicativo que processou a CT-e</xs:documentation>
+        </xs:annotation>
+      </xs:element>
+      <xs:element name="cStat" type="TStat">
+        <xs:annotation>
+          <xs:documentation>código do status do retorno da consulta.</xs:documentation>
+        </xs:annotation>
+      </xs:element>
+      <xs:element name="xMotivo" type="TMotivo">
+        <xs:annotation>
+          <xs:documentation>Descrição literal do status do do retorno da consulta.</xs:documentation>
+        </xs:annotation>
+      </xs:element>
+      <xs:element name="protCTe" type="TProtCTe" minOccurs="0">
+        <xs:annotation>
+          <xs:documentation>Reposta ao processamento do CT-e</xs:documentation>
+        </xs:annotation>
+      </xs:element>
+    </xs:sequence>
+    <xs:attribute name="versao" type="TVerCTe" use="required"/>
+  </xs:complexType>
   <xs:complexType name="TRetCTe">
     <xs:annotation>
       <xs:documentation>Tipo Retorno do Pedido de Autorização de CT-e (Modelo 57)</xs:documentation>
     </xs:annotation>
     <xs:sequence>
       <xs:element name="tpAmb" type="TAmb">
         <xs:annotation>
@@ -1306,14 +1346,1346 @@
         <xs:annotation>
           <xs:documentation>Reposta ao processamento do CT-e</xs:documentation>
         </xs:annotation>
       </xs:element>
     </xs:sequence>
     <xs:attribute name="versao" type="TVerCTe" use="required"/>
   </xs:complexType>
+  <xs:complexType name="TCTeSimp">
+    <xs:annotation>
+      <xs:documentation>Tipo Conhecimento de Transporte Eletrônico (Modelo 57) - Modelo Simplificado</xs:documentation>
+    </xs:annotation>
+    <xs:sequence>
+      <xs:element name="infCte">
+        <xs:annotation>
+          <xs:documentation>Informações do CT-e</xs:documentation>
+        </xs:annotation>
+        <xs:complexType>
+          <xs:sequence>
+            <xs:element name="ide">
+              <xs:annotation>
+                <xs:documentation>Identificação do CT-e</xs:documentation>
+              </xs:annotation>
+              <xs:complexType>
+                <xs:sequence>
+                  <xs:element name="cUF" type="TCodUfIBGE">
+                    <xs:annotation>
+                      <xs:documentation>Código da UF do emitente do CT-e.</xs:documentation>
+                      <xs:documentation>Utilizar a Tabela do IBGE.</xs:documentation>
+                    </xs:annotation>
+                  </xs:element>
+                  <xs:element name="cCT">
+                    <xs:annotation>
+                      <xs:documentation>Código numérico que compõe a Chave de Acesso.</xs:documentation>
+                      <xs:documentation>Número aleatório gerado pelo emitente para cada CT-e, com o objetivo de evitar acessos indevidos ao documento.</xs:documentation>
+                    </xs:annotation>
+                    <xs:simpleType>
+                      <xs:restriction base="xs:string">
+                        <xs:whiteSpace value="preserve"/>
+                        <xs:pattern value="[0-9]{8}"/>
+                      </xs:restriction>
+                    </xs:simpleType>
+                  </xs:element>
+                  <xs:element name="CFOP" type="TCfop">
+                    <xs:annotation>
+                      <xs:documentation>Código Fiscal de Operações e Prestações</xs:documentation>
+                    </xs:annotation>
+                  </xs:element>
+                  <xs:element name="natOp">
+                    <xs:annotation>
+                      <xs:documentation>Natureza da Operação</xs:documentation>
+                    </xs:annotation>
+                    <xs:simpleType>
+                      <xs:restriction base="TString">
+                        <xs:minLength value="1"/>
+                        <xs:maxLength value="60"/>
+                      </xs:restriction>
+                    </xs:simpleType>
+                  </xs:element>
+                  <xs:element name="mod" type="TModCT">
+                    <xs:annotation>
+                      <xs:documentation>Modelo do documento fiscal</xs:documentation>
+                      <xs:documentation>Utilizar o código 57 para identificação do CT-e, emitido em substituição aos modelos de conhecimentos em papel.</xs:documentation>
+                    </xs:annotation>
+                  </xs:element>
+                  <xs:element name="serie">
+                    <xs:annotation>
+                      <xs:documentation>Série do CT-e</xs:documentation>
+                      <xs:documentation>Preencher com &quot;0&quot; no caso de série única</xs:documentation>
+                    </xs:annotation>
+                    <xs:simpleType>
+                      <xs:restriction base="TSerie"/>
+                    </xs:simpleType>
+                  </xs:element>
+                  <xs:element name="nCT" type="TNF">
+                    <xs:annotation>
+                      <xs:documentation>Número do CT-e</xs:documentation>
+                    </xs:annotation>
+                  </xs:element>
+                  <xs:element name="dhEmi">
+                    <xs:annotation>
+                      <xs:documentation>Data e hora de emissão do CT-e</xs:documentation>
+                      <xs:documentation>Formato AAAA-MM-DDTHH:MM:DD TZD</xs:documentation>
+                    </xs:annotation>
+                    <xs:simpleType>
+                      <xs:restriction base="TDateTimeUTC"/>
+                    </xs:simpleType>
+                  </xs:element>
+                  <xs:element name="tpImp">
+                    <xs:annotation>
+                      <xs:documentation>Formato de impressão do DACTE</xs:documentation>
+                      <xs:documentation>Preencher com: 1 - Retrato; 2 - Paisagem.</xs:documentation>
+                    </xs:annotation>
+                    <xs:simpleType>
+                      <xs:restriction base="xs:string">
+                        <xs:whiteSpace value="preserve"/>
+                        <xs:enumeration value="1"/>
+                        <xs:enumeration value="2"/>
+                      </xs:restriction>
+                    </xs:simpleType>
+                  </xs:element>
+                  <xs:element name="tpEmis">
+                    <xs:annotation>
+                      <xs:documentation>Forma de emissão do CT-e</xs:documentation>
+                      <xs:documentation>Preencher com:
+1 - Normal;
+3 - Regime Especial NFF;  
+4 - EPEC pela SVC; 
+7 - Autorização pela SVC-RS;
+8 - Autorização pela SVC-SP</xs:documentation>
+                    </xs:annotation>
+                    <xs:simpleType>
+                      <xs:restriction base="xs:string">
+                        <xs:whiteSpace value="preserve"/>
+                        <xs:enumeration value="1"/>
+                        <xs:enumeration value="3"/>
+                        <xs:enumeration value="4"/>
+                        <xs:enumeration value="7"/>
+                        <xs:enumeration value="8"/>
+                      </xs:restriction>
+                    </xs:simpleType>
+                  </xs:element>
+                  <xs:element name="cDV">
+                    <xs:annotation>
+                      <xs:documentation>Digito Verificador da chave de acesso do CT-e</xs:documentation>
+                      <xs:documentation>Informar o dígito  de controle da chave de acesso do CT-e, que deve ser calculado com a aplicação do algoritmo módulo 11 (base 2,9) da chave de acesso.</xs:documentation>
+                    </xs:annotation>
+                    <xs:simpleType>
+                      <xs:restriction base="xs:string">
+                        <xs:whiteSpace value="preserve"/>
+                        <xs:pattern value="[0-9]{1}"/>
+                      </xs:restriction>
+                    </xs:simpleType>
+                  </xs:element>
+                  <xs:element name="tpAmb" type="TAmb">
+                    <xs:annotation>
+                      <xs:documentation>Tipo do Ambiente</xs:documentation>
+                      <xs:documentation>Preencher com:1 - Produção; 2 - Homologação.</xs:documentation>
+                    </xs:annotation>
+                  </xs:element>
+                  <xs:element name="tpCTe" type="TFinCTeSimp">
+                    <xs:annotation>
+                      <xs:documentation>Tipo do CT-e Simplificado</xs:documentation>
+                      <xs:documentation>Preencher com:
+4 - CTe Simplificado
+5 - Substituição CTe Simplificado</xs:documentation>
+                    </xs:annotation>
+                  </xs:element>
+                  <xs:element name="procEmi" type="TProcEmi">
+                    <xs:annotation>
+                      <xs:documentation>Identificador do processo de emissão do CT-e</xs:documentation>
+                      <xs:documentation>Preencher com: 
+											0 - emissão de CT-e com aplicativo do contribuinte;
+											3- emissão CT-e pelo contribuinte com aplicativo fornecido pelo SEBRAE.</xs:documentation>
+                    </xs:annotation>
+                  </xs:element>
+                  <xs:element name="verProc">
+                    <xs:annotation>
+                      <xs:documentation>Versão do processo de emissão</xs:documentation>
+                      <xs:documentation>Informar a versão do aplicativo emissor de CT-e.</xs:documentation>
+                    </xs:annotation>
+                    <xs:simpleType>
+                      <xs:restriction base="TString">
+                        <xs:minLength value="1"/>
+                        <xs:maxLength value="20"/>
+                      </xs:restriction>
+                    </xs:simpleType>
+                  </xs:element>
+                  <xs:element name="cMunEnv" type="TCodMunIBGE">
+                    <xs:annotation>
+                      <xs:documentation>Código do Município de envio do CT-e (de onde o documento foi transmitido)</xs:documentation>
+                      <xs:documentation>Utilizar a tabela do IBGE. Informar 9999999 para as operações com o exterior.</xs:documentation>
+                    </xs:annotation>
+                  </xs:element>
+                  <xs:element name="xMunEnv">
+                    <xs:annotation>
+                      <xs:documentation>Nome do Município de envio do CT-e (de onde o documento foi transmitido)</xs:documentation>
+                      <xs:documentation>Informar PAIS/Municipio para as operações com o exterior.</xs:documentation>
+                    </xs:annotation>
+                    <xs:simpleType>
+                      <xs:restriction base="TString">
+                        <xs:minLength value="2"/>
+                        <xs:maxLength value="60"/>
+                      </xs:restriction>
+                    </xs:simpleType>
+                  </xs:element>
+                  <xs:element name="UFEnv" type="TUf">
+                    <xs:annotation>
+                      <xs:documentation>Sigla da UF de envio do CT-e (de onde o documento foi transmitido)</xs:documentation>
+                      <xs:documentation>Informar 'EX' para operações com o exterior.</xs:documentation>
+                    </xs:annotation>
+                  </xs:element>
+                  <xs:element name="modal" type="TModTranspSimp">
+                    <xs:annotation>
+                      <xs:documentation>Modal</xs:documentation>
+                      <xs:documentation>Preencher com:
+01-Rodoviário
+02-Aéreo
+03-Aquaviário</xs:documentation>
+                    </xs:annotation>
+                  </xs:element>
+                  <xs:element name="tpServ">
+                    <xs:annotation>
+                      <xs:documentation>Tipo do Serviço</xs:documentation>
+                      <xs:documentation>Preencher com: 
+0 - Normal;
+1 - Subcontratação;
+2 - Redespacho;</xs:documentation>
+                    </xs:annotation>
+                    <xs:simpleType>
+                      <xs:restriction base="xs:string">
+                        <xs:whiteSpace value="preserve"/>
+                        <xs:enumeration value="0"/>
+                        <xs:enumeration value="1"/>
+                        <xs:enumeration value="2"/>
+                      </xs:restriction>
+                    </xs:simpleType>
+                  </xs:element>
+                  <xs:element name="UFIni" type="TUf">
+                    <xs:annotation>
+                      <xs:documentation>UF do início da prestação</xs:documentation>
+                      <xs:documentation>Informar 'EX' para operações com o exterior.</xs:documentation>
+                    </xs:annotation>
+                  </xs:element>
+                  <xs:element name="UFFim" type="TUf">
+                    <xs:annotation>
+                      <xs:documentation>UF do término da prestação</xs:documentation>
+                      <xs:documentation>Informar 'EX' para operações com o exterior.</xs:documentation>
+                    </xs:annotation>
+                  </xs:element>
+                  <xs:element name="retira">
+                    <xs:annotation>
+                      <xs:documentation>Indicador se o Recebedor retira no Aeroporto, Filial, Porto ou Estação de Destino?</xs:documentation>
+                      <xs:documentation>Preencher com: 0 - sim; 1 - não</xs:documentation>
+                    </xs:annotation>
+                    <xs:simpleType>
+                      <xs:restriction base="xs:string">
+                        <xs:whiteSpace value="preserve"/>
+                        <xs:enumeration value="0"/>
+                        <xs:enumeration value="1"/>
+                      </xs:restriction>
+                    </xs:simpleType>
+                  </xs:element>
+                  <xs:element name="xDetRetira" minOccurs="0">
+                    <xs:annotation>
+                      <xs:documentation>Detalhes do retira</xs:documentation>
+                    </xs:annotation>
+                    <xs:simpleType>
+                      <xs:restriction base="TString">
+                        <xs:minLength value="1"/>
+                        <xs:maxLength value="160"/>
+                      </xs:restriction>
+                    </xs:simpleType>
+                  </xs:element>
+                  <xs:sequence minOccurs="0">
+                    <xs:annotation>
+                      <xs:documentation>Informar apenas
+para tpEmis diferente de 1</xs:documentation>
+                    </xs:annotation>
+                    <xs:element name="dhCont" type="TDateTimeUTC">
+                      <xs:annotation>
+                        <xs:documentation>Data e Hora da entrada em contingência</xs:documentation>
+                        <xs:documentation>Informar a data e hora no formato AAAA-MM-DDTHH:MM:SS</xs:documentation>
+                      </xs:annotation>
+                    </xs:element>
+                    <xs:element name="xJust">
+                      <xs:annotation>
+                        <xs:documentation>Justificativa da entrada em contingência</xs:documentation>
+                      </xs:annotation>
+                      <xs:simpleType>
+                        <xs:restriction base="TString">
+                          <xs:minLength value="15"/>
+                          <xs:maxLength value="256"/>
+                        </xs:restriction>
+                      </xs:simpleType>
+                    </xs:element>
+                  </xs:sequence>
+                </xs:sequence>
+              </xs:complexType>
+            </xs:element>
+            <xs:element name="compl" minOccurs="0">
+              <xs:annotation>
+                <xs:documentation>Dados complementares do CT-e para fins operacionais ou comerciais</xs:documentation>
+              </xs:annotation>
+              <xs:complexType>
+                <xs:sequence>
+                  <xs:element name="xCaracAd" minOccurs="0">
+                    <xs:annotation>
+                      <xs:documentation>Característica adicional do transporte</xs:documentation>
+                      <xs:documentation>Texto livre:
+REENTREGA; DEVOLUÇÃO; REFATURAMENTO; etc</xs:documentation>
+                    </xs:annotation>
+                    <xs:simpleType>
+                      <xs:restriction base="TString">
+                        <xs:minLength value="1"/>
+                        <xs:maxLength value="15"/>
+                      </xs:restriction>
+                    </xs:simpleType>
+                  </xs:element>
+                  <xs:element name="xCaracSer" minOccurs="0">
+                    <xs:annotation>
+                      <xs:documentation>Característica adicional do serviço</xs:documentation>
+                      <xs:documentation>Texto livre:
+											ENTREGA EXPRESSA; LOGÍSTICA REVERSA; CONVENCIONAL; EMERGENCIAL; etc</xs:documentation>
+                    </xs:annotation>
+                    <xs:simpleType>
+                      <xs:restriction base="TString">
+                        <xs:minLength value="1"/>
+                        <xs:maxLength value="30"/>
+                      </xs:restriction>
+                    </xs:simpleType>
+                  </xs:element>
+                  <xs:element name="fluxo" minOccurs="0">
+                    <xs:annotation>
+                      <xs:documentation>Previsão do fluxo da carga</xs:documentation>
+                      <xs:documentation>Preenchimento obrigatório para o modal aéreo.</xs:documentation>
+                    </xs:annotation>
+                    <xs:complexType>
+                      <xs:sequence>
+                        <xs:element name="xOrig" minOccurs="0">
+                          <xs:annotation>
+                            <xs:documentation>Sigla ou código interno da Filial/Porto/Estação/ Aeroporto de Origem</xs:documentation>
+                            <xs:documentation>Observações para o modal aéreo:
+														- Preenchimento obrigatório para o modal aéreo.
+														- O código de três letras IATA do aeroporto de partida deverá ser incluído como primeira anotação. Quando não for possível, utilizar a sigla OACI.</xs:documentation>
+                          </xs:annotation>
+                          <xs:simpleType>
+                            <xs:restriction base="TString">
+                              <xs:minLength value="1"/>
+                              <xs:maxLength value="60"/>
+                            </xs:restriction>
+                          </xs:simpleType>
+                        </xs:element>
+                        <xs:element name="pass" minOccurs="0" maxOccurs="unbounded">
+                          <xs:complexType>
+                            <xs:sequence>
+                              <xs:element name="xPass" minOccurs="0">
+                                <xs:annotation>
+                                  <xs:documentation>Sigla ou código interno da Filial/Porto/Estação/Aeroporto de Passagem</xs:documentation>
+                                  <xs:documentation>Observação para o modal aéreo:
+																	- O código de três letras IATA, referente ao aeroporto de transferência, deverá ser incluído, quando for o caso. Quando não for possível,  utilizar a sigla OACI. Qualquer solicitação de itinerário deverá ser incluída.</xs:documentation>
+                                </xs:annotation>
+                                <xs:simpleType>
+                                  <xs:restriction base="TString">
+                                    <xs:minLength value="1"/>
+                                    <xs:maxLength value="15"/>
+                                  </xs:restriction>
+                                </xs:simpleType>
+                              </xs:element>
+                            </xs:sequence>
+                          </xs:complexType>
+                        </xs:element>
+                        <xs:element name="xDest" minOccurs="0">
+                          <xs:annotation>
+                            <xs:documentation>Sigla ou código interno da Filial/Porto/Estação/Aeroporto de Destino</xs:documentation>
+                            <xs:documentation>Observações para o modal aéreo:
+														- Preenchimento obrigatório para o modal aéreo.
+														- Deverá ser incluído o código de três letras IATA do aeroporto de destino. Quando não for possível, utilizar a sigla OACI.</xs:documentation>
+                          </xs:annotation>
+                          <xs:simpleType>
+                            <xs:restriction base="TString">
+                              <xs:minLength value="1"/>
+                              <xs:maxLength value="60"/>
+                            </xs:restriction>
+                          </xs:simpleType>
+                        </xs:element>
+                        <xs:element name="xRota" minOccurs="0">
+                          <xs:annotation>
+                            <xs:documentation>Código da Rota de Entrega</xs:documentation>
+                          </xs:annotation>
+                          <xs:simpleType>
+                            <xs:restriction base="TString">
+                              <xs:minLength value="1"/>
+                              <xs:maxLength value="10"/>
+                            </xs:restriction>
+                          </xs:simpleType>
+                        </xs:element>
+                      </xs:sequence>
+                    </xs:complexType>
+                  </xs:element>
+                  <xs:element name="xObs" minOccurs="0">
+                    <xs:annotation>
+                      <xs:documentation>Observações Gerais</xs:documentation>
+                    </xs:annotation>
+                    <xs:simpleType>
+                      <xs:restriction base="TString">
+                        <xs:minLength value="1"/>
+                        <xs:maxLength value="2000"/>
+                      </xs:restriction>
+                    </xs:simpleType>
+                  </xs:element>
+                  <xs:element name="ObsCont" minOccurs="0" maxOccurs="10">
+                    <xs:annotation>
+                      <xs:documentation>Campo de uso livre do contribuinte</xs:documentation>
+                      <xs:documentation>Informar o nome do campo no atributo xCampo e o conteúdo do campo no XTexto</xs:documentation>
+                    </xs:annotation>
+                    <xs:complexType>
+                      <xs:sequence>
+                        <xs:element name="xTexto">
+                          <xs:annotation>
+                            <xs:documentation>Conteúdo do campo</xs:documentation>
+                          </xs:annotation>
+                          <xs:simpleType>
+                            <xs:restriction base="TString">
+                              <xs:minLength value="1"/>
+                              <xs:maxLength value="160"/>
+                            </xs:restriction>
+                          </xs:simpleType>
+                        </xs:element>
+                      </xs:sequence>
+                      <xs:attribute name="xCampo" use="required">
+                        <xs:annotation>
+                          <xs:documentation>Identificação do campo</xs:documentation>
+                        </xs:annotation>
+                        <xs:simpleType>
+                          <xs:restriction base="TString">
+                            <xs:minLength value="1"/>
+                            <xs:maxLength value="20"/>
+                          </xs:restriction>
+                        </xs:simpleType>
+                      </xs:attribute>
+                    </xs:complexType>
+                  </xs:element>
+                  <xs:element name="ObsFisco" minOccurs="0" maxOccurs="10">
+                    <xs:annotation>
+                      <xs:documentation>Campo de uso livre do contribuinte</xs:documentation>
+                      <xs:documentation>Informar o nome do campo no atributo xCampo e o conteúdo do campo no XTexto</xs:documentation>
+                    </xs:annotation>
+                    <xs:complexType>
+                      <xs:sequence>
+                        <xs:element name="xTexto">
+                          <xs:annotation>
+                            <xs:documentation>Conteúdo do campo</xs:documentation>
+                          </xs:annotation>
+                          <xs:simpleType>
+                            <xs:restriction base="TString">
+                              <xs:minLength value="1"/>
+                              <xs:maxLength value="60"/>
+                            </xs:restriction>
+                          </xs:simpleType>
+                        </xs:element>
+                      </xs:sequence>
+                      <xs:attribute name="xCampo" use="required">
+                        <xs:annotation>
+                          <xs:documentation>Identificação do campo</xs:documentation>
+                        </xs:annotation>
+                        <xs:simpleType>
+                          <xs:restriction base="TString">
+                            <xs:minLength value="1"/>
+                            <xs:maxLength value="20"/>
+                          </xs:restriction>
+                        </xs:simpleType>
+                      </xs:attribute>
+                    </xs:complexType>
+                  </xs:element>
+                </xs:sequence>
+              </xs:complexType>
+            </xs:element>
+            <xs:element name="emit">
+              <xs:annotation>
+                <xs:documentation>Identificação do Emitente do CT-e</xs:documentation>
+              </xs:annotation>
+              <xs:complexType>
+                <xs:sequence>
+                  <xs:choice>
+                    <xs:element name="CNPJ" type="TCnpj">
+                      <xs:annotation>
+                        <xs:documentation>CNPJ do emitente</xs:documentation>
+                        <xs:documentation>Informar zeros não significativos</xs:documentation>
+                      </xs:annotation>
+                    </xs:element>
+                    <xs:element name="CPF" type="TCpf">
+                      <xs:annotation>
+                        <xs:documentation>CPF do emitente</xs:documentation>
+                        <xs:documentation>Informar zeros não significativos.
+
+Usar com série específica 920-969 para emitente pessoa física com inscrição estadual</xs:documentation>
+                      </xs:annotation>
+                    </xs:element>
+                  </xs:choice>
+                  <xs:element name="IE" minOccurs="0">
+                    <xs:annotation>
+                      <xs:documentation>Inscrição Estadual do Emitente</xs:documentation>
+                      <xs:documentation>A IE do emitente somente ficará sem informação para o caso do Regime Especial da NFF (tpEmis=3)</xs:documentation>
+                    </xs:annotation>
+                    <xs:simpleType>
+                      <xs:restriction base="TIe"/>
+                    </xs:simpleType>
+                  </xs:element>
+                  <xs:element name="IEST" minOccurs="0">
+                    <xs:annotation>
+                      <xs:documentation>Inscrição Estadual do Substituto Tributário</xs:documentation>
+                    </xs:annotation>
+                    <xs:simpleType>
+                      <xs:restriction base="TIe"/>
+                    </xs:simpleType>
+                  </xs:element>
+                  <xs:element name="xNome">
+                    <xs:annotation>
+                      <xs:documentation>Razão social ou Nome do emitente</xs:documentation>
+                    </xs:annotation>
+                    <xs:simpleType>
+                      <xs:restriction base="TString">
+                        <xs:maxLength value="60"/>
+                        <xs:minLength value="2"/>
+                      </xs:restriction>
+                    </xs:simpleType>
+                  </xs:element>
+                  <xs:element name="xFant" minOccurs="0">
+                    <xs:annotation>
+                      <xs:documentation>Nome fantasia</xs:documentation>
+                    </xs:annotation>
+                    <xs:simpleType>
+                      <xs:restriction base="TString">
+                        <xs:maxLength value="60"/>
+                        <xs:minLength value="2"/>
+                      </xs:restriction>
+                    </xs:simpleType>
+                  </xs:element>
+                  <xs:element name="enderEmit" type="TEndeEmi">
+                    <xs:annotation>
+                      <xs:documentation>Endereço do emitente</xs:documentation>
+                    </xs:annotation>
+                  </xs:element>
+                  <xs:element name="CRT" type="TCRT">
+                    <xs:annotation>
+                      <xs:documentation>Código do Regime Tributário</xs:documentation>
+                      <xs:documentation>Informar: 1=Simples Nacional; 
+2=Simples Nacional, excesso sublimite de receita bruta;
+3=Regime Normal. 
+4=Simples Nacional - Microempreendedor Individual – MEI.</xs:documentation>
+                    </xs:annotation>
+                  </xs:element>
+                </xs:sequence>
+              </xs:complexType>
+            </xs:element>
+            <xs:element name="toma">
+              <xs:annotation>
+                <xs:documentation>Identificação do tomador do serviço no CT-e</xs:documentation>
+              </xs:annotation>
+              <xs:complexType>
+                <xs:sequence>
+                  <xs:element name="toma">
+                    <xs:annotation>
+                      <xs:documentation>Tomador do Serviço</xs:documentation>
+                      <xs:documentation>Preencher com:
+
+0-Remetente;
+1-Expedidor;
+2-Recebedor;
+3-Destinatário
+4-Terceiro</xs:documentation>
+                    </xs:annotation>
+                    <xs:simpleType>
+                      <xs:restriction base="xs:string">
+                        <xs:whiteSpace value="preserve"/>
+                        <xs:enumeration value="1"/>
+                        <xs:enumeration value="2"/>
+                        <xs:enumeration value="3"/>
+                        <xs:enumeration value="4"/>
+                      </xs:restriction>
+                    </xs:simpleType>
+                  </xs:element>
+                  <xs:element name="indIEToma">
+                    <xs:annotation>
+                      <xs:documentation>Indicador do papel do tomador na prestação do serviço:
+1 – Contribuinte ICMS;
+2 – Contribuinte isento de inscrição;
+9 – Não Contribuinte</xs:documentation>
+                      <xs:documentation>Aplica-se ao tomador que for indicado no toma3 ou toma4</xs:documentation>
+                    </xs:annotation>
+                    <xs:simpleType>
+                      <xs:restriction base="xs:string">
+                        <xs:whiteSpace value="preserve"/>
+                        <xs:enumeration value="1"/>
+                        <xs:enumeration value="2"/>
+                        <xs:enumeration value="9"/>
+                      </xs:restriction>
+                    </xs:simpleType>
+                  </xs:element>
+                  <xs:choice>
+                    <xs:element name="CNPJ" type="TCnpjOpc">
+                      <xs:annotation>
+                        <xs:documentation>Número do CNPJ</xs:documentation>
+                        <xs:documentation>Em caso de empresa não estabelecida no Brasil, será informado o CNPJ com zeros.															
+Informar os zeros não significativos.</xs:documentation>
+                      </xs:annotation>
+                    </xs:element>
+                    <xs:element name="CPF" type="TCpf">
+                      <xs:annotation>
+                        <xs:documentation>Número do CPF</xs:documentation>
+                        <xs:documentation>Informar os zeros não significativos.</xs:documentation>
+                      </xs:annotation>
+                    </xs:element>
+                  </xs:choice>
+                  <xs:element name="IE" minOccurs="0">
+                    <xs:annotation>
+                      <xs:documentation>Inscrição Estadual</xs:documentation>
+                      <xs:documentation>Informar a IE do tomador ou ISENTO se tomador é contribuinte do ICMS isento de inscrição no cadastro de contribuintes do ICMS. Caso o tomador não seja contribuinte do ICMS não informar o conteúdo.</xs:documentation>
+                    </xs:annotation>
+                    <xs:simpleType>
+                      <xs:restriction base="TIeDest"/>
+                    </xs:simpleType>
+                  </xs:element>
+                  <xs:element name="xNome">
+                    <xs:annotation>
+                      <xs:documentation>Razão Social ou Nome</xs:documentation>
+                    </xs:annotation>
+                    <xs:simpleType>
+                      <xs:restriction base="TString">
+                        <xs:maxLength value="60"/>
+                        <xs:minLength value="2"/>
+                      </xs:restriction>
+                    </xs:simpleType>
+                  </xs:element>
+                  <xs:element name="ISUF" minOccurs="0">
+                    <xs:annotation>
+                      <xs:documentation>Inscrição na SUFRAMA</xs:documentation>
+                      <xs:documentation>(Obrigatório nas operações com as áreas com benefícios de incentivos fiscais sob controle da SUFRAMA)</xs:documentation>
+                    </xs:annotation>
+                    <xs:simpleType>
+                      <xs:restriction base="xs:string">
+                        <xs:whiteSpace value="preserve"/>
+                        <xs:pattern value="[0-9]{8,9}"/>
+                      </xs:restriction>
+                    </xs:simpleType>
+                  </xs:element>
+                  <xs:element name="fone" type="TFone" minOccurs="0">
+                    <xs:annotation>
+                      <xs:documentation>Telefone</xs:documentation>
+                    </xs:annotation>
+                  </xs:element>
+                  <xs:element name="enderToma" type="TEndereco">
+                    <xs:annotation>
+                      <xs:documentation>Dados do endereço</xs:documentation>
+                    </xs:annotation>
+                  </xs:element>
+                  <xs:element name="email" type="TEmail" minOccurs="0">
+                    <xs:annotation>
+                      <xs:documentation>Endereço de email</xs:documentation>
+                    </xs:annotation>
+                  </xs:element>
+                </xs:sequence>
+              </xs:complexType>
+            </xs:element>
+            <xs:element name="infCarga">
+              <xs:annotation>
+                <xs:documentation>Informações da Carga do CT-e</xs:documentation>
+              </xs:annotation>
+              <xs:complexType>
+                <xs:sequence>
+                  <xs:element name="vCarga" type="TDec_1302">
+                    <xs:annotation>
+                      <xs:documentation>Valor total da carga</xs:documentation>
+                    </xs:annotation>
+                  </xs:element>
+                  <xs:element name="proPred">
+                    <xs:annotation>
+                      <xs:documentation>Produto predominante</xs:documentation>
+                      <xs:documentation>Informar a descrição do produto predominante</xs:documentation>
+                    </xs:annotation>
+                    <xs:simpleType>
+                      <xs:restriction base="TString">
+                        <xs:minLength value="1"/>
+                        <xs:maxLength value="60"/>
+                      </xs:restriction>
+                    </xs:simpleType>
+                  </xs:element>
+                  <xs:element name="xOutCat" minOccurs="0">
+                    <xs:annotation>
+                      <xs:documentation>Outras características da carga</xs:documentation>
+                      <xs:documentation>&quot;FRIA&quot;, &quot;GRANEL&quot;, &quot;REFRIGERADA&quot;, &quot;Medidas: 12X12X12&quot;</xs:documentation>
+                    </xs:annotation>
+                    <xs:simpleType>
+                      <xs:restriction base="TString">
+                        <xs:minLength value="1"/>
+                        <xs:maxLength value="30"/>
+                      </xs:restriction>
+                    </xs:simpleType>
+                  </xs:element>
+                  <xs:element name="infQ" maxOccurs="unbounded">
+                    <xs:annotation>
+                      <xs:documentation>Informações de quantidades da Carga do CT-e</xs:documentation>
+                      <xs:documentation>Para o Aéreo é obrigatório o preenchimento desse campo da seguinte forma.
+1 - Peso Bruto, sempre em quilogramas (obrigatório);
+2 - Peso Cubado; sempre em quilogramas;
+3 - Quantidade de volumes, sempre em unidades (obrigatório);
+4 - Cubagem, sempre em metros cúbicos (obrigatório apenas quando for impossível preencher as dimensões da(s) embalagem(ens) na tag xDime do leiaute do Aéreo).</xs:documentation>
+                    </xs:annotation>
+                    <xs:complexType>
+                      <xs:sequence>
+                        <xs:element name="cUnid">
+                          <xs:annotation>
+                            <xs:documentation>Código da Unidade de Medida</xs:documentation>
+                            <xs:documentation>Preencher com:
+00-M3;
+01-KG;
+02-TON;
+03-UNIDADE;
+04-LITROS;
+05-MMBTU</xs:documentation>
+                          </xs:annotation>
+                          <xs:simpleType>
+                            <xs:restriction base="xs:string">
+                              <xs:whiteSpace value="preserve"/>
+                              <xs:enumeration value="00"/>
+                              <xs:enumeration value="01"/>
+                              <xs:enumeration value="02"/>
+                              <xs:enumeration value="03"/>
+                              <xs:enumeration value="04"/>
+                              <xs:enumeration value="05"/>
+                            </xs:restriction>
+                          </xs:simpleType>
+                        </xs:element>
+                        <xs:element name="tpMed">
+                          <xs:annotation>
+                            <xs:documentation>Tipo da Medida</xs:documentation>
+                            <xs:documentation>Informar com:
+00-Cubagem da NF-e
+01-Cubagem Aferida pelo Transportador
+02-Peso Bruto da NF-e
+03-Peso Bruto Aferido pelo Transportador
+04-Peso Cubado
+05-Peso Base do Cálculo do Frete
+06-Peso para uso Operacional
+07-Caixas
+08-Paletes
+09-Sacas
+10-Containers
+11-Rolos
+12-Bombonas
+13-Latas
+14-Litragem
+15-Milhão de BTU (British Thermal Units)
+99-Outros</xs:documentation>
+                          </xs:annotation>
+                          <xs:simpleType>
+                            <xs:restriction base="TString">
+                              <xs:minLength value="1"/>
+                              <xs:maxLength value="2"/>
+                              <xs:enumeration value="00"/>
+                              <xs:enumeration value="01"/>
+                              <xs:enumeration value="02"/>
+                              <xs:enumeration value="03"/>
+                              <xs:enumeration value="04"/>
+                              <xs:enumeration value="05"/>
+                              <xs:enumeration value="06"/>
+                              <xs:enumeration value="07"/>
+                              <xs:enumeration value="08"/>
+                              <xs:enumeration value="09"/>
+                              <xs:enumeration value="10"/>
+                              <xs:enumeration value="11"/>
+                              <xs:enumeration value="12"/>
+                              <xs:enumeration value="13"/>
+                              <xs:enumeration value="14"/>
+                              <xs:enumeration value="15"/>
+                              <xs:enumeration value="99"/>
+                            </xs:restriction>
+                          </xs:simpleType>
+                        </xs:element>
+                        <xs:element name="qCarga" type="TDec_1104">
+                          <xs:annotation>
+                            <xs:documentation>Quantidade</xs:documentation>
+                          </xs:annotation>
+                        </xs:element>
+                      </xs:sequence>
+                    </xs:complexType>
+                  </xs:element>
+                  <xs:element name="vCargaAverb" type="TDec_1302Opc" minOccurs="0">
+                    <xs:annotation>
+                      <xs:documentation>Valor da Carga para efeito de averbação</xs:documentation>
+                      <xs:documentation>Normalmente igual ao valor declarado da mercadoria, diferente por exemplo, quando a mercadoria transportada é isenta de tributos nacionais para exportação, onde é preciso averbar um valor maior, pois no caso de indenização, o valor a ser pago será maior</xs:documentation>
+                    </xs:annotation>
+                  </xs:element>
+                </xs:sequence>
+              </xs:complexType>
+            </xs:element>
+            <xs:element name="det" maxOccurs="999">
+              <xs:annotation>
+                <xs:documentation>Detalhamento das entregas / prestações do CTe Simplificado</xs:documentation>
+              </xs:annotation>
+              <xs:complexType>
+                <xs:sequence>
+                  <xs:sequence>
+                    <xs:element name="cMunIni" type="TCodMunIBGE">
+                      <xs:annotation>
+                        <xs:documentation>Código do Município de início da prestação</xs:documentation>
+                        <xs:documentation>Utilizar a tabela do IBGE. Informar 9999999 para operações com o exterior.</xs:documentation>
+                      </xs:annotation>
+                    </xs:element>
+                    <xs:element name="xMunIni">
+                      <xs:annotation>
+                        <xs:documentation>Nome do Município do início da prestação</xs:documentation>
+                        <xs:documentation>Informar 'EXTERIOR' para operações com o exterior.</xs:documentation>
+                      </xs:annotation>
+                      <xs:simpleType>
+                        <xs:restriction base="TString">
+                          <xs:minLength value="2"/>
+                          <xs:maxLength value="60"/>
+                        </xs:restriction>
+                      </xs:simpleType>
+                    </xs:element>
+                  </xs:sequence>
+                  <xs:sequence>
+                    <xs:element name="cMunFim" type="TCodMunIBGE">
+                      <xs:annotation>
+                        <xs:documentation>Código do Município de término da prestação</xs:documentation>
+                        <xs:documentation>Utilizar a tabela do IBGE. Informar 9999999 para operações com o exterior.</xs:documentation>
+                      </xs:annotation>
+                    </xs:element>
+                    <xs:element name="xMunFim">
+                      <xs:annotation>
+                        <xs:documentation>Nome do Município do término da prestação</xs:documentation>
+                        <xs:documentation>Informar 'EXTERIOR' para operações com o exterior.</xs:documentation>
+                      </xs:annotation>
+                      <xs:simpleType>
+                        <xs:restriction base="TString">
+                          <xs:minLength value="2"/>
+                          <xs:maxLength value="60"/>
+                        </xs:restriction>
+                      </xs:simpleType>
+                    </xs:element>
+                  </xs:sequence>
+                  <xs:element name="vPrest" type="TDec_1302">
+                    <xs:annotation>
+                      <xs:documentation>Valorl da Prestação do Serviço</xs:documentation>
+                      <xs:documentation>Pode conter zeros quando o CT-e for de complemento de ICMS</xs:documentation>
+                    </xs:annotation>
+                  </xs:element>
+                  <xs:element name="vRec" type="TDec_1302">
+                    <xs:annotation>
+                      <xs:documentation>Valor a Receber</xs:documentation>
+                    </xs:annotation>
+                  </xs:element>
+                  <xs:element name="Comp" minOccurs="0" maxOccurs="unbounded">
+                    <xs:annotation>
+                      <xs:documentation>Componentes do Valor da Prestação</xs:documentation>
+                    </xs:annotation>
+                    <xs:complexType>
+                      <xs:sequence>
+                        <xs:element name="xNome">
+                          <xs:annotation>
+                            <xs:documentation>Nome do componente</xs:documentation>
+                            <xs:documentation>Exxemplos: FRETE PESO, FRETE VALOR, SEC/CAT, ADEME, AGENDAMENTO, etc</xs:documentation>
+                          </xs:annotation>
+                          <xs:simpleType>
+                            <xs:restriction base="TString">
+                              <xs:maxLength value="15"/>
+                              <xs:minLength value="1"/>
+                            </xs:restriction>
+                          </xs:simpleType>
+                        </xs:element>
+                        <xs:element name="vComp" type="TDec_1302">
+                          <xs:annotation>
+                            <xs:documentation>Valor do componente</xs:documentation>
+                          </xs:annotation>
+                        </xs:element>
+                      </xs:sequence>
+                    </xs:complexType>
+                  </xs:element>
+                  <xs:choice>
+                    <xs:element name="infNFe" maxOccurs="unbounded">
+                      <xs:annotation>
+                        <xs:documentation>Informações das NF-e</xs:documentation>
+                      </xs:annotation>
+                      <xs:complexType>
+                        <xs:sequence>
+                          <xs:element name="chNFe" type="TChDFe">
+                            <xs:annotation>
+                              <xs:documentation>Chave de acesso da NF-e</xs:documentation>
+                            </xs:annotation>
+                          </xs:element>
+                          <xs:element name="PIN" minOccurs="0">
+                            <xs:annotation>
+                              <xs:documentation>PIN SUFRAMA</xs:documentation>
+                              <xs:documentation>PIN atribuído pela SUFRAMA para a operação.</xs:documentation>
+                            </xs:annotation>
+                            <xs:simpleType>
+                              <xs:restriction base="xs:string">
+                                <xs:whiteSpace value="preserve"/>
+                                <xs:minLength value="2"/>
+                                <xs:maxLength value="9"/>
+                                <xs:pattern value="[1-9]{1}[0-9]{1,8}"/>
+                              </xs:restriction>
+                            </xs:simpleType>
+                          </xs:element>
+                          <xs:element name="dPrev" type="TData" minOccurs="0">
+                            <xs:annotation>
+                              <xs:documentation>Data prevista de entrega</xs:documentation>
+                              <xs:documentation>Formato AAAA-MM-DD</xs:documentation>
+                            </xs:annotation>
+                          </xs:element>
+                          <xs:choice>
+                            <xs:element name="infUnidCarga" type="TUnidCarga" minOccurs="0" maxOccurs="unbounded">
+                              <xs:annotation>
+                                <xs:documentation>Informações das Unidades de Carga (Containeres/ULD/Outros)</xs:documentation>
+                                <xs:documentation>Dispositivo de carga utilizada (Unit Load Device - ULD) significa todo tipo de contêiner de carga, vagão, contêiner de avião, palete de aeronave com rede ou palete de aeronave com rede sobre um iglu.</xs:documentation>
+                              </xs:annotation>
+                            </xs:element>
+                            <xs:element name="infUnidTransp" type="TUnidadeTransp" minOccurs="0" maxOccurs="unbounded">
+                              <xs:annotation>
+                                <xs:documentation>Informações das Unidades de Transporte (Carreta/Reboque/Vagão)</xs:documentation>
+                                <xs:documentation>Deve ser preenchido com as informações das unidades de transporte utilizadas.</xs:documentation>
+                              </xs:annotation>
+                            </xs:element>
+                          </xs:choice>
+                        </xs:sequence>
+                      </xs:complexType>
+                    </xs:element>
+                    <xs:element name="infDocAnt" maxOccurs="unbounded">
+                      <xs:annotation>
+                        <xs:documentation>Documentos anteriores</xs:documentation>
+                      </xs:annotation>
+                      <xs:complexType>
+                        <xs:sequence>
+                          <xs:element name="chCTe" type="TChDFe">
+                            <xs:annotation>
+                              <xs:documentation>Chave de acesso do CT-e</xs:documentation>
+                            </xs:annotation>
+                          </xs:element>
+                          <xs:element name="tpPrest">
+                            <xs:annotation>
+                              <xs:documentation>indica se a prestação é total ou parcial em relação as notas do documento anterior</xs:documentation>
+                              <xs:documentation>Preencher com:
+
+1 - Total
+2 - Parcial</xs:documentation>
+                            </xs:annotation>
+                            <xs:simpleType>
+                              <xs:restriction base="xs:string">
+                                <xs:whiteSpace value="preserve"/>
+                                <xs:enumeration value="1"/>
+                                <xs:enumeration value="2"/>
+                              </xs:restriction>
+                            </xs:simpleType>
+                          </xs:element>
+                          <xs:element name="infNFeTranspParcial" minOccurs="0" maxOccurs="unbounded">
+                            <xs:complexType>
+                              <xs:sequence>
+                                <xs:element name="chNFe" type="TChDFe">
+                                  <xs:annotation>
+                                    <xs:documentation>Chave de acesso da NF-e</xs:documentation>
+                                    <xs:documentation>Informando o tpPrest com “2 – Parcial” deve-se informar as chaves de acesso das NF-e que acobertam a carga transportada.</xs:documentation>
+                                  </xs:annotation>
+                                </xs:element>
+                              </xs:sequence>
+                            </xs:complexType>
+                          </xs:element>
+                        </xs:sequence>
+                      </xs:complexType>
+                    </xs:element>
+                  </xs:choice>
+                </xs:sequence>
+                <xs:attribute name="nItem" use="required">
+                  <xs:annotation>
+                    <xs:documentation>Número identificador do item agrupador da prestação</xs:documentation>
+                  </xs:annotation>
+                  <xs:simpleType>
+                    <xs:restriction base="xs:string">
+                      <xs:whiteSpace value="preserve"/>
+                      <xs:pattern value="[1-9]{1}[0-9]{0,1}|[1-8]{1}[0-9]{2}|[9]{1}[0-8]{1}[0-9]{1}|[9]{1}[9]{1}[0]{1}"/>
+                    </xs:restriction>
+                  </xs:simpleType>
+                </xs:attribute>
+              </xs:complexType>
+            </xs:element>
+            <xs:element name="infModal">
+              <xs:annotation>
+                <xs:documentation>Informações do modal</xs:documentation>
+              </xs:annotation>
+              <xs:complexType>
+                <xs:sequence>
+                  <xs:any processContents="skip">
+                    <xs:annotation>
+                      <xs:documentation>XML do modal
+Insira neste local o XML específico do modal (rodoviário, aéreo, ferroviário, aquaviário ou dutoviário).</xs:documentation>
+                      <xs:documentation>O elemento do tipo -any- permite estender o documento XML com elementos não especificados pelo schema.
+															Insira neste local - any- o XML específico do modal (rodoviário, aéreo, ferroviário, aquaviário ou dutoviário). A especificação do schema XML para cada modal pode ser encontrada nos arquivos que acompanham este pacote de liberação:
+													Rodoviário - ver arquivo CTeModalRodoviario_v9.99
+			Aéreo - ver arquivo CTeModalAereo_v9.99
+				Aquaviário - arquivo CTeModalAquaviario_v9.99
+				Ferroviário - arquivo CTeModalFerroviario_v9.99
+				Dutoviário - arquivo CTeModalDutoviario_v9.99
+
+Onde v9.99 é a a designação genérica para a versão do arquivo. Por exemplo, o arquivo para o schema do modal Rodoviário na versão 1.04 será denominado &quot;CTeModalRodoviario_v1.04&quot;.</xs:documentation>
+                    </xs:annotation>
+                  </xs:any>
+                </xs:sequence>
+                <xs:attribute name="versaoModal" use="required">
+                  <xs:annotation>
+                    <xs:documentation>Versão do leiaute específico para o Modal</xs:documentation>
+                  </xs:annotation>
+                  <xs:simpleType>
+                    <xs:restriction base="xs:string">
+                      <xs:whiteSpace value="preserve"/>
+                      <xs:pattern value="4\.(0[0-9]|[1-9][0-9])"/>
+                    </xs:restriction>
+                  </xs:simpleType>
+                </xs:attribute>
+              </xs:complexType>
+            </xs:element>
+            <xs:element name="cobr" minOccurs="0">
+              <xs:annotation>
+                <xs:documentation>Dados da cobrança do CT-e</xs:documentation>
+              </xs:annotation>
+              <xs:complexType>
+                <xs:sequence>
+                  <xs:element name="fat" minOccurs="0">
+                    <xs:annotation>
+                      <xs:documentation>Dados da fatura</xs:documentation>
+                    </xs:annotation>
+                    <xs:complexType>
+                      <xs:sequence>
+                        <xs:element name="nFat" minOccurs="0">
+                          <xs:annotation>
+                            <xs:documentation>Número da fatura</xs:documentation>
+                          </xs:annotation>
+                          <xs:simpleType>
+                            <xs:restriction base="TString">
+                              <xs:minLength value="1"/>
+                              <xs:maxLength value="60"/>
+                            </xs:restriction>
+                          </xs:simpleType>
+                        </xs:element>
+                        <xs:element name="vOrig" type="TDec_1302Opc" minOccurs="0">
+                          <xs:annotation>
+                            <xs:documentation>Valor original da fatura</xs:documentation>
+                          </xs:annotation>
+                        </xs:element>
+                        <xs:element name="vDesc" type="TDec_1302Opc" minOccurs="0">
+                          <xs:annotation>
+                            <xs:documentation>Valor do desconto da fatura</xs:documentation>
+                          </xs:annotation>
+                        </xs:element>
+                        <xs:element name="vLiq" type="TDec_1302Opc" minOccurs="0">
+                          <xs:annotation>
+                            <xs:documentation>Valor líquido da fatura</xs:documentation>
+                          </xs:annotation>
+                        </xs:element>
+                      </xs:sequence>
+                    </xs:complexType>
+                  </xs:element>
+                  <xs:element name="dup" minOccurs="0" maxOccurs="unbounded">
+                    <xs:annotation>
+                      <xs:documentation>Dados das duplicatas</xs:documentation>
+                    </xs:annotation>
+                    <xs:complexType>
+                      <xs:sequence>
+                        <xs:element name="nDup" minOccurs="0">
+                          <xs:annotation>
+                            <xs:documentation>Número da duplicata</xs:documentation>
+                          </xs:annotation>
+                          <xs:simpleType>
+                            <xs:restriction base="TString">
+                              <xs:maxLength value="60"/>
+                              <xs:minLength value="1"/>
+                            </xs:restriction>
+                          </xs:simpleType>
+                        </xs:element>
+                        <xs:element name="dVenc" type="TData" minOccurs="0">
+                          <xs:annotation>
+                            <xs:documentation>Data de vencimento da duplicata (AAAA-MM-DD)</xs:documentation>
+                          </xs:annotation>
+                        </xs:element>
+                        <xs:element name="vDup" type="TDec_1302Opc" minOccurs="0">
+                          <xs:annotation>
+                            <xs:documentation>Valor da duplicata</xs:documentation>
+                          </xs:annotation>
+                        </xs:element>
+                      </xs:sequence>
+                    </xs:complexType>
+                  </xs:element>
+                </xs:sequence>
+              </xs:complexType>
+            </xs:element>
+            <xs:element name="infCteSub" minOccurs="0">
+              <xs:annotation>
+                <xs:documentation>Informações do CT-e de substituição</xs:documentation>
+              </xs:annotation>
+              <xs:complexType>
+                <xs:sequence>
+                  <xs:element name="chCte">
+                    <xs:annotation>
+                      <xs:documentation>Chave de acesso do CT-e a ser substituído (original)</xs:documentation>
+                    </xs:annotation>
+                    <xs:simpleType>
+                      <xs:restriction base="xs:string">
+                        <xs:pattern value="[0-9]{44}"/>
+                      </xs:restriction>
+                    </xs:simpleType>
+                  </xs:element>
+                  <xs:element name="indAlteraToma" minOccurs="0">
+                    <xs:annotation>
+                      <xs:documentation>Indicador de CT-e Alteração de Tomador</xs:documentation>
+                    </xs:annotation>
+                    <xs:simpleType>
+                      <xs:restriction base="xs:string">
+                        <xs:enumeration value="1"/>
+                      </xs:restriction>
+                    </xs:simpleType>
+                  </xs:element>
+                </xs:sequence>
+              </xs:complexType>
+            </xs:element>
+            <xs:element name="imp">
+              <xs:annotation>
+                <xs:documentation>Informações relativas aos Impostos</xs:documentation>
+              </xs:annotation>
+              <xs:complexType>
+                <xs:sequence>
+                  <xs:element name="ICMS" type="TImp">
+                    <xs:annotation>
+                      <xs:documentation>Informações relativas ao ICMS</xs:documentation>
+                      <xs:documentation/>
+                    </xs:annotation>
+                  </xs:element>
+                  <xs:element name="vTotTrib" type="TDec_1302" minOccurs="0">
+                    <xs:annotation>
+                      <xs:documentation>Valor Total dos Tributos</xs:documentation>
+                    </xs:annotation>
+                  </xs:element>
+                  <xs:element name="infAdFisco" minOccurs="0">
+                    <xs:annotation>
+                      <xs:documentation>Informações adicionais de interesse do Fisco</xs:documentation>
+                      <xs:documentation>Norma referenciada, informações complementares, etc</xs:documentation>
+                    </xs:annotation>
+                    <xs:simpleType>
+                      <xs:restriction base="TString">
+                        <xs:maxLength value="2000"/>
+                        <xs:minLength value="1"/>
+                      </xs:restriction>
+                    </xs:simpleType>
+                  </xs:element>
+                  <xs:element name="ICMSUFFim" minOccurs="0">
+                    <xs:annotation>
+                      <xs:documentation>Informações do ICMS de partilha com a UF de término do serviço de transporte na operação interestadual</xs:documentation>
+                      <xs:documentation>Grupo a ser informado nas prestações interestaduais para consumidor final, não contribuinte do ICMS</xs:documentation>
+                    </xs:annotation>
+                    <xs:complexType>
+                      <xs:sequence>
+                        <xs:element name="vBCUFFim" type="TDec_1302">
+                          <xs:annotation>
+                            <xs:documentation>Valor da BC do ICMS na UF de término da prestação do serviço de transporte</xs:documentation>
+                          </xs:annotation>
+                        </xs:element>
+                        <xs:element name="pFCPUFFim" type="TDec_0302">
+                          <xs:annotation>
+                            <xs:documentation>Percentual do ICMS relativo ao Fundo de Combate à pobreza (FCP) na UF de término da prestação do serviço de transporte</xs:documentation>
+                            <xs:documentation>Alíquota adotada nas operações internas na UF do destinatário</xs:documentation>
+                          </xs:annotation>
+                        </xs:element>
+                        <xs:element name="pICMSUFFim" type="TDec_0302">
+                          <xs:annotation>
+                            <xs:documentation>Alíquota interna da UF de término da prestação do serviço de transporte</xs:documentation>
+                            <xs:documentation>Alíquota adotada nas operações internas na UF do destinatário</xs:documentation>
+                          </xs:annotation>
+                        </xs:element>
+                        <xs:element name="pICMSInter" type="TDec_0302">
+                          <xs:annotation>
+                            <xs:documentation>Alíquota interestadual das UF envolvidas</xs:documentation>
+                            <xs:documentation>Alíquota interestadual das UF envolvidas</xs:documentation>
+                          </xs:annotation>
+                        </xs:element>
+                        <xs:element name="vFCPUFFim" type="TDec_1302">
+                          <xs:annotation>
+                            <xs:documentation>Valor do ICMS relativo ao Fundo de Combate á Pobreza (FCP) da UF de término da prestação</xs:documentation>
+                          </xs:annotation>
+                        </xs:element>
+                        <xs:element name="vICMSUFFim" type="TDec_1302">
+                          <xs:annotation>
+                            <xs:documentation>Valor do ICMS de partilha para a UF de término da prestação do serviço de transporte</xs:documentation>
+                          </xs:annotation>
+                        </xs:element>
+                        <xs:element name="vICMSUFIni" type="TDec_1302">
+                          <xs:annotation>
+                            <xs:documentation>Valor do ICMS de partilha para a UF de início da prestação do serviço de transporte</xs:documentation>
+                          </xs:annotation>
+                        </xs:element>
+                      </xs:sequence>
+                    </xs:complexType>
+                  </xs:element>
+                </xs:sequence>
+              </xs:complexType>
+            </xs:element>
+            <xs:element name="total">
+              <xs:annotation>
+                <xs:documentation>Valores Totais do CTe</xs:documentation>
+              </xs:annotation>
+              <xs:complexType>
+                <xs:sequence>
+                  <xs:element name="vTPrest" type="TDec_1302">
+                    <xs:annotation>
+                      <xs:documentation>Valor Total da Prestação do Serviço</xs:documentation>
+                      <xs:documentation>Pode conter zeros quando o CT-e for de complemento de ICMS</xs:documentation>
+                    </xs:annotation>
+                  </xs:element>
+                  <xs:element name="vTRec" type="TDec_1302">
+                    <xs:annotation>
+                      <xs:documentation>Valor total a Receber</xs:documentation>
+                    </xs:annotation>
+                  </xs:element>
+                </xs:sequence>
+              </xs:complexType>
+            </xs:element>
+            <xs:element name="autXML" minOccurs="0" maxOccurs="10">
+              <xs:annotation>
+                <xs:documentation>Autorizados para download do XML do DF-e</xs:documentation>
+                <xs:documentation>Informar CNPJ ou CPF. Preencher os zeros não significativos.</xs:documentation>
+              </xs:annotation>
+              <xs:complexType>
+                <xs:sequence>
+                  <xs:choice>
+                    <xs:element name="CNPJ" type="TCnpj">
+                      <xs:annotation>
+                        <xs:documentation>CNPJ do autorizado</xs:documentation>
+                        <xs:documentation>Informar zeros não significativos</xs:documentation>
+                      </xs:annotation>
+                    </xs:element>
+                    <xs:element name="CPF" type="TCpf">
+                      <xs:annotation>
+                        <xs:documentation>CPF do autorizado</xs:documentation>
+                        <xs:documentation>Informar zeros não significativos</xs:documentation>
+                      </xs:annotation>
+                    </xs:element>
+                  </xs:choice>
+                </xs:sequence>
+              </xs:complexType>
+            </xs:element>
+            <xs:element name="infRespTec" type="TRespTec" minOccurs="0">
+              <xs:annotation>
+                <xs:documentation>Informações do Responsável Técnico pela emissão do DF-e</xs:documentation>
+              </xs:annotation>
+            </xs:element>
+            <xs:element name="infSolicNFF" minOccurs="0">
+              <xs:annotation>
+                <xs:documentation>Grupo de informações do pedido de emissão da Nota Fiscal Fácil</xs:documentation>
+              </xs:annotation>
+              <xs:complexType>
+                <xs:sequence>
+                  <xs:element name="xSolic">
+                    <xs:annotation>
+                      <xs:documentation>Solicitação do pedido de emissão da NFF.</xs:documentation>
+                      <xs:documentation>Será preenchido com a totalidade de campos informados no aplicativo emissor serializado.</xs:documentation>
+                    </xs:annotation>
+                    <xs:simpleType>
+                      <xs:restriction base="TString">
+                        <xs:minLength value="2"/>
+                        <xs:maxLength value="2000"/>
+                      </xs:restriction>
+                    </xs:simpleType>
+                  </xs:element>
+                </xs:sequence>
+              </xs:complexType>
+            </xs:element>
+            <xs:element name="infPAA" minOccurs="0">
+              <xs:annotation>
+                <xs:documentation>Grupo de Informação do Provedor de Assinatura e Autorização</xs:documentation>
+              </xs:annotation>
+              <xs:complexType>
+                <xs:sequence>
+                  <xs:element name="CNPJPAA" type="TCnpj">
+                    <xs:annotation>
+                      <xs:documentation>CNPJ do Provedor de Assinatura e Autorização</xs:documentation>
+                    </xs:annotation>
+                  </xs:element>
+                  <xs:element name="PAASignature">
+                    <xs:annotation>
+                      <xs:documentation>Assinatura RSA do Emitente para DFe gerados por PAA</xs:documentation>
+                    </xs:annotation>
+                    <xs:complexType>
+                      <xs:sequence>
+                        <xs:element name="SignatureValue" type="xs:base64Binary">
+                          <xs:annotation>
+                            <xs:documentation>Assinatura digital padrão RSA</xs:documentation>
+                            <xs:documentation>Converter o atributo Id do DFe para array de bytes e assinar com a chave privada do RSA com algoritmo SHA1 gerando um valor no formato base64.</xs:documentation>
+                          </xs:annotation>
+                        </xs:element>
+                        <xs:element name="RSAKeyValue" type="TRSAKeyValueType">
+                          <xs:annotation>
+                            <xs:documentation>Chave Publica no padrão XML RSA Key</xs:documentation>
+                          </xs:annotation>
+                        </xs:element>
+                      </xs:sequence>
+                    </xs:complexType>
+                  </xs:element>
+                </xs:sequence>
+              </xs:complexType>
+            </xs:element>
+          </xs:sequence>
+          <xs:attribute name="versao" use="required">
+            <xs:annotation>
+              <xs:documentation>Versão do leiaute</xs:documentation>
+              <xs:documentation>Ex: &quot;4.00&quot;</xs:documentation>
+            </xs:annotation>
+            <xs:simpleType>
+              <xs:restriction base="TVerCTe"/>
+            </xs:simpleType>
+          </xs:attribute>
+          <xs:attribute name="Id" use="required">
+            <xs:annotation>
+              <xs:documentation>Identificador da tag a ser assinada</xs:documentation>
+              <xs:documentation>Informar a chave de acesso do CT-e e precedida do literal &quot;CTe&quot;</xs:documentation>
+            </xs:annotation>
+            <xs:simpleType>
+              <xs:restriction base="xs:ID">
+                <xs:pattern value="CTe[0-9]{44}"/>
+              </xs:restriction>
+            </xs:simpleType>
+          </xs:attribute>
+        </xs:complexType>
+        <xs:unique name="pk_nItem">
+          <xs:selector xpath="det"/>
+          <xs:field xpath="@nItem"/>
+        </xs:unique>
+      </xs:element>
+      <xs:element name="infCTeSupl" minOccurs="0">
+        <xs:annotation>
+          <xs:documentation>Informações suplementares do CT-e</xs:documentation>
+        </xs:annotation>
+        <xs:complexType>
+          <xs:sequence>
+            <xs:element name="qrCodCTe">
+              <xs:annotation>
+                <xs:documentation>Texto com o QR-Code impresso no DACTE</xs:documentation>
+              </xs:annotation>
+              <xs:simpleType>
+                <xs:restriction base="xs:string">
+                  <xs:whiteSpace value="preserve"/>
+                  <xs:minLength value="50"/>
+                  <xs:maxLength value="1000"/>
+                  <xs:pattern value="((HTTPS?|https?)://.*\?chCTe=[0-9]{44}&amp;tpAmb=[1-2](&amp;sign=[!-ÿ]{1}[ -ÿ]{0,}[!-ÿ]{1}|[!-ÿ]{1})?)"/>
+                </xs:restriction>
+              </xs:simpleType>
+            </xs:element>
+          </xs:sequence>
+        </xs:complexType>
+      </xs:element>
+      <xs:element ref="ds:Signature"/>
+    </xs:sequence>
+  </xs:complexType>
   <xs:complexType name="TCTe">
     <xs:annotation>
       <xs:documentation>Tipo Conhecimento de Transporte Eletrônico (Modelo 57)</xs:documentation>
     </xs:annotation>
     <xs:sequence>
       <xs:element name="infCte">
         <xs:annotation>
@@ -1513,16 +2885,19 @@
 02-Aéreo;03-Aquaviário;04-Ferroviário;05-Dutoviário;06-Multimodal;</xs:documentation>
                     </xs:annotation>
                   </xs:element>
                   <xs:element name="tpServ">
                     <xs:annotation>
                       <xs:documentation>Tipo do Serviço</xs:documentation>
                       <xs:documentation>Preencher com: 
-0 - Normal;1 - Subcontratação;
-2 - Redespacho;3 - Redespacho Intermediário; 4 - Serviço Vinculado a Multimodal</xs:documentation>
+0 - Normal;
+1 - Subcontratação;
+2 - Redespacho;
+3 - Redespacho Intermediário; 
+4 - Serviço Vinculado a Multimodal</xs:documentation>
                     </xs:annotation>
                     <xs:simpleType>
                       <xs:restriction base="xs:string">
                         <xs:whiteSpace value="preserve"/>
                         <xs:enumeration value="0"/>
                         <xs:enumeration value="1"/>
                         <xs:enumeration value="2"/>
@@ -3657,17 +5032,17 @@
                       </xs:restriction>
                     </xs:simpleType>
                   </xs:element>
                   <xs:element name="tpEmis">
                     <xs:annotation>
                       <xs:documentation>Forma de emissão do CT-e</xs:documentation>
                       <xs:documentation>Preencher com:
- 1 - Normal;
+1 - Normal;
  5 - Contingência FSDA;
- 7 - Autorização pela SVC-RS;
+7 - Autorização pela SVC-RS;
  8 - Autorização pela SVC-SP</xs:documentation>
                     </xs:annotation>
                     <xs:simpleType>
                       <xs:restriction base="xs:string">
                         <xs:whiteSpace value="preserve"/>
                         <xs:enumeration value="1"/>
                         <xs:enumeration value="5"/>
@@ -6413,14 +7788,24 @@
     <xs:restriction base="xs:string">
       <xs:whiteSpace value="preserve"/>
       <xs:enumeration value="0"/>
       <xs:enumeration value="1"/>
       <xs:enumeration value="3"/>
     </xs:restriction>
   </xs:simpleType>
+  <xs:simpleType name="TFinCTeSimp">
+    <xs:annotation>
+      <xs:documentation>Tipos Finalidade de CT-e Simplificado</xs:documentation>
+    </xs:annotation>
+    <xs:restriction base="xs:string">
+      <xs:whiteSpace value="preserve"/>
+      <xs:enumeration value="4"/>
+      <xs:enumeration value="5"/>
+    </xs:restriction>
+  </xs:simpleType>
   <xs:simpleType name="TIdLote">
     <xs:annotation>
       <xs:documentation>Tipo Identificador de controle do envio do lote. Número seqüencial auto-incremental, de controle correspondente ao identificador único do lote enviado. A responsabilidade de gerar e controlar esse número é do próprio contribuinte.</xs:documentation>
     </xs:annotation>
     <xs:restriction base="xs:string">
       <xs:whiteSpace value="preserve"/>
       <xs:pattern value="[0-9]{1,15}"/>
@@ -6485,14 +7870,25 @@
       <xs:enumeration value="02"/>
       <xs:enumeration value="03"/>
       <xs:enumeration value="04"/>
       <xs:enumeration value="05"/>
       <xs:enumeration value="06"/>
     </xs:restriction>
   </xs:simpleType>
+  <xs:simpleType name="TModTranspSimp">
+    <xs:annotation>
+      <xs:documentation>Tipo Modal transporte do CTe Simplificado</xs:documentation>
+    </xs:annotation>
+    <xs:restriction base="xs:string">
+      <xs:whiteSpace value="preserve"/>
+      <xs:enumeration value="01"/>
+      <xs:enumeration value="02"/>
+      <xs:enumeration value="03"/>
+    </xs:restriction>
+  </xs:simpleType>
   <xs:simpleType name="TRNTRC">
     <xs:annotation>
       <xs:documentation>Tipo RNTRC - Registro Nacional Transportadores Rodoviários de Carga</xs:documentation>
     </xs:annotation>
     <xs:restriction base="xs:string">
       <xs:whiteSpace value="preserve"/>
       <xs:pattern value="[0-9]{8}|ISENTO"/>
```

## Comparing `nfelib-2.0.4/nfelib/cte/schemas/v4_0/evGTV_v4.00.xsd` & `nfelib-2.0.5/nfelib/cte/schemas/v4_0/evGTV_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte/schemas/v4_0/retEventoCTe_v4.00.xsd` & `nfelib-2.0.5/nfelib/cte/schemas/v4_0/retEventoCTe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte/schemas/v4_0/cteModalFerroviario_v4.00.xsd` & `nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteModalFerroviario_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte/schemas/v4_0/evCCeCTe_v4.00.xsd` & `nfelib-2.0.5/nfelib/cte/schemas/v4_0/evCCeCTe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte/schemas/v4_0/eventoCTe_v4.00.xsd` & `nfelib-2.0.5/nfelib/cte/schemas/v4_0/eventoCTe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte/schemas/v4_0/evRegMultimodal_v4.00.xsd` & `nfelib-2.0.5/nfelib/cte/schemas/v4_0/evRegMultimodal_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte/schemas/v4_0/retCTeOS_v4.00.xsd` & `nfelib-2.0.5/nfelib/cte/schemas/v4_0/retCTeOS_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte/schemas/v4_0/retGTVe_v4.00.xsd` & `nfelib-2.0.5/nfelib/cte/schemas/v4_0/retGTVe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte/schemas/v4_0/retCTe_v4.00.xsd` & `nfelib-2.0.5/nfelib/cte/schemas/v4_0/retCTe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte/schemas/v4_0/evPrestDesacordo_v4.00.xsd` & `nfelib-2.0.5/nfelib/cte/schemas/v4_0/evPrestDesacordo_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte/schemas/v4_0/inutCTeTiposBasico_v4.00.xsd` & `nfelib-2.0.5/nfelib/cte/schemas/v4_0/inutCTeTiposBasico_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte/schemas/v4_0/evIECTe_v4.00.xsd` & `nfelib-2.0.5/nfelib/cte/schemas/v4_0/evIECTe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte/schemas/v4_0/evCancPrestDesacordo_v4.00.xsd` & `nfelib-2.0.5/nfelib/cte/schemas/v4_0/evCancPrestDesacordo_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte/schemas/v4_0/retConsStatServCTe_v4.00.xsd` & `nfelib-2.0.5/nfelib/cte/schemas/v4_0/retConsStatServCTe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte/schemas/v4_0/consStatServTiposBasico_v4.00.xsd` & `nfelib-2.0.5/nfelib/cte/schemas/v4_0/consStatServTiposBasico_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte/schemas/v4_0/cteModalAereo_v4.00.xsd` & `nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteModalAereo_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte/schemas/v4_0/procGTVe_v4.00.xsd` & `nfelib-2.0.5/nfelib/cte/schemas/v4_0/procGTVe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte/schemas/v4_0/evEPECCTe_v4.00.xsd` & `nfelib-2.0.5/nfelib/cte/schemas/v4_0/evEPECCTe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte/schemas/v4_0/cteModalRodoviarioOS_v4.00.xsd` & `nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteModalRodoviarioOS_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte/schemas/v4_0/cteModalDutoviario_v4.00.xsd` & `nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteModalDutoviario_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte/schemas/v4_0/tiposGeralCTe_v4.00.xsd` & `nfelib-2.0.5/nfelib/cte/schemas/v4_0/tiposGeralCTe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte/schemas/v4_0/GTVe_v4.00.xsd` & `nfelib-2.0.5/nfelib/cte/schemas/v4_0/GTVe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte/schemas/v4_0/evCancIECTe_v4.00.xsd` & `nfelib-2.0.5/nfelib/cte/schemas/v4_0/evCancIECTe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte/schemas/v4_0/cteMultiModal_v4.00.xsd` & `nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteMultiModal_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte/schemas/v4_0/retInutCTe_v4.00.xsd` & `nfelib-2.0.5/nfelib/cte/schemas/v4_0/retInutCTe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte/schemas/v4_0/procEventoCTe_v4.00.xsd` & `nfelib-2.0.5/nfelib/cte/schemas/v4_0/procEventoCTe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte/schemas/v4_0/evCECTe_v4.00.xsd` & `nfelib-2.0.5/nfelib/cte/schemas/v4_0/evCECTe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte/schemas/v4_0/inutCTe_v4.00.xsd` & `nfelib-2.0.5/nfelib/cte/schemas/v4_0/inutCTe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte/schemas/v4_0/eventoCTeTiposBasico_v4.00.xsd` & `nfelib-2.0.5/nfelib/cte/schemas/v4_0/eventoCTeTiposBasico_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte/schemas/v4_0/cteOS_v4.00.xsd` & `nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteOS_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte/schemas/v4_0/consSitCTeTiposBasico_v4.00.xsd` & `nfelib-2.0.5/nfelib/cte/schemas/v4_0/consSitCTeTiposBasico_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte/schemas/v4_0/consStatServCTe_v4.00.xsd` & `nfelib-2.0.5/nfelib/cte/schemas/v4_0/consStatServCTe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte/schemas/v4_0/procCTeOS_v4.00.xsd` & `nfelib-2.0.5/nfelib/cte/schemas/v4_0/procCTeOS_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte/schemas/v4_0/retConsSitCTe_v4.00.xsd` & `nfelib-2.0.5/nfelib/cte/schemas/v4_0/retConsSitCTe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte/schemas/v4_0/consSitCTe_v4.00.xsd` & `nfelib-2.0.5/nfelib/cte/schemas/v4_0/consSitCTe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte/schemas/v4_0/cteModalAquaviario_v4.00.xsd` & `nfelib-2.0.5/nfelib/cte/schemas/v4_0/cteModalAquaviario_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte/schemas/v4_0/cte_v4.00.xsd` & `nfelib-2.0.5/nfelib/cte/schemas/v4_0/cte_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte/schemas/v4_0/procInutCTe_v4.00.xsd` & `nfelib-2.0.5/nfelib/cte/schemas/v4_0/procInutCTe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte/schemas/v4_0/procCTe_v4.00.xsd` & `nfelib-2.0.5/nfelib/cte/schemas/v4_0/procCTe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte/schemas/v4_0/evCancCECTe_v4.00.xsd` & `nfelib-2.0.5/nfelib/cte/schemas/v4_0/evCancCECTe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte/schemas/v4_0/evCancCTe_v4.00.xsd` & `nfelib-2.0.5/nfelib/cte/schemas/v4_0/evCancCTe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/cte/schemas/v4_0/xmldsig-core-schema_v1.01.xsd` & `nfelib-2.0.5/nfelib/nfe_ator_interessado/schemas/v1_0/xmldsig-core-schema_v1.01.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_generico/bindings/v1_0/xmldsig_core_schema_v1_01.py` & `nfelib-2.0.5/nfelib/nfe/bindings/v4_0/xmldsig_core_schema_v1_01.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:16:22
+"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:31:20
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass, field
 from enum import Enum
 from nfelib import CommonMixin
```

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_generico/bindings/v1_0/__init__.py` & `nfelib-2.0.5/nfelib/nfe_evento_generico/bindings/v1_0/__init__.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_generico/bindings/v1_0/env_evento_v1_00.py` & `nfelib-2.0.5/nfelib/nfe_evento_generico/bindings/v1_0/env_evento_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_generico/bindings/v1_0/ret_env_evento_v1_00.py` & `nfelib-2.0.5/nfelib/nfe_evento_generico/bindings/v1_0/proc_evento_nfe_v1_00.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """This file was generated by xsdata, v24.2.1, on 2024-02-24 11:16:22
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass
 from nfelib.nfe_evento_generico.bindings.v1_0.leiaute_evento_v1_00 import (
-    TretEnvEvento,
+    TprocEvento,
 )
 
 __NAMESPACE__ = "http://www.portalfiscal.inf.br/nfe"
 
 
 @dataclass
-class RetEnvEvento(TretEnvEvento):
+class ProcEventoNfe(TprocEvento):
     """
-    Schema XML de Retorno da envio do Evento.
+    Schema XML de validação do proc Evento NFe.
     """
 
     class Meta:
-        name = "retEnvEvento"
+        name = "procEventoNFe"
         namespace = "http://www.portalfiscal.inf.br/nfe"
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_generico/bindings/v1_0/proc_evento_nfe_v1_00.py` & `nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/evento_insucesso_nfe_v1_00.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:16:22
+"""This file was generated by xsdata, v24.4, on 2024-05-08 08:25:46
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass
-from nfelib.nfe_evento_generico.bindings.v1_0.leiaute_evento_v1_00 import (
-    TprocEvento,
+
+from nfelib.nfe_insucesso.bindings.v1_0.leiaute_evento_insucesso_nfe_v1_00 import (
+    Tevento,
 )
 
 __NAMESPACE__ = "http://www.portalfiscal.inf.br/nfe"
 
 
 @dataclass
-class ProcEventoNfe(TprocEvento):
+class Evento(Tevento):
     """
-    Schema XML de validação do proc Evento NFe.
+    Schema XML de validação do evento de Insucesso na entrega da NF-e.
     """
 
     class Meta:
-        name = "procEventoNFe"
+        name = "evento"
         namespace = "http://www.portalfiscal.inf.br/nfe"
```

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_generico/bindings/v1_0/leiaute_evento_v1_00.py` & `nfelib-2.0.5/nfelib/nfe_evento_generico/bindings/v1_0/leiaute_evento_v1_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_generico/schemas/v1_0/envEvento_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfe_evento_generico/schemas/v1_0/envEvento_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_generico/schemas/v1_0/leiauteEvento_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfe_evento_generico/schemas/v1_0/leiauteEvento_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_generico/schemas/v1_0/procEventoNFe_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfe_evento_generico/schemas/v1_0/procEventoNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_generico/schemas/v1_0/retEnvEvento_v1.00.xsd` & `nfelib-2.0.5/nfelib/nfe_evento_generico/schemas/v1_0/retEnvEvento_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_generico/schemas/v1_0/tiposBasico_v1.03.xsd` & `nfelib-2.0.5/nfelib/nfe_evento_generico/schemas/v1_0/tiposBasico_v1.03.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_evento_generico/schemas/v1_0/xmldsig-core-schema_v1.01.xsd` & `nfelib-2.0.5/nfelib/cte/schemas/v4_0/xmldsig-core-schema_v1.01.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_cons/bindings/v2_0/xmldsig_core_schema_v1_01.py` & `nfelib-2.0.5/nfelib/nfe_cons/bindings/v2_0/xmldsig_core_schema_v1_01.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_cons/bindings/v2_0/tipos_basico_v1_03.py` & `nfelib-2.0.5/nfelib/nfe_cons/bindings/v2_0/tipos_basico_v1_03.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_cons/bindings/v2_0/__init__.py` & `nfelib-2.0.5/nfelib/nfe_cons/bindings/v2_0/__init__.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_cons/bindings/v2_0/cons_sit_nfe_v2_01.py` & `nfelib-2.0.5/nfelib/nfe_cons/bindings/v2_0/cons_sit_nfe_v2_01.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_cons/bindings/v2_0/leiaute_cons_sit_nfe_v2_01.py` & `nfelib-2.0.5/nfelib/nfe_cons/bindings/v2_0/leiaute_cons_sit_nfe_v2_01.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_cons/bindings/v2_0/ret_cons_sit_nfe_v2_01.py` & `nfelib-2.0.5/nfelib/nfe_cons/bindings/v2_0/ret_cons_sit_nfe_v2_01.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_cons/schemas/v2_0/consSitNFe_v2.01.xsd` & `nfelib-2.0.5/nfelib/nfe_cons/schemas/v2_0/consSitNFe_v2.01.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_cons/schemas/v2_0/leiauteConsSitNFe_v2.01.xsd` & `nfelib-2.0.5/nfelib/nfe_cons/schemas/v2_0/leiauteConsSitNFe_v2.01.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_cons/schemas/v2_0/tiposBasico_v1.03.xsd` & `nfelib-2.0.5/nfelib/nfe_cons/schemas/v2_0/tiposBasico_v1.03.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_cons/schemas/v2_0/xmldsig-core-schema_v1.01.xsd` & `nfelib-2.0.5/nfelib/nfe_evento_generico/schemas/v1_0/xmldsig-core-schema_v1.01.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe_cons/schemas/v2_0/retConsSitNFe_v2.01.xsd` & `nfelib-2.0.5/nfelib/nfe_cons/schemas/v2_0/retConsSitNFe_v2.01.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476711079516696-nfe.xml` & `nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476711079516696-nfe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteNFe/42220575277525000178550030000292481295366801-procNFe.xml` & `nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/42220575277525000178550030000292481295366801-procNFe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000474491454651420-nfe.xml` & `nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000474491454651420-nfe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476051695511860-nfe.xml` & `nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476051695511860-nfe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476491552806942-nfe.xml` & `nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476491552806942-nfe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteNFe/41170706117473000150550010000463202612756525-procNFe.xml` & `nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/41170706117473000150550010000463202612756525-procNFe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476861118934859-nfe.xml` & `nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476861118934859-nfe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteNFe/42210775277525000178550030000266631762885493-procNFe.xml` & `nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/42210775277525000178550030000266631762885493-procNFe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476781421693968-nfe.xml` & `nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476781421693968-nfe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteNFe/42211275277525000178550030000276771368212013-procNFe.xml` & `nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/42211275277525000178550030000276771368212013-procNFe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteNFe/26180875335849000115550010000016871192213331-nfe.xml` & `nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/26180875335849000115550010000016871192213331-nfe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476121675985748-nfe.xml` & `nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000476121675985748-nfe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000474501597356342-nfe.xml` & `nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000474501597356342-nfe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteNFe/NFe35200159594315000157550010000000012062777161.xml` & `nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/NFe35200159594315000157550010000000012062777161.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000474281920007498-nfe.xml` & `nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000474281920007498-nfe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000474641681223493-nfe.xml` & `nfelib-2.0.5/nfelib/nfe/samples/v4_0/leiauteNFe/35180834128745000152550010000474641681223493-nfe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe/bindings/v4_0/leiaute_cons_sit_nfe_v4_00.py` & `nfelib-2.0.5/nfelib/nfe/bindings/v4_0/leiaute_cons_sit_nfe_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe/bindings/v4_0/ret_cons_sit_nfe_v4_00.py` & `nfelib-2.0.5/nfelib/nfe/bindings/v4_0/cons_stat_serv_v4_00.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """This file was generated by xsdata, v24.2.1, on 2024-02-24 11:31:20
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass
-from nfelib.nfe.bindings.v4_0.leiaute_cons_sit_nfe_v4_00 import TretConsSitNfe
+from nfelib.nfe.bindings.v4_0.leiaute_cons_stat_serv_v4_00 import TconsStatServ
 
 __NAMESPACE__ = "http://www.portalfiscal.inf.br/nfe"
 
 
 @dataclass
-class RetConsSitNfe(TretConsSitNfe):
+class ConsStatServ(TconsStatServ):
     """
-    Schema XML de validação do retorno da consulta da situação atual da NF-e.
+    Schema XML de validação do Pedido de Consulta do Status do Serviço.
     """
 
     class Meta:
-        name = "retConsSitNFe"
+        name = "consStatServ"
         namespace = "http://www.portalfiscal.inf.br/nfe"
```

## Comparing `nfelib-2.0.4/nfelib/nfe/bindings/v4_0/cons_cad_v2_00.py` & `nfelib-2.0.5/nfelib/nfe/bindings/v4_0/cons_cad_v2_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe/bindings/v4_0/xmldsig_core_schema_v1_01.py` & `nfelib-2.0.5/nfelib/nfse/bindings/v1_0/xmldsig_core_schema_v1_00.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:31:20
+"""This file was generated by xsdata, v24.2.1, on 2024-03-11 16:13:50
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass, field
 from enum import Enum
 from nfelib import CommonMixin
```

## Comparing `nfelib-2.0.4/nfelib/nfe/bindings/v4_0/__init__.py` & `nfelib-2.0.5/nfelib/nfe/bindings/v4_0/__init__.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe/bindings/v4_0/ret_inut_nfe_v4_00.py` & `nfelib-2.0.5/nfelib/nfe/bindings/v4_0/ret_inut_nfe_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe/bindings/v4_0/inut_nfe_v4_00.py` & `nfelib-2.0.5/nfelib/nfe/bindings/v4_0/inut_nfe_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe/bindings/v4_0/cons_reci_nfe_v4_00.py` & `nfelib-2.0.5/nfelib/nfe/bindings/v4_0/cons_reci_nfe_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe/bindings/v4_0/tipos_basico_v4_00.py` & `nfelib-2.0.5/nfelib/nfe/bindings/v4_0/tipos_basico_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe/bindings/v4_0/ret_cons_stat_serv_v4_00.py` & `nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/env_evento_insucesso_nfe_v1_00.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:31:20
+"""This file was generated by xsdata, v24.4, on 2024-05-08 08:25:46
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass
-from nfelib.nfe.bindings.v4_0.leiaute_cons_stat_serv_v4_00 import (
-    TretConsStatServ,
+
+from nfelib.nfe_insucesso.bindings.v1_0.leiaute_evento_insucesso_nfe_v1_00 import (
+    TenvEvento,
 )
 
 __NAMESPACE__ = "http://www.portalfiscal.inf.br/nfe"
 
 
 @dataclass
-class RetConsStatServ(TretConsStatServ):
+class EnvEvento(TenvEvento):
     """
-    Schema XML de validação do Resultado da Consulta do Status do Serviço.
+    Schema XML de validação do lote de envio do evento de Insucesso na Entrega da
+    NF-e.
     """
 
     class Meta:
-        name = "retConsStatServ"
+        name = "envEvento"
         namespace = "http://www.portalfiscal.inf.br/nfe"
```

## Comparing `nfelib-2.0.4/nfelib/nfe/bindings/v4_0/leiaute_consulta_cadastro_v2_00.py` & `nfelib-2.0.5/nfelib/nfe/bindings/v4_0/leiaute_consulta_cadastro_v2_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe/bindings/v4_0/cons_stat_serv_v4_00.py` & `nfelib-2.0.5/nfelib/nfe/bindings/v4_0/ret_cons_cad_v2_00.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """This file was generated by xsdata, v24.2.1, on 2024-02-24 11:31:20
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass
-from nfelib.nfe.bindings.v4_0.leiaute_cons_stat_serv_v4_00 import TconsStatServ
+from nfelib.nfe.bindings.v4_0.leiaute_consulta_cadastro_v2_00 import (
+    TretConsCad,
+)
 
 __NAMESPACE__ = "http://www.portalfiscal.inf.br/nfe"
 
 
 @dataclass
-class ConsStatServ(TconsStatServ):
+class RetConsCad(TretConsCad):
     """
-    Schema XML de validação do Pedido de Consulta do Status do Serviço.
+    Schema XML de validação do retorno da consulta cadastro contribuintes.
     """
 
     class Meta:
-        name = "consStatServ"
+        name = "retConsCad"
         namespace = "http://www.portalfiscal.inf.br/nfe"
```

## Comparing `nfelib-2.0.4/nfelib/nfe/bindings/v4_0/leiaute_inut_nfe_v4_00.py` & `nfelib-2.0.5/nfelib/nfe/bindings/v4_0/leiaute_inut_nfe_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe/bindings/v4_0/cons_sit_nfe_v4_00.py` & `nfelib-2.0.5/nfelib/nfe/bindings/v4_0/cons_sit_nfe_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe/bindings/v4_0/ret_cons_reci_nfe_v4_00.py` & `nfelib-2.0.5/nfelib/nfe/bindings/v4_0/ret_cons_reci_nfe_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe/bindings/v4_0/leiaute_cons_stat_serv_v4_00.py` & `nfelib-2.0.5/nfelib/nfe/bindings/v4_0/leiaute_cons_stat_serv_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe/bindings/v4_0/envi_nfe_v4_00.py` & `nfelib-2.0.5/nfelib/nfe/bindings/v4_0/ret_envi_nfe_v4_00.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """This file was generated by xsdata, v24.2.1, on 2024-02-24 11:31:20
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass
-from nfelib.nfe.bindings.v4_0.leiaute_nfe_v4_00 import TenviNfe
+from nfelib.nfe.bindings.v4_0.leiaute_nfe_v4_00 import TretEnviNfe
 
 __NAMESPACE__ = "http://www.portalfiscal.inf.br/nfe"
 
 
 @dataclass
-class EnviNfe(TenviNfe):
+class RetEnviNfe(TretEnviNfe):
     """
-    Schema XML de validação do Pedido de Concessão de Autorização da Nota Fiscal
-    Eletrônica.
+    Schema XML de validação do retorno do Pedido de Concessão de Autorização da
+    Nota Fiscal Eletrônica.
     """
 
     class Meta:
-        name = "enviNFe"
+        name = "retEnviNFe"
         namespace = "http://www.portalfiscal.inf.br/nfe"
```

## Comparing `nfelib-2.0.4/nfelib/nfe/bindings/v4_0/proc_inut_nfe_v4_00.py` & `nfelib-2.0.5/nfelib/cte/bindings/v4_0/cons_sit_cte_v4_00.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,23 @@
-"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:31:20
+"""This file was generated by xsdata, v24.4, on 2024-04-08 21:52:20
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass
-from nfelib.nfe.bindings.v4_0.leiaute_inut_nfe_v4_00 import TprocInutNfe
 
-__NAMESPACE__ = "http://www.portalfiscal.inf.br/nfe"
+from nfelib.cte.bindings.v4_0.cons_sit_cte_tipos_basico_v4_00 import (
+    TconsSitCte,
+)
+
+__NAMESPACE__ = "http://www.portalfiscal.inf.br/cte"
 
 
 @dataclass
-class ProcInutNfe(TprocInutNfe):
+class ConsSitCte(TconsSitCte):
     """
-    Pedido de inutilização de númeração de  NF-e processado.
+    Schema de validação XML dp Pedido de Consulta da Situação Atual do CT-e.
     """
 
     class Meta:
-        name = "ProcInutNFe"
-        namespace = "http://www.portalfiscal.inf.br/nfe"
+        name = "consSitCTe"
+        namespace = "http://www.portalfiscal.inf.br/cte"
```

## Comparing `nfelib-2.0.4/nfelib/nfe/bindings/v4_0/ret_envi_nfe_v4_00.py` & `nfelib-2.0.5/nfelib/nfe_insucesso/bindings/v1_0/proc_evento_insucesso_nfe_v1_00.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-"""This file was generated by xsdata, v24.2.1, on 2024-02-24 11:31:20
+"""This file was generated by xsdata, v24.4, on 2024-05-08 08:25:46
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
 from dataclasses import dataclass
-from nfelib.nfe.bindings.v4_0.leiaute_nfe_v4_00 import TretEnviNfe
+
+from nfelib.nfe_insucesso.bindings.v1_0.leiaute_evento_insucesso_nfe_v1_00 import (
+    TprocEvento,
+)
 
 __NAMESPACE__ = "http://www.portalfiscal.inf.br/nfe"
 
 
 @dataclass
-class RetEnviNfe(TretEnviNfe):
+class ProcEventoNfe(TprocEvento):
     """
-    Schema XML de validação do retorno do Pedido de Concessão de Autorização da
-    Nota Fiscal Eletrônica.
+    Schema XML de validação do proc Insucesso na Entrega da NFe.
     """
 
     class Meta:
-        name = "retEnviNFe"
+        name = "procEventoNFe"
         namespace = "http://www.portalfiscal.inf.br/nfe"
```

## Comparing `nfelib-2.0.4/nfelib/nfe/bindings/v4_0/leiaute_nfe_v4_00.py` & `nfelib-2.0.5/nfelib/nfe/bindings/v4_0/leiaute_nfe_v4_00.py`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe/ws/edoc_legacy.py` & `nfelib-2.0.5/nfelib/nfe/ws/edoc_legacy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 # Copyright 2018 - TODAY Luis Felipe Mileo - KMEE INFORMATICA LTDA
 # Copyright 2023 - TODAY Akretion - Raphaël Valyi <raphael.valyi@akretion.com>
 
 from dataclasses import is_dataclass
 import base64
 from lxml import etree
 
+from nfelib.nfe.bindings.v4_0.cons_sit_nfe_v4_00 import ConsSitNfe
+from nfelib.nfe.bindings.v4_0.ret_cons_sit_nfe_v4_00 import RetConsSitNfe
+
 
 from erpbrasil.assinatura.assinatura import Assinatura
 
 try:
     from erpbrasil.edoc.edoc import DocumentoEletronico
     from erpbrasil.edoc.mde import MDe
     from erpbrasil.edoc.mdfe import MDFe
     from erpbrasil.edoc.nfce import NFCe
-    from erpbrasil.edoc.nfe import NFe
+    from erpbrasil.edoc.nfe import NFe, localizar_url, WS_NFE_CONSULTA
     from erpbrasil.edoc.resposta import RetornoSoap, analisar_retorno_raw
 
 
 except ImportError:
     raise RuntimeError(
         "You need to install the erpbrasil.edoc package to use this legacy webservice layer."
     )
@@ -94,15 +97,32 @@
             xml_assinado = Assinatura(self._transmissao.certificado).assina_xml2(
                 xml_etree, id, getchildren
             )
         return xml_assinado.replace('\n', '').replace('\r', '')
 
 
 class NFeAdapter(DocumentoElectronicoAdapter, NFe):
-    pass
+    def consulta_documento(self, chave):
+        raiz = ConsSitNfe(
+            versao=self.versao,
+            tpAmb=self.ambiente,
+            xServ="CONSULTAR",
+            chNFe=chave,
+        )
+        return self._post(
+            raiz=raiz,
+            url=localizar_url(
+                WS_NFE_CONSULTA,
+                str(self.uf),
+                self.mod,
+                int(self.ambiente)
+            ),
+            operacao="nfeConsultaNF",
+            classe=RetConsSitNfe,
+        )
 
 
 class NFCeAdapter(DocumentoElectronicoAdapter, NFCe):
     pass
 
 
 class MDeAdapter(DocumentoElectronicoAdapter, MDe):
```

## Comparing `nfelib-2.0.4/nfelib/nfe/schemas/v4_0/leiauteConsStatServ_v4.00.xsd` & `nfelib-2.0.5/nfelib/nfe/schemas/v4_0/leiauteConsStatServ_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe/schemas/v4_0/retConsReciNFe_v4.00.xsd` & `nfelib-2.0.5/nfelib/nfe/schemas/v4_0/retConsReciNFe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe/schemas/v4_0/consStatServ_v4.00.xsd` & `nfelib-2.0.5/nfelib/nfe/schemas/v4_0/consStatServ_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe/schemas/v4_0/procNFe_v4.00.xsd` & `nfelib-2.0.5/nfelib/nfe/schemas/v4_0/procNFe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe/schemas/v4_0/retInutNFe_v4.00.xsd` & `nfelib-2.0.5/nfelib/nfe/schemas/v4_0/retInutNFe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe/schemas/v4_0/procInutNFe_v4.00.xsd` & `nfelib-2.0.5/nfelib/nfe/schemas/v4_0/procInutNFe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe/schemas/v4_0/consCad_v2.00.xsd` & `nfelib-2.0.5/nfelib/nfe/schemas/v4_0/consCad_v2.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe/schemas/v4_0/leiauteConsSitNFe_v4.00.xsd` & `nfelib-2.0.5/nfelib/nfe/schemas/v4_0/leiauteConsSitNFe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe/schemas/v4_0/nfe_v4.00.xsd` & `nfelib-2.0.5/nfelib/nfe/schemas/v4_0/nfe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe/schemas/v4_0/retConsCad_v2.00.xsd` & `nfelib-2.0.5/nfelib/nfe/schemas/v4_0/retConsCad_v2.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe/schemas/v4_0/consReciNFe_v4.00.xsd` & `nfelib-2.0.5/nfelib/nfe/schemas/v4_0/consReciNFe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe/schemas/v4_0/leiauteInutNFe_v4.00.xsd` & `nfelib-2.0.5/nfelib/nfe/schemas/v4_0/leiauteInutNFe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe/schemas/v4_0/enviNFe_v4.00.xsd` & `nfelib-2.0.5/nfelib/nfe/schemas/v4_0/enviNFe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe/schemas/v4_0/inutNFe_v4.00.xsd` & `nfelib-2.0.5/nfelib/nfe/schemas/v4_0/inutNFe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe/schemas/v4_0/leiauteConsultaCadastro_v2.00.xsd` & `nfelib-2.0.5/nfelib/nfe/schemas/v4_0/leiauteConsultaCadastro_v2.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe/schemas/v4_0/retEnviNFe_v4.00.xsd` & `nfelib-2.0.5/nfelib/nfe/schemas/v4_0/retEnviNFe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe/schemas/v4_0/consSitNFe_v4.00.xsd` & `nfelib-2.0.5/nfelib/nfe/schemas/v4_0/consSitNFe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe/schemas/v4_0/tiposBasico_v4.00.xsd` & `nfelib-2.0.5/nfelib/nfe/schemas/v4_0/tiposBasico_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe/schemas/v4_0/leiauteNFe_v4.00.xsd` & `nfelib-2.0.5/nfelib/nfe/schemas/v4_0/leiauteNFe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe/schemas/v4_0/retConsStatServ_v4.00.xsd` & `nfelib-2.0.5/nfelib/nfe/schemas/v4_0/retConsStatServ_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe/schemas/v4_0/tiposBasico_v1.03.xsd` & `nfelib-2.0.5/nfelib/nfe/schemas/v4_0/tiposBasico_v1.03.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe/schemas/v4_0/retConsSitNFe_v4.00.xsd` & `nfelib-2.0.5/nfelib/nfe/schemas/v4_0/retConsSitNFe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-2.0.4/nfelib/nfe/schemas/v4_0/xmldsig-core-schema_v1.01.xsd` & `nfelib-2.0.5/nfelib/nfe/schemas/v4_0/xmldsig-core-schema_v1.01.xsd`

 * *Files identical despite different names*

