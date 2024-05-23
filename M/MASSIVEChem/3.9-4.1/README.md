# Comparing `tmp/massivechem-3.9.tar.gz` & `tmp/massivechem-4.1.tar.gz`

## Comparing `massivechem-3.9.tar` & `massivechem-4.1.tar`

### file list

```diff
@@ -1,143 +1,87 @@
--rw-r--r--   0        0        0   219083 2020-02-02 00:00:00.000000 massivechem-3.9/IMG_2856.jpg
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 massivechem-3.9/molecule_image.png
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 massivechem-3.9/project_CH200.yml
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 massivechem-3.9/project_final.yml
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 massivechem-3.9/.idea/modules.xml
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 massivechem-3.9/.idea/ppchem-project-Christiansson-Gonteri-Humery.iml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 massivechem-3.9/.idea/vcs.xml
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 massivechem-3.9/.idea/workspace.xml
--rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 massivechem-3.9/.idea/input/input.html
--rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 massivechem-3.9/.idea/input/input.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 massivechem-3.9/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0    35964 2020-02-02 00:00:00.000000 massivechem-3.9/THOMAS_IS_BEST/COPIED_VERSION.py
--rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 massivechem-3.9/THOMAS_IS_BEST/Preliminary_v2.py
--rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 massivechem-3.9/THOMAS_IS_BEST/abundance.txt
--rw-r--r--   0        0        0     4994 2020-02-02 00:00:00.000000 massivechem-3.9/THOMAS_IS_BEST/abundance_simplified.txt
--rw-r--r--   0        0        0    15880 2020-02-02 00:00:00.000000 massivechem-3.9/THOMAS_IS_BEST/big_func.html
--rw-r--r--   0        0        0    19780 2020-02-02 00:00:00.000000 massivechem-3.9/THOMAS_IS_BEST/big_func.py
--rw-r--r--   0        0        0    14755 2020-02-02 00:00:00.000000 massivechem-3.9/THOMAS_IS_BEST/copy_file.py
--rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 massivechem-3.9/THOMAS_IS_BEST/functional_group_finder.py
--rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 massivechem-3.9/THOMAS_IS_BEST/functions.html
--rw-r--r--   0        0        0    38793 2020-02-02 00:00:00.000000 massivechem-3.9/THOMAS_IS_BEST/functions.py
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 massivechem-3.9/THOMAS_IS_BEST/molecule_image.png
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 massivechem-3.9/THOMAS_IS_BEST/names.txt
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 massivechem-3.9/THOMAS_IS_BEST/test.py
--rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 massivechem-3.9/Thomas/Copy_spectrometer.py
--rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 massivechem-3.9/Thomas/Thomas_return_pyplot.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 massivechem-3.9/Thomas/random_tests.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 massivechem-3.9/Thomas/tests.py
--rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 massivechem-3.9/data/abundance.txt
--rw-r--r--   0        0        0     5099 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Acid_image.png
--rw-r--r--   0        0        0     5734 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Acyl_chloride_image.png
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Alcohol_image.png
--rw-r--r--   0        0        0     4567 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Aldehyde_image.png
--rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Alkene_image.png
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Alkyne_image.png
--rw-r--r--   0        0        0     5111 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Amide_image.png
--rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Amine_image.png
--rw-r--r--   0        0        0     8353 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Amino_acid_image.png
--rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Anhydride_image.png
--rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Azide_image.png
--rw-r--r--   0        0        0     8884 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Benzene_image.png
--rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Bromide_image.png
--rw-r--r--   0        0        0     3926 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Carbonate2_image.png
--rw-r--r--   0        0        0     5363 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Carbonate_image.png
--rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Disulfide_image.png
--rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Enamine2_image.png
--rw-r--r--   0        0        0     9081 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Enamine_2_image.png
--rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Enamine_image.png
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Enol_image.png
--rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Ester_image.png
--rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Ether_image.png
--rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Fluoride_image.png
--rw-r--r--   0        0        0     4450 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Halogen_image.png
--rw-r--r--   0        0        0     8205 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Hemiacetal_image.png
--rw-r--r--   0        0        0     6031 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Imide_image.png
--rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Imine_image.png
--rw-r--r--   0        0        0     4430 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Iodide_image.png
--rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Ketone_image.png
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Nitrile_image.png
--rw-r--r--   0        0        0     5415 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Nitro_image.png
--rw-r--r--   0        0        0     4623 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Peroxide_image.png
--rw-r--r--   0        0        0     8473 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Phosphate_image.png
--rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Phosphine_image.png
--rw-r--r--   0        0        0     8311 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Proline_image.png
--rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Sulfides_image.png
--rw-r--r--   0        0        0    11003 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Sulfone_image.png
--rw-r--r--   0        0        0    11216 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Sulfonic_acid_image.png
--rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Sulfoxide_image.png
--rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Thio_ether_image.png
--rw-r--r--   0        0        0     5536 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Thioester_image.png
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/Thiol_image.png
--rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 massivechem-3.9/data/Functional groups images/molecule_image.png
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 massivechem-3.9/notebooks/project_report.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-3.9/notebooks/test.ipynb
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 massivechem-3.9/scripts/SMILEs_interpreter.py
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 massivechem-3.9/scripts/all_in_one.py
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 massivechem-3.9/scripts/data_list_generator.py
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 massivechem-3.9/scripts/delete_mol_image_file.py
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 massivechem-3.9/scripts/delta_function_plotter.py
--rw-r--r--   0        0        0     4170 2020-02-02 00:00:00.000000 massivechem-3.9/scripts/double_plot.py
--rw-r--r--   0        0        0     6761 2020-02-02 00:00:00.000000 massivechem-3.9/scripts/functional_group_finder.py
--rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 massivechem-3.9/scripts/functional_list_display.html
--rw-r--r--   0        0        0     6664 2020-02-02 00:00:00.000000 massivechem-3.9/scripts/functional_list_display.py
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 massivechem-3.9/scripts/insaturation.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 massivechem-3.9/scripts/ionisation_method.py
--rw-r--r--   0        0        0     4889 2020-02-02 00:00:00.000000 massivechem-3.9/scripts/main_function.py
--rw-r--r--   0        0        0     7520 2020-02-02 00:00:00.000000 massivechem-3.9/scripts/mol_web_show.html
--rw-r--r--   0        0        0     3312 2020-02-02 00:00:00.000000 massivechem-3.9/scripts/mol_web_show.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 massivechem-3.9/scripts/molecule_list_generator.py
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 massivechem-3.9/scripts/peak_merger.py
--rw-r--r--   0        0        0    16398 2020-02-02 00:00:00.000000 massivechem-3.9/scripts/spectrum.html
--rw-r--r--   0        0        0    20744 2020-02-02 00:00:00.000000 massivechem-3.9/scripts/spectrum.py
--rw-r--r--   0        0        0    49233 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/MASSiveChem.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/__init__.py
--rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/abundance.txt
--rw-r--r--   0        0        0     5099 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Acid_image.png
--rw-r--r--   0        0        0     5734 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Acyl_chloride_image.png
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Alcohol_image.png
--rw-r--r--   0        0        0     4567 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Aldehyde_image.png
--rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Alkene_image.png
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Alkyne_image.png
--rw-r--r--   0        0        0     5111 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Amide_image.png
--rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Amine_image.png
--rw-r--r--   0        0        0     8353 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Amino_acid_image.png
--rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Anhydride_image.png
--rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Azide_image.png
--rw-r--r--   0        0        0     8884 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Benzene_image.png
--rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Bromide_image.png
--rw-r--r--   0        0        0     3926 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Carbonate2_image.png
--rw-r--r--   0        0        0     5363 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Carbonate_image.png
--rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Disulfide_image.png
--rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Enamine2_image.png
--rw-r--r--   0        0        0     9081 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Enamine_2_image.png
--rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Enamine_image.png
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Enol_image.png
--rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Ester_image.png
--rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Ether_image.png
--rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Fluoride_image.png
--rw-r--r--   0        0        0     4450 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Halogen_image.png
--rw-r--r--   0        0        0     8205 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Hemiacetal_image.png
--rw-r--r--   0        0        0     6031 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Imide_image.png
--rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Imine_image.png
--rw-r--r--   0        0        0     4430 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Iodide_image.png
--rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Ketone_image.png
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Nitrile_image.png
--rw-r--r--   0        0        0     5415 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Nitro_image.png
--rw-r--r--   0        0        0     4623 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Peroxide_image.png
--rw-r--r--   0        0        0     8473 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Phosphate_image.png
--rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Phosphine_image.png
--rw-r--r--   0        0        0     8311 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Proline_image.png
--rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Sulfides_image.png
--rw-r--r--   0        0        0    11003 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Sulfone_image.png
--rw-r--r--   0        0        0    11216 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Sulfonic_acid_image.png
--rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Sulfoxide_image.png
--rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Thio_ether_image.png
--rw-r--r--   0        0        0     5536 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Thioester_image.png
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/Thiol_image.png
--rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 massivechem-3.9/src/MASSiveChem/data/Functional groups images/molecule_image.png
--rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 massivechem-3.9/.gitignore
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 massivechem-3.9/LICENSE.txt
--rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 massivechem-3.9/README.md
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 massivechem-3.9/pyproject.toml
--rw-r--r--   0        0        0     5301 2020-02-02 00:00:00.000000 massivechem-3.9/PKG-INFO
+-rw-r--r--   0        0        0   219083 2020-02-02 00:00:00.000000 massivechem-4.1/IMG_2856.jpg
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 massivechem-4.1/MASSIVEChem.yml
+-rw-r--r--   0        0        0   196052 2020-02-02 00:00:00.000000 massivechem-4.1/Spectrum_output.png
+-rw-r--r--   0        0        0    79006 2020-02-02 00:00:00.000000 massivechem-4.1/bokeh_with_plotly.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-4.1/molecule_image.png
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 massivechem-4.1/project_final.yml
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 massivechem-4.1/.idea/modules.xml
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 massivechem-4.1/.idea/ppchem-project-Christiansson-Gonteri-Humery.iml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 massivechem-4.1/.idea/vcs.xml
+-rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 massivechem-4.1/.idea/workspace.xml
+-rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 massivechem-4.1/.idea/input/input.html
+-rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 massivechem-4.1/.idea/input/input.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 massivechem-4.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0    35964 2020-02-02 00:00:00.000000 massivechem-4.1/THOMAS_IS_BEST/COPIED_VERSION.py
+-rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 massivechem-4.1/THOMAS_IS_BEST/Preliminary_v2.py
+-rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 massivechem-4.1/THOMAS_IS_BEST/abundance.txt
+-rw-r--r--   0        0        0     4994 2020-02-02 00:00:00.000000 massivechem-4.1/THOMAS_IS_BEST/abundance_simplified.txt
+-rw-r--r--   0        0        0     6815 2020-02-02 00:00:00.000000 massivechem-4.1/THOMAS_IS_BEST/base64_encoded_images.pkl
+-rw-r--r--   0        0        0    15880 2020-02-02 00:00:00.000000 massivechem-4.1/THOMAS_IS_BEST/big_func.html
+-rw-r--r--   0        0        0    19780 2020-02-02 00:00:00.000000 massivechem-4.1/THOMAS_IS_BEST/big_func.py
+-rw-r--r--   0        0        0     4234 2020-02-02 00:00:00.000000 massivechem-4.1/THOMAS_IS_BEST/conversion.py
+-rw-r--r--   0        0        0    14755 2020-02-02 00:00:00.000000 massivechem-4.1/THOMAS_IS_BEST/copy_file.py
+-rw-r--r--   0        0        0     6815 2020-02-02 00:00:00.000000 massivechem-4.1/THOMAS_IS_BEST/encoded_image.py
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 massivechem-4.1/THOMAS_IS_BEST/functional_group_display.py
+-rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 massivechem-4.1/THOMAS_IS_BEST/functional_group_finder.py
+-rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 massivechem-4.1/THOMAS_IS_BEST/functions.html
+-rw-r--r--   0        0        0    38793 2020-02-02 00:00:00.000000 massivechem-4.1/THOMAS_IS_BEST/functions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-4.1/THOMAS_IS_BEST/gpt4otest.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 massivechem-4.1/THOMAS_IS_BEST/last.py
+-rw-r--r--   0        0        0    13760 2020-02-02 00:00:00.000000 massivechem-4.1/THOMAS_IS_BEST/mol_web_show_copy.html
+-rw-r--r--   0        0        0     6844 2020-02-02 00:00:00.000000 massivechem-4.1/THOMAS_IS_BEST/test.py
+-rw-r--r--   0        0        0    14962 2020-02-02 00:00:00.000000 massivechem-4.1/THOMAS_IS_BEST/test_image.html
+-rw-r--r--   0        0        0     3367 2020-02-02 00:00:00.000000 massivechem-4.1/THOMAS_IS_BEST/test_image.py
+-rw-r--r--   0        0        0  3897887 2020-02-02 00:00:00.000000 massivechem-4.1/THOMAS_IS_BEST/igor_chem/mol_3d.html
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 massivechem-4.1/THOMAS_IS_BEST/igor_chem/mol_web_show_copy.py
+-rw-r--r--   0        0        0    15657 2020-02-02 00:00:00.000000 massivechem-4.1/THOMAS_IS_BEST/igor_chem/smiles_to_3D_plot.html
+-rw-r--r--   0        0        0    30227 2020-02-02 00:00:00.000000 massivechem-4.1/THOMAS_IS_BEST/igor_chem/smiles_to_3D_plot.py
+-rw-r--r--   0        0        0    24297 2020-02-02 00:00:00.000000 massivechem-4.1/THOMAS_IS_BEST/igor_chem/spectrum_copy.html
+-rw-r--r--   0        0        0    26678 2020-02-02 00:00:00.000000 massivechem-4.1/THOMAS_IS_BEST/igor_chem/spectrum_copy.py
+-rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 massivechem-4.1/Thomas/Copy_spectrometer.py
+-rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 massivechem-4.1/Thomas/Thomas_return_pyplot.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 massivechem-4.1/Thomas/random_tests.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 massivechem-4.1/Thomas/tests.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-4.1/notebooks/checklist.txt
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 massivechem-4.1/notebooks/project_report.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-4.1/notebooks/test.ipynb
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 massivechem-4.1/scripts/SMILEs_interpreter.py
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 massivechem-4.1/scripts/all_in_one.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 massivechem-4.1/scripts/atom_present_list.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 massivechem-4.1/scripts/calculate_unsaturation.py
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 massivechem-4.1/scripts/delta_function_plotter.py
+-rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 massivechem-4.1/scripts/double_plot.py
+-rw-r--r--   0        0        0     4413 2020-02-02 00:00:00.000000 massivechem-4.1/scripts/functional_group_display.py
+-rw-r--r--   0        0        0     6769 2020-02-02 00:00:00.000000 massivechem-4.1/scripts/functional_group_finder.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 massivechem-4.1/scripts/ionisation_method.py
+-rw-r--r--   0        0        0    12336 2020-02-02 00:00:00.000000 massivechem-4.1/scripts/main_function.py
+-rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 massivechem-4.1/scripts/mol_web_show.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 massivechem-4.1/scripts/molecule_list_generator.py
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 massivechem-4.1/scripts/peak_merger.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 massivechem-4.1/scripts/peak_sorter.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 massivechem-4.1/scripts/smiles_to_3D_plot.py
+-rw-r--r--   0        0        0    64806 2020-02-02 00:00:00.000000 massivechem-4.1/scripts/spectrum.html
+-rw-r--r--   0        0        0    27288 2020-02-02 00:00:00.000000 massivechem-4.1/scripts/spectrum.py
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 massivechem-4.1/scripts/sulphur_nitrogen_adder.py
+-rw-r--r--   0        0        0    65603 2020-02-02 00:00:00.000000 massivechem-4.1/src/MASSiveChem/MASSiveChem.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-4.1/src/MASSiveChem/__init__.py
+-rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 massivechem-4.1/tests/tests/SMILEs_interpreter_tests.py
+-rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 massivechem-4.1/tests/tests/all_in_one_tests.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 massivechem-4.1/tests/tests/atom_present_list_tests.py
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 massivechem-4.1/tests/tests/delta_function_plotter_tests.py
+-rw-r--r--   0        0        0     4170 2020-02-02 00:00:00.000000 massivechem-4.1/tests/tests/double_plot_tests.py
+-rw-r--r--   0        0        0     6149 2020-02-02 00:00:00.000000 massivechem-4.1/tests/tests/functional_group_display_tests.py
+-rw-r--r--   0        0        0     8373 2020-02-02 00:00:00.000000 massivechem-4.1/tests/tests/functional_group_finder_tests.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 massivechem-4.1/tests/tests/ionisation_method_tests.py
+-rw-r--r--   0        0        0    12336 2020-02-02 00:00:00.000000 massivechem-4.1/tests/tests/main_function_tests.py
+-rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 massivechem-4.1/tests/tests/mol_web_show_tests.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 massivechem-4.1/tests/tests/molecule_list_generator_tests.py
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 massivechem-4.1/tests/tests/peak_merger_tests.py
+-rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 massivechem-4.1/tests/tests/smiles_to_3D_plot_tests.py
+-rw-r--r--   0        0        0    27563 2020-02-02 00:00:00.000000 massivechem-4.1/tests/tests/spectrum_tests.py
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 massivechem-4.1/tests/tests/sulphur_nitrogen_adder_tests.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 massivechem-4.1/tests/tests/unsaturation_tests.py
+-rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 massivechem-4.1/.gitignore
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 massivechem-4.1/LICENSE.txt
+-rw-r--r--   0        0        0     6627 2020-02-02 00:00:00.000000 massivechem-4.1/README.md
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 massivechem-4.1/pyproject.toml
+-rw-r--r--   0        0        0     7796 2020-02-02 00:00:00.000000 massivechem-4.1/PKG-INFO
```

### Comparing `massivechem-3.9/IMG_2856.jpg` & `massivechem-4.1/IMG_2856.jpg`

 * *Files identical despite different names*

### Comparing `massivechem-3.9/project_CH200.yml` & `massivechem-4.1/project_final.yml`

 * *Files 6% similar despite different names*

```diff
@@ -34,8 +34,8 @@
       - pytz==2024.1
       - pyyaml==6.0.1
       - rdkit==2023.9.6
       - six==1.16.0
       - tornado==6.4
       - tzdata==2024.1
       - xyzservices==2024.4.0
-
+prefix: C:\Users\maintenant Pret\anaconda3\envs\project_final
```

### Comparing `massivechem-3.9/project_final.yml` & `massivechem-4.1/MASSIVEChem.yml`

 * *Files 19% similar despite different names*

```diff
@@ -13,29 +13,54 @@
   - tk=8.6.14=h0416ee5_0
   - vc=14.2=h21ff451_1
   - vs2015_runtime=14.27.29016=h5e58377_2
   - wheel=0.43.0=py310haa95532_0
   - xz=5.4.6=h8cc25b3_1
   - zlib=1.2.13=h8cc25b3_1
   - pip:
+      - bleach==6.1.0
       - bokeh==3.4.1
+      - certifi==2024.2.2
+      - charset-normalizer==3.3.2
+      - colorama==0.4.6
       - contourpy==1.2.1
       - cycler==0.12.1
+      - filelock==3.14.0
       - fonttools==4.51.0
+      - idna==3.7
       - jinja2==3.1.4
       - kiwisolver==1.4.5
+      - linkify-it-py==2.0.3
+      - markdown==3.6
+      - markdown-it-py==3.0.0
       - markupsafe==2.1.5
       - matplotlib==3.8.4
+      - mdit-py-plugins==0.4.1
+      - mdurl==0.1.2
+      - networkx==3.3
       - numpy==1.26.4
       - packaging==24.0
       - pandas==2.2.2
+      - panel==1.4.2
+      - param==2.1.0
       - pillow==10.3.0
+      - plotly==5.22.0
       - pyparsing==3.1.2
+      - pyproject-api==1.6.1
       - python-dateutil==2.9.0.post0
       - pytz==2024.1
+      - pyviz-comms==3.0.2
       - pyyaml==6.0.1
       - rdkit==2023.9.6
+      - requests==2.32.2
       - six==1.16.0
+      - tenacity==8.3.0
       - tornado==6.4
+      - tqdm==4.66.4
+      - typing-extensions==4.11.0
       - tzdata==2024.1
+      - uc-micro-py==1.0.3
+      - urllib3==2.2.1
+      - webencodings==0.5.1
+      - xyz2graph==2.0.0
       - xyzservices==2024.4.0
 prefix: C:\Users\maintenant Pret\anaconda3\envs\project_final
```

### Comparing `massivechem-3.9/.idea/workspace.xml` & `massivechem-4.1/.idea/workspace.xml`

 * *Files 19% similar despite different names*

#### Comparing `massivechem-3.9/.idea/workspace.xml` & `massivechem-4.1/.idea/workspace.xml`

```diff
@@ -1,36 +1,52 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="ChangeListManager">
-    <list default="true" id="ffcf1e29-2798-48b4-8d94-48de648cdded" name="Changes" comment=""/>
+    <list default="true" id="ffcf1e29-2798-48b4-8d94-48de648cdded" name="Changes" comment="">
+      <change beforePath="$PROJECT_DIR$/THOMAS_IS_BEST/igor_chem/mol_3d.py" beforeDir="false" afterPath="$PROJECT_DIR$/THOMAS_IS_BEST/igor_chem/mol_3d.py" afterDir="false"/>
+    </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="Git.Settings">
     <option name="RECENT_GIT_ROOT_PATH" value="$PROJECT_DIR$"/>
   </component>
+  <component name="MarkdownSettingsMigration">
+    <option name="stateVersion" value="1"/>
+  </component>
   <component name="ProjectId" id="2gYRo6Bp8xU3j3nkVpz2Ga7hebT"/>
   <component name="ProjectLevelVcsManager" settingsEditedManually="true"/>
   <component name="ProjectViewState">
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showLibraryContents" value="true"/>
   </component>
-  <component name="PropertiesComponent"><![CDATA[{
-  "keyToString": {
-    "RunOnceActivity.OpenProjectViewOnStart": "true",
-    "RunOnceActivity.ShowReadmeOnStart": "true"
+  <component name="PropertiesComponent">{
+  &quot;keyToString&quot;: {
+    &quot;RunOnceActivity.OpenProjectViewOnStart&quot;: &quot;true&quot;,
+    &quot;RunOnceActivity.ShowReadmeOnStart&quot;: &quot;true&quot;
   }
-}]]></component>
+}</component>
   <component name="SpellCheckerSettings" RuntimeDictionaries="0" Folders="0" CustomDictionaries="0" DefaultDictionary="application-level" UseSingleDictionary="true" transferred="true"/>
   <component name="TaskManager">
     <task active="true" id="Default" summary="Default task">
       <changelist id="ffcf1e29-2798-48b4-8d94-48de648cdded" name="Changes" comment=""/>
       <created>1715872699767</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1715872699767</updated>
     </task>
     <servers/>
   </component>
+  <component name="Vcs.Log.Tabs.Properties">
+    <option name="TAB_STATES">
+      <map>
+        <entry key="MAIN">
+          <value>
+            <State/>
+          </value>
+        </entry>
+      </map>
+    </option>
+  </component>
 </project>
```

### Comparing `massivechem-3.9/.idea/input/input.html` & `massivechem-4.1/.idea/input/input.html`

 * *Files identical despite different names*

### Comparing `massivechem-3.9/.idea/input/input.py` & `massivechem-4.1/.idea/input/input.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.9/THOMAS_IS_BEST/COPIED_VERSION.py` & `massivechem-4.1/THOMAS_IS_BEST/COPIED_VERSION.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.9/THOMAS_IS_BEST/Preliminary_v2.py` & `massivechem-4.1/THOMAS_IS_BEST/Preliminary_v2.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.9/THOMAS_IS_BEST/abundance.txt` & `massivechem-4.1/THOMAS_IS_BEST/abundance.txt`

 * *Files identical despite different names*

### Comparing `massivechem-3.9/THOMAS_IS_BEST/abundance_simplified.txt` & `massivechem-4.1/THOMAS_IS_BEST/abundance_simplified.txt`

 * *Files identical despite different names*

### Comparing `massivechem-3.9/THOMAS_IS_BEST/big_func.html` & `massivechem-4.1/THOMAS_IS_BEST/big_func.html`

 * *Files identical despite different names*

### Comparing `massivechem-3.9/THOMAS_IS_BEST/big_func.py` & `massivechem-4.1/THOMAS_IS_BEST/big_func.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.9/THOMAS_IS_BEST/copy_file.py` & `massivechem-4.1/THOMAS_IS_BEST/copy_file.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.9/THOMAS_IS_BEST/functional_group_finder.py` & `massivechem-4.1/THOMAS_IS_BEST/functional_group_finder.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.9/THOMAS_IS_BEST/functions.html` & `massivechem-4.1/THOMAS_IS_BEST/functions.html`

 * *Files identical despite different names*

### Comparing `massivechem-3.9/THOMAS_IS_BEST/functions.py` & `massivechem-4.1/THOMAS_IS_BEST/functions.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.9/Thomas/Copy_spectrometer.py` & `massivechem-4.1/Thomas/Copy_spectrometer.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.9/Thomas/Thomas_return_pyplot.py` & `massivechem-4.1/Thomas/Thomas_return_pyplot.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.9/Thomas/tests.py` & `massivechem-4.1/Thomas/tests.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.9/scripts/SMILEs_interpreter.py` & `massivechem-4.1/scripts/SMILEs_interpreter.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.9/scripts/delta_function_plotter.py` & `massivechem-4.1/scripts/delta_function_plotter.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,17 @@
     '''
     #---------------------------------------------------------------------------------------------#
 
     min_x , max_x = min(x_in), max(x_in)
 
     x_axis, y_axis = [min_x-0.5],[0]
     for i in range (len(x_in)):
-        x_axis.append(x_in[i]-10**(-10))
+        x_axis.append(x_in[i]-10**(-100))
         x_axis.append(x_in[i])
-        x_axis.append(x_in[i]+10**(-10))
+        x_axis.append(x_in[i]+10**(-100))
         y_axis.append(0)
         y_axis.append(y_in[i])
         y_axis.append(0)
 
     x_axis.append(max_x+1)
     y_axis.append(0)
```

### Comparing `massivechem-3.9/scripts/double_plot.py` & `massivechem-4.1/tests/tests/double_plot_tests.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.9/scripts/functional_group_finder.py` & `massivechem-4.1/scripts/functional_group_finder.py`

 * *Files 10% similar despite different names*

```diff
@@ -65,99 +65,75 @@
 
     for name, smarts in functional_groups_smarts.items():
         if mol_in.HasSubstructMatch(Chem.MolFromSmarts(smarts)):
             for _ in range(len(mol_in.GetSubstructMatches(Chem.MolFromSmarts(smarts)))):
                 functional_groups_contained.append(name)
 
     # exceptions for conflicts during the iteration of functional groups
-
-    if 'Carboxylic Acid' in functional_groups_contained:
-        functional_groups_contained.remove('Alcohol')
-    if 'Ester' in functional_groups_contained:
-        functional_groups_contained.remove('Ether')
-    if 'Phosphate' in functional_groups_contained:
-        functional_groups_contained.remove('Ether')
-    if 'Thioester' in functional_groups_contained:
-        functional_groups_contained.remove('Sulfide')
-    if 'Sulfonic acid' in functional_groups_contained:
-        functional_groups_contained.remove('Sulfide')
-    if 'Sulfoxide' in functional_groups_contained:
-        functional_groups_contained.remove('Sulfide')
-    if 'Acyl Chloride' in functional_groups_contained:
-        functional_groups_contained.remove('Chloride')
-    if 'Anhydride' in functional_groups_contained:
-        functional_groups_contained.remove('Ester')
-        functional_groups_contained.remove('Ester')
-    if 'Enamine2' in functional_groups_contained:
-        functional_groups_contained.remove('Enamine2')
-        functional_groups_contained.append('Enamine')
-    if 'Enamine3' in functional_groups_contained:
-        functional_groups_contained.remove('Enamine3')
-        functional_groups_contained.remove('Amine')
-        functional_groups_contained.append('Enamine')
-    if 'Imide' in functional_groups_contained:
-        functional_groups_contained.remove('Amide')
-        functional_groups_contained.remove('Amide')
-    if 'Enol' in functional_groups_contained:
-        functional_groups_contained.remove('Alkene')
-        functional_groups_contained.remove('Alcohol')
-    if 'Hemiacetal' in functional_groups_contained:
-        functional_groups_contained.remove('Alcohol')
-        functional_groups_contained.remove('Alcohol')
-    if 'Carbonate2' in functional_groups_contained:
-        functional_groups_contained.remove('Alcohol')
-        functional_groups_contained.remove('Alcohol')
-        functional_groups_contained.remove('Carbonate2')
-        functional_groups_contained.append('Carbonate')
-    if 'Disulfide' in functional_groups_contained:
-        functional_groups_contained.remove('Sulfide')
-        functional_groups_contained.remove('Sulfide')
-    if 'Amine' in functional_groups_contained:
-        functional_groups_contained.remove('Amine')
-    if 'Peroxide' in functional_groups_contained:
-        functional_groups_contained.remove('Ether')
-        functional_groups_contained.remove('Ether')
+    for functional_group in functional_groups_contained:
+        if 'Ester' == functional_group:
+            for _ in range (functional_groups_contained.count(functional_group)):
+                functional_groups_contained.remove('Ether')
+        elif functional_group == 'Carboxylic Acid':
+            for _ in range (functional_groups_contained.count(functional_group)):
+                functional_groups_contained.remove('Alcohol')
+        elif 'Ester' == functional_group:
+            for _ in range (functional_groups_contained.count(functional_group)):
+                functional_groups_contained.remove('Ether')
+        elif 'Phosphate' == functional_group:
+            for _ in range (functional_groups_contained.count(functional_group)):
+                functional_groups_contained.remove('Ether')
+        elif 'Thioester' == functional_group:
+            for _ in range (functional_groups_contained.count(functional_group)):
+                functional_groups_contained.remove('Sulfide')
+        elif 'Sulfonic acid' == functional_group:
+            for _ in range (functional_groups_contained.count(functional_group)):
+                functional_groups_contained.remove('Sulfide')
+        elif 'Sulfoxide' == functional_group:
+            for _ in range (functional_groups_contained.count(functional_group)):
+                functional_groups_contained.remove('Sulfide')
+        elif 'Acyl Chloride' == functional_group:
+            for _ in range (functional_groups_contained.count(functional_group)):
+                functional_groups_contained.remove('Chloride')
+        elif 'Anhydride' == functional_group:
+            for _ in range (functional_groups_contained.count(functional_group)):
+                functional_groups_contained.remove('Ester')
+                functional_groups_contained.remove('Ester')
+                functional_groups_contained.append('Ether')
+        elif 'Enamine2' == functional_group:
+            for _ in range (functional_groups_contained.count(functional_group)):
+                functional_groups_contained.remove('Enamine2')
+                functional_groups_contained.append('Enamine')
+        elif 'Enamine3' == functional_group:
+            for _ in range (functional_groups_contained.count(functional_group)):
+                functional_groups_contained.remove('Enamine3')
+                functional_groups_contained.remove('Amine')
+                functional_groups_contained.append('Enamine')
+        elif 'Imide' == functional_group:
+            for _ in range (functional_groups_contained.count(functional_group)):
+                functional_groups_contained.remove('Amide')
+                functional_groups_contained.remove('Amide')
+        elif 'Enol' == functional_group:
+            for _ in range (functional_groups_contained.count(functional_group)):
+                functional_groups_contained.remove('Alkene')
+                functional_groups_contained.remove('Alcohol')
+        elif 'Hemiacetal' == functional_group:
+            for _ in range (functional_groups_contained.count(functional_group)):
+                functional_groups_contained.remove('Alcohol')
+                functional_groups_contained.remove('Alcohol')
+        elif 'Carbonate2' == functional_group:
+            for _ in range (functional_groups_contained.count(functional_group)):
+                functional_groups_contained.remove('Alcohol')
+                functional_groups_contained.remove('Alcohol')
+                functional_groups_contained.remove('Carbonate2')
+                functional_groups_contained.append('Carbonate')
+        elif 'Disulfide' == functional_group:
+            for _ in range (functional_groups_contained.count(functional_group)):
+                functional_groups_contained.remove('Sulfide')
+                functional_groups_contained.remove('Sulfide')
+        elif 'Peroxide' == functional_group:
+            for _ in range (functional_groups_contained.count(functional_group)):
+                functional_groups_contained.remove('Ether')
+                functional_groups_contained.remove('Ether')
     
     
     return functional_groups_contained
-
-import unittest
-
-class TestFunctionalGroupFinder(unittest.TestCase):
-    def test_functional_group_finder_empty(self):
-        # Test the function with an empty SMILES string
-        mol_smi = ""
-        functional_groups = functional_group_finder(mol_smi)
-        self.assertEqual(functional_groups, [])
-
-    def test_functional_group_finder_no_functional_groups(self):
-        # Test the function with a molecule without any functional groups
-        mol_smi = "CC"
-        functional_groups = functional_group_finder(mol_smi)
-        self.assertEqual(functional_groups, [])
-
-    def test_functional_group_finder_single_functional_group(self):
-        # Test the function with a molecule containing a single functional group
-        mol_smi = "CCO"
-        functional_groups = functional_group_finder(mol_smi)
-        self.assertEqual(functional_groups, ['Alcohol'])
-
-    def test_functional_group_finder_multiple_functional_groups(self):
-        # Test the function with a molecule containing multiple functional groups
-        mol_smi = "CCOCC(=O)OC"
-        functional_groups = functional_group_finder(mol_smi)
-        self.assertEqual(functional_groups, ['Ester', 'Ether'])
-
-    def test_functional_group_finder_duplicate_functional_groups(self):
-        # Test the function with a molecule containing duplicate functional groups
-        mol_smi = "CCOCC(=O)OCCC(=O)OC(=O)C"
-        functional_groups = functional_group_finder(mol_smi)
-        self.assertEqual(functional_groups, ['Ester', 'Ether', 'Anhydride'])
-
-if __name__ == '__main__':
-    unittest.main()
-
-
-
-
-
-print(functional_group_finder('CCCC(=O)OCCC(=O)O'))
```

### Comparing `massivechem-3.9/scripts/functional_list_display.py` & `massivechem-4.1/tests/tests/functional_group_display_tests.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,107 +1,140 @@
 from bokeh.models import ColumnDataSource, HTMLTemplateFormatter
 from bokeh.models.widgets import DataTable, TableColumn
 from bokeh.plotting import show
+import base64
+from io import BytesIO
+from bokeh.models import ColumnDataSource, HTMLTemplateFormatter
+from bokeh.models.widgets import DataTable, TableColumn
+from bokeh.plotting import show
+from rdkit import Chem
+from rdkit.Chem import Draw
+
 
-def functional_group_display(groups_list):
+def functional_group_display(contained_functional_groups):
 
     #---------------------------------------------------------------------------------------------#
     '''
-    functional_group_display(groups_list)
+    functional_group_display(contained_functional_groups)
     
-    Input: list of the groups present in the molecule
-    
-    Output: Bokeh table with the names of the present functional groups as well as an image of each present functional group
+    Input: list of all contained functional groups in the molecule
+
+    Output: bokeh table with the contained functional groups and their image
     '''
     #---------------------------------------------------------------------------------------------#
 
-    # dictionnary of the images of all functional groups
-
-    functional_groups_images = {
-        'Alcohol': '../data/Functional groups images/Alcohol_image.png',
-        'Aldehyde': '../data/Functional groups images/Aldehyde_image.png',
-        'Ketone': '../data/Functional groups images/Ketone_image.png',
-        'Carboxylic Acid': '../data/Functional groups images/Acid_image.png',
-        'Ester': '../data/Functional groups images/Ester_image.png',
-        'Ether': '../data/Functional groups images/Ether_image.png',
-        'Amide': '../data/Functional groups images/Amide_image.png',
-        'Amine': '../data/Functional groups images/Amine_image.png',
-        'Nitrile': '../data/Functional groups images/Nitrile_image.png',
-        'Chloride': '../data/Functional groups images/Halogen_image.png',
-        'Bromide': '../data/Functional groups images/Bromide_image.png',
-        'Fluoride': '../data/Functional groups images/Fluoride_image.png',
-        'Iodide': '../data/Functional groups images/Iodide_image.png',
-        'Alkene': '../data/Functional groups images/Alkene_image.png',
-        'Alkyne': '../data/Functional groups images/Alkyne_image.png',
-        'Imine': '../data/Functional groups images/Imine_image.png',
-        'Amino acid': '../data/Functional groups images/Amino_acid_image.png',
-        'Proline': '../data/Functional groups images/Proline_image.png',
-        'Thiol': '../data/Functional groups images/Thiol_image.png',
-        'Sulfides': '../data/Functional groups images/Sulfides_image.png',
-        'Acyl Chloride': '../data/Functional groups images/Acyl_chloride_image.png',
-        'Anhydride': '../data/Functional groups images/Anhydride_image.png',
-        'Nitro': '../data/Functional groups images/Nitro_image.png',
-        'Enamine': '../data/Functional groups images/Enamine_image.png',
-        'Enamine2': '../data/Functional groups images/Enamine2_image.png',
-        'Enamine3': '../data/Functional groups images/Enamine3_image.png',
-        'Imide': '../data/Functional groups images/Imide_image.png',
-        'Azide': '../data/Functional groups images/Azide_image.png',
-        'Enol': '../data/Functional groups images/Enol_image.png',
-        'Hemiacetal': '../data/Functional groups images/Hemiacetal_image.png',
-        'Carbonate': '../data/Functional groups images/Carbonate_image.png',
-        'Carbonate2': '../data/Functional groups images/Carbonate2_image.png',
-        'Disulfide': '../data/Functional groups images/Disulfide_image.png',
-        'Sulfoxide': '../data/Functional groups images/Sulfoxide_image.png',
-        'Sulfone': '../data/Functional groups images/Sulfone_image.png',
-        'Sulfonic acid': '../data/Functional groups images/Sulfonic_acid_image.png',
-        'Thioester': '../data/Functional groups images/Thioester_image.png',
-        'Phosphine': '../data/Functional groups images/Phosphine_image.png',
-        'Phosphate ester': '../data/Functional groups images/Phosphate_image.png',
-        'Benzene': '../data/Functional groups images/Benzene_image.png',
-        'Peroxide': '../data/Functional groups images/Peroxide_image.png'
-}
+    #dictionnary with functional groups and associated SMARTs
+    functional_groups_smarts = {
+        'Alcohol': 'C[Oh1+0]',
+        'Aldehyde': 'C[Ch1]=O',
+        'Ketone': 'CC(=O)C',
+        'Carboxylic Acid': 'CC(=O)[Oh1]',
+        'Ester': 'CC(=O)[Oh0]',
+        'Ether': '*[Oh0]*',
+        'Amide': 'C(=O)N',
+        'Amine': '[C][N]',
+        'Nitrile': 'C#N',
+        'Chloride': 'Cl',
+        'Bromide': 'Br',
+        'Fluoride': 'F',
+        'Iodide': 'I',
+        'Alkene': 'C=C',
+        'Alkyne': 'C#C',
+        'Imine': 'C=N*',
+        'Amino acid': '[Nh2][Ch1*]C(=O)O',
+        'Proline': '[Nh1][Ch1*]C(=O)O',
+        'Thiol': '[Sh1]',
+        'Sulfide': '*[Sh0]*',
+        'Acyl Chloride': 'CC(=O)Cl',
+        'Anhydride': '*[Ch0](=O)O[Ch0](=O)*',
+        'Nitro': 'C[N+](=O)[O-]',
+        'Enamine': 'C=C[Nh0]',
+        'Enamine2': 'C=C[Nh1]',
+        'Enamine3': 'C=C[Nh2]',
+        'Imide': 'C(=O)NC(=O)*',
+        'Azide': 'CNNN',
+        'Enol': 'C=C([Oh1])C',
+        'Hemiacetal': 'CC(O)(O)C',
+        'Carbonate': '[Oh0]C(=O)[Oh0]',
+        'Carbonate2': '[Oh1]C(=O)[Oh1]',
+        'Disulfide': 'CSSC',
+        'Sulfoxide': 'CS(=O)C',
+        'Sulfone': '*[So2](=O)(=O)*',
+        'Sulfonic acid': '*S(=O)(=O)[Oh1]',
+        'Thioester': 'C(=O)S*',
+        'Phosphine': '*[Po0](*)*',
+        'Phosphate': '*OP(=O)(O)O',
+        'Benzene': 'c1ccccc1',
+        'Peroxide':'C[Oh0][Oh0]C'
+    }
+
+    #initiate empty variables
+    present_group_smarts = []    
+    present_group_images_base64 = []
     
-    # creates a dictionnary of the present groups and associated images of the molecule
-
-    present_group_images = []
+    #appends the smarts of the contained functional groups
+    for i,j in functional_groups_smarts.items():
+        for x in contained_functional_groups:
+            if x == i:
+                present_group_smarts.append(j)
+
+    #converts the smarts to images in base64 format
+    for x in present_group_smarts:
+
+        #converts SMARTs to SMILEs for the images to be nicer
+        mol_x = Chem.MolFromSmarts(x)
+        mol_smi = Chem.MolToSmiles(mol_x)
+        mol = Chem.MolFromSmiles(mol_smi)
+
+        if mol:
+
+            #creates the image
+            image = Draw.MolToImage(mol)
+
+            # Convert the image to base64 format
+            buffered = BytesIO()
+            image.save(buffered, format="PNG")
+            image_base64 = base64.b64encode(buffered.getvalue()).decode("utf-8")
 
-    for x in groups_list:
-        if x in functional_groups_images.keys():
-            present_group_images.append(functional_groups_images[x])
-        else:
-            pass
+            #appends the image to an empty dictionnary
+            present_group_images_base64.append(image_base64)
 
+    #creates a dictionnary that links the name of the functional group to its image
     data = dict(
-        groups=groups_list,
-        images=[f'<img src="{group_image}" style="width:50px;height:50px;">' for group_image in present_group_images]
+        groups=contained_functional_groups,
+        images=present_group_images_base64
     )
     source = ColumnDataSource(data)
 
-    #template for the bokeh table
-
+    #template for the bokeh table that read the base64 format 
     template = """
     <div>
-    <%= value %>
+        <img src="data:image/png;base64, <%= value %>" style="width:50px;height:50px;">
     </div>
     """
 
     # initiallizing the bokeh figure using the previous template for each functional group
-
     columns = [
         TableColumn(field="groups", title="Functional Groups"),
         TableColumn(field="images", title="Images", width=200, formatter=HTMLTemplateFormatter(template=template))
     ]
-    num_groups = len(groups_list)
+    num_groups = len(contained_functional_groups)
 
     table_height = min(200 + num_groups * 60, 800)
 
     data_table = DataTable(source=source, columns=columns, width=250, height=table_height, row_height=60)
 
     return data_table
 
+
+groups = ['Aldehyde']
+
+show(functional_group_display(groups))
+
+
 show(functional_group_display(['Alcohol', 'InvalidGroup']))
 
 import unittest
 
 class TestFunctionalGroupDisplay(unittest.TestCase):
     def test_functional_group_display(self):
         # Test the function with a list of functional groups
@@ -127,7 +160,9 @@
         self.assertEqual(len(table.columns), 2)  # Check if there are two columns
         self.assertEqual(len(table.source.data['groups']), 2)  # Check if the number of groups is 1
         self.assertEqual(table.source.data['groups'][0], 'Alcohol')  # Check if the valid group is displayed
 
 if __name__ == '__main__':
     unittest.main()
 
+
+
```

### Comparing `massivechem-3.9/scripts/ionisation_method.py` & `massivechem-4.1/scripts/ionisation_method.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.9/scripts/molecule_list_generator.py` & `massivechem-4.1/scripts/molecule_list_generator.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.9/scripts/peak_merger.py` & `massivechem-4.1/scripts/peak_merger.py`

 * *Files identical despite different names*

### Comparing `massivechem-3.9/.gitignore` & `massivechem-4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `massivechem-3.9/LICENSE.txt` & `massivechem-4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `massivechem-3.9/README.md` & `massivechem-4.1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,92 +1,138 @@
 ![logo](IMG_2856.jpg)
-![Thomas1](https://img.shields.io/badge/GIT-E44C30?style=for-the-badge&logo=git&logoColor=white)
-![Thomas2](https://img.shields.io/badge/pypi-3775A9?style=for-the-badge&logo=pypi&logoColor=white)
-![Thomas3](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue)
+[![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ThomasCsson/MASSIVEChem)
+[![Thomas3](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue)](https://www.python.org/)
 ![Thomas4](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
-![Thomas5](	https://img.shields.io/badge/Electron-2B2E3A?style=for-the-badge&logo=electron&logoColor=9FEAF9)
-![Thomas6](https://img.shields.io/badge/Jupyter-F37626.svg?&style=for-the-badge&logo=Jupyter&logoColor=white)
-![Thomas7](https://img.shields.io/badge/WeChat-07C160?style=for-the-badge&logo=wechat&logoColor=white)
+[![Thomas6](https://img.shields.io/badge/Jupyter-F37626.svg?&style=for-the-badge&logo=Jupyter&logoColor=purple)](https://jupyter.org/)
+
+
 # -         MASSIVEChem       - 
+
+[![GitHub2](https://img.shields.io/badge/Maintained%3F-yes-turquoise.svg)](https://pypi.org/user/Arthur.hmy/)
+[![python](https://img.shields.io/badge/Python-3.10-3776AB.svg?style=flat&logo=python&logoColor=orange)](https://www.python.org)
+[![GitHub3](https://img.shields.io/badge/Contributors-3-green.svg)](https://github.com/ThomasCsson/MASSIVEChem/graphs/contributors)
+[![GitHub3](https://img.shields.io/badge/License-3-purple.svg)](https://github.com/ThomasCsson/MASSIVEChem/blob/main/LICENSE.txt)
+[![GitHub3](https://img.shields.io/badge/EPFL-CH200-red.svg)](https://edu.epfl.ch/studyplan/en/bachelor/chemistry-and-chemical-engineering/coursebook/practical-programming-in-chemistry-CH-200)
+
+
  - Python package for applied analytical chemistry focused primarily on mass speectrometry 
-#### Project in practical programming in chemistry course -- EPFL CH-200
+#### Project within _practical programming in chemistry_ course -- EPFL CH-200
 
-## Package description 
-MASSIVEChem, which stands for "Mass Analytical Spectrometry System for Investigation and Visual Extrapolation in Chemistry", is a pip-installable package developped at EPFL in 2024 focused on, as its name would suggest, analytical chemistry.
-The aim of this package is to provide the user functions in order to simulate the mass spectrum of a molecule and to display this spectrum on a graph. The package also provides other features that can facilitate the chemical analysis of a molecule such as a functional group finder and an unsaturation calculator.
+## Package description
+[![GitHub3](http://ForTheBadge.com/images/badges/built-with-science.svg)](https://x.com/pschwllr/status/1760713822111723990)
+[![GitHub4](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
+
+MASSIVEChem, which stands for "Mass Analytical Spectrometry System for Investigation and Visual Extrapolation in Chemistry", is a pip-installable python package developped at EPFL in 2024 focused on, as its name would suggest, analytical chemistry.
+The aim of this package is to provide the user with functions in order to simulate the mass spectrum of a molecule and to display this spectrum on a graph. The package also provides other features that can facilitate the chemical analysis of a molecule such as a functional group finder and an unsaturation calculator.
 
 Developpers:
-- Thomas Viking Christiansson, student in chemical engineering at EPFL    https://github.com/ThomasCsson
-- Igor Gonteri, student in chemistry at EPFL                             https://github.com/igorgonteri
-- Arthur Humery, student in chemical engineering at EPFL                https://github.com/Arthurhmy
+- Thomas Viking Christiansson, student in chemical engineering at EPFL    [![jhc github](https://img.shields.io/badge/GitHub-ThomasCsson-181717.svg?style=flat&logo=github)](https://github.com/ThomasCsson)
+- Igor Gonteri, student in chemistry at EPFL                             [![jhc github](https://img.shields.io/badge/GitHub-igorgonteri-181717.svg?style=flat&logo=github)](https://github.com/igorgonteri)
+- Arthur Humery, student in chemical engineering at EPFL                [![jhc github](https://img.shields.io/badge/GitHub-Arthurhmy-181717.svg?style=flat&logo=github)](https://github.com/Arthurhmy)
 
 ### What is mass spectrometry ?
    - Mass spectrometry is an analytical technique used to identify and quantify chemical compounds in a sample by measuring the mass and sometimes the charge of molecules. It involves separating pre-charged ions according to their mass-to-charge ratio (m/z), then detecting and analysing them. This method is widely used in chemistry, biochemistry, pharmacology and other fields to characterise substances and understand their composition.
 
-Now, let us go through the steps required to use this package !
+Now, let us go through the steps required to use this package!
 
 ## Installation
+[![Thomas2](https://img.shields.io/badge/pypi-3775A9?style=for-the-badge&logo=pypi&logoColor=white)](https://pypi.org/project/MASSIVEChem/)
 
 MASSIVEChem can be installed using pip as
 ```bash
 pip install MASSIVEChem
 ```
+
+
+[![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ThomasCsson/MASSIVEChem?tab=readme-ov-file)
+
+Alternatively, the package can be directly installed from the GitHub repository via pip using the following command in the terminal
+```bash
+pip install git+https://github.com/ThomasCsson/MASSIVEChem
+```
+
+
+![Thomas1](https://img.shields.io/badge/GIT-E44C30?style=for-the-badge&logo=git&logoColor=white)
+
 The package can also be installed from source by running the following commands
 
 First, clone the repository from github and go in the folder. 
 ```bash
 git clone https://github.com/ThomasCsson/MASSIVEChem.git
 cd MASSIVEChem
 ```
 Then, install the package using : 
 ```bash
-pip install -e . 
+pip install -e .
 ```
 
+
+
+
+
+
+
 ## Requirments
 The package runs on python 3.10 but supports python 3.8 through 3.10
 The package requires several other packages to function correctly.
 
 ```bash
 matplotlib
 bokeh
 rdkit
 pandas
+panel 
+xyz2graph
 ```
-If everything runs in order during the installation, the preceding packages should install automatically.
-But check that these packages are correctly installed using 
+
+
+If all goes well during installation, the preceding packages should all install automatically.
+But this can be checked by veryfying that they have all been installed in the desired environment. To do this, simply write the following command in the terminal:
 
 ```bash
 pip show "name of the package"
 ```
 
-If not, install them using the following commands, otherwise the package will not work. 
+If not, install them using the following commands. (Bear in mind that the package will not run without its dependencies. 
 
 ```bash
 pip install matplotlib
 pip install bokeh
 pip install rdkit
 pip install pandas
+pip install panel
 ```
+Additionally, the package 'xyz2graph' is required to run the 3D imaging functionallity in the function XXX. This package is not pip-installable, so to intall it yourslef, the following command needs to be run.
+
+```bash
+python -m pip install git+https://github.com/zotko/xyz2graph.git
+```
+
 
 ## Usage
 
 The principal function of this package takes the SMILEs of a molecule as an input and displays the mass spectrometry of the molecule as well as the molecule itself and  the functional groups it contains.
 
-An example on how to make the function work is shown below for penicilin:
+An example on how to make the function work is shown below for benzylpenicilin:
+
+The ionization method is set to monodeprotonation and the resolution of the apparatus is 0.01 Th
 
 ```bash
 import MASSIVEChem as ms
 from ms.MASSIVEChem import spectrum
 from bokeh.plotting import show
 
 mol_smi = 'CC1(C(N2C(S1)C(C2=O)NC(=O)CC3=CC=CC=C3)C(=O)O)C'
+apparatus_resolution = 0.01
 
-show(spectrum(mol_smi))
+show(spectrum(mol_smi, True, apparatus_resolution))
 ```
+The output of this command will be:
 
+![Spectrum](Spectrum_output.png)
 ## Getting started
+[![jupyter](https://img.shields.io/badge/Jupyter-Lab-F37626.svg?style=flat&logo=Jupyter)](https://jupyterlab.readthedocs.io/en/stable)
 
 To begin to use the package the following jupyter notebook will give you information about all the package's functions:
 
 '''link to jupter notebook'''
```

### Comparing `massivechem-3.9/pyproject.toml` & `massivechem-4.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 00000000: 5b62 7569 6c64 2d73 7973 7465 6d5d 0d0a  [build-system]..
 00000010: 7265 7175 6972 6573 203d 205b 2268 6174  requires = ["hat
 00000020: 6368 6c69 6e67 225d 0d0a 6275 696c 642d  chling"]..build-
 00000030: 6261 636b 656e 6420 3d20 2268 6174 6368  backend = "hatch
 00000040: 6c69 6e67 2e62 7569 6c64 220d 0a0d 0a5b  ling.build"....[
 00000050: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000060: 2022 4d41 5353 4956 4543 6865 6d22 0d0a   "MASSIVEChem"..
-00000070: 7665 7273 696f 6e20 3d20 2233 2e39 220d  version = "3.9".
+00000070: 7665 7273 696f 6e20 3d20 2234 2e31 220d  version = "4.1".
 00000080: 0a64 6573 6372 6970 7469 6f6e 203d 2022  .description = "
 00000090: 4d41 5353 4956 4543 6865 6d20 6973 2061  MASSIVEChem is a
 000000a0: 2070 6970 2d69 6e73 7461 6c6c 6162 6c65   pip-installable
 000000b0: 2070 6163 6b61 6765 2066 6f72 2061 6e61   package for ana
 000000c0: 6c79 7469 6361 6c20 6368 656d 6973 7472  lytical chemistr
 000000d0: 792e 2049 7420 7369 6d75 6c61 7465 7320  y. It simulates 
 000000e0: 6d6f 6c65 6375 6c65 206d 6173 7320 7370  molecule mass sp
@@ -55,44 +55,37 @@
 00000360: 6875 7220 4875 6d65 7279 222c 2065 6d61  hur Humery", ema
 00000370: 696c 203d 2022 6172 7468 7572 2e68 756d  il = "arthur.hum
 00000380: 6572 7940 6570 666c 2e63 6822 207d 0d0a  ery@epfl.ch" }..
 00000390: 5d0d 0a64 6570 656e 6465 6e63 6965 7320  ]..dependencies 
 000003a0: 3d20 5b0d 0a20 2022 7264 6b69 7422 2c0d  = [..  "rdkit",.
 000003b0: 0a20 2022 7061 6e64 6173 222c 0d0a 2020  .  "pandas",..  
 000003c0: 226d 6174 706c 6f74 6c69 6222 2c0d 0a20  "matplotlib",.. 
-000003d0: 2022 626f 6b65 6822 2c0d 0a5d 0d0a 636c   "bokeh",..]..cl
-000003e0: 6173 7369 6669 6572 7320 3d20 5b0d 0a20  assifiers = [.. 
-000003f0: 2020 2022 4465 7665 6c6f 706d 656e 7420     "Development 
-00000400: 5374 6174 7573 203a 3a20 3420 2d20 4265  Status :: 4 - Be
-00000410: 7461 222c 0d0a 2020 2020 2250 726f 6772  ta",..    "Progr
-00000420: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000430: 3a3a 2050 7974 686f 6e20 3a3a 2033 222c  :: Python :: 3",
-00000440: 0d0a 2020 2020 224c 6963 656e 7365 203a  ..    "License :
-00000450: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
-00000460: 3a20 4d49 5420 4c69 6365 6e73 6522 2c0d  : MIT License",.
-00000470: 0a20 2020 2022 4f70 6572 6174 696e 6720  .    "Operating 
-00000480: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
-00000490: 6570 656e 6465 6e74 220d 0a5d 0d0a 0d0a  ependent"..]....
-000004a0: 5b74 6f6f 6c2e 706f 6574 7279 2e66 696c  [tool.poetry.fil
-000004b0: 6573 5d0d 0a69 6e63 6c75 6465 203d 205b  es]..include = [
-000004c0: 2273 7263 2f4d 4153 5369 7665 4368 656d  "src/MASSiveChem
-000004d0: 2f64 6174 612f 6162 756e 6461 6e63 652e  /data/abundance.
-000004e0: 7478 7422 2c22 7372 632f 4d41 5353 6976  txt","src/MASSiv
-000004f0: 6543 6865 6d2f 6461 7461 2f46 756e 6374  eChem/data/Funct
-00000500: 696f 6e61 6c20 6772 6f75 7073 2069 6d61  ional groups ima
-00000510: 6765 7322 5d0d 0a0d 0a0d 0a5b 7072 6f6a  ges"]......[proj
-00000520: 6563 742e 7572 6c73 5d0d 0a48 6f6d 6570  ect.urls]..Homep
-00000530: 6167 6520 3d20 2268 7474 7073 3a2f 2f67  age = "https://g
-00000540: 6974 6875 622e 636f 6d2f 5468 6f6d 6173  ithub.com/Thomas
-00000550: 4373 736f 6e2f 4d41 5353 4956 4543 6865  Csson/MASSIVEChe
-00000560: 6d2e 6769 7422 0d0a 4769 7448 7562 5f54  m.git"..GitHub_T
-00000570: 686f 6d61 735f 4368 7269 7374 6961 6e73  homas_Christians
-00000580: 736f 6e20 3d20 2268 7474 7073 3a2f 2f67  son = "https://g
-00000590: 6974 6875 622e 636f 6d2f 5468 6f6d 6173  ithub.com/Thomas
-000005a0: 4373 736f 6e22 0d0a 4769 7448 7562 5f49  Csson"..GitHub_I
-000005b0: 676f 725f 476f 6e74 6572 6920 3d20 2268  gor_Gonteri = "h
-000005c0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000005d0: 6d2f 6967 6f72 676f 6e74 6572 6922 0d0a  m/igorgonteri"..
-000005e0: 4769 7448 7562 5f41 7274 6875 725f 4875  GitHub_Arthur_Hu
-000005f0: 6d65 7279 203d 2022 6874 7470 733a 2f2f  mery = "https://
-00000600: 6769 7468 7562 2e63 6f6d 2f41 7274 6875  github.com/Arthu
-00000610: 7268 6d79 220d 0a                        rhmy"..
+000003d0: 2022 626f 6b65 6822 2c0d 0a20 2022 7061   "bokeh",..  "pa
+000003e0: 6e65 6c22 2c0d 0a5d 0d0a 636c 6173 7369  nel",..]..classi
+000003f0: 6669 6572 7320 3d20 5b0d 0a20 2020 2022  fiers = [..    "
+00000400: 4465 7665 6c6f 706d 656e 7420 5374 6174  Development Stat
+00000410: 7573 203a 3a20 3420 2d20 4265 7461 222c  us :: 4 - Beta",
+00000420: 0d0a 2020 2020 2250 726f 6772 616d 6d69  ..    "Programmi
+00000430: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000440: 7974 686f 6e20 3a3a 2033 222c 0d0a 2020  ython :: 3",..  
+00000450: 2020 224c 6963 656e 7365 203a 3a20 4f53    "License :: OS
+00000460: 4920 4170 7072 6f76 6564 203a 3a20 4d49  I Approved :: MI
+00000470: 5420 4c69 6365 6e73 6522 2c0d 0a20 2020  T License",..   
+00000480: 2022 4f70 6572 6174 696e 6720 5379 7374   "Operating Syst
+00000490: 656d 203a 3a20 4f53 2049 6e64 6570 656e  em :: OS Indepen
+000004a0: 6465 6e74 220d 0a5d 0d0a 0d0a 5b70 726f  dent"..]....[pro
+000004b0: 6a65 6374 2e75 726c 735d 0d0a 486f 6d65  ject.urls]..Home
+000004c0: 7061 6765 203d 2022 6874 7470 733a 2f2f  page = "https://
+000004d0: 6769 7468 7562 2e63 6f6d 2f54 686f 6d61  github.com/Thoma
+000004e0: 7343 7373 6f6e 2f4d 4153 5349 5645 4368  sCsson/MASSIVECh
+000004f0: 656d 2e67 6974 220d 0a47 6974 4875 625f  em.git"..GitHub_
+00000500: 5468 6f6d 6173 5f43 6872 6973 7469 616e  Thomas_Christian
+00000510: 7373 6f6e 203d 2022 6874 7470 733a 2f2f  sson = "https://
+00000520: 6769 7468 7562 2e63 6f6d 2f54 686f 6d61  github.com/Thoma
+00000530: 7343 7373 6f6e 220d 0a47 6974 4875 625f  sCsson"..GitHub_
+00000540: 4967 6f72 5f47 6f6e 7465 7269 203d 2022  Igor_Gonteri = "
+00000550: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000560: 6f6d 2f69 676f 7267 6f6e 7465 7269 220d  om/igorgonteri".
+00000570: 0a47 6974 4875 625f 4172 7468 7572 5f48  .GitHub_Arthur_H
+00000580: 756d 6572 7920 3d20 2268 7474 7073 3a2f  umery = "https:/
+00000590: 2f67 6974 6875 622e 636f 6d2f 4172 7468  /github.com/Arth
+000005a0: 7572 686d 7922 0d0a                      urhmy"..
```

### Comparing `massivechem-3.9/PKG-INFO` & `massivechem-4.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: MASSIVEChem
-Version: 3.9
+Version: 4.1
 Summary: MASSIVEChem is a pip-installable package for analytical chemistry. It simulates molecule mass spectra and graphically displays them. It includes tools like a functional group finder and unsaturation calculator to aid chemical analysis.
 Project-URL: Homepage, https://github.com/ThomasCsson/MASSIVEChem.git
 Project-URL: GitHub_Thomas_Christiansson, https://github.com/ThomasCsson
 Project-URL: GitHub_Igor_Gonteri, https://github.com/igorgonteri
 Project-URL: GitHub_Arthur_Humery, https://github.com/Arthurhmy
 Author-email: Thomas Viking Christiansson <thomas.christiansson@epfl.ch>, Igor Gonteri <igor.gonteri@epfl.ch>, Arthur Humery <arthur.humery@epfl.ch>
 License-Expression: MIT
@@ -14,102 +14,149 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: bokeh
 Requires-Dist: matplotlib
 Requires-Dist: pandas
+Requires-Dist: panel
 Requires-Dist: rdkit
 Description-Content-Type: text/markdown
 
 ![logo](IMG_2856.jpg)
-![Thomas1](https://img.shields.io/badge/GIT-E44C30?style=for-the-badge&logo=git&logoColor=white)
-![Thomas2](https://img.shields.io/badge/pypi-3775A9?style=for-the-badge&logo=pypi&logoColor=white)
-![Thomas3](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue)
+[![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ThomasCsson/MASSIVEChem)
+[![Thomas3](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue)](https://www.python.org/)
 ![Thomas4](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
-![Thomas5](	https://img.shields.io/badge/Electron-2B2E3A?style=for-the-badge&logo=electron&logoColor=9FEAF9)
-![Thomas6](https://img.shields.io/badge/Jupyter-F37626.svg?&style=for-the-badge&logo=Jupyter&logoColor=white)
-![Thomas7](https://img.shields.io/badge/WeChat-07C160?style=for-the-badge&logo=wechat&logoColor=white)
+[![Thomas6](https://img.shields.io/badge/Jupyter-F37626.svg?&style=for-the-badge&logo=Jupyter&logoColor=purple)](https://jupyter.org/)
+
+
 # -         MASSIVEChem       - 
+
+[![GitHub2](https://img.shields.io/badge/Maintained%3F-yes-turquoise.svg)](https://pypi.org/user/Arthur.hmy/)
+[![python](https://img.shields.io/badge/Python-3.10-3776AB.svg?style=flat&logo=python&logoColor=orange)](https://www.python.org)
+[![GitHub3](https://img.shields.io/badge/Contributors-3-green.svg)](https://github.com/ThomasCsson/MASSIVEChem/graphs/contributors)
+[![GitHub3](https://img.shields.io/badge/License-3-purple.svg)](https://github.com/ThomasCsson/MASSIVEChem/blob/main/LICENSE.txt)
+[![GitHub3](https://img.shields.io/badge/EPFL-CH200-red.svg)](https://edu.epfl.ch/studyplan/en/bachelor/chemistry-and-chemical-engineering/coursebook/practical-programming-in-chemistry-CH-200)
+
+
  - Python package for applied analytical chemistry focused primarily on mass speectrometry 
-#### Project in practical programming in chemistry course -- EPFL CH-200
+#### Project within _practical programming in chemistry_ course -- EPFL CH-200
 
-## Package description 
-MASSIVEChem, which stands for "Mass Analytical Spectrometry System for Investigation and Visual Extrapolation in Chemistry", is a pip-installable package developped at EPFL in 2024 focused on, as its name would suggest, analytical chemistry.
-The aim of this package is to provide the user functions in order to simulate the mass spectrum of a molecule and to display this spectrum on a graph. The package also provides other features that can facilitate the chemical analysis of a molecule such as a functional group finder and an unsaturation calculator.
+## Package description
+[![GitHub3](http://ForTheBadge.com/images/badges/built-with-science.svg)](https://x.com/pschwllr/status/1760713822111723990)
+[![GitHub4](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
+
+MASSIVEChem, which stands for "Mass Analytical Spectrometry System for Investigation and Visual Extrapolation in Chemistry", is a pip-installable python package developped at EPFL in 2024 focused on, as its name would suggest, analytical chemistry.
+The aim of this package is to provide the user with functions in order to simulate the mass spectrum of a molecule and to display this spectrum on a graph. The package also provides other features that can facilitate the chemical analysis of a molecule such as a functional group finder and an unsaturation calculator.
 
 Developpers:
-- Thomas Viking Christiansson, student in chemical engineering at EPFL    https://github.com/ThomasCsson
-- Igor Gonteri, student in chemistry at EPFL                             https://github.com/igorgonteri
-- Arthur Humery, student in chemical engineering at EPFL                https://github.com/Arthurhmy
+- Thomas Viking Christiansson, student in chemical engineering at EPFL    [![jhc github](https://img.shields.io/badge/GitHub-ThomasCsson-181717.svg?style=flat&logo=github)](https://github.com/ThomasCsson)
+- Igor Gonteri, student in chemistry at EPFL                             [![jhc github](https://img.shields.io/badge/GitHub-igorgonteri-181717.svg?style=flat&logo=github)](https://github.com/igorgonteri)
+- Arthur Humery, student in chemical engineering at EPFL                [![jhc github](https://img.shields.io/badge/GitHub-Arthurhmy-181717.svg?style=flat&logo=github)](https://github.com/Arthurhmy)
 
 ### What is mass spectrometry ?
    - Mass spectrometry is an analytical technique used to identify and quantify chemical compounds in a sample by measuring the mass and sometimes the charge of molecules. It involves separating pre-charged ions according to their mass-to-charge ratio (m/z), then detecting and analysing them. This method is widely used in chemistry, biochemistry, pharmacology and other fields to characterise substances and understand their composition.
 
-Now, let us go through the steps required to use this package !
+Now, let us go through the steps required to use this package!
 
 ## Installation
+[![Thomas2](https://img.shields.io/badge/pypi-3775A9?style=for-the-badge&logo=pypi&logoColor=white)](https://pypi.org/project/MASSIVEChem/)
 
 MASSIVEChem can be installed using pip as
 ```bash
 pip install MASSIVEChem
 ```
+
+
+[![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ThomasCsson/MASSIVEChem?tab=readme-ov-file)
+
+Alternatively, the package can be directly installed from the GitHub repository via pip using the following command in the terminal
+```bash
+pip install git+https://github.com/ThomasCsson/MASSIVEChem
+```
+
+
+![Thomas1](https://img.shields.io/badge/GIT-E44C30?style=for-the-badge&logo=git&logoColor=white)
+
 The package can also be installed from source by running the following commands
 
 First, clone the repository from github and go in the folder. 
 ```bash
 git clone https://github.com/ThomasCsson/MASSIVEChem.git
 cd MASSIVEChem
 ```
 Then, install the package using : 
 ```bash
-pip install -e . 
+pip install -e .
 ```
 
+
+
+
+
+
+
 ## Requirments
 The package runs on python 3.10 but supports python 3.8 through 3.10
 The package requires several other packages to function correctly.
 
 ```bash
 matplotlib
 bokeh
 rdkit
 pandas
+panel 
+xyz2graph
 ```
-If everything runs in order during the installation, the preceding packages should install automatically.
-But check that these packages are correctly installed using 
+
+
+If all goes well during installation, the preceding packages should all install automatically.
+But this can be checked by veryfying that they have all been installed in the desired environment. To do this, simply write the following command in the terminal:
 
 ```bash
 pip show "name of the package"
 ```
 
-If not, install them using the following commands, otherwise the package will not work. 
+If not, install them using the following commands. (Bear in mind that the package will not run without its dependencies. 
 
 ```bash
 pip install matplotlib
 pip install bokeh
 pip install rdkit
 pip install pandas
+pip install panel
 ```
+Additionally, the package 'xyz2graph' is required to run the 3D imaging functionallity in the function XXX. This package is not pip-installable, so to intall it yourslef, the following command needs to be run.
+
+```bash
+python -m pip install git+https://github.com/zotko/xyz2graph.git
+```
+
 
 ## Usage
 
 The principal function of this package takes the SMILEs of a molecule as an input and displays the mass spectrometry of the molecule as well as the molecule itself and  the functional groups it contains.
 
-An example on how to make the function work is shown below for penicilin:
+An example on how to make the function work is shown below for benzylpenicilin:
+
+The ionization method is set to monodeprotonation and the resolution of the apparatus is 0.01 Th
 
 ```bash
 import MASSIVEChem as ms
 from ms.MASSIVEChem import spectrum
 from bokeh.plotting import show
 
 mol_smi = 'CC1(C(N2C(S1)C(C2=O)NC(=O)CC3=CC=CC=C3)C(=O)O)C'
+apparatus_resolution = 0.01
 
-show(spectrum(mol_smi))
+show(spectrum(mol_smi, True, apparatus_resolution))
 ```
+The output of this command will be:
 
+![Spectrum](Spectrum_output.png)
 ## Getting started
+[![jupyter](https://img.shields.io/badge/Jupyter-Lab-F37626.svg?style=flat&logo=Jupyter)](https://jupyterlab.readthedocs.io/en/stable)
 
 To begin to use the package the following jupyter notebook will give you information about all the package's functions:
 
 '''link to jupter notebook'''
```

