# Comparing `tmp/mediacloud_metadata-1.0.1.tar.gz` & `tmp/mediacloud_metadata-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mediacloud_metadata-1.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mediacloud_metadata-1.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mediacloud_metadata-1.0.1.tar` & `mediacloud_metadata-1.0.2.tar`

### file list

```diff
@@ -1,126 +1,126 @@
--rw-r--r--   0        0        0     2424 2024-05-07 20:49:34.378951 mediacloud_metadata-1.0.1/README.md
--rw-r--r--   0        0        0     7523 2024-05-07 20:49:34.378951 mediacloud_metadata-1.0.1/mcmetadata/__init__.py
--rw-r--r--   0        0        0    10598 2024-05-07 20:49:34.378951 mediacloud_metadata-1.0.1/mcmetadata/content.py
--rw-r--r--   0        0        0      234 2024-05-07 20:49:34.378951 mediacloud_metadata-1.0.1/mcmetadata/data/domain-skip-list.txt
--rw-r--r--   0        0        0     1108 2024-05-07 20:49:34.378951 mediacloud_metadata-1.0.1/mcmetadata/dates.py
--rw-r--r--   0        0        0      545 2024-05-07 20:49:34.378951 mediacloud_metadata-1.0.1/mcmetadata/exceptions.py
--rw-r--r--   0        0        0     1242 2024-05-07 20:49:34.378951 mediacloud_metadata-1.0.1/mcmetadata/feeds.py
--rw-r--r--   0        0        0     2751 2024-05-07 20:49:34.378951 mediacloud_metadata-1.0.1/mcmetadata/languages.py
--rw-r--r--   0        0        0        0 2024-05-07 20:49:34.378951 mediacloud_metadata-1.0.1/mcmetadata/py.typed
--rw-r--r--   0        0        0      492 2024-05-07 20:49:34.378951 mediacloud_metadata-1.0.1/mcmetadata/test/__init__.py
--rw-r--r--   0        0        0   855834 2024-05-07 20:49:34.382951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/bloomberg-no-meta.html
--rw-r--r--   0        0        0   855953 2024-05-07 20:49:34.386951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/bloomberg-original.html
--rw-r--r--   0        0        0     2588 2024-05-07 20:49:34.386951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httparchiveorg
--rw-r--r--   0        0        0     2677 2024-05-07 20:49:34.386951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpgpogovfdsyspkgpl
--rw-r--r--   0        0        0    18580 2024-05-07 20:49:34.386951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpmysitecom
--rw-r--r--   0        0        0    15517 2024-05-07 20:49:34.386951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpnewsmachetecompage2
--rw-r--r--   0        0        0   263006 2024-05-07 20:49:34.386951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpnytims4K9g6u
--rw-r--r--   0        0        0    95092 2024-05-07 20:49:34.390951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httppeoplesdailyngcomfeed
--rw-r--r--   0        0        0   157995 2024-05-07 20:49:34.390951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpsapifollowittrackrssstoryclickv3ecuhSAhRa8kTTPWTA7xaXioxzwoq1nFt
--rw-r--r--   0        0        0  2566654 2024-05-07 20:49:34.398951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpscnnit3wGkGU1
--rw-r--r--   0        0        0   103233 2024-05-07 20:49:34.398951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpsdatatherapywordpresscom20190313aligningyourdataandmethodsyourmission
--rw-r--r--   0        0        0  1078321 2024-05-07 20:49:34.402951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpsg1globocompipiauinoticia20230102mulhereesfaqueadapeloexnamoradodentrodecasanosuldopiauightml
--rw-r--r--   0        0        0    10912 2024-05-07 20:49:34.402951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpsobservadorvsportsptembd75404m9812obsrv53a58b677b53143428e47d43d5887139autostartfalse
--rw-r--r--   0        0        0   269738 2024-05-07 20:49:34.406951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpsobserversfrance24comen20190826mexicoafricanmigrantstrappedprotestjourney
--rw-r--r--   0        0        0    28840 2024-05-07 20:49:34.406951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpsradioaliancacombrplantaohomemde24anosemortoporgolpesdefacaemconcordiananoitedequartafeira
--rw-r--r--   0        0        0   758589 2024-05-07 20:49:34.406951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpsthekenyatimescomcountieskisumutradersalertedaboutcartelsinstallsissuance
--rw-r--r--   0        0        0    38178 2024-05-07 20:49:34.406951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpstravelgcca
--rw-r--r--   0        0        0   587306 2024-05-07 20:49:34.410951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpsupstractcomxfdf95bf448e1f2a8
--rw-r--r--   0        0        0   588319 2024-05-07 20:49:34.414951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpsupstractcomxfdf95bf448e1f2a8refrss
--rw-r--r--   0        0        0   589211 2024-05-07 20:49:34.414951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpsupstractcomxfdf95bf448e1f2a8refrssencodeutf8hexdigest
--rw-r--r--   0        0        0  2304212 2024-05-07 20:49:34.418951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswapost4FGH5Re3
--rw-r--r--   0        0        0   150555 2024-05-07 20:49:34.422951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgweb
--rw-r--r--   0        0        0    61612 2024-05-07 20:49:34.422951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgweb20111013162600id_httpwwwazftfgovFr8GSI1MAawoG8fkwp0vWYNSTuweOi89wgJOr4j83rTcpZDuFOV5E2PG737tNitGhzYAsUmVcwVEcgwKEtYFADTmzsQMJto9bZTOzDBHUGRpirFPIt4osB08CAslzBkih5ATrsMP7DRxDwcNdmfB4jU1Y1WhatWeDoVolunteerPagesdefaultaspx
--rw-r--r--   0        0        0    51041 2024-05-07 20:49:34.422951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgweb20161214220739id_httpservicessantabarbaracagovCAPMG130450Agendahtm
--rw-r--r--   0        0        0    20121 2024-05-07 20:49:34.422951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgweb20161214233744id_httpusnatarchivestumblrcompost66921244001castyourvotefortheimmigrationacttobeembed
--rw-r--r--   0        0        0    21416 2024-05-07 20:49:34.422951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgweb20210412063445id_httpsehpniehsnihgovactiondoUpdateAlertSettingsactionaddJournaljournalCodeehpreferreractiondoSearchContribAuthorRawDavis2CJacquelynContentItemTyperesearcharticlestartPageContribRawMartin2CDenny
--rw-r--r--   0        0        0   620039 2024-05-07 20:49:34.422951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgweb20220301020549httpwwwgraiulro20220225guralumiicabanasilvicavandutadarnuautoritatilorutm_sourcerssutm_mediumrssutm_campaignguralumii25e2259825bacabanasilvicavandutadarnuautoritatilor
--rw-r--r--   0        0        0   348068 2024-05-07 20:49:34.422951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgweb20220422074927httpswwwharpersbazaarcomjpfashionfashioncolumna36414759howtobesustainablefashion210514hns
--rw-r--r--   0        0        0   970498 2024-05-07 20:49:34.426951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpaptsvetlivejournalcom
--rw-r--r--   0        0        0   582587 2024-05-07 20:49:34.430951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpentretenimentouolcombrnoticiasredacao20190825semfeigesemstarkoseradohomemaranhalongedomcuhtm
--rw-r--r--   0        0        0  1630630 2024-05-07 20:49:34.434951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpsbostonglobecom
--rw-r--r--   0        0        0     2857 2024-05-07 20:49:34.434951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpsexamplecom
--rw-r--r--   0        0        0   103937 2024-05-07 20:49:34.434951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpshindioneindiacomamphtmlnewsindiaaamaadmipartyreactiononamitshahstatementoncoronacaseindelhi567287html
--rw-r--r--   0        0        0    65244 2024-05-07 20:49:34.434951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpsnaibaatpkamp2022040849027
--rw-r--r--   0        0        0   490296 2024-05-07 20:49:34.438951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpsnbcmontanacomnewslocal2womenkilledchildrenhurtinwesternnebraskacrash
--rw-r--r--   0        0        0   277606 2024-05-07 20:49:34.438951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpsobserversfrance24comen20190826mexicoafricanmigrantstrappedprotestjourney
--rw-r--r--   0        0        0   336608 2024-05-07 20:49:34.438951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpsuranewsnews1052317323
--rw-r--r--   0        0        0   197420 2024-05-07 20:49:34.438951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwalliedmarketresearchcomcytogeneticsmarket
--rw-r--r--   0        0        0   356280 2024-05-07 20:49:34.438951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwatvhubelfold20190730gyarfasugyvedjeakiavadiratotalkottanembiztoshogyazugymindenreszletetmegismerte
--rw-r--r--   0        0        0   179215 2024-05-07 20:49:34.438951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwbakerbottscomfootersubscribe
--rw-r--r--   0        0        0   278605 2024-05-07 20:49:34.442951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwcanarias7esculturacimientosartesescenicas20220718203045nthtml
--rw-r--r--   0        0        0   133247 2024-05-07 20:49:34.442951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwcbccanewscanadakitchenerwaterlooteendriverchargedfollowingcollisionnearshakespeareoppsay15230335cmprss
--rw-r--r--   0        0        0  2361789 2024-05-07 20:49:34.450951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwcnncom20210430politicsmcconnell1619projecteducationsecretaryindexhtml
--rw-r--r--   0        0        0   146273 2024-05-07 20:49:34.450951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwcorriereitesteri22_marzo_07bombeucrainedonbasssoldatirussiazioniumanitariemondoparallelomosca176a20ea9e4111ecaa45e6507f140451shtml
--rw-r--r--   0        0        0   128901 2024-05-07 20:49:34.450951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwweeaseuropaeueeaseuworld0_en
--rw-r--r--   0        0        0   397186 2024-05-07 20:49:34.454951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwelimpulsocomtagtregua
--rw-r--r--   0        0        0   217486 2024-05-07 20:49:34.454951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwfinanznachrichtendenachrichten20160838189388bittiumoyjbittiumcorporationshalfyearfinancialreportjanuaryjune2016004htm
--rw-r--r--   0        0        0   209778 2024-05-07 20:49:34.454951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwfoxnewscompoliticsbidencancelschoolloanscorinthiancollegestudents
--rw-r--r--   0        0        0   655665 2024-05-07 20:49:34.458951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwindiatimescomexplainersnewsunitednationsclimatereportmeansforindiawetbulbtemperature563318html
--rw-r--r--   0        0        0    91887 2024-05-07 20:49:34.458951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwjpnncomnewskamrussamadppkmdaruratdihentikanangkakematianberpotensitembus5000perhari
--rw-r--r--   0        0        0    53872 2024-05-07 20:49:34.458951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwkingjamesbibleonlineorg1ChroniclesChapter1
--rw-r--r--   0        0        0   239854 2024-05-07 20:49:34.458951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwlanacioncomaragenciasiranprometeunarespuestainmediataantecualquieraccionpoliticadeoieaministerionid03062022
--rw-r--r--   0        0        0   260032 2024-05-07 20:49:34.458951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwlanacioncomarseguridadcordobaenmarzoasesinaronatresmujeresnid1884942
--rw-r--r--   0        0        0   134716 2024-05-07 20:49:34.458951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwmkcokrnewssocietyview202007693939
--rw-r--r--   0        0        0   190613 2024-05-07 20:49:34.458951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwnytimescominteractive20181210businesslocationdataprivacyappshtml
--rw-r--r--   0        0        0   142191 2024-05-07 20:49:34.462951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwpagina12comar338796coronavirusenargentinaseregistraron26053casosy561m
--rw-r--r--   0        0        0   135362 2024-05-07 20:49:34.462951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwsdpnoticiascomenelshowmusicaintegrantequedautthtml
--rw-r--r--   0        0        0   244136 2024-05-07 20:49:34.462951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwsunsentinelcomcommunityflcncalendarevents2021120120211129sv3syeeuwzeallnr4vcanvaetistoryhtml
--rw-r--r--   0        0        0   142492 2024-05-07 20:49:34.462951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwthestarcombusinesseconomyopinion20190823whatthefedcouldlearnfromcanadahtml
--rw-r--r--   0        0        0    89130 2024-05-07 20:49:34.462951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwwomblebonddickinsoncomuspeoplesearch
--rw-r--r--   0        0        0   126521 2024-05-07 20:49:34.462951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttptelegrafalbotarajonimancestersulmitmerrshemplagosenpesepersona
--rw-r--r--   0        0        0   292705 2024-05-07 20:49:34.466951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttptimesofindiaindiatimescomvideosnewspunjabexitpollcvoterpredictsmajorityforaapvideoshow57559218cms
--rw-r--r--   0        0        0    51212 2024-05-07 20:49:34.466951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpworldhuanqiucomhot2016089334639html
--rw-r--r--   0        0        0    63027 2024-05-07 20:49:34.466951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpwwwozapcomactuinvitessalutlesterriensrecoitflorentpagnyetfredericlopez544047
--rw-r--r--   0        0        0    21345 2024-05-07 20:49:34.466951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpwwwprigepporgaulaforoanswerphpidcomentario301c4idforocc0idcrso467CodigoUni100190
--rw-r--r--   0        0        0   251494 2024-05-07 20:49:34.466951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswordpresscomblog20220519yourwebsitelooksgreatsoshouldyouremails
--rw-r--r--   0        0        0   393289 2024-05-07 20:49:34.466951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswwwbanduolcombrbandnewsfmriodejaneironoticiasacusadodeassassinarnamoradaafacadastemprisaoconvertidaempreventiva16574059
--rw-r--r--   0        0        0      212 2024-05-07 20:49:34.466951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswwwbizjournalscombizjournalsnews20220602remoteraisesalarypromotionpwchiringhtml
--rw-r--r--   0        0        0  2566654 2024-05-07 20:49:34.474951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswwwcnncom20220829weatherweathernewslabordaytropicalsystemtexasrainwxnindexhtml
--rw-r--r--   0        0        0  3470423 2024-05-07 20:49:34.494952 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswwwcnncom20231212entertainmentandrebraugherobitindexhtml
--rw-r--r--   0        0        0  3242138 2024-05-07 20:49:34.502951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswwwcnncom20231212politicstakeawaysvolodymyrzelenskywashingtonindexhtml
--rw-r--r--   0        0        0     1244 2024-05-07 20:49:34.502951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswwwexamplecom
--rw-r--r--   0        0        0     2677 2024-05-07 20:49:34.502951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswwwgpogovfdsyspkgPL
--rw-r--r--   0        0        0   884480 2024-05-07 20:49:34.502951 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswwwindiatimescomnewsindia75thindependencedayindiaaugust15576959html
--rw-r--r--   0        0        0   326590 2024-05-07 20:49:34.506952 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswwwkenyatodaycommediamoiburialconfusedrutoasmatiangideclarestuesdayapublicholidaycomments
--rw-r--r--   0        0        0   204274 2024-05-07 20:49:34.506952 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswwwkpbsorgnews2019jul09migrantscameroonprotestimmigrationprocesstiju
--rw-r--r--   0        0        0    17430 2024-05-07 20:49:34.506952 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswwwletrascombrbandandriveede
--rw-r--r--   0        0        0   102810 2024-05-07 20:49:34.506952 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswwwmkcokrnewssocietyview202007693939
--rw-r--r--   0        0        0   181095 2024-05-07 20:49:34.506952 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswwwnytimescominteractive20181210businesslocationdataprivacyappshtml
--rw-r--r--   0        0        0    95092 2024-05-07 20:49:34.506952 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswwwpeoplesdailyngcomfeed
--rw-r--r--   0        0        0    56852 2024-05-07 20:49:34.506952 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswwwsydneyeduau
--rw-r--r--   0        0        0   157995 2024-05-07 20:49:34.510952 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswwwtrussvilletribunecom20220302threestudentsfromcenterpointreceiveacademicscholarships
--rw-r--r--   0        0        0    48394 2024-05-07 20:49:34.510952 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswwwuniradioinformacomnoticiascoronavirus677354covidsegundacausademuerteenmexicoen2021htmlutm_sourcefeedutm_mediumlinkutm_campaignrss
--rw-r--r--   0        0        0   228954 2024-05-07 20:49:34.510952 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswwwwdsucomarticleuntitledcontent170181311946044845
--rw-r--r--   0        0        0   884978 2024-05-07 20:49:34.514952 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswwwyoutubecomwatchvaFCO6WidGVM
--rw-r--r--   0        0        0   758615 2024-05-07 20:49:34.514952 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpthekenyatimescomcountieskisumutradersalertedaboutcartelsinstallsissuance
--rw-r--r--   0        0        0   158103 2024-05-07 20:49:34.514952 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httptrussvilletribunecom20220302threestudentsfromcenterpointreceiveacademicscholarships
--rw-r--r--   0        0        0    48833 2024-05-07 20:49:34.514952 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpuniradioinformacomnoticiascoronavirus677126nuevossintomasdelcovidprolongadohtml
--rw-r--r--   0        0        0    48833 2024-05-07 20:49:34.514952 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpuniradioinformacomnoticiascoronavirus677126nuevossintomasdelcovidprolongadohtmlutm_campaignrssutm_mediumlink
--rw-r--r--   0        0        0    48394 2024-05-07 20:49:34.514952 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpuniradioinformacomnoticiascoronavirus677354covidsegundacausademuerteenmexicoen2021html
--rw-r--r--   0        0        0   590003 2024-05-07 20:49:34.514952 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpupstractcomxfdf95bf448e1f2a8
--rw-r--r--   0        0        0    73416 2024-05-07 20:49:34.514952 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpwwforgbr
--rw-r--r--   0        0        0    60065 2024-05-07 20:49:34.518952 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpwwforjp
--rw-r--r--   0        0        0   208253 2024-05-07 20:49:34.518952 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpwwwdiariobahiadecadizcomnoticiassanfernandocavadayromeromantienenotroencuentrocondefensaparanegociarladesafectaciondesueloencamposotorequerirauntiempoindeterminado
--rw-r--r--   0        0        0    68487 2024-05-07 20:49:34.518952 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpwwwgovcn
--rw-r--r--   0        0        0    19896 2024-05-07 20:49:34.518952 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpwwwinformecorrientescomvernotaaspid_noticia44619
--rw-r--r--   0        0        0  1239580 2024-05-07 20:49:34.522952 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpwwwnytimescom
--rw-r--r--   0        0        0  1120104 2024-05-07 20:49:34.522952 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpwwwnytimescomglobal
--rw-r--r--   0        0        0   426073 2024-05-07 20:49:34.522952 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpwwwwiredcom
--rw-r--r--   0        0        0   881817 2024-05-07 20:49:34.526952 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpyoutubecomwatchvaFCO6WidGVM
--rw-r--r--   0        0        0   117791 2024-05-07 20:49:34.526952 mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/focus-taiwan-202311170015.html
--rw-r--r--   0        0        0     7799 2024-05-07 20:49:34.526952 mediacloud_metadata-1.0.1/mcmetadata/test/test_content.py
--rw-r--r--   0        0        0     3726 2024-05-07 20:49:34.526952 mediacloud_metadata-1.0.1/mcmetadata/test/test_dates.py
--rw-r--r--   0        0        0    11212 2024-05-07 20:49:34.526952 mediacloud_metadata-1.0.1/mcmetadata/test/test_extract.py
--rw-r--r--   0        0        0      791 2024-05-07 20:49:34.526952 mediacloud_metadata-1.0.1/mcmetadata/test/test_feeds.py
--rw-r--r--   0        0        0     6544 2024-05-07 20:49:34.526952 mediacloud_metadata-1.0.1/mcmetadata/test/test_languages.py
--rw-r--r--   0        0        0     8721 2024-05-07 20:49:34.526952 mediacloud_metadata-1.0.1/mcmetadata/test/test_titles.py
--rw-r--r--   0        0        0     9665 2024-05-07 20:49:34.526952 mediacloud_metadata-1.0.1/mcmetadata/test/test_urls.py
--rw-r--r--   0        0        0     1607 2024-05-07 20:49:34.526952 mediacloud_metadata-1.0.1/mcmetadata/test/test_webpages.py
--rw-r--r--   0        0        0     1183 2024-05-07 20:49:34.526952 mediacloud_metadata-1.0.1/mcmetadata/text.py
--rw-r--r--   0        0        0     5958 2024-05-07 20:49:34.530952 mediacloud_metadata-1.0.1/mcmetadata/titles.py
--rw-r--r--   0        0        0    14652 2024-05-07 20:49:34.530952 mediacloud_metadata-1.0.1/mcmetadata/urls.py
--rw-r--r--   0        0        0     7061 2024-05-07 20:49:34.530952 mediacloud_metadata-1.0.1/mcmetadata/urlshortners.py
--rw-r--r--   0        0        0     2063 2024-05-07 20:49:34.530952 mediacloud_metadata-1.0.1/mcmetadata/webpages.py
--rw-r--r--   0        0        0     1616 2024-05-07 20:49:34.530952 mediacloud_metadata-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     4013 1970-01-01 00:00:00.000000 mediacloud_metadata-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2424 2024-05-07 22:00:58.588059 mediacloud_metadata-1.0.2/README.md
+-rw-r--r--   0        0        0     7523 2024-05-07 22:00:58.588059 mediacloud_metadata-1.0.2/mcmetadata/__init__.py
+-rw-r--r--   0        0        0    10598 2024-05-07 22:00:58.588059 mediacloud_metadata-1.0.2/mcmetadata/content.py
+-rw-r--r--   0        0        0      234 2024-05-07 22:00:58.588059 mediacloud_metadata-1.0.2/mcmetadata/data/domain-skip-list.txt
+-rw-r--r--   0        0        0     1108 2024-05-07 22:00:58.588059 mediacloud_metadata-1.0.2/mcmetadata/dates.py
+-rw-r--r--   0        0        0      545 2024-05-07 22:00:58.588059 mediacloud_metadata-1.0.2/mcmetadata/exceptions.py
+-rw-r--r--   0        0        0     1242 2024-05-07 22:00:58.588059 mediacloud_metadata-1.0.2/mcmetadata/feeds.py
+-rw-r--r--   0        0        0     2751 2024-05-07 22:00:58.588059 mediacloud_metadata-1.0.2/mcmetadata/languages.py
+-rw-r--r--   0        0        0        0 2024-05-07 22:00:58.588059 mediacloud_metadata-1.0.2/mcmetadata/py.typed
+-rw-r--r--   0        0        0      492 2024-05-07 22:00:58.588059 mediacloud_metadata-1.0.2/mcmetadata/test/__init__.py
+-rw-r--r--   0        0        0   855834 2024-05-07 22:00:58.592059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/bloomberg-no-meta.html
+-rw-r--r--   0        0        0   855953 2024-05-07 22:00:58.592059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/bloomberg-original.html
+-rw-r--r--   0        0        0     2588 2024-05-07 22:00:58.592059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httparchiveorg
+-rw-r--r--   0        0        0     2677 2024-05-07 22:00:58.592059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpgpogovfdsyspkgpl
+-rw-r--r--   0        0        0    18580 2024-05-07 22:00:58.592059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpmysitecom
+-rw-r--r--   0        0        0    15517 2024-05-07 22:00:58.592059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpnewsmachetecompage2
+-rw-r--r--   0        0        0   263006 2024-05-07 22:00:58.596059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpnytims4K9g6u
+-rw-r--r--   0        0        0    95092 2024-05-07 22:00:58.596059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httppeoplesdailyngcomfeed
+-rw-r--r--   0        0        0   157995 2024-05-07 22:00:58.596059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpsapifollowittrackrssstoryclickv3ecuhSAhRa8kTTPWTA7xaXioxzwoq1nFt
+-rw-r--r--   0        0        0  2566654 2024-05-07 22:00:58.608059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpscnnit3wGkGU1
+-rw-r--r--   0        0        0   103233 2024-05-07 22:00:58.608059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpsdatatherapywordpresscom20190313aligningyourdataandmethodsyourmission
+-rw-r--r--   0        0        0  1078321 2024-05-07 22:00:58.612059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpsg1globocompipiauinoticia20230102mulhereesfaqueadapeloexnamoradodentrodecasanosuldopiauightml
+-rw-r--r--   0        0        0    10912 2024-05-07 22:00:58.612059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpsobservadorvsportsptembd75404m9812obsrv53a58b677b53143428e47d43d5887139autostartfalse
+-rw-r--r--   0        0        0   269738 2024-05-07 22:00:58.612059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpsobserversfrance24comen20190826mexicoafricanmigrantstrappedprotestjourney
+-rw-r--r--   0        0        0    28840 2024-05-07 22:00:58.612059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpsradioaliancacombrplantaohomemde24anosemortoporgolpesdefacaemconcordiananoitedequartafeira
+-rw-r--r--   0        0        0   758589 2024-05-07 22:00:58.616059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpsthekenyatimescomcountieskisumutradersalertedaboutcartelsinstallsissuance
+-rw-r--r--   0        0        0    38178 2024-05-07 22:00:58.616059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpstravelgcca
+-rw-r--r--   0        0        0   587306 2024-05-07 22:00:58.616059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpsupstractcomxfdf95bf448e1f2a8
+-rw-r--r--   0        0        0   588319 2024-05-07 22:00:58.620059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpsupstractcomxfdf95bf448e1f2a8refrss
+-rw-r--r--   0        0        0   589211 2024-05-07 22:00:58.620059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpsupstractcomxfdf95bf448e1f2a8refrssencodeutf8hexdigest
+-rw-r--r--   0        0        0  2304212 2024-05-07 22:00:58.628059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswapost4FGH5Re3
+-rw-r--r--   0        0        0   150555 2024-05-07 22:00:58.628059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgweb
+-rw-r--r--   0        0        0    61612 2024-05-07 22:00:58.628059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgweb20111013162600id_httpwwwazftfgovFr8GSI1MAawoG8fkwp0vWYNSTuweOi89wgJOr4j83rTcpZDuFOV5E2PG737tNitGhzYAsUmVcwVEcgwKEtYFADTmzsQMJto9bZTOzDBHUGRpirFPIt4osB08CAslzBkih5ATrsMP7DRxDwcNdmfB4jU1Y1WhatWeDoVolunteerPagesdefaultaspx
+-rw-r--r--   0        0        0    51041 2024-05-07 22:00:58.628059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgweb20161214220739id_httpservicessantabarbaracagovCAPMG130450Agendahtm
+-rw-r--r--   0        0        0    20121 2024-05-07 22:00:58.628059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgweb20161214233744id_httpusnatarchivestumblrcompost66921244001castyourvotefortheimmigrationacttobeembed
+-rw-r--r--   0        0        0    21416 2024-05-07 22:00:58.628059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgweb20210412063445id_httpsehpniehsnihgovactiondoUpdateAlertSettingsactionaddJournaljournalCodeehpreferreractiondoSearchContribAuthorRawDavis2CJacquelynContentItemTyperesearcharticlestartPageContribRawMartin2CDenny
+-rw-r--r--   0        0        0   620039 2024-05-07 22:00:58.628059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgweb20220301020549httpwwwgraiulro20220225guralumiicabanasilvicavandutadarnuautoritatilorutm_sourcerssutm_mediumrssutm_campaignguralumii25e2259825bacabanasilvicavandutadarnuautoritatilor
+-rw-r--r--   0        0        0   348068 2024-05-07 22:00:58.632059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgweb20220422074927httpswwwharpersbazaarcomjpfashionfashioncolumna36414759howtobesustainablefashion210514hns
+-rw-r--r--   0        0        0   970498 2024-05-07 22:00:58.636059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpaptsvetlivejournalcom
+-rw-r--r--   0        0        0   582587 2024-05-07 22:00:58.636059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpentretenimentouolcombrnoticiasredacao20190825semfeigesemstarkoseradohomemaranhalongedomcuhtm
+-rw-r--r--   0        0        0  1630630 2024-05-07 22:00:58.640059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpsbostonglobecom
+-rw-r--r--   0        0        0     2857 2024-05-07 22:00:58.640059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpsexamplecom
+-rw-r--r--   0        0        0   103937 2024-05-07 22:00:58.640059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpshindioneindiacomamphtmlnewsindiaaamaadmipartyreactiononamitshahstatementoncoronacaseindelhi567287html
+-rw-r--r--   0        0        0    65244 2024-05-07 22:00:58.640059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpsnaibaatpkamp2022040849027
+-rw-r--r--   0        0        0   490296 2024-05-07 22:00:58.644059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpsnbcmontanacomnewslocal2womenkilledchildrenhurtinwesternnebraskacrash
+-rw-r--r--   0        0        0   277606 2024-05-07 22:00:58.644059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpsobserversfrance24comen20190826mexicoafricanmigrantstrappedprotestjourney
+-rw-r--r--   0        0        0   336608 2024-05-07 22:00:58.644059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpsuranewsnews1052317323
+-rw-r--r--   0        0        0   197420 2024-05-07 22:00:58.644059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwalliedmarketresearchcomcytogeneticsmarket
+-rw-r--r--   0        0        0   356280 2024-05-07 22:00:58.648059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwatvhubelfold20190730gyarfasugyvedjeakiavadiratotalkottanembiztoshogyazugymindenreszletetmegismerte
+-rw-r--r--   0        0        0   179215 2024-05-07 22:00:58.648059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwbakerbottscomfootersubscribe
+-rw-r--r--   0        0        0   278605 2024-05-07 22:00:58.648059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwcanarias7esculturacimientosartesescenicas20220718203045nthtml
+-rw-r--r--   0        0        0   133247 2024-05-07 22:00:58.648059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwcbccanewscanadakitchenerwaterlooteendriverchargedfollowingcollisionnearshakespeareoppsay15230335cmprss
+-rw-r--r--   0        0        0  2361789 2024-05-07 22:00:58.656059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwcnncom20210430politicsmcconnell1619projecteducationsecretaryindexhtml
+-rw-r--r--   0        0        0   146273 2024-05-07 22:00:58.660060 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwcorriereitesteri22_marzo_07bombeucrainedonbasssoldatirussiazioniumanitariemondoparallelomosca176a20ea9e4111ecaa45e6507f140451shtml
+-rw-r--r--   0        0        0   128901 2024-05-07 22:00:58.660060 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwweeaseuropaeueeaseuworld0_en
+-rw-r--r--   0        0        0   397186 2024-05-07 22:00:58.660060 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwelimpulsocomtagtregua
+-rw-r--r--   0        0        0   217486 2024-05-07 22:00:58.660060 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwfinanznachrichtendenachrichten20160838189388bittiumoyjbittiumcorporationshalfyearfinancialreportjanuaryjune2016004htm
+-rw-r--r--   0        0        0   209778 2024-05-07 22:00:58.660060 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwfoxnewscompoliticsbidencancelschoolloanscorinthiancollegestudents
+-rw-r--r--   0        0        0   655665 2024-05-07 22:00:58.664059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwindiatimescomexplainersnewsunitednationsclimatereportmeansforindiawetbulbtemperature563318html
+-rw-r--r--   0        0        0    91887 2024-05-07 22:00:58.664059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwjpnncomnewskamrussamadppkmdaruratdihentikanangkakematianberpotensitembus5000perhari
+-rw-r--r--   0        0        0    53872 2024-05-07 22:00:58.664059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwkingjamesbibleonlineorg1ChroniclesChapter1
+-rw-r--r--   0        0        0   239854 2024-05-07 22:00:58.664059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwlanacioncomaragenciasiranprometeunarespuestainmediataantecualquieraccionpoliticadeoieaministerionid03062022
+-rw-r--r--   0        0        0   260032 2024-05-07 22:00:58.664059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwlanacioncomarseguridadcordobaenmarzoasesinaronatresmujeresnid1884942
+-rw-r--r--   0        0        0   134716 2024-05-07 22:00:58.668059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwmkcokrnewssocietyview202007693939
+-rw-r--r--   0        0        0   190613 2024-05-07 22:00:58.668059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwnytimescominteractive20181210businesslocationdataprivacyappshtml
+-rw-r--r--   0        0        0   142191 2024-05-07 22:00:58.668059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwpagina12comar338796coronavirusenargentinaseregistraron26053casosy561m
+-rw-r--r--   0        0        0   135362 2024-05-07 22:00:58.668059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwsdpnoticiascomenelshowmusicaintegrantequedautthtml
+-rw-r--r--   0        0        0   244136 2024-05-07 22:00:58.668059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwsunsentinelcomcommunityflcncalendarevents2021120120211129sv3syeeuwzeallnr4vcanvaetistoryhtml
+-rw-r--r--   0        0        0   142492 2024-05-07 22:00:58.668059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwthestarcombusinesseconomyopinion20190823whatthefedcouldlearnfromcanadahtml
+-rw-r--r--   0        0        0    89130 2024-05-07 22:00:58.668059 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwwomblebonddickinsoncomuspeoplesearch
+-rw-r--r--   0        0        0   126521 2024-05-07 22:00:58.672060 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttptelegrafalbotarajonimancestersulmitmerrshemplagosenpesepersona
+-rw-r--r--   0        0        0   292705 2024-05-07 22:00:58.672060 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttptimesofindiaindiatimescomvideosnewspunjabexitpollcvoterpredictsmajorityforaapvideoshow57559218cms
+-rw-r--r--   0        0        0    51212 2024-05-07 22:00:58.672060 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpworldhuanqiucomhot2016089334639html
+-rw-r--r--   0        0        0    63027 2024-05-07 22:00:58.672060 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpwwwozapcomactuinvitessalutlesterriensrecoitflorentpagnyetfredericlopez544047
+-rw-r--r--   0        0        0    21345 2024-05-07 22:00:58.672060 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpwwwprigepporgaulaforoanswerphpidcomentario301c4idforocc0idcrso467CodigoUni100190
+-rw-r--r--   0        0        0   251494 2024-05-07 22:00:58.672060 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswordpresscomblog20220519yourwebsitelooksgreatsoshouldyouremails
+-rw-r--r--   0        0        0   393289 2024-05-07 22:00:58.672060 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswwwbanduolcombrbandnewsfmriodejaneironoticiasacusadodeassassinarnamoradaafacadastemprisaoconvertidaempreventiva16574059
+-rw-r--r--   0        0        0      212 2024-05-07 22:00:58.672060 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswwwbizjournalscombizjournalsnews20220602remoteraisesalarypromotionpwchiringhtml
+-rw-r--r--   0        0        0  2566654 2024-05-07 22:00:58.684060 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswwwcnncom20220829weatherweathernewslabordaytropicalsystemtexasrainwxnindexhtml
+-rw-r--r--   0        0        0  3470423 2024-05-07 22:00:58.700060 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswwwcnncom20231212entertainmentandrebraugherobitindexhtml
+-rw-r--r--   0        0        0  3242138 2024-05-07 22:00:58.712060 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswwwcnncom20231212politicstakeawaysvolodymyrzelenskywashingtonindexhtml
+-rw-r--r--   0        0        0     1244 2024-05-07 22:00:58.712060 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswwwexamplecom
+-rw-r--r--   0        0        0     2677 2024-05-07 22:00:58.712060 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswwwgpogovfdsyspkgPL
+-rw-r--r--   0        0        0   884480 2024-05-07 22:00:58.712060 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswwwindiatimescomnewsindia75thindependencedayindiaaugust15576959html
+-rw-r--r--   0        0        0   326590 2024-05-07 22:00:58.712060 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswwwkenyatodaycommediamoiburialconfusedrutoasmatiangideclarestuesdayapublicholidaycomments
+-rw-r--r--   0        0        0   204274 2024-05-07 22:00:58.712060 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswwwkpbsorgnews2019jul09migrantscameroonprotestimmigrationprocesstiju
+-rw-r--r--   0        0        0    17430 2024-05-07 22:00:58.716060 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswwwletrascombrbandandriveede
+-rw-r--r--   0        0        0   102810 2024-05-07 22:00:58.716060 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswwwmkcokrnewssocietyview202007693939
+-rw-r--r--   0        0        0   181095 2024-05-07 22:00:58.716060 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswwwnytimescominteractive20181210businesslocationdataprivacyappshtml
+-rw-r--r--   0        0        0    95092 2024-05-07 22:00:58.716060 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswwwpeoplesdailyngcomfeed
+-rw-r--r--   0        0        0    56852 2024-05-07 22:00:58.716060 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswwwsydneyeduau
+-rw-r--r--   0        0        0   157995 2024-05-07 22:00:58.716060 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswwwtrussvilletribunecom20220302threestudentsfromcenterpointreceiveacademicscholarships
+-rw-r--r--   0        0        0    48394 2024-05-07 22:00:58.716060 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswwwuniradioinformacomnoticiascoronavirus677354covidsegundacausademuerteenmexicoen2021htmlutm_sourcefeedutm_mediumlinkutm_campaignrss
+-rw-r--r--   0        0        0   228954 2024-05-07 22:00:58.720060 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswwwwdsucomarticleuntitledcontent170181311946044845
+-rw-r--r--   0        0        0   884978 2024-05-07 22:00:58.720060 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswwwyoutubecomwatchvaFCO6WidGVM
+-rw-r--r--   0        0        0   758615 2024-05-07 22:00:58.724060 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpthekenyatimescomcountieskisumutradersalertedaboutcartelsinstallsissuance
+-rw-r--r--   0        0        0   158103 2024-05-07 22:00:58.724060 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httptrussvilletribunecom20220302threestudentsfromcenterpointreceiveacademicscholarships
+-rw-r--r--   0        0        0    48833 2024-05-07 22:00:58.724060 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpuniradioinformacomnoticiascoronavirus677126nuevossintomasdelcovidprolongadohtml
+-rw-r--r--   0        0        0    48833 2024-05-07 22:00:58.724060 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpuniradioinformacomnoticiascoronavirus677126nuevossintomasdelcovidprolongadohtmlutm_campaignrssutm_mediumlink
+-rw-r--r--   0        0        0    48394 2024-05-07 22:00:58.724060 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpuniradioinformacomnoticiascoronavirus677354covidsegundacausademuerteenmexicoen2021html
+-rw-r--r--   0        0        0   590003 2024-05-07 22:00:58.724060 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpupstractcomxfdf95bf448e1f2a8
+-rw-r--r--   0        0        0    73416 2024-05-07 22:00:58.724060 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpwwforgbr
+-rw-r--r--   0        0        0    60065 2024-05-07 22:00:58.724060 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpwwforjp
+-rw-r--r--   0        0        0   208253 2024-05-07 22:00:58.724060 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpwwwdiariobahiadecadizcomnoticiassanfernandocavadayromeromantienenotroencuentrocondefensaparanegociarladesafectaciondesueloencamposotorequerirauntiempoindeterminado
+-rw-r--r--   0        0        0    68487 2024-05-07 22:00:58.724060 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpwwwgovcn
+-rw-r--r--   0        0        0    19896 2024-05-07 22:00:58.724060 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpwwwinformecorrientescomvernotaaspid_noticia44619
+-rw-r--r--   0        0        0  1239580 2024-05-07 22:00:58.728060 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpwwwnytimescom
+-rw-r--r--   0        0        0  1120104 2024-05-07 22:00:58.732060 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpwwwnytimescomglobal
+-rw-r--r--   0        0        0   426073 2024-05-07 22:00:58.732060 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpwwwwiredcom
+-rw-r--r--   0        0        0   881817 2024-05-07 22:00:58.736060 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpyoutubecomwatchvaFCO6WidGVM
+-rw-r--r--   0        0        0   117791 2024-05-07 22:00:58.736060 mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/focus-taiwan-202311170015.html
+-rw-r--r--   0        0        0     7799 2024-05-07 22:00:58.736060 mediacloud_metadata-1.0.2/mcmetadata/test/test_content.py
+-rw-r--r--   0        0        0     3726 2024-05-07 22:00:58.736060 mediacloud_metadata-1.0.2/mcmetadata/test/test_dates.py
+-rw-r--r--   0        0        0    11212 2024-05-07 22:00:58.736060 mediacloud_metadata-1.0.2/mcmetadata/test/test_extract.py
+-rw-r--r--   0        0        0      791 2024-05-07 22:00:58.736060 mediacloud_metadata-1.0.2/mcmetadata/test/test_feeds.py
+-rw-r--r--   0        0        0     6544 2024-05-07 22:00:58.736060 mediacloud_metadata-1.0.2/mcmetadata/test/test_languages.py
+-rw-r--r--   0        0        0     8721 2024-05-07 22:00:58.736060 mediacloud_metadata-1.0.2/mcmetadata/test/test_titles.py
+-rw-r--r--   0        0        0     9665 2024-05-07 22:00:58.736060 mediacloud_metadata-1.0.2/mcmetadata/test/test_urls.py
+-rw-r--r--   0        0        0     1607 2024-05-07 22:00:58.736060 mediacloud_metadata-1.0.2/mcmetadata/test/test_webpages.py
+-rw-r--r--   0        0        0     1183 2024-05-07 22:00:58.736060 mediacloud_metadata-1.0.2/mcmetadata/text.py
+-rw-r--r--   0        0        0     5958 2024-05-07 22:00:58.736060 mediacloud_metadata-1.0.2/mcmetadata/titles.py
+-rw-r--r--   0        0        0    14652 2024-05-07 22:00:58.736060 mediacloud_metadata-1.0.2/mcmetadata/urls.py
+-rw-r--r--   0        0        0     7061 2024-05-07 22:00:58.736060 mediacloud_metadata-1.0.2/mcmetadata/urlshortners.py
+-rw-r--r--   0        0        0     2063 2024-05-07 22:00:58.736060 mediacloud_metadata-1.0.2/mcmetadata/webpages.py
+-rw-r--r--   0        0        0     1616 2024-05-07 22:00:58.736060 mediacloud_metadata-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4013 1970-01-01 00:00:00.000000 mediacloud_metadata-1.0.2/PKG-INFO
```

### Comparing `mediacloud_metadata-1.0.1/README.md` & `mediacloud_metadata-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/__init__.py` & `mediacloud_metadata-1.0.2/mcmetadata/__init__.py`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/content.py` & `mediacloud_metadata-1.0.2/mcmetadata/content.py`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/dates.py` & `mediacloud_metadata-1.0.2/mcmetadata/dates.py`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/exceptions.py` & `mediacloud_metadata-1.0.2/mcmetadata/exceptions.py`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/feeds.py` & `mediacloud_metadata-1.0.2/mcmetadata/feeds.py`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/languages.py` & `mediacloud_metadata-1.0.2/mcmetadata/languages.py`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/bloomberg-no-meta.html` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/bloomberg-no-meta.html`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/bloomberg-original.html` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/bloomberg-original.html`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httparchiveorg` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httparchiveorg`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpgpogovfdsyspkgpl` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpgpogovfdsyspkgpl`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpmysitecom` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpmysitecom`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpnewsmachetecompage2` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpnewsmachetecompage2`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpnytims4K9g6u` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpnytims4K9g6u`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httppeoplesdailyngcomfeed` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httppeoplesdailyngcomfeed`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpsapifollowittrackrssstoryclickv3ecuhSAhRa8kTTPWTA7xaXioxzwoq1nFt` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpsapifollowittrackrssstoryclickv3ecuhSAhRa8kTTPWTA7xaXioxzwoq1nFt`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpscnnit3wGkGU1` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpscnnit3wGkGU1`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpsdatatherapywordpresscom20190313aligningyourdataandmethodsyourmission` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpsdatatherapywordpresscom20190313aligningyourdataandmethodsyourmission`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpsg1globocompipiauinoticia20230102mulhereesfaqueadapeloexnamoradodentrodecasanosuldopiauightml` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpsg1globocompipiauinoticia20230102mulhereesfaqueadapeloexnamoradodentrodecasanosuldopiauightml`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpsobservadorvsportsptembd75404m9812obsrv53a58b677b53143428e47d43d5887139autostartfalse` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpsobservadorvsportsptembd75404m9812obsrv53a58b677b53143428e47d43d5887139autostartfalse`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpsobserversfrance24comen20190826mexicoafricanmigrantstrappedprotestjourney` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpsobserversfrance24comen20190826mexicoafricanmigrantstrappedprotestjourney`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpsradioaliancacombrplantaohomemde24anosemortoporgolpesdefacaemconcordiananoitedequartafeira` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpsradioaliancacombrplantaohomemde24anosemortoporgolpesdefacaemconcordiananoitedequartafeira`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpsthekenyatimescomcountieskisumutradersalertedaboutcartelsinstallsissuance` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpsthekenyatimescomcountieskisumutradersalertedaboutcartelsinstallsissuance`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpstravelgcca` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpstravelgcca`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpsupstractcomxfdf95bf448e1f2a8` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpsupstractcomxfdf95bf448e1f2a8`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpsupstractcomxfdf95bf448e1f2a8refrss` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpsupstractcomxfdf95bf448e1f2a8refrss`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpsupstractcomxfdf95bf448e1f2a8refrssencodeutf8hexdigest` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpsupstractcomxfdf95bf448e1f2a8refrssencodeutf8hexdigest`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswapost4FGH5Re3` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswapost4FGH5Re3`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgweb` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgweb`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgweb20111013162600id_httpwwwazftfgovFr8GSI1MAawoG8fkwp0vWYNSTuweOi89wgJOr4j83rTcpZDuFOV5E2PG737tNitGhzYAsUmVcwVEcgwKEtYFADTmzsQMJto9bZTOzDBHUGRpirFPIt4osB08CAslzBkih5ATrsMP7DRxDwcNdmfB4jU1Y1WhatWeDoVolunteerPagesdefaultaspx` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgweb20111013162600id_httpwwwazftfgovFr8GSI1MAawoG8fkwp0vWYNSTuweOi89wgJOr4j83rTcpZDuFOV5E2PG737tNitGhzYAsUmVcwVEcgwKEtYFADTmzsQMJto9bZTOzDBHUGRpirFPIt4osB08CAslzBkih5ATrsMP7DRxDwcNdmfB4jU1Y1WhatWeDoVolunteerPagesdefaultaspx`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgweb20161214220739id_httpservicessantabarbaracagovCAPMG130450Agendahtm` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgweb20161214220739id_httpservicessantabarbaracagovCAPMG130450Agendahtm`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgweb20161214233744id_httpusnatarchivestumblrcompost66921244001castyourvotefortheimmigrationacttobeembed` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgweb20161214233744id_httpusnatarchivestumblrcompost66921244001castyourvotefortheimmigrationacttobeembed`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgweb20210412063445id_httpsehpniehsnihgovactiondoUpdateAlertSettingsactionaddJournaljournalCodeehpreferreractiondoSearchContribAuthorRawDavis2CJacquelynContentItemTyperesearcharticlestartPageContribRawMartin2CDenny` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgweb20210412063445id_httpsehpniehsnihgovactiondoUpdateAlertSettingsactionaddJournaljournalCodeehpreferreractiondoSearchContribAuthorRawDavis2CJacquelynContentItemTyperesearcharticlestartPageContribRawMartin2CDenny`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgweb20220301020549httpwwwgraiulro20220225guralumiicabanasilvicavandutadarnuautoritatilorutm_sourcerssutm_mediumrssutm_campaignguralumii25e2259825bacabanasilvicavandutadarnuautoritatilor` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgweb20220301020549httpwwwgraiulro20220225guralumiicabanasilvicavandutadarnuautoritatilorutm_sourcerssutm_mediumrssutm_campaignguralumii25e2259825bacabanasilvicavandutadarnuautoritatilor`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgweb20220422074927httpswwwharpersbazaarcomjpfashionfashioncolumna36414759howtobesustainablefashion210514hns` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgweb20220422074927httpswwwharpersbazaarcomjpfashionfashioncolumna36414759howtobesustainablefashion210514hns`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpaptsvetlivejournalcom` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpaptsvetlivejournalcom`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpentretenimentouolcombrnoticiasredacao20190825semfeigesemstarkoseradohomemaranhalongedomcuhtm` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpentretenimentouolcombrnoticiasredacao20190825semfeigesemstarkoseradohomemaranhalongedomcuhtm`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpsbostonglobecom` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpsbostonglobecom`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpsexamplecom` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpsexamplecom`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpshindioneindiacomamphtmlnewsindiaaamaadmipartyreactiononamitshahstatementoncoronacaseindelhi567287html` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpshindioneindiacomamphtmlnewsindiaaamaadmipartyreactiononamitshahstatementoncoronacaseindelhi567287html`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpsnaibaatpkamp2022040849027` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpsnaibaatpkamp2022040849027`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpsnbcmontanacomnewslocal2womenkilledchildrenhurtinwesternnebraskacrash` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpsnbcmontanacomnewslocal2womenkilledchildrenhurtinwesternnebraskacrash`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpsobserversfrance24comen20190826mexicoafricanmigrantstrappedprotestjourney` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpsobserversfrance24comen20190826mexicoafricanmigrantstrappedprotestjourney`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpsuranewsnews1052317323` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpsuranewsnews1052317323`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwalliedmarketresearchcomcytogeneticsmarket` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwalliedmarketresearchcomcytogeneticsmarket`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwatvhubelfold20190730gyarfasugyvedjeakiavadiratotalkottanembiztoshogyazugymindenreszletetmegismerte` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwatvhubelfold20190730gyarfasugyvedjeakiavadiratotalkottanembiztoshogyazugymindenreszletetmegismerte`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwbakerbottscomfootersubscribe` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwbakerbottscomfootersubscribe`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwcanarias7esculturacimientosartesescenicas20220718203045nthtml` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwcanarias7esculturacimientosartesescenicas20220718203045nthtml`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwcbccanewscanadakitchenerwaterlooteendriverchargedfollowingcollisionnearshakespeareoppsay15230335cmprss` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwcbccanewscanadakitchenerwaterlooteendriverchargedfollowingcollisionnearshakespeareoppsay15230335cmprss`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwcnncom20210430politicsmcconnell1619projecteducationsecretaryindexhtml` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwcnncom20210430politicsmcconnell1619projecteducationsecretaryindexhtml`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwcorriereitesteri22_marzo_07bombeucrainedonbasssoldatirussiazioniumanitariemondoparallelomosca176a20ea9e4111ecaa45e6507f140451shtml` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwcorriereitesteri22_marzo_07bombeucrainedonbasssoldatirussiazioniumanitariemondoparallelomosca176a20ea9e4111ecaa45e6507f140451shtml`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwweeaseuropaeueeaseuworld0_en` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwweeaseuropaeueeaseuworld0_en`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwelimpulsocomtagtregua` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwelimpulsocomtagtregua`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwfinanznachrichtendenachrichten20160838189388bittiumoyjbittiumcorporationshalfyearfinancialreportjanuaryjune2016004htm` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwfinanznachrichtendenachrichten20160838189388bittiumoyjbittiumcorporationshalfyearfinancialreportjanuaryjune2016004htm`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwfoxnewscompoliticsbidencancelschoolloanscorinthiancollegestudents` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwfoxnewscompoliticsbidencancelschoolloanscorinthiancollegestudents`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwindiatimescomexplainersnewsunitednationsclimatereportmeansforindiawetbulbtemperature563318html` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwindiatimescomexplainersnewsunitednationsclimatereportmeansforindiawetbulbtemperature563318html`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwjpnncomnewskamrussamadppkmdaruratdihentikanangkakematianberpotensitembus5000perhari` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwjpnncomnewskamrussamadppkmdaruratdihentikanangkakematianberpotensitembus5000perhari`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwkingjamesbibleonlineorg1ChroniclesChapter1` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwkingjamesbibleonlineorg1ChroniclesChapter1`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwlanacioncomaragenciasiranprometeunarespuestainmediataantecualquieraccionpoliticadeoieaministerionid03062022` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwlanacioncomaragenciasiranprometeunarespuestainmediataantecualquieraccionpoliticadeoieaministerionid03062022`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwlanacioncomarseguridadcordobaenmarzoasesinaronatresmujeresnid1884942` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwlanacioncomarseguridadcordobaenmarzoasesinaronatresmujeresnid1884942`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwmkcokrnewssocietyview202007693939` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwmkcokrnewssocietyview202007693939`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwnytimescominteractive20181210businesslocationdataprivacyappshtml` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwnytimescominteractive20181210businesslocationdataprivacyappshtml`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwpagina12comar338796coronavirusenargentinaseregistraron26053casosy561m` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwpagina12comar338796coronavirusenargentinaseregistraron26053casosy561m`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwsdpnoticiascomenelshowmusicaintegrantequedautthtml` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwsdpnoticiascomenelshowmusicaintegrantequedautthtml`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwsunsentinelcomcommunityflcncalendarevents2021120120211129sv3syeeuwzeallnr4vcanvaetistoryhtml` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwsunsentinelcomcommunityflcncalendarevents2021120120211129sv3syeeuwzeallnr4vcanvaetistoryhtml`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwthestarcombusinesseconomyopinion20190823whatthefedcouldlearnfromcanadahtml` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwthestarcombusinesseconomyopinion20190823whatthefedcouldlearnfromcanadahtml`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwwomblebonddickinsoncomuspeoplesearch` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpswwwwomblebonddickinsoncomuspeoplesearch`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttptelegrafalbotarajonimancestersulmitmerrshemplagosenpesepersona` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttptelegrafalbotarajonimancestersulmitmerrshemplagosenpesepersona`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttptimesofindiaindiatimescomvideosnewspunjabexitpollcvoterpredictsmajorityforaapvideoshow57559218cms` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttptimesofindiaindiatimescomvideosnewspunjabexitpollcvoterpredictsmajorityforaapvideoshow57559218cms`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpworldhuanqiucomhot2016089334639html` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpworldhuanqiucomhot2016089334639html`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpwwwozapcomactuinvitessalutlesterriensrecoitflorentpagnyetfredericlopez544047` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpwwwozapcomactuinvitessalutlesterriensrecoitflorentpagnyetfredericlopez544047`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpwwwprigepporgaulaforoanswerphpidcomentario301c4idforocc0idcrso467CodigoUni100190` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswebarchiveorgwebhttpwwwprigepporgaulaforoanswerphpidcomentario301c4idforocc0idcrso467CodigoUni100190`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswordpresscomblog20220519yourwebsitelooksgreatsoshouldyouremails` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswordpresscomblog20220519yourwebsitelooksgreatsoshouldyouremails`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswwwbanduolcombrbandnewsfmriodejaneironoticiasacusadodeassassinarnamoradaafacadastemprisaoconvertidaempreventiva16574059` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswwwbanduolcombrbandnewsfmriodejaneironoticiasacusadodeassassinarnamoradaafacadastemprisaoconvertidaempreventiva16574059`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswwwcnncom20220829weatherweathernewslabordaytropicalsystemtexasrainwxnindexhtml` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswwwcnncom20220829weatherweathernewslabordaytropicalsystemtexasrainwxnindexhtml`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswwwcnncom20231212entertainmentandrebraugherobitindexhtml` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswwwcnncom20231212entertainmentandrebraugherobitindexhtml`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswwwcnncom20231212politicstakeawaysvolodymyrzelenskywashingtonindexhtml` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswwwcnncom20231212politicstakeawaysvolodymyrzelenskywashingtonindexhtml`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswwwexamplecom` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswwwexamplecom`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswwwgpogovfdsyspkgPL` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswwwgpogovfdsyspkgPL`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswwwindiatimescomnewsindia75thindependencedayindiaaugust15576959html` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswwwindiatimescomnewsindia75thindependencedayindiaaugust15576959html`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswwwkenyatodaycommediamoiburialconfusedrutoasmatiangideclarestuesdayapublicholidaycomments` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswwwkenyatodaycommediamoiburialconfusedrutoasmatiangideclarestuesdayapublicholidaycomments`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswwwkpbsorgnews2019jul09migrantscameroonprotestimmigrationprocesstiju` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswwwkpbsorgnews2019jul09migrantscameroonprotestimmigrationprocesstiju`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswwwletrascombrbandandriveede` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswwwletrascombrbandandriveede`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswwwmkcokrnewssocietyview202007693939` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswwwmkcokrnewssocietyview202007693939`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswwwnytimescominteractive20181210businesslocationdataprivacyappshtml` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswwwnytimescominteractive20181210businesslocationdataprivacyappshtml`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswwwpeoplesdailyngcomfeed` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswwwpeoplesdailyngcomfeed`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswwwsydneyeduau` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswwwsydneyeduau`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswwwtrussvilletribunecom20220302threestudentsfromcenterpointreceiveacademicscholarships` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswwwtrussvilletribunecom20220302threestudentsfromcenterpointreceiveacademicscholarships`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswwwuniradioinformacomnoticiascoronavirus677354covidsegundacausademuerteenmexicoen2021htmlutm_sourcefeedutm_mediumlinkutm_campaignrss` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswwwuniradioinformacomnoticiascoronavirus677354covidsegundacausademuerteenmexicoen2021htmlutm_sourcefeedutm_mediumlinkutm_campaignrss`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswwwwdsucomarticleuntitledcontent170181311946044845` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswwwwdsucomarticleuntitledcontent170181311946044845`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpswwwyoutubecomwatchvaFCO6WidGVM` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpswwwyoutubecomwatchvaFCO6WidGVM`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpthekenyatimescomcountieskisumutradersalertedaboutcartelsinstallsissuance` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpthekenyatimescomcountieskisumutradersalertedaboutcartelsinstallsissuance`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httptrussvilletribunecom20220302threestudentsfromcenterpointreceiveacademicscholarships` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httptrussvilletribunecom20220302threestudentsfromcenterpointreceiveacademicscholarships`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpuniradioinformacomnoticiascoronavirus677126nuevossintomasdelcovidprolongadohtml` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpuniradioinformacomnoticiascoronavirus677126nuevossintomasdelcovidprolongadohtml`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpuniradioinformacomnoticiascoronavirus677126nuevossintomasdelcovidprolongadohtmlutm_campaignrssutm_mediumlink` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpuniradioinformacomnoticiascoronavirus677126nuevossintomasdelcovidprolongadohtmlutm_campaignrssutm_mediumlink`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpuniradioinformacomnoticiascoronavirus677354covidsegundacausademuerteenmexicoen2021html` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpuniradioinformacomnoticiascoronavirus677354covidsegundacausademuerteenmexicoen2021html`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpupstractcomxfdf95bf448e1f2a8` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpupstractcomxfdf95bf448e1f2a8`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpwwforgbr` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpwwforgbr`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpwwforjp` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpwwforjp`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpwwwdiariobahiadecadizcomnoticiassanfernandocavadayromeromantienenotroencuentrocondefensaparanegociarladesafectaciondesueloencamposotorequerirauntiempoindeterminado` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpwwwdiariobahiadecadizcomnoticiassanfernandocavadayromeromantienenotroencuentrocondefensaparanegociarladesafectaciondesueloencamposotorequerirauntiempoindeterminado`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpwwwgovcn` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpwwwgovcn`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpwwwinformecorrientescomvernotaaspid_noticia44619` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpwwwinformecorrientescomvernotaaspid_noticia44619`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpwwwnytimescom` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpwwwnytimescom`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpwwwnytimescomglobal` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpwwwnytimescomglobal`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpwwwwiredcom` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpwwwwiredcom`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/cached-httpyoutubecomwatchvaFCO6WidGVM` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/cached-httpyoutubecomwatchvaFCO6WidGVM`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/fixtures/focus-taiwan-202311170015.html` & `mediacloud_metadata-1.0.2/mcmetadata/test/fixtures/focus-taiwan-202311170015.html`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/test_content.py` & `mediacloud_metadata-1.0.2/mcmetadata/test/test_content.py`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/test_dates.py` & `mediacloud_metadata-1.0.2/mcmetadata/test/test_dates.py`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/test_extract.py` & `mediacloud_metadata-1.0.2/mcmetadata/test/test_extract.py`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/test_feeds.py` & `mediacloud_metadata-1.0.2/mcmetadata/test/test_feeds.py`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/test_languages.py` & `mediacloud_metadata-1.0.2/mcmetadata/test/test_languages.py`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/test_titles.py` & `mediacloud_metadata-1.0.2/mcmetadata/test/test_titles.py`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/test_urls.py` & `mediacloud_metadata-1.0.2/mcmetadata/test/test_urls.py`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/test/test_webpages.py` & `mediacloud_metadata-1.0.2/mcmetadata/test/test_webpages.py`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/text.py` & `mediacloud_metadata-1.0.2/mcmetadata/text.py`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/titles.py` & `mediacloud_metadata-1.0.2/mcmetadata/titles.py`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/urls.py` & `mediacloud_metadata-1.0.2/mcmetadata/urls.py`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/urlshortners.py` & `mediacloud_metadata-1.0.2/mcmetadata/urlshortners.py`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/mcmetadata/webpages.py` & `mediacloud_metadata-1.0.2/mcmetadata/webpages.py`

 * *Files identical despite different names*

### Comparing `mediacloud_metadata-1.0.1/pyproject.toml` & `mediacloud_metadata-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "mediacloud-metadata"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
     {name='Rahul Bhargava', email='rahul@mediacloud.org'}
 ]
 description='Media Cloud news article metadata extraction'
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `mediacloud_metadata-1.0.1/PKG-INFO` & `mediacloud_metadata-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mediacloud-metadata
-Version: 1.0.1
+Version: 1.0.2
 Summary: Media Cloud news article metadata extraction
 Author-email: Rahul Bhargava <rahul@mediacloud.org>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

