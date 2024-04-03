# Comparing `tmp/cdsclient-1.1.8.tar.gz` & `tmp/cdsclient-1.1.9.tar.gz`

## Comparing `cdsclient-1.1.8.tar` & `cdsclient-1.1.9.tar`

### file list

```diff
@@ -1,142 +1,143 @@
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 cdsclient-1.1.8/setup.old
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/LICENSE.txt
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/__init__.py
--rwxr-xr-x   0        0        0     9946 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_2020aj_159_84b.py
--rwxr-xr-x   0        0        0     7100 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_2mass.py
--rwxr-xr-x   0        0        0     9986 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_2mass6x.py
--rwxr-xr-x   0        0        0     7074 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_2psc3.py
--rwxr-xr-x   0        0        0    10090 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_allwise.py
--rwxr-xr-x   0        0        0     9962 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_allwise.v2.py
--rwxr-xr-x   0        0        0    10001 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_allwise_v2.py
--rwxr-xr-x   0        0        0     9933 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_apass9.py
--rwxr-xr-x   0        0        0     7071 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_apm.py
--rwxr-xr-x   0        0        0     9978 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_apop.py
--rwxr-xr-x   0        0        0     9922 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_atlas_refcat2.py
--rwxr-xr-x   0        0        0     9974 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_attitude.py
--rwxr-xr-x   0        0        0    10179 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_catwise.py
--rwxr-xr-x   0        0        0    10060 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_catwise2020.py
--rwxr-xr-x   0        0        0    10057 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_cfht_ls_d1to4.py
--rwxr-xr-x   0        0        0    10057 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_cfht_ls_w1to4.py
--rwxr-xr-x   0        0        0     7038 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_cmc14.py
--rwxr-xr-x   0        0        0     9916 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_cmc15.py
--rwxr-xr-x   0        0        0     7053 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_const.py
--rwxr-xr-x   0        0        0     7108 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_denis3.py
--rwxr-xr-x   0        0        0    10190 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_des_dr1.py
--rwxr-xr-x   0        0        0    10186 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_des_dr2.py
--rwxr-xr-x   0        0        0     9989 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_desi_lis_dr8_pzn.py
--rwxr-xr-x   0        0        0     9991 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_desi_lis_dr8_pzs.py
--rwxr-xr-x   0        0        0     9954 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_erass1_simu_agnin.py
--rwxr-xr-x   0        0        0     9977 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_gaia2_allwise_yso.py
--rwxr-xr-x   0        0        0     9866 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_gaia2_dist.py
--rwxr-xr-x   0        0        0    10234 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_gaia_dr1.py
--rwxr-xr-x   0        0        0    10590 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_gaia_dr2.py
--rwxr-xr-x   0        0        0     9883 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_gaia_dr2_teff.py
--rwxr-xr-x   0        0        0    10617 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_gaia_dr3.py
--rwxr-xr-x   0        0        0     9952 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_gaia_dr3_astroparams.py
--rwxr-xr-x   0        0        0     9969 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_gaia_dr3_astroparamssupp.py
--rwxr-xr-x   0        0        0     9972 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_gaia_dr3_epochphot.py
--rwxr-xr-x   0        0        0     9938 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_gaia_dr3_rvsmean.py
--rwxr-xr-x   0        0        0     9985 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_gaia_dr3_ssoobs.py
--rwxr-xr-x   0        0        0     9947 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_gaia_dr3_syntphot.py
--rwxr-xr-x   0        0        0     9976 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_gaia_dr3_varispursign.py
--rwxr-xr-x   0        0        0     9968 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_gaia_dr3_varisum.py
--rwxr-xr-x   0        0        0     9937 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_gaia_dr3_xpcont.py
--rwxr-xr-x   0        0        0     9941 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_gaia_dr3_xpsum.py
--rwxr-xr-x   0        0        0    10414 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_gaia_edr3.py
--rwxr-xr-x   0        0        0     9938 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_gaia_edr3_dist.py
--rwxr-xr-x   0        0        0     9943 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_gaia_fpr_lensobs.py
--rwxr-xr-x   0        0        0     9937 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_gaia_fpr_ssoobs.py
--rwxr-xr-x   0        0        0    10003 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_gaia_gums_gal.py
--rwxr-xr-x   0        0        0     9974 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_galex_gr5_ais.py
--rwxr-xr-x   0        0        0     9950 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_galex_gr5_mis.py
--rwxr-xr-x   0        0        0    10033 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_galex_gr67.py
--rwxr-xr-x   0        0        0     9948 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_gdr2_wise_gp.py
--rwxr-xr-x   0        0        0     9913 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_gdr2ap.py
--rwxr-xr-x   0        0        0     7116 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_glimpse.py
--rwxr-xr-x   0        0        0    10076 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_gps1.py
--rwxr-xr-x   0        0        0     9918 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_gps1_plus.py
--rwxr-xr-x   0        0        0     7038 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_gsc.py
--rwxr-xr-x   0        0        0     7005 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_gsc1.2.py
--rwxr-xr-x   0        0        0     7005 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_gsc1.3.py
--rwxr-xr-x   0        0        0     7044 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_gsc1_2.py
--rwxr-xr-x   0        0        0     7044 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_gsc1_3.py
--rwxr-xr-x   0        0        0     7086 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_gsc2.3.py
--rwxr-xr-x   0        0        0    10074 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_gsc242.py
--rwxr-xr-x   0        0        0    10109 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_gsc242_v2.py
--rwxr-xr-x   0        0        0     7125 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_gsc2_3.py
--rwxr-xr-x   0        0        0     9994 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_gums10_lmc.py
--rwxr-xr-x   0        0        0     9989 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_gums10_mw.py
--rwxr-xr-x   0        0        0     9994 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_gums10_smc.py
--rwxr-xr-x   0        0        0     9926 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_hsc1_detailed.py
--rwxr-xr-x   0        0        0     9926 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_hsc2_detailed.py
--rwxr-xr-x   0        0        0     9886 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_hsoy.py
--rwxr-xr-x   0        0        0    10123 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_igaps_dr1.py
--rwxr-xr-x   0        0        0    10160 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_igsl3.py
--rwxr-xr-x   0        0        0    10006 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_iphas_dr2.py
--rwxr-xr-x   0        0        0     9986 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_irsf_mcpsc.py
--rwxr-xr-x   0        0        0     9954 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_j_aa_669_a104.py
--rwxr-xr-x   0        0        0    10165 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_k2_epic.py
--rwxr-xr-x   0        0        0     7134 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_kic.py
--rwxr-xr-x   0        0        0    10012 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_kids_dr2.py
--rwxr-xr-x   0        0        0    10019 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_kids_dr3.py
--rwxr-xr-x   0        0        0     9990 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_lmcps.py
--rwxr-xr-x   0        0        0     9972 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_mc2.py
--rwxr-xr-x   0        0        0     7115 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_nomad1.py
--rwxr-xr-x   0        0        0     6308 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_notavailable.py
--rwxr-xr-x   0        0        0     9981 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_ogle_bulge.py
--rwxr-xr-x   0        0        0    10010 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_panstarrs_dr1.py
--rwxr-xr-x   0        0        0     9891 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_phat.py
--rwxr-xr-x   0        0        0     7034 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_pmm2.py
--rwxr-xr-x   0        0        0     7097 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_ppmx.py
--rwxr-xr-x   0        0        0     7102 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_ppmxl.py
--rwxr-xr-x   0        0        0     9942 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_rgbphotcal_gdr3.py
--rwxr-xr-x   0        0        0     9992 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_sage.py
--rwxr-xr-x   0        0        0    10007 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_sage_arch.py
--rwxr-xr-x   0        0        0     7150 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_sdss8.py
--rwxr-xr-x   0        0        0     7230 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_sdss9.py
--rwxr-xr-x   0        0        0    10222 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_sdss_dr12.py
--rwxr-xr-x   0        0        0    10220 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_sdss_dr16.py
--rwxr-xr-x   0        0        0     9954 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_seip_srclist_phot_dr4.py
--rwxr-xr-x   0        0        0     9902 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_skymapper_dr11.py
--rwxr-xr-x   0        0        0     9959 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_skymapper_dr4.py
--rwxr-xr-x   0        0        0     7144 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_spm4.py
--rwxr-xr-x   0        0        0     9926 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_starhorse.py
--rwxr-xr-x   0        0        0     9945 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_starhorse2021.py
--rwxr-xr-x   0        0        0     9991 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_tic.py
--rwxr-xr-x   0        0        0    10045 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_tic82.py
--rwxr-xr-x   0        0        0     7066 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_ucac3.py
--rwxr-xr-x   0        0        0     7146 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_ucac4.py
--rwxr-xr-x   0        0        0     9803 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_ucac5.py
--rwxr-xr-x   0        0        0    10022 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_ukidss_dr6_gps.py
--rwxr-xr-x   0        0        0     9999 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_ukidss_dr7_las.py
--rwxr-xr-x   0        0        0     9974 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_ukidss_dr8_dxs.py
--rwxr-xr-x   0        0        0    10046 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_ukidss_dr8_gcs.py
--rwxr-xr-x   0        0        0    10022 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_ukidss_dr8_las.py
--rwxr-xr-x   0        0        0     9974 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_ukidss_dr9_dxs.py
--rwxr-xr-x   0        0        0    10074 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_ukidss_dr9_gcs.py
--rwxr-xr-x   0        0        0     9998 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_ukidss_dr9_las.py
--rwxr-xr-x   0        0        0     9909 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_unwise.py
--rwxr-xr-x   0        0        0    10022 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_urat1.py
--rwxr-xr-x   0        0        0     7166 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_usnob1.py
--rwxr-xr-x   0        0        0     9919 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_vexasdes.py
--rwxr-xr-x   0        0        0     9914 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_vexasps.py
--rwxr-xr-x   0        0        0     9914 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_vexassm.py
--rwxr-xr-x   0        0        0    10023 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_vhs_dr41.py
--rwxr-xr-x   0        0        0    10044 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_vhs_dr5.py
--rwxr-xr-x   0        0        0    10055 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_viking_dr1.py
--rwxr-xr-x   0        0        0    10055 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_viking_dr2.py
--rwxr-xr-x   0        0        0    10080 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_vmc_cat_dr4.py
--rwxr-xr-x   0        0        0    10068 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_vmc_dr6.py
--rwxr-xr-x   0        0        0    10035 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_vphasplus_dr2.py
--rwxr-xr-x   0        0        0    10030 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_vst_atlas_dr3.py
--rwxr-xr-x   0        0        0    10026 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_vvv_cat_dr2.py
--rwxr-xr-x   0        0        0     9948 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_vvv_cat_dr4.py
--rwxr-xr-x   0        0        0    10014 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_vvv_dr1.py
--rwxr-xr-x   0        0        0    10086 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_vvv_virac_pm_dr41.py
--rwxr-xr-x   0        0        0     9989 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_wise_allsky.py
--rwxr-xr-x   0        0        0    10086 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/find_xpm.py
--rwxr-xr-x   0        0        0    12716 2020-02-02 00:00:00.000000 cdsclient-1.1.8/cdsclient/vizquery.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 cdsclient-1.1.8/.gitignore
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 cdsclient-1.1.8/README.md
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 cdsclient-1.1.8/pyproject.toml
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 cdsclient-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 cdsclient-1.1.9/__init__.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 cdsclient-1.1.9/setup.old
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/LICENSE.txt
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/__init__.py
+-rwxr-xr-x   0        0        0    10288 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_2020aj_159_84b.py
+-rwxr-xr-x   0        0        0     7332 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_2mass.py
+-rwxr-xr-x   0        0        0    10328 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_2mass6x.py
+-rwxr-xr-x   0        0        0     7306 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_2psc3.py
+-rwxr-xr-x   0        0        0    10090 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_allwise.py
+-rwxr-xr-x   0        0        0     9962 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_allwise.v2.py
+-rwxr-xr-x   0        0        0    10343 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_allwise_v2.py
+-rwxr-xr-x   0        0        0    10275 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_apass9.py
+-rwxr-xr-x   0        0        0     7303 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_apm.py
+-rwxr-xr-x   0        0        0    10320 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_apop.py
+-rwxr-xr-x   0        0        0    10264 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_atlas_refcat2.py
+-rwxr-xr-x   0        0        0    10316 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_attitude.py
+-rwxr-xr-x   0        0        0    10179 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_catwise.py
+-rwxr-xr-x   0        0        0    10402 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_catwise2020.py
+-rwxr-xr-x   0        0        0    10399 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_cfht_ls_d1to4.py
+-rwxr-xr-x   0        0        0    10399 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_cfht_ls_w1to4.py
+-rwxr-xr-x   0        0        0     7270 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_cmc14.py
+-rwxr-xr-x   0        0        0    10258 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_cmc15.py
+-rwxr-xr-x   0        0        0     7053 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_const.py
+-rwxr-xr-x   0        0        0     7340 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_denis3.py
+-rwxr-xr-x   0        0        0    10532 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_des_dr1.py
+-rwxr-xr-x   0        0        0    10528 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_des_dr2.py
+-rwxr-xr-x   0        0        0    10331 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_desi_lis_dr8_pzn.py
+-rwxr-xr-x   0        0        0    10333 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_desi_lis_dr8_pzs.py
+-rwxr-xr-x   0        0        0    10296 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_erass1_simu_agnin.py
+-rwxr-xr-x   0        0        0    10319 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_gaia2_allwise_yso.py
+-rwxr-xr-x   0        0        0    10208 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_gaia2_dist.py
+-rwxr-xr-x   0        0        0    10576 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_gaia_dr1.py
+-rwxr-xr-x   0        0        0    10932 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_gaia_dr2.py
+-rwxr-xr-x   0        0        0    10225 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_gaia_dr2_teff.py
+-rwxr-xr-x   0        0        0    10959 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_gaia_dr3.py
+-rwxr-xr-x   0        0        0    10294 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_gaia_dr3_astroparams.py
+-rwxr-xr-x   0        0        0    10311 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_gaia_dr3_astroparamssupp.py
+-rwxr-xr-x   0        0        0    10314 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_gaia_dr3_epochphot.py
+-rwxr-xr-x   0        0        0    10280 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_gaia_dr3_rvsmean.py
+-rwxr-xr-x   0        0        0    10327 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_gaia_dr3_ssoobs.py
+-rwxr-xr-x   0        0        0    10289 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_gaia_dr3_syntphot.py
+-rwxr-xr-x   0        0        0    10318 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_gaia_dr3_varispursign.py
+-rwxr-xr-x   0        0        0    10310 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_gaia_dr3_varisum.py
+-rwxr-xr-x   0        0        0    10279 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_gaia_dr3_xpcont.py
+-rwxr-xr-x   0        0        0    10283 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_gaia_dr3_xpsum.py
+-rwxr-xr-x   0        0        0    10756 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_gaia_edr3.py
+-rwxr-xr-x   0        0        0    10280 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_gaia_edr3_dist.py
+-rwxr-xr-x   0        0        0    10285 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_gaia_fpr_lensobs.py
+-rwxr-xr-x   0        0        0    10279 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_gaia_fpr_ssoobs.py
+-rwxr-xr-x   0        0        0    10345 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_gaia_gums_gal.py
+-rwxr-xr-x   0        0        0    10316 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_galex_gr5_ais.py
+-rwxr-xr-x   0        0        0    10292 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_galex_gr5_mis.py
+-rwxr-xr-x   0        0        0    10375 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_galex_gr67.py
+-rwxr-xr-x   0        0        0    10290 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_gdr2_wise_gp.py
+-rwxr-xr-x   0        0        0    10255 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_gdr2ap.py
+-rwxr-xr-x   0        0        0     7348 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_glimpse.py
+-rwxr-xr-x   0        0        0    10418 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_gps1.py
+-rwxr-xr-x   0        0        0    10260 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_gps1_plus.py
+-rwxr-xr-x   0        0        0     7270 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_gsc.py
+-rwxr-xr-x   0        0        0     7005 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_gsc1.2.py
+-rwxr-xr-x   0        0        0     7005 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_gsc1.3.py
+-rwxr-xr-x   0        0        0     7276 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_gsc1_2.py
+-rwxr-xr-x   0        0        0     7276 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_gsc1_3.py
+-rwxr-xr-x   0        0        0     7086 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_gsc2.3.py
+-rwxr-xr-x   0        0        0    10074 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_gsc242.py
+-rwxr-xr-x   0        0        0    10451 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_gsc242_v2.py
+-rwxr-xr-x   0        0        0     7357 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_gsc2_3.py
+-rwxr-xr-x   0        0        0    10336 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_gums10_lmc.py
+-rwxr-xr-x   0        0        0    10331 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_gums10_mw.py
+-rwxr-xr-x   0        0        0    10336 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_gums10_smc.py
+-rwxr-xr-x   0        0        0    10268 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_hsc1_detailed.py
+-rwxr-xr-x   0        0        0    10268 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_hsc2_detailed.py
+-rwxr-xr-x   0        0        0    10228 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_hsoy.py
+-rwxr-xr-x   0        0        0    10465 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_igaps_dr1.py
+-rwxr-xr-x   0        0        0    10502 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_igsl3.py
+-rwxr-xr-x   0        0        0    10348 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_iphas_dr2.py
+-rwxr-xr-x   0        0        0    10328 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_irsf_mcpsc.py
+-rwxr-xr-x   0        0        0    10296 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_j_aa_669_a104.py
+-rwxr-xr-x   0        0        0    10507 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_k2_epic.py
+-rwxr-xr-x   0        0        0     7366 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_kic.py
+-rwxr-xr-x   0        0        0    10354 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_kids_dr2.py
+-rwxr-xr-x   0        0        0    10361 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_kids_dr3.py
+-rwxr-xr-x   0        0        0    10332 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_lmcps.py
+-rwxr-xr-x   0        0        0    10314 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_mc2.py
+-rwxr-xr-x   0        0        0     7347 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_nomad1.py
+-rwxr-xr-x   0        0        0     6308 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_notavailable.py
+-rwxr-xr-x   0        0        0    10323 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_ogle_bulge.py
+-rwxr-xr-x   0        0        0    10352 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_panstarrs_dr1.py
+-rwxr-xr-x   0        0        0    10233 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_phat.py
+-rwxr-xr-x   0        0        0     7266 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_pmm2.py
+-rwxr-xr-x   0        0        0     7329 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_ppmx.py
+-rwxr-xr-x   0        0        0     7334 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_ppmxl.py
+-rwxr-xr-x   0        0        0    10284 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_rgbphotcal_gdr3.py
+-rwxr-xr-x   0        0        0    10334 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_sage.py
+-rwxr-xr-x   0        0        0    10349 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_sage_arch.py
+-rwxr-xr-x   0        0        0     7382 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_sdss8.py
+-rwxr-xr-x   0        0        0     7462 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_sdss9.py
+-rwxr-xr-x   0        0        0    10564 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_sdss_dr12.py
+-rwxr-xr-x   0        0        0    10562 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_sdss_dr16.py
+-rwxr-xr-x   0        0        0    10296 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_seip_srclist_phot_dr4.py
+-rwxr-xr-x   0        0        0    10244 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_skymapper_dr11.py
+-rwxr-xr-x   0        0        0    10301 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_skymapper_dr4.py
+-rwxr-xr-x   0        0        0     7376 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_spm4.py
+-rwxr-xr-x   0        0        0    10268 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_starhorse.py
+-rwxr-xr-x   0        0        0    10287 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_starhorse2021.py
+-rwxr-xr-x   0        0        0    10333 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_tic.py
+-rwxr-xr-x   0        0        0    10387 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_tic82.py
+-rwxr-xr-x   0        0        0     7298 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_ucac3.py
+-rwxr-xr-x   0        0        0     7378 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_ucac4.py
+-rwxr-xr-x   0        0        0    10145 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_ucac5.py
+-rwxr-xr-x   0        0        0    10364 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_ukidss_dr6_gps.py
+-rwxr-xr-x   0        0        0    10341 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_ukidss_dr7_las.py
+-rwxr-xr-x   0        0        0    10316 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_ukidss_dr8_dxs.py
+-rwxr-xr-x   0        0        0    10388 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_ukidss_dr8_gcs.py
+-rwxr-xr-x   0        0        0    10364 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_ukidss_dr8_las.py
+-rwxr-xr-x   0        0        0    10316 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_ukidss_dr9_dxs.py
+-rwxr-xr-x   0        0        0    10416 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_ukidss_dr9_gcs.py
+-rwxr-xr-x   0        0        0    10340 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_ukidss_dr9_las.py
+-rwxr-xr-x   0        0        0    10251 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_unwise.py
+-rwxr-xr-x   0        0        0    10364 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_urat1.py
+-rwxr-xr-x   0        0        0     7398 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_usnob1.py
+-rwxr-xr-x   0        0        0    10261 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_vexasdes.py
+-rwxr-xr-x   0        0        0    10256 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_vexasps.py
+-rwxr-xr-x   0        0        0    10256 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_vexassm.py
+-rwxr-xr-x   0        0        0    10365 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_vhs_dr41.py
+-rwxr-xr-x   0        0        0    10386 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_vhs_dr5.py
+-rwxr-xr-x   0        0        0    10397 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_viking_dr1.py
+-rwxr-xr-x   0        0        0    10397 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_viking_dr2.py
+-rwxr-xr-x   0        0        0    10422 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_vmc_cat_dr4.py
+-rwxr-xr-x   0        0        0    10410 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_vmc_dr6.py
+-rwxr-xr-x   0        0        0    10377 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_vphasplus_dr2.py
+-rwxr-xr-x   0        0        0    10372 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_vst_atlas_dr3.py
+-rwxr-xr-x   0        0        0    10368 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_vvv_cat_dr2.py
+-rwxr-xr-x   0        0        0    10290 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_vvv_cat_dr4.py
+-rwxr-xr-x   0        0        0    10356 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_vvv_dr1.py
+-rwxr-xr-x   0        0        0    10428 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_vvv_virac_pm_dr41.py
+-rwxr-xr-x   0        0        0    10331 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_wise_allsky.py
+-rwxr-xr-x   0        0        0    10428 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/find_xpm.py
+-rwxr-xr-x   0        0        0    12717 2020-02-02 00:00:00.000000 cdsclient-1.1.9/cdsclient/vizquery.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 cdsclient-1.1.9/.gitignore
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 cdsclient-1.1.9/README.md
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 cdsclient-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 cdsclient-1.1.9/PKG-INFO
```

### Comparing `cdsclient-1.1.8/setup.old` & `cdsclient-1.1.9/setup.old`

 * *Files identical despite different names*

### Comparing `cdsclient-1.1.8/cdsclient/LICENSE.txt` & `cdsclient-1.1.9/cdsclient/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cdsclient-1.1.8/cdsclient/find_2020aj_159_84b.py` & `cdsclient-1.1.9/cdsclient/find_2020aj_159_84b.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,25 +5,27 @@
    find_2020aj_159_84b.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
                 example: find_2020aj_159_84b.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
+		--noheader : ...
 		--Source= : ...
 		--RA_ICRS= : ...
 		--DE_ICRS= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
@@ -144,14 +146,15 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
@@ -178,14 +181,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -218,23 +224,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','Source=','RA_ICRS=','DE_ICRS=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','Source=','RA_ICRS=','DE_ICRS=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -263,14 +270,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -298,27 +308,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_2mass.py` & `cdsclient-1.1.9/cdsclient/find_gsc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query II/246/out
+   Query I/220/out
 
-   find_2mass.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_gsc.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_2mass.py M1
+                example: find_gsc.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
+		--noheader : ...
+		--GSC= : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
-		--2MASS= : ...
-		--Jmag= : ...
-		--Hmag= : ...
-		--Kmag= : ...
+		--Pmag= : ...
 
 
-     Example: --RAJ2000=">10"
+     Example: --GSC=">10"
 
      Licensed under a BSD license - see LICENSE.txt for details
 
 """
 
 import os, sys
 import getopt
@@ -109,15 +109,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("II/246/out", params=params, filename=filename)
+        self.__client.query("I/220/out", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -130,23 +130,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','RAJ2000=','DEJ2000=','2MASS=','Jmag=','Hmag=','Kmag=')
+    __options = ('help','format=','sort','add=','file=','noheader','GSC=','RAJ2000=','DEJ2000=','Pmag=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -175,14 +176,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -210,27 +214,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_2mass6x.py` & `cdsclient-1.1.9/cdsclient/find_gaia_dr3_epochphot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query II/281/2mass6x
+   Query I/355/epphot
 
-   find_2mass6x.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_gaia_dr3_epochphot.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_2mass6x.py M1
+                example: find_gaia_dr3_epochphot.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--2MASS= : ...
-		--RAJ2000= : ...
-		--DEJ2000= : ...
-		--Jmag= : ...
-		--Hmag= : ...
-		--Kmag= : ...
+		--noheader : ...
+		--Source= : ...
+		--RA_ICRS= : ...
+		--DE_ICRS= : ...
+		--TimeG= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --2MASS=">10"
+     Example: --Source=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -118,15 +118,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("II/281/2mass6x", params=params, filename=filename)
+        self.__client.query("I/355/epphot", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -147,26 +147,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=2MASS6X"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=gaia_dr3_epochphot"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -181,14 +182,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -221,23 +225,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','2MASS=','RAJ2000=','DEJ2000=','Jmag=','Hmag=','Kmag=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','Source=','RA_ICRS=','DE_ICRS=','TimeG=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -266,14 +271,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -301,27 +309,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_2psc3.py` & `cdsclient-1.1.9/cdsclient/find_apm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query II/241/out
+   Query I/267/out
 
-   find_2psc3.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_apm.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_2psc3.py M1
+                example: find_apm.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
+		--noheader : ...
+		--APM-ID= : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
-		--Jmag= : ...
-		--Hmag= : ...
-		--Kmag= : ...
+		--rmag= : ...
+		--bmag= : ...
 
 
-     Example: --RAJ2000=">10"
+     Example: --APM-ID=">10"
 
      Licensed under a BSD license - see LICENSE.txt for details
 
 """
 
 import os, sys
 import getopt
@@ -108,15 +110,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("II/241/out", params=params, filename=filename)
+        self.__client.query("I/267/out", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -129,23 +131,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','RAJ2000=','DEJ2000=','Jmag=','Hmag=','Kmag=')
+    __options = ('help','format=','sort','add=','file=','noheader','APM-ID=','RAJ2000=','DEJ2000=','rmag=','bmag=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -174,14 +177,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -209,27 +215,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_allwise.py` & `cdsclient-1.1.9/cdsclient/find_allwise.py`

 * *Files identical despite different names*

### Comparing `cdsclient-1.1.8/cdsclient/find_allwise.v2.py` & `cdsclient-1.1.9/cdsclient/find_allwise.v2.py`

 * *Files identical despite different names*

### Comparing `cdsclient-1.1.8/cdsclient/find_allwise_v2.py` & `cdsclient-1.1.9/cdsclient/find_ukidss_dr9_las.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query II/328/allwise
+   Query II/319/las9
 
-   find_allwise_v2.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_ukidss_dr9_las.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_allwise_v2.py M1
+                example: find_ukidss_dr9_las.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--AllWISE= : ...
+		--noheader : ...
+		--ULAS= : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
-		--Jmag= : ...
+		--Ymag= : ...
 		--Hmag= : ...
 		--Kmag= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --AllWISE=">10"
+     Example: --ULAS=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -118,15 +120,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("II/328/allwise", params=params, filename=filename)
+        self.__client.query("II/319/las9", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -147,26 +149,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=allwise.v2"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=ukidss_dr9_las"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -181,14 +184,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -221,23 +227,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','AllWISE=','RAJ2000=','DEJ2000=','Jmag=','Hmag=','Kmag=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','ULAS=','RAJ2000=','DEJ2000=','Ymag=','Hmag=','Kmag=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -266,14 +273,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -301,27 +311,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_apass9.py` & `cdsclient-1.1.9/cdsclient/find_galex_gr5_mis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query II/336/apass9
+   Query II/312/mis
 
-   find_apass9.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_galex_gr5_mis.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_apass9.py M1
+                example: find_galex_gr5_mis.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
+		--noheader : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
-		--Vmag= : ...
-		--Bmag= : ...
+		--phID= : ...
+		--objid= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
      Example: --RAJ2000=">10"
 
@@ -116,15 +118,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("II/336/apass9", params=params, filename=filename)
+        self.__client.query("II/312/mis", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -145,26 +147,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=APASS9"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=GALEX_GR5_MIS"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -179,14 +182,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -219,23 +225,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','RAJ2000=','DEJ2000=','Vmag=','Bmag=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','RAJ2000=','DEJ2000=','phID=','objid=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -264,14 +271,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -299,27 +309,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_apm.py` & `cdsclient-1.1.9/cdsclient/find_gsc1.3.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,44 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query I/267/out
+   Query I/255/out
 
-   find_apm.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_gsc1.3.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_apm.py M1
+                example: find_gsc1.3.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--APM-ID= : ...
+		--GSC= : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
-		--rmag= : ...
-		--bmag= : ...
+		--Pmag= : ...
 
 
-     Example: --APM-ID=">10"
+     Example: --GSC=">10"
 
      Licensed under a BSD license - see LICENSE.txt for details
 
 """
 
 import os, sys
 import getopt
-import cdsclient.vizquery as vizquery
-#import vizquery
+import vizquery
 
 if int(sys.version[0])<3:
     from urllib2 import quote
 else:
     from urllib.parse import quote
 
 NO_FORMAT = "noformat"
@@ -108,15 +106,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("I/267/out", params=params, filename=filename)
+        self.__client.query("I/255/out", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -137,15 +135,15 @@
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','APM-ID=','RAJ2000=','DEJ2000=','rmag=','bmag=')
+    __options = ('help','format=','sort','add=','file=','GSC=','RAJ2000=','DEJ2000=','Pmag=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_apop.py` & `cdsclient-1.1.9/cdsclient/find_gaia_dr3_astroparams.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,42 +1,40 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query I/331/apop
+   Query I/355/paramp
 
-   find_apop.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_gaia_dr3_astroparams.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_apop.py M1
+                example: find_gaia_dr3_astroparams.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--Rmag= : ...
-		--Bmag= : ...
-		--Nmag= : ...
-		--Vmag= : ...
-		--Jmag= : ...
-		--Hmag= : ...
-		--Kmag= : ...
+		--noheader : ...
+		--Source= : ...
+		--RA_ICRS= : ...
+		--DE_ICRS= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --Rmag=">10"
+     Example: --Source=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -119,15 +117,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("I/331/apop", params=params, filename=filename)
+        self.__client.query("I/355/paramp", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -148,26 +146,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=APOP"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=gaia_dr3_astroparams"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -182,14 +181,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -222,23 +224,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','Rmag=','Bmag=','Nmag=','Vmag=','Jmag=','Hmag=','Kmag=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','Source=','RA_ICRS=','DE_ICRS=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -267,14 +270,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -302,27 +308,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_atlas_refcat2.py` & `cdsclient-1.1.9/cdsclient/find_gaia_fpr_ssoobs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query J/ApJ/867/105/refcat2
+   Query I/361/ssoobs
 
-   find_atlas_refcat2.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_gaia_fpr_ssoobs.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_atlas_refcat2.py M1
+                example: find_gaia_fpr_ssoobs.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
+		--noheader : ...
+		--Source= : ...
 		--RA_ICRS= : ...
 		--DE_ICRS= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --RA_ICRS=">10"
+     Example: --Source=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -114,15 +117,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("J/ApJ/867/105/refcat2", params=params, filename=filename)
+        self.__client.query("I/361/ssoobs", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -143,26 +146,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=ATLAS_REFCAT2"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=gaia_fpr_ssoobs"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -177,14 +181,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -217,23 +224,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','RA_ICRS=','DE_ICRS=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','Source=','RA_ICRS=','DE_ICRS=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -262,14 +270,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -297,27 +308,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_attitude.py` & `cdsclient-1.1.9/cdsclient/find_atlas_refcat2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query VI/145/attitude
+   Query J/ApJ/867/105/refcat2
 
-   find_attitude.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_atlas_refcat2.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_attitude.py M1
+                example: find_atlas_refcat2.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--sourceId= : ...
-		--magBJ= : ...
-		--magRF= : ...
-		--magG= : ...
-		--magGrvs= : ...
+		--noheader : ...
+		--RA_ICRS= : ...
+		--DE_ICRS= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --sourceId=">10"
+     Example: --RA_ICRS=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -117,15 +116,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("VI/145/attitude", params=params, filename=filename)
+        self.__client.query("J/ApJ/867/105/refcat2", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -146,26 +145,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=ATTITUDE"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=ATLAS_REFCAT2"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -180,14 +180,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -220,23 +223,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','sourceId=','magBJ=','magRF=','magG=','magGrvs=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','RA_ICRS=','DE_ICRS=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -265,14 +269,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -300,27 +307,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_catwise.py` & `cdsclient-1.1.9/cdsclient/find_catwise.py`

 * *Files identical despite different names*

### Comparing `cdsclient-1.1.8/cdsclient/find_catwise2020.py` & `cdsclient-1.1.9/cdsclient/find_gsc242.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query II/365/catwise
+   Query I/353/gsc242
 
-   find_catwise2020.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_gsc242.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_catwise2020.py M1
+                example: find_gsc242.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--objID= : ...
+		--GSC2= : ...
 		--RA_ICRS= : ...
 		--DE_ICRS= : ...
-		--Name= : ...
-		--MJD= : ...
-		--W1mproPM= : ...
-		--W2mproPM= : ...
-		--Dist= : ...
+		--objID= : ...
+		--umag= : ...
+		--gmag= : ...
+		--rmag= : ...
+		--imag= : ...
+		--zmag= : ...
+		--ymag= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --objID=">10"
+     Example: --GSC2=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -120,15 +122,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("II/365/catwise", params=params, filename=filename)
+        self.__client.query("I/353/gsc242", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -160,15 +162,15 @@
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=catwise2020"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=gsc242"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -231,15 +233,15 @@
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','objID=','RA_ICRS=','DE_ICRS=','Name=','MJD=','W1mproPM=','W2mproPM=','Dist=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','GSC2=','RA_ICRS=','DE_ICRS=','objID=','umag=','gmag=','rmag=','imag=','zmag=','ymag=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_cfht_ls_d1to4.py` & `cdsclient-1.1.9/cdsclient/find_cfht_ls_d1to4.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,25 +5,27 @@
    find_cfht_ls_d1to4.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
                 example: find_cfht_ls_d1to4.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
+		--noheader : ...
 		--CFHTLS= : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
 		--umag= : ...
 		--gmag= : ...
 		--rmag= : ...
 		--imag= : ...
@@ -149,14 +151,15 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
@@ -183,14 +186,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -223,23 +229,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','CFHTLS=','RAJ2000=','DEJ2000=','umag=','gmag=','rmag=','imag=','zmag=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','CFHTLS=','RAJ2000=','DEJ2000=','umag=','gmag=','rmag=','imag=','zmag=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -268,14 +275,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -303,27 +313,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_cfht_ls_w1to4.py` & `cdsclient-1.1.9/cdsclient/find_cfht_ls_w1to4.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,25 +5,27 @@
    find_cfht_ls_w1to4.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
                 example: find_cfht_ls_w1to4.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
+		--noheader : ...
 		--CFHTLS= : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
 		--umag= : ...
 		--gmag= : ...
 		--rmag= : ...
 		--imag= : ...
@@ -149,14 +151,15 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
@@ -183,14 +186,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -223,23 +229,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','CFHTLS=','RAJ2000=','DEJ2000=','umag=','gmag=','rmag=','imag=','zmag=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','CFHTLS=','RAJ2000=','DEJ2000=','umag=','gmag=','rmag=','imag=','zmag=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -268,14 +275,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -303,27 +313,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_cmc14.py` & `cdsclient-1.1.9/cdsclient/find_gsc1.2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query I/304/out
+   Query I/254/out
 
-   find_cmc14.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_gsc1.2.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_cmc14.py M1
+                example: find_gsc1.2.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--CMC14= : ...
-		--Jmag= : ...
-		--Hmag= : ...
-		--Ksmag= : ...
+		--GSC= : ...
+		--RAJ2000= : ...
+		--DEJ2000= : ...
+		--Pmag= : ...
 
 
-     Example: --CMC14=">10"
+     Example: --GSC=">10"
 
      Licensed under a BSD license - see LICENSE.txt for details
 
 """
 
 import os, sys
 import getopt
-import cdsclient.vizquery as vizquery
-#import vizquery
+import vizquery
 
 if int(sys.version[0])<3:
     from urllib2 import quote
 else:
     from urllib.parse import quote
 
 NO_FORMAT = "noformat"
@@ -107,15 +106,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("I/304/out", params=params, filename=filename)
+        self.__client.query("I/254/out", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -136,15 +135,15 @@
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','CMC14=','Jmag=','Hmag=','Ksmag=')
+    __options = ('help','format=','sort','add=','file=','GSC=','RAJ2000=','DEJ2000=','Pmag=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_cmc15.py` & `cdsclient-1.1.9/cdsclient/find_irsf_mcpsc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query I/327/cmc15
+   Query II/288/out
 
-   find_cmc15.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_irsf_mcpsc.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_cmc15.py M1
+                example: find_irsf_mcpsc.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--CMC15= : ...
+		--noheader : ...
+		--IRSF= : ...
+		--RAJ2000= : ...
+		--DEJ2000= : ...
 		--Jmag= : ...
 		--Hmag= : ...
 		--Ksmag= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --CMC15=">10"
+     Example: --IRSF=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -116,15 +120,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("I/327/cmc15", params=params, filename=filename)
+        self.__client.query("II/288/out", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -145,26 +149,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=CMC15"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=IRSF_MCPSC"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -179,14 +184,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -219,23 +227,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','CMC15=','Jmag=','Hmag=','Ksmag=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','IRSF=','RAJ2000=','DEJ2000=','Jmag=','Hmag=','Ksmag=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -264,14 +273,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -299,27 +311,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_const.py` & `cdsclient-1.1.9/cdsclient/find_const.py`

 * *Files identical despite different names*

### Comparing `cdsclient-1.1.8/cdsclient/find_denis3.py` & `cdsclient-1.1.9/cdsclient/find_denis3.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,25 +5,27 @@
    find_denis3.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
                 example: find_denis3.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
+		--noheader : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
 		--Imag= : ...
 		--Jmag= : ...
 		--Kmag= : ...
 		--DENIS= : ...
 
@@ -130,23 +132,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','RAJ2000=','DEJ2000=','Imag=','Jmag=','Kmag=','DENIS=')
+    __options = ('help','format=','sort','add=','file=','noheader','RAJ2000=','DEJ2000=','Imag=','Jmag=','Kmag=','DENIS=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -175,14 +178,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -210,27 +216,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_des_dr1.py` & `cdsclient-1.1.9/cdsclient/find_k2_epic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query II/357/des_dr1
+   Query IV/34/epic
 
-   find_des_dr1.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_k2_epic.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_des_dr1.py M1
+                example: find_k2_epic.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
+		--noheader : ...
+		--ID= : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
-		--DES= : ...
-		--CoadID= : ...
+		--Bmag= : ...
+		--Vmag= : ...
+		--umag= : ...
 		--gmag= : ...
 		--rmag= : ...
 		--imag= : ...
 		--zmag= : ...
-		--Ymag= : ...
-		--gFlag= : ...
-		--rFlag= : ...
-		--iFlag= : ...
-		--zFlag= : ...
-		--YFlag= : ...
+		--Jmag= : ...
+		--Hmag= : ...
+		--Ksmag= : ...
+		--Kpmag= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --RAJ2000=">10"
+     Example: --ID=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -126,15 +128,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("II/357/des_dr1", params=params, filename=filename)
+        self.__client.query("IV/34/epic", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -155,26 +157,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=des_dr1"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=K2_EPIC"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -189,14 +192,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -229,23 +235,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','RAJ2000=','DEJ2000=','DES=','CoadID=','gmag=','rmag=','imag=','zmag=','Ymag=','gFlag=','rFlag=','iFlag=','zFlag=','YFlag=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','ID=','RAJ2000=','DEJ2000=','Bmag=','Vmag=','umag=','gmag=','rmag=','imag=','zmag=','Jmag=','Hmag=','Ksmag=','Kpmag=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -274,14 +281,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -309,27 +319,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_des_dr2.py` & `cdsclient-1.1.9/cdsclient/find_gaia2_allwise_yso.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,49 +1,41 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query II/371/des_dr2
+   Query II/360/catalog
 
-   find_des_dr2.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_gaia2_allwise_yso.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_des_dr2.py M1
+                example: find_gaia2_allwise_yso.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--DES= : ...
+		--noheader : ...
+		--Source= : ...
 		--RA_ICRS= : ...
 		--DE_ICRS= : ...
-		--CoadID= : ...
-		--gFlag= : ...
-		--rFlag= : ...
-		--iFlag= : ...
-		--zFlag= : ...
-		--yFlag= : ...
-		--gmag= : ...
-		--rmag= : ...
-		--imag= : ...
-		--zmag= : ...
-		--Ymag= : ...
+		--AllWISE= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --DES=">10"
+     Example: --Source=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -126,15 +118,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("II/371/des_dr2", params=params, filename=filename)
+        self.__client.query("II/360/catalog", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -155,26 +147,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=des_dr2"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=gaia2_allwise_yso"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -189,14 +182,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -229,23 +225,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','DES=','RA_ICRS=','DE_ICRS=','CoadID=','gFlag=','rFlag=','iFlag=','zFlag=','yFlag=','gmag=','rmag=','imag=','zmag=','Ymag=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','Source=','RA_ICRS=','DE_ICRS=','AllWISE=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -274,14 +271,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -309,27 +309,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_desi_lis_dr8_pzn.py` & `cdsclient-1.1.9/cdsclient/find_desi_lis_dr8_pzs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query VII/292/north
+   Query VII/292/south
 
-   find_desi_lis_dr8_pzn.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_desi_lis_dr8_pzs.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_desi_lis_dr8_pzn.py M1
+                example: find_desi_lis_dr8_pzs.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--objid= : ...
+		--noheader : ...
 		--brickid= : ...
-		--DEJ2000= : ...
+		--objid= : ...
 		--RAJ2000= : ...
 		--id= : ...
+		--DEJ2000= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --objid=">10"
+     Example: --brickid=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -117,15 +119,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("VII/292/north", params=params, filename=filename)
+        self.__client.query("VII/292/south", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -146,26 +148,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=desi_lis_dr8_pzn"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=desi_lis_dr8_pzs"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -180,14 +183,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -220,23 +226,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','objid=','brickid=','DEJ2000=','RAJ2000=','id=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','brickid=','objid=','RAJ2000=','id=','DEJ2000=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -265,14 +272,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -300,27 +310,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_desi_lis_dr8_pzs.py` & `cdsclient-1.1.9/cdsclient/find_desi_lis_dr8_pzn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query VII/292/south
+   Query VII/292/north
 
-   find_desi_lis_dr8_pzs.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_desi_lis_dr8_pzn.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_desi_lis_dr8_pzs.py M1
+                example: find_desi_lis_dr8_pzn.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--brickid= : ...
+		--noheader : ...
 		--objid= : ...
+		--brickid= : ...
+		--DEJ2000= : ...
 		--RAJ2000= : ...
 		--id= : ...
-		--DEJ2000= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --brickid=">10"
+     Example: --objid=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -117,15 +119,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("VII/292/south", params=params, filename=filename)
+        self.__client.query("VII/292/north", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -146,26 +148,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=desi_lis_dr8_pzs"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=desi_lis_dr8_pzn"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -180,14 +183,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -220,23 +226,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','brickid=','objid=','RAJ2000=','id=','DEJ2000=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','objid=','brickid=','DEJ2000=','RAJ2000=','id=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -265,14 +272,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -300,27 +310,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_erass1_simu_agnin.py` & `cdsclient-1.1.9/cdsclient/find_gaia_dr3_astroparamssupp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query J/A+A/665/A78/agnin
+   Query I/355/paramsup
 
-   find_erass1_simu_agnin.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_gaia_dr3_astroparamssupp.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_erass1_simu_agnin.py M1
+                example: find_gaia_dr3_astroparamssupp.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--SRCID= : ...
-		--DEJ2000= : ...
-		--RAJ2000= : ...
+		--noheader : ...
+		--RA_ICRS= : ...
+		--DE_ICRS= : ...
+		--Source= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --SRCID=">10"
+     Example: --RA_ICRS=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -115,15 +117,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("J/A+A/665/A78/agnin", params=params, filename=filename)
+        self.__client.query("I/355/paramsup", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -144,26 +146,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=erass1_simu_agnin"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=gaia_dr3_astroparamssupp"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -178,14 +181,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -218,23 +224,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','SRCID=','DEJ2000=','RAJ2000=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','RA_ICRS=','DE_ICRS=','Source=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -263,14 +270,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -298,27 +308,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_gaia2_allwise_yso.py` & `cdsclient-1.1.9/cdsclient/find_gaia_fpr_lensobs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query II/360/catalog
+   Query I/361/lensobs
 
-   find_gaia2_allwise_yso.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_gaia_fpr_lensobs.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_gaia2_allwise_yso.py M1
+                example: find_gaia_fpr_lensobs.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--Source= : ...
-		--RA_ICRS= : ...
+		--noheader : ...
 		--DE_ICRS= : ...
-		--AllWISE= : ...
+		--RA_ICRS= : ...
+		--Source= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --Source=">10"
+     Example: --DE_ICRS=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -116,15 +117,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("II/360/catalog", params=params, filename=filename)
+        self.__client.query("I/361/lensobs", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -145,26 +146,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=gaia2_allwise_yso"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=gaia_fpr_lensobs"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -179,14 +181,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -219,23 +224,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','Source=','RA_ICRS=','DE_ICRS=','AllWISE=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','DE_ICRS=','RA_ICRS=','Source=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -264,14 +270,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -299,27 +308,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_gaia2_dist.py` & `cdsclient-1.1.9/cdsclient/find_vexasdes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query I/347/gaia2dis
+   Query II/369/vexasdes
 
-   find_gaia2_dist.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_vexasdes.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_gaia2_dist.py M1
+                example: find_vexasdes.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--Source= : ...
+		--noheader : ...
+		--VISTA= : ...
+		--RAJ2000= : ...
+		--DEJ2000= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --Source=">10"
+     Example: --VISTA=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -113,15 +117,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("I/347/gaia2dis", params=params, filename=filename)
+        self.__client.query("II/369/vexasdes", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -142,26 +146,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=gaia2_dist"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=vexasdes"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -176,14 +181,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -216,23 +224,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','Source=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','VISTA=','RAJ2000=','DEJ2000=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -261,14 +270,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -296,27 +308,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_gaia_dr1.py` & `cdsclient-1.1.9/cdsclient/find_gaia_dr1.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,25 +5,27 @@
    find_gaia_dr1.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
                 example: find_gaia_dr1.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
+		--noheader : ...
 		--ra= : ...
 		--ra_error= : ...
 		--dec= : ...
 		--dec_error= : ...
 		--source_id= : ...
 		--parallax= : ...
 		--pmRA= : ...
@@ -154,14 +156,15 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
@@ -188,14 +191,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -228,23 +234,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','ra=','ra_error=','dec=','dec_error=','source_id=','parallax=','pmRA=','pmdec=','phot_g_mean_flux=','phot_g_mean_flux_error=','phot_g_mean_mag=','l=','b=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','ra=','ra_error=','dec=','dec_error=','source_id=','parallax=','pmRA=','pmdec=','phot_g_mean_flux=','phot_g_mean_flux_error=','phot_g_mean_mag=','l=','b=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -273,14 +280,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -308,27 +318,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_gaia_dr2.py` & `cdsclient-1.1.9/cdsclient/find_gaia_dr2.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,25 +5,27 @@
    find_gaia_dr2.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
                 example: find_gaia_dr2.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
+		--noheader : ...
 		--ra= : ...
 		--dec= : ...
 		--source_id= : ...
 		--random_index= : ...
 		--ref_epoch= : ...
 		--parallax= : ...
 		--parallax_error= : ...
@@ -163,14 +165,15 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
@@ -197,14 +200,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -237,23 +243,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','ra=','dec=','source_id=','random_index=','ref_epoch=','parallax=','parallax_error=','parallax_over_error=','pmra=','pmdec=','phot_g_mean_mag=','phot_bp_mean_mag=','phot_rp_mean_mag=','radial_velocity=','radial_velocity_error=','l=','b=','ra_epoch2000=','dec_epoch2000=','bp_g=','g_rp=','bp_rp=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','ra=','dec=','source_id=','random_index=','ref_epoch=','parallax=','parallax_error=','parallax_over_error=','pmra=','pmdec=','phot_g_mean_mag=','phot_bp_mean_mag=','phot_rp_mean_mag=','radial_velocity=','radial_velocity_error=','l=','b=','ra_epoch2000=','dec_epoch2000=','bp_g=','g_rp=','bp_rp=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -282,14 +289,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -317,27 +327,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_gaia_dr2_teff.py` & `cdsclient-1.1.9/cdsclient/find_gaia_dr3_ssoobs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query J/AJ/158/93/table2
+   Query I/359/ssoobs
 
-   find_gaia_dr2_teff.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_gaia_dr3_ssoobs.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_gaia_dr2_teff.py M1
+                example: find_gaia_dr3_ssoobs.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
+		--noheader : ...
 		--Source= : ...
+		--RA_ICRS= : ...
+		--DE_ICRS= : ...
+		--MPC= : ...
+		--Epoch= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
      Example: --Source=">10"
 
@@ -113,15 +119,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("J/AJ/158/93/table2", params=params, filename=filename)
+        self.__client.query("I/359/ssoobs", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -142,26 +148,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=GAIA_DR2_TEFF"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=gaia_dr3_ssoobs"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -176,14 +183,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -216,23 +226,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','Source=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','Source=','RA_ICRS=','DE_ICRS=','MPC=','Epoch=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -261,14 +272,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -296,27 +310,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_gaia_dr3.py` & `cdsclient-1.1.9/cdsclient/find_gaia_dr3.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,25 +5,27 @@
    find_gaia_dr3.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
                 example: find_gaia_dr3.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
+		--noheader : ...
 		--Plx= : ...
 		--Gmag= : ...
 		--PS1coid= : ...
 		--APASS9coid= : ...
 		--RPlx= : ...
 		--TYC2= : ...
 		--Source= : ...
@@ -171,14 +173,15 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
@@ -205,14 +208,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -245,23 +251,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','Plx=','Gmag=','PS1coid=','APASS9coid=','RPlx=','TYC2=','Source=','RV=','GLON=','URAT1=','RAVE5=','RAVE6=','AllWISE=','2MASS=','RA_ICRS=','RPmag=','GSC23=','DEJ2000=','DE_ICRS=','pmRA=','BPmag=','HIP=','APASS9=','GLAT=','RAJ2000=','pmDE=','BP-G=','G-RP=','BP-RP=','RandomI=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','Plx=','Gmag=','PS1coid=','APASS9coid=','RPlx=','TYC2=','Source=','RV=','GLON=','URAT1=','RAVE5=','RAVE6=','AllWISE=','2MASS=','RA_ICRS=','RPmag=','GSC23=','DEJ2000=','DE_ICRS=','pmRA=','BPmag=','HIP=','APASS9=','GLAT=','RAJ2000=','pmDE=','BP-G=','G-RP=','BP-RP=','RandomI=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -290,14 +297,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -325,27 +335,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_gaia_dr3_astroparams.py` & `cdsclient-1.1.9/cdsclient/find_gaia_dr2_teff.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query I/355/paramp
+   Query J/AJ/158/93/table2
 
-   find_gaia_dr3_astroparams.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_gaia_dr2_teff.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_gaia_dr3_astroparams.py M1
+                example: find_gaia_dr2_teff.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
+		--noheader : ...
 		--Source= : ...
-		--RA_ICRS= : ...
-		--DE_ICRS= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
      Example: --Source=">10"
 
@@ -115,15 +115,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("I/355/paramp", params=params, filename=filename)
+        self.__client.query("J/AJ/158/93/table2", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -144,26 +144,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=gaia_dr3_astroparams"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=GAIA_DR2_TEFF"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -178,14 +179,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -218,23 +222,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','Source=','RA_ICRS=','DE_ICRS=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','Source=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -263,14 +268,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -298,27 +306,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_gaia_dr3_astroparamssupp.py` & `cdsclient-1.1.9/cdsclient/find_gaia_dr3_rvsmean.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query I/355/paramsup
+   Query I/355/rvsmean
 
-   find_gaia_dr3_astroparamssupp.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_gaia_dr3_rvsmean.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_gaia_dr3_astroparamssupp.py M1
+                example: find_gaia_dr3_rvsmean.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--RA_ICRS= : ...
-		--DE_ICRS= : ...
+		--noheader : ...
 		--Source= : ...
+		--RAICRS= : ...
+		--DEICRS= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --RA_ICRS=">10"
+     Example: --Source=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -115,15 +117,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("I/355/paramsup", params=params, filename=filename)
+        self.__client.query("I/355/rvsmean", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -144,26 +146,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=gaia_dr3_astroparamssupp"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=gaia_dr3_rvsmean"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -178,14 +181,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -218,23 +224,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','RA_ICRS=','DE_ICRS=','Source=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','Source=','RAICRS=','DEICRS=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -263,14 +270,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -298,27 +308,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_gaia_dr3_epochphot.py` & `cdsclient-1.1.9/cdsclient/find_gaia_edr3_dist.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query I/355/epphot
+   Query I/352/gedr3dis
 
-   find_gaia_dr3_epochphot.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_gaia_edr3_dist.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_gaia_dr3_epochphot.py M1
+                example: find_gaia_edr3_dist.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
+		--noheader : ...
 		--Source= : ...
 		--RA_ICRS= : ...
 		--DE_ICRS= : ...
-		--TimeG= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
      Example: --Source=">10"
 
@@ -116,15 +117,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("I/355/epphot", params=params, filename=filename)
+        self.__client.query("I/352/gedr3dis", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -145,26 +146,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=gaia_dr3_epochphot"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=gaia_edr3_dist"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -179,14 +181,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -219,23 +224,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','Source=','RA_ICRS=','DE_ICRS=','TimeG=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','Source=','RA_ICRS=','DE_ICRS=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -264,14 +270,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -299,27 +308,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_gaia_dr3_rvsmean.py` & `cdsclient-1.1.9/cdsclient/find_hsoy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query I/355/rvsmean
+   Query I/339/hsoy
 
-   find_gaia_dr3_rvsmean.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_hsoy.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_gaia_dr3_rvsmean.py M1
+                example: find_hsoy.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--Source= : ...
-		--RAICRS= : ...
-		--DEICRS= : ...
+		--noheader : ...
+		--ipix= : ...
+		--GaiaId= : ...
+		--Gmag= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --Source=">10"
+     Example: --ipix=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -115,15 +117,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("I/355/rvsmean", params=params, filename=filename)
+        self.__client.query("I/339/hsoy", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -144,26 +146,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=gaia_dr3_rvsmean"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=HSOY"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -178,14 +181,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -218,23 +224,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','Source=','RAICRS=','DEICRS=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','ipix=','GaiaId=','Gmag=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -263,14 +270,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -298,27 +308,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_gaia_dr3_ssoobs.py` & `cdsclient-1.1.9/cdsclient/find_panstarrs_dr1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query I/359/ssoobs
+   Query II/349/ps1
 
-   find_gaia_dr3_ssoobs.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_panstarrs_dr1.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_gaia_dr3_ssoobs.py M1
+                example: find_panstarrs_dr1.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--Source= : ...
-		--RA_ICRS= : ...
-		--DE_ICRS= : ...
-		--MPC= : ...
+		--noheader : ...
+		--objID= : ...
 		--Epoch= : ...
+		--gmag= : ...
+		--rmag= : ...
+		--imag= : ...
+		--zmag= : ...
+		--ymag= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --Source=">10"
+     Example: --objID=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -117,15 +121,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("I/359/ssoobs", params=params, filename=filename)
+        self.__client.query("II/349/ps1", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -146,26 +150,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=gaia_dr3_ssoobs"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=PanSTARRS_DR1"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -180,14 +185,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -220,23 +228,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','Source=','RA_ICRS=','DE_ICRS=','MPC=','Epoch=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','objID=','Epoch=','gmag=','rmag=','imag=','zmag=','ymag=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -265,14 +274,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -300,27 +312,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_gaia_dr3_syntphot.py` & `cdsclient-1.1.9/cdsclient/find_ukidss_dr7_las.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query I/360/syntphot
+   Query II/310/las
 
-   find_gaia_dr3_syntphot.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_ukidss_dr7_las.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_gaia_dr3_syntphot.py M1
+                example: find_ukidss_dr7_las.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--Source= : ...
-		--RA_ICRS= : ...
-		--DE_ICRS= : ...
+		--noheader : ...
+		--RAJ2000= : ...
+		--DEJ2000= : ...
+		--Ymag= : ...
+		--Jmag= : ...
+		--Hmag= : ...
+		--Kmag= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --Source=">10"
+     Example: --RAJ2000=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -115,15 +120,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("I/360/syntphot", params=params, filename=filename)
+        self.__client.query("II/310/las", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -144,26 +149,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=gaia_dr3_syntphot"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=UKIDSS_DR7_LAS"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -178,14 +184,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -218,23 +227,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','Source=','RA_ICRS=','DE_ICRS=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','RAJ2000=','DEJ2000=','Ymag=','Jmag=','Hmag=','Kmag=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -263,14 +273,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -298,27 +311,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_gaia_dr3_varispursign.py` & `cdsclient-1.1.9/cdsclient/find_rgbphotcal_gdr3.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query J/A+A/674/A25/vspursig
+   Query II/374/table2
 
-   find_gaia_dr3_varispursign.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_rgbphotcal_gdr3.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_gaia_dr3_varispursign.py M1
+                example: find_rgbphotcal_gdr3.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
+		--noheader : ...
 		--DE_ICRS= : ...
-		--Source= : ...
 		--RA_ICRS= : ...
+		--GaiaDR3= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
      Example: --DE_ICRS=">10"
 
@@ -115,15 +117,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("J/A+A/674/A25/vspursig", params=params, filename=filename)
+        self.__client.query("II/374/table2", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -144,26 +146,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=gaia_dr3_varispursign"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=rgbphotcal_gdr3"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -178,14 +181,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -218,23 +224,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','DE_ICRS=','Source=','RA_ICRS=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','DE_ICRS=','RA_ICRS=','GaiaDR3=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -263,14 +270,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -298,27 +308,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_gaia_dr3_varisum.py` & `cdsclient-1.1.9/cdsclient/find_seip_srclist_phot_dr4.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query I/358/varisum
+   Query II/368/sstsl2
 
-   find_gaia_dr3_varisum.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_seip_srclist_phot_dr4.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_gaia_dr3_varisum.py M1
+                example: find_seip_srclist_phot_dr4.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--Source= : ...
-		--RA_ICRS= : ...
-		--DE_ICRS= : ...
-		--TimeG= : ...
+		--noheader : ...
+		--RAJ2000= : ...
+		--DEJ2000= : ...
+		--Name= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --Source=">10"
+     Example: --RAJ2000=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -116,15 +117,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("I/358/varisum", params=params, filename=filename)
+        self.__client.query("II/368/sstsl2", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -145,26 +146,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=gaia_dr3_varisum"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=seip_srclist_phot_dr4"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -179,14 +181,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -219,23 +224,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','Source=','RA_ICRS=','DE_ICRS=','TimeG=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','RAJ2000=','DEJ2000=','Name=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -264,14 +270,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -299,27 +308,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_gaia_dr3_xpcont.py` & `cdsclient-1.1.9/cdsclient/find_gaia_dr3_xpcont.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,25 +5,27 @@
    find_gaia_dr3_xpcont.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
                 example: find_gaia_dr3_xpcont.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
+		--noheader : ...
 		--Source= : ...
 		--RA_ICRS= : ...
 		--DE_ICRS= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
@@ -144,14 +146,15 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
@@ -178,14 +181,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -218,23 +224,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','Source=','RA_ICRS=','DE_ICRS=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','Source=','RA_ICRS=','DE_ICRS=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -263,14 +270,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -298,27 +308,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_gaia_dr3_xpsum.py` & `cdsclient-1.1.9/cdsclient/find_gaia_dr3_xpsum.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,25 +5,27 @@
    find_gaia_dr3_xpsum.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
                 example: find_gaia_dr3_xpsum.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
+		--noheader : ...
 		--RA_ICRS= : ...
 		--DE_ICRS= : ...
 		--Source= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
@@ -144,14 +146,15 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
@@ -178,14 +181,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -218,23 +224,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','RA_ICRS=','DE_ICRS=','Source=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','RA_ICRS=','DE_ICRS=','Source=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -263,14 +270,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -298,27 +308,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_gaia_edr3.py` & `cdsclient-1.1.9/cdsclient/find_des_dr1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,57 +1,51 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query I/350/gaiaedr3
+   Query II/357/des_dr1
 
-   find_gaia_edr3.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_des_dr1.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_gaia_edr3.py M1
+                example: find_des_dr1.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--RA_ICRS= : ...
-		--DE_ICRS= : ...
-		--Source= : ...
-		--RandomI= : ...
-		--Epoch= : ...
-		--Plx= : ...
-		--e_Plx= : ...
-		--RPlx= : ...
-		--pmRA= : ...
-		--pmDE= : ...
-		--Gmag= : ...
-		--BPmag= : ...
-		--RPmag= : ...
-		--RVDR2= : ...
-		--e_RVDR2= : ...
-		--GLON= : ...
-		--GLAT= : ...
+		--noheader : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
-		--BP-RP= : ...
-		--BP-G= : ...
-		--G-RP= : ...
+		--DES= : ...
+		--CoadID= : ...
+		--gmag= : ...
+		--rmag= : ...
+		--imag= : ...
+		--zmag= : ...
+		--Ymag= : ...
+		--gFlag= : ...
+		--rFlag= : ...
+		--iFlag= : ...
+		--zFlag= : ...
+		--YFlag= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --RA_ICRS=">10"
+     Example: --RAJ2000=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -134,15 +128,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("I/350/gaiaedr3", params=params, filename=filename)
+        self.__client.query("II/357/des_dr1", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -163,26 +157,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=GAIA_EDR3"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=des_dr1"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -197,14 +192,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -237,23 +235,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','RA_ICRS=','DE_ICRS=','Source=','RandomI=','Epoch=','Plx=','e_Plx=','RPlx=','pmRA=','pmDE=','Gmag=','BPmag=','RPmag=','RVDR2=','e_RVDR2=','GLON=','GLAT=','RAJ2000=','DEJ2000=','BP-RP=','BP-G=','G-RP=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','RAJ2000=','DEJ2000=','DES=','CoadID=','gmag=','rmag=','imag=','zmag=','Ymag=','gFlag=','rFlag=','iFlag=','zFlag=','YFlag=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -282,14 +281,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -317,27 +319,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_gaia_edr3_dist.py` & `cdsclient-1.1.9/cdsclient/find_gaia_dr3_syntphot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query I/352/gedr3dis
+   Query I/360/syntphot
 
-   find_gaia_edr3_dist.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_gaia_dr3_syntphot.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_gaia_edr3_dist.py M1
+                example: find_gaia_dr3_syntphot.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
+		--noheader : ...
 		--Source= : ...
 		--RA_ICRS= : ...
 		--DE_ICRS= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
@@ -115,15 +117,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("I/352/gedr3dis", params=params, filename=filename)
+        self.__client.query("I/360/syntphot", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -144,26 +146,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=gaia_edr3_dist"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=gaia_dr3_syntphot"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -178,14 +181,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -218,23 +224,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','Source=','RA_ICRS=','DE_ICRS=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','Source=','RA_ICRS=','DE_ICRS=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -263,14 +270,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -298,27 +308,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_gaia_fpr_lensobs.py` & `cdsclient-1.1.9/cdsclient/find_skymapper_dr11.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query I/361/lensobs
+   Query II/358/smss
 
-   find_gaia_fpr_lensobs.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_skymapper_dr11.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_gaia_fpr_lensobs.py M1
+                example: find_skymapper_dr11.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--DE_ICRS= : ...
-		--RA_ICRS= : ...
-		--Source= : ...
+		--noheader : ...
+		--ObjectId= : ...
+		--SMSS= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --DE_ICRS=">10"
+     Example: --ObjectId=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -115,15 +116,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("I/361/lensobs", params=params, filename=filename)
+        self.__client.query("II/358/smss", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -144,26 +145,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=gaia_fpr_lensobs"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=SKYMAPPER_DR11"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -178,14 +180,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -218,23 +223,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','DE_ICRS=','RA_ICRS=','Source=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','ObjectId=','SMSS=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -263,14 +269,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -298,27 +307,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_gaia_fpr_ssoobs.py` & `cdsclient-1.1.9/cdsclient/find_gaia_gums_gal.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query I/361/ssoobs
+   Query VI/137/gum_gal
 
-   find_gaia_fpr_ssoobs.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_gaia_gums_gal.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_gaia_fpr_ssoobs.py M1
+                example: find_gaia_gums_gal.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--Source= : ...
-		--RA_ICRS= : ...
-		--DE_ICRS= : ...
+		--noheader : ...
+		--Gmag= : ...
+		--GBmag= : ...
+		--GRmag= : ...
+		--Gsmag= : ...
+		--RAICRS= : ...
+		--DEICRS= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --Source=">10"
+     Example: --Gmag=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -115,15 +120,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("I/361/ssoobs", params=params, filename=filename)
+        self.__client.query("VI/137/gum_gal", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -144,26 +149,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=gaia_fpr_ssoobs"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=gaia_gums_gal"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -178,14 +184,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -218,23 +227,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','Source=','RA_ICRS=','DE_ICRS=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','Gmag=','GBmag=','GRmag=','Gsmag=','RAICRS=','DEICRS=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -263,14 +273,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -298,27 +311,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_gaia_gums_gal.py` & `cdsclient-1.1.9/cdsclient/find_vexassm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query VI/137/gum_gal
+   Query II/369/vexassm
 
-   find_gaia_gums_gal.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_vexassm.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_gaia_gums_gal.py M1
+                example: find_vexassm.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--Gmag= : ...
-		--GBmag= : ...
-		--GRmag= : ...
-		--Gsmag= : ...
-		--RAICRS= : ...
-		--DEICRS= : ...
+		--noheader : ...
+		--VISTA= : ...
+		--RAJ2000= : ...
+		--DEJ2000= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --Gmag=">10"
+     Example: --VISTA=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -118,15 +117,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("VI/137/gum_gal", params=params, filename=filename)
+        self.__client.query("II/369/vexassm", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -147,26 +146,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=gaia_gums_gal"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=vexassm"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -181,14 +181,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -221,23 +224,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','Gmag=','GBmag=','GRmag=','Gsmag=','RAICRS=','DEICRS=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','VISTA=','RAJ2000=','DEJ2000=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -266,14 +270,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -301,27 +308,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_galex_gr5_ais.py` & `cdsclient-1.1.9/cdsclient/find_galex_gr5_ais.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,25 +5,27 @@
    find_galex_gr5_ais.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
                 example: find_galex_gr5_ais.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
+		--noheader : ...
 		--recno= : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
 		--phID= : ...
 		--objid= : ...
 		--ipix= : ...
 		--no-format : ...
@@ -146,14 +148,15 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
@@ -180,14 +183,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -220,23 +226,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','recno=','RAJ2000=','DEJ2000=','phID=','objid=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','recno=','RAJ2000=','DEJ2000=','phID=','objid=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -265,14 +272,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -300,27 +310,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_galex_gr5_mis.py` & `cdsclient-1.1.9/cdsclient/find_vphasplus_dr2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query II/312/mis
+   Query II/341/vphasp
 
-   find_galex_gr5_mis.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_vphasplus_dr2.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_galex_gr5_mis.py M1
+                example: find_vphasplus_dr2.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
+		--noheader : ...
+		--sourceID= : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
-		--phID= : ...
-		--objid= : ...
+		--umag= : ...
+		--gmag= : ...
+		--rmag= : ...
+		--imag= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --RAJ2000=">10"
+     Example: --sourceID=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -116,15 +121,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("II/312/mis", params=params, filename=filename)
+        self.__client.query("II/341/vphasp", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -145,26 +150,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=GALEX_GR5_MIS"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=VPHASPLUS_DR2"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -179,14 +185,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -219,23 +228,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','RAJ2000=','DEJ2000=','phID=','objid=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','sourceID=','RAJ2000=','DEJ2000=','umag=','gmag=','rmag=','imag=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -264,14 +274,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -299,27 +312,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_galex_gr67.py` & `cdsclient-1.1.9/cdsclient/find_galex_gr67.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,25 +5,27 @@
    find_galex_gr67.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
                 example: find_galex_gr67.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
+		--noheader : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
 		--Name= : ...
 		--objid= : ...
 		--phID= : ...
 		--FUVmag= : ...
 		--NUVmag= : ...
@@ -148,14 +150,15 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
@@ -182,14 +185,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -222,23 +228,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','RAJ2000=','DEJ2000=','Name=','objid=','phID=','FUVmag=','NUVmag=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','RAJ2000=','DEJ2000=','Name=','objid=','phID=','FUVmag=','NUVmag=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -267,14 +274,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -302,27 +312,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_gdr2_wise_gp.py` & `cdsclient-1.1.9/cdsclient/find_gdr2_wise_gp.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,25 +5,27 @@
    find_gdr2_wise_gp.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
                 example: find_gdr2_wise_gp.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
+		--noheader : ...
 		--RAICRS= : ...
 		--DEICRS= : ...
 		--GAIA= : ...
 		--WISE= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
@@ -145,14 +147,15 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
@@ -179,14 +182,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -219,23 +225,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','RAICRS=','DEICRS=','GAIA=','WISE=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','RAICRS=','DEICRS=','GAIA=','WISE=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -264,14 +271,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -299,27 +309,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_gdr2ap.py` & `cdsclient-1.1.9/cdsclient/find_kids_dr3.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,44 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query V/155/gdr2ap
+   Query II/347/kids_dr3
 
-   find_gdr2ap.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_kids_dr3.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_gdr2ap.py M1
+                example: find_kids_dr3.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--GaiaDR2= : ...
-		--RA_ICRS= : ...
-		--DE_ICRS= : ...
+		--noheader : ...
+		--RAJ2000= : ...
+		--DEJ2000= : ...
+		--CollID= : ...
+		--umag= : ...
+		--gmag= : ...
+		--rmag= : ...
+		--imag= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --GaiaDR2=">10"
+     Example: --RAJ2000=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -115,15 +121,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("V/155/gdr2ap", params=params, filename=filename)
+        self.__client.query("II/347/kids_dr3", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -144,26 +150,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=gdr2ap"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=KIDS_DR3"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -178,14 +185,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -218,23 +228,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','GaiaDR2=','RA_ICRS=','DE_ICRS=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','RAJ2000=','DEJ2000=','CollID=','umag=','gmag=','rmag=','imag=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -263,14 +274,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -298,27 +312,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_glimpse.py` & `cdsclient-1.1.9/cdsclient/find_sdss8.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query II/293/glimpse
+   Query II/306/sdss8
 
-   find_glimpse.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_sdss8.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_glimpse.py M1
+                example: find_sdss8.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--GLIMPSE= : ...
-		--RAJ2000= : ...
-		--DEJ2000= : ...
-		--Jmag= : ...
-		--Hmag= : ...
-		--Kmag= : ...
+		--noheader : ...
+		--SDSS8= : ...
+		--RA_ICRS= : ...
+		--DE_ICRS= : ...
+		--umag= : ...
+		--gmag= : ...
+		--rmag= : ...
+		--imag= : ...
+		--zmag= : ...
 
 
-     Example: --GLIMPSE=">10"
+     Example: --SDSS8=">10"
 
      Licensed under a BSD license - see LICENSE.txt for details
 
 """
 
 import os, sys
 import getopt
@@ -109,15 +113,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("II/293/glimpse", params=params, filename=filename)
+        self.__client.query("II/306/sdss8", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -130,23 +134,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','GLIMPSE=','RAJ2000=','DEJ2000=','Jmag=','Hmag=','Kmag=')
+    __options = ('help','format=','sort','add=','file=','noheader','SDSS8=','RA_ICRS=','DE_ICRS=','umag=','gmag=','rmag=','imag=','zmag=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -175,14 +180,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -210,27 +218,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_gps1.py` & `cdsclient-1.1.9/cdsclient/find_vvv_cat_dr2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,44 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query I/343/gps1
+   Query II/348/vvv2
 
-   find_gps1.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_vvv_cat_dr2.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_gps1.py M1
+                example: find_vvv_cat_dr2.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--pmRA= : ...
-		--pmDE= : ...
-		--gmag= : ...
-		--rmag= : ...
-		--imag= : ...
-		--zmag= : ...
-		--ymag= : ...
-		--Jmag= : ...
-		--Hmag= : ...
-		--Ksmag= : ...
-		--Gmag= : ...
+		--noheader : ...
+		--srcid= : ...
+		--RAJ2000= : ...
+		--DEJ2000= : ...
+		--Ymag3= : ...
+		--Jmag3= : ...
+		--Hmag3= : ...
+		--Ksmag3= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --pmRA=">10"
+     Example: --srcid=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -123,15 +121,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("I/343/gps1", params=params, filename=filename)
+        self.__client.query("II/348/vvv2", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -152,26 +150,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=GPS1"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=VVV_CAT_DR2"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -186,14 +185,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -226,23 +228,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','pmRA=','pmDE=','gmag=','rmag=','imag=','zmag=','ymag=','Jmag=','Hmag=','Ksmag=','Gmag=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','srcid=','RAJ2000=','DEJ2000=','Ymag3=','Jmag3=','Hmag3=','Ksmag3=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -271,14 +274,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -306,27 +312,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_gps1_plus.py` & `cdsclient-1.1.9/cdsclient/find_vexasps.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query I/351/gps1_p
+   Query II/369/vexasps
 
-   find_gps1_plus.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_vexasps.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_gps1_plus.py M1
+                example: find_vexasps.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--RA_ICRS= : ...
-		--DE_ICRS= : ...
-		--objID= : ...
+		--noheader : ...
+		--VISTA= : ...
+		--RAJ2000= : ...
+		--DEJ2000= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --RA_ICRS=">10"
+     Example: --VISTA=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -115,15 +117,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("I/351/gps1_p", params=params, filename=filename)
+        self.__client.query("II/369/vexasps", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -144,26 +146,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=gps1_plus"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=vexasps"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -178,14 +181,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -218,23 +224,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','RA_ICRS=','DE_ICRS=','objID=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','VISTA=','RAJ2000=','DEJ2000=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -263,14 +270,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -298,27 +308,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_gsc.py` & `cdsclient-1.1.9/cdsclient/find_gsc2.3.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query I/220/out
+   Query I/305/out
 
-   find_gsc.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_gsc2.3.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_gsc.py M1
+                example: find_gsc2.3.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--GSC= : ...
+		--GSC2.3= : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
-		--Pmag= : ...
+		--Fmag= : ...
+		--jmag= : ...
+		--Vmag= : ...
+		--Nmag= : ...
 
 
-     Example: --GSC=">10"
+     Example: --GSC2.3=">10"
 
      Licensed under a BSD license - see LICENSE.txt for details
 
 """
 
 import os, sys
 import getopt
-import cdsclient.vizquery as vizquery
-#import vizquery
+import vizquery
 
 if int(sys.version[0])<3:
     from urllib2 import quote
 else:
     from urllib.parse import quote
 
 NO_FORMAT = "noformat"
@@ -107,15 +109,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("I/220/out", params=params, filename=filename)
+        self.__client.query("I/305/out", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -136,15 +138,15 @@
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','GSC=','RAJ2000=','DEJ2000=','Pmag=')
+    __options = ('help','format=','sort','add=','file=','GSC2.3=','RAJ2000=','DEJ2000=','Fmag=','jmag=','Vmag=','Nmag=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_gsc1.2.py` & `cdsclient-1.1.9/cdsclient/find_gsc1_3.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query I/254/out
+   Query I/255/out
 
-   find_gsc1.2.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_gsc1_3.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_gsc1.2.py M1
+                example: find_gsc1_3.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
+		--noheader : ...
 		--GSC= : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
 		--Pmag= : ...
 
 
      Example: --GSC=">10"
 
      Licensed under a BSD license - see LICENSE.txt for details
 
 """
 
 import os, sys
 import getopt
-import vizquery
+import cdsclient.vizquery as vizquery
+#import vizquery
 
 if int(sys.version[0])<3:
     from urllib2 import quote
 else:
     from urllib.parse import quote
 
 NO_FORMAT = "noformat"
@@ -106,15 +109,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("I/254/out", params=params, filename=filename)
+        self.__client.query("I/255/out", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -127,23 +130,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','GSC=','RAJ2000=','DEJ2000=','Pmag=')
+    __options = ('help','format=','sort','add=','file=','noheader','GSC=','RAJ2000=','DEJ2000=','Pmag=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -172,14 +176,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -207,27 +214,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_gsc1.3.py` & `cdsclient-1.1.9/cdsclient/find_gsc1_2.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query I/255/out
+   Query I/254/out
 
-   find_gsc1.3.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_gsc1_2.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_gsc1.3.py M1
+                example: find_gsc1_2.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
+		--noheader : ...
 		--GSC= : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
 		--Pmag= : ...
 
 
      Example: --GSC=">10"
 
      Licensed under a BSD license - see LICENSE.txt for details
 
 """
 
 import os, sys
 import getopt
-import vizquery
+import cdsclient.vizquery as vizquery
+#import vizquery
 
 if int(sys.version[0])<3:
     from urllib2 import quote
 else:
     from urllib.parse import quote
 
 NO_FORMAT = "noformat"
@@ -106,15 +109,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("I/255/out", params=params, filename=filename)
+        self.__client.query("I/254/out", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -127,23 +130,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','GSC=','RAJ2000=','DEJ2000=','Pmag=')
+    __options = ('help','format=','sort','add=','file=','noheader','GSC=','RAJ2000=','DEJ2000=','Pmag=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -172,14 +176,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -207,27 +214,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_gsc1_2.py` & `cdsclient-1.1.9/cdsclient/find_pmm2.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query I/254/out
+   Query I/252/out
 
-   find_gsc1_2.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_pmm2.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_gsc1_2.py M1
+                example: find_pmm2.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--GSC= : ...
+		--noheader : ...
+		--USNO-A2.0= : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
-		--Pmag= : ...
 
 
-     Example: --GSC=">10"
+     Example: --USNO-A2.0=">10"
 
      Licensed under a BSD license - see LICENSE.txt for details
 
 """
 
 import os, sys
 import getopt
@@ -107,15 +108,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("I/254/out", params=params, filename=filename)
+        self.__client.query("I/252/out", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -128,23 +129,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','GSC=','RAJ2000=','DEJ2000=','Pmag=')
+    __options = ('help','format=','sort','add=','file=','noheader','USNO-A2.0=','RAJ2000=','DEJ2000=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -173,14 +175,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -208,27 +213,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_gsc1_3.py` & `cdsclient-1.1.9/cdsclient/find_kic.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query I/255/out
+   Query V/133/kic
 
-   find_gsc1_3.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_kic.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_gsc1_3.py M1
+                example: find_kic.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--GSC= : ...
+		--noheader : ...
+		--KIC= : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
-		--Pmag= : ...
+		--umag= : ...
+		--gmag= : ...
+		--rmag= : ...
+		--imag= : ...
+		--zmag= : ...
 
 
-     Example: --GSC=">10"
+     Example: --KIC=">10"
 
      Licensed under a BSD license - see LICENSE.txt for details
 
 """
 
 import os, sys
 import getopt
@@ -107,15 +113,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("I/255/out", params=params, filename=filename)
+        self.__client.query("V/133/kic", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -128,23 +134,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','GSC=','RAJ2000=','DEJ2000=','Pmag=')
+    __options = ('help','format=','sort','add=','file=','noheader','KIC=','RAJ2000=','DEJ2000=','umag=','gmag=','rmag=','imag=','zmag=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -173,14 +180,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -208,27 +218,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_gsc2.3.py` & `cdsclient-1.1.9/cdsclient/find_cmc14.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query I/305/out
+   Query I/304/out
 
-   find_gsc2.3.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_cmc14.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_gsc2.3.py M1
+                example: find_cmc14.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--GSC2.3= : ...
-		--RAJ2000= : ...
-		--DEJ2000= : ...
-		--Fmag= : ...
-		--jmag= : ...
-		--Vmag= : ...
-		--Nmag= : ...
+		--noheader : ...
+		--CMC14= : ...
+		--Jmag= : ...
+		--Hmag= : ...
+		--Ksmag= : ...
 
 
-     Example: --GSC2.3=">10"
+     Example: --CMC14=">10"
 
      Licensed under a BSD license - see LICENSE.txt for details
 
 """
 
 import os, sys
 import getopt
-import vizquery
+import cdsclient.vizquery as vizquery
+#import vizquery
 
 if int(sys.version[0])<3:
     from urllib2 import quote
 else:
     from urllib.parse import quote
 
 NO_FORMAT = "noformat"
@@ -109,15 +109,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("I/305/out", params=params, filename=filename)
+        self.__client.query("I/304/out", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -130,23 +130,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','GSC2.3=','RAJ2000=','DEJ2000=','Fmag=','jmag=','Vmag=','Nmag=')
+    __options = ('help','format=','sort','add=','file=','noheader','CMC14=','Jmag=','Hmag=','Ksmag=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -175,14 +176,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -210,27 +214,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_gsc242.py` & `cdsclient-1.1.9/cdsclient/find_gsc242_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
    Query I/353/gsc242
 
-   find_gsc242.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_gsc242_v2.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_gsc242.py M1
+                example: find_gsc242_v2.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
+		--noheader : ...
 		--GSC2= : ...
 		--RA_ICRS= : ...
 		--DE_ICRS= : ...
 		--objID= : ...
+		--Epoch= : ...
 		--umag= : ...
 		--gmag= : ...
 		--rmag= : ...
 		--imag= : ...
 		--zmag= : ...
 		--ymag= : ...
 		--ipix= : ...
@@ -151,26 +154,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=gsc242"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=gsc242_v2"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -185,14 +189,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -225,23 +232,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','GSC2=','RA_ICRS=','DE_ICRS=','objID=','umag=','gmag=','rmag=','imag=','zmag=','ymag=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','GSC2=','RA_ICRS=','DE_ICRS=','objID=','Epoch=','umag=','gmag=','rmag=','imag=','zmag=','ymag=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -270,14 +278,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -305,27 +316,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_gsc242_v2.py` & `cdsclient-1.1.9/cdsclient/find_gps1_plus.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,40 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query I/353/gsc242
+   Query I/351/gps1_p
 
-   find_gsc242_v2.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_gps1_plus.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_gsc242_v2.py M1
+                example: find_gps1_plus.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--GSC2= : ...
+		--noheader : ...
 		--RA_ICRS= : ...
 		--DE_ICRS= : ...
 		--objID= : ...
-		--Epoch= : ...
-		--umag= : ...
-		--gmag= : ...
-		--rmag= : ...
-		--imag= : ...
-		--zmag= : ...
-		--ymag= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --GSC2=">10"
+     Example: --RA_ICRS=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -123,15 +117,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("I/353/gsc242", params=params, filename=filename)
+        self.__client.query("I/351/gps1_p", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -152,26 +146,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=gsc242_v2"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=gps1_plus"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -186,14 +181,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -226,23 +224,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','GSC2=','RA_ICRS=','DE_ICRS=','objID=','Epoch=','umag=','gmag=','rmag=','imag=','zmag=','ymag=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','RA_ICRS=','DE_ICRS=','objID=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -271,14 +270,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -306,27 +308,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_gsc2_3.py` & `cdsclient-1.1.9/cdsclient/find_nomad1.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query I/305/out
+   Query I/297/out
 
-   find_gsc2_3.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_nomad1.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_gsc2_3.py M1
+                example: find_nomad1.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--GSC2.3= : ...
+		--noheader : ...
+		--NOMAD1= : ...
+		--USNO-B1= : ...
+		--UCAC2= : ...
+		--Tycho-2= : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
-		--Fmag= : ...
-		--jmag= : ...
-		--Vmag= : ...
-		--Nmag= : ...
 
 
-     Example: --GSC2.3=">10"
+     Example: --NOMAD1=">10"
 
      Licensed under a BSD license - see LICENSE.txt for details
 
 """
 
 import os, sys
 import getopt
@@ -110,15 +111,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("I/305/out", params=params, filename=filename)
+        self.__client.query("I/297/out", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -131,23 +132,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','GSC2.3=','RAJ2000=','DEJ2000=','Fmag=','jmag=','Vmag=','Nmag=')
+    __options = ('help','format=','sort','add=','file=','noheader','NOMAD1=','USNO-B1=','UCAC2=','Tycho-2=','RAJ2000=','DEJ2000=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -176,14 +178,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -211,27 +216,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_gums10_lmc.py` & `cdsclient-1.1.9/cdsclient/find_ukidss_dr8_dxs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query VI/137/gum_lmc
+   Query II/314/dxs8
 
-   find_gums10_lmc.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_ukidss_dr8_dxs.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_gums10_lmc.py M1
+                example: find_ukidss_dr8_dxs.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--Gmag= : ...
-		--GBmag= : ...
-		--GRmag= : ...
-		--Gsmag= : ...
-		--RAICRS= : ...
-		--DEICRS= : ...
+		--noheader : ...
+		--UDXS= : ...
+		--RAJ2000= : ...
+		--DEJ2000= : ...
+		--Jmag= : ...
+		--Kmag= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --Gmag=">10"
+     Example: --UDXS=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -118,15 +119,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("VI/137/gum_lmc", params=params, filename=filename)
+        self.__client.query("II/314/dxs8", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -147,26 +148,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=gums10_lmc"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=ukidss_dr8_dxs"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -181,14 +183,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -221,23 +226,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','Gmag=','GBmag=','GRmag=','Gsmag=','RAICRS=','DEICRS=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','UDXS=','RAJ2000=','DEJ2000=','Jmag=','Kmag=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -266,14 +272,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -301,27 +310,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_gums10_mw.py` & `cdsclient-1.1.9/cdsclient/find_ukidss_dr8_las.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query VI/137/gum_mw
+   Query II/314/las8
 
-   find_gums10_mw.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_ukidss_dr8_las.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_gums10_mw.py M1
+                example: find_ukidss_dr8_las.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--Gmag= : ...
-		--GBmag= : ...
-		--GRmag= : ...
-		--Gsmag= : ...
-		--RAICRS= : ...
-		--DEICRS= : ...
+		--noheader : ...
+		--ULAS= : ...
+		--RAJ2000= : ...
+		--DEJ2000= : ...
+		--Ymag= : ...
+		--Jmag= : ...
+		--Hmag= : ...
+		--Kmag= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --Gmag=">10"
+     Example: --ULAS=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -118,15 +121,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("VI/137/gum_mw", params=params, filename=filename)
+        self.__client.query("II/314/las8", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -147,26 +150,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=gums10_mw"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=ukidss_dr8_las"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -181,14 +185,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -221,23 +228,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','Gmag=','GBmag=','GRmag=','Gsmag=','RAICRS=','DEICRS=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','ULAS=','RAJ2000=','DEJ2000=','Ymag=','Jmag=','Hmag=','Kmag=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -266,14 +274,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -301,27 +312,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_gums10_smc.py` & `cdsclient-1.1.9/cdsclient/find_ukidss_dr9_dxs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query VI/137/gum_smc
+   Query II/319/dxs9
 
-   find_gums10_smc.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_ukidss_dr9_dxs.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_gums10_smc.py M1
+                example: find_ukidss_dr9_dxs.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--Gmag= : ...
-		--GBmag= : ...
-		--GRmag= : ...
-		--Gsmag= : ...
-		--RAICRS= : ...
-		--DEICRS= : ...
+		--noheader : ...
+		--UDXS= : ...
+		--RAJ2000= : ...
+		--DEJ2000= : ...
+		--Jmag= : ...
+		--Kmag= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --Gmag=">10"
+     Example: --UDXS=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -118,15 +119,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("VI/137/gum_smc", params=params, filename=filename)
+        self.__client.query("II/319/dxs9", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -147,26 +148,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=gums10_smc"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=ukidss_dr9_dxs"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -181,14 +183,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -221,23 +226,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','Gmag=','GBmag=','GRmag=','Gsmag=','RAICRS=','DEICRS=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','UDXS=','RAJ2000=','DEJ2000=','Jmag=','Kmag=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -266,14 +272,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -301,27 +310,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_hsc1_detailed.py` & `cdsclient-1.1.9/cdsclient/find_lmcps.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query II/342/hsc1
+   Query J/AJ/128/1606/lmcps
 
-   find_hsc1_detailed.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_lmcps.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_hsc1_detailed.py M1
+                example: find_lmcps.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--CatID= : ...
+		--noheader : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
+		--Umag= : ...
+		--Bmag= : ...
+		--Vmag= : ...
+		--Imag= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --CatID=">10"
+     Example: --RAJ2000=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -115,15 +120,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("II/342/hsc1", params=params, filename=filename)
+        self.__client.query("J/AJ/128/1606/lmcps", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -144,26 +149,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=HSC1_DETAILED"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=LMCPS"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -178,14 +184,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -218,23 +227,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','CatID=','RAJ2000=','DEJ2000=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','RAJ2000=','DEJ2000=','Umag=','Bmag=','Vmag=','Imag=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -263,14 +273,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -298,27 +311,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_hsc2_detailed.py` & `cdsclient-1.1.9/cdsclient/find_vst_atlas_dr3.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,38 +1,44 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query II/342/hsc2
+   Query II/350/vstatlas
 
-   find_hsc2_detailed.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_vst_atlas_dr3.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_hsc2_detailed.py M1
+                example: find_vst_atlas_dr3.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--CatID= : ...
+		--noheader : ...
+		--SrcID= : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
+		--Uap3= : ...
+		--Rap3= : ...
+		--Iap3= : ...
+		--Zap3= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --CatID=">10"
+     Example: --SrcID=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -115,15 +121,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("II/342/hsc2", params=params, filename=filename)
+        self.__client.query("II/350/vstatlas", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -144,26 +150,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=HSC2_DETAILED"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=VST_ATLAS_DR3"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -178,14 +185,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -218,23 +228,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','CatID=','RAJ2000=','DEJ2000=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','SrcID=','RAJ2000=','DEJ2000=','Uap3=','Rap3=','Iap3=','Zap3=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -263,14 +274,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -298,27 +312,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_hsoy.py` & `cdsclient-1.1.9/cdsclient/find_iphas_dr2.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,44 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query I/339/hsoy
+   Query II/321/iphas2
 
-   find_hsoy.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_iphas_dr2.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_hsoy.py M1
+                example: find_iphas_dr2.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--ipix= : ...
-		--GaiaId= : ...
-		--Gmag= : ...
+		--noheader : ...
+		--IPHAS= : ...
+		--RAJ2000= : ...
+		--DEJ2000= : ...
+		--sourceID= : ...
+		--r= : ...
+		--i= : ...
+		--ha= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --ipix=">10"
+     Example: --IPHAS=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -115,15 +121,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("I/339/hsoy", params=params, filename=filename)
+        self.__client.query("II/321/iphas2", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -144,26 +150,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=HSOY"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=IPHAS_DR2"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -178,14 +185,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -218,23 +228,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','ipix=','GaiaId=','Gmag=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','IPHAS=','RAJ2000=','DEJ2000=','sourceID=','r=','i=','ha=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -263,14 +274,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -298,27 +312,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_igaps_dr1.py` & `cdsclient-1.1.9/cdsclient/find_attitude.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,42 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query V/165/igapsdr1
+   Query VI/145/attitude
 
-   find_igaps_dr1.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_attitude.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_igaps_dr1.py M1
+                example: find_attitude.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--Name= : ...
-		--RAJ2000= : ...
-		--DEJ2000= : ...
-		--SourceID= : ...
-		--imag= : ...
-		--MJDi= : ...
-		--Hamag= : ...
-		--rImag= : ...
-		--rUmag= : ...
-		--gmag= : ...
-		--Umag= : ...
+		--noheader : ...
+		--sourceId= : ...
+		--magBJ= : ...
+		--magRF= : ...
+		--magG= : ...
+		--magGrvs= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --Name=">10"
+     Example: --sourceId=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -123,15 +119,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("V/165/igapsdr1", params=params, filename=filename)
+        self.__client.query("VI/145/attitude", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -152,26 +148,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=igaps_dr1"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=ATTITUDE"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -186,14 +183,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -226,23 +226,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','Name=','RAJ2000=','DEJ2000=','SourceID=','imag=','MJDi=','Hamag=','rImag=','rUmag=','gmag=','Umag=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','sourceId=','magBJ=','magRF=','magG=','magGrvs=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -271,14 +272,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -306,27 +310,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_igsl3.py` & `cdsclient-1.1.9/cdsclient/find_igsl3.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,25 +5,27 @@
    find_igsl3.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
                 example: find_igsl3.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
+		--noheader : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
 		--magBJ= : ...
 		--magRF= : ...
 		--idGSC23= : ...
 		--idSDSS= : ...
 		--idUCAC= : ...
@@ -153,14 +155,15 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
@@ -187,14 +190,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -227,23 +233,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','RAJ2000=','DEJ2000=','magBJ=','magRF=','idGSC23=','idSDSS=','idUCAC=','idTYCHO=','idHIP=','idPPMXL=','idOGLE=','idTMASS=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','RAJ2000=','DEJ2000=','magBJ=','magRF=','idGSC23=','idSDSS=','idUCAC=','idTYCHO=','idHIP=','idPPMXL=','idOGLE=','idTMASS=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -272,14 +279,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -307,27 +317,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_iphas_dr2.py` & `cdsclient-1.1.9/cdsclient/find_mc2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query II/321/iphas2
+   Query IV/33/mc2
 
-   find_iphas_dr2.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_mc2.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_iphas_dr2.py M1
+                example: find_mc2.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--IPHAS= : ...
+		--noheader : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
-		--sourceID= : ...
-		--r= : ...
-		--i= : ...
-		--ha= : ...
+		--2MASS= : ...
+		--DCMC= : ...
+		--GSC2.2= : ...
+		--UCAC1= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --IPHAS=">10"
+     Example: --RAJ2000=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -119,15 +120,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("II/321/iphas2", params=params, filename=filename)
+        self.__client.query("IV/33/mc2", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -148,26 +149,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=IPHAS_DR2"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=mc2"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -182,14 +184,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -222,23 +227,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','IPHAS=','RAJ2000=','DEJ2000=','sourceID=','r=','i=','ha=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','RAJ2000=','DEJ2000=','2MASS=','DCMC=','GSC2.2=','UCAC1=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -267,14 +273,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -302,27 +311,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_irsf_mcpsc.py` & `cdsclient-1.1.9/cdsclient/find_cmc15.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query II/288/out
+   Query I/327/cmc15
 
-   find_irsf_mcpsc.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_cmc15.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_irsf_mcpsc.py M1
+                example: find_cmc15.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--IRSF= : ...
-		--RAJ2000= : ...
-		--DEJ2000= : ...
+		--noheader : ...
+		--CMC15= : ...
 		--Jmag= : ...
 		--Hmag= : ...
 		--Ksmag= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --IRSF=">10"
+     Example: --CMC15=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -118,15 +118,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("II/288/out", params=params, filename=filename)
+        self.__client.query("I/327/cmc15", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -147,26 +147,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=IRSF_MCPSC"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=CMC15"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -181,14 +182,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -221,23 +225,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','IRSF=','RAJ2000=','DEJ2000=','Jmag=','Hmag=','Ksmag=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','CMC15=','Jmag=','Hmag=','Ksmag=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -266,14 +271,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -301,27 +309,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_j_aa_669_a104.py` & `cdsclient-1.1.9/cdsclient/find_gdr2ap.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query J/A+A/669/A104/catalog
+   Query V/155/gdr2ap
 
-   find_j_aa_669_a104.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_gdr2ap.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_j_aa_669_a104.py M1
+                example: find_gdr2ap.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--DE_ICRS= : ...
+		--noheader : ...
+		--GaiaDR2= : ...
 		--RA_ICRS= : ...
-		--GaiaDR3= : ...
+		--DE_ICRS= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --DE_ICRS=">10"
+     Example: --GaiaDR2=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -115,15 +117,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("J/A+A/669/A104/catalog", params=params, filename=filename)
+        self.__client.query("V/155/gdr2ap", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -144,26 +146,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=j_aa_669_a104"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=gdr2ap"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -178,14 +181,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -218,23 +224,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','DE_ICRS=','RA_ICRS=','GaiaDR3=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','GaiaDR2=','RA_ICRS=','DE_ICRS=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -263,14 +270,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -298,27 +308,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_k2_epic.py` & `cdsclient-1.1.9/cdsclient/find_gaia_edr3.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,49 +1,59 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query IV/34/epic
+   Query I/350/gaiaedr3
 
-   find_k2_epic.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_gaia_edr3.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_k2_epic.py M1
+                example: find_gaia_edr3.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--ID= : ...
+		--noheader : ...
+		--RA_ICRS= : ...
+		--DE_ICRS= : ...
+		--Source= : ...
+		--RandomI= : ...
+		--Epoch= : ...
+		--Plx= : ...
+		--e_Plx= : ...
+		--RPlx= : ...
+		--pmRA= : ...
+		--pmDE= : ...
+		--Gmag= : ...
+		--BPmag= : ...
+		--RPmag= : ...
+		--RVDR2= : ...
+		--e_RVDR2= : ...
+		--GLON= : ...
+		--GLAT= : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
-		--Bmag= : ...
-		--Vmag= : ...
-		--umag= : ...
-		--gmag= : ...
-		--rmag= : ...
-		--imag= : ...
-		--zmag= : ...
-		--Jmag= : ...
-		--Hmag= : ...
-		--Ksmag= : ...
-		--Kpmag= : ...
+		--BP-RP= : ...
+		--BP-G= : ...
+		--G-RP= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --ID=">10"
+     Example: --RA_ICRS=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -126,15 +136,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("IV/34/epic", params=params, filename=filename)
+        self.__client.query("I/350/gaiaedr3", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -155,26 +165,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=K2_EPIC"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=GAIA_EDR3"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -189,14 +200,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -229,23 +243,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','ID=','RAJ2000=','DEJ2000=','Bmag=','Vmag=','umag=','gmag=','rmag=','imag=','zmag=','Jmag=','Hmag=','Ksmag=','Kpmag=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','RA_ICRS=','DE_ICRS=','Source=','RandomI=','Epoch=','Plx=','e_Plx=','RPlx=','pmRA=','pmDE=','Gmag=','BPmag=','RPmag=','RVDR2=','e_RVDR2=','GLON=','GLAT=','RAJ2000=','DEJ2000=','BP-RP=','BP-G=','G-RP=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -274,14 +289,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -309,27 +327,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_kic.py` & `cdsclient-1.1.9/cdsclient/find_gsc2_3.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query V/133/kic
+   Query I/305/out
 
-   find_kic.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_gsc2_3.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_kic.py M1
+                example: find_gsc2_3.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--KIC= : ...
+		--noheader : ...
+		--GSC2.3= : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
-		--umag= : ...
-		--gmag= : ...
-		--rmag= : ...
-		--imag= : ...
-		--zmag= : ...
+		--Fmag= : ...
+		--jmag= : ...
+		--Vmag= : ...
+		--Nmag= : ...
 
 
-     Example: --KIC=">10"
+     Example: --GSC2.3=">10"
 
      Licensed under a BSD license - see LICENSE.txt for details
 
 """
 
 import os, sys
 import getopt
@@ -111,15 +112,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("V/133/kic", params=params, filename=filename)
+        self.__client.query("I/305/out", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -132,23 +133,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','KIC=','RAJ2000=','DEJ2000=','umag=','gmag=','rmag=','imag=','zmag=')
+    __options = ('help','format=','sort','add=','file=','noheader','GSC2.3=','RAJ2000=','DEJ2000=','Fmag=','jmag=','Vmag=','Nmag=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -177,14 +179,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -212,27 +217,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_kids_dr2.py` & `cdsclient-1.1.9/cdsclient/find_kids_dr2.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,25 +5,27 @@
    find_kids_dr2.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
                 example: find_kids_dr2.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
+		--noheader : ...
 		--KiDS= : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
 		--gmag= : ...
 		--imag= : ...
 		--rmag= : ...
 		--umag= : ...
@@ -148,14 +150,15 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
@@ -182,14 +185,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -222,23 +228,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','KiDS=','RAJ2000=','DEJ2000=','gmag=','imag=','rmag=','umag=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','KiDS=','RAJ2000=','DEJ2000=','gmag=','imag=','rmag=','umag=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -267,14 +274,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -302,27 +312,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_kids_dr3.py` & `cdsclient-1.1.9/cdsclient/find_vvv_cat_dr4.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query II/347/kids_dr3
+   Query II/376/vvv4
 
-   find_kids_dr3.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_vvv_cat_dr4.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_kids_dr3.py M1
+                example: find_vvv_cat_dr4.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
+		--noheader : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
-		--CollID= : ...
-		--umag= : ...
-		--gmag= : ...
-		--rmag= : ...
-		--imag= : ...
+		--SrcID= : ...
+		--Z1MJD= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
      Example: --RAJ2000=">10"
 
@@ -119,15 +118,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("II/347/kids_dr3", params=params, filename=filename)
+        self.__client.query("II/376/vvv4", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -148,26 +147,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=KIDS_DR3"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=vvv_cat_dr4"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -182,14 +182,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -222,23 +225,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','RAJ2000=','DEJ2000=','CollID=','umag=','gmag=','rmag=','imag=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','RAJ2000=','DEJ2000=','SrcID=','Z1MJD=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -267,14 +271,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -302,27 +309,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_lmcps.py` & `cdsclient-1.1.9/cdsclient/find_phat.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query J/AJ/128/1606/lmcps
+   Query J/ApJS/215/9/table5
 
-   find_lmcps.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_phat.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_lmcps.py M1
+                example: find_phat.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
+		--noheader : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
-		--Umag= : ...
-		--Bmag= : ...
-		--Vmag= : ...
-		--Imag= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
      Example: --RAJ2000=">10"
 
@@ -118,15 +116,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("J/AJ/128/1606/lmcps", params=params, filename=filename)
+        self.__client.query("J/ApJS/215/9/table5", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -147,26 +145,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=LMCPS"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=phat"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -181,14 +180,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -221,23 +223,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','RAJ2000=','DEJ2000=','Umag=','Bmag=','Vmag=','Imag=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','RAJ2000=','DEJ2000=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -266,14 +269,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -301,27 +307,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_mc2.py` & `cdsclient-1.1.9/cdsclient/find_wise_allsky.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query IV/33/mc2
+   Query II/311/wise
 
-   find_mc2.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_wise_allsky.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_mc2.py M1
+                example: find_wise_allsky.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
+		--noheader : ...
+		--WISE= : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
-		--2MASS= : ...
-		--DCMC= : ...
-		--GSC2.2= : ...
-		--UCAC1= : ...
+		--Jmag= : ...
+		--Hmag= : ...
+		--Kmag= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --RAJ2000=">10"
+     Example: --WISE=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -118,15 +120,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("IV/33/mc2", params=params, filename=filename)
+        self.__client.query("II/311/wise", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -147,26 +149,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=mc2"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=WISE_ALLSKY"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -181,14 +184,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -221,23 +227,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','RAJ2000=','DEJ2000=','2MASS=','DCMC=','GSC2.2=','UCAC1=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','WISE=','RAJ2000=','DEJ2000=','Jmag=','Hmag=','Kmag=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -266,14 +273,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -301,27 +311,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_nomad1.py` & `cdsclient-1.1.9/cdsclient/find_2psc3.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query I/297/out
+   Query II/241/out
 
-   find_nomad1.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_2psc3.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_nomad1.py M1
+                example: find_2psc3.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--NOMAD1= : ...
-		--USNO-B1= : ...
-		--UCAC2= : ...
-		--Tycho-2= : ...
+		--noheader : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
+		--Jmag= : ...
+		--Hmag= : ...
+		--Kmag= : ...
 
 
-     Example: --NOMAD1=">10"
+     Example: --RAJ2000=">10"
 
      Licensed under a BSD license - see LICENSE.txt for details
 
 """
 
 import os, sys
 import getopt
@@ -109,15 +110,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("I/297/out", params=params, filename=filename)
+        self.__client.query("II/241/out", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -130,23 +131,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','NOMAD1=','USNO-B1=','UCAC2=','Tycho-2=','RAJ2000=','DEJ2000=')
+    __options = ('help','format=','sort','add=','file=','noheader','RAJ2000=','DEJ2000=','Jmag=','Hmag=','Kmag=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -175,14 +177,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -210,27 +215,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_notavailable.py` & `cdsclient-1.1.9/cdsclient/find_notavailable.py`

 * *Files identical despite different names*

### Comparing `cdsclient-1.1.8/cdsclient/find_ogle_bulge.py` & `cdsclient-1.1.9/cdsclient/find_ogle_bulge.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,25 +5,27 @@
    find_ogle_bulge.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
                 example: find_ogle_bulge.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
+		--noheader : ...
 		--recno= : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
 		--Vmag= : ...
 		--Imag= : ...
 		--ipix= : ...
 		--no-format : ...
@@ -146,14 +148,15 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
@@ -180,14 +183,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -220,23 +226,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','recno=','RAJ2000=','DEJ2000=','Vmag=','Imag=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','recno=','RAJ2000=','DEJ2000=','Vmag=','Imag=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -265,14 +272,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -300,27 +310,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_panstarrs_dr1.py` & `cdsclient-1.1.9/cdsclient/find_ucac5.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,37 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query II/349/ps1
+   Query I/340/ucac5
 
-   find_panstarrs_dr1.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_ucac5.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_panstarrs_dr1.py M1
+                example: find_ucac5.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--objID= : ...
-		--Epoch= : ...
-		--gmag= : ...
-		--rmag= : ...
-		--imag= : ...
-		--zmag= : ...
-		--ymag= : ...
+		--noheader : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --objID=">10"
+     Example: 
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -119,15 +114,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("II/349/ps1", params=params, filename=filename)
+        self.__client.query("I/340/ucac5", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -148,26 +143,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=PanSTARRS_DR1"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=UCAC5"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -182,14 +178,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -222,23 +221,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','objID=','Epoch=','gmag=','rmag=','imag=','zmag=','ymag=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -267,14 +267,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -302,27 +305,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_phat.py` & `cdsclient-1.1.9/cdsclient/find_unwise.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query J/ApJS/215/9/table5
+   Query II/363/unwise
 
-   find_phat.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_unwise.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_phat.py M1
+                example: find_unwise.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
+		--noheader : ...
+		--objID= : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --RAJ2000=">10"
+     Example: --objID=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -114,15 +117,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("J/ApJS/215/9/table5", params=params, filename=filename)
+        self.__client.query("II/363/unwise", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -143,26 +146,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=phat"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=unwise"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -177,14 +181,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -217,23 +224,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','RAJ2000=','DEJ2000=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','objID=','RAJ2000=','DEJ2000=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -262,14 +270,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -297,27 +308,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_pmm2.py` & `cdsclient-1.1.9/cdsclient/find_ppmx.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query I/252/out
+   Query I/312/sample
 
-   find_pmm2.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_ppmx.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_pmm2.py M1
+                example: find_ppmx.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--USNO-A2.0= : ...
+		--noheader : ...
+		--PPMX= : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
+		--Jmag= : ...
+		--Hmag= : ...
+		--Kmag= : ...
 
 
-     Example: --USNO-A2.0=">10"
+     Example: --PPMX=">10"
 
      Licensed under a BSD license - see LICENSE.txt for details
 
 """
 
 import os, sys
 import getopt
@@ -106,15 +111,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("I/252/out", params=params, filename=filename)
+        self.__client.query("I/312/sample", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -127,23 +132,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','USNO-A2.0=','RAJ2000=','DEJ2000=')
+    __options = ('help','format=','sort','add=','file=','noheader','PPMX=','RAJ2000=','DEJ2000=','Jmag=','Hmag=','Kmag=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -172,14 +178,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -207,27 +216,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_ppmx.py` & `cdsclient-1.1.9/cdsclient/find_ppmxl.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query I/312/sample
+   Query I/317/sample
 
-   find_ppmx.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_ppmxl.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_ppmx.py M1
+                example: find_ppmxl.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--PPMX= : ...
+		--noheader : ...
+		--PPMXL= : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
 		--Jmag= : ...
 		--Hmag= : ...
 		--Kmag= : ...
 
 
-     Example: --PPMX=">10"
+     Example: --PPMXL=">10"
 
      Licensed under a BSD license - see LICENSE.txt for details
 
 """
 
 import os, sys
 import getopt
@@ -109,15 +111,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("I/312/sample", params=params, filename=filename)
+        self.__client.query("I/317/sample", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -130,23 +132,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','PPMX=','RAJ2000=','DEJ2000=','Jmag=','Hmag=','Kmag=')
+    __options = ('help','format=','sort','add=','file=','noheader','PPMXL=','RAJ2000=','DEJ2000=','Jmag=','Hmag=','Kmag=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -175,14 +178,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -210,27 +216,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_ppmxl.py` & `cdsclient-1.1.9/cdsclient/find_ucac3.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query I/317/sample
+   Query I/315/out
 
-   find_ppmxl.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_ucac3.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_ppmxl.py M1
+                example: find_ucac3.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--PPMXL= : ...
+		--noheader : ...
+		--3UC= : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
 		--Jmag= : ...
-		--Hmag= : ...
 		--Kmag= : ...
 
 
-     Example: --PPMXL=">10"
+     Example: --3UC=">10"
 
      Licensed under a BSD license - see LICENSE.txt for details
 
 """
 
 import os, sys
 import getopt
@@ -109,15 +110,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("I/317/sample", params=params, filename=filename)
+        self.__client.query("I/315/out", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -130,23 +131,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','PPMXL=','RAJ2000=','DEJ2000=','Jmag=','Hmag=','Kmag=')
+    __options = ('help','format=','sort','add=','file=','noheader','3UC=','RAJ2000=','DEJ2000=','Jmag=','Kmag=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -175,14 +177,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -210,27 +215,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_rgbphotcal_gdr3.py` & `cdsclient-1.1.9/cdsclient/find_j_aa_669_a104.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query II/374/table2
+   Query J/A+A/669/A104/catalog
 
-   find_rgbphotcal_gdr3.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_j_aa_669_a104.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_rgbphotcal_gdr3.py M1
+                example: find_j_aa_669_a104.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
+		--noheader : ...
 		--DE_ICRS= : ...
 		--RA_ICRS= : ...
 		--GaiaDR3= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
@@ -115,15 +117,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("II/374/table2", params=params, filename=filename)
+        self.__client.query("J/A+A/669/A104/catalog", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -144,26 +146,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=rgbphotcal_gdr3"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=j_aa_669_a104"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -178,14 +181,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -218,23 +224,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','DE_ICRS=','RA_ICRS=','GaiaDR3=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','DE_ICRS=','RA_ICRS=','GaiaDR3=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -263,14 +270,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -298,27 +308,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_sage.py` & `cdsclient-1.1.9/cdsclient/find_xpm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,48 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query II/305/catalog
+   Query I/319/xpm
 
-   find_sage.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_xpm.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_sage.py M1
+                example: find_xpm.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--SSTISAGEMC= : ...
+		--noheader : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
+		--Fmag= : ...
+		--Bjmag= : ...
+		--Vmag= : ...
+		--Nmag= : ...
 		--Jmag= : ...
 		--Hmag= : ...
 		--Kmag= : ...
+		--Bmag= : ...
+		--Rmag= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --SSTISAGEMC=">10"
+     Example: --RAJ2000=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -118,15 +125,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("II/305/catalog", params=params, filename=filename)
+        self.__client.query("I/319/xpm", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -147,26 +154,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=SAGE"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=XPM"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -181,14 +189,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -221,23 +232,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','SSTISAGEMC=','RAJ2000=','DEJ2000=','Jmag=','Hmag=','Kmag=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','RAJ2000=','DEJ2000=','Fmag=','Bjmag=','Vmag=','Nmag=','Jmag=','Hmag=','Kmag=','Bmag=','Rmag=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -266,14 +278,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -301,27 +316,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_sage_arch.py` & `cdsclient-1.1.9/cdsclient/find_tic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query II/305/archive
+   Query IV/38/tic
 
-   find_sage_arch.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_tic.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_sage_arch.py M1
+                example: find_tic.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--SSTISAGEMA= : ...
+		--noheader : ...
+		--GAIA= : ...
+		--RAOdeg= : ...
+		--TIC= : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
-		--Jmag= : ...
-		--Hmag= : ...
-		--Kmag= : ...
+		--Tmag= : ...
+		--DEOdeg= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --SSTISAGEMA=">10"
+     Example: --GAIA=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -118,15 +121,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("II/305/archive", params=params, filename=filename)
+        self.__client.query("IV/38/tic", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -147,26 +150,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=SAGE_ARCH"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=TIC"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -181,14 +185,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -221,23 +228,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','SSTISAGEMA=','RAJ2000=','DEJ2000=','Jmag=','Hmag=','Kmag=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','GAIA=','RAOdeg=','TIC=','RAJ2000=','DEJ2000=','Tmag=','DEOdeg=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -266,14 +274,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -301,27 +312,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_sdss8.py` & `cdsclient-1.1.9/cdsclient/find_glimpse.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query II/306/sdss8
+   Query II/293/glimpse
 
-   find_sdss8.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_glimpse.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_sdss8.py M1
+                example: find_glimpse.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--SDSS8= : ...
-		--RA_ICRS= : ...
-		--DE_ICRS= : ...
-		--umag= : ...
-		--gmag= : ...
-		--rmag= : ...
-		--imag= : ...
-		--zmag= : ...
+		--noheader : ...
+		--GLIMPSE= : ...
+		--RAJ2000= : ...
+		--DEJ2000= : ...
+		--Jmag= : ...
+		--Hmag= : ...
+		--Kmag= : ...
 
 
-     Example: --SDSS8=">10"
+     Example: --GLIMPSE=">10"
 
      Licensed under a BSD license - see LICENSE.txt for details
 
 """
 
 import os, sys
 import getopt
@@ -111,15 +111,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("II/306/sdss8", params=params, filename=filename)
+        self.__client.query("II/293/glimpse", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -132,23 +132,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','SDSS8=','RA_ICRS=','DE_ICRS=','umag=','gmag=','rmag=','imag=','zmag=')
+    __options = ('help','format=','sort','add=','file=','noheader','GLIMPSE=','RAJ2000=','DEJ2000=','Jmag=','Hmag=','Kmag=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -177,14 +178,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -212,27 +216,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_sdss9.py` & `cdsclient-1.1.9/cdsclient/find_sdss9.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,25 +5,27 @@
    find_sdss9.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
                 example: find_sdss9.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
+		--noheader : ...
 		--SDSS9= : ...
 		--SDSS-ID= : ...
 		--objID= : ...
 		--Sp-ID= : ...
 		--RA_ICRS= : ...
 		--DE_ICRS= : ...
 		--umag= : ...
@@ -135,23 +137,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','SDSS9=','SDSS-ID=','objID=','Sp-ID=','RA_ICRS=','DE_ICRS=','umag=','gmag=','rmag=','imag=','zmag=')
+    __options = ('help','format=','sort','add=','file=','noheader','SDSS9=','SDSS-ID=','objID=','Sp-ID=','RA_ICRS=','DE_ICRS=','umag=','gmag=','rmag=','imag=','zmag=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -180,14 +183,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -215,27 +221,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_sdss_dr12.py` & `cdsclient-1.1.9/cdsclient/find_gaia2_dist.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,50 +1,38 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query V/147/sdss12
+   Query I/347/gaia2dis
 
-   find_sdss_dr12.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_gaia2_dist.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_sdss_dr12.py M1
+                example: find_gaia2_dist.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--RA_ICRS= : ...
-		--DE_ICRS= : ...
-		--SDSS12= : ...
-		--SDSS-ID= : ...
-		--objID= : ...
-		--Sp-ID= : ...
-		--ObsDate= : ...
-		--umag= : ...
-		--gmag= : ...
-		--rmag= : ...
-		--imag= : ...
-		--zmag= : ...
-		--zsp= : ...
-		--zph= : ...
-		--rpmag= : ...
+		--noheader : ...
+		--Source= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --RA_ICRS=">10"
+     Example: --Source=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -127,15 +115,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("V/147/sdss12", params=params, filename=filename)
+        self.__client.query("I/347/gaia2dis", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -156,26 +144,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=SDSS-DR12"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=gaia2_dist"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -190,14 +179,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -230,23 +222,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','RA_ICRS=','DE_ICRS=','SDSS12=','SDSS-ID=','objID=','Sp-ID=','ObsDate=','umag=','gmag=','rmag=','imag=','zmag=','zsp=','zph=','rpmag=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','Source=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -275,14 +268,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -310,27 +306,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_sdss_dr16.py` & `cdsclient-1.1.9/cdsclient/find_vmc_cat_dr4.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,50 +1,46 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query V/154/sdss16
+   Query II/351/vmc_dr4
 
-   find_sdss_dr16.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_vmc_cat_dr4.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_sdss_dr16.py M1
+                example: find_vmc_cat_dr4.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--objID= : ...
-		--RA_ICRS= : ...
-		--DE_ICRS= : ...
-		--upmag= : ...
-		--SpObjID= : ...
-		--umag= : ...
-		--gmag= : ...
-		--rmag= : ...
-		--imag= : ...
-		--zmag= : ...
-		--zsp= : ...
-		--zph= : ...
-		--SDSS16= : ...
-		--SDSS-ID= : ...
-		--Sp-ID= : ...
+		--noheader : ...
+		--SrcID= : ...
+		--RAJ2000= : ...
+		--DEJ2000= : ...
+		--KsMJD= : ...
+		--Kspmag= : ...
+		--JMJD= : ...
+		--Jpmag= : ...
+		--YMJD= : ...
+		--Ypmag= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --objID=">10"
+     Example: --SrcID=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -127,15 +123,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("V/154/sdss16", params=params, filename=filename)
+        self.__client.query("II/351/vmc_dr4", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -156,26 +152,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=SDSS_DR16"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=VMC_CAT_DR4"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -190,14 +187,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -230,23 +230,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','objID=','RA_ICRS=','DE_ICRS=','upmag=','SpObjID=','umag=','gmag=','rmag=','imag=','zmag=','zsp=','zph=','SDSS16=','SDSS-ID=','Sp-ID=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','SrcID=','RAJ2000=','DEJ2000=','KsMJD=','Kspmag=','JMJD=','Jpmag=','YMJD=','Ypmag=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -275,14 +276,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -310,27 +314,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_seip_srclist_phot_dr4.py` & `cdsclient-1.1.9/cdsclient/find_viking_dr2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query II/368/sstsl2
+   Query II/343/viking2
 
-   find_seip_srclist_phot_dr4.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_viking_dr2.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_seip_srclist_phot_dr4.py M1
+                example: find_viking_dr2.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
+		--noheader : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
 		--Name= : ...
+		--Zpmag= : ...
+		--Ypmag= : ...
+		--Jpmag= : ...
+		--Hpmag= : ...
+		--Kspmag= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
      Example: --RAJ2000=">10"
 
@@ -115,15 +122,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("II/368/sstsl2", params=params, filename=filename)
+        self.__client.query("II/343/viking2", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -144,26 +151,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=seip_srclist_phot_dr4"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=VIKING_DR2"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -178,14 +186,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -218,23 +229,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','RAJ2000=','DEJ2000=','Name=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','RAJ2000=','DEJ2000=','Name=','Zpmag=','Ypmag=','Jpmag=','Hpmag=','Kspmag=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -263,14 +275,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -298,27 +313,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_skymapper_dr11.py` & `cdsclient-1.1.9/cdsclient/find_gaia_dr3_varisum.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query II/358/smss
+   Query I/358/varisum
 
-   find_skymapper_dr11.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_gaia_dr3_varisum.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_skymapper_dr11.py M1
+                example: find_gaia_dr3_varisum.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--ObjectId= : ...
-		--SMSS= : ...
+		--noheader : ...
+		--Source= : ...
+		--RA_ICRS= : ...
+		--DE_ICRS= : ...
+		--TimeG= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --ObjectId=">10"
+     Example: --Source=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -114,15 +118,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("II/358/smss", params=params, filename=filename)
+        self.__client.query("I/358/varisum", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -143,26 +147,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=SKYMAPPER_DR11"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=gaia_dr3_varisum"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -177,14 +182,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -217,23 +225,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','ObjectId=','SMSS=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','Source=','RA_ICRS=','DE_ICRS=','TimeG=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -262,14 +271,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -297,27 +309,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_skymapper_dr4.py` & `cdsclient-1.1.9/cdsclient/find_allwise_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query II/379/smssdr4
+   Query II/328/allwise
 
-   find_skymapper_dr4.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_allwise_v2.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_skymapper_dr4.py M1
+                example: find_allwise_v2.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--DEICRS= : ...
-		--ObjectId= : ...
-		--RAICRS= : ...
-		--SMSS= : ...
+		--noheader : ...
+		--AllWISE= : ...
+		--RAJ2000= : ...
+		--DEJ2000= : ...
+		--Jmag= : ...
+		--Hmag= : ...
+		--Kmag= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --DEICRS=">10"
+     Example: --AllWISE=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -116,15 +120,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("II/379/smssdr4", params=params, filename=filename)
+        self.__client.query("II/328/allwise", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -145,26 +149,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=skymapper_dr4"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=allwise.v2"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -179,14 +184,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -219,23 +227,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','DEICRS=','ObjectId=','RAICRS=','SMSS=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','AllWISE=','RAJ2000=','DEJ2000=','Jmag=','Hmag=','Kmag=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -264,14 +273,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -299,27 +311,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_spm4.py` & `cdsclient-1.1.9/cdsclient/find_spm4.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,25 +5,27 @@
    find_spm4.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
                 example: find_spm4.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
+		--noheader : ...
 		--SPMID= : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
 		--Bmag= : ...
 		--Vmag= : ...
 		--Jmag= : ...
 		--Hmag= : ...
@@ -132,23 +134,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','SPMID=','RAJ2000=','DEJ2000=','Bmag=','Vmag=','Jmag=','Hmag=','Kmag=')
+    __options = ('help','format=','sort','add=','file=','noheader','SPMID=','RAJ2000=','DEJ2000=','Bmag=','Vmag=','Jmag=','Hmag=','Kmag=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -177,14 +180,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -212,27 +218,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_starhorse.py` & `cdsclient-1.1.9/cdsclient/find_starhorse.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,25 +5,27 @@
    find_starhorse.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
                 example: find_starhorse.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
+		--noheader : ...
 		--DE_ICRS= : ...
 		--Source= : ...
 		--RA_ICRS= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
@@ -144,14 +146,15 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
@@ -178,14 +181,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -218,23 +224,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','DE_ICRS=','Source=','RA_ICRS=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','DE_ICRS=','Source=','RA_ICRS=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -263,14 +270,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -298,27 +308,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_starhorse2021.py` & `cdsclient-1.1.9/cdsclient/find_viking_dr1.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query I/354/starhorse2021
+   Query II/329/viking1
 
-   find_starhorse2021.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_viking_dr1.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_starhorse2021.py M1
+                example: find_viking_dr1.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--Source= : ...
-		--RA_ICRS= : ...
-		--DE_ICRS= : ...
+		--noheader : ...
+		--RAJ2000= : ...
+		--DEJ2000= : ...
+		--Name= : ...
+		--Zpmag= : ...
+		--Ypmag= : ...
+		--Jpmag= : ...
+		--Hpmag= : ...
+		--Kspmag= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --Source=">10"
+     Example: --RAJ2000=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -115,15 +122,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("I/354/starhorse2021", params=params, filename=filename)
+        self.__client.query("II/329/viking1", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -144,26 +151,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=starhorse2021"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=VIKING_DR1"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -178,14 +186,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -218,23 +229,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','Source=','RA_ICRS=','DE_ICRS=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','RAJ2000=','DEJ2000=','Name=','Zpmag=','Ypmag=','Jpmag=','Hpmag=','Kspmag=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -263,14 +275,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -298,27 +313,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_tic.py` & `cdsclient-1.1.9/cdsclient/find_ukidss_dr8_gcs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query IV/38/tic
+   Query II/314/gcs8
 
-   find_tic.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_ukidss_dr8_gcs.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_tic.py M1
+                example: find_ukidss_dr8_gcs.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--GAIA= : ...
-		--RAOdeg= : ...
-		--TIC= : ...
+		--noheader : ...
+		--UGCS= : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
-		--Tmag= : ...
-		--DEOdeg= : ...
+		--Zmag= : ...
+		--Ymag= : ...
+		--Jmag= : ...
+		--Hmag= : ...
+		--Kmag= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --GAIA=">10"
+     Example: --UGCS=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -119,15 +122,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("IV/38/tic", params=params, filename=filename)
+        self.__client.query("II/314/gcs8", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -148,26 +151,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=TIC"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=ukidss_dr8_gcs"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -182,14 +186,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -222,23 +229,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','GAIA=','RAOdeg=','TIC=','RAJ2000=','DEJ2000=','Tmag=','DEOdeg=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','UGCS=','RAJ2000=','DEJ2000=','Zmag=','Ymag=','Jmag=','Hmag=','Kmag=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -267,14 +275,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -302,27 +313,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_tic82.py` & `cdsclient-1.1.9/cdsclient/find_tic82.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,25 +5,27 @@
    find_tic82.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
                 example: find_tic82.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
+		--noheader : ...
 		--Tmag= : ...
 		--DEJ2000= : ...
 		--HIP= : ...
 		--TIC= : ...
 		--RAJ2000= : ...
 		--GAIA= : ...
 		--KIC= : ...
@@ -150,14 +152,15 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
@@ -184,14 +187,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -224,23 +230,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','Tmag=','DEJ2000=','HIP=','TIC=','RAJ2000=','GAIA=','KIC=','DEOdeg=','RAOdeg=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','Tmag=','DEJ2000=','HIP=','TIC=','RAJ2000=','GAIA=','KIC=','DEOdeg=','RAOdeg=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -269,14 +276,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -304,27 +314,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_ucac3.py` & `cdsclient-1.1.9/cdsclient/find_usnob1.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query I/315/out
+   Query I/284/out
 
-   find_ucac3.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_usnob1.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_ucac3.py M1
+                example: find_usnob1.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--3UC= : ...
+		--noheader : ...
+		--USNO-B1.0= : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
-		--Jmag= : ...
-		--Kmag= : ...
+		--B1mag= : ...
+		--R1mag= : ...
+		--B2mag= : ...
+		--R2mag= : ...
+		--Imag= : ...
 
 
-     Example: --3UC=">10"
+     Example: --USNO-B1.0=">10"
 
      Licensed under a BSD license - see LICENSE.txt for details
 
 """
 
 import os, sys
 import getopt
@@ -108,15 +113,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("I/315/out", params=params, filename=filename)
+        self.__client.query("I/284/out", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -129,23 +134,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','3UC=','RAJ2000=','DEJ2000=','Jmag=','Kmag=')
+    __options = ('help','format=','sort','add=','file=','noheader','USNO-B1.0=','RAJ2000=','DEJ2000=','B1mag=','R1mag=','B2mag=','R2mag=','Imag=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -174,14 +180,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -209,27 +218,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_ucac4.py` & `cdsclient-1.1.9/cdsclient/find_ucac4.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,25 +5,27 @@
    find_ucac4.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
                 example: find_ucac4.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
+		--noheader : ...
 		--UCAC4= : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
 		--Jmag= : ...
 		--Hmag= : ...
 		--Kmag= : ...
 		--Bmag= : ...
@@ -132,23 +134,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','UCAC4=','RAJ2000=','DEJ2000=','Jmag=','Hmag=','Kmag=','Bmag=','Vmag=')
+    __options = ('help','format=','sort','add=','file=','noheader','UCAC4=','RAJ2000=','DEJ2000=','Jmag=','Hmag=','Kmag=','Bmag=','Vmag=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -177,14 +180,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -212,27 +218,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_ucac5.py` & `cdsclient-1.1.9/cdsclient/find_erass1_simu_agnin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query I/340/ucac5
+   Query J/A+A/665/A78/agnin
 
-   find_ucac5.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_erass1_simu_agnin.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_ucac5.py M1
+                example: find_erass1_simu_agnin.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
+		--noheader : ...
+		--SRCID= : ...
+		--DEJ2000= : ...
+		--RAJ2000= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: 
+     Example: --SRCID=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -112,15 +117,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("I/340/ucac5", params=params, filename=filename)
+        self.__client.query("J/A+A/665/A78/agnin", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -141,26 +146,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=UCAC5"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=erass1_simu_agnin"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -175,14 +181,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -215,23 +224,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','SRCID=','DEJ2000=','RAJ2000=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -260,14 +270,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -295,27 +308,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_ukidss_dr6_gps.py` & `cdsclient-1.1.9/cdsclient/find_apop.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query II/316/gps6
+   Query I/331/apop
 
-   find_ukidss_dr6_gps.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_apop.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_ukidss_dr6_gps.py M1
+                example: find_apop.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--UGPS= : ...
-		--RAICRS= : ...
-		--DEICRS= : ...
+		--noheader : ...
+		--Rmag= : ...
+		--Bmag= : ...
+		--Nmag= : ...
+		--Vmag= : ...
 		--Jmag= : ...
 		--Hmag= : ...
-		--Kmag1= : ...
-		--Kmag2= : ...
+		--Kmag= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --UGPS=">10"
+     Example: --Rmag=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -119,15 +121,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("II/316/gps6", params=params, filename=filename)
+        self.__client.query("I/331/apop", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -148,26 +150,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=ukidss_dr6_gps"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=APOP"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -182,14 +185,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -222,23 +228,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','UGPS=','RAICRS=','DEICRS=','Jmag=','Hmag=','Kmag1=','Kmag2=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','Rmag=','Bmag=','Nmag=','Vmag=','Jmag=','Hmag=','Kmag=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -267,14 +274,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -302,27 +312,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_ukidss_dr7_las.py` & `cdsclient-1.1.9/cdsclient/find_vvv_dr1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query II/310/las
+   Query II/337/vvv1
 
-   find_ukidss_dr7_las.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_vvv_dr1.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_ukidss_dr7_las.py M1
+                example: find_vvv_dr1.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
+		--noheader : ...
+		--srcid= : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
-		--Ymag= : ...
-		--Jmag= : ...
-		--Hmag= : ...
-		--Kmag= : ...
+		--Ymag3= : ...
+		--Jmag3= : ...
+		--Hmag3= : ...
+		--Ksmag3= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --RAJ2000=">10"
+     Example: --srcid=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -118,15 +121,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("II/310/las", params=params, filename=filename)
+        self.__client.query("II/337/vvv1", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -147,26 +150,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=UKIDSS_DR7_LAS"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=VVV_DR1"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -181,14 +185,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -221,23 +228,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','RAJ2000=','DEJ2000=','Ymag=','Jmag=','Hmag=','Kmag=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','srcid=','RAJ2000=','DEJ2000=','Ymag3=','Jmag3=','Hmag3=','Ksmag3=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -266,14 +274,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -301,27 +312,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_ukidss_dr8_dxs.py` & `cdsclient-1.1.9/cdsclient/find_vmc_dr6.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,46 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query II/314/dxs8
+   Query II/375/vmc_dr6
 
-   find_ukidss_dr8_dxs.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_vmc_dr6.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_ukidss_dr8_dxs.py M1
+                example: find_vmc_dr6.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--UDXS= : ...
+		--noheader : ...
+		--KsMJD= : ...
+		--JMJD= : ...
+		--YMJD= : ...
+		--SrcID= : ...
+		--Jpmag= : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
-		--Jmag= : ...
-		--Kmag= : ...
+		--Kspmag= : ...
+		--Ypmag= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --UDXS=">10"
+     Example: --KsMJD=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -117,15 +123,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("II/314/dxs8", params=params, filename=filename)
+        self.__client.query("II/375/vmc_dr6", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -146,26 +152,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=ukidss_dr8_dxs"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=vmc_dr6"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -180,14 +187,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -220,23 +230,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','UDXS=','RAJ2000=','DEJ2000=','Jmag=','Kmag=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','KsMJD=','JMJD=','YMJD=','SrcID=','Jpmag=','RAJ2000=','DEJ2000=','Kspmag=','Ypmag=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -265,14 +276,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -300,27 +314,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_ukidss_dr8_gcs.py` & `cdsclient-1.1.9/cdsclient/find_vhs_dr5.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query II/314/gcs8
+   Query II/367/vhs_dr5
 
-   find_ukidss_dr8_gcs.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_vhs_dr5.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_ukidss_dr8_gcs.py M1
+                example: find_vhs_dr5.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--UGCS= : ...
+		--noheader : ...
+		--SrcID= : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
-		--Zmag= : ...
-		--Ymag= : ...
-		--Jmag= : ...
-		--Hmag= : ...
-		--Kmag= : ...
+		--YMJD= : ...
+		--Ypmag= : ...
+		--Jpmag= : ...
+		--Hpmag= : ...
+		--Kspmag= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --UGCS=">10"
+     Example: --SrcID=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -120,15 +122,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("II/314/gcs8", params=params, filename=filename)
+        self.__client.query("II/367/vhs_dr5", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -149,26 +151,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=ukidss_dr8_gcs"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=vhs_dr5"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -183,14 +186,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -223,23 +229,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','UGCS=','RAJ2000=','DEJ2000=','Zmag=','Ymag=','Jmag=','Hmag=','Kmag=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','SrcID=','RAJ2000=','DEJ2000=','YMJD=','Ypmag=','Jpmag=','Hpmag=','Kspmag=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -268,14 +275,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -303,27 +313,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_ukidss_dr8_las.py` & `cdsclient-1.1.9/cdsclient/find_urat1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query II/314/las8
+   Query I/329/urat1
 
-   find_ukidss_dr8_las.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_urat1.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_ukidss_dr8_las.py M1
+                example: find_urat1.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--ULAS= : ...
+		--noheader : ...
+		--URAT1= : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
-		--Ymag= : ...
 		--Jmag= : ...
 		--Hmag= : ...
 		--Kmag= : ...
+		--Bmag= : ...
+		--Vmag= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --ULAS=">10"
+     Example: --URAT1=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -119,15 +122,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("II/314/las8", params=params, filename=filename)
+        self.__client.query("I/329/urat1", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -148,26 +151,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=ukidss_dr8_las"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=URAT1"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -182,14 +186,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -222,23 +229,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','ULAS=','RAJ2000=','DEJ2000=','Ymag=','Jmag=','Hmag=','Kmag=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','URAT1=','RAJ2000=','DEJ2000=','Jmag=','Hmag=','Kmag=','Bmag=','Vmag=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -267,14 +275,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -302,27 +313,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_ukidss_dr9_dxs.py` & `cdsclient-1.1.9/cdsclient/find_hsc2_detailed.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query II/319/dxs9
+   Query II/342/hsc2
 
-   find_ukidss_dr9_dxs.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_hsc2_detailed.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_ukidss_dr9_dxs.py M1
+                example: find_hsc2_detailed.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--UDXS= : ...
+		--noheader : ...
+		--CatID= : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
-		--Jmag= : ...
-		--Kmag= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --UDXS=">10"
+     Example: --CatID=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -117,15 +117,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("II/319/dxs9", params=params, filename=filename)
+        self.__client.query("II/342/hsc2", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -146,26 +146,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=ukidss_dr9_dxs"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=HSC2_DETAILED"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -180,14 +181,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -220,23 +224,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','UDXS=','RAJ2000=','DEJ2000=','Jmag=','Kmag=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','CatID=','RAJ2000=','DEJ2000=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -265,14 +270,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -300,27 +308,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_ukidss_dr9_gcs.py` & `cdsclient-1.1.9/cdsclient/find_ukidss_dr9_gcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,25 +5,27 @@
    find_ukidss_dr9_gcs.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
                 example: find_ukidss_dr9_gcs.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
+		--noheader : ...
 		--UGCS= : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
 		--Zmag= : ...
 		--Ymag= : ...
 		--Jmag= : ...
 		--Hmag= : ...
@@ -150,14 +152,15 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
@@ -184,14 +187,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -224,23 +230,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','UGCS=','RAJ2000=','DEJ2000=','Zmag=','Ymag=','Jmag=','Hmag=','Kmag1=','Kmag2=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','UGCS=','RAJ2000=','DEJ2000=','Zmag=','Ymag=','Jmag=','Hmag=','Kmag1=','Kmag2=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -269,14 +276,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -304,27 +314,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_ukidss_dr9_las.py` & `cdsclient-1.1.9/cdsclient/find_gums10_smc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query II/319/las9
+   Query VI/137/gum_smc
 
-   find_ukidss_dr9_las.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_gums10_smc.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_ukidss_dr9_las.py M1
+                example: find_gums10_smc.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--ULAS= : ...
-		--RAJ2000= : ...
-		--DEJ2000= : ...
-		--Ymag= : ...
-		--Hmag= : ...
-		--Kmag= : ...
+		--noheader : ...
+		--Gmag= : ...
+		--GBmag= : ...
+		--GRmag= : ...
+		--Gsmag= : ...
+		--RAICRS= : ...
+		--DEICRS= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --ULAS=">10"
+     Example: --Gmag=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -118,15 +120,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("II/319/las9", params=params, filename=filename)
+        self.__client.query("VI/137/gum_smc", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -147,26 +149,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=ukidss_dr9_las"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=gums10_smc"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -181,14 +184,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -221,23 +227,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','ULAS=','RAJ2000=','DEJ2000=','Ymag=','Hmag=','Kmag=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','Gmag=','GBmag=','GRmag=','Gsmag=','RAICRS=','DEICRS=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -266,14 +273,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -301,27 +311,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_unwise.py` & `cdsclient-1.1.9/cdsclient/find_gums10_mw.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query II/363/unwise
+   Query VI/137/gum_mw
 
-   find_unwise.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_gums10_mw.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_unwise.py M1
+                example: find_gums10_mw.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--objID= : ...
-		--RAJ2000= : ...
-		--DEJ2000= : ...
+		--noheader : ...
+		--Gmag= : ...
+		--GBmag= : ...
+		--GRmag= : ...
+		--Gsmag= : ...
+		--RAICRS= : ...
+		--DEICRS= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --objID=">10"
+     Example: --Gmag=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -115,15 +120,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("II/363/unwise", params=params, filename=filename)
+        self.__client.query("VI/137/gum_mw", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -144,26 +149,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=unwise"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=gums10_mw"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -178,14 +184,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -218,23 +227,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','objID=','RAJ2000=','DEJ2000=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','Gmag=','GBmag=','GRmag=','Gsmag=','RAICRS=','DEICRS=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -263,14 +273,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -298,27 +311,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_urat1.py` & `cdsclient-1.1.9/cdsclient/find_vhs_dr41.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query I/329/urat1
+   Query II/359/vhs_dr4
 
-   find_urat1.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_vhs_dr41.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_urat1.py M1
+                example: find_vhs_dr41.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--URAT1= : ...
+		--noheader : ...
+		--SrcID= : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
-		--Jmag= : ...
-		--Hmag= : ...
-		--Kmag= : ...
-		--Bmag= : ...
-		--Vmag= : ...
+		--Ypmag= : ...
+		--Jpmag= : ...
+		--Hpmag= : ...
+		--Kspmag= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --URAT1=">10"
+     Example: --SrcID=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -120,15 +121,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("I/329/urat1", params=params, filename=filename)
+        self.__client.query("II/359/vhs_dr4", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -149,26 +150,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=URAT1"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=vhs_dr41"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -183,14 +185,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -223,23 +228,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','URAT1=','RAJ2000=','DEJ2000=','Jmag=','Hmag=','Kmag=','Bmag=','Vmag=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','SrcID=','RAJ2000=','DEJ2000=','Ypmag=','Jpmag=','Hpmag=','Kspmag=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -268,14 +274,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -303,27 +312,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_usnob1.py` & `cdsclient-1.1.9/cdsclient/find_2mass.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query I/284/out
+   Query II/246/out
 
-   find_usnob1.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_2mass.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_usnob1.py M1
+                example: find_2mass.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--USNO-B1.0= : ...
+		--noheader : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
-		--B1mag= : ...
-		--R1mag= : ...
-		--B2mag= : ...
-		--R2mag= : ...
-		--Imag= : ...
+		--2MASS= : ...
+		--Jmag= : ...
+		--Hmag= : ...
+		--Kmag= : ...
 
 
-     Example: --USNO-B1.0=">10"
+     Example: --RAJ2000=">10"
 
      Licensed under a BSD license - see LICENSE.txt for details
 
 """
 
 import os, sys
 import getopt
@@ -111,15 +111,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("I/284/out", params=params, filename=filename)
+        self.__client.query("II/246/out", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -132,23 +132,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','USNO-B1.0=','RAJ2000=','DEJ2000=','B1mag=','R1mag=','B2mag=','R2mag=','Imag=')
+    __options = ('help','format=','sort','add=','file=','noheader','RAJ2000=','DEJ2000=','2MASS=','Jmag=','Hmag=','Kmag=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -177,14 +178,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -212,27 +216,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_vexasdes.py` & `cdsclient-1.1.9/cdsclient/find_apass9.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query II/369/vexasdes
+   Query II/336/apass9
 
-   find_vexasdes.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_apass9.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_vexasdes.py M1
+                example: find_apass9.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--VISTA= : ...
+		--noheader : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
+		--Vmag= : ...
+		--Bmag= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --VISTA=">10"
+     Example: --RAJ2000=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -115,15 +118,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("II/369/vexasdes", params=params, filename=filename)
+        self.__client.query("II/336/apass9", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -144,26 +147,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=vexasdes"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=APASS9"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -178,14 +182,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -218,23 +225,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','VISTA=','RAJ2000=','DEJ2000=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','RAJ2000=','DEJ2000=','Vmag=','Bmag=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -263,14 +271,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -298,27 +309,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_vexasps.py` & `cdsclient-1.1.9/cdsclient/find_sage.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query II/369/vexasps
+   Query II/305/catalog
 
-   find_vexasps.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_sage.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_vexasps.py M1
+                example: find_sage.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--VISTA= : ...
+		--noheader : ...
+		--SSTISAGEMC= : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
+		--Jmag= : ...
+		--Hmag= : ...
+		--Kmag= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --VISTA=">10"
+     Example: --SSTISAGEMC=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -115,15 +120,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("II/369/vexasps", params=params, filename=filename)
+        self.__client.query("II/305/catalog", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -144,26 +149,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=vexasps"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=SAGE"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -178,14 +184,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -218,23 +227,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','VISTA=','RAJ2000=','DEJ2000=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','SSTISAGEMC=','RAJ2000=','DEJ2000=','Jmag=','Hmag=','Kmag=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -263,14 +273,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -298,27 +311,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_vexassm.py` & `cdsclient-1.1.9/cdsclient/find_gaia_dr3_varispursign.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query II/369/vexassm
+   Query J/A+A/674/A25/vspursig
 
-   find_vexassm.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_gaia_dr3_varispursign.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_vexassm.py M1
+                example: find_gaia_dr3_varispursign.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--VISTA= : ...
-		--RAJ2000= : ...
-		--DEJ2000= : ...
+		--noheader : ...
+		--DE_ICRS= : ...
+		--Source= : ...
+		--RA_ICRS= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --VISTA=">10"
+     Example: --DE_ICRS=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -115,15 +117,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("II/369/vexassm", params=params, filename=filename)
+        self.__client.query("J/A+A/674/A25/vspursig", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -144,26 +146,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=vexassm"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=gaia_dr3_varispursign"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -178,14 +181,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -218,23 +224,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','VISTA=','RAJ2000=','DEJ2000=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','DE_ICRS=','Source=','RA_ICRS=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -263,14 +270,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -298,27 +308,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_vhs_dr41.py` & `cdsclient-1.1.9/cdsclient/find_starhorse2021.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,40 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query II/359/vhs_dr4
+   Query I/354/starhorse2021
 
-   find_vhs_dr41.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_starhorse2021.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_vhs_dr41.py M1
+                example: find_starhorse2021.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--SrcID= : ...
-		--RAJ2000= : ...
-		--DEJ2000= : ...
-		--Ypmag= : ...
-		--Jpmag= : ...
-		--Hpmag= : ...
-		--Kspmag= : ...
+		--noheader : ...
+		--Source= : ...
+		--RA_ICRS= : ...
+		--DE_ICRS= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --SrcID=">10"
+     Example: --Source=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -119,15 +117,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("II/359/vhs_dr4", params=params, filename=filename)
+        self.__client.query("I/354/starhorse2021", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -148,26 +146,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=vhs_dr41"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=starhorse2021"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -182,14 +181,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -222,23 +224,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','SrcID=','RAJ2000=','DEJ2000=','Ypmag=','Jpmag=','Hpmag=','Kspmag=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','Source=','RA_ICRS=','DE_ICRS=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -267,14 +270,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -302,27 +308,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_vhs_dr5.py` & `cdsclient-1.1.9/cdsclient/find_gums10_lmc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query II/367/vhs_dr5
+   Query VI/137/gum_lmc
 
-   find_vhs_dr5.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_gums10_lmc.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_vhs_dr5.py M1
+                example: find_gums10_lmc.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--SrcID= : ...
-		--RAJ2000= : ...
-		--DEJ2000= : ...
-		--YMJD= : ...
-		--Ypmag= : ...
-		--Jpmag= : ...
-		--Hpmag= : ...
-		--Kspmag= : ...
+		--noheader : ...
+		--Gmag= : ...
+		--GBmag= : ...
+		--GRmag= : ...
+		--Gsmag= : ...
+		--RAICRS= : ...
+		--DEICRS= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --SrcID=">10"
+     Example: --Gmag=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -120,15 +120,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("II/367/vhs_dr5", params=params, filename=filename)
+        self.__client.query("VI/137/gum_lmc", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -149,26 +149,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=vhs_dr5"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=gums10_lmc"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -183,14 +184,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -223,23 +227,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','SrcID=','RAJ2000=','DEJ2000=','YMJD=','Ypmag=','Jpmag=','Hpmag=','Kspmag=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','Gmag=','GBmag=','GRmag=','Gsmag=','RAICRS=','DEICRS=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -268,14 +273,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -303,27 +311,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_viking_dr1.py` & `cdsclient-1.1.9/cdsclient/find_sdss_dr16.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,52 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query II/329/viking1
+   Query V/154/sdss16
 
-   find_viking_dr1.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_sdss_dr16.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_viking_dr1.py M1
+                example: find_sdss_dr16.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--RAJ2000= : ...
-		--DEJ2000= : ...
-		--Name= : ...
-		--Zpmag= : ...
-		--Ypmag= : ...
-		--Jpmag= : ...
-		--Hpmag= : ...
-		--Kspmag= : ...
+		--noheader : ...
+		--objID= : ...
+		--RA_ICRS= : ...
+		--DE_ICRS= : ...
+		--upmag= : ...
+		--SpObjID= : ...
+		--umag= : ...
+		--gmag= : ...
+		--rmag= : ...
+		--imag= : ...
+		--zmag= : ...
+		--zsp= : ...
+		--zph= : ...
+		--SDSS16= : ...
+		--SDSS-ID= : ...
+		--Sp-ID= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --RAJ2000=">10"
+     Example: --objID=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -120,15 +129,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("II/329/viking1", params=params, filename=filename)
+        self.__client.query("V/154/sdss16", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -149,26 +158,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=VIKING_DR1"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=SDSS_DR16"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -183,14 +193,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -223,23 +236,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','RAJ2000=','DEJ2000=','Name=','Zpmag=','Ypmag=','Jpmag=','Hpmag=','Kspmag=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','objID=','RA_ICRS=','DE_ICRS=','upmag=','SpObjID=','umag=','gmag=','rmag=','imag=','zmag=','zsp=','zph=','SDSS16=','SDSS-ID=','Sp-ID=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -268,14 +282,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -303,27 +320,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_viking_dr2.py` & `cdsclient-1.1.9/cdsclient/find_sdss_dr12.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,52 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query II/343/viking2
+   Query V/147/sdss12
 
-   find_viking_dr2.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_sdss_dr12.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_viking_dr2.py M1
+                example: find_sdss_dr12.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--RAJ2000= : ...
-		--DEJ2000= : ...
-		--Name= : ...
-		--Zpmag= : ...
-		--Ypmag= : ...
-		--Jpmag= : ...
-		--Hpmag= : ...
-		--Kspmag= : ...
+		--noheader : ...
+		--RA_ICRS= : ...
+		--DE_ICRS= : ...
+		--SDSS12= : ...
+		--SDSS-ID= : ...
+		--objID= : ...
+		--Sp-ID= : ...
+		--ObsDate= : ...
+		--umag= : ...
+		--gmag= : ...
+		--rmag= : ...
+		--imag= : ...
+		--zmag= : ...
+		--zsp= : ...
+		--zph= : ...
+		--rpmag= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --RAJ2000=">10"
+     Example: --RA_ICRS=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -120,15 +129,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("II/343/viking2", params=params, filename=filename)
+        self.__client.query("V/147/sdss12", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -149,26 +158,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=VIKING_DR2"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=SDSS-DR12"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -183,14 +193,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -223,23 +236,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','RAJ2000=','DEJ2000=','Name=','Zpmag=','Ypmag=','Jpmag=','Hpmag=','Kspmag=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','RA_ICRS=','DE_ICRS=','SDSS12=','SDSS-ID=','objID=','Sp-ID=','ObsDate=','umag=','gmag=','rmag=','imag=','zmag=','zsp=','zph=','rpmag=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -268,14 +282,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -303,27 +320,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_vmc_cat_dr4.py` & `cdsclient-1.1.9/cdsclient/find_2mass6x.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query II/351/vmc_dr4
+   Query II/281/2mass6x
 
-   find_vmc_cat_dr4.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_2mass6x.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_vmc_cat_dr4.py M1
+                example: find_2mass6x.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--SrcID= : ...
+		--noheader : ...
+		--2MASS= : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
-		--KsMJD= : ...
-		--Kspmag= : ...
-		--JMJD= : ...
-		--Jpmag= : ...
-		--YMJD= : ...
-		--Ypmag= : ...
+		--Jmag= : ...
+		--Hmag= : ...
+		--Kmag= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --SrcID=">10"
+     Example: --2MASS=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -121,15 +120,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("II/351/vmc_dr4", params=params, filename=filename)
+        self.__client.query("II/281/2mass6x", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -150,26 +149,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=VMC_CAT_DR4"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=2MASS6X"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -184,14 +184,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -224,23 +227,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','SrcID=','RAJ2000=','DEJ2000=','KsMJD=','Kspmag=','JMJD=','Jpmag=','YMJD=','Ypmag=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','2MASS=','RAJ2000=','DEJ2000=','Jmag=','Hmag=','Kmag=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -269,14 +273,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -304,27 +311,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_vmc_dr6.py` & `cdsclient-1.1.9/cdsclient/find_gps1.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query II/375/vmc_dr6
+   Query I/343/gps1
 
-   find_vmc_dr6.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_gps1.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_vmc_dr6.py M1
+                example: find_gps1.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--KsMJD= : ...
-		--JMJD= : ...
-		--YMJD= : ...
-		--SrcID= : ...
-		--Jpmag= : ...
-		--RAJ2000= : ...
-		--DEJ2000= : ...
-		--Kspmag= : ...
-		--Ypmag= : ...
+		--noheader : ...
+		--pmRA= : ...
+		--pmDE= : ...
+		--gmag= : ...
+		--rmag= : ...
+		--imag= : ...
+		--zmag= : ...
+		--ymag= : ...
+		--Jmag= : ...
+		--Hmag= : ...
+		--Ksmag= : ...
+		--Gmag= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --KsMJD=">10"
+     Example: --pmRA=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -121,15 +125,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("II/375/vmc_dr6", params=params, filename=filename)
+        self.__client.query("I/343/gps1", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -150,26 +154,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=vmc_dr6"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=GPS1"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -184,14 +189,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -224,23 +232,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','KsMJD=','JMJD=','YMJD=','SrcID=','Jpmag=','RAJ2000=','DEJ2000=','Kspmag=','Ypmag=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','pmRA=','pmDE=','gmag=','rmag=','imag=','zmag=','ymag=','Jmag=','Hmag=','Ksmag=','Gmag=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -269,14 +278,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -304,27 +316,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_vphasplus_dr2.py` & `cdsclient-1.1.9/cdsclient/find_vvv_virac_pm_dr41.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query II/341/vphasp
+   Query II/364/virac
 
-   find_vphasplus_dr2.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_vvv_virac_pm_dr41.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_vphasplus_dr2.py M1
+                example: find_vvv_virac_pm_dr41.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--sourceID= : ...
-		--RAJ2000= : ...
-		--DEJ2000= : ...
-		--umag= : ...
-		--gmag= : ...
-		--rmag= : ...
-		--imag= : ...
+		--noheader : ...
+		--srcid= : ...
+		--RA_ICRS= : ...
+		--DE_ICRS= : ...
+		--Ksmag= : ...
+		--pmRA= : ...
+		--Zmag= : ...
+		--Ymag= : ...
+		--Jmag= : ...
+		--Hmag= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --sourceID=">10"
+     Example: --srcid=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -119,15 +123,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("II/341/vphasp", params=params, filename=filename)
+        self.__client.query("II/364/virac", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -148,26 +152,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=VPHASPLUS_DR2"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=vvv_virac_pm_dr41"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -182,14 +187,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -222,23 +230,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','sourceID=','RAJ2000=','DEJ2000=','umag=','gmag=','rmag=','imag=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','srcid=','RA_ICRS=','DE_ICRS=','Ksmag=','pmRA=','Zmag=','Ymag=','Jmag=','Hmag=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -267,14 +276,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -302,27 +314,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_vst_atlas_dr3.py` & `cdsclient-1.1.9/cdsclient/find_hsc1_detailed.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,40 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query II/350/vstatlas
+   Query II/342/hsc1
 
-   find_vst_atlas_dr3.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_hsc1_detailed.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_vst_atlas_dr3.py M1
+                example: find_hsc1_detailed.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--SrcID= : ...
+		--noheader : ...
+		--CatID= : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
-		--Uap3= : ...
-		--Rap3= : ...
-		--Iap3= : ...
-		--Zap3= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --SrcID=">10"
+     Example: --CatID=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -119,15 +117,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("II/350/vstatlas", params=params, filename=filename)
+        self.__client.query("II/342/hsc1", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -148,26 +146,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=VST_ATLAS_DR3"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=HSC1_DETAILED"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -182,14 +181,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -222,23 +224,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','SrcID=','RAJ2000=','DEJ2000=','Uap3=','Rap3=','Iap3=','Zap3=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','CatID=','RAJ2000=','DEJ2000=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -267,14 +270,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -302,27 +308,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_vvv_cat_dr2.py` & `cdsclient-1.1.9/cdsclient/find_skymapper_dr4.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query II/348/vvv2
+   Query II/379/smssdr4
 
-   find_vvv_cat_dr2.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_skymapper_dr4.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_vvv_cat_dr2.py M1
+                example: find_skymapper_dr4.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--srcid= : ...
-		--RAJ2000= : ...
-		--DEJ2000= : ...
-		--Ymag3= : ...
-		--Jmag3= : ...
-		--Hmag3= : ...
-		--Ksmag3= : ...
+		--noheader : ...
+		--DEICRS= : ...
+		--ObjectId= : ...
+		--RAICRS= : ...
+		--SMSS= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --srcid=">10"
+     Example: --DEICRS=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -119,15 +118,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("II/348/vvv2", params=params, filename=filename)
+        self.__client.query("II/379/smssdr4", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -148,26 +147,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=VVV_CAT_DR2"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=skymapper_dr4"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -182,14 +182,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -222,23 +225,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','srcid=','RAJ2000=','DEJ2000=','Ymag3=','Jmag3=','Hmag3=','Ksmag3=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','DEICRS=','ObjectId=','RAICRS=','SMSS=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -267,14 +271,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -302,27 +309,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_vvv_cat_dr4.py` & `cdsclient-1.1.9/cdsclient/find_igaps_dr1.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,48 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query II/376/vvv4
+   Query V/165/igapsdr1
 
-   find_vvv_cat_dr4.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_igaps_dr1.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_vvv_cat_dr4.py M1
+                example: find_igaps_dr1.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
+		--noheader : ...
+		--Name= : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
-		--SrcID= : ...
-		--Z1MJD= : ...
+		--SourceID= : ...
+		--imag= : ...
+		--MJDi= : ...
+		--Hamag= : ...
+		--rImag= : ...
+		--rUmag= : ...
+		--gmag= : ...
+		--Umag= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --RAJ2000=">10"
+     Example: --Name=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -116,15 +125,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("II/376/vvv4", params=params, filename=filename)
+        self.__client.query("V/165/igapsdr1", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -145,26 +154,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=vvv_cat_dr4"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=igaps_dr1"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -179,14 +189,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -219,23 +232,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','RAJ2000=','DEJ2000=','SrcID=','Z1MJD=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','Name=','RAJ2000=','DEJ2000=','SourceID=','imag=','MJDi=','Hamag=','rImag=','rUmag=','gmag=','Umag=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -264,14 +278,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -299,27 +316,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_vvv_dr1.py` & `cdsclient-1.1.9/cdsclient/find_sage_arch.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query II/337/vvv1
+   Query II/305/archive
 
-   find_vvv_dr1.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_sage_arch.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_vvv_dr1.py M1
+                example: find_sage_arch.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--srcid= : ...
+		--noheader : ...
+		--SSTISAGEMA= : ...
 		--RAJ2000= : ...
 		--DEJ2000= : ...
-		--Ymag3= : ...
-		--Jmag3= : ...
-		--Hmag3= : ...
-		--Ksmag3= : ...
+		--Jmag= : ...
+		--Hmag= : ...
+		--Kmag= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --srcid=">10"
+     Example: --SSTISAGEMA=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -119,15 +120,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("II/337/vvv1", params=params, filename=filename)
+        self.__client.query("II/305/archive", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -148,26 +149,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=VVV_DR1"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=SAGE_ARCH"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -182,14 +184,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -222,23 +227,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','srcid=','RAJ2000=','DEJ2000=','Ymag3=','Jmag3=','Hmag3=','Ksmag3=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','SSTISAGEMA=','RAJ2000=','DEJ2000=','Jmag=','Hmag=','Kmag=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -267,14 +273,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -302,27 +311,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_vvv_virac_pm_dr41.py` & `cdsclient-1.1.9/cdsclient/find_des_dr2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,51 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query II/364/virac
+   Query II/371/des_dr2
 
-   find_vvv_virac_pm_dr41.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_des_dr2.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_vvv_virac_pm_dr41.py M1
+                example: find_des_dr2.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--srcid= : ...
+		--noheader : ...
+		--DES= : ...
 		--RA_ICRS= : ...
 		--DE_ICRS= : ...
-		--Ksmag= : ...
-		--pmRA= : ...
-		--Zmag= : ...
+		--CoadID= : ...
+		--gFlag= : ...
+		--rFlag= : ...
+		--iFlag= : ...
+		--zFlag= : ...
+		--yFlag= : ...
+		--gmag= : ...
+		--rmag= : ...
+		--imag= : ...
+		--zmag= : ...
 		--Ymag= : ...
-		--Jmag= : ...
-		--Hmag= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --srcid=">10"
+     Example: --DES=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -121,15 +128,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("II/364/virac", params=params, filename=filename)
+        self.__client.query("II/371/des_dr2", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -150,26 +157,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=vvv_virac_pm_dr41"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=des_dr2"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -184,14 +192,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -224,23 +235,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','srcid=','RA_ICRS=','DE_ICRS=','Ksmag=','pmRA=','Zmag=','Ymag=','Jmag=','Hmag=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','DES=','RA_ICRS=','DE_ICRS=','CoadID=','gFlag=','rFlag=','iFlag=','zFlag=','yFlag=','gmag=','rmag=','imag=','zmag=','Ymag=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -269,14 +281,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -304,27 +319,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_wise_allsky.py` & `cdsclient-1.1.9/cdsclient/find_ukidss_dr6_gps.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query II/311/wise
+   Query II/316/gps6
 
-   find_wise_allsky.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_ukidss_dr6_gps.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_wise_allsky.py M1
+                example: find_ukidss_dr6_gps.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--WISE= : ...
-		--RAJ2000= : ...
-		--DEJ2000= : ...
+		--noheader : ...
+		--UGPS= : ...
+		--RAICRS= : ...
+		--DEICRS= : ...
 		--Jmag= : ...
 		--Hmag= : ...
-		--Kmag= : ...
+		--Kmag1= : ...
+		--Kmag2= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --WISE=">10"
+     Example: --UGPS=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -118,15 +121,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("II/311/wise", params=params, filename=filename)
+        self.__client.query("II/316/gps6", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -147,26 +150,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=WISE_ALLSKY"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=ukidss_dr6_gps"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -181,14 +185,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -221,23 +228,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','WISE=','RAJ2000=','DEJ2000=','Jmag=','Hmag=','Kmag=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','UGPS=','RAICRS=','DEICRS=','Jmag=','Hmag=','Kmag1=','Kmag2=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -266,14 +274,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -301,27 +312,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/find_xpm.py` & `cdsclient-1.1.9/cdsclient/find_catwise2020.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,45 @@
 #!/usr/bin/env python
 """G.Landais (CDS) 24-mar-2018
-   Query I/319/xpm
+   Query II/365/catwise
 
-   find_xpm.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
+   find_catwise2020.py [-h] [-a] [-r radius] [-m max] [constraints] [--format=tsv|votable|ascii] [position]
             [--ipix=order:num] [--no-format] [--offset=begin...nb_occurences]
      -a: display all columns
      -r: radius in arcsec
      -m: max number of lines in output
      -h: this help
      --format: output (--format=tsv|votable|ascii)
+   --noheader: remove header (not available for all options)
      --sort  : sort by distance (available with position only)
      --add   : column name in output
      --file  : query with a list
 
      position : ra dec position or target name
-                example: find_xpm.py M1
+                example: find_catwise2020.py M1
 
      Other constraints:
 		--sort : ...
 		--add= : ...
 		--file= : ...
-		--RAJ2000= : ...
-		--DEJ2000= : ...
-		--Fmag= : ...
-		--Bjmag= : ...
-		--Vmag= : ...
-		--Nmag= : ...
-		--Jmag= : ...
-		--Hmag= : ...
-		--Kmag= : ...
-		--Bmag= : ...
-		--Rmag= : ...
+		--noheader : ...
+		--objID= : ...
+		--RA_ICRS= : ...
+		--DE_ICRS= : ...
+		--Name= : ...
+		--MJD= : ...
+		--W1mproPM= : ...
+		--W2mproPM= : ...
+		--Dist= : ...
 		--ipix= : ...
 		--no-format : ...
 		--offset= : ...
 
 
-     Example: --RAJ2000=">10"
+     Example: --objID=">10"
 
 Note: ouput&capabilites are specific to the options
 
 use --no-format to get original precision
 (only available with position or ipix constraint)
 
 
@@ -123,15 +122,15 @@
 
             if file_col is not None:
                 params.append("-sort={0}".format(file_col))
             else:
                 params.append("-out.add=_r")
                 params.append("-sort=_r")
 
-        self.__client.query("I/319/xpm", params=params, filename=filename)
+        self.__client.query("II/365/catwise", params=params, filename=filename)
 
         if self.format is not None:
             self.__client.format = self.format
 
     def get(self):
         return self.__client.get()
 
@@ -152,26 +151,27 @@
         """
         QueryCat.__init__(self)
         self.__url = None
         self.__ipix = None
         self.__offset = None
         self.limit = vizquery.DEFAULT_LIMIT
         self.noformat = False
+        self.noheader = False
 
     def set_healpix(self, ipix):
         self.__ipix  = ipix
 
     def set_offset(self, begin, end):
         self.__offset = "{}..{}".format(begin, end)
 
     def query_cat(self, constraints=None, all=False, limit=vizquery.DEFAULT_LIMIT, columns=None, filename=None):
         if filename is not None:
             raise Exception("file upload is not available")
 
-        self.__url = VIZIER_BIG_CAT_URL + "?-source=XPM"
+        self.__url = VIZIER_BIG_CAT_URL + "?-source=catwise2020"
         self.__url += "&-c.rs=" + str(self.radius)
 
         if self.position:
             self.__url += "&-c="+quote(self.position)
 
         elif self.__ipix is not None:
             self.__url += "&--ipix="+self.__ipix
@@ -186,14 +186,17 @@
             self.__url += "&-out.max=" + str(self.limit)
 
         if self.noformat is True:
             self.__url += "&--noformat=true"
             if self.format not in (vizquery.FORMAT_TSV, vizquery.FORMAT_VOTABLE):
                 self.format = vizquery.FORMAT_TSV
 
+        if self.noheader is True:
+            self.__url += "&--noheader=true"
+
         if self.format is None:
             self.__url += "&--format="+vizquery.FORMAT_TSV
 
         else:
             self.__url += "&--format="+self.format
 
         if columns is not None:
@@ -226,23 +229,24 @@
 if __name__ == "__main__":
 
     __radius = vizquery.DEFAULT_RADIUS
     __position = None
     __limit = None
     __mime = vizquery.FORMAT_ASCII
     __noformat = False
+    __noheader = False
     __ipix = None
     __all = False
     __sort = False
     __add = None
     __filename = None
     __constraints = []
     __offset = None
 
-    __options = ('help','format=','sort','add=','file=','RAJ2000=','DEJ2000=','Fmag=','Bjmag=','Vmag=','Nmag=','Jmag=','Hmag=','Kmag=','Bmag=','Rmag=','ipix=','no-format','offset=')
+    __options = ('help','format=','sort','add=','file=','noheader','objID=','RA_ICRS=','DE_ICRS=','Name=','MJD=','W1mproPM=','W2mproPM=','Dist=','ipix=','no-format','offset=')
     try :
         __opts, __args = getopt.getopt(sys.argv[1:], 'hvar:m:f:', __options)
     except:
         help("__main__")
         sys.exit(1)
 
     for __o, __a in __opts:
@@ -271,14 +275,17 @@
 
         elif __o == "--format":
             __mime = __a
 
         elif __o == "--no-format":
             __noformat = True
 
+        elif __o == "--noheader":
+            __noheader = True
+
         elif __o == "--ipix":
             __ipix = __a
 
         elif __o == "--count":
             __count = True
 
         elif __o == "--sort":
@@ -306,27 +313,28 @@
 
     for __arg in __args:
         if __position is None:
             __position = __arg
         else:
             __position += " "+ __arg
 
-    if __noformat is True or __ipix is not None or __offset is not None:
+    if __noformat is True or __ipix is not None or __offset is not None or __noheader:
         if __sort is True :
             raise Exception("--sort function is not compatible with --ipix/--no-format")
         if __filename is not None:
             raise Exception("--file option is not compatible with --ipix/--no-format")
 
         if len(__constraints)>0:
             raise Exception("Constraints "+str(__constraints)+" is not available in this mode (--ipix/--offset/--no-format)")
 
         __querycat = QueryCatClient()
         if __ipix is not None:
             __querycat.set_healpix(__ipix)
         __querycat.noformat=__noformat
+        __querycat.noheader=__noheader
 
         if __offset :
             s = __offset.split("..")
             if len(s) != 2: raise Exception("error offset syntax: min..max")
             try:
                 __querycat.set_offset(int(s[0]), int(s[1]))
             except:
```

### Comparing `cdsclient-1.1.8/cdsclient/vizquery.py` & `cdsclient-1.1.9/cdsclient/vizquery.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 else:
     import urllib.request as ulib
 
 DEFAULT_RADIUS = 2. # arcsec
 DEFAULT_LIMIT = 100
 DEBUG = True
 VIZIER_URL = "https://vizier.cds.unistra.fr/viz-bin/"
-TAPVIZIER = "http://tapvizier.cds.unistra.fr/TAPVizieR/"
+TAPVIZIER = "https://tapvizier.cds.unistra.fr/TAPVizieR/"
 
 
 FORMAT_TSV = "tsv"
 FORMAT_VOTABLE = "votable"
 FORMAT_ASCII = "ascii"
```

### Comparing `cdsclient-1.1.8/README.md` & `cdsclient-1.1.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 ## CDS Python package to query large catalogues
 
 **Note**: API import changed in the last version - see example below
 
 **License** : BSD License
 
 **Installation** : 
-python3 setup.py install --user
+```
+git clone https://github.com/cds-astro/cds.cdsclient.git
+cd cds.cdsclient
+pip install .
+```
 
 **vizquery.py** : the vizquery package
               query all VizieR catalogues using ASU parameters
               metadata retrieving: get columns/table information 
 				   and list large tables
 
 **Examples** :
```

### Comparing `cdsclient-1.1.8/pyproject.toml` & `cdsclient-1.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 repository = "https://github.com/cds-astro/cds.cdsclient"
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.hatch.version]
-path = "cdsclient/__init__.py"
+path = "__init__.py"
```

### Comparing `cdsclient-1.1.8/PKG-INFO` & `cdsclient-1.1.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cdsclient
-Version: 1.1.8
+Version: 1.1.9
 Summary: CDS VizieR client (query large table)
 Project-URL: repository, https://github.com/cds-astro/cds.cdsclient
 Author: Gilles Landais (CDS)
 Keywords: astronomy
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -18,15 +18,19 @@
 ## CDS Python package to query large catalogues
 
 **Note**: API import changed in the last version - see example below
 
 **License** : BSD License
 
 **Installation** : 
-python3 setup.py install --user
+```
+git clone https://github.com/cds-astro/cds.cdsclient.git
+cd cds.cdsclient
+pip install .
+```
 
 **vizquery.py** : the vizquery package
               query all VizieR catalogues using ASU parameters
               metadata retrieving: get columns/table information 
 				   and list large tables
 
 **Examples** :
```

