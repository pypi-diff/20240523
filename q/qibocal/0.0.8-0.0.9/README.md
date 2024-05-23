# Comparing `tmp/qibocal-0.0.8.tar.gz` & `tmp/qibocal-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qibocal-0.0.8.tar", max compression
+gzip compressed data, was "qibocal-0.0.9.tar", max compression
```

## Comparing `qibocal-0.0.8.tar` & `qibocal-0.0.9.tar`

### file list

```diff
@@ -1,128 +1,132 @@
--rw-r--r--   0        0        0    11357 2024-04-06 07:35:22.825498 qibocal-0.0.8/LICENSE
--rw-r--r--   0        0        0     3045 2024-04-06 07:35:22.825498 qibocal-0.0.8/README.md
--rw-r--r--   0        0        0     2797 2024-04-06 07:35:22.837499 qibocal-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      173 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/__init__.py
--rw-r--r--   0        0        0       30 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/auto/__init__.py
--rw-r--r--   0        0        0     2293 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/auto/execute.py
--rw-r--r--   0        0        0     1422 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/auto/history.py
--rw-r--r--   0        0        0      153 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/auto/mode.py
--rw-r--r--   0        0        0    10411 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/auto/operation.py
--rw-r--r--   0        0        0     2602 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/auto/runcard.py
--rw-r--r--   0        0        0      758 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/auto/serialize.py
--rw-r--r--   0        0        0     1180 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/auto/status.py
--rw-r--r--   0        0        0     6064 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/auto/task.py
--rw-r--r--   0        0        0       51 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/cli/__init__.py
--rw-r--r--   0        0        0     4479 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/cli/_base.py
--rw-r--r--   0        0        0     1602 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/cli/acquisition.py
--rw-r--r--   0        0        0     2137 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/cli/autocalibration.py
--rw-r--r--   0        0        0     2518 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/cli/fit.py
--rw-r--r--   0        0        0     3627 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/cli/report.py
--rw-r--r--   0        0        0     2538 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/cli/upload.py
--rw-r--r--   0        0        0     2290 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/cli/utils.py
--rw-r--r--   0        0        0     1755 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/config.py
--rw-r--r--   0        0        0        0 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/fitting/classifier/__init__.py
--rw-r--r--   0        0        0     1224 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/fitting/classifier/ada_boost.py
--rw-r--r--   0        0        0      804 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/fitting/classifier/data.py
--rw-r--r--   0        0        0     1139 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/fitting/classifier/decision_tree.py
--rw-r--r--   0        0        0      895 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/fitting/classifier/gaussian_process.py
--rw-r--r--   0        0        0      801 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/fitting/classifier/linear_svm.py
--rw-r--r--   0        0        0      737 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/fitting/classifier/naive_bayes.py
--rw-r--r--   0        0        0     1675 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/fitting/classifier/qblox_fit.py
--rw-r--r--   0        0        0     4530 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/fitting/classifier/qubit_fit.py
--rw-r--r--   0        0        0     1241 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/fitting/classifier/random_forest.py
--rw-r--r--   0        0        0     1133 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/fitting/classifier/rbf_svm.py
--rw-r--r--   0        0        0     8095 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/fitting/classifier/run.py
--rw-r--r--   0        0        0     1121 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/fitting/classifier/scikit_utils.py
--rw-r--r--   0        0        0     5501 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/__init__.py
--rw-r--r--   0        0        0        0 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/allxy/__init__.py
--rw-r--r--   0        0        0     7601 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/allxy/allxy.py
--rw-r--r--   0        0        0     4842 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/allxy/allxy_drag_pulse_tuning.py
--rw-r--r--   0        0        0    14336 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/classification.py
--rw-r--r--   0        0        0        0 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/coherence/__init__.py
--rw-r--r--   0        0        0     6247 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/coherence/spin_echo.py
--rw-r--r--   0        0        0     6804 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/coherence/spin_echo_signal.py
--rw-r--r--   0        0        0     6230 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/coherence/t1.py
--rw-r--r--   0        0        0     3329 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/coherence/t1_sequences.py
--rw-r--r--   0        0        0     6343 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/coherence/t1_signal.py
--rw-r--r--   0        0        0     5411 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/coherence/t2.py
--rw-r--r--   0        0        0     2551 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/coherence/t2_sequences.py
--rw-r--r--   0        0        0     5492 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/coherence/t2_signal.py
--rw-r--r--   0        0        0     3939 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/coherence/utils.py
--rw-r--r--   0        0        0     5757 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/coherence/zeno.py
--rw-r--r--   0        0        0     5676 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/coherence/zeno_signal.py
--rw-r--r--   0        0        0        0 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/couplers/__init__.py
--rw-r--r--   0        0        0     4905 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/couplers/coupler_chevron.py
--rw-r--r--   0        0        0     4892 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/couplers/coupler_qubit_spectroscopy.py
--rw-r--r--   0        0        0     5858 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/couplers/coupler_resonator_spectroscopy.py
--rw-r--r--   0        0        0     2047 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/couplers/utils.py
--rw-r--r--   0        0        0    11118 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/dispersive_shift.py
--rw-r--r--   0        0        0     9492 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/dispersive_shift_qutrit.py
--rw-r--r--   0        0        0     8688 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/drag.py
--rw-r--r--   0        0        0        0 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/fast_reset/_init__.py
--rw-r--r--   0        0        0     6896 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/fast_reset/fast_reset.py
--rw-r--r--   0        0        0     9675 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/flipping.py
--rw-r--r--   0        0        0     9992 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/flipping_signal.py
--rw-r--r--   0        0        0        0 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/flux_dependence/__init__.py
--rw-r--r--   0        0        0    11514 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/flux_dependence/avoided_crossing.py
--rw-r--r--   0        0        0     5808 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/flux_dependence/qubit_crosstalk.py
--rw-r--r--   0        0        0     8921 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/flux_dependence/qubit_flux_dependence.py
--rw-r--r--   0        0        0     5439 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/flux_dependence/qubit_flux_tracking.py
--rw-r--r--   0        0        0     5546 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/flux_dependence/resonator_crosstalk.py
--rw-r--r--   0        0        0    14467 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/flux_dependence/resonator_flux_dependence.py
--rw-r--r--   0        0        0     8839 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/flux_dependence/utils.py
--rw-r--r--   0        0        0     5647 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/qubit_spectroscopy.py
--rw-r--r--   0        0        0     6371 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/qubit_spectroscopy_ef.py
--rw-r--r--   0        0        0     5732 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/qutrit_classification.py
--rw-r--r--   0        0        0        0 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/rabi/__init__.py
--rw-r--r--   0        0        0     5971 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/rabi/amplitude.py
--rw-r--r--   0        0        0     6553 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/rabi/amplitude_signal.py
--rw-r--r--   0        0        0     3760 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/rabi/ef.py
--rw-r--r--   0        0        0     6744 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/rabi/length.py
--rw-r--r--   0        0        0     2843 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/rabi/length_sequences.py
--rw-r--r--   0        0        0     6712 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/rabi/length_signal.py
--rw-r--r--   0        0        0     5819 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/rabi/utils.py
--rw-r--r--   0        0        0        0 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/ramsey/__init__.py
--rw-r--r--   0        0        0    10249 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/ramsey/ramsey.py
--rw-r--r--   0        0        0     9650 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/ramsey/ramsey_signal.py
--rw-r--r--   0        0        0     3351 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/ramsey/utils.py
--rw-r--r--   0        0        0        0 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/randomized_benchmarking/__init__.py
--rw-r--r--   0        0        0     2496 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/randomized_benchmarking/circuit_tools.py
--rw-r--r--   0        0        0     7044 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/randomized_benchmarking/fitting.py
--rw-r--r--   0        0        0     1808 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/randomized_benchmarking/noisemodels.py
--rw-r--r--   0        0        0    14201 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/randomized_benchmarking/standard_rb.py
--rw-r--r--   0        0        0     5997 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/randomized_benchmarking/utils.py
--rw-r--r--   0        0        0     8532 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/readout_characterization.py
--rw-r--r--   0        0        0     6498 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/readout_mitigation_matrix.py
--rw-r--r--   0        0        0     7038 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/readout_optimization/resonator_amplitude.py
--rw-r--r--   0        0        0     7546 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/readout_optimization/resonator_frequency.py
--rw-r--r--   0        0        0        0 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/readout_optimization/twpa_calibration/__init__.py
--rw-r--r--   0        0        0     6140 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/readout_optimization/twpa_calibration/frequency.py
--rw-r--r--   0        0        0     8192 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/readout_optimization/twpa_calibration/frequency_SNR.py
--rw-r--r--   0        0        0     7707 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/readout_optimization/twpa_calibration/frequency_power.py
--rw-r--r--   0        0        0     5805 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/readout_optimization/twpa_calibration/power.py
--rw-r--r--   0        0        0     7938 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/readout_optimization/twpa_calibration/power_SNR.py
--rw-r--r--   0        0        0     8182 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/resonator_punchout.py
--rw-r--r--   0        0        0     8168 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/resonator_punchout_attenuation.py
--rw-r--r--   0        0        0     9282 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/resonator_spectroscopy.py
--rw-r--r--   0        0        0     6928 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/signal_experiments/calibrate_state_discrimination.py
--rw-r--r--   0        0        0     4706 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/signal_experiments/time_of_flight_readout.py
--rw-r--r--   0        0        0      178 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/two_qubit_interaction/__init__.py
--rw-r--r--   0        0        0       72 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/two_qubit_interaction/chevron/__init__.py
--rw-r--r--   0        0        0    10062 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/two_qubit_interaction/chevron/chevron.py
--rw-r--r--   0        0        0     4199 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/two_qubit_interaction/chevron/chevron_signal.py
--rw-r--r--   0        0        0     2290 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/two_qubit_interaction/chevron/utils.py
--rw-r--r--   0        0        0       49 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/two_qubit_interaction/chsh/__init__.py
--rw-r--r--   0        0        0     2970 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/two_qubit_interaction/chsh/circuits.py
--rw-r--r--   0        0        0    11961 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/two_qubit_interaction/chsh/protocol.py
--rw-r--r--   0        0        0     3269 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/two_qubit_interaction/chsh/pulses.py
--rw-r--r--   0        0        0      722 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/two_qubit_interaction/chsh/utils.py
--rw-r--r--   0        0        0    15482 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/two_qubit_interaction/cz_virtualz.py
--rw-r--r--   0        0        0     4868 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/two_qubit_interaction/cz_virtualz_signal.py
--rw-r--r--   0        0        0     2342 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/two_qubit_interaction/utils.py
--rw-r--r--   0        0        0    22117 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/utils.py
--rw-r--r--   0        0        0     7198 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/update.py
--rw-r--r--   0        0        0        0 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/web/__init__.py
--rw-r--r--   0        0        0      811 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/web/report.py
--rw-r--r--   0        0        0     4168 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/web/static/styles.css
--rw-r--r--   0        0        0     8558 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/web/templates/template.html
--rw-r--r--   0        0        0     4720 1970-01-01 00:00:00.000000 qibocal-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-23 09:00:58.840306 qibocal-0.0.9/LICENSE
+-rw-r--r--   0        0        0     3036 2024-05-23 09:00:58.840306 qibocal-0.0.9/README.md
+-rw-r--r--   0        0        0     2797 2024-05-23 09:00:58.856306 qibocal-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      173 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/__init__.py
+-rw-r--r--   0        0        0       30 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/auto/__init__.py
+-rw-r--r--   0        0        0     2009 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/auto/execute.py
+-rw-r--r--   0        0        0     1176 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/auto/history.py
+-rw-r--r--   0        0        0      153 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/auto/mode.py
+-rw-r--r--   0        0        0    11261 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/auto/operation.py
+-rw-r--r--   0        0        0     2243 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/auto/runcard.py
+-rw-r--r--   0        0        0      758 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/auto/serialize.py
+-rw-r--r--   0        0        0     1180 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/auto/status.py
+-rw-r--r--   0        0        0     5626 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/auto/task.py
+-rw-r--r--   0        0        0     3220 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/auto/transpile.py
+-rw-r--r--   0        0        0       51 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/cli/__init__.py
+-rw-r--r--   0        0        0     4479 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/cli/_base.py
+-rw-r--r--   0        0        0     1601 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/cli/acquisition.py
+-rw-r--r--   0        0        0     2044 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/cli/autocalibration.py
+-rw-r--r--   0        0        0     2518 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/cli/fit.py
+-rw-r--r--   0        0        0     3453 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/cli/report.py
+-rw-r--r--   0        0        0     2538 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/cli/upload.py
+-rw-r--r--   0        0        0     2290 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/cli/utils.py
+-rw-r--r--   0        0        0     1755 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/config.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/fitting/classifier/__init__.py
+-rw-r--r--   0        0        0     1224 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/fitting/classifier/ada_boost.py
+-rw-r--r--   0        0        0      804 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/fitting/classifier/data.py
+-rw-r--r--   0        0        0     1139 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/fitting/classifier/decision_tree.py
+-rw-r--r--   0        0        0      895 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/fitting/classifier/gaussian_process.py
+-rw-r--r--   0        0        0      801 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/fitting/classifier/linear_svm.py
+-rw-r--r--   0        0        0      737 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/fitting/classifier/naive_bayes.py
+-rw-r--r--   0        0        0     1675 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/fitting/classifier/qblox_fit.py
+-rw-r--r--   0        0        0     4500 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/fitting/classifier/qubit_fit.py
+-rw-r--r--   0        0        0     1241 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/fitting/classifier/random_forest.py
+-rw-r--r--   0        0        0     1133 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/fitting/classifier/rbf_svm.py
+-rw-r--r--   0        0        0     8095 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/fitting/classifier/run.py
+-rw-r--r--   0        0        0     1121 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/fitting/classifier/scikit_utils.py
+-rw-r--r--   0        0        0     5957 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/protocols/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/protocols/allxy/__init__.py
+-rw-r--r--   0        0        0     7998 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/protocols/allxy/allxy.py
+-rw-r--r--   0        0        0     4842 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/protocols/allxy/allxy_drag_pulse_tuning.py
+-rw-r--r--   0        0        0     5376 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/protocols/allxy/allxy_resonator_depletion_tuning.py
+-rw-r--r--   0        0        0    14319 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/protocols/classification.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/protocols/coherence/__init__.py
+-rw-r--r--   0        0        0     6245 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/protocols/coherence/spin_echo.py
+-rw-r--r--   0        0        0     6802 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/protocols/coherence/spin_echo_signal.py
+-rw-r--r--   0        0        0     6230 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/protocols/coherence/t1.py
+-rw-r--r--   0        0        0     3329 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/protocols/coherence/t1_sequences.py
+-rw-r--r--   0        0        0     6343 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/protocols/coherence/t1_signal.py
+-rw-r--r--   0        0        0     5411 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/protocols/coherence/t2.py
+-rw-r--r--   0        0        0     2551 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/protocols/coherence/t2_sequences.py
+-rw-r--r--   0        0        0     5492 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/protocols/coherence/t2_signal.py
+-rw-r--r--   0        0        0     3939 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/protocols/coherence/utils.py
+-rw-r--r--   0        0        0     5757 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/protocols/coherence/zeno.py
+-rw-r--r--   0        0        0     5676 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/protocols/coherence/zeno_signal.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/protocols/couplers/__init__.py
+-rw-r--r--   0        0        0     4905 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/protocols/couplers/coupler_chevron.py
+-rw-r--r--   0        0        0     4662 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/protocols/couplers/coupler_qubit_spectroscopy.py
+-rw-r--r--   0        0        0     5576 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/protocols/couplers/coupler_resonator_spectroscopy.py
+-rw-r--r--   0        0        0     2053 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/protocols/couplers/utils.py
+-rw-r--r--   0        0        0    10911 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/protocols/dispersive_shift.py
+-rw-r--r--   0        0        0     9481 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/protocols/dispersive_shift_qutrit.py
+-rw-r--r--   0        0        0     8688 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/protocols/drag.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/protocols/fast_reset/_init__.py
+-rw-r--r--   0        0        0     6879 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/protocols/fast_reset/fast_reset.py
+-rw-r--r--   0        0        0     9881 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/protocols/flipping.py
+-rw-r--r--   0        0        0    11074 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/protocols/flipping_signal.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/protocols/flux_dependence/__init__.py
+-rw-r--r--   0        0        0    11480 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/protocols/flux_dependence/avoided_crossing.py
+-rw-r--r--   0        0        0    12516 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/protocols/flux_dependence/qubit_crosstalk.py
+-rw-r--r--   0        0        0     8675 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/protocols/flux_dependence/qubit_flux_dependence.py
+-rw-r--r--   0        0        0     5406 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/protocols/flux_dependence/qubit_flux_tracking.py
+-rw-r--r--   0        0        0    13491 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/protocols/flux_dependence/resonator_crosstalk.py
+-rw-r--r--   0        0        0     9731 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/protocols/flux_dependence/resonator_flux_dependence.py
+-rw-r--r--   0        0        0    12108 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/protocols/flux_dependence/utils.py
+-rw-r--r--   0        0        0     5429 2024-05-23 09:00:58.860306 qibocal-0.0.9/src/qibocal/protocols/qubit_spectroscopy.py
+-rw-r--r--   0        0        0     6780 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/protocols/qubit_spectroscopy_ef.py
+-rw-r--r--   0        0        0     5681 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/protocols/qutrit_classification.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/protocols/rabi/__init__.py
+-rw-r--r--   0        0        0     5971 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/protocols/rabi/amplitude.py
+-rw-r--r--   0        0        0     6553 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/protocols/rabi/amplitude_signal.py
+-rw-r--r--   0        0        0     3760 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/protocols/rabi/ef.py
+-rw-r--r--   0        0        0     6727 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/protocols/rabi/length.py
+-rw-r--r--   0        0        0     2843 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/protocols/rabi/length_sequences.py
+-rw-r--r--   0        0        0     6712 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/protocols/rabi/length_signal.py
+-rw-r--r--   0        0        0     5819 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/protocols/rabi/utils.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/protocols/ramsey/__init__.py
+-rw-r--r--   0        0        0    10249 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/protocols/ramsey/ramsey.py
+-rw-r--r--   0        0        0     9650 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/protocols/ramsey/ramsey_signal.py
+-rw-r--r--   0        0        0     3351 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/protocols/ramsey/utils.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/protocols/randomized_benchmarking/__init__.py
+-rw-r--r--   0        0        0     2450 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/protocols/randomized_benchmarking/circuit_tools.py
+-rw-r--r--   0        0        0     3276 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/protocols/randomized_benchmarking/filtered_rb.py
+-rw-r--r--   0        0        0     7044 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/protocols/randomized_benchmarking/fitting.py
+-rw-r--r--   0        0        0     1808 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/protocols/randomized_benchmarking/noisemodels.py
+-rw-r--r--   0        0        0     8828 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/protocols/randomized_benchmarking/standard_rb.py
+-rw-r--r--   0        0        0    12715 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/protocols/randomized_benchmarking/utils.py
+-rw-r--r--   0        0        0    10473 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/protocols/readout_characterization.py
+-rw-r--r--   0        0        0     6968 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/protocols/readout_mitigation_matrix.py
+-rw-r--r--   0        0        0     7021 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/protocols/readout_optimization/resonator_amplitude.py
+-rw-r--r--   0        0        0     7529 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/protocols/readout_optimization/resonator_frequency.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/protocols/readout_optimization/twpa_calibration/__init__.py
+-rw-r--r--   0        0        0     6089 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/protocols/readout_optimization/twpa_calibration/frequency.py
+-rw-r--r--   0        0        0     8128 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/protocols/readout_optimization/twpa_calibration/frequency_SNR.py
+-rw-r--r--   0        0        0     7673 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/protocols/readout_optimization/twpa_calibration/frequency_power.py
+-rw-r--r--   0        0        0     5771 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/protocols/readout_optimization/twpa_calibration/power.py
+-rw-r--r--   0        0        0     7872 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/protocols/readout_optimization/twpa_calibration/power_SNR.py
+-rw-r--r--   0        0        0     8179 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/protocols/resonator_punchout.py
+-rw-r--r--   0        0        0     8166 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/protocols/resonator_punchout_attenuation.py
+-rw-r--r--   0        0        0     9025 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/protocols/resonator_spectroscopy.py
+-rw-r--r--   0        0        0     6928 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/protocols/signal_experiments/calibrate_state_discrimination.py
+-rw-r--r--   0        0        0     4689 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/protocols/signal_experiments/time_of_flight_readout.py
+-rw-r--r--   0        0        0     9526 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/protocols/state_tomography.py
+-rw-r--r--   0        0        0      178 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/protocols/two_qubit_interaction/__init__.py
+-rw-r--r--   0        0        0       72 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/protocols/two_qubit_interaction/chevron/__init__.py
+-rw-r--r--   0        0        0     9885 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/protocols/two_qubit_interaction/chevron/chevron.py
+-rw-r--r--   0        0        0     4255 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/protocols/two_qubit_interaction/chevron/chevron_signal.py
+-rw-r--r--   0        0        0     2291 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/protocols/two_qubit_interaction/chevron/utils.py
+-rw-r--r--   0        0        0       49 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/protocols/two_qubit_interaction/chsh/__init__.py
+-rw-r--r--   0        0        0     2970 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/protocols/two_qubit_interaction/chsh/circuits.py
+-rw-r--r--   0        0        0    12560 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/protocols/two_qubit_interaction/chsh/protocol.py
+-rw-r--r--   0        0        0     3269 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/protocols/two_qubit_interaction/chsh/pulses.py
+-rw-r--r--   0        0        0      872 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/protocols/two_qubit_interaction/chsh/utils.py
+-rw-r--r--   0        0        0    15529 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/protocols/two_qubit_interaction/cz_virtualz.py
+-rw-r--r--   0        0        0     4932 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/protocols/two_qubit_interaction/cz_virtualz_signal.py
+-rw-r--r--   0        0        0     2348 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/protocols/two_qubit_interaction/utils.py
+-rw-r--r--   0        0        0    23446 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/protocols/utils.py
+-rw-r--r--   0        0        0     7431 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/update.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/web/__init__.py
+-rw-r--r--   0        0        0     1010 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/web/report.py
+-rw-r--r--   0        0        0     4168 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/web/static/styles.css
+-rw-r--r--   0        0        0     8531 2024-05-23 09:00:58.864306 qibocal-0.0.9/src/qibocal/web/templates/template.html
+-rw-r--r--   0        0        0     4711 1970-01-01 00:00:00.000000 qibocal-0.0.9/PKG-INFO
```

### Comparing `qibocal-0.0.8/LICENSE` & `qibocal-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.8/README.md` & `qibocal-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -43,26 +43,25 @@
 This section shows the steps to perform a resonator spectroscopy with Qibocal.
 ### Write a runcard
 A runcard contains all the essential information to run a specific task.
 For our purposes, we can use the following:
 ```yml
 platform: tii1q
 
-qubits: [0]
+targets: [0]
 
 - id: resonator spectroscopy high power
-  priority: 0
   operation: resonator_spectroscopy
   parameters:
     freq_width: 10_000_000
     freq_step: 500_000
     amplitude: 0.4
     power_level: high
     nshots: 1024
-    relaxation_time: 0
+    relaxation_time: 5_000
 
 ```
 ### How to run protocols
 To run the protocols specified in the ```runcard```, Qibocal uses the `qq auto` command
 ```sh
 qq auto <runcard> -o <output_folder>
 ```
```

#### html2text {}

```diff
@@ -13,18 +13,18 @@
 cd qibocal pip install . ``` ### Developer instructions For development make
 sure to install the package using [`poetry`](https://python-poetry.org/) and to
 install the pre-commit hooks: ```sh git clone https://github.com/qiboteam/
 qibocal.git cd qibocal poetry install pre-commit install ``` ## Minimal working
 example This section shows the steps to perform a resonator spectroscopy with
 Qibocal. ### Write a runcard A runcard contains all the essential information
 to run a specific task. For our purposes, we can use the following: ```yml
-platform: tii1q qubits: [0] - id: resonator spectroscopy high power priority: 0
-operation: resonator_spectroscopy parameters: freq_width: 10_000_000 freq_step:
-500_000 amplitude: 0.4 power_level: high nshots: 1024 relaxation_time: 0 ```
-### How to run protocols To run the protocols specified in the ```runcard```,
+platform: tii1q targets: [0] - id: resonator spectroscopy high power operation:
+resonator_spectroscopy parameters: freq_width: 10_000_000 freq_step: 500_000
+amplitude: 0.4 power_level: high nshots: 1024 relaxation_time: 5_000 ``` ###
+How to run protocols To run the protocols specified in the ```runcard```,
 Qibocal uses the `qq auto` command ```sh qq auto -o ``` if `````` is specified,
 the results will be saved in it, otherwise ```qq``` will automatically create a
 default folder containing the current date and the username. ### Uploading
 reports to server In order to upload the report to a centralized server, send
 to the server administrators your public ssh key (from the machine(s) you are
 planning to upload the report) and then use the `qq upload ` command. This
 program will upload your report to the server and generate an unique URL. ##
```

### Comparing `qibocal-0.0.8/pyproject.toml` & `qibocal-0.0.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qibocal"
-version = "0.0.8"
+version = "0.0.9"
 description = "Qibo's quantum calibration, characterization and validation module."
 authors = ["andrea-pasquale <andreapasquale97@gmail.com>"]
 license = "Apache License 2.0"
 readme = "README.md"
 homepage = "https://qibo.science/"
 repository = "https://github.com/qiboteam/qibocal/"
 documentation = "https://qibo.science/qibocal/stable/"
@@ -13,28 +13,28 @@
   "Programming Language :: Python :: 3",
   "Topic :: Scientific/Engineering :: Physics",
 ]
 
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
-qibolab = "^0.1.6"
+qibolab = "^0.1.7"
 qibo ="^0.2.6"
 numpy = "^1.26.4"
 scipy = "^1.10.1"
 pandas = "^1.4.3"
 pydantic = "^1.10.5"
 click = "^8.1.3"
 jinja2 = "^3.1.2"
 plotly = "^5.15.0"
 dash = "^2.6.0"
 skops = "^0.6.0"
 scikit-learn = "^1.2.1"
 # Explicit dependency required to cope for dash: https://github.com/plotly/dash/issues/2557
-setuptools = "^67.8.0"
+setuptools = "^69.1.1"
 matplotlib = { version = "^3.7.0", optional = true }
 seaborn = { version = "^0.12.2", optional = true }
 pydot = { version = "^1.4.2", optional = true }
 skl2onnx = { version = "^1.14.0", optional = true }
 pyyaml = "^6.0"
 onnxruntime = { version = "^1.14.1", optional = true }
```

### Comparing `qibocal-0.0.8/src/qibocal/auto/execute.py` & `qibocal-0.0.9/src/qibocal/auto/execute.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,16 +22,14 @@
     """The execution history, with results and exit states."""
     output: Path
     """Output path."""
     targets: Targets
     """Qubits/Qubit Pairs to be calibrated."""
     platform: Platform
     """Qubits' platform."""
-    max_iterations: int
-    """Maximum number of iterations."""
     update: bool = True
     """Runcard update mechanism."""
 
     # TODO: find a more elegant way to pass everything
     @classmethod
     def load(
         cls,
@@ -42,15 +40,14 @@
         update: bool = True,
     ):
         """Load execution graph and associated executor from a runcard."""
 
         return cls(
             actions=card.actions,
             history=History({}),
-            max_iterations=card.max_iterations,
             output=output,
             platform=platform,
             targets=targets,
             update=update,
         )
 
     def run(self, mode):
@@ -58,24 +55,20 @@
 
         The platform's update method is called if:
         - self.update is True and task.update is None
         - task.update is True
         """
         for action in self.actions:
             task = Task(action)
-            task.iteration = self.history.iterations(task.id)
-            log.info(
-                f"Executing mode {mode.name} on {task.id} iteration {task.iteration}."
-            )
+            log.info(f"Executing mode {mode.name} on {task.id}.")
             completed = task.run(
-                max_iterations=self.max_iterations,
                 platform=self.platform,
                 targets=self.targets,
                 folder=self.output,
                 mode=mode,
             )
             self.history.push(completed)
 
             if mode.name in ["autocalibration", "fit"] and self.platform is not None:
                 completed.update_platform(platform=self.platform, update=self.update)
 
-            yield completed.task.uid
+            yield completed.task.id
```

### Comparing `qibocal-0.0.8/src/qibocal/auto/history.py` & `qibocal-0.0.9/src/qibocal/auto/history.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Track execution history."""
 
 from .runcard import Id
 from .task import Completed
 
 
 def add_timings_to_meta(meta, history):
-    for task_id, iteration in history:
-        completed = history[(task_id, iteration)]
+    for task_id in history:
+        completed = history[task_id]
         if task_id not in meta:
             meta[task_id] = {}
 
         if "acquisition" not in meta[task_id] and completed.data_time > 0:
             meta[task_id]["acquisition"] = completed.data_time
         if "fit" not in meta[task_id] and completed.results_time > 0:
             meta[task_id]["fit"] = completed.results_time
@@ -29,18 +29,10 @@
     of the execution itself, since later routines can retrieve the output of
     former ones from here.
 
     """
 
     def push(self, completed: Completed):
         """Adding completed task to history."""
-        self[completed.task.uid] = completed
-
-    def iterations(self, task_id: Id):
-        """Count task id present in history."""
-        counter = 0
-        for task, _ in self:
-            if task == task_id:
-                counter += 1
-        return counter
+        self[completed.task.id] = completed
 
     # TODO: implemet time_travel()
```

### Comparing `qibocal-0.0.8/src/qibocal/auto/operation.py` & `qibocal-0.0.9/src/qibocal/auto/operation.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from dataclasses import asdict, dataclass, fields
 from functools import wraps
 from pathlib import Path
 from typing import Callable, Generic, NewType, Optional, TypeVar, Union
 
 import numpy as np
 import numpy.typing as npt
+from qibolab import AcquisitionType, AveragingMode, ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.qubits import Qubit, QubitId, QubitPair, QubitPairId
 
 from qibocal.config import log
 
 from .serialize import deserialize, load, serialize
 
@@ -67,14 +68,18 @@
 
     """
 
     nshots: int
     """Number of executions on hardware"""
     relaxation_time: float
     """Wait time for the qubit to decohere back to the `gnd` state"""
+    hardware_average: bool = False
+    """By default hardware average will be performed."""
+    classify: bool = False
+    """By default qubit state classification will not be performed."""
 
     @classmethod
     def load(cls, input_parameters):
         """Load parameters from runcard.
 
         Possibly looking into previous steps outputs.
         Parameters defined in Parameters class are removed from `parameters`
@@ -92,14 +97,32 @@
         for parameter, value in default_parent_parameters.items():
             default_parent_parameters[parameter] = parameters.pop(parameter, value)
         instantiated_class = cls(**parameters)
         for parameter, value in default_parent_parameters.items():
             setattr(instantiated_class, parameter, value)
         return instantiated_class
 
+    @property
+    def execution_parameters(self):
+        """Default execution parameters."""
+        averaging_mode = (
+            AveragingMode.CYCLIC if self.hardware_average else AveragingMode.SINGLESHOT
+        )
+        acquisition_type = (
+            AcquisitionType.DISCRIMINATION
+            if self.classify
+            else AcquisitionType.INTEGRATION
+        )
+        return ExecutionParameters(
+            nshots=self.nshots,
+            relaxation_time=self.relaxation_time,
+            acquisition_type=acquisition_type,
+            averaging_mode=averaging_mode,
+        )
+
 
 class AbstractData:
     """Abstract data class."""
 
     def __init__(
         self, data: dict[Union[tuple[QubitId, int], QubitId], npt.NDArray] = None
     ):
@@ -193,17 +216,18 @@
 
         Args:
             data_keys (tuple): Keys of Data.data.
             data_dict (dict): The keys are the fields of `dtype` and
             the values are the related arrays.
         """
         # to be able to handle the non-sweeper case
-        ar = np.empty(np.shape(data_dict[list(data_dict.keys())[0]]), dtype=dtype)
+        ar = np.empty(np.shape(data_dict[list(data_dict)[0]]), dtype=dtype)
         for key, value in data_dict.items():
             ar[key] = value
+
         if data_keys in self.data:
             self.data[data_keys] = np.rec.array(
                 np.concatenate((self.data[data_keys], ar))
             )
         else:
             self.data[data_keys] = np.rec.array(ar)
```

### Comparing `qibocal-0.0.8/src/qibocal/auto/runcard.py` & `qibocal-0.0.9/src/qibocal/auto/runcard.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 """Specify runcard layout, handles (de)serialization."""
 
 import os
 from typing import Any, NewType, Optional, Union
 
 from pydantic.dataclasses import dataclass
-from qibo.backends import Backend, GlobalBackend
-from qibo.transpiler.pipeline import Passes
+from qibo.backends import GlobalBackend
+from qibo.backends.abstract import Backend
 from qibolab.platform import Platform
 from qibolab.qubits import QubitId, QubitPairId
 
 from .operation import OperationId
 
 Id = NewType("Id", str)
 """Action identifiers type."""
 
 Targets = Union[list[QubitId], list[QubitPairId], list[tuple[QubitId, ...]]]
 """Elements to be calibrated by a single protocol."""
 
-MAX_ITERATIONS = 5
-"""Default max iterations."""
-
 
 @dataclass(config=dict(smart_union=True))
 class Action:
     """Action specification in the runcard."""
 
     id: Id
     """Action unique identifier."""
@@ -51,30 +48,24 @@
     """Qubits to be calibrated.
        If `None` the protocols will be executed on all qubits
        available in the platform."""
     backend: str = "qibolab"
     """Qibo backend."""
     platform: str = os.environ.get("QIBO_PLATFORM", "dummy")
     """Qibolab platform."""
-    max_iterations: int = MAX_ITERATIONS
-    """Maximum number of iterations."""
 
     def __post_init__(self):
         if self.targets is None and self.platform_obj is not None:
             self.targets = list(self.platform_obj.qubits)
 
     @property
     def backend_obj(self) -> Backend:
         """Allocate backend."""
         GlobalBackend.set_backend(self.backend, platform=self.platform)
-        backend = GlobalBackend()
-        if backend.platform is not None:
-            backend.transpiler = Passes(connectivity=backend.platform.topology)
-            backend.transpiler.passes = backend.transpiler.passes[-1:]
-        return backend
+        return GlobalBackend()
 
     @property
     def platform_obj(self) -> Platform:
         """Allocate platform."""
         return self.backend_obj.platform
 
     @classmethod
```

### Comparing `qibocal-0.0.8/src/qibocal/auto/serialize.py` & `qibocal-0.0.9/src/qibocal/auto/serialize.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.8/src/qibocal/auto/status.py` & `qibocal-0.0.9/src/qibocal/auto/status.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.8/src/qibocal/auto/task.py` & `qibocal-0.0.9/src/qibocal/auto/task.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from pathlib import Path
 from statistics import mode
 from typing import Optional
 
 from qibolab.platform import Platform
 from qibolab.serialize import dump_platform
 
-from ..config import log, raise_error
-from ..protocols.characterization import Operation
+from ..config import log
+from ..protocols import Operation
 from .mode import ExecutionMode
 from .operation import Data, DummyPars, Results, Routine, dummy_operation
 from .runcard import Action, Id, Targets
 
 MAX_PRIORITY = int(1e9)
 """A number bigger than whatever will be manually typed. But not so insanely big not to fit in a native integer."""
 DEFAULT_NSHOTS = 100
@@ -25,33 +25,26 @@
 """Folder where platform will be dumped."""
 
 
 @dataclass
 class Task:
     action: Action
     """Action object parsed from Runcard."""
-    iteration: int = 0
-    """Task iteration."""
 
     @property
     def targets(self) -> Targets:
         """Protocol targets."""
         return self.action.targets
 
     @property
     def id(self) -> Id:
         """Task Id."""
         return self.action.id
 
     @property
-    def uid(self) -> TaskId:
-        """Task unique Id."""
-        return (self.action.id, self.iteration)
-
-    @property
     def operation(self):
         """Routine object from Operation Enum."""
         if self.action.operation is None:
             raise RuntimeError("No operation specified")
 
         return Operation[self.action.operation].value
 
@@ -63,25 +56,19 @@
     @property
     def update(self):
         """Local update parameter."""
         return self.action.update
 
     def run(
         self,
-        max_iterations: int,
         platform: Platform = None,
         targets: Targets = list,
         mode: ExecutionMode = None,
         folder: Path = None,
     ):
-        if self.iteration > max_iterations:
-            raise_error(
-                ValueError,
-                f"Maximum number of iterations {max_iterations} reached!",
-            )
 
         if self.targets is None:
             self.action.targets = targets
 
         completed = Completed(self, folder)
 
         try:
@@ -146,15 +133,15 @@
 
     def __post_init__(self):
         self.task = copy.deepcopy(self.task)
 
     @property
     def datapath(self):
         """Path contaning data and results file for task."""
-        path = self.folder / "data" / f"{self.task.id}_{self.task.iteration}"
+        path = self.folder / "data" / f"{self.task.id}"
         if not path.is_dir():
             path.mkdir(parents=True)
         return path
 
     @property
     def results(self):
         """Access task's results."""
```

### Comparing `qibocal-0.0.8/src/qibocal/cli/_base.py` & `qibocal-0.0.9/src/qibocal/cli/_base.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.8/src/qibocal/cli/acquisition.py` & `qibocal-0.0.9/src/qibocal/cli/acquisition.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 
     # dump action runcard
     (path / RUNCARD).write_text(yaml.safe_dump(asdict(runcard)))
     # dump meta
     (path / META).write_text(json.dumps(meta, indent=4))
 
     executor = Executor.load(runcard, path, platform, runcard.targets)
-
     # connect and initialize platform
     if platform is not None:
         platform.connect()
 
     # run protocols
     list(executor.run(mode=ExecutionMode.acquire))
```

### Comparing `qibocal-0.0.8/src/qibocal/cli/autocalibration.py` & `qibocal-0.0.9/src/qibocal/cli/autocalibration.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import yaml
 from qibolab.serialize import dump_platform
 
 from ..auto.execute import Executor
 from ..auto.history import add_timings_to_meta
 from ..auto.mode import ExecutionMode
-from ..cli.report import ReportBuilder
+from .report import report
 from .utils import (
     META,
     PLATFORM,
     RUNCARD,
     UPDATED_PLATFORM,
     generate_meta,
     generate_output_folder,
@@ -50,22 +50,21 @@
 
     # connect and initialize platform
     if platform is not None:
         platform.connect()
 
     # run protocols
     for _ in executor.run(mode=ExecutionMode.autocalibration):
-        report = ReportBuilder(path, runcard.targets, executor, meta, executor.history)
-        report.run(path)
-        # meta needs to be updated after each report to show correct end-time
+        # meta needs to be updated before each report to show correct end-time
         e = datetime.datetime.now(datetime.timezone.utc)
         meta["end-time"] = e.strftime("%H:%M:%S")
         # dump updated meta
         meta = add_timings_to_meta(meta, executor.history)
         (path / META).write_text(json.dumps(meta, indent=4))
+        report(path, executor)
 
     # stop and disconnect platform
     if platform is not None:
         platform.disconnect()
 
     # dump updated runcard
     if platform is not None:
```

### Comparing `qibocal-0.0.8/src/qibocal/cli/fit.py` & `qibocal-0.0.9/src/qibocal/cli/fit.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.8/src/qibocal/cli/report.py` & `qibocal-0.0.9/src/qibocal/cli/report.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,110 +1,106 @@
+import io
 import json
-import tempfile
-from functools import cached_property
-from pathlib import Path
+import pathlib
+from typing import Optional, Union
 
+import plotly.graph_objects as go
 import yaml
+from jinja2 import Environment, FileSystemLoader
 from qibo.backends import GlobalBackend
-from qibolab.qubits import QubitId
+from qibolab.qubits import QubitId, QubitPairId
 
 from qibocal.auto.execute import Executor
 from qibocal.auto.mode import ExecutionMode
 from qibocal.auto.runcard import Runcard
-from qibocal.auto.task import TaskId
+from qibocal.auto.task import Completed
+from qibocal.cli.utils import META, RUNCARD
 from qibocal.config import log
+from qibocal.web.report import STYLES, TEMPLATES, Report
 
-META = "meta.json"
-RUNCARD = "runcard.yml"
-UPDATED_PLATFORM = "new_platform.yml"
-PLATFORM = "platform.yml"
+ReportOutcome = tuple[str, list[go.Figure]]
+"""Report produced by protocol."""
 
 
-def generate_figures_and_report(node, target):
-    """Returns figures and table for report."""
+def generate_figures_and_report(
+    node: Completed, target: Union[QubitId, QubitPairId, list[QubitId]]
+) -> ReportOutcome:
+    """Calling protocol plot by checking if fit has been performed.
+
+    It operates on a completed `node` and a specific protocol `target`, generating
+    a report outcome (cf. `ReportOutcome`).
+    """
 
     if node.results is None:
         # plot acquisition data
         return node.task.operation.report(data=node.data, fit=None, target=target)
     if target not in node.results:
         # plot acquisition data and message for unsuccessful fit
         figures = node.task.operation.report(data=node.data, fit=None, target=target)[0]
         return figures, "An error occurred when performing the fit."
     # plot acquisition and fit
     return node.task.operation.report(data=node.data, fit=node.results, target=target)
 
 
-def report(path):
-    """Report generation
+def plotter(
+    node: Completed, target: Union[QubitId, QubitPairId, list[QubitId]]
+) -> tuple[str, str]:
+    """Run plotly pipeline for generating html.
+
+    Performs conversions of plotly figures in html rendered code for completed
+    node on specific target.
+
+    """
+    figures, fitting_report = generate_figures_and_report(node, target)
+    buffer = io.StringIO()
+    html_list = []
+    for figure in figures:
+        figure.write_html(buffer, include_plotlyjs=False, full_html=False)
+        buffer.seek(0)
+        html_list.append(buffer.read())
+    buffer.close()
+    all_html = "".join(html_list)
+    return all_html, fitting_report
 
-    Arguments:
 
-    - FOLDER: input folder.
+def report(path: pathlib.Path, executor: Optional[Executor] = None):
+    """Report generation.
 
+    Generates the report for protocol dumped in `path`.
+    Executor can be passed to generate report on the fly.
     """
+
     if path.exists():
         log.warning(f"Regenerating {path}/index.html")
     # load meta
     meta = json.loads((path / META).read_text())
     # load runcard
     runcard = Runcard.load(yaml.safe_load((path / RUNCARD).read_text()))
 
     # set backend, platform and qubits
     GlobalBackend.set_backend(backend=meta["backend"], platform=meta["platform"])
-    backend = GlobalBackend()
-    platform = backend.platform
 
     # load executor
-    executor = Executor.load(runcard, path, targets=runcard.targets)
-    # produce html
-    builder = ReportBuilder(path, runcard.targets, executor, meta)
-    builder.run(path)
-
-
-class ReportBuilder:
-    """Builder to produce html report."""
-
-    def __init__(self, path: Path, targets, executor: Executor, metadata, history=None):
-        self.path = self.title = path
-        self.targets = targets
-        self.executor = executor
-        self.metadata = metadata
-        self._history = history
-
-    @cached_property
-    def history(self):
-        if self._history is None:
-            list(self.executor.run(mode=ExecutionMode.report))
-            return self.executor.history
-        else:
-            return self._history
-
-    def routine_name(self, routine, iteration):
-        """Prettify routine's name for report headers."""
-        name = routine.replace("_", " ").title()
-        return f"{name} - {iteration}"
-
-    def routine_targets(self, task_id: TaskId):
-        """Get local targets parameter from Task if available otherwise use global one."""
-        local_targets = self.history[task_id].task.targets
-        return local_targets if len(local_targets) > 0 else self.targets
-
-    def single_qubit_plot(self, task_id: TaskId, qubit: QubitId):
-        """Generate single qubit plot."""
-        node = self.history[task_id]
-        figures, fitting_report = generate_figures_and_report(node, qubit)
-        with tempfile.NamedTemporaryFile(delete=False) as temp:
-            html_list = []
-            for figure in figures:
-                figure.write_html(temp.name, include_plotlyjs=False, full_html=False)
-                temp.seek(0)
-                fightml = temp.read().decode("utf-8")
-                html_list.append(fightml)
-
-        all_html = "".join(html_list)
-        return all_html, fitting_report
-
-    def run(self, path):
-        """Generation of html report."""
-        from qibocal.web.report import create_report
+    if executor is None:
+        executor = Executor.load(runcard, path, targets=runcard.targets)
+        # produce html
+        list(executor.run(mode=ExecutionMode.report))
+
+    css_styles = f"<style>\n{pathlib.Path(STYLES).read_text()}\n</style>"
+
+    env = Environment(loader=FileSystemLoader(TEMPLATES))
+    template = env.get_template("template.html")
+    html = template.render(
+        is_static=True,
+        css_styles=css_styles,
+        path=path,
+        title=path.name,
+        report=Report(
+            path=path,
+            targets=executor.targets,
+            history=executor.history,
+            meta=meta,
+            plotter=plotter,
+        ),
+    )
 
-        create_report(path, self)
+    (path / "index.html").write_text(html)
```

### Comparing `qibocal-0.0.8/src/qibocal/cli/upload.py` & `qibocal-0.0.9/src/qibocal/cli/upload.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.8/src/qibocal/cli/utils.py` & `qibocal-0.0.9/src/qibocal/cli/utils.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.8/src/qibocal/config.py` & `qibocal-0.0.9/src/qibocal/config.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.8/src/qibocal/fitting/classifier/ada_boost.py` & `qibocal-0.0.9/src/qibocal/fitting/classifier/ada_boost.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.8/src/qibocal/fitting/classifier/data.py` & `qibocal-0.0.9/src/qibocal/fitting/classifier/data.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.8/src/qibocal/fitting/classifier/decision_tree.py` & `qibocal-0.0.9/src/qibocal/fitting/classifier/decision_tree.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.8/src/qibocal/fitting/classifier/gaussian_process.py` & `qibocal-0.0.9/src/qibocal/fitting/classifier/gaussian_process.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.8/src/qibocal/fitting/classifier/linear_svm.py` & `qibocal-0.0.9/src/qibocal/fitting/classifier/linear_svm.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.8/src/qibocal/fitting/classifier/naive_bayes.py` & `qibocal-0.0.9/src/qibocal/fitting/classifier/naive_bayes.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.8/src/qibocal/fitting/classifier/qblox_fit.py` & `qibocal-0.0.9/src/qibocal/fitting/classifier/qblox_fit.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.8/src/qibocal/fitting/classifier/qubit_fit.py` & `qibocal-0.0.9/src/qibocal/fitting/classifier/qubit_fit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 from dataclasses import dataclass, field
 from math import atan2
 from pathlib import Path
 
 import numpy as np
 import numpy.typing as npt
 
-from qibocal.protocols.characterization.utils import (
-    cumulative,
-    effective_qubit_temperature,
-)
+from qibocal.protocols.utils import cumulative, effective_qubit_temperature
 
 
 def constructor(_hyperparams):
     r"""Return the model class.
 
     Args:
         _hyperparams: Model hyperparameters.
```

### Comparing `qibocal-0.0.8/src/qibocal/fitting/classifier/random_forest.py` & `qibocal-0.0.9/src/qibocal/fitting/classifier/random_forest.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.8/src/qibocal/fitting/classifier/rbf_svm.py` & `qibocal-0.0.9/src/qibocal/fitting/classifier/rbf_svm.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.8/src/qibocal/fitting/classifier/run.py` & `qibocal-0.0.9/src/qibocal/fitting/classifier/run.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.8/src/qibocal/fitting/classifier/scikit_utils.py` & `qibocal-0.0.9/src/qibocal/fitting/classifier/scikit_utils.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/__init__.py` & `qibocal-0.0.9/src/qibocal/protocols/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from enum import Enum
 
 from .allxy.allxy import allxy
+from .allxy.allxy_drag_pulse_tuning import allxy_drag_pulse_tuning
+from .allxy.allxy_resonator_depletion_tuning import allxy_resonator_depletion_tuning
 from .classification import single_shot_classification
 from .coherence.spin_echo import spin_echo
 from .coherence.spin_echo_signal import spin_echo_signal
 from .coherence.t1 import t1
 from .coherence.t1_sequences import t1_sequences
 from .coherence.t1_signal import t1_signal
 from .coherence.t2 import t2
@@ -34,14 +36,15 @@
 from .rabi.amplitude_signal import rabi_amplitude_signal
 from .rabi.ef import rabi_amplitude_ef
 from .rabi.length import rabi_length
 from .rabi.length_sequences import rabi_length_sequences
 from .rabi.length_signal import rabi_length_signal
 from .ramsey.ramsey import ramsey
 from .ramsey.ramsey_signal import ramsey_signal
+from .randomized_benchmarking.filtered_rb import filtered_rb
 from .randomized_benchmarking.standard_rb import standard_rb
 from .readout_characterization import readout_characterization
 from .readout_mitigation_matrix import readout_mitigation_matrix
 from .readout_optimization.resonator_amplitude import resonator_amplitude
 from .readout_optimization.resonator_frequency import resonator_frequency
 from .readout_optimization.twpa_calibration.frequency import twpa_frequency
 from .readout_optimization.twpa_calibration.frequency_power import twpa_frequency_power
@@ -51,14 +54,15 @@
 from .resonator_punchout import resonator_punchout
 from .resonator_punchout_attenuation import resonator_punchout_attenuation
 from .resonator_spectroscopy import resonator_spectroscopy
 from .signal_experiments.calibrate_state_discrimination import (
     calibrate_state_discrimination,
 )
 from .signal_experiments.time_of_flight_readout import time_of_flight_readout
+from .state_tomography import state_tomography
 from .two_qubit_interaction import (
     chevron,
     chevron_signal,
     chsh_circuits,
     chsh_pulses,
     cz_virtualz,
     cz_virtualz_signal,
@@ -89,27 +93,30 @@
     t2_signal = t2_signal
     t2_sequences = t2_sequences
     time_of_flight_readout = time_of_flight_readout
     single_shot_classification = single_shot_classification
     spin_echo = spin_echo
     spin_echo_signal = spin_echo_signal
     allxy = allxy
+    allxy_drag_pulse_tuning = allxy_drag_pulse_tuning
     drag_tuning = drag_tuning
+    allxy_resonator_depletion_tuning = allxy_resonator_depletion_tuning
     flipping = flipping
     dispersive_shift = dispersive_shift
     chevron = chevron
     chevron_signal = chevron_signal
     cz_virtualz = cz_virtualz
     standard_rb = standard_rb
-    readout_characterization = readout_characterization
+    filtered_rb = filtered_rb
     resonator_frequency = resonator_frequency
     fast_reset = fast_reset
     zeno = zeno
     zeno_signal = zeno_signal
     chsh_pulses = chsh_pulses
+    readout_characterization = readout_characterization
     chsh_circuits = chsh_circuits
     readout_mitigation_matrix = readout_mitigation_matrix
     twpa_frequency = twpa_frequency
     twpa_frequency_SNR = twpa_frequency_snr
     twpa_power = twpa_power
     twpa_power_SNR = twpa_power_snr
     twpa_frequency_power = twpa_frequency_power
@@ -121,7 +128,8 @@
     dispersive_shift_qutrit = dispersive_shift_qutrit
     coupler_resonator_spectroscopy = coupler_resonator_spectroscopy
     coupler_qubit_spectroscopy = coupler_qubit_spectroscopy
     cz_virtualz_signal = cz_virtualz_signal
     coupler_chevron = coupler_chevron
     flipping_signal = flipping_signal
     calibrate_state_discrimination = calibrate_state_discrimination
+    state_tomography = state_tomography
```

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/allxy/allxy.py` & `qibocal-0.0.9/src/qibocal/protocols/allxy/allxy.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 
 @dataclass
 class AllXYResults(Results):
     """AllXY outputs."""
 
 
-AllXYType = np.dtype([("prob", np.float64), ("gate", "<U5")])
+AllXYType = np.dtype([("prob", np.float64), ("gate", "<U5"), ("errors", np.float64)])
 
 
 @dataclass
 class AllXYData(Data):
     """AllXY acquisition outputs."""
 
     beta_param: float = None
@@ -85,15 +85,15 @@
     # for iteration in range(params.software_averages):
     sequences, all_ro_pulses = [], []
     for gates in gatelist:
         sequences.append(PulseSequence())
         all_ro_pulses.append({})
         for qubit in targets:
             sequences[-1], all_ro_pulses[-1][qubit] = add_gate_pair_pulses_to_sequence(
-                platform, gates, qubit, sequences[-1], params.beta_param
+                platform, gates, qubit, sequences[-1], beta_param=params.beta_param
             )
 
     # execute the pulse sequence
     options = ExecutionParameters(
         nshots=params.nshots, averaging_mode=AveragingMode.CYCLIC
     )
     if params.unrolling:
@@ -104,75 +104,83 @@
         ]
 
     for ig, (gates, ro_pulses) in enumerate(zip(gatelist, all_ro_pulses)):
         gate = "-".join(gates)
         for qubit in targets:
             serial = ro_pulses[qubit].serial
             if params.unrolling:
-                z_proj = 2 * results[serial][ig].probability(0) - 1
+                prob = results[serial][ig].probability(0)
+                z_proj = 2 * prob - 1
             else:
-                z_proj = 2 * results[ig][serial].probability(0) - 1
+                prob = results[ig][serial].probability(0)
+                z_proj = 2 * prob - 1
+
+            errors = 2 * np.sqrt(prob * (1 - prob) / params.nshots)
             data.register_qubit(
-                AllXYType, (qubit), dict(prob=np.array([z_proj]), gate=np.array([gate]))
+                AllXYType,
+                (qubit),
+                dict(
+                    prob=np.array([z_proj]),
+                    gate=np.array([gate]),
+                    errors=np.array([errors]),
+                ),
             )
 
     # finally, save the remaining data
     return data
 
 
 def add_gate_pair_pulses_to_sequence(
     platform: Platform,
     gates,
     qubit,
     sequence,
+    sequence_delay=0,
+    readout_delay=0,
     beta_param=None,
 ):
     pulse_duration = platform.create_RX_pulse(qubit, start=0).duration
     # All gates have equal pulse duration
 
-    sequenceDuration = 0
-    pulse_start = 0
+    sequence_duration = sequence.get_qubit_pulses(qubit).duration + sequence_delay
+    pulse_start = sequence.get_qubit_pulses(qubit).duration + sequence_delay
 
     for gate in gates:
         if gate == "I":
-            # print("Transforming to sequence I gate")
             pass
 
         if gate == "Xp":
-            # print("Transforming to sequence Xp gate")
             if beta_param == None:
                 RX_pulse = platform.create_RX_pulse(
                     qubit,
                     start=pulse_start,
                 )
             else:
                 RX_pulse = platform.create_RX_drag_pulse(
                     qubit,
                     start=pulse_start,
                     beta=beta_param,
                 )
             sequence.add(RX_pulse)
 
         if gate == "X9":
-            # print("Transforming to sequence X9 gate")
             if beta_param == None:
                 RX90_pulse = platform.create_RX90_pulse(
                     qubit,
                     start=pulse_start,
                 )
             else:
                 RX90_pulse = platform.create_RX90_drag_pulse(
                     qubit,
                     start=pulse_start,
                     beta=beta_param,
                 )
             sequence.add(RX90_pulse)
 
         if gate == "Yp":
-            # print("Transforming to sequence Yp gate")
             if beta_param == None:
                 RY_pulse = platform.create_RX_pulse(
                     qubit,
                     start=pulse_start,
                     relative_phase=np.pi / 2,
                 )
             else:
@@ -181,15 +189,14 @@
                     start=pulse_start,
                     relative_phase=np.pi / 2,
                     beta=beta_param,
                 )
             sequence.add(RY_pulse)
 
         if gate == "Y9":
-            # print("Transforming to sequence Y9 gate")
             if beta_param == None:
                 RY90_pulse = platform.create_RX90_pulse(
                     qubit,
                     start=pulse_start,
                     relative_phase=np.pi / 2,
                 )
             else:
@@ -197,19 +204,22 @@
                     qubit,
                     start=pulse_start,
                     relative_phase=np.pi / 2,
                     beta=beta_param,
                 )
             sequence.add(RY90_pulse)
 
-        sequenceDuration = sequenceDuration + pulse_duration
-        pulse_start = pulse_duration
+        sequence_duration += pulse_duration
+        pulse_start = sequence_duration
 
     # RO pulse starting just after pair of gates
-    ro_pulse = platform.create_qubit_readout_pulse(qubit, start=sequenceDuration + 4)
+    ro_pulse = platform.create_qubit_readout_pulse(
+        qubit, start=sequence_duration + readout_delay
+    )
+
     sequence.add(ro_pulse)
     return sequence, ro_pulse
 
 
 def _fit(_data: AllXYData) -> AllXYResults:
     """Post-Processing for allXY"""
     return AllXYResults()
@@ -220,19 +230,27 @@
     """Plotting function for allXY."""
 
     figures = []
     fitting_report = ""
     fig = go.Figure()
 
     qubit_data = data[target]
+    error_bars = qubit_data.errors
+    probs = qubit_data.prob
+    gates = qubit_data.gate
 
     fig.add_trace(
         go.Scatter(
-            x=qubit_data.gate,
-            y=qubit_data.prob,
+            x=gates,
+            y=probs,
+            error_y=dict(
+                type="data",
+                array=error_bars,
+                visible=True,
+            ),
             mode="markers",
             text=gatelist,
             textposition="bottom center",
             name="Expectation value",
             showlegend=True,
             legendgroup="group1",
         ),
```

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/allxy/allxy_drag_pulse_tuning.py` & `qibocal-0.0.9/src/qibocal/protocols/allxy/allxy_drag_pulse_tuning.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/classification.py` & `qibocal-0.0.9/src/qibocal/protocols/classification.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from qibolab.qubits import QubitId
 from sklearn.metrics import roc_auc_score, roc_curve
 
 from qibocal import update
 from qibocal.auto.operation import RESULTSFILE, Data, Parameters, Results, Routine
 from qibocal.auto.serialize import serialize
 from qibocal.fitting.classifier import run
-from qibocal.protocols.characterization.utils import (
+from qibocal.protocols.utils import (
     LEGEND_FONT_SIZE,
     MESH_SIZE,
     TITLE_SIZE,
     evaluate_grid,
     format_error_single_cell,
     get_color_state0,
     plot_results,
```

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/coherence/spin_echo.py` & `qibocal-0.0.9/src/qibocal/protocols/coherence/spin_echo.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,16 +83,16 @@
     data = SpinEchoData()
     sequences, all_ro_pulses = [], []
     # sweep the parameter
     for wait in ro_wait_range:
         # save data as often as defined by points
 
         for qubit in targets:
-            RX_pulses[qubit].start = RX90_pulses1[qubit].finish + wait // 2
-            RX90_pulses2[qubit].start = RX_pulses[qubit].finish + wait // 2
+            RX_pulses[qubit].start = RX90_pulses1[qubit].finish + wait / 2
+            RX90_pulses2[qubit].start = RX_pulses[qubit].finish + wait / 2
             ro_pulses[qubit].start = RX90_pulses2[qubit].finish
 
         sequences.append(deepcopy(sequence))
         all_ro_pulses.append(deepcopy(sequence).ro_pulses)
 
     if params.unrolling:
         results = platform.execute_pulse_sequences(sequences, options)
```

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/coherence/spin_echo_signal.py` & `qibocal-0.0.9/src/qibocal/protocols/coherence/spin_echo_signal.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,16 +98,16 @@
     sequences, all_ro_pulses = [], []
 
     # sweep the parameter
     for wait in ro_wait_range:
         # save data as often as defined by points
 
         for qubit in targets:
-            RX_pulses[qubit].start = RX90_pulses1[qubit].finish + wait // 2
-            RX90_pulses2[qubit].start = RX_pulses[qubit].finish + wait // 2
+            RX_pulses[qubit].start = RX90_pulses1[qubit].finish + wait / 2
+            RX90_pulses2[qubit].start = RX_pulses[qubit].finish + wait / 2
             ro_pulses[qubit].start = RX90_pulses2[qubit].finish
 
         sequences.append(deepcopy(sequence))
         all_ro_pulses.append(deepcopy(sequence).ro_pulses)
 
     if params.unrolling:
         results = platform.execute_pulse_sequences(sequences, options)
```

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/coherence/t1.py` & `qibocal-0.0.9/src/qibocal/protocols/coherence/t1.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/coherence/t1_sequences.py` & `qibocal-0.0.9/src/qibocal/protocols/coherence/t1_sequences.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/coherence/t1_signal.py` & `qibocal-0.0.9/src/qibocal/protocols/coherence/t1_signal.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/coherence/t2.py` & `qibocal-0.0.9/src/qibocal/protocols/coherence/t2.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/coherence/t2_sequences.py` & `qibocal-0.0.9/src/qibocal/protocols/coherence/t2_sequences.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/coherence/t2_signal.py` & `qibocal-0.0.9/src/qibocal/protocols/coherence/t2_signal.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/coherence/utils.py` & `qibocal-0.0.9/src/qibocal/protocols/coherence/utils.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/coherence/zeno.py` & `qibocal-0.0.9/src/qibocal/protocols/coherence/zeno.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/coherence/zeno_signal.py` & `qibocal-0.0.9/src/qibocal/protocols/coherence/zeno_signal.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/couplers/coupler_chevron.py` & `qibocal-0.0.9/src/qibocal/protocols/couplers/coupler_chevron.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/couplers/coupler_qubit_spectroscopy.py` & `qibocal-0.0.9/src/qibocal/protocols/couplers/coupler_qubit_spectroscopy.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitPairId
 from qibolab.sweeper import Parameter, Sweeper, SweeperType
 
 from qibocal.auto.operation import Routine
 
-from ..flux_dependence import resonator_flux_dependence
 from ..two_qubit_interaction.utils import order_pair
 from .coupler_resonator_spectroscopy import _fit, _plot, _update
 from .utils import CouplerSpectroscopyData, CouplerSpectroscopyParameters
 
 
 class CouplerSpectroscopyParametersQubit(CouplerSpectroscopyParameters):
     drive_duration: Optional[int] = 2000
@@ -44,21 +43,24 @@
 
     if params.measured_qubits is None:
         params.measured_qubits = [order_pair(pair, platform)[0] for pair in targets]
 
     sequence = PulseSequence()
     ro_pulses = {}
     qd_pulses = {}
+    offset = {}
     couplers = []
     for i, pair in enumerate(targets):
         ordered_pair = order_pair(pair, platform)
         measured_qubit = params.measured_qubits[i]
 
         qubit = platform.qubits[measured_qubit].name
-        couplers.append(platform.pairs[tuple(sorted(ordered_pair))].coupler)
+        offset[qubit] = platform.pairs[tuple(sorted(ordered_pair))].coupler.sweetspot
+        coupler = platform.pairs[tuple(sorted(ordered_pair))].coupler.name
+        couplers.append(coupler)
 
         ro_pulses[qubit] = platform.create_qubit_readout_pulse(
             qubit, start=params.drive_duration
         )
         qd_pulses[qubit] = platform.create_qubit_drive_pulse(
             qubit, start=0, duration=params.drive_duration
         )
@@ -66,47 +68,39 @@
             qd_pulses[qubit].amplitude = params.amplitude
 
         sequence.add(qd_pulses[qubit])
         sequence.add(ro_pulses[qubit])
 
     # define the parameter to sweep and its range:
     delta_frequency_range = np.arange(
-        -params.freq_width // 2, params.freq_width // 2, params.freq_step
+        -params.freq_width / 2, params.freq_width / 2, params.freq_step
     )
 
     sweeper_freq = Sweeper(
         Parameter.frequency,
         delta_frequency_range,
         pulses=[qd_pulses[qubit] for qubit in params.measured_qubits],
         type=SweeperType.OFFSET,
     )
 
-    if params.flux_pulses:
-        (
-            delta_bias_flux_range,
-            sweepers,
-        ) = resonator_flux_dependence.create_flux_pulse_sweepers(
-            params, platform, couplers, sequence
-        )
-    else:
-        delta_bias_flux_range = np.arange(
-            -params.bias_width / 2, params.bias_width / 2, params.bias_step
+    delta_bias_range = np.arange(
+        -params.bias_width / 2, params.bias_width / 2, params.bias_step
+    )
+    sweepers = [
+        Sweeper(
+            Parameter.bias,
+            delta_bias_range,
+            qubits=couplers,
+            type=SweeperType.OFFSET,
         )
-        sweepers = [
-            Sweeper(
-                Parameter.bias,
-                delta_bias_flux_range,
-                qubits=couplers,
-                type=SweeperType.OFFSET,
-            )
-        ]
+    ]
 
     data = CouplerSpectroscopyData(
         resonator_type=platform.resonator_type,
-        flux_pulses=params.flux_pulses,
+        offset=offset,
     )
 
     for bias_sweeper in sweepers:
         results = platform.sweep(
             sequence,
             ExecutionParameters(
                 nshots=params.nshots,
@@ -125,14 +119,14 @@
         result = results[ro_pulses[qubit].serial]
         # store the results
         data.register_qubit(
             qubit,
             signal=result.magnitude,
             phase=result.phase,
             freq=delta_frequency_range + qd_pulses[qubit].frequency,
-            bias=delta_bias_flux_range,
+            bias=delta_bias_range,
         )
     return data
 
 
 coupler_qubit_spectroscopy = Routine(_acquisition, _fit, _plot, _update)
 """CouplerQubitSpectroscopy Routine object."""
```

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/couplers/coupler_resonator_spectroscopy.py` & `qibocal-0.0.9/src/qibocal/protocols/couplers/coupler_resonator_spectroscopy.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitPairId
 from qibolab.sweeper import Parameter, Sweeper, SweeperType
 
 from qibocal.auto.operation import Routine
 
-from ..flux_dependence import resonator_flux_dependence
 from ..flux_dependence.utils import flux_dependence_plot
 from ..two_qubit_interaction.utils import order_pair
 from .utils import (
     CouplerSpectroscopyData,
     CouplerSpectroscopyParameters,
     CouplerSpectroscopyResults,
 )
@@ -39,65 +38,58 @@
     # Coupler pulse while MZ
 
     if params.measured_qubits is None:
         params.measured_qubits = [order_pair(pair, platform)[0] for pair in targets]
 
     sequence = PulseSequence()
     ro_pulses = {}
+    offset = {}
     couplers = []
     for i, pair in enumerate(targets):
         ordered_pair = order_pair(pair, platform)
         measured_qubit = params.measured_qubits[i]
 
         qubit = platform.qubits[measured_qubit].name
-        coupler = platform.pairs[tuple(sorted(ordered_pair))].coupler
+        offset[qubit] = platform.pairs[tuple(sorted(ordered_pair))].coupler.sweetspot
+        coupler = platform.pairs[tuple(sorted(ordered_pair))].coupler.name
         couplers.append(coupler)
         # TODO: May measure both qubits on the pair
         ro_pulses[qubit] = platform.create_qubit_readout_pulse(qubit, start=0)
         if params.amplitude is not None:
             ro_pulses[qubit].amplitude = params.amplitude
 
         sequence.add(ro_pulses[qubit])
 
     # define the parameter to sweep and its range:
     delta_frequency_range = np.arange(
-        -params.freq_width // 2, params.freq_width // 2, params.freq_step
+        -params.freq_width / 2, params.freq_width / 2, params.freq_step
     )
 
     sweeper_freq = Sweeper(
         Parameter.frequency,
         delta_frequency_range,
         pulses=[ro_pulses[qubit] for qubit in params.measured_qubits],
         type=SweeperType.OFFSET,
     )
 
-    if params.flux_pulses:
-        # TODO: Add delay
-        (
-            delta_bias_flux_range,
-            sweepers,
-        ) = resonator_flux_dependence.create_flux_pulse_sweepers(
-            params, platform, couplers, sequence
-        )
-    else:
-        delta_bias_flux_range = np.arange(
-            -params.bias_width / 2, params.bias_width / 2, params.bias_step
+    delta_bias_range = np.arange(
+        -params.bias_width / 2, params.bias_width / 2, params.bias_step
+    )
+    sweepers = [
+        Sweeper(
+            Parameter.bias,
+            delta_bias_range,
+            qubits=couplers,
+            type=SweeperType.OFFSET,
         )
-        sweepers = [
-            Sweeper(
-                Parameter.bias,
-                delta_bias_flux_range,
-                qubits=couplers,
-                type=SweeperType.OFFSET,
-            )
-        ]
+    ]
 
     data = CouplerSpectroscopyData(
         resonator_type=platform.resonator_type,
-        flux_pulses=params.flux_pulses,
+        offset=offset,
     )
 
     for bias_sweeper in sweepers:
         results = platform.sweep(
             sequence,
             ExecutionParameters(
                 nshots=params.nshots,
@@ -116,15 +108,15 @@
         result = results[ro_pulses[qubit].serial]
         # store the results
         data.register_qubit(
             qubit,
             signal=result.magnitude,
             phase=result.phase,
             freq=delta_frequency_range + ro_pulses[qubit].frequency,
-            bias=delta_bias_flux_range,
+            bias=delta_bias_range,
         )
     return data
 
 
 def _fit(data: CouplerSpectroscopyData) -> CouplerSpectroscopyResults:
     """Post-processing function for CouplerResonatorSpectroscopy."""
     qubits = data.qubits
```

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/couplers/utils.py` & `qibocal-0.0.9/src/qibocal/protocols/couplers/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,16 +47,16 @@
 
 @dataclass
 class CouplerSpectroscopyData(Data):
     """Data structure for CouplerResonatorSpectroscopy or CouplerQubitSpectroscopy."""
 
     resonator_type: str
     """Resonator type."""
-    flux_pulses: bool
-    """True if sweeping flux pulses, False if sweeping bias."""
+    offset: dict[QubitId, float] = field(default_factory=dict)
+    """Qubit bias offset."""
     data: dict[QubitId, npt.NDArray[CouplerSpecType]] = field(default_factory=dict)
     """Raw data acquired."""
 
     def register_qubit(self, qubit, freq, bias, signal, phase):
         """Store output for single qubit."""
         self.data[qubit] = create_data_array(
             freq, bias, signal, phase, dtype=CouplerSpecType
```

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/dispersive_shift.py` & `qibocal-0.0.9/src/qibocal/protocols/dispersive_shift.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
 from qibolab.sweeper import Parameter, Sweeper, SweeperType
 
 from qibocal import update
 from qibocal.auto.operation import Data, Parameters, Results, Routine
-from qibocal.protocols.characterization.utils import (
+from qibocal.protocols.utils import (
     HZ_TO_GHZ,
     lorentzian,
     lorentzian_fit,
     table_dict,
     table_html,
 )
 
@@ -109,15 +109,15 @@
         )
         sequence_0.add(ro_pulses[qubit])
         sequence_1.add(qd_pulses[qubit])
         sequence_1.add(ro_pulses[qubit])
 
     # define the parameter to sweep and its range:
     delta_frequency_range = np.arange(
-        -params.freq_width // 2, params.freq_width // 2, params.freq_step
+        -params.freq_width / 2, params.freq_width / 2, params.freq_step
     )
 
     # create a DataUnits objects to store the results
     data = DispersiveShiftData(resonator_type=platform.resonator_type)
     sweeper = Sweeper(
         Parameter.frequency,
         delta_frequency_range,
@@ -134,27 +134,22 @@
             averaging_mode=AveragingMode.CYCLIC,
         ),
         sweeper,
     )
 
     results_1 = platform.sweep(
         sequence_1,
-        ExecutionParameters(
-            nshots=params.nshots,
-            relaxation_time=params.relaxation_time,
-            acquisition_type=AcquisitionType.INTEGRATION,
-            averaging_mode=AveragingMode.CYCLIC,
-        ),
+        params.execution_parameters,
         sweeper,
     )
 
     # retrieve the results for every qubit
     for qubit in targets:
         for i, results in enumerate([results_0, results_1]):
-            result = results[ro_pulses[qubit].serial]
+            result = results[ro_pulses[qubit].serial].average
             # store the results
             data.register_qubit(
                 DispersiveShiftType,
                 (qubit, i),
                 dict(
                     freq=ro_pulses[qubit].frequency + delta_frequency_range,
                     signal=result.magnitude,
```

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/dispersive_shift_qutrit.py` & `qibocal-0.0.9/src/qibocal/protocols/dispersive_shift_qutrit.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from qibolab import AcquisitionType, AveragingMode, ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
 from qibolab.sweeper import Parameter, Sweeper, SweeperType
 
 from qibocal.auto.operation import Results, Routine
-from qibocal.protocols.characterization.utils import (
+from qibocal.protocols.utils import (
     GHZ_TO_HZ,
     HZ_TO_GHZ,
     lorentzian,
     lorentzian_fit,
     table_dict,
     table_html,
 )
@@ -101,15 +101,15 @@
         for sequence in [sequence_0, sequence_1, sequence_2]:
             readout_pulse = deepcopy(ro_pulse)
             readout_pulse.start = sequence.qd_pulses.finish
             sequence.add(readout_pulse)
 
     # define the parameter to sweep and its range:
     delta_frequency_range = np.arange(
-        -params.freq_width // 2, params.freq_width // 2, params.freq_step
+        -params.freq_width / 2, params.freq_width / 2, params.freq_step
     )
 
     data = DispersiveShiftQutritData(resonator_type=platform.resonator_type)
 
     for state, sequence in enumerate([sequence_0, sequence_1, sequence_2]):
         sweeper = Sweeper(
             Parameter.frequency,
@@ -126,15 +126,15 @@
                 acquisition_type=AcquisitionType.INTEGRATION,
                 averaging_mode=AveragingMode.CYCLIC,
             ),
             sweeper,
         )
 
         for qubit in targets:
-            result = results[qubit]
+            result = results[qubit].average
             # store the results
             data.register_qubit(
                 ResSpecType,
                 (qubit, state),
                 dict(
                     freq=sequence.get_qubit_pulses(qubit).ro_pulses[0].frequency
                     + delta_frequency_range,
```

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/drag.py` & `qibocal-0.0.9/src/qibocal/protocols/drag.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/fast_reset/fast_reset.py` & `qibocal-0.0.9/src/qibocal/protocols/fast_reset/fast_reset.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from plotly.subplots import make_subplots
 from qibolab import ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
 
 from qibocal.auto.operation import Data, Parameters, Results, Routine
-from qibocal.protocols.characterization.utils import table_dict, table_html
+from qibocal.protocols.utils import table_dict, table_html
 
 # TODO: IBM Fast Reset until saturation loop
 # https://quantum-computing.ibm.com/lab/docs/iql/manage/systems/reset/backend_reset
 
 
 @dataclass
 class FastResetParameters(Parameters):
```

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/flipping.py` & `qibocal-0.0.9/src/qibocal/protocols/flipping.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,41 +5,35 @@
 import numpy.typing as npt
 import plotly.graph_objects as go
 from qibolab import AcquisitionType, AveragingMode, ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
 from scipy.optimize import curve_fit
+from scipy.signal import find_peaks
 
 from qibocal.auto.operation import Routine
 from qibocal.config import log
-from qibocal.protocols.characterization.utils import table_dict, table_html
+from qibocal.protocols.utils import table_dict, table_html
 
 from .flipping_signal import (
     FlippingSignalData,
     FlippingSignalParameters,
     FlippingSignalResults,
     _update,
     flipping_fit,
+    flipping_sequence,
 )
 from .utils import COLORBAND, COLORBAND_LINE, chi2_reduced
 
 
 @dataclass
 class FlippingParameters(FlippingSignalParameters):
     """Flipping runcard inputs."""
 
-    nflips_max: int
-    """Maximum number of flips ([RX(pi) - RX(pi)] sequences). """
-    nflips_step: int
-    """Flip step."""
-    unrolling: bool = False
-    """If ``True`` it uses sequence unrolling to deploy multiple sequences in a single instrument call.
-    Defaults to ``False``."""
-
 
 @dataclass
 class FlippingResults(FlippingSignalResults):
     """Flipping outputs."""
 
     chi2: dict[QubitId, tuple[float, Optional[float]]] = field(default_factory=dict)
     """Chi squared estimate mean value and error. """
@@ -50,15 +44,14 @@
 )
 
 
 @dataclass
 class FlippingData(FlippingSignalData):
     """Flipping acquisition outputs."""
 
-    """Pi pulse amplitudes for each qubit."""
     data: dict[QubitId, npt.NDArray[FlippingType]] = field(default_factory=dict)
     """Raw data acquired."""
 
 
 def _acquisition(
     params: FlippingParameters,
     platform: Platform,
@@ -77,14 +70,15 @@
 
     Returns:
         data (:class:`FlippingData`)
     """
 
     data = FlippingData(
         resonator_type=platform.resonator_type,
+        detuning=params.detuning,
         pi_pulse_amplitudes={
             qubit: platform.qubits[qubit].native_gates.RX.amplitude for qubit in targets
         },
     )
 
     options = ExecutionParameters(
         nshots=params.nshots,
@@ -95,47 +89,34 @@
 
     # sweep the parameter
     sequences, all_ro_pulses = [], []
     flips_sweep = range(0, params.nflips_max, params.nflips_step)
     for flips in flips_sweep:
         # create a sequence of pulses for the experiment
         sequence = PulseSequence()
-        ro_pulses = {}
         for qubit in targets:
-            RX90_pulse = platform.create_RX90_pulse(qubit, start=0)
-            sequence.add(RX90_pulse)
-            # execute sequence RX(pi/2) - [RX(pi) - RX(pi)] from 0...flips times - RO
-            start1 = RX90_pulse.duration
-            for _ in range(flips):
-                RX_pulse1 = platform.create_RX_pulse(qubit, start=start1)
-                start2 = start1 + RX_pulse1.duration
-                RX_pulse2 = platform.create_RX_pulse(qubit, start=start2)
-                sequence.add(RX_pulse1)
-                sequence.add(RX_pulse2)
-                start1 = start2 + RX_pulse2.duration
-
-            # add ro pulse at the end of the sequence
-            ro_pulses[qubit] = platform.create_qubit_readout_pulse(qubit, start=start1)
-            sequence.add(ro_pulses[qubit])
+            sequence += flipping_sequence(
+                platform=platform, qubit=qubit, detuning=params.detuning, flips=flips
+            )
 
         sequences.append(sequence)
-        all_ro_pulses.append(ro_pulses)
+        all_ro_pulses.append(sequence.ro_pulses)
 
     # execute the pulse sequence
     if params.unrolling:
         results = platform.execute_pulse_sequences(sequences, options)
 
     elif not params.unrolling:
         results = [
             platform.execute_pulse_sequence(sequence, options) for sequence in sequences
         ]
 
     for ig, (flips, ro_pulses) in enumerate(zip(flips_sweep, all_ro_pulses)):
         for qubit in targets:
-            serial = ro_pulses[qubit].serial
+            serial = ro_pulses.get_qubit_pulses(qubit)[0].serial
             if params.unrolling:
                 result = results[serial][0]
             else:
                 result = results[ig][serial]
             prob = result.probability(state=1)
             error = np.sqrt(prob * (1 - prob) / params.nshots)
             data.register_qubit(
@@ -159,22 +140,37 @@
     .. math::
 
         y = p_0 sin\Big(\frac{2 \pi x}{p_2} + p_3\Big) + p_1.
     """
     qubits = data.qubits
     corrected_amplitudes = {}
     fitted_parameters = {}
-    amplitude_correction_factors = {}
+    delta_amplitude = {}
+    delta_amplitude_detuned = {}
     chi2 = {}
     for qubit in qubits:
         qubit_data = data[qubit]
-        pi_pulse_amplitude = data.pi_pulse_amplitudes[qubit]
+        detuned_pi_pulse_amplitude = data.pi_pulse_amplitudes[qubit]
         y = qubit_data.prob
         x = qubit_data.flips
-        pguess = [0.5, 0.5, 1, np.pi, 0]
+
+        ft = np.fft.rfft(y)
+        # Remove the zero frequency mode
+        mags = abs(ft)[1:]
+        local_maxima = find_peaks(mags, height=0)
+        peak_heights = local_maxima[1]["peak_heights"]
+        # Select the frequency with the highest peak
+        index = (
+            int(local_maxima[0][np.argmax(peak_heights)] + 1)
+            if len(local_maxima[0]) > 0
+            else None
+        )
+        f = x[index] / (x[1] - x[0]) if index is not None else 1
+        pguess = [0.5, 0.5, 1 / f, np.pi, 0]
+
         try:
             popt, perr = curve_fit(
                 flipping_fit,
                 x,
                 y,
                 p0=pguess,
                 maxfev=2000000,
@@ -182,60 +178,76 @@
                     [0, 0, -np.inf, 0, 0],
                     [1, np.inf, np.inf, 2 * np.pi, np.inf],
                 ),
                 sigma=qubit_data.error,
             )
             perr = np.sqrt(np.diag(perr)).tolist()
             popt = popt.tolist()
-        except:
-            log.warning("flipping_fit: the fitting was not succesful")
-            popt = [0] * 5
-            perr = [1] * 5
-
-        if popt[3] > np.pi / 2 and popt[3] < 3 * np.pi / 2:
-            signed_correction = -popt[2] / 2
-        else:
-            signed_correction = popt[2] / 2
-        # The amplitude is directly proportional to the rotation angle
-        corrected_amplitudes[qubit] = (
-            float((pi_pulse_amplitude * np.pi) / (np.pi + signed_correction)),
-            float(
-                pi_pulse_amplitude
-                * np.pi
-                * 1
-                / (np.pi + signed_correction) ** 2
+
+            if popt[3] > np.pi / 2 and popt[3] < 3 * np.pi / 2:
+                signed_correction = -popt[2] / 2
+            else:
+                signed_correction = popt[2] / 2
+            # The amplitude is directly proportional to the rotation angle
+            corrected_amplitudes[qubit] = (
+                float(detuned_pi_pulse_amplitude * np.pi / (np.pi + signed_correction)),
+                float(
+                    detuned_pi_pulse_amplitude
+                    * np.pi
+                    * 1
+                    / (np.pi + signed_correction) ** 2
+                    * perr[2]
+                    / 2
+                ),
+            )
+
+            fitted_parameters[qubit] = popt
+
+            delta_amplitude[qubit] = (
+                -signed_correction
+                * detuned_pi_pulse_amplitude
+                / (np.pi + signed_correction),
+                np.abs(
+                    np.pi
+                    * detuned_pi_pulse_amplitude
+                    * np.power(np.pi + signed_correction, -2)
+                )
                 * perr[2]
-                / 2
-            ),
-        )
-        fitted_parameters[qubit] = popt
-        amplitude_correction_factors[qubit] = (
-            float(signed_correction / np.pi * pi_pulse_amplitude),
-            float(perr[2] * pi_pulse_amplitude / np.pi / 2),
-        )
-        chi2[qubit] = (
-            chi2_reduced(
-                y,
-                flipping_fit(x, *popt),
-                qubit_data.error,
-            ),
-            np.sqrt(2 / len(x)),
-        )
+                / 2,
+            )
+            delta_amplitude_detuned[qubit] = (
+                delta_amplitude[qubit][0] - data.detuning,
+                delta_amplitude[qubit][1],
+            )
+
+            chi2[qubit] = (
+                chi2_reduced(
+                    y,
+                    flipping_fit(x, *popt),
+                    qubit_data.error,
+                ),
+                np.sqrt(2 / len(x)),
+            )
+        except Exception as e:
+            log.warning(f"Error in flipping fit for qubit {qubit} due to {e}.")
 
     return FlippingResults(
-        corrected_amplitudes, amplitude_correction_factors, fitted_parameters, chi2
+        corrected_amplitudes,
+        delta_amplitude,
+        delta_amplitude_detuned,
+        fitted_parameters,
+        chi2,
     )
 
 
 def _plot(data: FlippingData, target: QubitId, fit: FlippingResults = None):
     """Plotting function for Flipping."""
 
     figures = []
     fig = go.Figure()
-
     fitting_report = ""
     qubit_data = data[target]
 
     probs = qubit_data.prob
     error_bars = qubit_data.error
 
     fig.add_trace(
@@ -282,21 +294,23 @@
                 line=go.scatter.Line(dash="dot"),
             ),
         )
         fitting_report = table_html(
             table_dict(
                 target,
                 [
-                    "Amplitude correction factor",
+                    "Delta amplitude [a.u.]",
+                    "Delta amplitude (with detuning) [a.u.]",
                     "Corrected amplitude [a.u.]",
                     "chi2 reduced",
                 ],
                 [
-                    np.round(fit.amplitude_factors[target], 4),
-                    np.round(fit.amplitude[target], 4),
+                    fit.delta_amplitude[target],
+                    fit.delta_amplitude_detuned[target],
+                    fit.amplitude[target],
                     fit.chi2[target],
                 ],
                 display_error=True,
             )
         )
 
     # last part
```

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/flipping_signal.py` & `qibocal-0.0.9/src/qibocal/protocols/flipping_signal.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,57 +10,88 @@
 from qibolab.qubits import QubitId
 from scipy.optimize import curve_fit
 from scipy.signal import find_peaks
 
 from qibocal import update
 from qibocal.auto.operation import Data, Parameters, Results, Routine
 from qibocal.config import log
-from qibocal.protocols.characterization.utils import table_dict, table_html
+from qibocal.protocols.utils import table_dict, table_html
 
 
 @dataclass
 class FlippingSignalParameters(Parameters):
     """Flipping runcard inputs."""
 
     nflips_max: int
     """Maximum number of flips ([RX(pi) - RX(pi)] sequences). """
     nflips_step: int
     """Flip step."""
     unrolling: bool = False
     """If ``True`` it uses sequence unrolling to deploy multiple sequences in a single instrument call.
     Defaults to ``False``."""
+    detuning: float = 0
+    """Amplitude detuning."""
 
 
 @dataclass
 class FlippingSignalResults(Results):
     """Flipping outputs."""
 
     amplitude: dict[QubitId, tuple[float, Optional[float]]]
     """Drive amplitude for each qubit."""
-    amplitude_factors: dict[QubitId, tuple[float, Optional[float]]]
-    """Drive amplitude correction factor for each qubit."""
+    delta_amplitude: dict[QubitId, tuple[float, Optional[float]]]
+    """Difference in amplitude between initial value and fit."""
+    delta_amplitude_detuned: dict[QubitId, tuple[float, Optional[float]]]
+    """Difference in amplitude between detuned value and fit."""
     fitted_parameters: dict[QubitId, dict[str, float]]
     """Raw fitting output."""
 
 
 FlippingType = np.dtype([("flips", np.float64), ("signal", np.float64)])
 
 
 @dataclass
 class FlippingSignalData(Data):
     """Flipping acquisition outputs."""
 
     resonator_type: str
     """Resonator type."""
+    detuning: float
+    """Amplitude detuning."""
     pi_pulse_amplitudes: dict[QubitId, float]
     """Pi pulse amplitudes for each qubit."""
     data: dict[QubitId, npt.NDArray[FlippingType]] = field(default_factory=dict)
     """Raw data acquired."""
 
 
+def flipping_sequence(platform: Platform, qubit: QubitId, detuning: float, flips: int):
+
+    sequence = PulseSequence()
+    RX90_pulse = platform.create_RX90_pulse(qubit, start=0)
+    sequence.add(RX90_pulse)
+    # execute sequence RX(pi/2) - [RX(pi) - RX(pi)] from 0...flips times - RO
+    start1 = RX90_pulse.duration
+    drive_frequency = platform.qubits[qubit].native_gates.RX.frequency
+    for _ in range(flips):
+        RX_pulse1 = platform.create_RX_pulse(qubit, start=start1)
+        RX_pulse1.frequency = drive_frequency + detuning
+        start2 = start1 + RX_pulse1.duration
+        RX_pulse2 = platform.create_RX_pulse(qubit, start=start2)
+        RX_pulse2.frequency = drive_frequency + detuning
+
+        sequence.add(RX_pulse1)
+        sequence.add(RX_pulse2)
+        start1 = start2 + RX_pulse2.duration
+
+    # add ro pulse at the end of the sequence
+    sequence.add(platform.create_qubit_readout_pulse(qubit, start=start1))
+
+    return sequence
+
+
 def _acquisition(
     params: FlippingSignalParameters,
     platform: Platform,
     targets: list[QubitId],
 ) -> FlippingSignalData:
     r"""
     Data acquisition for flipping.
@@ -75,14 +106,15 @@
 
     Returns:
         data (:class:`FlippingSignalData`)
     """
 
     data = FlippingSignalData(
         resonator_type=platform.resonator_type,
+        detuning=params.detuning,
         pi_pulse_amplitudes={
             qubit: platform.qubits[qubit].native_gates.RX.amplitude for qubit in targets
         },
     )
 
     options = ExecutionParameters(
         nshots=params.nshots,
@@ -93,47 +125,34 @@
 
     # sweep the parameter
     sequences, all_ro_pulses = [], []
     flips_sweep = range(0, params.nflips_max, params.nflips_step)
     for flips in flips_sweep:
         # create a sequence of pulses for the experiment
         sequence = PulseSequence()
-        ro_pulses = {}
         for qubit in targets:
-            RX90_pulse = platform.create_RX90_pulse(qubit, start=0)
-            sequence.add(RX90_pulse)
-            # execute sequence RX(pi/2) - [RX(pi) - RX(pi)] from 0...flips times - RO
-            start1 = RX90_pulse.duration
-            for _ in range(flips):
-                RX_pulse1 = platform.create_RX_pulse(qubit, start=start1)
-                start2 = start1 + RX_pulse1.duration
-                RX_pulse2 = platform.create_RX_pulse(qubit, start=start2)
-                sequence.add(RX_pulse1)
-                sequence.add(RX_pulse2)
-                start1 = start2 + RX_pulse2.duration
-
-            # add ro pulse at the end of the sequence
-            ro_pulses[qubit] = platform.create_qubit_readout_pulse(qubit, start=start1)
-            sequence.add(ro_pulses[qubit])
+            sequence += flipping_sequence(
+                platform=platform, qubit=qubit, detuning=params.detuning, flips=flips
+            )
 
         sequences.append(sequence)
-        all_ro_pulses.append(ro_pulses)
+        all_ro_pulses.append(sequence.ro_pulses)
 
     # execute the pulse sequence
     if params.unrolling:
         results = platform.execute_pulse_sequences(sequences, options)
 
     elif not params.unrolling:
         results = [
             platform.execute_pulse_sequence(sequence, options) for sequence in sequences
         ]
 
     for ig, (flips, ro_pulses) in enumerate(zip(flips_sweep, all_ro_pulses)):
         for qubit in targets:
-            serial = ro_pulses[qubit].serial
+            serial = ro_pulses.get_qubit_pulses(qubit)[0].serial
             if params.unrolling:
                 result = results[serial][0]
             else:
                 result = results[ig][serial]
             data.register_qubit(
                 FlippingType,
                 (qubit),
@@ -158,18 +177,19 @@
     .. math::
 
         y = p_0 sin\Big(\frac{2 \pi x}{p_2} + p_3\Big)*\exp{-x*p4} + p_1.
     """
     qubits = data.qubits
     corrected_amplitudes = {}
     fitted_parameters = {}
-    amplitude_correction_factors = {}
+    delta_amplitude = {}
+    delta_amplitude_detuned = {}
     for qubit in qubits:
         qubit_data = data[qubit]
-        pi_pulse_amplitude = data.pi_pulse_amplitudes[qubit]
+        detuned_pi_pulse_amplitude = data.pi_pulse_amplitudes[qubit] + data.detuning
         voltages = qubit_data.signal
         flips = qubit_data.flips
         y_min = np.min(voltages)
         # Guessing period using Fourier transform
         ft = np.fft.rfft(voltages)
         # Remove the zero frequency mode
         mags = abs(ft)[1:]
@@ -197,42 +217,48 @@
                 p0=pguess,
                 maxfev=2000000,
                 bounds=(
                     [0, 0, -np.inf, 0, 0],
                     [1, np.inf, np.inf, 2 * np.pi, np.inf],
                 ),
             )
-        except:
-            log.warning("flipping_fit: the fitting was not succesful")
-            popt = [0] * 5
-
-        translated_popt = [
-            y_min + (y_max - y_min) * popt[0],
-            (y_max - y_min)
-            * popt[1]
-            * np.exp(x_min * popt[4] * 2 * np.pi * f / (x_max - x_min)),
-            popt[2] * 2 * np.pi * f / (x_max - x_min),
-            popt[3] - x_min * 2 * np.pi * f / (x_max - x_min) * popt[2],
-            popt[4] * 2 * np.pi * f / (x_max - x_min),
-        ]
-        # TODO: this might be related to the resonator type
-        if popt[3] > np.pi / 2 and popt[3] < 3 * np.pi / 2:
-            signed_correction = translated_popt[2] / 2
-        else:
-            signed_correction = -translated_popt[2] / 2
-        # The amplitude is directly proportional to the rotation angle
-        corrected_amplitudes[qubit] = (pi_pulse_amplitude * np.pi) / (
-            np.pi + signed_correction
-        )
-        fitted_parameters[qubit] = translated_popt
-        amplitude_correction_factors[qubit] = (
-            signed_correction / np.pi * pi_pulse_amplitude
-        )
+
+            translated_popt = [
+                y_min + (y_max - y_min) * popt[0],
+                (y_max - y_min)
+                * popt[1]
+                * np.exp(x_min * popt[4] * 2 * np.pi * f / (x_max - x_min)),
+                popt[2] * 2 * np.pi * f / (x_max - x_min),
+                popt[3] - x_min * 2 * np.pi * f / (x_max - x_min) * popt[2],
+                popt[4] * 2 * np.pi * f / (x_max - x_min),
+            ]
+            # TODO: this might be related to the resonator type
+            if popt[3] > np.pi / 2 and popt[3] < 3 * np.pi / 2:
+                signed_correction = translated_popt[2] / 2
+            else:
+                signed_correction = -translated_popt[2] / 2
+            # The amplitude is directly proportional to the rotation angle
+            corrected_amplitudes[qubit] = (detuned_pi_pulse_amplitude * np.pi) / (
+                np.pi + signed_correction
+            )
+            fitted_parameters[qubit] = translated_popt
+            delta_amplitude[qubit] = (
+                -signed_correction
+                * detuned_pi_pulse_amplitude
+                / (np.pi + signed_correction)
+            )
+            delta_amplitude_detuned[qubit] = delta_amplitude[qubit] - data.detuning
+        except Exception as e:
+            log.warning(f"Error in flipping fit for qubit {qubit} due to {e}.")
+
     return FlippingSignalResults(
-        corrected_amplitudes, amplitude_correction_factors, fitted_parameters
+        corrected_amplitudes,
+        delta_amplitude,
+        delta_amplitude_detuned,
+        fitted_parameters,
     )
 
 
 def _plot(data: FlippingSignalData, target, fit: FlippingSignalResults = None):
     """Plotting function for Flipping."""
 
     figures = []
@@ -272,17 +298,22 @@
                 name="Fit",
                 line=go.scatter.Line(dash="dot"),
             ),
         )
         fitting_report = table_html(
             table_dict(
                 target,
-                ["Amplitude correction factor", "Corrected amplitude [a.u.]"],
                 [
-                    np.round(fit.amplitude_factors[target], 4),
+                    "Delta amplitude [a.u.]",
+                    "Delta amplitude (with detuning) [a.u.]",
+                    "Corrected amplitude [a.u.]",
+                ],
+                [
+                    np.round(fit.delta_amplitude[target], 4),
+                    np.round(fit.delta_amplitude_detuned[target], 4),
                     np.round(fit.amplitude[target], 4),
                 ],
             )
         )
 
     # last part
     fig.update_layout(
```

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/flux_dependence/avoided_crossing.py` & `qibocal-0.0.9/src/qibocal/protocols/flux_dependence/avoided_crossing.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 import numpy.typing as npt
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
 from qibolab.platform import Platform
 from qibolab.qubits import QubitId, QubitPairId
 
 from qibocal.auto.operation import Data, Results, Routine
-from qibocal.protocols.characterization.two_qubit_interaction.utils import order_pair
-from qibocal.protocols.characterization.utils import HZ_TO_GHZ, table_dict, table_html
+from qibocal.protocols.two_qubit_interaction.utils import order_pair
+from qibocal.protocols.utils import HZ_TO_GHZ, table_dict, table_html
 
 from .qubit_flux_dependence import QubitFluxParameters, QubitFluxType
 from .qubit_flux_dependence import _acquisition as flux_acquisition
 
 STEP = 60
 POINT_SIZE = 10
```

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/flux_dependence/qubit_crosstalk.py` & `qibocal-0.0.9/src/qibocal/protocols/flux_dependence/qubit_flux_tracking.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,88 +1,73 @@
-from dataclasses import dataclass, field
-from typing import Optional
+from dataclasses import dataclass
 
 import numpy as np
-import numpy.typing as npt
 from qibolab import AcquisitionType, AveragingMode, ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
 from qibolab.sweeper import Parameter, Sweeper, SweeperType
 
-from qibocal.auto.operation import Results, Routine
+from qibocal.auto.operation import Routine
+from qibocal.config import raise_error
 
 from ..qubit_spectroscopy_ef import DEFAULT_ANHARMONICITY
-from . import utils
-from .qubit_flux_dependence import (
-    QubitFluxData,
-    QubitFluxParameters,
-    QubitFluxResults,
-    QubitFluxType,
-)
-from .resonator_flux_dependence import create_flux_pulse_sweepers
+from . import qubit_flux_dependence, utils
 
 
 @dataclass
-class QubitCrosstalkParameters(QubitFluxParameters):
-    """Crosstalk runcard inputs."""
-
-    flux_qubits: Optional[list[QubitId]] = None
-    """IDs of the qubits that we will sweep the flux on.
-    If ``None`` flux will be swept on all qubits that we are running the routine on in a multiplex fashion.
-    If given flux will be swept on the given qubits in a sequential fashion (n qubits will result to n different executions).
-    Multiple qubits may be measured in each execution as specified by the ``qubits`` option in the runcard.
-    """
+class QubitFluxTrackParameters(qubit_flux_dependence.QubitFluxParameters):
+    """QubitFluxTrack runcard inputs."""
 
 
 @dataclass
-class QubitCrosstalkData(QubitFluxData):
-    """Crosstalk acquisition outputs when ``flux_qubits`` are given."""
+class QubitFluxTrackResults(qubit_flux_dependence.QubitFluxParameters):
+    """QubitFluxTrack outputs."""
 
-    data: dict[QubitId, dict[QubitId, npt.NDArray[QubitFluxType]]] = field(
-        default_factory=dict
-    )
-    """Raw data acquired for (qubit, qubit_flux) pairs saved in nested dictionaries."""
 
-    def register_qubit(self, qubit, flux_qubit, freq, bias, signal, phase):
+@dataclass
+class QubitFluxTrackData(qubit_flux_dependence.QubitFluxData):
+    """QubitFluxTrack acquisition outputs."""
+
+    def register_qubit_track(self, qubit, freq, bias, signal, phase):
         """Store output for single qubit."""
-        ar = utils.create_data_array(freq, bias, signal, phase, dtype=QubitFluxType)
-        if (qubit, flux_qubit) in self.data:
-            self.data[qubit, flux_qubit] = np.rec.array(
-                np.concatenate((self.data[qubit, flux_qubit], ar))
-            )
+        # to be able to handle the 1D sweeper case
+        size = len(freq)
+        ar = np.empty(size, dtype=qubit_flux_dependence.QubitFluxType)
+        ar["freq"] = freq
+        ar["bias"] = [bias] * size
+        ar["signal"] = signal
+        ar["phase"] = phase
+        if qubit in self.data:
+            self.data[qubit] = np.rec.array(np.concatenate((self.data[qubit], ar)))
         else:
-            self.data[qubit, flux_qubit] = ar
-
-
-@dataclass
-class QubitCrosstalkResult(Results):
-    """
-    Qubit Crosstalk outputs.
-    """
+            self.data[qubit] = np.rec.array(ar)
 
 
 def _acquisition(
-    params: QubitCrosstalkParameters,
+    params: QubitFluxTrackResults,
     platform: Platform,
     targets: list[QubitId],
-) -> QubitCrosstalkData:
-    """Data acquisition for Crosstalk Experiment."""
+) -> QubitFluxTrackData:
+    """Data acquisition for QubitFlux Experiment."""
+    # create a sequence of pulses for the experiment:
+    # MZ
 
     # taking advantage of multiplexing, apply the same set of gates to all qubits in parallel
     sequence = PulseSequence()
     ro_pulses = {}
     qd_pulses = {}
+    qubit_frequency = {}
     for qubit in targets:
         qd_pulses[qubit] = platform.create_qubit_drive_pulse(
             qubit, start=0, duration=params.drive_duration
         )
-
+        qubit_frequency[qubit] = platform.qubits[qubit].drive_frequency
         if params.transition == "02":
-            if platform.qubits[qubit].anharmonicity:
+            if platform.qubits[qubit].anharmonicity != 0:
                 qd_pulses[qubit].frequency -= platform.qubits[qubit].anharmonicity / 2
             else:
                 qd_pulses[qubit].frequency -= DEFAULT_ANHARMONICITY / 2
 
         if params.drive_amplitude is not None:
             qd_pulses[qubit].amplitude = params.drive_amplitude
 
@@ -90,79 +75,83 @@
             qubit, start=qd_pulses[qubit].finish
         )
         sequence.add(qd_pulses[qubit])
         sequence.add(ro_pulses[qubit])
 
     # define the parameters to sweep and their range:
     delta_frequency_range = np.arange(
-        -params.freq_width // 2, params.freq_width // 2, params.freq_step
+        -params.freq_width / 2, params.freq_width / 2, params.freq_step
     )
+
+    delta_bias_range = np.arange(
+        -params.bias_width / 2, params.bias_width / 2, params.bias_step
+    )
+
     freq_sweeper = Sweeper(
         Parameter.frequency,
         delta_frequency_range,
         pulses=[qd_pulses[qubit] for qubit in targets],
         type=SweeperType.OFFSET,
     )
-    # TODO : abstract common lines with qubit flux dep routine
-    if params.flux_qubits is None:
-        flux_qubits = list(platform.qubits.keys())
-    else:
-        flux_qubits = params.flux_qubits
-    if params.flux_pulses:
-        delta_bias_flux_range, sweepers = create_flux_pulse_sweepers(
-            params, platform, targets, sequence
-        )
-    else:
-        delta_bias_flux_range = np.arange(
-            -params.bias_width / 2, params.bias_width / 2, params.bias_step
-        )
-        sweepers = [
-            Sweeper(
-                Parameter.bias,
-                delta_bias_flux_range,
-                qubits=[platform.qubits[flux_qubit]],
-                type=SweeperType.OFFSET,
-            )
-            for flux_qubit in flux_qubits
-        ]
-    data = QubitCrosstalkData(
-        resonator_type=platform.resonator_type, flux_pulses=params.flux_pulses
-    )
 
-    options = ExecutionParameters(
-        nshots=params.nshots,
-        relaxation_time=params.relaxation_time,
-        acquisition_type=AcquisitionType.INTEGRATION,
-        averaging_mode=AveragingMode.CYCLIC,
+    data = QubitFluxTrackData(
+        resonator_type=platform.resonator_type,
+        qubit_frequency=qubit_frequency,
     )
-    for flux_qubit, bias_sweeper in zip(flux_qubits, sweepers):
-        results = platform.sweep(sequence, options, bias_sweeper, freq_sweeper)
+
+    for bias in delta_bias_range:
+        for qubit in targets:
+            try:
+                freq_resonator = utils.transmon_readout_frequency_diagonal(
+                    bias,
+                    platform.qubits[qubit].drive_frequency,
+                    platform.qubits[qubit].asymmetry,
+                    platform.qubits[qubit].crosstalk_matrix[qubit],
+                    platform.qubits[qubit].sweetspot,
+                    platform.qubits[qubit].bare_resonator_frequency,
+                    platform.qubits[qubit].g,
+                )
+                # modify qubit resonator frequency
+                platform.qubits[qubit].readout_frequency = freq_resonator
+            except:
+                raise_error
+                (
+                    RuntimeError,
+                    "qubit_flux_track: Not enough parameters to estimate the resonator freq for the given bias. Please run resonator spectroscopy flux and update the runcard",
+                )
+
+            # modify qubit flux
+            platform.qubits[qubit].flux.offset = bias
+
+            # execute pulse sequence sweeping only qubit resonator
+            results = platform.sweep(
+                sequence,
+                ExecutionParameters(
+                    nshots=params.nshots,
+                    relaxation_time=params.relaxation_time,
+                    acquisition_type=AcquisitionType.INTEGRATION,
+                    averaging_mode=AveragingMode.CYCLIC,
+                ),
+                freq_sweeper,
+            )
+
         # retrieve the results for every qubit
         for qubit in targets:
             result = results[ro_pulses[qubit].serial]
-            if flux_qubit is None:
-                sweetspot = platform.qubits[qubit].sweetspot
-            else:
-                sweetspot = platform.qubits[flux_qubit].sweetspot
-            data.register_qubit(
+            data.register_qubit_track(
                 qubit,
-                flux_qubit,
                 signal=result.magnitude,
                 phase=result.phase,
                 freq=delta_frequency_range + qd_pulses[qubit].frequency,
-                bias=delta_bias_flux_range + sweetspot,
+                bias=bias + platform.qubits[qubit].sweetspot,
             )
 
     return data
 
 
-def _fit(data: QubitCrosstalkData) -> QubitCrosstalkResult:
-    return QubitCrosstalkResult()
-
-
-def _plot(data: QubitFluxData, fit: QubitFluxResults, target: QubitId):
-    """Plotting function for Crosstalk Experiment."""
-    return utils.flux_crosstalk_plot(data, target)
-
-
-qubit_crosstalk = Routine(_acquisition, _fit, _plot)
-"""Qubit crosstalk Routine object"""
+qubit_flux_tracking = Routine(
+    _acquisition,
+    qubit_flux_dependence._fit,
+    qubit_flux_dependence._plot,
+    qubit_flux_dependence._update,
+)
+"""QubitFluxTrack Routine object."""
```

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/flux_dependence/qubit_flux_dependence.py` & `qibocal-0.0.9/src/qibocal/protocols/flux_dependence/qubit_flux_dependence.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,20 +9,18 @@
 from qibolab.qubits import QubitId
 from qibolab.sweeper import Parameter, Sweeper, SweeperType
 from scipy.optimize import curve_fit
 
 from qibocal import update
 from qibocal.auto.operation import Data, Results, Routine
 from qibocal.config import log
-from qibocal.protocols.characterization.qubit_spectroscopy_ef import (
-    DEFAULT_ANHARMONICITY,
-)
+from qibocal.protocols.qubit_spectroscopy_ef import DEFAULT_ANHARMONICITY
 
-from ..utils import GHZ_TO_HZ, HZ_TO_GHZ, table_dict, table_html
-from . import resonator_flux_dependence, utils
+from ..utils import GHZ_TO_HZ, HZ_TO_GHZ, extract_feature, table_dict, table_html
+from . import utils
 from .resonator_flux_dependence import ResonatorFluxParameters
 
 
 @dataclass
 class QubitFluxParameters(ResonatorFluxParameters):
     """QubitFlux runcard inputs."""
 
@@ -65,20 +63,20 @@
 @dataclass
 class QubitFluxData(Data):
     """QubitFlux acquisition outputs."""
 
     resonator_type: str
     """Resonator type."""
 
-    flux_pulses: bool
-    """True if sweeping flux pulses, False if sweeping bias."""
-
     qubit_frequency: dict[QubitId, float] = field(default_factory=dict)
     """Qubit frequencies."""
 
+    offset: dict[QubitId, float] = field(default_factory=dict)
+    """Qubit bias offset."""
+
     data: dict[QubitId, npt.NDArray[QubitFluxType]] = field(default_factory=dict)
     """Raw data acquired."""
 
     def register_qubit(self, qubit, freq, bias, signal, phase):
         """Store output for single qubit."""
         self.data[qubit] = utils.create_data_array(
             freq, bias, signal, phase, dtype=QubitFluxType
@@ -93,19 +91,21 @@
     """Data acquisition for QubitFlux Experiment."""
 
     # taking advantage of multiplexing, apply the same set of gates to all qubits in parallel
     sequence = PulseSequence()
     ro_pulses = {}
     qd_pulses = {}
     qubit_frequency = {}
+    offset = {}
     for qubit in targets:
         qd_pulses[qubit] = platform.create_qubit_drive_pulse(
             qubit, start=0, duration=params.drive_duration
         )
         qubit_frequency[qubit] = platform.qubits[qubit].drive_frequency
+        offset[qubit] = platform.qubits[qubit].sweetspot
 
         if params.transition == "02":
             if platform.qubits[qubit].anharmonicity:
                 qd_pulses[qubit].frequency -= platform.qubits[qubit].anharmonicity / 2
             else:
                 qd_pulses[qubit].frequency -= DEFAULT_ANHARMONICITY / 2
 
@@ -116,47 +116,40 @@
             qubit, start=qd_pulses[qubit].finish
         )
         sequence.add(qd_pulses[qubit])
         sequence.add(ro_pulses[qubit])
 
     # define the parameters to sweep and their range:
     delta_frequency_range = np.arange(
-        -params.freq_width // 2, params.freq_width // 2, params.freq_step
+        -params.freq_width / 2, params.freq_width / 2, params.freq_step
     )
     freq_sweeper = Sweeper(
         Parameter.frequency,
         delta_frequency_range,
         pulses=[qd_pulses[qubit] for qubit in targets],
         type=SweeperType.OFFSET,
     )
-    if params.flux_pulses:
-        (
-            delta_bias_flux_range,
-            sweepers,
-        ) = resonator_flux_dependence.create_flux_pulse_sweepers(
-            params, platform, targets, sequence
-        )
-    else:
-        delta_bias_flux_range = np.arange(
-            -params.bias_width / 2, params.bias_width / 2, params.bias_step
+
+    delta_bias_range = np.arange(
+        -params.bias_width / 2, params.bias_width / 2, params.bias_step
+    )
+    sweepers = [
+        Sweeper(
+            Parameter.bias,
+            delta_bias_range,
+            qubits=[platform.qubits[qubit] for qubit in targets],
+            type=SweeperType.OFFSET,
         )
-        sweepers = [
-            Sweeper(
-                Parameter.bias,
-                delta_bias_flux_range,
-                qubits=[platform.qubits[qubit] for qubit in targets],
-                type=SweeperType.OFFSET,
-            )
-        ]
+    ]
+
     data = QubitFluxData(
         resonator_type=platform.resonator_type,
-        flux_pulses=params.flux_pulses,
         qubit_frequency=qubit_frequency,
+        offset=offset,
     )
-
     options = ExecutionParameters(
         nshots=params.nshots,
         relaxation_time=params.relaxation_time,
         acquisition_type=AcquisitionType.INTEGRATION,
         averaging_mode=AveragingMode.CYCLIC,
     )
     for bias_sweeper in sweepers:
@@ -166,15 +159,15 @@
             result = results[ro_pulses[qubit].serial]
             sweetspot = platform.qubits[qubit].sweetspot
             data.register_qubit(
                 qubit,
                 signal=result.magnitude,
                 phase=result.phase,
                 freq=delta_frequency_range + qd_pulses[qubit].frequency,
-                bias=delta_bias_flux_range + sweetspot,
+                bias=delta_bias_range + sweetspot,
             )
     return data
 
 
 def _fit(data: QubitFluxData) -> QubitFluxResults:
     """
     Post-processing for QubitFlux Experiment. See arxiv:0703002
@@ -192,19 +185,19 @@
     for qubit in qubits:
         qubit_data = data[qubit]
 
         biases = qubit_data.bias
         frequencies = qubit_data.freq
         signal = qubit_data.signal
 
-        frequencies, biases = utils.extract_feature(frequencies, biases, signal, "max")
+        frequencies, biases = extract_feature(frequencies, biases, signal, "max")
 
         try:
             popt = curve_fit(
-                utils.transmon_frequency,
+                utils.transmon_frequency_diagonal,
                 biases,
                 frequencies * HZ_TO_GHZ,
                 bounds=utils.qubit_flux_dependence_fit_bounds(
                     data.qubit_frequency[qubit], qubit_data.bias
                 ),
                 maxfev=100000,
             )[0]
@@ -229,29 +222,28 @@
         fitted_parameters=fitted_parameters,
     )
 
 
 def _plot(data: QubitFluxData, fit: QubitFluxResults, target: QubitId):
     """Plotting function for QubitFlux Experiment."""
     figures = utils.flux_dependence_plot(
-        data, fit, target, fit_function=utils.transmon_frequency
+        data,
+        fit,
+        target,
+        fit_function=utils.transmon_frequency_diagonal,
     )
-    if data.flux_pulses:
-        bias_flux_unit = "a.u."
-    else:
-        bias_flux_unit = "V"
     if fit is not None:
         fitting_report = table_html(
             table_dict(
                 target,
                 [
-                    f"Sweetspot [{bias_flux_unit}]",
+                    f"Sweetspot [V]",
                     "Qubit Frequency at Sweetspot [Hz]",
                     "Asymmetry d",
-                    "V_ii [V]",
+                    "Flux dependence",
                 ],
                 [
                     np.round(fit.sweetspot[target], 4),
                     np.round(fit.frequency[target], 4),
                     np.round(fit.asymmetry[target], 4),
                     np.round(fit.matrix_element[target], 4),
                 ],
@@ -261,11 +253,12 @@
     return figures, ""
 
 
 def _update(results: QubitFluxResults, platform: Platform, qubit: QubitId):
     update.drive_frequency(results.frequency[qubit], platform, qubit)
     update.sweetspot(results.sweetspot[qubit], platform, qubit)
     update.asymmetry(results.asymmetry[qubit], platform, qubit)
+    update.crosstalk_matrix(results.matrix_element[qubit], platform, qubit, qubit)
 
 
 qubit_flux = Routine(_acquisition, _fit, _plot, _update)
 """QubitFlux Routine object."""
```

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/flux_dependence/qubit_flux_tracking.py` & `qibocal-0.0.9/src/qibocal/protocols/qubit_spectroscopy.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,158 +1,164 @@
-from dataclasses import dataclass
+from dataclasses import dataclass, field
+from typing import Optional
 
 import numpy as np
-from qibolab import AcquisitionType, AveragingMode, ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
 from qibolab.sweeper import Parameter, Sweeper, SweeperType
 
-from qibocal.auto.operation import Routine
-from qibocal.config import raise_error
+from qibocal import update
+from qibocal.auto.operation import Parameters, Results, Routine
 
-from ..qubit_spectroscopy_ef import DEFAULT_ANHARMONICITY
-from . import qubit_flux_dependence, utils
+from .resonator_spectroscopy import ResonatorSpectroscopyData, ResSpecType
+from .utils import chi2_reduced, lorentzian, lorentzian_fit, spectroscopy_plot
 
 
 @dataclass
-class QubitFluxTrackParameters(qubit_flux_dependence.QubitFluxParameters):
-    """QubitFluxTrack runcard inputs."""
+class QubitSpectroscopyParameters(Parameters):
+    """QubitSpectroscopy runcard inputs."""
+
+    freq_width: int
+    """Width [Hz] for frequency sweep relative  to the qubit frequency."""
+    freq_step: int
+    """Frequency [Hz] step for sweep."""
+    drive_duration: int
+    """Drive pulse duration [ns]. Same for all qubits."""
+    drive_amplitude: Optional[float] = None
+    """Drive pulse amplitude (optional). Same for all qubits."""
+    hardware_average: bool = True
+    """By default hardware average will be performed."""
 
 
 @dataclass
-class QubitFluxTrackResults(qubit_flux_dependence.QubitFluxParameters):
-    """QubitFluxTrack outputs."""
+class QubitSpectroscopyResults(Results):
+    """QubitSpectroscopy outputs."""
 
+    frequency: dict[QubitId, dict[str, float]]
+    """Drive frequecy [GHz] for each qubit."""
+    amplitude: dict[QubitId, float]
+    """Input drive amplitude. Same for all qubits."""
+    fitted_parameters: dict[QubitId, list[float]]
+    """Raw fitting output."""
+    chi2_reduced: dict[QubitId, tuple[float, Optional[float]]] = field(
+        default_factory=dict
+    )
+    """Chi2 reduced."""
+    error_fit_pars: dict[QubitId, list] = field(default_factory=dict)
+    """Errors of the fit parameters."""
 
-@dataclass
-class QubitFluxTrackData(qubit_flux_dependence.QubitFluxData):
-    """QubitFluxTrack acquisition outputs."""
 
-    def register_qubit_track(self, qubit, freq, bias, signal, phase):
-        """Store output for single qubit."""
-        # to be able to handle the 1D sweeper case
-        size = len(freq)
-        ar = np.empty(size, dtype=qubit_flux_dependence.QubitFluxType)
-        ar["freq"] = freq
-        ar["bias"] = [bias] * size
-        ar["signal"] = signal
-        ar["phase"] = phase
-        if qubit in self.data:
-            self.data[qubit] = np.rec.array(np.concatenate((self.data[qubit], ar)))
-        else:
-            self.data[qubit] = np.rec.array(ar)
+class QubitSpectroscopyData(ResonatorSpectroscopyData):
+    """QubitSpectroscopy acquisition outputs."""
 
 
 def _acquisition(
-    params: QubitFluxTrackResults,
-    platform: Platform,
-    targets: list[QubitId],
-) -> QubitFluxTrackData:
-    """Data acquisition for QubitFlux Experiment."""
+    params: QubitSpectroscopyParameters, platform: Platform, targets: list[QubitId]
+) -> QubitSpectroscopyData:
+    """Data acquisition for qubit spectroscopy."""
     # create a sequence of pulses for the experiment:
-    # MZ
+    # long drive probing pulse - MZ
 
     # taking advantage of multiplexing, apply the same set of gates to all qubits in parallel
     sequence = PulseSequence()
     ro_pulses = {}
     qd_pulses = {}
-    qubit_frequency = {}
+    amplitudes = {}
     for qubit in targets:
         qd_pulses[qubit] = platform.create_qubit_drive_pulse(
             qubit, start=0, duration=params.drive_duration
         )
-        qubit_frequency[qubit] = platform.qubits[qubit].drive_frequency
-        if params.transition == "02":
-            if platform.qubits[qubit].anharmonicity != 0:
-                qd_pulses[qubit].frequency -= platform.qubits[qubit].anharmonicity / 2
-            else:
-                qd_pulses[qubit].frequency -= DEFAULT_ANHARMONICITY / 2
-
         if params.drive_amplitude is not None:
             qd_pulses[qubit].amplitude = params.drive_amplitude
 
+        amplitudes[qubit] = qd_pulses[qubit].amplitude
+
         ro_pulses[qubit] = platform.create_qubit_readout_pulse(
             qubit, start=qd_pulses[qubit].finish
         )
         sequence.add(qd_pulses[qubit])
         sequence.add(ro_pulses[qubit])
 
-    # define the parameters to sweep and their range:
+    # define the parameter to sweep and its range:
     delta_frequency_range = np.arange(
-        -params.freq_width // 2, params.freq_width // 2, params.freq_step
-    )
-
-    delta_bias_range = np.arange(
-        -params.bias_width / 2, params.bias_width / 2, params.bias_step
+        -params.freq_width / 2, params.freq_width / 2, params.freq_step
     )
-
-    freq_sweeper = Sweeper(
+    sweeper = Sweeper(
         Parameter.frequency,
         delta_frequency_range,
         pulses=[qd_pulses[qubit] for qubit in targets],
         type=SweeperType.OFFSET,
     )
 
-    data = QubitFluxTrackData(
-        resonator_type=platform.resonator_type,
-        flux_pulses=params.flux_pulses,
-        qubit_frequency=qubit_frequency,
-    )
-
-    for bias in delta_bias_range:
-        for qubit in targets:
-            try:
-                freq_resonator = utils.transmon_readout_frequency(
-                    bias,
-                    platform.qubits[qubit].drive_frequency,
-                    platform.qubits[qubit].asymmetry,
-                    platform.qubits[qubit].crosstalk_matrix[qubit],
-                    platform.qubits[qubit].sweetspot,
-                    platform.qubits[qubit].bare_resonator_frequency,
-                    platform.qubits[qubit].g,
-                )
-                # modify qubit resonator frequency
-                platform.qubits[qubit].readout_frequency = freq_resonator
-            except:
-                raise_error
-                (
-                    RuntimeError,
-                    "qubit_flux_track: Not enough parameters to estimate the resonator freq for the given bias. Please run resonator spectroscopy flux and update the runcard",
-                )
-
-            # modify qubit flux
-            platform.qubits[qubit].flux.offset = bias
-
-            # execute pulse sequence sweeping only qubit resonator
-            results = platform.sweep(
-                sequence,
-                ExecutionParameters(
-                    nshots=params.nshots,
-                    relaxation_time=params.relaxation_time,
-                    acquisition_type=AcquisitionType.INTEGRATION,
-                    averaging_mode=AveragingMode.CYCLIC,
-                ),
-                freq_sweeper,
-            )
+    # Create data structure for data acquisition.
+    data = QubitSpectroscopyData(
+        resonator_type=platform.resonator_type, amplitudes=amplitudes
+    )
+
+    results = platform.sweep(
+        sequence,
+        params.execution_parameters,
+        sweeper,
+    )
 
-        # retrieve the results for every qubit
-        for qubit in targets:
-            result = results[ro_pulses[qubit].serial]
-            data.register_qubit_track(
-                qubit,
-                signal=result.magnitude,
-                phase=result.phase,
+    # retrieve the results for every qubit
+    for qubit, ro_pulse in ro_pulses.items():
+        result = results[ro_pulse.serial]
+        # store the results
+        data.register_qubit(
+            ResSpecType,
+            (qubit),
+            dict(
+                signal=result.average.magnitude,
+                phase=result.average.phase,
                 freq=delta_frequency_range + qd_pulses[qubit].frequency,
-                bias=bias + platform.qubits[qubit].sweetspot,
+                error_signal=result.average.std,
+                error_phase=result.phase_std,
+            ),
+        )
+    return data
+
+
+def _fit(data: QubitSpectroscopyData) -> QubitSpectroscopyResults:
+    """Post-processing function for QubitSpectroscopy."""
+    qubits = data.qubits
+    frequency = {}
+    fitted_parameters = {}
+    error_fit_pars = {}
+    chi2 = {}
+    for qubit in qubits:
+        fit_result = lorentzian_fit(
+            data[qubit], resonator_type=data.resonator_type, fit="qubit"
+        )
+        if fit_result is not None:
+            frequency[qubit], fitted_parameters[qubit], error_fit_pars[qubit] = (
+                fit_result
+            )
+            chi2[qubit] = (
+                chi2_reduced(
+                    data[qubit].signal,
+                    lorentzian(data[qubit].freq, *fitted_parameters[qubit]),
+                    data[qubit].error_signal,
+                ),
+                np.sqrt(2 / len(data[qubit].freq)),
             )
+    return QubitSpectroscopyResults(
+        frequency=frequency,
+        fitted_parameters=fitted_parameters,
+        amplitude=data.amplitudes,
+        error_fit_pars=error_fit_pars,
+        chi2_reduced=chi2,
+    )
 
-    return data
+
+def _plot(data: QubitSpectroscopyData, target: QubitId, fit: QubitSpectroscopyResults):
+    """Plotting function for QubitSpectroscopy."""
+    return spectroscopy_plot(data, target, fit)
+
+
+def _update(results: QubitSpectroscopyResults, platform: Platform, target: QubitId):
+    update.drive_frequency(results.frequency[target], platform, target)
 
 
-qubit_flux_tracking = Routine(
-    _acquisition,
-    qubit_flux_dependence._fit,
-    qubit_flux_dependence._plot,
-    qubit_flux_dependence._update,
-)
-"""QubitFluxTrack Routine object."""
+qubit_spectroscopy = Routine(_acquisition, _fit, _plot, _update)
+"""QubitSpectroscopy Routine object."""
```

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/flux_dependence/resonator_crosstalk.py` & `qibocal-0.0.9/src/qibocal/protocols/rabi/amplitude.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,155 +4,182 @@
 import numpy as np
 import numpy.typing as npt
 from qibolab import AcquisitionType, AveragingMode, ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
 from qibolab.sweeper import Parameter, Sweeper, SweeperType
+from scipy.optimize import curve_fit
+from scipy.signal import find_peaks
 
-from qibocal.auto.operation import Results, Routine
-from qibocal.protocols.characterization.flux_dependence.resonator_flux_dependence import (
-    ResFluxType,
-    ResonatorFluxData,
-    ResonatorFluxParameters,
-    create_flux_pulse_sweepers,
-)
+from qibocal import update
+from qibocal.auto.operation import Data, Routine
+from qibocal.config import log
 
+from ..utils import chi2_reduced
 from . import utils
+from .amplitude_signal import RabiAmplitudeVoltParameters, RabiAmplitudeVoltResults
 
 
 @dataclass
-class ResCrosstalkParameters(ResonatorFluxParameters):
-    """ResonatorFlux runcard inputs."""
-
-    flux_qubits: Optional[list[QubitId]] = None
-    """IDs of the qubits that we will sweep the flux on.
-    If ``None`` flux will be swept on all qubits that we are running the routine on in a multiplex fashion.
-    If given flux will be swept on the given qubits in a sequential fashion (n qubits will result to n different executions).
-    Multiple qubits may be measured in each execution as specified by the ``qubits`` option in the runcard.
-    """
+class RabiAmplitudeParameters(RabiAmplitudeVoltParameters):
+    """RabiAmplitude runcard inputs."""
 
 
 @dataclass
-class ResCrosstalkResults(Results):
-    """Empty fitting outputs for cross talk because fitting is not implemented in this case."""
+class RabiAmplitudeResults(RabiAmplitudeVoltResults):
+    """RabiAmplitude outputs."""
 
+    chi2: dict[QubitId, tuple[float, Optional[float]]] = field(default_factory=dict)
 
-@dataclass
-class ResCrosstalkData(ResonatorFluxData):
-    """QubitFlux acquisition outputs when ``flux_qubits`` are given."""
 
-    data: dict[tuple[QubitId, QubitId], npt.NDArray[ResFluxType]] = field(
-        default_factory=dict
-    )
-    """Raw data acquired for (qubit, qubit_flux) pairs saved in nested dictionaries."""
+RabiAmpType = np.dtype(
+    [("amp", np.float64), ("prob", np.float64), ("error", np.float64)]
+)
+"""Custom dtype for rabi amplitude."""
 
-    def register_qubit(self, qubit, flux_qubit, freq, bias, signal, phase):
-        """Store output for single qubit."""
-        ar = utils.create_data_array(freq, bias, signal, phase, dtype=ResFluxType)
-        if (qubit, flux_qubit) in self.data:
-            self.data[qubit, flux_qubit] = np.rec.array(
-                np.concatenate((self.data[qubit, flux_qubit], ar))
-            )
-        else:
-            self.data[qubit, flux_qubit] = ar
+
+@dataclass
+class RabiAmplitudeData(Data):
+    """RabiAmplitude data acquisition."""
+
+    durations: dict[QubitId, float] = field(default_factory=dict)
+    """Pulse durations provided by the user."""
+    data: dict[QubitId, npt.NDArray[RabiAmpType]] = field(default_factory=dict)
+    """Raw data acquired."""
 
 
 def _acquisition(
-    params: ResCrosstalkParameters, platform: Platform, targets: list[QubitId]
-) -> ResonatorFluxData:
-    """Data acquisition for ResonatorFlux experiment."""
-    # create a sequence of pulses for the experiment:
-    # MZ
+    params: RabiAmplitudeParameters, platform: Platform, targets: list[QubitId]
+) -> RabiAmplitudeData:
+    r"""
+    Data acquisition for Rabi experiment sweeping amplitude.
+    In the Rabi experiment we apply a pulse at the frequency of the qubit and scan the drive pulse amplitude
+    to find the drive pulse amplitude that creates a rotation of a desired angle.
+    """
 
-    # taking advantage of multiplexing, apply the same set of gates to all qubits in parallel
+    # create a sequence of pulses for the experiment
     sequence = PulseSequence()
+    qd_pulses = {}
     ro_pulses = {}
-    bare_resonator_frequency = {}
-    qubit_frequency = {}
+    durations = {}
     for qubit in targets:
-        bare_resonator_frequency[qubit] = platform.qubits[
-            qubit
-        ].bare_resonator_frequency
-        qubit_frequency[qubit] = platform.qubits[qubit].drive_frequency
-
-        ro_pulses[qubit] = platform.create_qubit_readout_pulse(qubit, start=0)
+        qd_pulses[qubit] = platform.create_RX_pulse(qubit, start=0)
+        if params.pulse_length is not None:
+            qd_pulses[qubit].duration = params.pulse_length
+
+        durations[qubit] = qd_pulses[qubit].duration
+        ro_pulses[qubit] = platform.create_qubit_readout_pulse(
+            qubit, start=qd_pulses[qubit].finish
+        )
+        sequence.add(qd_pulses[qubit])
         sequence.add(ro_pulses[qubit])
 
-    # define the parameters to sweep and their range:
-    delta_frequency_range = np.arange(
-        -params.freq_width // 2, params.freq_width // 2, params.freq_step
+    # define the parameter to sweep and its range:
+    # qubit drive pulse amplitude
+    qd_pulse_amplitude_range = np.arange(
+        params.min_amp_factor,
+        params.max_amp_factor,
+        params.step_amp_factor,
     )
-    freq_sweeper = Sweeper(
-        Parameter.frequency,
-        delta_frequency_range,
-        [ro_pulses[qubit] for qubit in targets],
-        type=SweeperType.OFFSET,
+    sweeper = Sweeper(
+        Parameter.amplitude,
+        qd_pulse_amplitude_range,
+        [qd_pulses[qubit] for qubit in targets],
+        type=SweeperType.FACTOR,
     )
 
-    if params.flux_qubits is None:
-        flux_qubits = list(platform.qubits.keys())
+    data = RabiAmplitudeData(durations=durations)
 
-    else:
-        flux_qubits = params.flux_qubits
-    if params.flux_pulses:
-        delta_bias_flux_range, sweepers = create_flux_pulse_sweepers(
-            params, platform, targets, sequence
-        )
-    else:
-        delta_bias_flux_range = np.arange(
-            -params.bias_width / 2, params.bias_width / 2, params.bias_step
+    # sweep the parameter
+    results = platform.sweep(
+        sequence,
+        ExecutionParameters(
+            nshots=params.nshots,
+            relaxation_time=params.relaxation_time,
+            acquisition_type=AcquisitionType.DISCRIMINATION,
+            averaging_mode=AveragingMode.SINGLESHOT,
+        ),
+        sweeper,
+    )
+    for qubit in targets:
+        prob = results[qubit].probability(state=1)
+        data.register_qubit(
+            RabiAmpType,
+            (qubit),
+            dict(
+                amp=qd_pulses[qubit].amplitude * qd_pulse_amplitude_range,
+                prob=prob.tolist(),
+                error=np.sqrt(prob * (1 - prob) / params.nshots).tolist(),
+            ),
         )
-        sweepers = [
-            Sweeper(
-                Parameter.bias,
-                delta_bias_flux_range,
-                qubits=[platform.qubits[flux_qubit]],
-                type=SweeperType.OFFSET,
-            )
-            for flux_qubit in flux_qubits
-        ]
+    return data
 
-    data = ResCrosstalkData(
-        resonator_type=platform.resonator_type,
-        flux_pulses=params.flux_pulses,
-        qubit_frequency=qubit_frequency,
-        bare_resonator_frequency=bare_resonator_frequency,
-    )
-    options = ExecutionParameters(
-        nshots=params.nshots,
-        relaxation_time=params.relaxation_time,
-        acquisition_type=AcquisitionType.INTEGRATION,
-        averaging_mode=AveragingMode.CYCLIC,
-    )
-    for flux_qubit, bias_sweeper in zip(flux_qubits, sweepers):
-        results = platform.sweep(sequence, options, bias_sweeper, freq_sweeper)
-        # retrieve the results for every qubit
-        for qubit in targets:
-            result = results[ro_pulses[qubit].serial]
-            if flux_qubit is None:
-                sweetspot = platform.qubits[qubit].sweetspot
-            else:
-                sweetspot = platform.qubits[flux_qubit].sweetspot
-            data.register_qubit(
-                qubit,
-                flux_qubit,
-                signal=result.magnitude,
-                phase=result.phase,
-                freq=delta_frequency_range + ro_pulses[qubit].frequency,
-                bias=delta_bias_flux_range + sweetspot,
+
+def _fit(data: RabiAmplitudeData) -> RabiAmplitudeResults:
+    """Post-processing for RabiAmplitude."""
+    qubits = data.qubits
+
+    pi_pulse_amplitudes = {}
+    fitted_parameters = {}
+    durations = {}
+    chi2 = {}
+
+    for qubit in qubits:
+        qubit_data = data[qubit]
+
+        x = qubit_data.amp
+        y = qubit_data.prob
+
+        # Guessing period using fourier transform
+        ft = np.fft.rfft(y)
+        mags = abs(ft)
+        local_maxima = find_peaks(mags, threshold=10)[0]
+        index = local_maxima[0] if len(local_maxima) > 0 else None
+        # 0.5 hardcoded guess for less than one oscillation
+        f = x[index] / (x[1] - x[0]) if index is not None else 0.5
+        pguess = [0.5, 0.5, 1 / f, 0]
+        try:
+            popt, perr = curve_fit(
+                utils.rabi_amplitude_function,
+                x,
+                y,
+                p0=pguess,
+                maxfev=100000,
+                bounds=(
+                    [0, 0, 0, -np.pi],
+                    [1, 1, np.inf, np.pi],
+                ),
+                sigma=qubit_data.error,
+            )
+            perr = np.sqrt(np.diag(perr))
+            pi_pulse_parameter = (
+                popt[2] / 2 * utils.period_correction_factor(phase=popt[3])
+            )
+            pi_pulse_amplitudes[qubit] = (pi_pulse_parameter, perr[2] / 2)
+            fitted_parameters[qubit] = popt.tolist()
+            durations = {key: (value, 0) for key, value in data.durations.items()}
+            chi2[qubit] = (
+                chi2_reduced(
+                    y,
+                    utils.rabi_amplitude_function(x, *popt),
+                    qubit_data.error,
+                ),
+                np.sqrt(2 / len(y)),
             )
 
-    return data
+        except Exception as e:
+            log.warning(f"Rabi fit failed for qubit {qubit} due to {e}.")
+    return RabiAmplitudeResults(pi_pulse_amplitudes, durations, fitted_parameters, chi2)
 
 
-def _fit(data: ResCrosstalkData) -> ResCrosstalkResults:
-    return ResCrosstalkResults()
+def _plot(data: RabiAmplitudeData, target: QubitId, fit: RabiAmplitudeResults = None):
+    """Plotting function for RabiAmplitude."""
+    return utils.plot_probabilities(data, target, fit)
 
 
-def _plot(data: ResCrosstalkData, fit: ResCrosstalkResults, target: QubitId):
-    """Plotting function for ResonatorFlux Experiment."""
-    return utils.flux_crosstalk_plot(data, target)
+def _update(results: RabiAmplitudeResults, platform: Platform, target: QubitId):
+    update.drive_amplitude(results.amplitude[target], platform, target)
 
 
-resonator_crosstalk = Routine(_acquisition, _fit, _plot)
-"""Resonator crosstalk Routine object"""
+rabi_amplitude = Routine(_acquisition, _fit, _plot, _update)
+"""RabiAmplitude Routine object."""
```

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/flux_dependence/resonator_flux_dependence.py` & `qibocal-0.0.9/src/qibocal/protocols/flux_dependence/resonator_crosstalk.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,413 +1,361 @@
 from dataclasses import dataclass, field
-from typing import List, Optional, Union
+from typing import Optional
 
 import numpy as np
 import numpy.typing as npt
 from qibolab import AcquisitionType, AveragingMode, ExecutionParameters
-from qibolab.couplers import Coupler
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
 from qibolab.sweeper import Parameter, Sweeper, SweeperType
 from scipy.optimize import curve_fit
 
 from qibocal import update
-from qibocal.auto.operation import Data, Parameters, Qubits, Results, Routine
+from qibocal.auto.operation import Routine
 from qibocal.config import log
 
-from ..utils import GHZ_TO_HZ, HZ_TO_GHZ, table_dict, table_html
+from ..utils import HZ_TO_GHZ, extract_feature, table_dict, table_html
 from . import utils
+from .resonator_flux_dependence import (
+    ResFluxType,
+    ResonatorFluxData,
+    ResonatorFluxParameters,
+    ResonatorFluxResults,
+)
+from .resonator_flux_dependence import _fit as diagonal_fit
 
 
 @dataclass
-class ResonatorFluxParameters(Parameters):
+class ResCrosstalkParameters(ResonatorFluxParameters):
     """ResonatorFlux runcard inputs."""
 
-    freq_width: int
-    """Width for frequency sweep relative to the readout frequency [Hz]."""
-    freq_step: int
-    """Frequency step for sweep [Hz]."""
-    bias_width: Optional[float] = None
-    """Width for bias sweep [V]."""
-    bias_step: Optional[float] = None
-    """Bias step for sweep [a.u.]."""
-    flux_amplitude_start: Optional[Union[int, float, List[float]]] = None
-    """Amplitude start value(s) for flux pulses sweep relative to the qubit sweetspot [a.u.]."""
-    flux_amplitude_end: Optional[Union[int, float, List[float]]] = None
-    """Amplitude end value(s) for flux pulses sweep relative to the qubit sweetspot [a.u.]."""
-    flux_amplitude_step: Optional[Union[int, float, List[float]]] = None
-    """Amplitude step(s) for flux pulses sweep [a.u.]."""
-
-    def __post_init__(self):
-        if not self.has_bias_params:
-            if self.has_flux_params:
-                self.check_flux_params()
-                return
-        if not self.has_flux_params:
-            if self.has_bias_params:
-                return
-        raise ValueError(
-            "Too many arguments provided. Provide either bias_width "
-            "and bias_step or flux_amplitude_width and flux_amplitude_step."
-        )
-
-    def check_flux_params(self):
-        """All flux params must be either all float or all lists with the same length.
-
-        This function does not check if the lenght of the lists is equal to the number
-        of qubits in the experiment.
-        """
-        flux_params = (
-            self.flux_amplitude_start,
-            self.flux_amplitude_end,
-            self.flux_amplitude_step,
-        )
-        if all(isinstance(param, (int, float)) for param in flux_params):
-            return
-
-        if all(isinstance(param, list) for param in flux_params):
-            if all(len(param) == len(flux_params[0]) for param in flux_params):
-                return
-            raise ValueError("Flux lists do not have the same length.")
-        raise ValueError(
-            "flux parameters have the wrong type. Expected one of (int, float, list)."
-        )
-
-    @property
-    def has_bias_params(self):
-        """True if both bias_width and bias_step are set."""
-        return self.bias_width is not None and self.bias_step is not None
-
-    @property
-    def has_flux_params(self):
-        """True if both all flux amplitude parameters are set."""
-        return (
-            self.flux_amplitude_start is not None
-            and self.flux_amplitude_end is not None
-            and self.flux_amplitude_step is not None
-        )
-
-    @property
-    def flux_pulses(self):
-        """True if sweeping flux pulses, False if sweeping bias."""
-        if self.has_flux_params:
-            return True
-        return False
+    flux_qubits: Optional[list[QubitId]] = None
+    """IDs of the qubits that we will sweep the flux on.
+    If ``None`` flux will be swept on all qubits that we are running the routine on in a multiplex fashion.
+    If given flux will be swept on the given qubits in a sequential fashion (n qubits will result to n different executions).
+    Multiple qubits may be measured in each execution as specified by the ``qubits`` option in the runcard.
+    """
 
 
 @dataclass
-class ResonatorFluxResults(Results):
-    """ResonatoFlux outputs."""
+class ResCrosstalkResults(ResonatorFluxResults):
+    """ResCrosstalk outputs."""
 
-    frequency: dict[QubitId, float]
-    """Readout frequency for each qubit."""
-    sweetspot: dict[QubitId, float]
-    """Sweetspot for each qubit."""
-    asymmetry: dict[QubitId, float]
-    """Asymmetry between junctions."""
-    bare_frequency: dict[QubitId, float]
-    """Resonator bare frequency."""
-    drive_frequency: dict[QubitId, float]
-    """Qubit frequency at sweetspot."""
-    fitted_parameters: dict[QubitId, dict[str, float]]
-    """Raw fitting output."""
-    coupling: dict[QubitId, float]
-    """Qubit-resonator coupling."""
-    matrix_element: dict[QubitId, float]
-    """C_ii coefficient."""
-
-
-ResFluxType = np.dtype(
-    [
-        ("freq", np.float64),
-        ("bias", np.float64),
-        ("signal", np.float64),
-        ("phase", np.float64),
-    ]
-)
-"""Custom dtype for resonator flux dependence."""
+    crosstalk_matrix: dict[QubitId, dict[QubitId, float]] = field(default_factory=dict)
+    """Crosstalk matrix element."""
+    fitted_parameters: dict[tuple[QubitId, QubitId], dict] = field(default_factory=dict)
+    """Fitted parameters for each couple target-flux qubit."""
+
+    def __contains__(self, key: QubitId):
+        """Checking if qubit is in crosstalk_matrix attribute."""
+        return key in self.crosstalk_matrix
 
 
 @dataclass
-class ResonatorFluxData(Data):
-    """ResonatorFlux acquisition outputs."""
-
-    resonator_type: str
-    """Resonator type."""
-
-    flux_pulses: bool
-    """True if sweeping flux pulses, False if sweeping bias."""
+class ResCrosstalkData(ResonatorFluxData):
+    """ResFlux acquisition outputs when ``flux_qubits`` are given."""
 
-    qubit_frequency: dict[QubitId, float] = field(default_factory=dict)
-    """Qubit frequencies."""
-
-    bare_resonator_frequency: dict[QubitId, int] = field(default_factory=dict)
-    """Qubit bare resonator frequency power provided by the user."""
-
-    data: dict[QubitId, npt.NDArray[ResFluxType]] = field(default_factory=dict)
-    """Raw data acquired."""
+    sweetspot: dict[QubitId, float] = field(default_factory=dict)
+    """Sweetspot for each qubit."""
+    asymmetry: dict[QubitId, float] = field(default_factory=dict)
+    """Asymmetry for each qubit."""
+    coupling: dict[QubitId, float] = field(default_factory=dict)
+    """Coupling parameter g for each qubit."""
+    voltage: dict[QubitId, float] = field(default_factory=dict)
+    """Voltage provided to each qubit."""
+    resonator_frequency: dict[QubitId, float] = field(default_factory=dict)
+    """Readout resonator frequency for each qubit."""
+    matrix_element: dict[QubitId, float] = field(default_factory=dict)
+    """Diagonal crosstalk matrix element."""
+    data: dict[tuple[QubitId, QubitId], npt.NDArray[ResFluxType]] = field(
+        default_factory=dict
+    )
+    """Raw data acquired for (qubit, qubit_flux) pairs saved in nested dictionaries."""
 
-    def register_qubit(self, qubit, freq, bias, signal, phase):
+    def register_qubit(self, qubit, flux_qubit, freq, bias, signal, phase):
         """Store output for single qubit."""
-        self.data[qubit] = utils.create_data_array(
-            freq, bias, signal, phase, dtype=ResFluxType
-        )
-
-
-def create_flux_pulse_sweepers(
-    params: ResonatorFluxParameters,
-    platform: Platform,
-    qubits: Qubits,
-    sequence: PulseSequence,
-) -> tuple[np.ndarray, list[Sweeper]]:
-    """Create a list of sweepers containing flux pulses.
-
-    Args:
-        params (ResonatorFluxParameters): parameters of the experiment (here flux amplitude is used).
-        platform (Platform): platform on which to run the experiment.
-        qubits (Qubits): qubits on which to run the experiment.
-        sequence (PulseSequence): pulse sequence of the experiment (updated with flux pulses).
-    """
-    qf_pulses = {}
-    for i, qubit in enumerate(qubits):
-        if isinstance(params.flux_amplitude_start, list):
-            flux_amplitude_start = params.flux_amplitude_start[i]
-            flux_amplitude_end = params.flux_amplitude_end[i]
-            flux_amplitude_step = params.flux_amplitude_step[i]
-        else:
-            flux_amplitude_start = params.flux_amplitude_start
-            flux_amplitude_end = params.flux_amplitude_end
-            flux_amplitude_step = params.flux_amplitude_step
-        delta_bias_flux_range = np.arange(
-            flux_amplitude_start,
-            flux_amplitude_end,
-            flux_amplitude_step,
-        )
-        if isinstance(qubit, Coupler):
-            # FIXME: Missmatch with create_coupler_pulse and create_qubit_flux_pulse
-            pulse = platform.create_coupler_pulse(
-                qubit.name,
-                start=0,
-                duration=sequence.duration,
-                amplitude=1,
+        ar = utils.create_data_array(freq, bias, signal, phase, dtype=ResFluxType)
+        if (qubit, flux_qubit) in self.data:
+            self.data[qubit, flux_qubit] = np.rec.array(
+                np.concatenate((self.data[qubit, flux_qubit], ar))
             )
-            qubit = qubit.name
         else:
-            pulse = platform.create_qubit_flux_pulse(
-                qubit, start=0, duration=sequence.duration
-            )
-        qf_pulses[qubit] = pulse
-        sequence.add(pulse)
+            self.data[qubit, flux_qubit] = ar
 
-    # FIXME: This is a patch to fix couplers/qubits
-    if isinstance(qubits[0], Coupler):
-        pulses = [qf_pulses[qubit.name] for qubit in qubits]
-    else:
-        pulses = [qf_pulses[qubit] for qubit in qubits]
-
-    sweepers = [
-        Sweeper(
-            Parameter.amplitude,
-            delta_bias_flux_range,
-            pulses=pulses,
-            type=SweeperType.ABSOLUTE,
+    @property
+    def diagonal(self) -> Optional[ResonatorFluxData]:
+        instance = ResonatorFluxData(
+            resonator_type=self.resonator_type,
+            qubit_frequency=self.qubit_frequency,
+            bare_resonator_frequency=self.bare_resonator_frequency,
+        )
+        for qubit in self.qubits:
+            try:
+                instance.data[qubit] = self.data[qubit, qubit]
+            except KeyError:
+                log.info(
+                    f"Diagonal acquisition not found for qubit {qubit}. Runcard values will be used to perform the off-diagonal fit."
+                )
+
+        if len(instance.data) > 0:
+            return instance
+        return ResonatorFluxData(
+            resonator_type=self.resonator_type,
+            qubit_frequency=self.qubit_frequency,
         )
-    ]
-    return delta_bias_flux_range, sweepers
 
 
 def _acquisition(
-    params: ResonatorFluxParameters, platform: Platform, targets: list[QubitId]
-) -> ResonatorFluxData:
+    params: ResCrosstalkParameters, platform: Platform, targets: list[QubitId]
+) -> ResCrosstalkData:
     """Data acquisition for ResonatorFlux experiment."""
     # create a sequence of pulses for the experiment:
     # MZ
 
     # taking advantage of multiplexing, apply the same set of gates to all qubits in parallel
     sequence = PulseSequence()
     ro_pulses = {}
-    qubit_frequency = {}
     bare_resonator_frequency = {}
+    resonator_frequency = {}
+    qubit_frequency = {}
+    sweetspots = {}
+    asymmetry = {}
+    coupling = {}
+    voltage = {}
+    matrix_element = {}
     for qubit in targets:
-        qubit_frequency[qubit] = platform.qubits[qubit].drive_frequency
+        try:
+            sweetspots[qubit] = voltage[qubit] = platform.qubits[qubit].sweetspot
+            asymmetry[qubit] = platform.qubits[qubit].asymmetry
+            coupling[qubit] = platform.qubits[qubit].g
+            matrix_element[qubit] = platform.qubits[qubit].crosstalk_matrix[qubit]
+        except KeyError:
+            log.warning(f"Missing flux parameters for qubit {qubit}.")
+
         bare_resonator_frequency[qubit] = platform.qubits[
             qubit
         ].bare_resonator_frequency
+        qubit_frequency[qubit] = platform.qubits[qubit].drive_frequency
+        resonator_frequency[qubit] = platform.qubits[qubit].readout_frequency
 
         ro_pulses[qubit] = platform.create_qubit_readout_pulse(qubit, start=0)
         sequence.add(ro_pulses[qubit])
 
     # define the parameters to sweep and their range:
     delta_frequency_range = np.arange(
-        -params.freq_width // 2, params.freq_width // 2, params.freq_step
+        -params.freq_width / 2, params.freq_width / 2, params.freq_step
     )
     freq_sweeper = Sweeper(
         Parameter.frequency,
         delta_frequency_range,
         [ro_pulses[qubit] for qubit in targets],
         type=SweeperType.OFFSET,
     )
-    if params.flux_pulses:
-        delta_bias_flux_range, sweepers = create_flux_pulse_sweepers(
-            params, platform, targets, sequence
-        )
+
+    if params.flux_qubits is None:
+        flux_qubits = list(platform.qubits)
+
     else:
-        delta_bias_flux_range = np.arange(
-            -params.bias_width / 2, params.bias_width / 2, params.bias_step
+        flux_qubits = params.flux_qubits
+
+    delta_bias_range = np.arange(
+        -params.bias_width / 2, params.bias_width / 2, params.bias_step
+    )
+    sequences = [sequence] * len(flux_qubits)
+    sweepers = [
+        Sweeper(
+            Parameter.bias,
+            delta_bias_range,
+            qubits=[platform.qubits[flux_qubit]],
+            type=SweeperType.OFFSET,
         )
-        sweepers = [
-            Sweeper(
-                Parameter.bias,
-                delta_bias_flux_range,
-                qubits=[platform.qubits[qubit] for qubit in targets],
-                type=SweeperType.OFFSET,
-            )
-        ]
+        for flux_qubit in flux_qubits
+    ]
 
-    data = ResonatorFluxData(
+    data = ResCrosstalkData(
         resonator_type=platform.resonator_type,
-        flux_pulses=params.flux_pulses,
         qubit_frequency=qubit_frequency,
+        resonator_frequency=resonator_frequency,
+        sweetspot=sweetspots,
+        voltage=voltage,
+        matrix_element=matrix_element,
+        asymmetry=asymmetry,
+        coupling=coupling,
         bare_resonator_frequency=bare_resonator_frequency,
     )
-
     options = ExecutionParameters(
         nshots=params.nshots,
         relaxation_time=params.relaxation_time,
         acquisition_type=AcquisitionType.INTEGRATION,
         averaging_mode=AveragingMode.CYCLIC,
     )
-    for bias_sweeper in sweepers:
+    for flux_qubit, bias_sweeper, sequence in zip(flux_qubits, sweepers, sequences):
         results = platform.sweep(sequence, options, bias_sweeper, freq_sweeper)
         # retrieve the results for every qubit
         for qubit in targets:
             result = results[ro_pulses[qubit].serial]
-            sweetspot = platform.qubits[qubit].sweetspot
+            if flux_qubit is None:
+                sweetspot = platform.qubits[qubit].sweetspot
+            else:
+                sweetspot = platform.qubits[flux_qubit].sweetspot
             data.register_qubit(
                 qubit,
+                flux_qubit,
                 signal=result.magnitude,
                 phase=result.phase,
                 freq=delta_frequency_range + ro_pulses[qubit].frequency,
-                bias=delta_bias_flux_range + sweetspot,
+                bias=delta_bias_range + sweetspot,
             )
     return data
 
 
-def _fit(data: ResonatorFluxData) -> ResonatorFluxResults:
-    """
-    Post-processing for QubitFlux Experiment. See arxiv:0703002
-    Fit frequency as a function of current for the flux qubit spectroscopy
-    data (QubitFluxData): data object with information on the feature response at each current point.
-    """
+def _fit(data: ResCrosstalkData) -> ResCrosstalkResults:
+    crosstalk_matrix = {qubit: {} for qubit in data.qubit_frequency}
+    fitted_parameters = {}
+    diagonal = diagonal_fit(data.diagonal)
 
-    qubits = data.qubits
-    frequency = {}
+    voltage = {}
     sweetspot = {}
     asymmetry = {}
-    bare_frequency = {}
-    drive_frequency = {}
-    fitted_parameters = {}
-    matrix_element = {}
     coupling = {}
+    matrix_element = {}
+    qubit_frequency = {}
+    bare_resonator_frequency = {}
+    resonator_frequency = {}
 
-    for qubit in qubits:
-        qubit_data = data[qubit]
+    for qubit in data.qubits:
+        condition = qubit in diagonal
+        voltage[qubit] = diagonal.sweetspot[qubit] if condition else data.voltage[qubit]
+        sweetspot[qubit] = (
+            diagonal.sweetspot[qubit] if condition else data.sweetspot[qubit]
+        )
+        asymmetry[qubit] = (
+            diagonal.asymmetry[qubit] if condition else data.asymmetry[qubit]
+        )
+        coupling[qubit] = (
+            diagonal.coupling[qubit] if condition else data.coupling[qubit]
+        )
+        matrix_element[qubit] = (
+            diagonal.matrix_element[qubit] if condition else data.matrix_element[qubit]
+        )
+        qubit_frequency[qubit] = (
+            diagonal.drive_frequency[qubit]
+            if condition
+            else data.qubit_frequency[qubit]
+        )
+        bare_resonator_frequency[qubit] = (
+            diagonal.bare_frequency[qubit]
+            if condition
+            else data.bare_resonator_frequency[qubit]
+        )
+        resonator_frequency[qubit] = (
+            diagonal.frequency[qubit] if condition else data.resonator_frequency[qubit]
+        )
 
-        biases = qubit_data.bias
-        frequencies = qubit_data.freq
-        signal = qubit_data.signal
+    for target_flux_qubit, qubit_data in data.data.items():
+        target_qubit, flux_qubit = target_flux_qubit
 
-        frequencies, biases = utils.extract_feature(frequencies, biases, signal, "min")
+        frequencies, biases = extract_feature(
+            qubit_data.freq, qubit_data.bias, qubit_data.signal, "min"
+        )
 
-        try:
-            popt = curve_fit(
-                utils.transmon_readout_frequency,
-                biases,
-                frequencies * HZ_TO_GHZ,
-                bounds=utils.resonator_flux_dependence_fit_bounds(
-                    data.qubit_frequency[qubit],
-                    qubit_data.bias,
-                    data.bare_resonator_frequency[qubit],
-                ),
-                maxfev=100000,
-            )[0]
-            fitted_parameters[qubit] = popt.tolist()
-
-            # frequency corresponds to transmon readout frequency
-            # at the sweetspot popt[3]
-            frequency[qubit] = (
-                utils.transmon_readout_frequency(popt[3], *popt) * GHZ_TO_HZ
-            )
-            sweetspot[qubit] = popt[3]
-            asymmetry[qubit] = popt[1]
-            bare_frequency[qubit] = popt[4] * GHZ_TO_HZ
-            drive_frequency[qubit] = popt[0] * GHZ_TO_HZ
-            coupling[qubit] = popt[5]
-            matrix_element[qubit] = popt[2]
-        except ValueError as e:
-            log.error(
-                f"Error in resonator_flux protocol fit: {e} "
-                "The threshold for the SNR mask is probably too high. "
-                "Lowering the value of `threshold` in `extract_*_feature`"
-                "should fix the problem."
-            )
+        if target_qubit != flux_qubit:
+            # fit function needs to be defined here to pass correct parameters
+            # at runtime
+            def fit_function(x, crosstalk_element):
+                return utils.transmon_readout_frequency(
+                    xi=voltage[target_qubit],
+                    xj=x,
+                    w_max=qubit_frequency[target_qubit],
+                    d=asymmetry[target_qubit],
+                    sweetspot=sweetspot[target_qubit],
+                    matrix_element=matrix_element[target_qubit],
+                    g=coupling[target_qubit],
+                    resonator_freq=bare_resonator_frequency[target_qubit],
+                    crosstalk_element=crosstalk_element,
+                )
+
+            try:
+                popt, _ = curve_fit(
+                    fit_function, biases, frequencies * HZ_TO_GHZ, bounds=(-1e-1, 1e-1)
+                )
+                fitted_parameters[target_qubit, flux_qubit] = dict(
+                    xi=voltage[target_qubit],
+                    w_max=qubit_frequency[target_qubit],
+                    d=asymmetry[target_qubit],
+                    sweetspot=sweetspot[target_qubit],
+                    matrix_element=matrix_element[target_qubit],
+                    g=coupling[target_qubit],
+                    resonator_freq=bare_resonator_frequency[target_qubit],
+                    crosstalk_element=float(popt),
+                )
+                crosstalk_matrix[target_qubit][flux_qubit] = float(popt)
+            except ValueError as e:
+                log.error(
+                    f"Off-diagonal flux fit failed for qubit {flux_qubit} due to {e}."
+                )
+        else:
+            fitted_parameters[target_qubit, flux_qubit] = diagonal.fitted_parameters[
+                target_qubit
+            ]
+            crosstalk_matrix[target_qubit][flux_qubit] = matrix_element[target_qubit]
 
-    return ResonatorFluxResults(
-        frequency=frequency,
+    return ResCrosstalkResults(
+        frequency=resonator_frequency,
         sweetspot=sweetspot,
         asymmetry=asymmetry,
-        bare_frequency=bare_frequency,
-        drive_frequency=drive_frequency,
+        bare_frequency=bare_resonator_frequency,
+        drive_frequency=qubit_frequency,
         coupling=coupling,
-        matrix_element=matrix_element,
+        crosstalk_matrix=crosstalk_matrix,
         fitted_parameters=fitted_parameters,
     )
 
 
-def _plot(data: ResonatorFluxData, fit: ResonatorFluxResults, target: QubitId):
+def _plot(data: ResCrosstalkData, fit: ResCrosstalkResults, target: QubitId):
     """Plotting function for ResonatorFlux Experiment."""
-    figures = utils.flux_dependence_plot(
-        data, fit, target, utils.transmon_readout_frequency
+    figures, fitting_report = utils.flux_crosstalk_plot(
+        data, target, fit, fit_function=utils.transmon_readout_frequency
     )
-    if data.flux_pulses:
-        bias_flux_unit = "a.u."
-    else:
-        bias_flux_unit = "V"
     if fit is not None:
+        labels = [
+            "Sweetspot [V]",
+            "Resonator Frequency at Sweetspot [Hz]",
+            "Asymmetry d",
+            "Coupling g",
+            "Bare Resonator Frequency [Hz]",
+            "Qubit Frequency [Hz]",
+        ]
+        values = [
+            np.round(fit.sweetspot[target], 4),
+            np.round(fit.frequency[target], 4),
+            np.round(fit.asymmetry[target], 4),
+            np.round(fit.coupling[target], 4),
+            np.round(fit.bare_frequency[target], 4),
+            np.round(fit.drive_frequency[target], 4),
+        ]
+        for flux_qubit in fit.crosstalk_matrix[target]:
+            if flux_qubit != target:
+                labels.append(f"Crosstalk with qubit {flux_qubit}")
+            else:
+                labels.append(f"Flux dependence")
+            values.append(np.round(fit.crosstalk_matrix[target][flux_qubit], 4))
+
         fitting_report = table_html(
             table_dict(
                 target,
-                [
-                    f"Sweetspot [{bias_flux_unit}]",
-                    "Bare Resonator Frequency [Hz]",
-                    "Readout Frequency [Hz]",
-                    "Qubit Frequency at Sweetspot [Hz]",
-                    "Asymmetry d",
-                    "Coupling g",
-                    "V_ii [V]",
-                ],
-                [
-                    np.round(fit.sweetspot[target], 4),
-                    np.round(fit.bare_frequency[target], 4),
-                    np.round(fit.frequency[target], 4),
-                    np.round(fit.drive_frequency[target], 4),
-                    np.round(fit.asymmetry[target], 4),
-                    np.round(fit.coupling[target], 4),
-                    np.round(fit.matrix_element[target], 4),
-                ],
+                labels,
+                values,
             )
         )
-        return figures, fitting_report
-    return figures, ""
+    return figures, fitting_report
 
 
-def _update(results: ResonatorFluxResults, platform: Platform, qubit: QubitId):
-    update.bare_resonator_frequency(results.bare_frequency[qubit], platform, qubit)
-    update.readout_frequency(results.frequency[qubit], platform, qubit)
-    update.drive_frequency(results.drive_frequency[qubit], platform, qubit)
-    update.asymmetry(results.asymmetry[qubit], platform, qubit)
-    update.coupling(results.coupling[qubit], platform, qubit)
+def _update(results: ResCrosstalkResults, platform: Platform, qubit: QubitId):
+    """Update crosstalk matrix."""
+    for flux_qubit, element in results.crosstalk_matrix[qubit].items():
+        update.crosstalk_matrix(element, platform, qubit, flux_qubit)
 
 
-resonator_flux = Routine(_acquisition, _fit, _plot, _update)
-"""ResonatorFlux Routine object."""
+resonator_crosstalk = Routine(_acquisition, _fit, _plot, _update)
+"""Resonator crosstalk Routine object"""
```

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/flux_dependence/utils.py` & `qibocal-0.0.9/src/qibocal/protocols/resonator_punchout.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,295 +1,270 @@
+from dataclasses import dataclass, field
+from typing import Optional
+
 import numpy as np
+import numpy.typing as npt
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
+from qibolab import AcquisitionType, AveragingMode, ExecutionParameters
+from qibolab.platform import Platform
+from qibolab.pulses import PulseSequence
+from qibolab.qubits import QubitId
+from qibolab.sweeper import Parameter, Sweeper, SweeperType
+
+from qibocal import update
+from qibocal.auto.operation import Data, Parameters, Results, Routine
+
+from .utils import HZ_TO_GHZ, fit_punchout, norm, table_dict, table_html
+
+
+@dataclass
+class ResonatorPunchoutParameters(Parameters):
+    """ResonatorPunchout runcard inputs."""
+
+    freq_width: int
+    """Width for frequency sweep relative  to the readout frequency [Hz]."""
+    freq_step: int
+    """Frequency step for sweep [Hz]."""
+    min_amp_factor: float
+    """Minimum amplitude multiplicative factor."""
+    max_amp_factor: float
+    """Maximum amplitude multiplicative factor."""
+    step_amp_factor: float
+    """Step amplitude multiplicative factor."""
+    amplitude: float = None
+    """Initial readout amplitude."""
+
+
+@dataclass
+class ResonatorPunchoutResults(Results):
+    """ResonatorPunchout outputs."""
+
+    readout_frequency: dict[QubitId, float]
+    """Readout frequency [GHz] for each qubit."""
+    bare_frequency: Optional[dict[QubitId, float]]
+    """Bare resonator frequency [GHz] for each qubit."""
+    readout_amplitude: dict[QubitId, float]
+    """Readout amplitude for each qubit."""
+
+
+ResPunchoutType = np.dtype(
+    [
+        ("freq", np.float64),
+        ("amp", np.float64),
+        ("signal", np.float64),
+        ("phase", np.float64),
+    ]
+)
+"""Custom dtype for resonator punchout."""
+
+
+@dataclass
+class ResonatorPunchoutData(Data):
+    """ResonatorPunchout data acquisition."""
+
+    resonator_type: str
+    """Resonator type."""
+    amplitudes: dict[QubitId, float]
+    """Amplitudes provided by the user."""
+    data: dict[QubitId, npt.NDArray[ResPunchoutType]] = field(default_factory=dict)
+    """Raw data acquired."""
+
+    def register_qubit(self, qubit, freq, amp, signal, phase):
+        """Store output for single qubit."""
+        size = len(freq) * len(amp)
+        frequency, amplitude = np.meshgrid(freq, amp)
+        ar = np.empty(size, dtype=ResPunchoutType)
+        ar["freq"] = frequency.ravel()
+        ar["amp"] = amplitude.ravel()
+        ar["signal"] = signal.ravel()
+        ar["phase"] = phase.ravel()
+        self.data[qubit] = np.rec.array(ar)
+
+
+def _acquisition(
+    params: ResonatorPunchoutParameters,
+    platform: Platform,
+    targets: list[QubitId],
+) -> ResonatorPunchoutData:
+    """Data acquisition for Punchout over amplitude."""
+    # create a sequence of pulses for the experiment:
+    # MZ
+
+    # taking advantage of multiplexing, apply the same set of gates to all qubits in parallel
+    sequence = PulseSequence()
+
+    ro_pulses = {}
+    amplitudes = {}
+    for qubit in targets:
+        ro_pulses[qubit] = platform.create_qubit_readout_pulse(qubit, start=0)
+        if params.amplitude is not None:
+            ro_pulses[qubit].amplitude = params.amplitude
+
+        amplitudes[qubit] = ro_pulses[qubit].amplitude
+        sequence.add(ro_pulses[qubit])
+
+    # define the parameters to sweep and their range:
+    # resonator frequency
+    delta_frequency_range = np.arange(
+        -params.freq_width / 2, params.freq_width / 2, params.freq_step
+    )
+    freq_sweeper = Sweeper(
+        Parameter.frequency,
+        delta_frequency_range,
+        [ro_pulses[qubit] for qubit in targets],
+        type=SweeperType.OFFSET,
+    )
+
+    # amplitude
+    amplitude_range = np.arange(
+        params.min_amp_factor, params.max_amp_factor, params.step_amp_factor
+    )
+    amp_sweeper = Sweeper(
+        Parameter.amplitude,
+        amplitude_range,
+        [ro_pulses[qubit] for qubit in targets],
+        type=SweeperType.FACTOR,
+    )
+
+    data = ResonatorPunchoutData(
+        amplitudes=amplitudes,
+        resonator_type=platform.resonator_type,
+    )
+
+    results = platform.sweep(
+        sequence,
+        ExecutionParameters(
+            nshots=params.nshots,
+            relaxation_time=params.relaxation_time,
+            acquisition_type=AcquisitionType.INTEGRATION,
+            averaging_mode=AveragingMode.CYCLIC,
+        ),
+        amp_sweeper,
+        freq_sweeper,
+    )
 
-from ..utils import HZ_TO_GHZ
-
-CONFIDENCE_INTERVAL_FIRST_MASK = 99
-"""Confidence interval used to mask flux data."""
-CONFIDENCE_INTERVAL_SECOND_MASK = 70
-"""Confidence interval used to clean outliers."""
+    # retrieve the results for every qubit
+    for qubit, ro_pulse in ro_pulses.items():
+        # average signal, phase, i and q over the number of shots defined in the runcard
+        result = results[ro_pulse.serial]
+        data.register_qubit(
+            qubit,
+            signal=result.magnitude,
+            phase=result.phase,
+            freq=delta_frequency_range + ro_pulse.frequency,
+            amp=amplitude_range * amplitudes[qubit],
+        )
 
+    return data
 
-def is_crosstalk(data):
-    """Check if keys are tuple which corresponds to crosstalk data structure."""
-    return all(isinstance(key, tuple) for key in data.data.keys())
 
+def _fit(data: ResonatorPunchoutData, fit_type="amp") -> ResonatorPunchoutResults:
+    """Fit frequency and attenuation at high and low power for a given resonator."""
 
-def create_data_array(freq, bias, signal, phase, dtype):
-    """Create custom dtype array for acquired data."""
-    size = len(freq) * len(bias)
-    ar = np.empty(size, dtype=dtype)
-    frequency, biases = np.meshgrid(freq, bias)
-    ar["freq"] = frequency.ravel()
-    ar["bias"] = biases.ravel()
-    ar["signal"] = signal.ravel()
-    ar["phase"] = phase.ravel()
-    return np.rec.array(ar)
+    return ResonatorPunchoutResults(*fit_punchout(data, fit_type))
 
 
-def flux_dependence_plot(data, fit, qubit, fit_function=None):
+def _plot(
+    data: ResonatorPunchoutData, target: QubitId, fit: ResonatorPunchoutResults = None
+):
+    """Plotting function for ResonatorPunchout."""
     figures = []
-    qubit_data = data[qubit]
-    frequencies = qubit_data.freq * HZ_TO_GHZ
-
-    subplot_titles = (
-        "Signal [a.u.]",
-        "Phase [rad]",
-    )
-
+    fitting_report = ""
     fig = make_subplots(
         rows=1,
         cols=2,
         horizontal_spacing=0.1,
-        vertical_spacing=0.1,
-        subplot_titles=subplot_titles,
+        vertical_spacing=0.2,
+        subplot_titles=(
+            "Normalised Signal [a.u.]",
+            "phase [rad]",
+        ),
     )
+    qubit_data = data[target]
+    frequencies = qubit_data.freq * HZ_TO_GHZ
+    amplitudes = qubit_data.amp
+    n_amps = len(np.unique(qubit_data.amp))
+    n_freq = len(np.unique(qubit_data.freq))
+    for i in range(n_amps):
+        qubit_data.signal[i * n_freq : (i + 1) * n_freq] = norm(
+            qubit_data.signal[i * n_freq : (i + 1) * n_freq]
+        )
 
     fig.add_trace(
         go.Heatmap(
-            x=qubit_data.freq * HZ_TO_GHZ,
-            y=qubit_data.bias,
+            x=frequencies,
+            y=amplitudes,
             z=qubit_data.signal,
             colorbar_x=0.46,
         ),
         row=1,
         col=1,
     )
 
-    # TODO: This fit is for frequency, can it be reused here, do we even want the fit ?
-    if (
-        fit is not None
-        and not data.__class__.__name__ == "CouplerSpectroscopyData"
-        and qubit in fit.fitted_parameters
-    ):
-        params = fit.fitted_parameters[qubit]
-        bias = np.unique(qubit_data.bias)
-        fig.add_trace(
-            go.Scatter(
-                x=fit_function(bias, *params),
-                y=bias,
-                showlegend=True,
-                name="Fit",
-                marker=dict(color="black"),
-            ),
-            row=1,
-            col=1,
-        )
-
-    fig.update_xaxes(
-        title_text=f"Frequency [GHz]",
-        row=1,
-        col=1,
-    )
-
-    if data.flux_pulses:
-        fig.update_yaxes(title_text="Flux [a.u.]", row=1, col=1)
-    else:
-        fig.update_yaxes(title_text="Bias [V]", row=1, col=1)
-
     fig.add_trace(
         go.Heatmap(
-            x=qubit_data.freq * HZ_TO_GHZ,
-            y=qubit_data.bias,
+            x=frequencies,
+            y=amplitudes,
             z=qubit_data.phase,
             colorbar_x=1.01,
         ),
         row=1,
         col=2,
     )
-    fig.update_xaxes(
-        title_text=f"Frequency [GHz]",
-        row=1,
-        col=2,
-    )
-
-    fig.update_layout(xaxis1=dict(range=[np.min(frequencies), np.max(frequencies)]))
-
-    fig.update_layout(
-        showlegend=True,
-        legend=dict(orientation="h"),
-    )
-
-    figures.append(fig)
-
-    return figures
-
-
-def flux_crosstalk_plot(data, qubit):
-    figures = []
-    fitting_report = ""
-
-    all_qubit_data = {
-        index: data_qubit
-        for index, data_qubit in data.data.items()
-        if index[0] == qubit
-    }
-
-    fig = make_subplots(
-        rows=1,
-        cols=len(all_qubit_data),
-        horizontal_spacing=0.3 / len(all_qubit_data),
-        vertical_spacing=0.1,
-        subplot_titles=len(all_qubit_data) * ("Signal [a.u.]",),
-    )
-    for col, (flux_qubit, qubit_data) in enumerate(all_qubit_data.items()):
-        frequencies = qubit_data.freq * HZ_TO_GHZ
-        signal = qubit_data.signal
-        if data.resonator_type == "2D":
-            signal = -signal
-
+    if fit is not None:
         fig.add_trace(
-            go.Heatmap(
-                x=frequencies,
-                y=qubit_data.bias,
-                z=qubit_data.signal,
-            ),
-            row=1,
-            col=col + 1,
-        )
-
-        fig.update_xaxes(
-            title_text="Frequency [GHz]",
-            row=1,
-            col=col + 1,
-        )
-
-        if data.flux_pulses:
-            fig.update_yaxes(
-                title_text=f"Qubit {flux_qubit[1]}: Flux [a.u.]", row=1, col=col + 1
+            go.Scatter(
+                x=[
+                    fit.readout_frequency[target] * HZ_TO_GHZ,
+                ],
+                y=[
+                    fit.readout_amplitude[target],
+                ],
+                mode="markers",
+                marker=dict(
+                    size=8,
+                    color="gray",
+                    symbol="circle",
+                ),
+                name="Estimated readout point",
+                showlegend=True,
             )
-        else:
-            fig.update_yaxes(
-                title_text=f"Qubit {flux_qubit[1]}: Bias [V]", row=1, col=col + 1
+        )
+        fitting_report = table_html(
+            table_dict(
+                target,
+                [
+                    "Low Power Resonator Frequency [Hz]",
+                    "Low Power readout amplitude [a.u.]",
+                    "High Power Resonator Frequency [Hz]",
+                ],
+                [
+                    np.round(fit.readout_frequency[target]),
+                    np.round(fit.readout_amplitude[target], 3),
+                    np.round(fit.bare_frequency[target]),
+                ],
             )
+        )
 
-    fig.update_layout(xaxis1=dict(range=[np.min(frequencies), np.max(frequencies)]))
-    fig.update_traces(showscale=False)  # disable colorbar
     fig.update_layout(
-        showlegend=False,
+        showlegend=True,
+        legend=dict(orientation="h"),
     )
 
+    fig.update_xaxes(title_text="Frequency [GHz]", row=1, col=1)
+    fig.update_xaxes(title_text="Frequency [GHz]", row=1, col=2)
+    fig.update_yaxes(title_text="Amplitude [a.u.]", row=1, col=1)
+
     figures.append(fig)
 
     return figures, fitting_report
 
 
-def G_f_d(x, offset, d, element):
-    """Auxiliary function to calculate qubit frequency as a function of bias.
-
-    It also determines the flux dependence of :math:`E_J`,:math:`E_J(\\phi)=E_J(0)G_f_d^2`.
-    For more details see: https://arxiv.org/pdf/cond-mat/0703002.pdf
-
-    Args:
-        offset (float): bias offset.
-        matrix_element(float): constant to convert flux (:math:`\\phi_0`) to bias (:math:`v_0`). Typically denoted as :math:`\\Xi`. :math:`v_0 = \\Xi \\phi_0`.
-        d (float): asymmetry between the two junctions of the transmon.
-                   Typically denoted as :math:`d`. :math:`d = (E_J^1 - E_J^2) / (E_J^1 + E_J^2)`.
-
-    Returns:
-        (float)
-    """
-    return (d**2 + (1 - d**2) * np.cos(np.pi * (x - offset) * element) ** 2) ** 0.25
-
-
-def transmon_frequency(x, w_max, d, element, offset):
-    r"""Approximation to transmon frequency.
-
-    The formula holds in the transmon regime Ej / Ec >> 1.
-
-    See  https://arxiv.org/pdf/cond-mat/0703002.pdf for the complete formula.
-
-    Args:
-         x (float): bias value
-         w_max (float): maximum frequency  :math:`w_{max} = \sqrt{8 E_j E_c}
-         d (float):  d (float): asymmetry between the two junctions of the transmon.
-         element (float): matrix element
-         offset (float): bias corresponding to zero flux (sweetspot).
+def _update(results: ResonatorPunchoutResults, platform: Platform, target: QubitId):
+    update.readout_frequency(results.readout_frequency[target], platform, target)
+    update.bare_resonator_frequency(results.bare_frequency[target], platform, target)
+    update.readout_amplitude(results.readout_amplitude[target], platform, target)
 
-     Returns:
-         (float): qubit frequency as a function of bias.
-    """
-    return w_max * G_f_d(x, offset=offset, d=d, element=element)
 
-
-def transmon_readout_frequency(x, w_max, d, element, offset, resonator_freq, g):
-    r"""Approximation to flux dependent resonator frequency.
-
-    The formula holds in the transmon regime Ej / Ec >> 1.
-
-    See  https://arxiv.org/pdf/cond-mat/0703002.pdf for the complete formula.
-
-    Args:
-         x (float): bias value
-         w_max (float): maximum frequency  :math:`w_{max} = \sqrt{8 E_j E_c}
-         d (float):  d (float): asymmetry between the two junctions of the transmon.
-         element (float): matrix element
-         offset (float): bias corresponding to zero flux (sweetspot).
-         resonator_freq (float): bare resonator frequency [GHz]
-         g (float): readout coupling.
-
-     Returns:
-         (float): resonator frequency as a function of bias.
-    """
-    return resonator_freq + g**2 * G_f_d(x, offset, d, element) / (
-        resonator_freq - transmon_frequency(x, w_max, d, element, offset)
-    )
-
-
-def extract_feature(freq: np.ndarray, bias: np.ndarray, signal: np.ndarray, feat: str):
-    """Extract feature using confidence intervals.
-
-    A first mask is construct by looking at 99% confidence interval for each bias bin.
-    A second mask is applied by looking at 70% confidence interval to remove outliers.
-    """
-
-    masks = []
-    for bias_bin in np.unique(bias):
-        signal_fixed_bias = signal[bias == bias_bin]
-        min, max = np.percentile(
-            signal_fixed_bias,
-            [100 - CONFIDENCE_INTERVAL_FIRST_MASK, CONFIDENCE_INTERVAL_FIRST_MASK],
-        )
-        masks.append(
-            signal_fixed_bias < min if feat == "min" else signal_fixed_bias > max
-        )
-
-    first_mask = np.vstack(masks).ravel()
-    min, max = np.percentile(
-        signal[first_mask],
-        [100 - CONFIDENCE_INTERVAL_SECOND_MASK, CONFIDENCE_INTERVAL_SECOND_MASK],
-    )
-    second_mask = (
-        signal[first_mask] < max if feat == "min" else signal[first_mask] > min
-    )
-    return freq[first_mask][second_mask], bias[first_mask][second_mask]
-
-
-def qubit_flux_dependence_fit_bounds(qubit_frequency: float, bias: np.array):
-    """Returns bounds for qubit flux fit."""
-    return (
-        [
-            qubit_frequency * HZ_TO_GHZ - 1,
-            0,
-            0,
-            np.mean(bias) - 0.5,
-        ],
-        [
-            qubit_frequency * HZ_TO_GHZ + 1,
-            1,
-            np.inf,
-            np.mean(bias) + 0.5,
-        ],
-    )
-
-
-def resonator_flux_dependence_fit_bounds(
-    qubit_frequency: float, bias: np.array, bare_resonator_frequency: float
-):
-    """Returns bounds for resonator flux fit."""
-    left_bound, right_bound = qubit_flux_dependence_fit_bounds(
-        qubit_frequency=qubit_frequency, bias=bias
-    )
-    left_bound += [bare_resonator_frequency * HZ_TO_GHZ - 0.5, 0]
-    right_bound += [bare_resonator_frequency * HZ_TO_GHZ + 0.5, 1]
-    return (left_bound, right_bound)
+resonator_punchout = Routine(_acquisition, _fit, _plot, _update)
+"""ResonatorPunchout Routine object."""
```

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/qubit_spectroscopy.py` & `qibocal-0.0.9/src/qibocal/protocols/readout_optimization/twpa_calibration/frequency.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,168 +1,182 @@
 from dataclasses import dataclass, field
-from typing import Optional
 
 import numpy as np
-from qibolab import AcquisitionType, AveragingMode, ExecutionParameters
+import numpy.typing as npt
+import plotly.graph_objects as go
 from qibolab.platform import Platform
-from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
-from qibolab.sweeper import Parameter, Sweeper, SweeperType
 
 from qibocal import update
-from qibocal.auto.operation import Parameters, Results, Routine
-
-from .resonator_spectroscopy import ResonatorSpectroscopyData, ResSpecType
-from .utils import chi2_reduced, lorentzian, lorentzian_fit, spectroscopy_plot
+from qibocal.auto.operation import Data, Parameters, Results, Routine
+from qibocal.protocols import classification
+from qibocal.protocols.readout_optimization.resonator_frequency import (
+    ResonatorFrequencyType,
+)
+from qibocal.protocols.utils import HZ_TO_GHZ, table_dict, table_html
 
 
 @dataclass
-class QubitSpectroscopyParameters(Parameters):
-    """QubitSpectroscopy runcard inputs."""
+class TwpaFrequencyParameters(Parameters):
+    """TwpaFrequency runcard inputs."""
 
-    freq_width: int
-    """Width [Hz] for frequency sweep relative  to the qubit frequency."""
-    freq_step: int
-    """Frequency [Hz] step for sweep."""
-    drive_duration: int
-    """Drive pulse duration [ns]. Same for all qubits."""
-    drive_amplitude: Optional[float] = None
-    """Drive pulse amplitude (optional). Same for all qubits."""
+    frequency_width: float
+    """Relative frequency width [Hz]"""
+    frequency_step: float
+    """Frequency step [Hz]"""
 
 
 @dataclass
-class QubitSpectroscopyResults(Results):
-    """QubitSpectroscopy outputs."""
+class TwpaFrequencyData(Data):
+    """TwpaFrequency acquisition outputs."""
 
-    frequency: dict[QubitId, dict[str, float]]
-    """Drive frequecy [GHz] for each qubit."""
-    amplitude: dict[QubitId, float]
-    """Input drive amplitude. Same for all qubits."""
-    fitted_parameters: dict[QubitId, list[float]]
-    """Raw fitting output."""
-    chi2_reduced: dict[QubitId, tuple[float, Optional[float]]] = field(
-        default_factory=dict
-    )
-    """Chi2 reduced."""
-    error_fit_pars: dict[QubitId, list] = field(default_factory=dict)
-    """Errors of the fit parameters."""
+    data: dict[
+        tuple[QubitId, float], npt.NDArray[classification.ClassificationType]
+    ] = field(default_factory=dict)
+    """Raw data acquired."""
+    frequencies: dict[QubitId, float] = field(default_factory=dict)
+    """Frequencies for each qubit."""
 
 
-class QubitSpectroscopyData(ResonatorSpectroscopyData):
-    """QubitSpectroscopy acquisition outputs."""
+@dataclass
+class TwpaFrequencyResults(Results):
+    """TwpaFrequency outputs."""
+
+    best_freqs: dict[QubitId, float] = field(default_factory=dict)
+    best_fidelities: dict[QubitId, float] = field(default_factory=dict)
+    best_angles: dict[QubitId, float] = field(default_factory=dict)
+    best_thresholds: dict[QubitId, float] = field(default_factory=dict)
 
 
 def _acquisition(
-    params: QubitSpectroscopyParameters, platform: Platform, targets: list[QubitId]
-) -> QubitSpectroscopyData:
-    """Data acquisition for qubit spectroscopy."""
-    # create a sequence of pulses for the experiment:
-    # long drive probing pulse - MZ
-
-    # taking advantage of multiplexing, apply the same set of gates to all qubits in parallel
-    sequence = PulseSequence()
-    ro_pulses = {}
-    qd_pulses = {}
-    amplitudes = {}
+    params: TwpaFrequencyParameters,
+    platform: Platform,
+    targets: list[QubitId],
+) -> TwpaFrequencyData:
+    r"""
+    Data acquisition for TWPA power optmization.
+    This protocol perform a classification protocol for twpa frequencies
+    in the range [twpa_frequency - frequency_width / 2, twpa_frequency + frequency_width / 2]
+    with step frequency_step.
+
+    Args:
+        params (:class:`TwpaFrequencyParameters`): input parameters
+        platform (:class:`Platform`): Qibolab's platform
+        qubits (dict): dict of target :class:`Qubit` objects to be characterized
+
+    Returns:
+        data (:class:`TwpaFrequencyData`)
+    """
+
+    data = TwpaFrequencyData()
+
+    freq_range = np.arange(
+        -params.frequency_width / 2, params.frequency_width / 2, params.frequency_step
+    ).astype(int)
+
+    initial_twpa_freq = {}
     for qubit in targets:
-        qd_pulses[qubit] = platform.create_qubit_drive_pulse(
-            qubit, start=0, duration=params.drive_duration
+        initial_twpa_freq[qubit] = float(
+            platform.qubits[qubit].twpa.local_oscillator.frequency
         )
-        if params.drive_amplitude is not None:
-            qd_pulses[qubit].amplitude = params.drive_amplitude
-
-        amplitudes[qubit] = qd_pulses[qubit].amplitude
-
-        ro_pulses[qubit] = platform.create_qubit_readout_pulse(
-            qubit, start=qd_pulses[qubit].finish
+        data.frequencies[qubit] = list(
+            float(platform.qubits[qubit].twpa.local_oscillator.frequency) + freq_range
         )
-        sequence.add(qd_pulses[qubit])
-        sequence.add(ro_pulses[qubit])
 
-    # define the parameter to sweep and its range:
-    delta_frequency_range = np.arange(
-        -params.freq_width // 2, params.freq_width // 2, params.freq_step
-    )
-    sweeper = Sweeper(
-        Parameter.frequency,
-        delta_frequency_range,
-        pulses=[qd_pulses[qubit] for qubit in targets],
-        type=SweeperType.OFFSET,
-    )
-
-    # Create data structure for data acquisition.
-    data = QubitSpectroscopyData(
-        resonator_type=platform.resonator_type, amplitudes=amplitudes
-    )
-
-    results = platform.sweep(
-        sequence,
-        ExecutionParameters(
-            nshots=params.nshots,
-            relaxation_time=params.relaxation_time,
-            acquisition_type=AcquisitionType.INTEGRATION,
-            averaging_mode=AveragingMode.SINGLESHOT,
-        ),
-        sweeper,
-    )
+    for freq in freq_range:
+        for qubit in targets:
+            platform.qubits[qubit].twpa.local_oscillator.frequency = (
+                initial_twpa_freq[qubit] + freq
+            )
 
-    # retrieve the results for every qubit
-    for qubit, ro_pulse in ro_pulses.items():
-        result = results[ro_pulse.serial]
-        # store the results
-        data.register_qubit(
-            ResSpecType,
-            (qubit),
-            dict(
-                signal=np.abs(result.average.voltage),
-                phase=np.mean(result.phase, axis=0),
-                freq=delta_frequency_range + qd_pulses[qubit].frequency,
-                error_signal=result.average.std,
-                error_phase=np.std(result.phase, axis=0, ddof=1),
+        classification_data = classification._acquisition(
+            classification.SingleShotClassificationParameters.load(
+                {"nshots": params.nshots}
             ),
+            platform,
+            targets,
         )
+        classification_result = classification._fit(classification_data)
+        for qubit in targets:
+            data.register_qubit(
+                ResonatorFrequencyType,
+                (qubit),
+                dict(
+                    freq=np.array(
+                        [platform.qubits[qubit].twpa.local_oscillator.frequency],
+                        dtype=np.float64,
+                    ),
+                    assignment_fidelity=np.array(
+                        [classification_result.assignment_fidelity[qubit]],
+                    ),
+                    angle=np.array([classification_result.rotation_angle[qubit]]),
+                    threshold=np.array([classification_result.threshold[qubit]]),
+                ),
+            )
     return data
 
 
-def _fit(data: QubitSpectroscopyData) -> QubitSpectroscopyResults:
-    """Post-processing function for QubitSpectroscopy."""
+def _fit(data: TwpaFrequencyData) -> TwpaFrequencyResults:
+    """Extract fidelity for each configuration qubit / param.
+    Where param can be either frequency or power."""
+
     qubits = data.qubits
-    frequency = {}
-    fitted_parameters = {}
-    error_fit_pars = {}
-    chi2 = {}
+    best_freq = {}
+    best_fidelity = {}
+    best_angle = {}
+    best_threshold = {}
     for qubit in qubits:
-        fit_result = lorentzian_fit(
-            data[qubit], resonator_type=data.resonator_type, fit="qubit"
-        )
-        if fit_result is not None:
-            frequency[qubit], fitted_parameters[qubit], error_fit_pars[qubit] = (
-                fit_result
-            )
-            chi2[qubit] = (
-                chi2_reduced(
-                    data[qubit].signal,
-                    lorentzian(data[qubit].freq, *fitted_parameters[qubit]),
-                    data[qubit].error_signal,
-                ),
-                np.sqrt(2 / len(data[qubit].freq)),
-            )
-    return QubitSpectroscopyResults(
-        frequency=frequency,
-        fitted_parameters=fitted_parameters,
-        amplitude=data.amplitudes,
-        error_fit_pars=error_fit_pars,
-        chi2_reduced=chi2,
+        data_qubit = data[qubit]
+        index_best_err = np.argmax(data_qubit["assignment_fidelity"])
+        best_fidelity[qubit] = data_qubit["assignment_fidelity"][index_best_err]
+        best_freq[qubit] = data_qubit["freq"][index_best_err]
+        best_angle[qubit] = data_qubit["angle"][index_best_err]
+        best_threshold[qubit] = data_qubit["threshold"][index_best_err]
+
+    return TwpaFrequencyResults(
+        best_freq, best_fidelity, best_thresholds=best_threshold, best_angles=best_angle
     )
 
 
-def _plot(data: QubitSpectroscopyData, target: QubitId, fit: QubitSpectroscopyResults):
-    """Plotting function for QubitSpectroscopy."""
-    return spectroscopy_plot(data, target, fit)
+def _plot(data: TwpaFrequencyData, fit: TwpaFrequencyResults, target: QubitId):
+    """Plotting function that shows the assignment fidelity
+    for different values of the twpa frequency for a single qubit"""
+
+    figures = []
+    fitting_report = ""
+    if fit is not None:
+        qubit_data = data.data[target]
+        fidelities = qubit_data["assignment_fidelity"]
+        frequencies = qubit_data["freq"]
+        fitting_report = table_html(
+            table_dict(
+                target,
+                ["Best assignment fidelity", "TWPA Frequency [Hz]"],
+                [
+                    np.round(fit.best_fidelities[target], 3),
+                    fit.best_freqs[target],
+                ],
+            )
+        )
+        fig = go.Figure(
+            [go.Scatter(x=frequencies * HZ_TO_GHZ, y=fidelities, name="Fidelity")]
+        )
+
+        fig.update_layout(
+            showlegend=True,
+            xaxis_title="TWPA Frequency [GHz]",
+            yaxis_title="Assignment Fidelity",
+        )
+
+        figures.append(fig)
+
+    return figures, fitting_report
 
 
-def _update(results: QubitSpectroscopyResults, platform: Platform, target: QubitId):
-    update.drive_frequency(results.frequency[target], platform, target)
+def _update(results: TwpaFrequencyResults, platform: Platform, target: QubitId):
+    update.twpa_frequency(results.best_freqs[target], platform, target)
+    update.iq_angle(results.best_angles[target], platform, target)
+    update.threshold(results.best_thresholds[target], platform, target)
 
 
-qubit_spectroscopy = Routine(_acquisition, _fit, _plot, _update)
-"""QubitSpectroscopy Routine object."""
+twpa_frequency = Routine(_acquisition, _fit, _plot, _update)
+"""Twpa frequency Routine  object."""
```

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/qubit_spectroscopy_ef.py` & `qibocal-0.0.9/src/qibocal/protocols/qubit_spectroscopy_ef.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from dataclasses import asdict, dataclass, field
 
 import numpy as np
-from qibolab import AcquisitionType, AveragingMode, ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
 from qibolab.sweeper import Parameter, Sweeper, SweeperType
 
 from qibocal import update
 from qibocal.auto.operation import Routine
@@ -120,65 +119,79 @@
         resonator_type=platform.resonator_type,
         amplitudes=amplitudes,
         drive_frequencies=drive_frequencies,
     )
 
     results = platform.sweep(
         sequence,
-        ExecutionParameters(
-            nshots=params.nshots,
-            relaxation_time=params.relaxation_time,
-            acquisition_type=AcquisitionType.INTEGRATION,
-            averaging_mode=AveragingMode.SINGLESHOT,
-        ),
+        params.execution_parameters,
         sweeper,
     )
 
     # retrieve the results for every qubit
     for qubit, ro_pulse in ro_pulses.items():
         result = results[ro_pulse.serial]
         # store the results
         data.register_qubit(
             ResSpecType,
             (qubit),
             dict(
-                signal=np.abs(result.average.voltage),
-                phase=np.mean(result.phase, axis=0),
+                signal=result.average.magnitude,
+                phase=result.average.phase,
                 freq=delta_frequency_range + qd_pulses[qubit].frequency,
                 error_signal=result.average.std,
-                error_phase=np.std(result.phase, axis=0, ddof=1),
+                error_phase=result.phase_std,
             ),
         )
     return data
 
 
 def _plot(
     data: QubitSpectroscopyEFData, target: QubitId, fit: QubitSpectroscopyEFResults
 ):
     """Plotting function for QubitSpectroscopy."""
     figures, report = spectroscopy_plot(data, target, fit)
+    show_error_bars = not np.isnan(data[target].error_signal).any()
     if fit is not None:
-        report = table_html(
-            table_dict(
-                target,
-                [
-                    "Frequency 1->2 [Hz]",
-                    "Amplitude [a.u.]",
-                    "Anharmonicity [Hz]",
-                    "Chi2",
-                ],
-                [
-                    (fit.frequency[target], fit.error_fit_pars[target][1]),
-                    (fit.amplitude[target], fit.error_fit_pars[target][0]),
-                    (fit.anharmonicity[target], fit.error_fit_pars[target][2]),
-                    fit.chi2_reduced[target],
-                ],
-                display_error=True,
+        if show_error_bars:
+            report = table_html(
+                table_dict(
+                    target,
+                    [
+                        "Frequency 1->2 [Hz]",
+                        "Amplitude [a.u.]",
+                        "Anharmonicity [Hz]",
+                        "Chi2",
+                    ],
+                    [
+                        (fit.frequency[target], fit.error_fit_pars[target][1]),
+                        (fit.amplitude[target], fit.error_fit_pars[target][0]),
+                        (fit.anharmonicity[target], fit.error_fit_pars[target][2]),
+                        fit.chi2_reduced[target],
+                    ],
+                    display_error=True,
+                )
+            )
+        else:
+            report = table_html(
+                table_dict(
+                    target,
+                    [
+                        "Frequency 1->2 [Hz]",
+                        "Amplitude [a.u.]",
+                        "Anharmonicity [Hz]",
+                    ],
+                    [
+                        fit.frequency[target],
+                        fit.amplitude[target],
+                        fit.anharmonicity[target],
+                    ],
+                    display_error=False,
+                )
             )
-        )
 
     return figures, report
 
 
 def _update(results: QubitSpectroscopyEFResults, platform: Platform, target: QubitId):
     """Update w12 frequency"""
     update.frequency_12_transition(results.frequency[target], platform, target)
```

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/qutrit_classification.py` & `qibocal-0.0.9/src/qibocal/protocols/qutrit_classification.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,25 +5,21 @@
 from qibolab import AcquisitionType, ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
 
 from qibocal.auto.operation import Routine
 from qibocal.fitting.classifier import run
-from qibocal.protocols.characterization.classification import (
+from qibocal.protocols.classification import (
     ClassificationType,
     SingleShotClassificationData,
     SingleShotClassificationParameters,
     SingleShotClassificationResults,
 )
-from qibocal.protocols.characterization.utils import (
-    MESH_SIZE,
-    evaluate_grid,
-    plot_results,
-)
+from qibocal.protocols.utils import MESH_SIZE, evaluate_grid, plot_results
 
 COLUMNWIDTH = 600
 LEGEND_FONT_SIZE = 20
 TITLE_SIZE = 25
 SPACING = 0.1
 DEFAULT_CLASSIFIER = "naive_bayes"
```

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/rabi/amplitude.py` & `qibocal-0.0.9/src/qibocal/protocols/rabi/length.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,178 +8,207 @@
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
 from qibolab.sweeper import Parameter, Sweeper, SweeperType
 from scipy.optimize import curve_fit
 from scipy.signal import find_peaks
 
 from qibocal import update
-from qibocal.auto.operation import Data, Routine
+from qibocal.auto.operation import Parameters, Routine
 from qibocal.config import log
+from qibocal.protocols.rabi.length_signal import (
+    RabiLengthVoltData,
+    RabiLengthVoltResults,
+)
 
 from ..utils import chi2_reduced
 from . import utils
-from .amplitude_signal import RabiAmplitudeVoltParameters, RabiAmplitudeVoltResults
 
 
 @dataclass
-class RabiAmplitudeParameters(RabiAmplitudeVoltParameters):
-    """RabiAmplitude runcard inputs."""
+class RabiLengthParameters(Parameters):
+    """RabiLength runcard inputs."""
+
+    pulse_duration_start: float
+    """Initial pi pulse duration [ns]."""
+    pulse_duration_end: float
+    """Final pi pulse duration [ns]."""
+    pulse_duration_step: float
+    """Step pi pulse duration [ns]."""
+    pulse_amplitude: Optional[float] = None
+    """Pi pulse amplitude. Same for all qubits."""
 
 
 @dataclass
-class RabiAmplitudeResults(RabiAmplitudeVoltResults):
-    """RabiAmplitude outputs."""
+class RabiLengthResults(RabiLengthVoltResults):
+    """RabiLength outputs."""
 
     chi2: dict[QubitId, tuple[float, Optional[float]]] = field(default_factory=dict)
 
 
-RabiAmpType = np.dtype(
-    [("amp", np.float64), ("prob", np.float64), ("error", np.float64)]
+RabiLenType = np.dtype(
+    [("length", np.float64), ("prob", np.float64), ("error", np.float64)]
 )
 """Custom dtype for rabi amplitude."""
 
 
 @dataclass
-class RabiAmplitudeData(Data):
-    """RabiAmplitude data acquisition."""
+class RabiLengthData(RabiLengthVoltData):
+    """RabiLength acquisition outputs."""
 
-    durations: dict[QubitId, float] = field(default_factory=dict)
-    """Pulse durations provided by the user."""
-    data: dict[QubitId, npt.NDArray[RabiAmpType]] = field(default_factory=dict)
+    data: dict[QubitId, npt.NDArray[RabiLenType]] = field(default_factory=dict)
     """Raw data acquired."""
 
 
 def _acquisition(
-    params: RabiAmplitudeParameters, platform: Platform, targets: list[QubitId]
-) -> RabiAmplitudeData:
+    params: RabiLengthParameters, platform: Platform, targets: list[QubitId]
+) -> RabiLengthData:
     r"""
-    Data acquisition for Rabi experiment sweeping amplitude.
-    In the Rabi experiment we apply a pulse at the frequency of the qubit and scan the drive pulse amplitude
-    to find the drive pulse amplitude that creates a rotation of a desired angle.
+    Data acquisition for RabiLength Experiment.
+    In the Rabi experiment we apply a pulse at the frequency of the qubit and scan the drive pulse length
+    to find the drive pulse length that creates a rotation of a desired angle.
     """
 
     # create a sequence of pulses for the experiment
     sequence = PulseSequence()
     qd_pulses = {}
     ro_pulses = {}
-    durations = {}
+    amplitudes = {}
     for qubit in targets:
-        qd_pulses[qubit] = platform.create_RX_pulse(qubit, start=0)
-        if params.pulse_length is not None:
-            qd_pulses[qubit].duration = params.pulse_length
+        # TODO: made duration optional for qd pulse?
+        qd_pulses[qubit] = platform.create_qubit_drive_pulse(
+            qubit, start=0, duration=params.pulse_duration_start
+        )
+        if params.pulse_amplitude is not None:
+            qd_pulses[qubit].amplitude = params.pulse_amplitude
+        amplitudes[qubit] = qd_pulses[qubit].amplitude
 
-        durations[qubit] = qd_pulses[qubit].duration
         ro_pulses[qubit] = platform.create_qubit_readout_pulse(
             qubit, start=qd_pulses[qubit].finish
         )
         sequence.add(qd_pulses[qubit])
         sequence.add(ro_pulses[qubit])
 
     # define the parameter to sweep and its range:
-    # qubit drive pulse amplitude
-    qd_pulse_amplitude_range = np.arange(
-        params.min_amp_factor,
-        params.max_amp_factor,
-        params.step_amp_factor,
+    # qubit drive pulse duration time
+    qd_pulse_duration_range = np.arange(
+        params.pulse_duration_start,
+        params.pulse_duration_end,
+        params.pulse_duration_step,
     )
+
     sweeper = Sweeper(
-        Parameter.amplitude,
-        qd_pulse_amplitude_range,
+        Parameter.duration,
+        qd_pulse_duration_range,
         [qd_pulses[qubit] for qubit in targets],
-        type=SweeperType.FACTOR,
+        type=SweeperType.ABSOLUTE,
     )
 
-    data = RabiAmplitudeData(durations=durations)
+    data = RabiLengthData(amplitudes=amplitudes)
 
-    # sweep the parameter
+    # execute the sweep
     results = platform.sweep(
         sequence,
         ExecutionParameters(
             nshots=params.nshots,
             relaxation_time=params.relaxation_time,
             acquisition_type=AcquisitionType.DISCRIMINATION,
             averaging_mode=AveragingMode.SINGLESHOT,
         ),
         sweeper,
     )
+
     for qubit in targets:
         prob = results[qubit].probability(state=1)
         data.register_qubit(
-            RabiAmpType,
+            RabiLenType,
             (qubit),
             dict(
-                amp=qd_pulses[qubit].amplitude * qd_pulse_amplitude_range,
-                prob=prob.tolist(),
+                length=qd_pulse_duration_range,
+                prob=prob,
                 error=np.sqrt(prob * (1 - prob) / params.nshots).tolist(),
             ),
         )
     return data
 
 
-def _fit(data: RabiAmplitudeData) -> RabiAmplitudeResults:
-    """Post-processing for RabiAmplitude."""
-    qubits = data.qubits
+def _fit(data: RabiLengthData) -> RabiLengthResults:
+    """Post-processing for RabiLength experiment."""
 
-    pi_pulse_amplitudes = {}
+    qubits = data.qubits
     fitted_parameters = {}
     durations = {}
+    amplitudes = {}
     chi2 = {}
 
     for qubit in qubits:
         qubit_data = data[qubit]
-
-        x = qubit_data.amp
+        raw_x = qubit_data.length
+        min_x = np.min(raw_x)
+        max_x = np.max(raw_x)
         y = qubit_data.prob
 
+        x = (raw_x - min_x) / (max_x - min_x)
         # Guessing period using fourier transform
         ft = np.fft.rfft(y)
         mags = abs(ft)
-        local_maxima = find_peaks(mags, threshold=10)[0]
+        local_maxima = find_peaks(mags, threshold=1)[0]
         index = local_maxima[0] if len(local_maxima) > 0 else None
         # 0.5 hardcoded guess for less than one oscillation
         f = x[index] / (x[1] - x[0]) if index is not None else 0.5
-        pguess = [0.5, 0.5, 1 / f, 0]
+        pguess = [0.5, 0.5, 1 / f, 0, 0]
+
         try:
             popt, perr = curve_fit(
-                utils.rabi_amplitude_function,
+                utils.rabi_length_function,
                 x,
                 y,
                 p0=pguess,
                 maxfev=100000,
                 bounds=(
-                    [0, 0, 0, -np.pi],
-                    [1, 1, np.inf, np.pi],
+                    [0, 0, 0, -np.pi, 0],
+                    [1, 1, np.inf, np.pi, np.inf],
                 ),
                 sigma=qubit_data.error,
             )
+
+            translated_popt = [
+                popt[0],
+                popt[1] * np.exp(min_x * popt[4] / (max_x - min_x)),
+                popt[2] * (max_x - min_x),
+                popt[3] - 2 * np.pi * min_x / popt[2] / (max_x - min_x),
+                popt[4] / (max_x - min_x),
+            ]
+
             perr = np.sqrt(np.diag(perr))
             pi_pulse_parameter = (
-                popt[2] / 2 * utils.period_correction_factor(phase=popt[3])
+                translated_popt[2]
+                / 2
+                * utils.period_correction_factor(phase=translated_popt[3])
             )
-            pi_pulse_amplitudes[qubit] = (pi_pulse_parameter, perr[2] / 2)
-            fitted_parameters[qubit] = popt.tolist()
-            durations = {key: (value, 0) for key, value in data.durations.items()}
+            durations[qubit] = (pi_pulse_parameter, perr[2] * (max_x - min_x) / 2)
+            fitted_parameters[qubit] = translated_popt
+            amplitudes = {key: (value, 0) for key, value in data.amplitudes.items()}
             chi2[qubit] = (
                 chi2_reduced(
                     y,
-                    utils.rabi_amplitude_function(x, *popt),
+                    utils.rabi_length_function(raw_x, *translated_popt),
                     qubit_data.error,
                 ),
                 np.sqrt(2 / len(y)),
             )
-
         except Exception as e:
             log.warning(f"Rabi fit failed for qubit {qubit} due to {e}.")
-    return RabiAmplitudeResults(pi_pulse_amplitudes, durations, fitted_parameters, chi2)
 
+    return RabiLengthResults(durations, amplitudes, fitted_parameters, chi2)
 
-def _plot(data: RabiAmplitudeData, target: QubitId, fit: RabiAmplitudeResults = None):
-    """Plotting function for RabiAmplitude."""
-    return utils.plot_probabilities(data, target, fit)
 
+def _update(results: RabiLengthResults, platform: Platform, target: QubitId):
+    update.drive_duration(results.length[target], platform, target)
 
-def _update(results: RabiAmplitudeResults, platform: Platform, target: QubitId):
-    update.drive_amplitude(results.amplitude[target], platform, target)
+
+def _plot(data: RabiLengthData, fit: RabiLengthResults, target: QubitId):
+    """Plotting function for RabiLength experiment."""
+    return utils.plot_probabilities(data, target, fit)
 
 
-rabi_amplitude = Routine(_acquisition, _fit, _plot, _update)
-"""RabiAmplitude Routine object."""
+rabi_length = Routine(_acquisition, _fit, _plot, _update)
+"""RabiLength Routine object."""
```

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/rabi/amplitude_signal.py` & `qibocal-0.0.9/src/qibocal/protocols/rabi/amplitude_signal.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/rabi/ef.py` & `qibocal-0.0.9/src/qibocal/protocols/rabi/ef.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/rabi/length.py` & `qibocal-0.0.9/src/qibocal/protocols/rabi/length_signal.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,63 +8,65 @@
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
 from qibolab.sweeper import Parameter, Sweeper, SweeperType
 from scipy.optimize import curve_fit
 from scipy.signal import find_peaks
 
 from qibocal import update
-from qibocal.auto.operation import Parameters, Routine
+from qibocal.auto.operation import Data, Parameters, Results, Routine
 from qibocal.config import log
-from qibocal.protocols.characterization.rabi.length_signal import (
-    RabiLengthVoltData,
-    RabiLengthVoltResults,
-)
 
-from ..utils import chi2_reduced
 from . import utils
 
 
 @dataclass
-class RabiLengthParameters(Parameters):
-    """RabiLength runcard inputs."""
+class RabiLengthVoltParameters(Parameters):
+    """RabiLengthVolt runcard inputs."""
 
     pulse_duration_start: float
     """Initial pi pulse duration [ns]."""
     pulse_duration_end: float
     """Final pi pulse duration [ns]."""
     pulse_duration_step: float
     """Step pi pulse duration [ns]."""
     pulse_amplitude: Optional[float] = None
     """Pi pulse amplitude. Same for all qubits."""
 
 
 @dataclass
-class RabiLengthResults(RabiLengthVoltResults):
-    """RabiLength outputs."""
+class RabiLengthVoltResults(Results):
+    """RabiLengthVolt outputs."""
 
-    chi2: dict[QubitId, tuple[float, Optional[float]]] = field(default_factory=dict)
+    length: dict[QubitId, tuple[int, Optional[float]]]
+    """Pi pulse duration for each qubit."""
+    amplitude: dict[QubitId, tuple[float, Optional[float]]]
+    """Pi pulse amplitude. Same for all qubits."""
+    fitted_parameters: dict[QubitId, dict[str, float]]
+    """Raw fitting output."""
 
 
-RabiLenType = np.dtype(
-    [("length", np.float64), ("prob", np.float64), ("error", np.float64)]
+RabiLenVoltType = np.dtype(
+    [("length", np.float64), ("signal", np.float64), ("phase", np.float64)]
 )
 """Custom dtype for rabi amplitude."""
 
 
 @dataclass
-class RabiLengthData(RabiLengthVoltData):
+class RabiLengthVoltData(Data):
     """RabiLength acquisition outputs."""
 
-    data: dict[QubitId, npt.NDArray[RabiLenType]] = field(default_factory=dict)
+    amplitudes: dict[QubitId, float] = field(default_factory=dict)
+    """Pulse durations provided by the user."""
+    data: dict[QubitId, npt.NDArray[RabiLenVoltType]] = field(default_factory=dict)
     """Raw data acquired."""
 
 
 def _acquisition(
-    params: RabiLengthParameters, platform: Platform, targets: list[QubitId]
-) -> RabiLengthData:
+    params: RabiLengthVoltParameters, platform: Platform, targets: list[QubitId]
+) -> RabiLengthVoltData:
     r"""
     Data acquisition for RabiLength Experiment.
     In the Rabi experiment we apply a pulse at the frequency of the qubit and scan the drive pulse length
     to find the drive pulse length that creates a rotation of a desired angle.
     """
 
     # create a sequence of pulses for the experiment
@@ -98,117 +100,107 @@
     sweeper = Sweeper(
         Parameter.duration,
         qd_pulse_duration_range,
         [qd_pulses[qubit] for qubit in targets],
         type=SweeperType.ABSOLUTE,
     )
 
-    data = RabiLengthData(amplitudes=amplitudes)
+    data = RabiLengthVoltData(amplitudes=amplitudes)
 
     # execute the sweep
     results = platform.sweep(
         sequence,
         ExecutionParameters(
             nshots=params.nshots,
             relaxation_time=params.relaxation_time,
-            acquisition_type=AcquisitionType.DISCRIMINATION,
-            averaging_mode=AveragingMode.SINGLESHOT,
+            acquisition_type=AcquisitionType.INTEGRATION,
+            averaging_mode=AveragingMode.CYCLIC,
         ),
         sweeper,
     )
 
     for qubit in targets:
-        prob = results[qubit].probability(state=1)
+        result = results[ro_pulses[qubit].serial]
         data.register_qubit(
-            RabiLenType,
+            RabiLenVoltType,
             (qubit),
             dict(
                 length=qd_pulse_duration_range,
-                prob=prob,
-                error=np.sqrt(prob * (1 - prob) / params.nshots).tolist(),
+                signal=result.magnitude,
+                phase=result.phase,
             ),
         )
     return data
 
 
-def _fit(data: RabiLengthData) -> RabiLengthResults:
+def _fit(data: RabiLengthVoltData) -> RabiLengthVoltResults:
     """Post-processing for RabiLength experiment."""
 
     qubits = data.qubits
     fitted_parameters = {}
     durations = {}
-    amplitudes = {}
-    chi2 = {}
 
     for qubit in qubits:
         qubit_data = data[qubit]
-        raw_x = qubit_data.length
-        min_x = np.min(raw_x)
-        max_x = np.max(raw_x)
-        y = qubit_data.prob
+        rabi_parameter = qubit_data.length
+        voltages = qubit_data.signal
+
+        y_min = np.min(voltages)
+        y_max = np.max(voltages)
+        x_min = np.min(rabi_parameter)
+        x_max = np.max(rabi_parameter)
+        x = (rabi_parameter - x_min) / (x_max - x_min)
+        y = (voltages - y_min) / (y_max - y_min) - 1 / 2
 
-        x = (raw_x - min_x) / (max_x - min_x)
         # Guessing period using fourier transform
         ft = np.fft.rfft(y)
         mags = abs(ft)
         local_maxima = find_peaks(mags, threshold=1)[0]
         index = local_maxima[0] if len(local_maxima) > 0 else None
         # 0.5 hardcoded guess for less than one oscillation
         f = x[index] / (x[1] - x[0]) if index is not None else 0.5
-        pguess = [0.5, 0.5, 1 / f, 0, 0]
 
+        pguess = [0, np.sign(y[0]) * 0.5, 1 / f, 0, 0]
         try:
-            popt, perr = curve_fit(
+            popt, _ = curve_fit(
                 utils.rabi_length_function,
                 x,
                 y,
                 p0=pguess,
                 maxfev=100000,
                 bounds=(
-                    [0, 0, 0, -np.pi, 0],
+                    [0, -1, 0, -np.pi, 0],
                     [1, 1, np.inf, np.pi, np.inf],
                 ),
-                sigma=qubit_data.error,
             )
-
-            translated_popt = [
-                popt[0],
-                popt[1] * np.exp(min_x * popt[4] / (max_x - min_x)),
-                popt[2] * (max_x - min_x),
-                popt[3] - 2 * np.pi * min_x / popt[2] / (max_x - min_x),
-                popt[4] / (max_x - min_x),
+            translated_popt = [  # change it according to the fit function
+                (y_max - y_min) * (popt[0] + 1 / 2) + y_min,
+                (y_max - y_min) * popt[1] * np.exp(x_min * popt[4] / (x_max - x_min)),
+                popt[2] * (x_max - x_min),
+                popt[3] - 2 * np.pi * x_min / popt[2] / (x_max - x_min),
+                popt[4] / (x_max - x_min),
             ]
-
-            perr = np.sqrt(np.diag(perr))
             pi_pulse_parameter = (
                 translated_popt[2]
                 / 2
                 * utils.period_correction_factor(phase=translated_popt[3])
             )
-            durations[qubit] = (pi_pulse_parameter, perr[2] * (max_x - min_x) / 2)
+            durations[qubit] = pi_pulse_parameter
             fitted_parameters[qubit] = translated_popt
-            amplitudes = {key: (value, 0) for key, value in data.amplitudes.items()}
-            chi2[qubit] = (
-                chi2_reduced(
-                    y,
-                    utils.rabi_length_function(raw_x, *translated_popt),
-                    qubit_data.error,
-                ),
-                np.sqrt(2 / len(y)),
-            )
+
         except Exception as e:
             log.warning(f"Rabi fit failed for qubit {qubit} due to {e}.")
 
-    return RabiLengthResults(durations, amplitudes, fitted_parameters, chi2)
+    return RabiLengthVoltResults(durations, data.amplitudes, fitted_parameters)
 
 
-def _update(results: RabiLengthResults, platform: Platform, target: QubitId):
+def _update(results: RabiLengthVoltResults, platform: Platform, target: QubitId):
     update.drive_duration(results.length[target], platform, target)
 
 
-def _plot(data: RabiLengthData, fit: RabiLengthResults, target: QubitId):
+def _plot(data: RabiLengthVoltData, fit: RabiLengthVoltResults, target: QubitId):
     """Plotting function for RabiLength experiment."""
-    return utils.plot_probabilities(data, target, fit)
+    return utils.plot(data, target, fit)
 
 
-rabi_length = Routine(_acquisition, _fit, _plot, _update)
+rabi_length_signal = Routine(_acquisition, _fit, _plot, _update)
 """RabiLength Routine object."""
```

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/rabi/length_sequences.py` & `qibocal-0.0.9/src/qibocal/protocols/rabi/length_sequences.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/rabi/length_signal.py` & `qibocal-0.0.9/src/qibocal/protocols/readout_optimization/resonator_amplitude.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,206 +1,213 @@
 from dataclasses import dataclass, field
-from typing import Optional
+from os import error
 
 import numpy as np
 import numpy.typing as npt
-from qibolab import AcquisitionType, AveragingMode, ExecutionParameters
+import plotly.graph_objects as go
+from plotly.subplots import make_subplots
+from qibolab import AcquisitionType, ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
-from qibolab.sweeper import Parameter, Sweeper, SweeperType
-from scipy.optimize import curve_fit
-from scipy.signal import find_peaks
 
 from qibocal import update
 from qibocal.auto.operation import Data, Parameters, Results, Routine
-from qibocal.config import log
-
-from . import utils
+from qibocal.fitting.classifier.qubit_fit import QubitFit
+from qibocal.protocols.utils import table_dict, table_html
 
 
 @dataclass
-class RabiLengthVoltParameters(Parameters):
-    """RabiLengthVolt runcard inputs."""
+class ResonatorAmplitudeParameters(Parameters):
+    """ResonatorAmplitude runcard inputs."""
 
-    pulse_duration_start: float
-    """Initial pi pulse duration [ns]."""
-    pulse_duration_end: float
-    """Final pi pulse duration [ns]."""
-    pulse_duration_step: float
-    """Step pi pulse duration [ns]."""
-    pulse_amplitude: Optional[float] = None
-    """Pi pulse amplitude. Same for all qubits."""
+    amplitude_step: float
+    """Amplituude step to be probed."""
+    amplitude_start: float = 0.0
+    """Amplitude start."""
+    amplitude_stop: float = 1.0
+    """Amplitude stop value"""
+    error_threshold: float = 0.003
+    """Probability error threshold to stop the best amplitude search"""
+
+
+ResonatorAmplitudeType = np.dtype(
+    [
+        ("error", np.float64),
+        ("amp", np.float64),
+        ("angle", np.float64),
+        ("threshold", np.float64),
+    ]
+)
+"""Custom dtype for Optimization RO amplitude."""
 
 
 @dataclass
-class RabiLengthVoltResults(Results):
-    """RabiLengthVolt outputs."""
-
-    length: dict[QubitId, tuple[int, Optional[float]]]
-    """Pi pulse duration for each qubit."""
-    amplitude: dict[QubitId, tuple[float, Optional[float]]]
-    """Pi pulse amplitude. Same for all qubits."""
-    fitted_parameters: dict[QubitId, dict[str, float]]
-    """Raw fitting output."""
+class ResonatorAmplitudeData(Data):
+    """Data class for `resoantor_amplitude` protocol."""
 
-
-RabiLenVoltType = np.dtype(
-    [("length", np.float64), ("signal", np.float64), ("phase", np.float64)]
-)
-"""Custom dtype for rabi amplitude."""
+    data: dict[tuple, npt.NDArray[ResonatorAmplitudeType]] = field(default_factory=dict)
 
 
 @dataclass
-class RabiLengthVoltData(Data):
-    """RabiLength acquisition outputs."""
+class ResonatorAmplitudeResults(Results):
+    """Result class for `resonator_amplitude` protocol."""
 
-    amplitudes: dict[QubitId, float] = field(default_factory=dict)
-    """Pulse durations provided by the user."""
-    data: dict[QubitId, npt.NDArray[RabiLenVoltType]] = field(default_factory=dict)
-    """Raw data acquired."""
+    lowest_errors: dict[QubitId, list]
+    """Lowest probability errors"""
+    best_amp: dict[QubitId, list]
+    """Amplitude with lowest error"""
+    best_angle: dict[QubitId, float]
+    """IQ angle that gives lower error."""
+    best_threshold: dict[QubitId, float]
+    """Thershold that gives lower error."""
 
 
 def _acquisition(
-    params: RabiLengthVoltParameters, platform: Platform, targets: list[QubitId]
-) -> RabiLengthVoltData:
+    params: ResonatorAmplitudeParameters,
+    platform: Platform,
+    targets: list[QubitId],
+) -> ResonatorAmplitudeData:
     r"""
-    Data acquisition for RabiLength Experiment.
-    In the Rabi experiment we apply a pulse at the frequency of the qubit and scan the drive pulse length
-    to find the drive pulse length that creates a rotation of a desired angle.
+    Data acquisition for resoantor amplitude optmization.
+    This protocol sweeps the readout amplitude performing a classification routine
+    and evaluating the error probability at each step. The sweep will be interrupted
+    if the probability error is less than the `error_threshold`.
+
+    Args:
+        params (:class:`ResonatorAmplitudeParameters`): input parameters
+        platform (:class:`Platform`): Qibolab's platform
+        targets (list): list of QubitIds to be characterized
+
+    Returns:
+        data (:class:`ResonatorAmplitudeData`)
     """
 
-    # create a sequence of pulses for the experiment
-    sequence = PulseSequence()
-    qd_pulses = {}
-    ro_pulses = {}
-    amplitudes = {}
+    data = ResonatorAmplitudeData()
     for qubit in targets:
-        # TODO: made duration optional for qd pulse?
-        qd_pulses[qubit] = platform.create_qubit_drive_pulse(
-            qubit, start=0, duration=params.pulse_duration_start
-        )
-        if params.pulse_amplitude is not None:
-            qd_pulses[qubit].amplitude = params.pulse_amplitude
-        amplitudes[qubit] = qd_pulses[qubit].amplitude
-
-        ro_pulses[qubit] = platform.create_qubit_readout_pulse(
-            qubit, start=qd_pulses[qubit].finish
-        )
-        sequence.add(qd_pulses[qubit])
-        sequence.add(ro_pulses[qubit])
+        error = 1
+        old_amp = platform.qubits[qubit].native_gates.MZ.amplitude
+        new_amp = params.amplitude_start
+        while error > params.error_threshold and new_amp <= params.amplitude_stop:
+            platform.qubits[qubit].native_gates.MZ.amplitude = new_amp
+            sequence_0 = PulseSequence()
+            sequence_1 = PulseSequence()
+
+            qd_pulses = platform.create_RX_pulse(qubit, start=0)
+            ro_pulses = platform.create_qubit_readout_pulse(
+                qubit, start=qd_pulses.finish
+            )
+            sequence_0.add(ro_pulses)
+            sequence_1.add(qd_pulses)
+            sequence_1.add(ro_pulses)
+
+            state0_results = platform.execute_pulse_sequence(
+                sequence_0,
+                ExecutionParameters(
+                    nshots=params.nshots,
+                    relaxation_time=params.relaxation_time,
+                    acquisition_type=AcquisitionType.INTEGRATION,
+                ),
+            )
 
-    # define the parameter to sweep and its range:
-    # qubit drive pulse duration time
-    qd_pulse_duration_range = np.arange(
-        params.pulse_duration_start,
-        params.pulse_duration_end,
-        params.pulse_duration_step,
-    )
+            state1_results = platform.execute_pulse_sequence(
+                sequence_1,
+                ExecutionParameters(
+                    nshots=params.nshots,
+                    relaxation_time=params.relaxation_time,
+                    acquisition_type=AcquisitionType.INTEGRATION,
+                ),
+            )
+            result0 = state0_results[ro_pulses.serial]
+            result1 = state1_results[ro_pulses.serial]
 
-    sweeper = Sweeper(
-        Parameter.duration,
-        qd_pulse_duration_range,
-        [qd_pulses[qubit] for qubit in targets],
-        type=SweeperType.ABSOLUTE,
-    )
+            i_values = np.concatenate((result0.voltage_i, result1.voltage_i))
+            q_values = np.concatenate((result0.voltage_q, result1.voltage_q))
+            iq_values = np.stack((i_values, q_values), axis=-1)
+            nshots = int(len(i_values) / 2)
+            states = [0] * nshots + [1] * nshots
+            model = QubitFit()
+            model.fit(iq_values, np.array(states))
+            error = model.probability_error
+            data.register_qubit(
+                ResonatorAmplitudeType,
+                (qubit),
+                dict(
+                    amp=np.array([new_amp]),
+                    error=np.array([error]),
+                    angle=np.array([model.angle]),
+                    threshold=np.array([model.threshold]),
+                ),
+            )
+            platform.qubits[qubit].native_gates.MZ.amplitude = old_amp
+            new_amp += params.amplitude_step
+    return data
 
-    data = RabiLengthVoltData(amplitudes=amplitudes)
 
-    # execute the sweep
-    results = platform.sweep(
-        sequence,
-        ExecutionParameters(
-            nshots=params.nshots,
-            relaxation_time=params.relaxation_time,
-            acquisition_type=AcquisitionType.INTEGRATION,
-            averaging_mode=AveragingMode.CYCLIC,
-        ),
-        sweeper,
+def _fit(data: ResonatorAmplitudeData) -> ResonatorAmplitudeResults:
+    qubits = data.qubits
+    best_amps = {}
+    best_angle = {}
+    best_threshold = {}
+    lowest_err = {}
+    for qubit in qubits:
+        data_qubit = data[qubit]
+        index_best_err = np.argmin(data_qubit["error"])
+        lowest_err[qubit] = data_qubit["error"][index_best_err]
+        best_amps[qubit] = data_qubit["amp"][index_best_err]
+        best_angle[qubit] = data_qubit["angle"][index_best_err]
+        best_threshold[qubit] = data_qubit["threshold"][index_best_err]
+
+    return ResonatorAmplitudeResults(lowest_err, best_amps, best_angle, best_threshold)
+
+
+def _plot(
+    data: ResonatorAmplitudeData, fit: ResonatorAmplitudeResults, target: QubitId
+):
+    """Plotting function for Optimization RO amplitude."""
+    figures = []
+    opacity = 1
+    fitting_report = None
+    fig = make_subplots(
+        rows=1,
+        cols=1,
     )
-
-    for qubit in targets:
-        result = results[ro_pulses[qubit].serial]
-        data.register_qubit(
-            RabiLenVoltType,
-            (qubit),
-            dict(
-                length=qd_pulse_duration_range,
-                signal=result.magnitude,
-                phase=result.phase,
+    if fit is not None:
+        fig.add_trace(
+            go.Scatter(
+                x=data[target]["amp"],
+                y=data[target]["error"],
+                opacity=opacity,
+                showlegend=True,
+                mode="lines+markers",
             ),
+            row=1,
+            col=1,
         )
-    return data
-
-
-def _fit(data: RabiLengthVoltData) -> RabiLengthVoltResults:
-    """Post-processing for RabiLength experiment."""
 
-    qubits = data.qubits
-    fitted_parameters = {}
-    durations = {}
-
-    for qubit in qubits:
-        qubit_data = data[qubit]
-        rabi_parameter = qubit_data.length
-        voltages = qubit_data.signal
-
-        y_min = np.min(voltages)
-        y_max = np.max(voltages)
-        x_min = np.min(rabi_parameter)
-        x_max = np.max(rabi_parameter)
-        x = (rabi_parameter - x_min) / (x_max - x_min)
-        y = (voltages - y_min) / (y_max - y_min) - 1 / 2
-
-        # Guessing period using fourier transform
-        ft = np.fft.rfft(y)
-        mags = abs(ft)
-        local_maxima = find_peaks(mags, threshold=1)[0]
-        index = local_maxima[0] if len(local_maxima) > 0 else None
-        # 0.5 hardcoded guess for less than one oscillation
-        f = x[index] / (x[1] - x[0]) if index is not None else 0.5
-
-        pguess = [0, np.sign(y[0]) * 0.5, 1 / f, 0, 0]
-        try:
-            popt, _ = curve_fit(
-                utils.rabi_length_function,
-                x,
-                y,
-                p0=pguess,
-                maxfev=100000,
-                bounds=(
-                    [0, -1, 0, -np.pi, 0],
-                    [1, 1, np.inf, np.pi, np.inf],
-                ),
+        fitting_report = table_html(
+            table_dict(
+                target,
+                "Best Readout Amplitude [a.u.]",
+                np.round(fit.best_amp[target], 4),
             )
-            translated_popt = [  # change it according to the fit function
-                (y_max - y_min) * (popt[0] + 1 / 2) + y_min,
-                (y_max - y_min) * popt[1] * np.exp(x_min * popt[4] / (x_max - x_min)),
-                popt[2] * (x_max - x_min),
-                popt[3] - 2 * np.pi * x_min / popt[2] / (x_max - x_min),
-                popt[4] / (x_max - x_min),
-            ]
-            pi_pulse_parameter = (
-                translated_popt[2]
-                / 2
-                * utils.period_correction_factor(phase=translated_popt[3])
-            )
-            durations[qubit] = pi_pulse_parameter
-            fitted_parameters[qubit] = translated_popt
-
-        except Exception as e:
-            log.warning(f"Rabi fit failed for qubit {qubit} due to {e}.")
+        )
 
-    return RabiLengthVoltResults(durations, data.amplitudes, fitted_parameters)
+    fig.update_layout(
+        showlegend=True,
+        xaxis_title="Readout Amplitude [a.u.]",
+        yaxis_title="Probability Error",
+    )
 
+    figures.append(fig)
 
-def _update(results: RabiLengthVoltResults, platform: Platform, target: QubitId):
-    update.drive_duration(results.length[target], platform, target)
+    return figures, fitting_report
 
 
-def _plot(data: RabiLengthVoltData, fit: RabiLengthVoltResults, target: QubitId):
-    """Plotting function for RabiLength experiment."""
-    return utils.plot(data, target, fit)
+def _update(results: ResonatorAmplitudeResults, platform: Platform, target: QubitId):
+    update.readout_amplitude(results.best_amp[target], platform, target)
+    update.iq_angle(results.best_angle[target], platform, target)
+    update.threshold(results.best_threshold[target], platform, target)
 
 
-rabi_length_signal = Routine(_acquisition, _fit, _plot, _update)
-"""RabiLength Routine object."""
+resonator_amplitude = Routine(_acquisition, _fit, _plot, _update)
+"""Resonator Amplitude Routine  object."""
```

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/rabi/utils.py` & `qibocal-0.0.9/src/qibocal/protocols/rabi/utils.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/ramsey/ramsey.py` & `qibocal-0.0.9/src/qibocal/protocols/ramsey/ramsey.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/ramsey/ramsey_signal.py` & `qibocal-0.0.9/src/qibocal/protocols/ramsey/ramsey_signal.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/ramsey/utils.py` & `qibocal-0.0.9/src/qibocal/protocols/ramsey/utils.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/randomized_benchmarking/circuit_tools.py` & `qibocal-0.0.9/src/qibocal/protocols/randomized_benchmarking/circuit_tools.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     qubits_str = [str(qubit)]
 
     for _ in range(depth):
         # Generate a layer.
         new_layer, random_index = rb_gen.layer_gen()
         # Ensure new_layer is a circuit
         if isinstance(new_layer, Gate):
-            new_circuit = Circuit(1, wire_names=qubits_str)
+            new_circuit = Circuit(1)
             new_circuit.add(new_layer)
             random_indexes.append(random_index)
 
         # We are only using this for the RB we have right now
         elif all(isinstance(gate, Gate) for gate in new_layer):
             new_circuit = Circuit(1, wire_names=qubits_str)
             new_circuit.add(new_layer)
@@ -44,15 +44,15 @@
             new_circuit = new_layer
         else:
             raise_error(
                 TypeError,
                 f"layer_gen must return type Circuit or Gate, but it is type {type(new_layer)}.",
             )
         if full_circuit is None:  # instantiate in first loop
-            full_circuit = Circuit(new_circuit.nqubits, wire_names=qubits_str)
+            full_circuit = Circuit(new_circuit.nqubits)
         full_circuit = full_circuit + new_circuit
     return full_circuit, random_indexes
 
 
 def add_inverse_layer(circuit: Circuit, single_qubit=True):
     """Adds an inverse gate/inverse gates at the end of a circuit (in place).
```

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/randomized_benchmarking/fitting.py` & `qibocal-0.0.9/src/qibocal/protocols/randomized_benchmarking/fitting.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/randomized_benchmarking/noisemodels.py` & `qibocal-0.0.9/src/qibocal/protocols/randomized_benchmarking/noisemodels.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/randomized_benchmarking/standard_rb.py` & `qibocal-0.0.9/src/qibocal/protocols/randomized_benchmarking/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,124 +1,159 @@
 from collections import defaultdict
 from dataclasses import dataclass, field
-from typing import Iterable, Optional, TypedDict, Union
+from numbers import Number
+from typing import Iterable, Optional, Union
 
 import numpy as np
 import numpy.typing as npt
-import plotly.graph_objects as go
+from qibo import gates
 from qibo.backends import GlobalBackend
-from qibolab.platform import Platform
 from qibolab.qubits import QubitId
 
-from qibocal.auto.operation import Data, Parameters, Results, Routine
+from qibocal.auto.operation import Data, Parameters
+from qibocal.auto.transpile import (
+    dummy_transpiler,
+    execute_transpiled_circuit,
+    execute_transpiled_circuits,
+)
 from qibocal.config import raise_error
-from qibocal.protocols.characterization.randomized_benchmarking import noisemodels
+from qibocal.protocols.randomized_benchmarking import noisemodels
+from qibocal.protocols.utils import significant_digit
 
-from ..utils import table_dict, table_html
 from .circuit_tools import add_inverse_layer, add_measurement_layer, layer_circuit
-from .fitting import exp1B_func, fit_exp1B_func
-from .utils import data_uncertainties, number_to_str, random_clifford
 
-NPULSES_PER_CLIFFORD = 1.875
+SINGLE_QUBIT_CLIFFORDS = {
+    # Virtual gates
+    0: gates.I,
+    1: lambda q: gates.U3(q, 0, np.pi / 2, np.pi / 2),  # Z,
+    2: lambda q: gates.U3(q, 0, np.pi / 2, 0),  # gates.RZ(q, np.pi / 2),
+    3: lambda q: gates.U3(q, 0, -np.pi / 2, 0),  # gates.RZ(q, -np.pi / 2),
+    # pi rotations
+    4: lambda q: gates.U3(q, np.pi, 0, np.pi),  # X,
+    5: lambda q: gates.U3(q, np.pi, 0, 0),  # Y,
+    # pi/2 rotations
+    6: lambda q: gates.U3(q, np.pi / 2, -np.pi / 2, np.pi / 2),
+    7: lambda q: gates.U3(q, -np.pi / 2, -np.pi / 2, np.pi / 2),
+    8: lambda q: gates.U3(q, np.pi / 2, 0, 0),
+    9: lambda q: gates.U3(q, -np.pi / 2, 0, 0),
+    # 2pi/3 rotations
+    10: lambda q: gates.U3(q, np.pi / 2, -np.pi / 2, 0),  # Rx(pi/2)Ry(pi/2)
+    11: lambda q: gates.U3(q, np.pi / 2, -np.pi / 2, np.pi),  # Rx(pi/2)Ry(-pi/2)
+    12: lambda q: gates.U3(q, np.pi / 2, np.pi / 2, 0),  # Rx(-pi/2)Ry(pi/2)
+    13: lambda q: gates.U3(q, np.pi / 2, np.pi / 2, -np.pi),  # Rx(-pi/2)Ry(-pi/2)
+    14: lambda q: gates.U3(q, np.pi / 2, 0, np.pi / 2),  # Ry(pi/2)Rx(pi/2)
+    15: lambda q: gates.U3(q, np.pi / 2, 0, -np.pi / 2),  # Ry(pi/2)Rx(-pi/2)
+    16: lambda q: gates.U3(q, np.pi / 2, -np.pi, np.pi / 2),  # Ry(-pi/2)Rx(pi/2)
+    17: lambda q: gates.U3(q, np.pi / 2, np.pi, -np.pi / 2),  # Ry(-pi/2)Rx(-pi/2)
+    # Hadamard-like
+    18: lambda q: gates.U3(q, np.pi / 2, -np.pi, 0),  # X Ry(pi/2)
+    19: lambda q: gates.U3(q, np.pi / 2, 0, np.pi),  # X Ry(-pi/2)
+    20: lambda q: gates.U3(q, np.pi / 2, np.pi / 2, np.pi / 2),  # Y Rx(pi/2)
+    21: lambda q: gates.U3(q, np.pi / 2, -np.pi / 2, -np.pi / 2),  # Y Rx(pi/2)
+    22: lambda q: gates.U3(q, np.pi, -np.pi / 4, np.pi / 4),  # Rx(pi/2)Ry(pi/2)Rx(pi/2)
+    23: lambda q: gates.U3(
+        q, np.pi, np.pi / 4, -np.pi / 4
+    ),  # Rx(-pi/2)Ry(pi/2)Rx(-pi/2)
+}
 
 
-class Depthsdict(TypedDict):
-    """dictionary used to build a list of depths as ``range(start, stop, step)``."""
+def random_clifford(random_index_gen):
+    """Generates random Clifford operator.
 
-    start: int
-    stop: int
-    step: int
+    Args:
+        qubits (int or list or ndarray): if ``int``, the number of qubits for the Clifford.
+            If ``list`` or ``ndarray``, indexes of the qubits for the Clifford to act on.
+        seed (int or ``numpy.random.Generator``, optional): Either a generator of
+            random numbers or a fixed seed to initialize a generator. If ``None``,
+            initializes a generator with a random seed. Default is ``None``.
 
+    Returns:
+        (list of :class:`qibo.gates.Gate`): Random Clifford operator(s).
+    """
 
-@dataclass
-class StandardRBParameters(Parameters):
-    """Standard Randomized Benchmarking runcard inputs."""
+    random_index = int(random_index_gen(SINGLE_QUBIT_CLIFFORDS))
+    clifford_gate = SINGLE_QUBIT_CLIFFORDS[random_index](0)
 
-    depths: Union[list, Depthsdict]
-    """A list of depths/sequence lengths. If a dictionary is given the list will be build."""
-    niter: int
-    """Sets how many iterations over the same depth value."""
-    uncertainties: Optional[float] = None
-    """Method of computing the error bars of the signal and uncertainties of the fit. If ``None``,
-    it computes the standard deviation. Otherwise it computes the corresponding confidence interval. Defaults `None`."""
-    unrolling: bool = False
-    """If ``True`` it uses sequence unrolling to deploy multiple circuits in a single instrument call.
-    Defaults to ``False``."""
-    seed: Optional[int] = None
-    """A fixed seed to initialize ``np.random.Generator``. If ``None``, uses a random seed.
-    Defaults is ``None``."""
-    noise_model: Optional[str] = None
-    """For simulation purposes, string has to match what is in
-    :mod:`qibocal.protocols.characterization.randomized_benchmarking.noisemodels`"""
-    noise_params: Optional[list] = field(default_factory=list)
-    """With this the noise model will be initialized, if not given random values will be used."""
-    nshots: int = 10
-    """Just to add the default value"""
-
-    def __post_init__(self):
-        if isinstance(self.depths, dict):
-            self.depths = list(
-                range(self.depths["start"], self.depths["stop"], self.depths["step"])
-            )
+    return clifford_gate, random_index
 
 
-RBType = np.dtype(
-    [
-        ("samples", np.int32),
-    ]
-)
-"""Custom dtype for RB."""
+def number_to_str(
+    value: Number,
+    uncertainty: Optional[Union[Number, list, tuple, np.ndarray]] = None,
+    precision: Optional[int] = None,
+):
+    """Converts a number into a string.
 
+    Args:
+        value (Number): the number to display
+        uncertainty (Number or list or tuple or np.ndarray, optional): number or 2-element
+            interval with the low and high uncertainties of ``value``. Defaults to ``None``.
+        precision (int, optional): nonnegative number of floating points of the displayed value.
+            If ``None``, defaults to the second significant digit of ``uncertainty``
+            or ``3`` if ``uncertainty`` is ``None``. Defaults to ``None``.
 
-@dataclass
-class RBData(Data):
-    """The output of the acquisition function."""
+    Returns:
+        str: The number expressed as a string, with the uncertainty if given.
+    """
 
-    depths: list
-    """Circuits depths."""
-    uncertainties: Optional[float]
-    """Parameters uncertainties."""
-    seed: Optional[int]
-    nshots: int
-    """Number of shots."""
-    niter: int
-    """Number of iterations for each depth."""
-    data: dict[QubitId, npt.NDArray[RBType]] = field(default_factory=dict)
-    """Raw data acquired."""
-    circuits: dict[QubitId, list[list[int]]] = field(default_factory=dict)
-    """Clifford gate indexes executed."""
+    # If uncertainty is not given, return the value with precision
+    if uncertainty is None:
+        precision = precision if precision is not None else 3
+        return f"{value:.{precision}f}"
 
-    def extract_probabilities(self, qubit):
-        """Extract the probabilities given `qubit`"""
-        probs = []
-        for depth in self.depths:
-            data_list = np.array(self.data[qubit, depth].tolist())
-            data_list = data_list.reshape((-1, self.nshots))
-            probs.append(np.count_nonzero(1 - data_list, axis=1) / data_list.shape[1])
-        return probs
+    if isinstance(uncertainty, Number):
+        if precision is None:
+            precision = (significant_digit(uncertainty) + 1) or 3
+        return f"{value:.{precision}f} \u00B1 {uncertainty:.{precision}f}"
 
+    # If any uncertainty is None, return the value with precision
+    if any(u is None for u in uncertainty):
+        return f"{value:.{precision if precision is not None else 3}f}"
 
-@dataclass
-class StandardRBResult(Results):
-    """Standard RB outputs."""
+    # If precision is None, get the first significant digit of the uncertainty
+    if precision is None:
+        precision = max(significant_digit(u) + 1 for u in uncertainty) or 3
+
+    # Check if both uncertainties are equal up to precision
+    if np.round(uncertainty[0], precision) == np.round(uncertainty[1], precision):
+        return f"{value:.{precision}f} \u00B1 {uncertainty[0]:.{precision}f}"
+
+    return f"{value:.{precision}f} +{uncertainty[1]:.{precision}f} / -{uncertainty[0]:.{precision}f}"
+
+
+def data_uncertainties(data, method=None, data_median=None, homogeneous=True):
+    """Compute the uncertainties of the median (or specified) values.
+
+    Args:
+        data (list or np.ndarray): 2d array with rows containing data points
+            from which the median value is extracted.
+        method (float, optional): method of computing the method.
+            If it is `None`, computes the standard deviation, otherwise it
+            computes the corresponding confidence interval using ``np.percentile``.
+            Defaults to ``None``.
+        data_median (list or np.ndarray, optional): 1d array for computing the errors from the
+            confidence interval. If ``None``, the median values are computed from ``data``.
+        homogeneous (bool): if ``True``, assumes that all rows in ``data`` are of the same size
+            and returns ``np.ndarray``. Default is ``True``.
+
+    Returns:
+        np.ndarray: uncertainties of the data.
+    """
+    if method is None:
+        return np.std(data, axis=1) if homogeneous else [np.std(row) for row in data]
+
+    percentiles = [
+        (100 - method) / 2,
+        (100 + method) / 2,
+    ]
+    percentile_interval = np.percentile(data, percentiles, axis=1)
 
-    fidelity: dict[QubitId, float]
-    """The overall fidelity of this qubit."""
-    pulse_fidelity: dict[QubitId, float]
-    """The pulse fidelity of the gates acting on this qubit."""
-    fit_parameters: dict[QubitId, tuple[float, float, float]]
-    """Raw fitting parameters."""
-    fit_uncertainties: dict[QubitId, tuple[float, float, float]]
-    """Fitting parameters uncertainties."""
-    error_bars: dict[QubitId, Optional[Union[float, list[float]]]] = None
-    """Error bars for y."""
-
-    # FIXME: fix this after https://github.com/qiboteam/qibocal/pull/597
-    def __contains__(self, qubit: QubitId):
-        return True
+    uncertainties = np.abs(np.vstack([data_median, data_median]) - percentile_interval)
+
+    return uncertainties
 
 
 class RB_Generator:
     """
     This class generates random single qubit cliffords for randomized benchmarking.
     """
 
@@ -152,63 +187,98 @@
 
 def random_circuits(
     depth: int,
     targets: list[QubitId],
     niter,
     rb_gen,
     noise_model=None,
+    inverse_layer=True,
 ) -> Iterable:
     """Returns single-qubit random self-inverting Clifford circuits.
 
     Args:
         params (StandardRBParameters): Parameters of the RB protocol.
         targets (list[QubitId]):
             list of qubits the circuit is executed on.
         nqubits (int, optional): Number of qubits of the resulting circuits.
             If ``None``, sets ``len(qubits)``. Defaults to ``None``.
+        inverse_layer (bool): If `True` a layer inverting the circuit is added.
+            Default to `True`.
 
     Returns:
         Iterable: The iterator of circuits.
     """
 
     circuits = []
     indexes = defaultdict(list)
     for _ in range(niter):
         for target in targets:
             circuit, random_index = layer_circuit(rb_gen, depth, target)
-            add_inverse_layer(circuit)
+            if inverse_layer:
+                add_inverse_layer(circuit)
             add_measurement_layer(circuit)
             if noise_model is not None:
                 circuit = noise_model.apply(circuit)
             circuits.append(circuit)
             indexes[target].append(random_index)
 
     return circuits, indexes
 
 
-def _acquisition(
-    params: StandardRBParameters,
-    platform: Platform,
-    targets: list[QubitId],
-) -> RBData:
-    """The data acquisition stage of Standard Randomized Benchmarking.
+RBType = np.dtype(
+    [
+        ("samples", np.int32),
+    ]
+)
+"""Custom dtype for RB."""
 
-    1. Set up the scan
-    2. Execute the scan
-    3. Post process the data and initialize a standard rb data object with it.
+
+@dataclass
+class RBData(Data):
+    """The output of the acquisition function."""
+
+    depths: list
+    """Circuits depths."""
+    uncertainties: Optional[float]
+    """Parameters uncertainties."""
+    seed: Optional[int]
+    nshots: int
+    """Number of shots."""
+    niter: int
+    """Number of iterations for each depth."""
+    data: dict[QubitId, npt.NDArray[RBType]] = field(default_factory=dict)
+    """Raw data acquired."""
+    circuits: dict[QubitId, list[list[int]]] = field(default_factory=dict)
+    """Clifford gate indexes executed."""
+
+    def extract_probabilities(self, qubit):
+        """Extract the probabilities given `qubit`"""
+        probs = []
+        for depth in self.depths:
+            data_list = np.array(self.data[qubit, depth].tolist())
+            data_list = data_list.reshape((-1, self.nshots))
+            probs.append(np.count_nonzero(1 - data_list, axis=1) / data_list.shape[1])
+        return probs
+
+
+def rb_acquisition(
+    params: Parameters,
+    targets: list[QubitId],
+    add_inverse_layer: bool = True,
+) -> Data:
+    """RB data acquisition function.
 
     Args:
-        params (StandardRBParameters): All parameters in one object.
-        platform (Platform): Platform the experiment is executed on.
-        qubits (dict[int, Union[str, int]] or list[Union[str, int]]): list of qubits the experiment is executed on.
+        params (FilteredRBParameters): All parameters in one object.
+        targets (dict[int, Union[str, int]] or list[Union[str, int]]): list of qubits the experiment is executed on.
 
     Returns:
         RBData: The depths, samples and ground state probability of each experiment in the scan.
-    """
 
+    """
     backend = GlobalBackend()
     # For simulations, a noise model can be added.
     noise_model = None
     if params.noise_model is not None:
         if backend.name == "qibolab":
             raise_error(
                 ValueError,
@@ -231,26 +301,45 @@
     indexes = {}
     samples = []
     qubits_ids = targets
     rb_gen = RB_Generator(params.seed)
     for depth in params.depths:
         # TODO: This does not generate multi qubit circuits
         circuits_depth, random_indexes = random_circuits(
-            depth, qubits_ids, params.niter, rb_gen, noise_model
+            depth,
+            qubits_ids,
+            params.niter,
+            rb_gen,
+            noise_model,
+            add_inverse_layer,
         )
         circuits.extend(circuits_depth)
         for qubit in random_indexes.keys():
             indexes[(qubit, depth)] = random_indexes[qubit]
     # Execute the circuits
+    transpiler = dummy_transpiler(backend)
+    qubit_maps = [[i] for i in targets] * (len(params.depths) * params.niter)
     if params.unrolling:
-        executed_circuits = backend.execute_circuits(circuits, nshots=params.nshots)
+        _, executed_circuits = execute_transpiled_circuits(
+            circuits,
+            qubit_maps=qubit_maps,
+            backend=backend,
+            nshots=params.nshots,
+            transpiler=transpiler,
+        )
     else:
         executed_circuits = [
-            backend.execute_circuit(circuit, nshots=params.nshots)
-            for circuit in circuits
+            execute_transpiled_circuit(
+                circuit,
+                qubit_map=qubit_map,
+                backend=backend,
+                nshots=params.nshots,
+                transpiler=transpiler,
+            )[1]
+            for circuit, qubit_map in zip(circuits, qubit_maps)
         ]
 
     for circ in executed_circuits:
         samples.extend(circ.samples())
     samples = np.reshape(samples, (-1, nqubits, params.nshots))
 
     for i, depth in enumerate(params.depths):
@@ -262,177 +351,7 @@
                 dict(
                     samples=samples[index[0] : index[1]][:, nqubit],
                 ),
             )
     data.circuits = indexes
 
     return data
-
-
-def _fit(data: RBData) -> StandardRBResult:
-    """Takes a data frame, extracts the depths and the signal and fits it with an
-    exponential function y = Ap^x+B.
-
-    Args:
-        data (RBData): Data from the data acquisition stage.
-
-    Returns:
-        StandardRBResult: Aggregated and processed data.
-    """
-    qubits = data.qubits
-
-    fidelity, pulse_fidelity = {}, {}
-    popts, perrs = {}, {}
-    error_barss = {}
-    for qubit in qubits:
-        # Extract depths and probabilities
-        x = data.depths
-        probs = data.extract_probabilities(qubit)
-        samples_mean = np.mean(probs, axis=1)
-        # TODO: Should we use the median or the mean?
-        median = np.median(probs, axis=1)
-
-        error_bars = data_uncertainties(
-            probs,
-            method=data.uncertainties,
-            data_median=median,
-        )
-
-        sigma = (
-            np.max(error_bars, axis=0) if data.uncertainties is not None else error_bars
-        )
-
-        popt, perr = fit_exp1B_func(x, samples_mean, sigma=sigma, bounds=[0, 1])
-        # Compute the fidelities
-        infidelity = (1 - popt[1]) / 2
-        fidelity[qubit] = 1 - infidelity
-        pulse_fidelity[qubit] = 1 - infidelity / NPULSES_PER_CLIFFORD
-
-        # conversion from np.array to list/tuple
-        error_bars = error_bars.tolist()
-        error_barss[qubit] = error_bars
-        perrs[qubit] = perr
-        popts[qubit] = popt
-
-    return StandardRBResult(fidelity, pulse_fidelity, popts, perrs, error_barss)
-
-
-def _plot(
-    data: RBData, fit: StandardRBResult, target: QubitId
-) -> tuple[list[go.Figure], str]:
-    """Builds the table for the qq pipe, calls the plot function of the result object
-    and returns the figure es list.
-
-    Args:
-        data (RBData): Data object used for the table.
-        fit (StandardRBResult): Is called for the plot.
-        target (_type_): Not used yet.
-
-    Returns:
-        tuple[list[go.Figure], str]:
-    """
-
-    qubit = target
-    fig = go.Figure()
-    fitting_report = ""
-    x = data.depths
-    raw_data = data.extract_probabilities(qubit)
-    y = np.mean(raw_data, axis=1)
-    raw_depths = [[depth] * data.niter for depth in data.depths]
-
-    fig.add_trace(
-        go.Scatter(
-            x=np.hstack(raw_depths),
-            y=np.hstack(raw_data),
-            line=dict(color="#6597aa"),
-            mode="markers",
-            marker={"opacity": 0.2, "symbol": "square"},
-            name="iterations",
-        )
-    )
-
-    fig.add_trace(
-        go.Scatter(
-            x=x,
-            y=y,
-            line=dict(color="#aa6464"),
-            mode="markers",
-            name="average",
-        )
-    )
-    # Create a dictionary for the error bars
-    error_y_dict = None
-    if fit is not None:
-        popt, perr = fit.fit_parameters[qubit], fit.fit_uncertainties[qubit]
-        label = "Fit: y=Ap^x<br>A: {}<br>p: {}<br>B: {}".format(
-            number_to_str(popt[0], perr[0]),
-            number_to_str(popt[1], perr[1]),
-            number_to_str(popt[2], perr[2]),
-        )
-        x_fit = np.linspace(min(x), max(x), len(x) * 20)
-        y_fit = exp1B_func(x_fit, *popt)
-        fig.add_trace(
-            go.Scatter(
-                x=x_fit,
-                y=y_fit,
-                name=label,
-                line=go.scatter.Line(dash="dot", color="#00cc96"),
-            )
-        )
-        if fit.error_bars is not None:
-            error_bars = fit.error_bars[qubit]
-            # Constant error bars
-            if isinstance(error_bars, Iterable) is False:
-                error_y_dict = {"type": "constant", "value": error_bars}
-            # Symmetric error bars
-            elif isinstance(error_bars[0], Iterable) is False:
-                error_y_dict = {"type": "data", "array": error_bars}
-            # Asymmetric error bars
-            else:
-                error_y_dict = {
-                    "type": "data",
-                    "symmetric": False,
-                    "array": error_bars[1],
-                    "arrayminus": error_bars[0],
-                }
-            fig.add_trace(
-                go.Scatter(
-                    x=x,
-                    y=y,
-                    error_y=error_y_dict,
-                    line={"color": "#aa6464"},
-                    mode="markers",
-                    name="error bars",
-                )
-            )
-    if fit is not None:
-        fitting_report = table_html(
-            table_dict(
-                qubit,
-                ["niter", "nshots", "uncertainties", "fidelity", "pulse_fidelity"],
-                [
-                    data.niter,
-                    data.nshots,
-                    data.uncertainties,
-                    number_to_str(
-                        fit.fidelity[qubit],
-                        np.array(fit.fit_uncertainties[qubit][1]) / 2,
-                    ),
-                    number_to_str(
-                        fit.pulse_fidelity[qubit],
-                        np.array(fit.fit_uncertainties[qubit][1])
-                        / (2 * NPULSES_PER_CLIFFORD),
-                    ),
-                ],
-            )
-        )
-
-    fig.update_layout(
-        showlegend=True,
-        xaxis_title="Circuit depth",
-        yaxis_title="Survival Probability",
-    )
-
-    return [fig], fitting_report
-
-
-standard_rb = Routine(_acquisition, _fit, _plot)
```

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/readout_characterization.py` & `qibocal-0.0.9/src/qibocal/protocols/readout_characterization.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,53 @@
 from dataclasses import dataclass, field
 
 import numpy as np
 import numpy.typing as npt
 import plotly.graph_objects as go
+from plotly.subplots import make_subplots
 from qibolab import AcquisitionType, ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
 
 from qibocal import update
 from qibocal.auto.operation import Data, Parameters, Results, Routine
-from qibocal.protocols.characterization.utils import (
+from qibocal.protocols.utils import (
     effective_qubit_temperature,
     format_error_single_cell,
     round_report,
     table_dict,
     table_html,
 )
 
 
 @dataclass
 class ReadoutCharacterizationParameters(Parameters):
     """ReadoutCharacterization runcard inputs."""
 
+    delay: float = 0
+    """Delay between readouts, could account for resonator deplation or not [ns]."""
+
 
 @dataclass
 class ReadoutCharacterizationResults(Results):
     """ReadoutCharacterization outputs."""
 
     fidelity: dict[QubitId, float]
     "Fidelity of the measurement"
     assignment_fidelity: dict[QubitId, float]
     """Assignment fidelity."""
     qnd: dict[QubitId, float]
     "QND-ness of the measurement"
     effective_temperature: dict[QubitId, tuple[float, float]]
     """Effective qubit temperature."""
     Lambda_M: dict[QubitId, float]
-    "Mapping between a given initial state to an outcome adter the measurement"
+    "Mapping between a given initial state to an outcome after the measurement"
+    Lambda_M2: dict[QubitId, float]
+    "Mapping between the outcome after the measurement and it still being that outcame after another measurement"
 
 
 ReadoutCharacterizationType = np.dtype(
     [
         ("i", np.float64),
         ("q", np.float64),
     ]
@@ -51,14 +57,17 @@
 
 @dataclass
 class ReadoutCharacterizationData(Data):
     """ReadoutCharacterization acquisition outputs."""
 
     qubit_frequencies: dict[QubitId, float] = field(default_factory=dict)
     """Qubit frequencies."""
+
+    delay: float = 0
+    """Delay between readouts [ns]."""
     data: dict[tuple, npt.NDArray[ReadoutCharacterizationType]] = field(
         default_factory=dict
     )
     """Raw data acquired."""
     samples: dict[tuple, npt.NDArray] = field(default_factory=dict)
     """Raw data acquired."""
 
@@ -69,15 +78,16 @@
     targets: list[QubitId],
 ) -> ReadoutCharacterizationData:
     """Data acquisition for resonator spectroscopy."""
 
     data = ReadoutCharacterizationData(
         qubit_frequencies={
             qubit: platform.qubits[qubit].drive_frequency for qubit in targets
-        }
+        },
+        delay=float(params.delay),
     )
 
     # FIXME: ADD 1st measurament and post_selection for accurate state preparation ?
 
     for state in [0, 1]:
         # Define the pulse sequences
         if state == 1:
@@ -89,15 +99,17 @@
             if state == 1:
                 RX_pulses[qubit] = platform.create_RX_pulse(qubit, start=0)
                 sequence.add(RX_pulses[qubit])
                 start = RX_pulses[qubit].finish
             ro_pulses[qubit] = []
             for _ in range(2):
                 ro_pulse = platform.create_qubit_readout_pulse(qubit, start=start)
-                start += ro_pulse.duration
+                start += ro_pulse.duration + int(
+                    params.delay
+                )  # device required conversion
                 sequence.add(ro_pulse)
                 ro_pulses[qubit].append(ro_pulse)
 
         # execute the pulse sequence
         results = platform.execute_pulse_sequence(
             sequence,
             ExecutionParameters(
@@ -134,14 +146,15 @@
 
     qubits = data.qubits
     assignment_fidelity = {}
     fidelity = {}
     effective_temperature = {}
     qnd = {}
     Lambda_M = {}
+    Lambda_M2 = {}
     for qubit in qubits:
         # 1st measurement (m=1)
         m1_state_1 = data.samples[qubit, 1, 0]
         nshots = len(m1_state_1)
         # state 1
         state1_count_1_m1 = np.count_nonzero(m1_state_1)
         state0_count_1_m1 = nshots - state1_count_1_m1
@@ -164,14 +177,20 @@
 
         # Repeat Lambda and fidelity for each measurement ?
         Lambda_M[qubit] = [
             [state0_count_0_m1 / nshots, state0_count_1_m1 / nshots],
             [state1_count_0_m1 / nshots, state1_count_1_m1 / nshots],
         ]
 
+        # Repeat Lambda and fidelity for each measurement ?
+        Lambda_M2[qubit] = [
+            [state0_count_0_m2 / nshots, state0_count_1_m2 / nshots],
+            [state1_count_0_m2 / nshots, state1_count_1_m2 / nshots],
+        ]
+
         assignment_fidelity[qubit] = (
             1 - (state1_count_0_m1 / nshots + state0_count_1_m1 / nshots) / 2
         )
 
         fidelity[qubit] = 2 * assignment_fidelity[qubit] - 1
 
         # QND FIXME: Careful revision
@@ -188,15 +207,15 @@
             prob_1=state0_count_1_m1 / nshots,
             prob_0=state0_count_0_m1 / nshots,
             qubit_frequency=data.qubit_frequencies[qubit],
             nshots=nshots,
         )
 
     return ReadoutCharacterizationResults(
-        fidelity, assignment_fidelity, qnd, effective_temperature, Lambda_M
+        fidelity, assignment_fidelity, qnd, effective_temperature, Lambda_M, Lambda_M2
     )
 
 
 def _plot(
     data: ReadoutCharacterizationData,
     fit: ReadoutCharacterizationResults,
     target: QubitId,
@@ -212,50 +231,96 @@
         for measure in range(2):
             shots = data.data[target, state, measure]
 
             fig.add_trace(
                 go.Scatter(
                     x=shots.i,
                     y=shots.q,
-                    name=f"state {state} measure {measure}",
+                    name=f"Prepared state {state} measurement {measure}",
                     mode="markers",
                     showlegend=True,
                     opacity=0.7,
                     marker=dict(size=3),
                 )
             )
+    fig.update_layout(
+        title={
+            "text": "IQ Plane",
+            "y": 0.9,
+            "x": 0.5,
+            "xanchor": "center",
+            "yanchor": "top",
+        },
+        xaxis_title="I",
+        yaxis_title="Q",
+    )
+
     figures.append(fig)
     if fit is not None:
-        fig2 = go.Figure()
 
-        fig2.add_trace(
+        fig = make_subplots(
+            rows=1,
+            cols=2,
+            subplot_titles=(
+                "1st measurement statistics",
+                "2nd measurement statistics",
+            ),
+        )
+
+        fig.add_trace(
             go.Heatmap(
                 z=fit.Lambda_M[target],
-            )
+                x=["0", "1"],
+                y=["0", "1"],
+                coloraxis="coloraxis",
+            ),
+            row=1,
+            col=1,
+        )
+
+        fig.add_trace(
+            go.Heatmap(
+                z=fit.Lambda_M2[target],
+                x=["0", "1"],
+                y=["0", "1"],
+                coloraxis="coloraxis",
+            ),
+            row=1,
+            col=2,
         )
+
+        fig.update_xaxes(title_text="Measured state", row=1, col=1)
+        fig.update_xaxes(title_text="Measured state", row=1, col=2)
+        fig.update_yaxes(title_text="Prepared state", row=1, col=1)
+        fig.update_yaxes(title_text="Prepared state", row=1, col=2)
+
+        figures.append(fig)
+
         fitting_report = table_html(
             table_dict(
                 target,
                 [
+                    "Delay between readouts [ns]",
                     "Assignment Fidelity",
                     "Fidelity",
                     "QND",
                     "Effective Qubit Temperature [K]",
                 ],
                 [
+                    np.round(data.delay),
                     np.round(fit.assignment_fidelity[target], 6),
                     np.round(fit.fidelity[target], 6),
                     np.round(fit.qnd[target], 6),
                     format_error_single_cell(
                         round_report([fit.effective_temperature[target]])
                     ),
                 ],
             )
         )
-        figures.append(fig2)
+
     return figures, fitting_report
 
 
 def _update(
     results: ReadoutCharacterizationResults, platform: Platform, target: QubitId
 ):
     update.readout_fidelity(results.fidelity[target], platform, target)
```

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/readout_mitigation_matrix.py` & `qibocal-0.0.9/src/qibocal/protocols/readout_mitigation_matrix.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from dataclasses import dataclass, field
 from typing import Optional
 
 import numpy as np
 import numpy.typing as npt
 import plotly.express as px
 from qibo import gates
+from qibo.backends import GlobalBackend
 from qibo.models import Circuit
 from qibolab import ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
 
 from qibocal.auto.operation import Data, Parameters, Results, Routine
+from qibocal.auto.transpile import dummy_transpiler, execute_transpiled_circuit
 from qibocal.config import log
 
 from .utils import calculate_frequencies
 
 
 @dataclass
 class ReadoutMitigationMatrixParameters(Parameters):
@@ -91,14 +93,17 @@
     params: ReadoutMitigationMatrixParameters,
     platform: Platform,
     targets: list[list[QubitId]],
 ) -> ReadoutMitigationMatrixData:
     data = ReadoutMitigationMatrixData(
         nshots=params.nshots, qubit_list=[list(qq) for qq in targets]
     )
+    backend = GlobalBackend()
+    transpiler = dummy_transpiler(backend)
+    qubit_map = [i for i in range(platform.nqubits)]
     for qubits in targets:
         nqubits = len(qubits)
         for i in range(2**nqubits):
             state = format(i, f"0{nqubits}b")
             if params.pulses:
                 sequence = PulseSequence()
                 for q, bit in enumerate(state):
@@ -117,21 +122,25 @@
                 results = platform.execute_pulse_sequence(
                     sequence, ExecutionParameters(nshots=params.nshots)
                 )
                 data.add(
                     tuple(qubits), state, calculate_frequencies(results, tuple(qubits))
                 )
             else:
-                c = Circuit(platform.nqubits)
+                c = Circuit(
+                    platform.nqubits,
+                    wire_names=[str(i) for i in range(platform.nqubits)],
+                )
                 for q, bit in enumerate(state):
                     if bit == "1":
                         c.add(gates.X(qubits[q]))
                     c.add(gates.M(qubits[q]))
-                results = c(nshots=params.nshots)
-
+                _, results = execute_transpiled_circuit(
+                    c, qubit_map, backend, nshots=params.nshots, transpiler=transpiler
+                )
                 data.add(tuple(qubits), state, dict(results.frequencies()))
     return data
 
 
 def _fit(data: ReadoutMitigationMatrixData) -> ReadoutMitigationMatrixResults:
     """Post processing for readout mitigation matrix protocol."""
     readout_mitigation_matrix = {}
```

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/readout_optimization/resonator_amplitude.py` & `qibocal-0.0.9/src/qibocal/protocols/readout_optimization/resonator_frequency.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,213 +1,236 @@
 from dataclasses import dataclass, field
-from os import error
 
 import numpy as np
 import numpy.typing as npt
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
 from qibolab import AcquisitionType, ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
+from qibolab.sweeper import Parameter, Sweeper, SweeperType
 
 from qibocal import update
 from qibocal.auto.operation import Data, Parameters, Results, Routine
 from qibocal.fitting.classifier.qubit_fit import QubitFit
-from qibocal.protocols.characterization.utils import table_dict, table_html
+from qibocal.protocols.utils import HZ_TO_GHZ, table_dict, table_html
 
 
 @dataclass
-class ResonatorAmplitudeParameters(Parameters):
-    """ResonatorAmplitude runcard inputs."""
+class ResonatorFrequencyParameters(Parameters):
+    """Optimization RO frequency inputs."""
 
-    amplitude_step: float
-    """Amplituude step to be probed."""
-    amplitude_start: float = 0.0
-    """Amplitude start."""
-    amplitude_stop: float = 1.0
-    """Amplitude stop value"""
-    error_threshold: float = 0.003
-    """Probability error threshold to stop the best amplitude search"""
+    freq_width: int
+    """Width [Hz] for frequency sweep relative to the readout frequency [Hz]."""
+    freq_step: int
+    """Frequency step for sweep [Hz]."""
 
 
-ResonatorAmplitudeType = np.dtype(
+@dataclass
+class ResonatorFrequencyResults(Results):
+    """Optimization Resonator frequency outputs."""
+
+    fidelities: dict[QubitId, list]
+    """Assignment fidelities."""
+    best_freq: dict[QubitId, float]
+    """Resonator Frequency with the highest assignment fidelity."""
+    best_angle: dict[QubitId, float]
+    """IQ angle that maximes assignment fidelity"""
+    best_threshold: dict[QubitId, float]
+    """Threshold that maximes assignment fidelity"""
+
+
+ResonatorFrequencyType = np.dtype(
     [
-        ("error", np.float64),
-        ("amp", np.float64),
+        ("freq", np.float64),
+        ("assignment_fidelity", np.float64),
         ("angle", np.float64),
         ("threshold", np.float64),
     ]
 )
-"""Custom dtype for Optimization RO amplitude."""
+"""Custom dtype for Optimization RO frequency."""
 
 
 @dataclass
-class ResonatorAmplitudeData(Data):
-    """Data class for `resoantor_amplitude` protocol."""
-
-    data: dict[tuple, npt.NDArray[ResonatorAmplitudeType]] = field(default_factory=dict)
-
+class ResonatorFrequencyData(Data):
+    """ "Optimization RO frequency acquisition outputs."""
 
-@dataclass
-class ResonatorAmplitudeResults(Results):
-    """Result class for `resonator_amplitude` protocol."""
+    resonator_type: str
+    """Resonator type."""
+    data: dict[QubitId, npt.NDArray[ResonatorFrequencyType]] = field(
+        default_factory=dict
+    )
 
-    lowest_errors: dict[QubitId, list]
-    """Lowest probability errors"""
-    best_amp: dict[QubitId, list]
-    """Amplitude with lowest error"""
-    best_angle: dict[QubitId, float]
-    """IQ angle that gives lower error."""
-    best_threshold: dict[QubitId, float]
-    """Thershold that gives lower error."""
+    def unique_freqs(self, qubit: QubitId) -> np.ndarray:
+        return np.unique(self.data[qubit]["freq"])
 
 
 def _acquisition(
-    params: ResonatorAmplitudeParameters,
-    platform: Platform,
-    targets: list[QubitId],
-) -> ResonatorAmplitudeData:
+    params: ResonatorFrequencyParameters, platform: Platform, targets: list[QubitId]
+) -> ResonatorFrequencyData:
     r"""
-    Data acquisition for resoantor amplitude optmization.
-    This protocol sweeps the readout amplitude performing a classification routine
-    and evaluating the error probability at each step. The sweep will be interrupted
-    if the probability error is less than the `error_threshold`.
+    Data acquisition for readout frequency optimization.
+    While sweeping the readout frequency, the routine performs a single shot
+    classification and evaluates the assignement fidelity.
+    At the end, the readout frequency is updated, choosing the one that has
+    the highest assignment fidelity.
 
     Args:
-        params (:class:`ResonatorAmplitudeParameters`): input parameters
-        platform (:class:`Platform`): Qibolab's platform
-        targets (list): list of QubitIds to be characterized
+        params (ResonatorFrequencyParameters): experiment's parameters
+        platform (Platform): Qibolab platform object
+        qubits (list): list of target qubits to perform the action
 
-    Returns:
-        data (:class:`ResonatorAmplitudeData`)
     """
 
-    data = ResonatorAmplitudeData()
+    # create 2 sequences of pulses for the experiment:
+    # sequence_0: I  - MZ
+    # sequence_1: RX - MZ
+
+    # taking advantage of multiplexing, apply the same set of gates to all qubits in parallel
+    sequence_0 = PulseSequence()
+    sequence_1 = PulseSequence()
+    ro_pulses = {}
+    qd_pulses = {}
     for qubit in targets:
-        error = 1
-        old_amp = platform.qubits[qubit].native_gates.MZ.amplitude
-        new_amp = params.amplitude_start
-        while error > params.error_threshold and new_amp <= params.amplitude_stop:
-            platform.qubits[qubit].native_gates.MZ.amplitude = new_amp
-            sequence_0 = PulseSequence()
-            sequence_1 = PulseSequence()
-
-            qd_pulses = platform.create_RX_pulse(qubit, start=0)
-            ro_pulses = platform.create_qubit_readout_pulse(
-                qubit, start=qd_pulses.finish
-            )
-            sequence_0.add(ro_pulses)
-            sequence_1.add(qd_pulses)
-            sequence_1.add(ro_pulses)
-
-            state0_results = platform.execute_pulse_sequence(
-                sequence_0,
-                ExecutionParameters(
-                    nshots=params.nshots,
-                    relaxation_time=params.relaxation_time,
-                    acquisition_type=AcquisitionType.INTEGRATION,
-                ),
-            )
+        qd_pulses[qubit] = platform.create_RX_pulse(qubit, start=0)
+        ro_pulses[qubit] = platform.create_qubit_readout_pulse(
+            qubit, start=qd_pulses[qubit].finish
+        )
+        sequence_0.add(ro_pulses[qubit])
+        sequence_1.add(qd_pulses[qubit])
+        sequence_1.add(ro_pulses[qubit])
+
+    # define the parameter to sweep and its range:
+    delta_frequency_range = np.arange(
+        -params.freq_width / 2, params.freq_width / 2, params.freq_step
+    )
 
-            state1_results = platform.execute_pulse_sequence(
-                sequence_1,
-                ExecutionParameters(
-                    nshots=params.nshots,
-                    relaxation_time=params.relaxation_time,
-                    acquisition_type=AcquisitionType.INTEGRATION,
-                ),
-            )
-            result0 = state0_results[ro_pulses.serial]
-            result1 = state1_results[ro_pulses.serial]
+    data = ResonatorFrequencyData(resonator_type=platform.resonator_type)
+    sweeper = Sweeper(
+        Parameter.frequency,
+        delta_frequency_range,
+        pulses=[ro_pulses[qubit] for qubit in targets],
+        type=SweeperType.OFFSET,
+    )
+
+    results_0 = platform.sweep(
+        sequence_0,
+        ExecutionParameters(
+            nshots=params.nshots,
+            relaxation_time=params.relaxation_time,
+            acquisition_type=AcquisitionType.INTEGRATION,
+        ),
+        sweeper,
+    )
+
+    results_1 = platform.sweep(
+        sequence_1,
+        ExecutionParameters(
+            nshots=params.nshots,
+            relaxation_time=params.relaxation_time,
+            acquisition_type=AcquisitionType.INTEGRATION,
+        ),
+        sweeper,
+    )
+
+    # retrieve the results for every qubit
+    for qubit in targets:
+        for k, freq in enumerate(delta_frequency_range):
+            i_values = []
+            q_values = []
+            states = []
+            for i, results in enumerate([results_0, results_1]):
+                result = results[ro_pulses[qubit].serial]
+                i_values.extend(result.voltage_i[k])
+                q_values.extend(result.voltage_q[k])
+                states.extend([i] * len(result.voltage_i[k]))
 
-            i_values = np.concatenate((result0.voltage_i, result1.voltage_i))
-            q_values = np.concatenate((result0.voltage_q, result1.voltage_q))
-            iq_values = np.stack((i_values, q_values), axis=-1)
-            nshots = int(len(i_values) / 2)
-            states = [0] * nshots + [1] * nshots
             model = QubitFit()
-            model.fit(iq_values, np.array(states))
-            error = model.probability_error
+            model.fit(np.stack((i_values, q_values), axis=-1), np.array(states))
             data.register_qubit(
-                ResonatorAmplitudeType,
+                ResonatorFrequencyType,
                 (qubit),
                 dict(
-                    amp=np.array([new_amp]),
-                    error=np.array([error]),
+                    freq=np.array([(ro_pulses[qubit].frequency + freq) * HZ_TO_GHZ]),
+                    assignment_fidelity=np.array([model.assignment_fidelity]),
                     angle=np.array([model.angle]),
                     threshold=np.array([model.threshold]),
                 ),
             )
-            platform.qubits[qubit].native_gates.MZ.amplitude = old_amp
-            new_amp += params.amplitude_step
     return data
 
 
-def _fit(data: ResonatorAmplitudeData) -> ResonatorAmplitudeResults:
+def _fit(data: ResonatorFrequencyData) -> ResonatorFrequencyResults:
+    """Post-Processing for Optimization RO frequency"""
     qubits = data.qubits
-    best_amps = {}
+    best_freq = {}
     best_angle = {}
     best_threshold = {}
-    lowest_err = {}
+    highest_fidelity = {}
     for qubit in qubits:
         data_qubit = data[qubit]
-        index_best_err = np.argmin(data_qubit["error"])
-        lowest_err[qubit] = data_qubit["error"][index_best_err]
-        best_amps[qubit] = data_qubit["amp"][index_best_err]
-        best_angle[qubit] = data_qubit["angle"][index_best_err]
-        best_threshold[qubit] = data_qubit["threshold"][index_best_err]
-
-    return ResonatorAmplitudeResults(lowest_err, best_amps, best_angle, best_threshold)
+        index_best_fid = np.argmax(data_qubit["assignment_fidelity"])
+        highest_fidelity[qubit] = data_qubit["assignment_fidelity"][index_best_fid]
+        best_freq[qubit] = data_qubit["freq"][index_best_fid]
+        best_angle[qubit] = data_qubit["angle"][index_best_fid]
+        best_threshold[qubit] = data_qubit["threshold"][index_best_fid]
+
+    return ResonatorFrequencyResults(
+        fidelities=highest_fidelity,
+        best_freq=best_freq,
+        best_angle=best_angle,
+        best_threshold=best_threshold,
+    )
 
 
 def _plot(
-    data: ResonatorAmplitudeData, fit: ResonatorAmplitudeResults, target: QubitId
+    data: ResonatorFrequencyData, fit: ResonatorFrequencyResults, target: QubitId
 ):
-    """Plotting function for Optimization RO amplitude."""
+    """Plotting function for Optimization RO frequency."""
     figures = []
+    freqs = data[target]["freq"]
     opacity = 1
-    fitting_report = None
+    fitting_report = ""
     fig = make_subplots(
         rows=1,
         cols=1,
     )
     if fit is not None:
         fig.add_trace(
             go.Scatter(
-                x=data[target]["amp"],
-                y=data[target]["error"],
+                x=freqs,
+                y=data[target]["assignment_fidelity"],
                 opacity=opacity,
                 showlegend=True,
-                mode="lines+markers",
             ),
             row=1,
             col=1,
         )
 
         fitting_report = table_html(
             table_dict(
                 target,
-                "Best Readout Amplitude [a.u.]",
-                np.round(fit.best_amp[target], 4),
+                "Best Resonator Frequency [Hz]",
+                np.round(fit.best_freq[target], 4),
             )
         )
 
     fig.update_layout(
         showlegend=True,
-        xaxis_title="Readout Amplitude [a.u.]",
-        yaxis_title="Probability Error",
+        xaxis_title="Resonator Frequencies [GHz]",
+        yaxis_title="Assignment Fidelities",
     )
 
     figures.append(fig)
 
     return figures, fitting_report
 
 
-def _update(results: ResonatorAmplitudeResults, platform: Platform, target: QubitId):
-    update.readout_amplitude(results.best_amp[target], platform, target)
-    update.iq_angle(results.best_angle[target], platform, target)
+def _update(results: ResonatorFrequencyResults, platform: Platform, target: QubitId):
+    update.readout_frequency(results.best_freq[target], platform, target)
     update.threshold(results.best_threshold[target], platform, target)
+    update.iq_angle(results.best_angle[target], platform, target)
 
 
-resonator_amplitude = Routine(_acquisition, _fit, _plot, _update)
-"""Resonator Amplitude Routine  object."""
+resonator_frequency = Routine(_acquisition, _fit, _plot, _update)
+""""Optimization RO frequency Routine object."""
```

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/readout_optimization/resonator_frequency.py` & `qibocal-0.0.9/src/qibocal/protocols/flux_dependence/resonator_flux_dependence.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,236 +1,279 @@
 from dataclasses import dataclass, field
+from typing import Optional
 
 import numpy as np
 import numpy.typing as npt
-import plotly.graph_objects as go
-from plotly.subplots import make_subplots
-from qibolab import AcquisitionType, ExecutionParameters
+from qibolab import AcquisitionType, AveragingMode, ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
 from qibolab.sweeper import Parameter, Sweeper, SweeperType
+from scipy.optimize import curve_fit
 
 from qibocal import update
 from qibocal.auto.operation import Data, Parameters, Results, Routine
-from qibocal.fitting.classifier.qubit_fit import QubitFit
-from qibocal.protocols.characterization.utils import HZ_TO_GHZ, table_dict, table_html
+from qibocal.config import log
+
+from ..utils import GHZ_TO_HZ, HZ_TO_GHZ, extract_feature, table_dict, table_html
+from . import utils
 
 
 @dataclass
-class ResonatorFrequencyParameters(Parameters):
-    """Optimization RO frequency inputs."""
+class ResonatorFluxParameters(Parameters):
+    """ResonatorFlux runcard inputs."""
 
     freq_width: int
-    """Width [Hz] for frequency sweep relative to the readout frequency [Hz]."""
+    """Width for frequency sweep relative to the readout frequency [Hz]."""
     freq_step: int
     """Frequency step for sweep [Hz]."""
+    bias_width: Optional[float] = None
+    """Width for bias sweep [V]."""
+    bias_step: Optional[float] = None
+    """Bias step for sweep [a.u.]."""
 
 
 @dataclass
-class ResonatorFrequencyResults(Results):
-    """Optimization Resonator frequency outputs."""
+class ResonatorFluxResults(Results):
+    """ResonatoFlux outputs."""
 
-    fidelities: dict[QubitId, list]
-    """Assignment fidelities."""
-    best_freq: dict[QubitId, float]
-    """Resonator Frequency with the highest assignment fidelity."""
-    best_angle: dict[QubitId, float]
-    """IQ angle that maximes assignment fidelity"""
-    best_threshold: dict[QubitId, float]
-    """Threshold that maximes assignment fidelity"""
+    frequency: dict[QubitId, float] = field(default_factory=dict)
+    """Readout frequency for each qubit."""
+    sweetspot: dict[QubitId, float] = field(default_factory=dict)
+    """Sweetspot for each qubit."""
+    asymmetry: dict[QubitId, float] = field(default_factory=dict)
+    """Asymmetry between junctions."""
+    bare_frequency: dict[QubitId, float] = field(default_factory=dict)
+    """Resonator bare frequency."""
+    drive_frequency: dict[QubitId, float] = field(default_factory=dict)
+    """Qubit frequency at sweetspot."""
+    fitted_parameters: dict[QubitId, dict[str, float]] = field(default_factory=dict)
+    """Raw fitting output."""
+    coupling: dict[QubitId, float] = field(default_factory=dict)
+    """Qubit-resonator coupling."""
+    matrix_element: dict[QubitId, float] = field(default_factory=dict)
+    """C_ii coefficient."""
 
 
-ResonatorFrequencyType = np.dtype(
+ResFluxType = np.dtype(
     [
         ("freq", np.float64),
-        ("assignment_fidelity", np.float64),
-        ("angle", np.float64),
-        ("threshold", np.float64),
+        ("bias", np.float64),
+        ("signal", np.float64),
+        ("phase", np.float64),
     ]
 )
-"""Custom dtype for Optimization RO frequency."""
+"""Custom dtype for resonator flux dependence."""
 
 
 @dataclass
-class ResonatorFrequencyData(Data):
-    """ "Optimization RO frequency acquisition outputs."""
+class ResonatorFluxData(Data):
+    """ResonatorFlux acquisition outputs."""
 
     resonator_type: str
     """Resonator type."""
-    data: dict[QubitId, npt.NDArray[ResonatorFrequencyType]] = field(
-        default_factory=dict
-    )
-
-    def unique_freqs(self, qubit: QubitId) -> np.ndarray:
-        return np.unique(self.data[qubit]["freq"])
+    qubit_frequency: dict[QubitId, float] = field(default_factory=dict)
+    """Qubit frequencies."""
+    offset: dict[QubitId, float] = field(default_factory=dict)
+    """Qubit bias offset."""
+    bare_resonator_frequency: dict[QubitId, int] = field(default_factory=dict)
+    """Qubit bare resonator frequency power provided by the user."""
+
+    data: dict[QubitId, npt.NDArray[ResFluxType]] = field(default_factory=dict)
+    """Raw data acquired."""
+
+    def register_qubit(self, qubit, freq, bias, signal, phase):
+        """Store output for single qubit."""
+        self.data[qubit] = utils.create_data_array(
+            freq, bias, signal, phase, dtype=ResFluxType
+        )
 
 
 def _acquisition(
-    params: ResonatorFrequencyParameters, platform: Platform, targets: list[QubitId]
-) -> ResonatorFrequencyData:
-    r"""
-    Data acquisition for readout frequency optimization.
-    While sweeping the readout frequency, the routine performs a single shot
-    classification and evaluates the assignement fidelity.
-    At the end, the readout frequency is updated, choosing the one that has
-    the highest assignment fidelity.
-
-    Args:
-        params (ResonatorFrequencyParameters): experiment's parameters
-        platform (Platform): Qibolab platform object
-        qubits (list): list of target qubits to perform the action
-
-    """
-
-    # create 2 sequences of pulses for the experiment:
-    # sequence_0: I  - MZ
-    # sequence_1: RX - MZ
+    params: ResonatorFluxParameters, platform: Platform, targets: list[QubitId]
+) -> ResonatorFluxData:
+    """Data acquisition for ResonatorFlux experiment."""
+    # create a sequence of pulses for the experiment:
+    # MZ
 
     # taking advantage of multiplexing, apply the same set of gates to all qubits in parallel
-    sequence_0 = PulseSequence()
-    sequence_1 = PulseSequence()
+    sequence = PulseSequence()
     ro_pulses = {}
-    qd_pulses = {}
+    qubit_frequency = {}
+    bare_resonator_frequency = {}
+    offset = {}
     for qubit in targets:
-        qd_pulses[qubit] = platform.create_RX_pulse(qubit, start=0)
-        ro_pulses[qubit] = platform.create_qubit_readout_pulse(
-            qubit, start=qd_pulses[qubit].finish
-        )
-        sequence_0.add(ro_pulses[qubit])
-        sequence_1.add(qd_pulses[qubit])
-        sequence_1.add(ro_pulses[qubit])
+        qubit_frequency[qubit] = platform.qubits[qubit].drive_frequency
+        bare_resonator_frequency[qubit] = platform.qubits[
+            qubit
+        ].bare_resonator_frequency
+        offset[qubit] = platform.qubits[qubit].sweetspot
+        ro_pulses[qubit] = platform.create_qubit_readout_pulse(qubit, start=0)
+        sequence.add(ro_pulses[qubit])
 
-    # define the parameter to sweep and its range:
+    # define the parameters to sweep and their range:
     delta_frequency_range = np.arange(
         -params.freq_width / 2, params.freq_width / 2, params.freq_step
     )
-
-    data = ResonatorFrequencyData(resonator_type=platform.resonator_type)
-    sweeper = Sweeper(
+    freq_sweeper = Sweeper(
         Parameter.frequency,
         delta_frequency_range,
-        pulses=[ro_pulses[qubit] for qubit in targets],
+        [ro_pulses[qubit] for qubit in targets],
         type=SweeperType.OFFSET,
     )
 
-    results_0 = platform.sweep(
-        sequence_0,
-        ExecutionParameters(
-            nshots=params.nshots,
-            relaxation_time=params.relaxation_time,
-            acquisition_type=AcquisitionType.INTEGRATION,
-        ),
-        sweeper,
-    )
-
-    results_1 = platform.sweep(
-        sequence_1,
-        ExecutionParameters(
-            nshots=params.nshots,
-            relaxation_time=params.relaxation_time,
-            acquisition_type=AcquisitionType.INTEGRATION,
-        ),
-        sweeper,
+    delta_bias_range = np.arange(
+        -params.bias_width / 2, params.bias_width / 2, params.bias_step
     )
+    sweepers = [
+        Sweeper(
+            Parameter.bias,
+            delta_bias_range,
+            qubits=[platform.qubits[qubit] for qubit in targets],
+            type=SweeperType.OFFSET,
+        )
+    ]
 
-    # retrieve the results for every qubit
-    for qubit in targets:
-        for k, freq in enumerate(delta_frequency_range):
-            i_values = []
-            q_values = []
-            states = []
-            for i, results in enumerate([results_0, results_1]):
-                result = results[ro_pulses[qubit].serial]
-                i_values.extend(result.voltage_i[k])
-                q_values.extend(result.voltage_q[k])
-                states.extend([i] * len(result.voltage_i[k]))
+    data = ResonatorFluxData(
+        resonator_type=platform.resonator_type,
+        qubit_frequency=qubit_frequency,
+        offset=offset,
+        bare_resonator_frequency=bare_resonator_frequency,
+    )
 
-            model = QubitFit()
-            model.fit(np.stack((i_values, q_values), axis=-1), np.array(states))
+    options = ExecutionParameters(
+        nshots=params.nshots,
+        relaxation_time=params.relaxation_time,
+        acquisition_type=AcquisitionType.INTEGRATION,
+        averaging_mode=AveragingMode.CYCLIC,
+    )
+    for bias_sweeper in sweepers:
+        results = platform.sweep(sequence, options, bias_sweeper, freq_sweeper)
+        # retrieve the results for every qubit
+        for qubit in targets:
+            result = results[ro_pulses[qubit].serial]
+            sweetspot = platform.qubits[qubit].sweetspot
             data.register_qubit(
-                ResonatorFrequencyType,
-                (qubit),
-                dict(
-                    freq=np.array([(ro_pulses[qubit].frequency + freq) * HZ_TO_GHZ]),
-                    assignment_fidelity=np.array([model.assignment_fidelity]),
-                    angle=np.array([model.angle]),
-                    threshold=np.array([model.threshold]),
-                ),
+                qubit,
+                signal=result.magnitude,
+                phase=result.phase,
+                freq=delta_frequency_range + ro_pulses[qubit].frequency,
+                bias=delta_bias_range + sweetspot,
             )
     return data
 
 
-def _fit(data: ResonatorFrequencyData) -> ResonatorFrequencyResults:
-    """Post-Processing for Optimization RO frequency"""
+def _fit(data: ResonatorFluxData) -> ResonatorFluxResults:
+    """
+    Post-processing for QubitFlux Experiment. See arxiv:0703002
+    Fit frequency as a function of current for the flux qubit spectroscopy
+    data (QubitFluxData): data object with information on the feature response at each current point.
+    """
+
     qubits = data.qubits
-    best_freq = {}
-    best_angle = {}
-    best_threshold = {}
-    highest_fidelity = {}
+    frequency = {}
+    sweetspot = {}
+    asymmetry = {}
+    bare_frequency = {}
+    drive_frequency = {}
+    fitted_parameters = {}
+    matrix_element = {}
+    coupling = {}
+
     for qubit in qubits:
-        data_qubit = data[qubit]
-        index_best_fid = np.argmax(data_qubit["assignment_fidelity"])
-        highest_fidelity[qubit] = data_qubit["assignment_fidelity"][index_best_fid]
-        best_freq[qubit] = data_qubit["freq"][index_best_fid]
-        best_angle[qubit] = data_qubit["angle"][index_best_fid]
-        best_threshold[qubit] = data_qubit["threshold"][index_best_fid]
-
-    return ResonatorFrequencyResults(
-        fidelities=highest_fidelity,
-        best_freq=best_freq,
-        best_angle=best_angle,
-        best_threshold=best_threshold,
+        qubit_data = data[qubit]
+
+        biases = qubit_data.bias
+        frequencies = qubit_data.freq
+        signal = qubit_data.signal
+
+        frequencies, biases = extract_feature(frequencies, biases, signal, "min")
+
+        try:
+            popt = curve_fit(
+                utils.transmon_readout_frequency_diagonal,
+                biases,
+                frequencies * HZ_TO_GHZ,
+                bounds=utils.resonator_flux_dependence_fit_bounds(
+                    data.qubit_frequency[qubit],
+                    qubit_data.bias,
+                    data.bare_resonator_frequency[qubit],
+                ),
+                maxfev=100000,
+            )[0]
+            fitted_parameters[qubit] = popt.tolist()
+
+            # frequency corresponds to transmon readout frequency
+            # at the sweetspot popt[3]
+            frequency[qubit] = (
+                utils.transmon_readout_frequency_diagonal(popt[3], *popt) * GHZ_TO_HZ
+            )
+            sweetspot[qubit] = popt[3]
+            asymmetry[qubit] = popt[1]
+            bare_frequency[qubit] = popt[4] * GHZ_TO_HZ
+            drive_frequency[qubit] = popt[0] * GHZ_TO_HZ
+            coupling[qubit] = popt[5]
+            matrix_element[qubit] = popt[2]
+        except ValueError as e:
+            log.error(
+                f"Error in resonator_flux protocol fit: {e} "
+                "The threshold for the SNR mask is probably too high. "
+                "Lowering the value of `threshold` in `extract_*_feature`"
+                "should fix the problem."
+            )
+
+    return ResonatorFluxResults(
+        frequency=frequency,
+        sweetspot=sweetspot,
+        asymmetry=asymmetry,
+        bare_frequency=bare_frequency,
+        drive_frequency=drive_frequency,
+        coupling=coupling,
+        matrix_element=matrix_element,
+        fitted_parameters=fitted_parameters,
     )
 
 
-def _plot(
-    data: ResonatorFrequencyData, fit: ResonatorFrequencyResults, target: QubitId
-):
-    """Plotting function for Optimization RO frequency."""
-    figures = []
-    freqs = data[target]["freq"]
-    opacity = 1
-    fitting_report = ""
-    fig = make_subplots(
-        rows=1,
-        cols=1,
+def _plot(data: ResonatorFluxData, fit: ResonatorFluxResults, target: QubitId):
+    """Plotting function for ResonatorFlux Experiment."""
+    figures = utils.flux_dependence_plot(
+        data, fit, target, utils.transmon_readout_frequency_diagonal
     )
-    if fit is not None:
-        fig.add_trace(
-            go.Scatter(
-                x=freqs,
-                y=data[target]["assignment_fidelity"],
-                opacity=opacity,
-                showlegend=True,
-            ),
-            row=1,
-            col=1,
-        )
 
+    if fit is not None:
         fitting_report = table_html(
             table_dict(
                 target,
-                "Best Resonator Frequency [Hz]",
-                np.round(fit.best_freq[target], 4),
+                [
+                    f"Sweetspot [V]",
+                    "Bare Resonator Frequency [Hz]",
+                    "Readout Frequency [Hz]",
+                    "Qubit Frequency at Sweetspot [Hz]",
+                    "Asymmetry d",
+                    "Coupling g",
+                    "Flux dependence",
+                ],
+                [
+                    np.round(fit.sweetspot[target], 4),
+                    np.round(fit.bare_frequency[target], 4),
+                    np.round(fit.frequency[target], 4),
+                    np.round(fit.drive_frequency[target], 4),
+                    np.round(fit.asymmetry[target], 4),
+                    np.round(fit.coupling[target], 4),
+                    np.round(fit.matrix_element[target], 4),
+                ],
             )
         )
-
-    fig.update_layout(
-        showlegend=True,
-        xaxis_title="Resonator Frequencies [GHz]",
-        yaxis_title="Assignment Fidelities",
-    )
-
-    figures.append(fig)
-
-    return figures, fitting_report
+        return figures, fitting_report
+    return figures, ""
 
 
-def _update(results: ResonatorFrequencyResults, platform: Platform, target: QubitId):
-    update.readout_frequency(results.best_freq[target], platform, target)
-    update.threshold(results.best_threshold[target], platform, target)
-    update.iq_angle(results.best_angle[target], platform, target)
+def _update(results: ResonatorFluxResults, platform: Platform, qubit: QubitId):
+    update.bare_resonator_frequency(results.bare_frequency[qubit], platform, qubit)
+    update.readout_frequency(results.frequency[qubit], platform, qubit)
+    update.drive_frequency(results.drive_frequency[qubit], platform, qubit)
+    update.asymmetry(results.asymmetry[qubit], platform, qubit)
+    update.coupling(results.coupling[qubit], platform, qubit)
 
 
-resonator_frequency = Routine(_acquisition, _fit, _plot, _update)
-""""Optimization RO frequency Routine object."""
+resonator_flux = Routine(_acquisition, _fit, _plot, _update)
+"""ResonatorFlux Routine object."""
```

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/readout_optimization/twpa_calibration/frequency.py` & `qibocal-0.0.9/src/qibocal/protocols/readout_optimization/twpa_calibration/frequency_power.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,179 +4,224 @@
 import numpy.typing as npt
 import plotly.graph_objects as go
 from qibolab.platform import Platform
 from qibolab.qubits import QubitId
 
 from qibocal import update
 from qibocal.auto.operation import Data, Parameters, Results, Routine
-from qibocal.protocols.characterization import classification
-from qibocal.protocols.characterization.readout_optimization.resonator_frequency import (
-    ResonatorFrequencyType,
-)
-from qibocal.protocols.characterization.utils import HZ_TO_GHZ, table_dict, table_html
+from qibocal.protocols import classification
+from qibocal.protocols.utils import HZ_TO_GHZ, table_dict, table_html
 
 
 @dataclass
-class TwpaFrequencyParameters(Parameters):
-    """TwpaFrequency runcard inputs."""
+class TwpaFrequencyPowerParameters(Parameters):
+    """Twpa Frequency Power runcard inputs."""
 
     frequency_width: float
-    """Relative frequency width [Hz]"""
+    """Frequency total width."""
     frequency_step: float
-    """Frequency step [Hz]"""
+    """Frequency step to be probed."""
+    power_width: float
+    """Power total width."""
+    power_step: float
+    """Power step to be probed."""
+
+
+TwpaFrequencyPowerType = np.dtype(
+    [
+        ("freq", np.float64),
+        ("power", np.float64),
+        ("assignment_fidelity", np.float64),
+        ("angle", np.float64),
+        ("threshold", np.float64),
+    ]
+)
 
 
 @dataclass
-class TwpaFrequencyData(Data):
-    """TwpaFrequency acquisition outputs."""
+class TwpaFrequencyPowerData(Data):
+    """Twpa Frequency Power acquisition outputs."""
 
     data: dict[
-        tuple[QubitId, float], npt.NDArray[classification.ClassificationType]
+        tuple[QubitId, float, float], npt.NDArray[classification.ClassificationType]
     ] = field(default_factory=dict)
     """Raw data acquired."""
     frequencies: dict[QubitId, float] = field(default_factory=dict)
     """Frequencies for each qubit."""
+    powers: dict[QubitId, float] = field(default_factory=dict)
+    """Powers for each qubit."""
 
 
 @dataclass
-class TwpaFrequencyResults(Results):
-    """TwpaFrequency outputs."""
+class TwpaFrequencyPowerResults(Results):
+    """Twpa Frequency Power outputs."""
 
     best_freqs: dict[QubitId, float] = field(default_factory=dict)
+    best_powers: dict[QubitId, float] = field(default_factory=dict)
     best_fidelities: dict[QubitId, float] = field(default_factory=dict)
     best_angles: dict[QubitId, float] = field(default_factory=dict)
     best_thresholds: dict[QubitId, float] = field(default_factory=dict)
 
 
 def _acquisition(
-    params: TwpaFrequencyParameters,
+    params: TwpaFrequencyPowerParameters,
     platform: Platform,
     targets: list[QubitId],
-) -> TwpaFrequencyData:
+) -> TwpaFrequencyPowerData:
     r"""
-    Data acquisition for TWPA power optmization.
+    Data acquisition for TWPA frequency vs. power optmization.
     This protocol perform a classification protocol for twpa frequencies
     in the range [twpa_frequency - frequency_width / 2, twpa_frequency + frequency_width / 2]
-    with step frequency_step.
+    with step frequency_step and powers in the range [twpa_power - power_width / 2, twpa_power + power_width / 2]
 
     Args:
-        params (:class:`TwpaFrequencyParameters`): input parameters
+        params (:class:`TwpaFrequencyPowerParameters`): input parameters
         platform (:class:`Platform`): Qibolab's platform
-        qubits (dict): dict of target :class:`Qubit` objects to be characterized
+        targets (list): list of qubit to be characterized
 
     Returns:
-        data (:class:`TwpaFrequencyData`)
+        data (:class:`TwpaFrequencyPowerData`)
     """
 
-    data = TwpaFrequencyData()
+    data = TwpaFrequencyPowerData()
 
     freq_range = np.arange(
         -params.frequency_width / 2, params.frequency_width / 2, params.frequency_step
     ).astype(int)
+    power_range = np.arange(
+        -params.power_width / 2, params.power_width / 2, params.power_step
+    )
+    data = TwpaFrequencyPowerData()
 
     initial_twpa_freq = {}
+    initial_twpa_power = {}
     for qubit in targets:
-        initial_twpa_freq[qubit] = float(
-            platform.qubits[qubit].twpa.local_oscillator.frequency
-        )
-        data.frequencies[qubit] = list(
-            float(platform.qubits[qubit].twpa.local_oscillator.frequency) + freq_range
-        )
+        initial_twpa_freq[qubit] = platform.qubits[
+            qubit
+        ].twpa.local_oscillator.frequency
+        initial_twpa_power[qubit] = platform.qubits[qubit].twpa.local_oscillator.power
 
-    for freq in freq_range:
-        for qubit in targets:
+        for freq in freq_range:
             platform.qubits[qubit].twpa.local_oscillator.frequency = (
                 initial_twpa_freq[qubit] + freq
             )
 
-        classification_data = classification._acquisition(
-            classification.SingleShotClassificationParameters.load(
-                {"nshots": params.nshots}
-            ),
-            platform,
-            targets,
-        )
-        classification_result = classification._fit(classification_data)
-        for qubit in targets:
-            data.register_qubit(
-                ResonatorFrequencyType,
-                (qubit),
-                dict(
-                    freq=np.array(
-                        [platform.qubits[qubit].twpa.local_oscillator.frequency],
-                        dtype=np.float64,
+            for power in power_range:
+                for qubit in targets:
+                    platform.qubits[qubit].twpa.local_oscillator.power = (
+                        initial_twpa_power[qubit] + power
+                    )
+
+                classification_data = classification._acquisition(
+                    classification.SingleShotClassificationParameters.load(
+                        {"nshots": params.nshots}
                     ),
-                    assignment_fidelity=np.array(
-                        [classification_result.assignment_fidelity[qubit]],
+                    platform,
+                    targets,
+                )
+
+                classification_result = classification._fit(classification_data)
+
+                data.register_qubit(
+                    TwpaFrequencyPowerType,
+                    (qubit),
+                    dict(
+                        freq=np.array(
+                            [platform.qubits[qubit].twpa.local_oscillator.frequency],
+                            dtype=np.float64,
+                        ),
+                        power=np.array(
+                            [platform.qubits[qubit].twpa.local_oscillator.power],
+                            dtype=np.float64,
+                        ),
+                        assignment_fidelity=np.array(
+                            [classification_result.assignment_fidelity[qubit]],
+                        ),
+                        angle=np.array([classification_result.rotation_angle[qubit]]),
+                        threshold=np.array([classification_result.threshold[qubit]]),
                     ),
-                    angle=np.array([classification_result.rotation_angle[qubit]]),
-                    threshold=np.array([classification_result.threshold[qubit]]),
-                ),
-            )
+                )
     return data
 
 
-def _fit(data: TwpaFrequencyData) -> TwpaFrequencyResults:
+def _fit(data: TwpaFrequencyPowerData) -> TwpaFrequencyPowerResults:
     """Extract fidelity for each configuration qubit / param.
     Where param can be either frequency or power."""
 
-    qubits = data.qubits
     best_freq = {}
+    best_power = {}
     best_fidelity = {}
     best_angle = {}
     best_threshold = {}
+    qubits = data.qubits
+
     for qubit in qubits:
         data_qubit = data[qubit]
         index_best_err = np.argmax(data_qubit["assignment_fidelity"])
         best_fidelity[qubit] = data_qubit["assignment_fidelity"][index_best_err]
         best_freq[qubit] = data_qubit["freq"][index_best_err]
+        best_power[qubit] = data_qubit["power"][index_best_err]
         best_angle[qubit] = data_qubit["angle"][index_best_err]
         best_threshold[qubit] = data_qubit["threshold"][index_best_err]
 
-    return TwpaFrequencyResults(
-        best_freq, best_fidelity, best_thresholds=best_threshold, best_angles=best_angle
+    return TwpaFrequencyPowerResults(
+        best_freq,
+        best_power,
+        best_fidelity,
+        best_angles=best_angle,
+        best_thresholds=best_threshold,
     )
 
 
-def _plot(data: TwpaFrequencyData, fit: TwpaFrequencyResults, target: QubitId):
+def _plot(
+    data: TwpaFrequencyPowerData, fit: TwpaFrequencyPowerResults, target: QubitId
+):
     """Plotting function that shows the assignment fidelity
     for different values of the twpa frequency for a single qubit"""
 
     figures = []
     fitting_report = ""
     if fit is not None:
         qubit_data = data.data[target]
         fidelities = qubit_data["assignment_fidelity"]
         frequencies = qubit_data["freq"]
+        powers = qubit_data["power"]
         fitting_report = table_html(
             table_dict(
                 target,
-                ["Best assignment fidelity", "TWPA Frequency [Hz]"],
+                ["Best assignment fidelity", "TWPA Frequency [Hz]", "TWPA Power [dBm]"],
                 [
                     np.round(fit.best_fidelities[target], 3),
                     fit.best_freqs[target],
+                    np.round(fit.best_powers[target], 3),
                 ],
             )
         )
+
         fig = go.Figure(
-            [go.Scatter(x=frequencies * HZ_TO_GHZ, y=fidelities, name="Fidelity")]
+            [
+                go.Heatmap(
+                    x=frequencies * HZ_TO_GHZ, y=powers, z=fidelities, name="Fidelity"
+                )
+            ]
         )
 
         fig.update_layout(
             showlegend=True,
             xaxis_title="TWPA Frequency [GHz]",
-            yaxis_title="Assignment Fidelity",
+            yaxis_title="TWPA Power [dBm]",
         )
 
         figures.append(fig)
 
     return figures, fitting_report
 
 
-def _update(results: TwpaFrequencyResults, platform: Platform, target: QubitId):
+def _update(results: TwpaFrequencyPowerResults, platform: Platform, target: QubitId):
     update.twpa_frequency(results.best_freqs[target], platform, target)
+    update.twpa_power(results.best_powers[target], platform, target)
     update.iq_angle(results.best_angles[target], platform, target)
     update.threshold(results.best_thresholds[target], platform, target)
 
 
-twpa_frequency = Routine(_acquisition, _fit, _plot, _update)
+twpa_frequency_power = Routine(_acquisition, _fit, _plot, _update)
 """Twpa frequency Routine  object."""
```

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/readout_optimization/twpa_calibration/frequency_SNR.py` & `qibocal-0.0.9/src/qibocal/protocols/readout_optimization/twpa_calibration/frequency_SNR.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,23 +5,16 @@
 import numpy.typing as npt
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
 from qibolab.platform import Platform
 from qibolab.qubits import QubitId
 
 from qibocal.auto.operation import Data, Parameters, Results, Routine
-from qibocal.protocols.characterization.resonator_spectroscopy import (
-    resonator_spectroscopy,
-)
-from qibocal.protocols.characterization.utils import (
-    HZ_TO_GHZ,
-    PowerLevel,
-    table_dict,
-    table_html,
-)
+from qibocal.protocols.resonator_spectroscopy import resonator_spectroscopy
+from qibocal.protocols.utils import HZ_TO_GHZ, PowerLevel, table_dict, table_html
 
 
 @dataclass
 class ResonatorTWPAFrequencyParameters(Parameters):
     """ResonatorTWPAFrequency runcard inputs."""
 
     freq_width: int
```

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/readout_optimization/twpa_calibration/frequency_power.py` & `qibocal-0.0.9/src/qibocal/protocols/readout_optimization/twpa_calibration/power_SNR.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,227 +1,264 @@
 from dataclasses import dataclass, field
+from typing import Optional
 
 import numpy as np
 import numpy.typing as npt
 import plotly.graph_objects as go
+from plotly.subplots import make_subplots
 from qibolab.platform import Platform
 from qibolab.qubits import QubitId
 
-from qibocal import update
 from qibocal.auto.operation import Data, Parameters, Results, Routine
-from qibocal.protocols.characterization import classification
-from qibocal.protocols.characterization.utils import HZ_TO_GHZ, table_dict, table_html
+from qibocal.protocols.resonator_spectroscopy import resonator_spectroscopy
+from qibocal.protocols.utils import HZ_TO_GHZ, PowerLevel, table_dict, table_html
 
 
 @dataclass
-class TwpaFrequencyPowerParameters(Parameters):
-    """Twpa Frequency Power runcard inputs."""
+class ResonatorTWPAPowerParameters(Parameters):
+    """ResonatorTWPAPower runcard inputs."""
 
-    frequency_width: float
-    """Frequency total width."""
-    frequency_step: float
-    """Frequency step to be probed."""
-    power_width: float
-    """Power total width."""
-    power_step: float
-    """Power step to be probed."""
+    freq_width: int
+    """Width for frequency sweep relative to the readout frequency (Hz)."""
+    freq_step: int
+    """Frequency step for sweep (Hz)."""
+    twpa_pow_width: int
+    """Width for TPWA power sweep (dBm)."""
+    twpa_pow_step: int
+    """TPWA power step (dBm)."""
+    power_level: PowerLevel
+    """resonator Power regime (low or high)."""
+    nshots: Optional[int] = None
+    """Number of shots."""
+    relaxation_time: Optional[int] = None
+    """Relaxation time (ns)."""
 
+    def __post_init__(self):
+        self.power_level = PowerLevel(self.power_level)
 
-TwpaFrequencyPowerType = np.dtype(
+
+@dataclass
+class ResonatorTWPAPowerResults(Results):
+    """ResonatorTWPAPower outputs."""
+
+    twpa_power: dict[QubitId, float] = field(default_factory=dict)
+    """TWPA frequency [GHz] for each qubit."""
+    frequency: Optional[dict[QubitId, float]] = field(default_factory=dict)
+    """Readout frequency [GHz] for each qubit."""
+    bare_frequency: Optional[dict[QubitId, float]] = field(default_factory=dict)
+    """Bare frequency [GHz] for each qubit."""
+
+
+ResonatorTWPAPowerType = np.dtype(
     [
         ("freq", np.float64),
-        ("power", np.float64),
-        ("assignment_fidelity", np.float64),
-        ("angle", np.float64),
-        ("threshold", np.float64),
+        ("twpa_pow", np.float64),
+        ("signal", np.float64),
+        ("phase", np.float64),
     ]
 )
+"""Custom dtype for Resonator TWPA Power."""
 
 
 @dataclass
-class TwpaFrequencyPowerData(Data):
-    """Twpa Frequency Power acquisition outputs."""
+class ResonatorTWPAPowerData(Data):
+    """ResonatorTWPAPower data acquisition."""
 
-    data: dict[
-        tuple[QubitId, float, float], npt.NDArray[classification.ClassificationType]
-    ] = field(default_factory=dict)
+    resonator_type: str
+    """Resonator type."""
+    data: dict[QubitId, npt.NDArray[ResonatorTWPAPowerType]] = field(
+        default_factory=dict
+    )
     """Raw data acquired."""
-    frequencies: dict[QubitId, float] = field(default_factory=dict)
-    """Frequencies for each qubit."""
-    powers: dict[QubitId, float] = field(default_factory=dict)
-    """Powers for each qubit."""
-
-
-@dataclass
-class TwpaFrequencyPowerResults(Results):
-    """Twpa Frequency Power outputs."""
+    power_level: Optional[PowerLevel] = None
+    """Power regime of the resonator."""
 
-    best_freqs: dict[QubitId, float] = field(default_factory=dict)
-    best_powers: dict[QubitId, float] = field(default_factory=dict)
-    best_fidelities: dict[QubitId, float] = field(default_factory=dict)
-    best_angles: dict[QubitId, float] = field(default_factory=dict)
-    best_thresholds: dict[QubitId, float] = field(default_factory=dict)
+    @classmethod
+    def load(cls, path):
+        obj = super().load(path)
+        # Instantiate PowerLevel object
+        if obj.power_level is not None:  # pylint: disable=E1101
+            obj.power_level = PowerLevel(obj.power_level)  # pylint: disable=E1101
+        return obj
 
 
 def _acquisition(
-    params: TwpaFrequencyPowerParameters,
+    params: ResonatorTWPAPowerParameters,
     platform: Platform,
     targets: list[QubitId],
-) -> TwpaFrequencyPowerData:
+) -> ResonatorTWPAPowerData:
     r"""
-    Data acquisition for TWPA frequency vs. power optmization.
-    This protocol perform a classification protocol for twpa frequencies
-    in the range [twpa_frequency - frequency_width / 2, twpa_frequency + frequency_width / 2]
-    with step frequency_step and powers in the range [twpa_power - power_width / 2, twpa_power + power_width / 2]
+    Data acquisition for TWPA power optmization using SNR.
+    This protocol perform a classification protocol for twpa powers
+    in the range [twpa_power - frequency_width / 2, twpa_power + frequency_width / 2]
+    with step frequency_step.
 
     Args:
-        params (:class:`TwpaFrequencyPowerParameters`): input parameters
+        params (:class:`ResonatorTWPAPowerParameters`): input parameters
         platform (:class:`Platform`): Qibolab's platform
-        targets (list): list of qubit to be characterized
+        qubits (dict): dict of target :class:`Qubit` objects to be characterized
 
     Returns:
-        data (:class:`TwpaFrequencyPowerData`)
+        data (:class:`ResonatorTWPAPowerData`)
     """
 
-    data = TwpaFrequencyPowerData()
+    data = ResonatorTWPAPowerData(
+        power_level=params.power_level,
+        resonator_type=platform.resonator_type,
+    )
 
-    freq_range = np.arange(
-        -params.frequency_width / 2, params.frequency_width / 2, params.frequency_step
-    ).astype(int)
-    power_range = np.arange(
-        -params.power_width / 2, params.power_width / 2, params.power_step
+    TWPAPower_range = np.arange(
+        -params.twpa_pow_width / 2, params.twpa_pow_width / 2, params.twpa_pow_step
     )
-    data = TwpaFrequencyPowerData()
 
-    initial_twpa_freq = {}
-    initial_twpa_power = {}
+    initial_twpa_pow = {}
     for qubit in targets:
-        initial_twpa_freq[qubit] = platform.qubits[
-            qubit
-        ].twpa.local_oscillator.frequency
-        initial_twpa_power[qubit] = platform.qubits[qubit].twpa.local_oscillator.power
-
-        for freq in freq_range:
-            platform.qubits[qubit].twpa.local_oscillator.frequency = (
-                initial_twpa_freq[qubit] + freq
+        initial_twpa_pow[qubit] = float(
+            platform.qubits[qubit].twpa.local_oscillator.power
+        )
+
+    for _pow in TWPAPower_range:
+        for qubit in targets:
+            platform.qubits[qubit].twpa.local_oscillator.power = (
+                initial_twpa_pow[qubit] + _pow
+            )
+
+        resonator_spectroscopy_data, _ = resonator_spectroscopy.acquisition(
+            resonator_spectroscopy.parameters_type.load(
+                {
+                    "freq_width": params.freq_width,
+                    "freq_step": params.freq_step,
+                    "power_level": params.power_level,
+                    "nshots": params.nshots,
+                }
+            ),
+            platform,
+            targets,
+        )
+
+        for qubit in targets:
+            data.register_qubit(
+                ResonatorTWPAPowerType,
+                (qubit),
+                dict(
+                    signal=resonator_spectroscopy_data.data[qubit].signal,
+                    phase=resonator_spectroscopy_data.data[qubit].phase,
+                    freq=resonator_spectroscopy_data.data[qubit].freq,
+                    twpa_pow=_pow + initial_twpa_pow[qubit],
+                ),
             )
 
-            for power in power_range:
-                for qubit in targets:
-                    platform.qubits[qubit].twpa.local_oscillator.power = (
-                        initial_twpa_power[qubit] + power
-                    )
-
-                classification_data = classification._acquisition(
-                    classification.SingleShotClassificationParameters.load(
-                        {"nshots": params.nshots}
-                    ),
-                    platform,
-                    targets,
-                )
-
-                classification_result = classification._fit(classification_data)
-
-                data.register_qubit(
-                    TwpaFrequencyPowerType,
-                    (qubit),
-                    dict(
-                        freq=np.array(
-                            [platform.qubits[qubit].twpa.local_oscillator.frequency],
-                            dtype=np.float64,
-                        ),
-                        power=np.array(
-                            [platform.qubits[qubit].twpa.local_oscillator.power],
-                            dtype=np.float64,
-                        ),
-                        assignment_fidelity=np.array(
-                            [classification_result.assignment_fidelity[qubit]],
-                        ),
-                        angle=np.array([classification_result.rotation_angle[qubit]]),
-                        threshold=np.array([classification_result.threshold[qubit]]),
-                    ),
-                )
     return data
 
 
-def _fit(data: TwpaFrequencyPowerData) -> TwpaFrequencyPowerResults:
-    """Extract fidelity for each configuration qubit / param.
-    Where param can be either frequency or power."""
-
-    best_freq = {}
-    best_power = {}
-    best_fidelity = {}
-    best_angle = {}
-    best_threshold = {}
+def _fit(data: ResonatorTWPAPowerData, fit_type="att") -> ResonatorTWPAPowerResults:
+    """Post-processing function for ResonatorTWPASpectroscopy."""
     qubits = data.qubits
-
+    bare_frequency = {}
+    frequency = {}
+    twpa_power = {}
     for qubit in qubits:
         data_qubit = data[qubit]
-        index_best_err = np.argmax(data_qubit["assignment_fidelity"])
-        best_fidelity[qubit] = data_qubit["assignment_fidelity"][index_best_err]
-        best_freq[qubit] = data_qubit["freq"][index_best_err]
-        best_power[qubit] = data_qubit["power"][index_best_err]
-        best_angle[qubit] = data_qubit["angle"][index_best_err]
-        best_threshold[qubit] = data_qubit["threshold"][index_best_err]
-
-    return TwpaFrequencyPowerResults(
-        best_freq,
-        best_power,
-        best_fidelity,
-        best_angles=best_angle,
-        best_thresholds=best_threshold,
-    )
+        if data.resonator_type == "3D":
+            index_best_pow = np.argmax(data_qubit["signal"])
+        else:
+            index_best_pow = np.argmin(data_qubit["signal"])
+        twpa_power[qubit] = data_qubit["twpa_pow"][index_best_pow]
+
+        if data.power_level is PowerLevel.high:
+            bare_frequency[qubit] = data_qubit["freq"][index_best_pow]
+        else:
+            frequency[qubit] = data_qubit["freq"][index_best_pow]
+
+    if data.power_level is PowerLevel.high:
+        return ResonatorTWPAPowerResults(
+            twpa_power=twpa_power,
+            bare_frequency=bare_frequency,
+        )
+    else:
+        return ResonatorTWPAPowerResults(
+            twpa_power=twpa_power,
+            frequency=frequency,
+        )
 
 
-def _plot(
-    data: TwpaFrequencyPowerData, fit: TwpaFrequencyPowerResults, target: QubitId
-):
-    """Plotting function that shows the assignment fidelity
-    for different values of the twpa frequency for a single qubit"""
+def _plot(data: ResonatorTWPAPowerData, fit: ResonatorTWPAPowerResults, target):
+    """Plotting for ResonatorTWPAPower."""
 
     figures = []
     fitting_report = ""
+    fig = make_subplots(
+        rows=1,
+        cols=2,
+        horizontal_spacing=0.1,
+        vertical_spacing=0.2,
+        subplot_titles=(
+            "Signal [a.u.]",
+            "Phase [rad]",
+        ),
+    )
+
+    fitting_report = ""
+    qubit_data = data[target]
+    frequencies = qubit_data.freq * HZ_TO_GHZ
+    powers = qubit_data.twpa_pow
+
+    fig.add_trace(
+        go.Heatmap(
+            x=frequencies,
+            y=powers,
+            z=qubit_data.signal,
+            colorbar_x=0.46,
+        ),
+        row=1,
+        col=1,
+    )
+    fig.update_xaxes(title_text="Frequency [GHz]", row=1, col=1)
+    fig.update_yaxes(title_text="TWPA Power [dBm]", row=1, col=1)
+    fig.add_trace(
+        go.Heatmap(
+            x=frequencies,
+            y=powers,
+            z=qubit_data.phase,
+            colorbar_x=1.01,
+        ),
+        row=1,
+        col=2,
+    )
+    fig.update_xaxes(title_text="Frequency [GHz]", row=1, col=2)
+    fig.update_yaxes(title_text="TWPA Power [dBm]", row=1, col=2)
+
     if fit is not None:
-        qubit_data = data.data[target]
-        fidelities = qubit_data["assignment_fidelity"]
-        frequencies = qubit_data["freq"]
-        powers = qubit_data["power"]
-        fitting_report = table_html(
-            table_dict(
-                target,
-                ["Best assignment fidelity", "TWPA Frequency [Hz]", "TWPA Power [dBm]"],
-                [
-                    np.round(fit.best_fidelities[target], 3),
-                    fit.best_freqs[target],
-                    np.round(fit.best_powers[target], 3),
-                ],
-            )
-        )
+        label_1 = "TWPA Power"
+        twpa_power = np.round(fit.twpa_power[target])
+        if target in fit.bare_frequency:
+            label_2 = "High Power Resonator Frequency [Hz]"
+            resonator_frequency = np.round(fit.bare_frequency[target])
+        else:
+            label_2 = "Low Power Resonator Frequency [Hz]"
+            resonator_frequency = np.round(fit.frequency[target])
 
-        fig = go.Figure(
+        summary = table_dict(
+            target,
             [
-                go.Heatmap(
-                    x=frequencies * HZ_TO_GHZ, y=powers, z=fidelities, name="Fidelity"
-                )
-            ]
-        )
-
-        fig.update_layout(
-            showlegend=True,
-            xaxis_title="TWPA Frequency [GHz]",
-            yaxis_title="TWPA Power [dBm]",
+                label_2,
+                label_1,
+            ],
+            [
+                resonator_frequency,
+                twpa_power,
+            ],
         )
 
-        figures.append(fig)
+        fitting_report = table_html(summary)
 
-    return figures, fitting_report
+    fig.update_layout(
+        showlegend=False,
+    )
 
+    figures.append(fig)
 
-def _update(results: TwpaFrequencyPowerResults, platform: Platform, target: QubitId):
-    update.twpa_frequency(results.best_freqs[target], platform, target)
-    update.twpa_power(results.best_powers[target], platform, target)
-    update.iq_angle(results.best_angles[target], platform, target)
-    update.threshold(results.best_thresholds[target], platform, target)
+    return figures, fitting_report
 
 
-twpa_frequency_power = Routine(_acquisition, _fit, _plot, _update)
-"""Twpa frequency Routine  object."""
+twpa_power_snr = Routine(_acquisition, _fit, _plot)
+"""Resonator TWPA Power Routine object."""
```

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/readout_optimization/twpa_calibration/power.py` & `qibocal-0.0.9/src/qibocal/protocols/readout_optimization/twpa_calibration/power.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import numpy as np
 import plotly.graph_objects as go
 from qibolab.platform import Platform
 from qibolab.qubits import QubitId
 
 from qibocal import update
 from qibocal.auto.operation import Parameters, Results, Routine
-from qibocal.protocols.characterization import classification
-from qibocal.protocols.characterization.utils import table_dict, table_html
+from qibocal.protocols import classification
+from qibocal.protocols.utils import table_dict, table_html
 
 from . import frequency
 
 
 @dataclass
 class TwpaPowerParameters(Parameters):
     """TwpaPower runcard inputs."""
```

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/resonator_punchout.py` & `qibocal-0.0.9/src/qibocal/protocols/resonator_punchout_attenuation.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,216 +14,214 @@
 from qibocal import update
 from qibocal.auto.operation import Data, Parameters, Results, Routine
 
 from .utils import HZ_TO_GHZ, fit_punchout, norm, table_dict, table_html
 
 
 @dataclass
-class ResonatorPunchoutParameters(Parameters):
-    """ResonatorPunchout runcard inputs."""
+class ResonatorPunchoutAttenuationParameters(Parameters):
+    """ResonatorPunchoutAttenuation runcard inputs."""
 
     freq_width: int
     """Width for frequency sweep relative  to the readout frequency [Hz]."""
     freq_step: int
     """Frequency step for sweep [Hz]."""
-    min_amp_factor: float
-    """Minimum amplitude multiplicative factor."""
-    max_amp_factor: float
-    """Maximum amplitude multiplicative factor."""
-    step_amp_factor: float
-    """Step amplitude multiplicative factor."""
-    amplitude: float = None
-    """Initial readout amplitude."""
+    min_att: int
+    """Attenuation minimum value [dB]."""
+    max_att: int
+    """Attenuation maximum value [dB]."""
+    step_att: int
+    """Attenuation step [dB]."""
 
 
 @dataclass
-class ResonatorPunchoutResults(Results):
-    """ResonatorPunchout outputs."""
+class ResonatorPunchoutAttenuationResults(Results):
+    """ResonatorPunchoutAttenation outputs."""
 
     readout_frequency: dict[QubitId, float]
     """Readout frequency [GHz] for each qubit."""
     bare_frequency: Optional[dict[QubitId, float]]
-    """Bare resonator frequency [GHz] for each qubit."""
-    readout_amplitude: dict[QubitId, float]
-    """Readout amplitude for each qubit."""
+    """Bare resonator frequency [GHZ] for each qubit."""
+    readout_attenuation: dict[QubitId, int]
+    """Readout attenuation [dB] for each qubit."""
 
 
-ResPunchoutType = np.dtype(
+ResPunchoutAttType = np.dtype(
     [
         ("freq", np.float64),
-        ("amp", np.float64),
+        ("att", np.float64),
         ("signal", np.float64),
         ("phase", np.float64),
     ]
 )
 """Custom dtype for resonator punchout."""
 
 
 @dataclass
-class ResonatorPunchoutData(Data):
-    """ResonatorPunchout data acquisition."""
+class ResonatorPunchoutAttenuationData(Data):
+    """ResonatorPunchoutAttenuation data acquisition."""
 
     resonator_type: str
     """Resonator type."""
-    amplitudes: dict[QubitId, float]
-    """Amplitudes provided by the user."""
-    data: dict[QubitId, npt.NDArray[ResPunchoutType]] = field(default_factory=dict)
+    data: dict[QubitId, npt.NDArray[ResPunchoutAttType]] = field(default_factory=dict)
     """Raw data acquired."""
 
-    def register_qubit(self, qubit, freq, amp, signal, phase):
+    def register_qubit(self, qubit, freq, att, signal, phase):
         """Store output for single qubit."""
-        size = len(freq) * len(amp)
-        frequency, amplitude = np.meshgrid(freq, amp)
-        ar = np.empty(size, dtype=ResPunchoutType)
+        size = len(freq) * len(att)
+        ar = np.empty(size, dtype=ResPunchoutAttType)
+        frequency, attenuation = np.meshgrid(freq, att)
         ar["freq"] = frequency.ravel()
-        ar["amp"] = amplitude.ravel()
+        ar["att"] = attenuation.ravel()
         ar["signal"] = signal.ravel()
         ar["phase"] = phase.ravel()
         self.data[qubit] = np.rec.array(ar)
 
 
 def _acquisition(
-    params: ResonatorPunchoutParameters,
+    params: ResonatorPunchoutAttenuationParameters,
     platform: Platform,
     targets: list[QubitId],
-) -> ResonatorPunchoutData:
-    """Data acquisition for Punchout over amplitude."""
+) -> ResonatorPunchoutAttenuationData:
+    """Data acquisition for Punchout over attenuation."""
     # create a sequence of pulses for the experiment:
     # MZ
 
     # taking advantage of multiplexing, apply the same set of gates to all qubits in parallel
     sequence = PulseSequence()
 
     ro_pulses = {}
-    amplitudes = {}
     for qubit in targets:
         ro_pulses[qubit] = platform.create_qubit_readout_pulse(qubit, start=0)
-        if params.amplitude is not None:
-            ro_pulses[qubit].amplitude = params.amplitude
-
-        amplitudes[qubit] = ro_pulses[qubit].amplitude
         sequence.add(ro_pulses[qubit])
 
     # define the parameters to sweep and their range:
     # resonator frequency
     delta_frequency_range = np.arange(
-        -params.freq_width // 2, params.freq_width // 2, params.freq_step
+        -params.freq_width / 2, params.freq_width / 2, params.freq_step
     )
     freq_sweeper = Sweeper(
         Parameter.frequency,
         delta_frequency_range,
         [ro_pulses[qubit] for qubit in targets],
         type=SweeperType.OFFSET,
     )
 
-    # amplitude
-    amplitude_range = np.arange(
-        params.min_amp_factor, params.max_amp_factor, params.step_amp_factor
-    )
-    amp_sweeper = Sweeper(
-        Parameter.amplitude,
-        amplitude_range,
-        [ro_pulses[qubit] for qubit in targets],
-        type=SweeperType.FACTOR,
+    # attenuation
+    attenuation_range = np.arange(params.min_att, params.max_att, params.step_att)
+    att_sweeper = Sweeper(
+        Parameter.attenuation,
+        attenuation_range,
+        qubits=[platform.qubits[qubit] for qubit in targets],
+        type=SweeperType.ABSOLUTE,
     )
 
-    data = ResonatorPunchoutData(
-        amplitudes=amplitudes,
-        resonator_type=platform.resonator_type,
-    )
+    data = ResonatorPunchoutAttenuationData(resonator_type=platform.resonator_type)
 
     results = platform.sweep(
         sequence,
         ExecutionParameters(
             nshots=params.nshots,
             relaxation_time=params.relaxation_time,
             acquisition_type=AcquisitionType.INTEGRATION,
             averaging_mode=AveragingMode.CYCLIC,
         ),
-        amp_sweeper,
+        att_sweeper,
         freq_sweeper,
     )
 
     # retrieve the results for every qubit
-    for qubit, ro_pulse in ro_pulses.items():
-        # average signal, phase, i and q over the number of shots defined in the runcard
-        result = results[ro_pulse.serial]
+    for qubit in targets:
+        result = results[ro_pulses[qubit].serial]
         data.register_qubit(
             qubit,
             signal=result.magnitude,
             phase=result.phase,
-            freq=delta_frequency_range + ro_pulse.frequency,
-            amp=amplitude_range * amplitudes[qubit],
+            freq=delta_frequency_range + ro_pulses[qubit].frequency,
+            att=attenuation_range,
         )
 
+        # # Temporary fixe to force to reset the attenuation to the original value in qblox
+        # # sweeper method returning to orig value not working for attenuation
+        # # After fitting punchout the reload_settings will be called automatically
+        # platform.reload_settings()
+        # save data
     return data
 
 
-def _fit(data: ResonatorPunchoutData, fit_type="amp") -> ResonatorPunchoutResults:
+def _fit(
+    data: ResonatorPunchoutAttenuationData, fit_type="att"
+) -> ResonatorPunchoutAttenuationResults:
     """Fit frequency and attenuation at high and low power for a given resonator."""
 
-    return ResonatorPunchoutResults(*fit_punchout(data, fit_type))
+    return ResonatorPunchoutAttenuationResults(*fit_punchout(data, fit_type))
 
 
 def _plot(
-    data: ResonatorPunchoutData, target: QubitId, fit: ResonatorPunchoutResults = None
+    data: ResonatorPunchoutAttenuationData,
+    target: QubitId,
+    fit: ResonatorPunchoutAttenuationResults = None,
 ):
-    """Plotting function for ResonatorPunchout."""
+    """Plotting for ResonatorPunchoutAttenuation."""
+
     figures = []
     fitting_report = ""
     fig = make_subplots(
         rows=1,
         cols=2,
         horizontal_spacing=0.1,
         vertical_spacing=0.2,
         subplot_titles=(
             "Normalised Signal [a.u.]",
             "phase [rad]",
         ),
     )
+
     qubit_data = data[target]
     frequencies = qubit_data.freq * HZ_TO_GHZ
-    amplitudes = qubit_data.amp
-    n_amps = len(np.unique(qubit_data.amp))
+    attenuations = qubit_data.att
+    n_att = len(np.unique(qubit_data.att))
     n_freq = len(np.unique(qubit_data.freq))
-    for i in range(n_amps):
+    for i in range(n_att):
         qubit_data.signal[i * n_freq : (i + 1) * n_freq] = norm(
             qubit_data.signal[i * n_freq : (i + 1) * n_freq]
         )
 
     fig.add_trace(
         go.Heatmap(
             x=frequencies,
-            y=amplitudes,
+            y=attenuations,
             z=qubit_data.signal,
             colorbar_x=0.46,
         ),
         row=1,
         col=1,
     )
-
+    fig.update_xaxes(title_text="Frequency [GHz]", row=1, col=1)
+    fig.update_yaxes(title_text="Attenuation [dB]", row=1, col=1)
     fig.add_trace(
         go.Heatmap(
             x=frequencies,
-            y=amplitudes,
+            y=attenuations,
             z=qubit_data.phase,
             colorbar_x=1.01,
         ),
         row=1,
         col=2,
     )
+    fig.update_xaxes(title_text="Frequency [GHz]", row=1, col=2)
 
     if fit is not None:
         fig.add_trace(
             go.Scatter(
                 x=[
                     fit.readout_frequency[target] * HZ_TO_GHZ,
                 ],
                 y=[
-                    fit.readout_amplitude[target],
+                    fit.readout_attenuation[target],
                 ],
                 mode="markers",
                 marker=dict(
                     size=8,
                     color="gray",
                     symbol="circle",
                 ),
@@ -232,40 +230,37 @@
             )
         )
         fitting_report = table_html(
             table_dict(
                 target,
                 [
                     "Low Power Resonator Frequency [Hz]",
-                    "Low Power readout amplitude [a.u.]",
+                    "Readout Attenuation [dB]",
                     "High Power Resonator Frequency [Hz]",
                 ],
                 [
-                    np.round(fit.readout_frequency[target]),
-                    np.round(fit.readout_amplitude[target], 3),
+                    np.round(fit.readout_frequency[target], 0),
+                    fit.readout_attenuation[target],
                     np.round(fit.bare_frequency[target]),
                 ],
             )
         )
-
     fig.update_layout(
         showlegend=True,
         legend=dict(orientation="h"),
     )
 
-    fig.update_xaxes(title_text="Frequency [GHz]", row=1, col=1)
-    fig.update_xaxes(title_text="Frequency [GHz]", row=1, col=2)
-    fig.update_yaxes(title_text="Amplitude [a.u.]", row=1, col=1)
-
     figures.append(fig)
 
     return figures, fitting_report
 
 
-def _update(results: ResonatorPunchoutResults, platform: Platform, target: QubitId):
+def _update(
+    results: ResonatorPunchoutAttenuationResults, platform: Platform, target: QubitId
+):
     update.readout_frequency(results.readout_frequency[target], platform, target)
     update.bare_resonator_frequency(results.bare_frequency[target], platform, target)
-    update.readout_amplitude(results.readout_amplitude[target], platform, target)
+    update.readout_attenuation(results.readout_attenuation[target], platform, target)
 
 
-resonator_punchout = Routine(_acquisition, _fit, _plot, _update)
-"""ResonatorPunchout Routine object."""
+resonator_punchout_attenuation = Routine(_acquisition, _fit, _plot, _update)
+"""ResonatorPunchoutAttenuation Routine object."""
```

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/resonator_spectroscopy.py` & `qibocal-0.0.9/src/qibocal/protocols/resonator_spectroscopy.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from dataclasses import dataclass, field, fields
 from typing import Optional, Union
 
 import numpy as np
 import numpy.typing as npt
-from qibolab import AcquisitionType, AveragingMode, ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
 from qibolab.sweeper import Parameter, Sweeper, SweeperType
 
 from qibocal import update
 from qibocal.auto.operation import Data, Parameters, Results, Routine
@@ -45,14 +44,16 @@
     If high both the readout frequency and the bare resonator frequency will be updated."""
     amplitude: Optional[float] = None
     """Readout amplitude (optional). If defined, same amplitude will be used in all qubits.
     Otherwise the default amplitude defined on the platform runcard will be used"""
     attenuation: Optional[int] = None
     """Readout attenuation (optional). If defined, same attenuation will be used in all qubits.
     Otherwise the default attenuation defined on the platform runcard will be used"""
+    hardware_average: bool = True
+    """By default hardware average will be performed."""
 
     def __post_init__(self):
         if isinstance(self.power_level, str):
             self.power_level = PowerLevel(self.power_level)
 
 
 @dataclass
@@ -145,15 +146,15 @@
             attenuation = None
 
         attenuations[qubit] = attenuation
         sequence.add(ro_pulses[qubit])
 
     # define the parameter to sweep and its range:
     delta_frequency_range = np.arange(
-        -params.freq_width // 2, params.freq_width // 2, params.freq_step
+        -params.freq_width / 2, params.freq_width / 2, params.freq_step
     )
     sweeper = Sweeper(
         Parameter.frequency,
         delta_frequency_range,
         pulses=[ro_pulses[qubit] for qubit in targets],
         type=SweeperType.OFFSET,
     )
@@ -162,39 +163,33 @@
         power_level=params.power_level,
         amplitudes=amplitudes,
         attenuations=attenuations,
     )
 
     results = platform.sweep(
         sequence,
-        ExecutionParameters(
-            nshots=params.nshots,
-            relaxation_time=params.relaxation_time,
-            acquisition_type=AcquisitionType.INTEGRATION,
-            averaging_mode=AveragingMode.SINGLESHOT,
-        ),
+        params.execution_parameters,
         sweeper,
     )
 
     # retrieve the results for every qubit
     for qubit in targets:
         result = results[ro_pulses[qubit].serial]
         # store the results
         data.register_qubit(
             ResSpecType,
             (qubit),
             dict(
-                signal=np.abs(result.average.voltage),
-                phase=np.mean(result.phase, axis=0),
+                signal=result.average.magnitude,
+                phase=result.average.phase,
                 freq=delta_frequency_range + ro_pulses[qubit].frequency,
                 error_signal=result.average.std,
-                error_phase=np.std(result.phase, axis=0, ddof=1),
+                error_phase=result.phase_std,
             ),
         )
-    # finally, save the remaining data
     return data
 
 
 def _fit(
     data: ResonatorSpectroscopyData,
 ) -> ResonatorSpectroscopyResults:
     """Post-processing function for ResonatorSpectroscopy."""
```

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/signal_experiments/calibrate_state_discrimination.py` & `qibocal-0.0.9/src/qibocal/protocols/signal_experiments/calibrate_state_discrimination.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/signal_experiments/time_of_flight_readout.py` & `qibocal-0.0.9/src/qibocal/protocols/signal_experiments/time_of_flight_readout.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import plotly.graph_objects as go
 from qibolab import AcquisitionType, AveragingMode, ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
 
 from qibocal.auto.operation import Data, Parameters, Results, Routine
-from qibocal.protocols.characterization.utils import S_TO_NS, table_dict, table_html
+from qibocal.protocols.utils import S_TO_NS, table_dict, table_html
 
 
 @dataclass
 class TimeOfFlightReadoutParameters(Parameters):
     """TimeOfFlightReadout runcard inputs."""
 
     readout_amplitude: Optional[int] = None
```

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/two_qubit_interaction/chevron/chevron.py` & `qibocal-0.0.9/src/qibocal/protocols/two_qubit_interaction/chevron/chevron.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 from qibolab.platform import Platform
 from qibolab.qubits import QubitPairId
 from qibolab.sweeper import Parameter, Sweeper, SweeperType
 from scipy.optimize import curve_fit
 
 from qibocal import update
 from qibocal.auto.operation import Data, Parameters, Results, Routine
-from qibocal.protocols.characterization.utils import table_dict, table_html
+from qibocal.config import log
+from qibocal.protocols.utils import table_dict, table_html
 
 from ..utils import fit_flux_amplitude, order_pair
 from .utils import COLORAXIS, chevron_fit, chevron_sequence
 
 
 @dataclass
 class ChevronParameters(Parameters):
@@ -144,23 +145,21 @@
             platform=platform,
             pair=pair,
             duration_max=params.duration_max,
             parking=params.parking,
             dt=params.dt,
         )
         ordered_pair = order_pair(pair, platform)
-
         # TODO: move in function to avoid code duplications
         sweeper_amplitude = Sweeper(
             Parameter.amplitude,
             params.amplitude_range,
             pulses=[sequence.get_qubit_pulses(ordered_pair[1]).qf_pulses[0]],
             type=SweeperType.FACTOR,
         )
-
         data.native_amplitude[ordered_pair] = (
             sequence.get_qubit_pulses(ordered_pair[1]).qf_pulses[0].amplitude
         )
         data.sweetspot[ordered_pair] = platform.qubits[ordered_pair[1]].sweetspot
         sweeper_duration = Sweeper(
             Parameter.duration,
             params.duration_range,
@@ -168,14 +167,15 @@
             type=SweeperType.ABSOLUTE,
         )
 
         results = platform.sweep(
             sequence,
             ExecutionParameters(
                 nshots=params.nshots,
+                relaxation_time=params.relaxation_time,
                 acquisition_type=AcquisitionType.DISCRIMINATION,
                 averaging_mode=AveragingMode.CYCLIC,
             ),
             sweeper_duration,
             sweeper_amplitude,
         )
         data.register_qubit(
@@ -189,43 +189,36 @@
     return data
 
 
 def _fit(data: ChevronData) -> ChevronResults:
     durations = {}
     amplitudes = {}
     for pair in data.data:
-        pair_amplitude = []
-        pair_duration = []
         amps = data.amplitudes(pair)
         times = data.durations(pair)
 
-        for qubit in pair:
-            signal = (
-                data.low_frequency(pair)
-                if pair[0] == qubit
-                else data.high_frequency(pair)
-            )
-            signal_matrix = signal.reshape(len(times), len(amps)).T
+        signal = data.low_frequency(pair)
+        signal_matrix = signal.reshape(len(times), len(amps)).T
 
-            # guess amplitude computing FFT
-            amplitude, index, delta = fit_flux_amplitude(signal_matrix, amps, times)
-            # estimate duration by rabi curve at amplitude previously estimated
-            y = signal_matrix[index, :].ravel()
+        # guess amplitude computing FFT
+        amplitude, index, delta = fit_flux_amplitude(signal_matrix, amps, times)
+        # estimate duration by rabi curve at amplitude previously estimated
+        y = signal_matrix[index, :].ravel()
 
+        try:
             popt, _ = curve_fit(
                 chevron_fit, times, y, p0=[delta, 0, np.mean(y), np.mean(y)]
             )
 
             # duration can be estimated as the period of the oscillation
             duration = 1 / (popt[0] / 2 / np.pi)
-            pair_amplitude.append(amplitude)
-            pair_duration.append(duration)
-
-        amplitudes[pair] = np.mean(pair_amplitude)
-        durations[pair] = int(np.mean(duration))
+            amplitudes[pair] = amplitude
+            durations[pair] = int(duration)
+        except Exception as e:
+            log.warning(f"Chevron fit failed for pair {pair} due to {e}")
 
     return ChevronResults(amplitude=amplitudes, duration=durations)
 
 
 def _plot(data: ChevronData, fit: ChevronResults, target: QubitPairId):
     """Plot the experiment result for a single pair."""
 
@@ -284,15 +277,15 @@
                         symbol="cross",
                     ),
                     name="CZ estimate",  #  Change name from the params
                     showlegend=True if measured_qubit == target[0] else False,
                     legendgroup="Voltage",
                 ),
                 row=1,
-                col=1 if measured_qubit == target[0] else 2,
+                col=1,
             )
 
     fig.update_layout(
         xaxis_title="Duration [ns]",
         xaxis2_title="Duration [ns]",
         yaxis_title="Amplitude [a.u.]",
         legend=dict(orientation="h"),
```

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/two_qubit_interaction/chevron/chevron_signal.py` & `qibocal-0.0.9/src/qibocal/protocols/two_qubit_interaction/chevron/chevron_signal.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,14 +119,15 @@
             pulses=[sequence.get_qubit_pulses(ordered_pair[1]).qf_pulses[0]],
             type=SweeperType.ABSOLUTE,
         )
         results = platform.sweep(
             sequence,
             ExecutionParameters(
                 nshots=params.nshots,
+                relaxation_time=params.relaxation_time,
                 acquisition_type=AcquisitionType.INTEGRATION,
                 averaging_mode=AveragingMode.CYCLIC,
             ),
             sweeper_duration,
             sweeper_amplitude,
         )
         data.register_qubit(
```

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/two_qubit_interaction/chevron/utils.py` & `qibocal-0.0.9/src/qibocal/protocols/two_qubit_interaction/chevron/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,13 +65,14 @@
     measure_highfreq = platform.create_qubit_readout_pulse(
         ordered_pair[1],
         start=initialize_highfreq.finish + delay_measurement + dt,
     )
 
     sequence.add(measure_lowfreq)
     sequence.add(measure_highfreq)
+
     return sequence
 
 
 # fitting function for single row in chevron plot (rabi-like curve)
 def chevron_fit(x, omega, phase, amplitude, offset):
     return amplitude * np.cos(x * omega + phase) + offset
```

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/two_qubit_interaction/chsh/circuits.py` & `qibocal-0.0.9/src/qibocal/protocols/two_qubit_interaction/chsh/circuits.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/two_qubit_interaction/chsh/protocol.py` & `qibocal-0.0.9/src/qibocal/protocols/two_qubit_interaction/chsh/protocol.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,19 +4,21 @@
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import Optional
 
 import numpy as np
 import numpy.typing as npt
 import plotly.graph_objects as go
+from qibo.backends import GlobalBackend
 from qibolab import ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.qubits import QubitId, QubitPairId
 
 from qibocal.auto.operation import Data, Parameters, Results, Routine
+from qibocal.auto.transpile import dummy_transpiler, execute_transpiled_circuit
 
 from ...readout_mitigation_matrix import (
     ReadoutMitigationMatrixParameters as mitigation_params,
 )
 from ...readout_mitigation_matrix import _acquisition as mitigation_acquisition
 from ...readout_mitigation_matrix import _fit as mitigation_fit
 from ...utils import calculate_frequencies
@@ -186,15 +188,18 @@
                     platform=platform,
                     qubits=pair,
                     theta=theta,
                     bell_state=bell_state,
                 )
                 for basis, sequence in chsh_sequences.items():
                     results = platform.execute_pulse_sequence(
-                        sequence, ExecutionParameters(nshots=params.nshots)
+                        sequence,
+                        ExecutionParameters(
+                            nshots=params.nshots, relaxation_time=params.relaxation_time
+                        ),
                     )
                     frequencies = calculate_frequencies(results, list(pair))
                     data.register_basis(pair, bell_state, basis, frequencies)
     return data
 
 
 def _acquisition_circuits(
@@ -204,15 +209,17 @@
 ) -> CHSHData:
     """Data acquisition for CHSH protocol using circuits."""
     thetas = np.linspace(0, 2 * np.pi, params.ntheta)
     data = CHSHData(
         bell_states=params.bell_states,
         thetas=thetas.tolist(),
     )
-
+    backend = GlobalBackend()
+    transpiler = dummy_transpiler(backend)
+    qubit_map = [i for i in range(platform.nqubits)]
     if params.apply_error_mitigation:
         mitigation_data = mitigation_acquisition(
             mitigation_params(pulses=False, nshots=params.nshots), platform, targets
         )
         mitigation_results = mitigation_fit(mitigation_data)
     for pair in targets:
         if params.apply_error_mitigation:
@@ -225,15 +232,21 @@
                     platform,
                     qubits=pair,
                     bell_state=bell_state,
                     theta=theta,
                     native=params.native,
                 )
                 for basis, circuit in chsh_circuits.items():
-                    result = circuit(nshots=params.nshots)
+                    _, result = execute_transpiled_circuit(
+                        circuit,
+                        nshots=params.nshots,
+                        transpiler=transpiler,
+                        backend=backend,
+                        qubit_map=qubit_map,
+                    )
                     frequencies = result.frequencies()
                     data.register_basis(pair, bell_state, basis, frequencies)
 
     return data
 
 
 def _plot(data: CHSHData, fit: CHSHResults, target: QubitPairId):
```

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/two_qubit_interaction/chsh/pulses.py` & `qibocal-0.0.9/src/qibocal/protocols/two_qubit_interaction/chsh/pulses.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/two_qubit_interaction/chsh/utils.py` & `qibocal-0.0.9/src/qibocal/protocols/two_qubit_interaction/chsh/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Auxiliary functions to run CHSH protocol."""
 
+from qibo.config import log
+
 READOUT_BASIS = ["ZZ", "ZX", "XZ", "XX"]
 
 
 def compute_chsh(frequencies, basis, i):
     """Computes the chsh inequality out of the frequencies of the 4 circuits executed."""
     chsh = 0
     aux = 0
@@ -13,8 +15,12 @@
                 basis % 2
             ):  # This value sets where the minus sign is in the CHSH inequality
                 chsh -= (-1) ** (int(outcome[0]) + int(outcome[1])) * freq[outcome][i]
             else:
                 chsh += (-1) ** (int(outcome[0]) + int(outcome[1])) * freq[outcome][i]
         aux += 1
     nshots = sum(freq[x][i] for x in freq)
-    return chsh / nshots
+    try:
+        return chsh / nshots
+    except ZeroDivisionError:
+        log.warning("Zero number of shots, returning zero.")
+        return 0
```

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/two_qubit_interaction/cz_virtualz.py` & `qibocal-0.0.9/src/qibocal/protocols/two_qubit_interaction/cz_virtualz.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from qibolab.qubits import QubitId, QubitPairId
 from qibolab.sweeper import Parameter, Sweeper, SweeperType
 from scipy.optimize import curve_fit
 
 from qibocal import update
 from qibocal.auto.operation import Data, Parameters, Results, Routine
 from qibocal.config import log
-from qibocal.protocols.characterization.utils import table_dict, table_html
+from qibocal.protocols.utils import table_dict, table_html
 
 from .utils import order_pair
 
 
 @dataclass
 class CZVirtualZParameters(Parameters):
     """CzVirtualZ runcard inputs."""
@@ -232,14 +232,15 @@
                     pulses=[theta_pulse],
                     type=SweeperType.ABSOLUTE,
                 )
                 results = platform.sweep(
                     sequence,
                     ExecutionParameters(
                         nshots=params.nshots,
+                        relaxation_time=params.relaxation_time,
                         acquisition_type=AcquisitionType.DISCRIMINATION,
                         averaging_mode=AveragingMode.CYCLIC,
                     ),
                     sweeper,
                 )
 
                 result_target = results[target_q].probability(1)
```

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/two_qubit_interaction/cz_virtualz_signal.py` & `qibocal-0.0.9/src/qibocal/protocols/two_qubit_interaction/cz_virtualz_signal.py`

 * *Files 6% similar despite different names*

```diff
@@ -102,14 +102,15 @@
                     pulses=[theta_pulse],
                     type=SweeperType.ABSOLUTE,
                 )
                 results = platform.sweep(
                     sequence,
                     ExecutionParameters(
                         nshots=params.nshots,
+                        relaxation_time=params.relaxation_time,
                         acquisition_type=AcquisitionType.INTEGRATION,
                         averaging_mode=AveragingMode.CYCLIC,
                     ),
                     sweeper,
                 )
 
                 result_target = results[target_q].magnitude
```

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/two_qubit_interaction/utils.py` & `qibocal-0.0.9/src/qibocal/protocols/two_qubit_interaction/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,11 +61,11 @@
         values = np.arange(int(len(y) / 2))
         period = len(y) / sampling_freq
         frequencies = values / period
         f = frequencies[index] if index is not None else RANDOM_HIGH_VALUE
         fs.append(2 * np.pi * f)
 
     low_freq_interval = np.where(fs == np.min(fs))
-    amplitude = median_high(amps[low_freq_interval])
+    amplitude = median_high(amps[::-1][low_freq_interval])
     index = int(np.where(np.unique(amps) == amplitude)[0])
     delta = np.min(fs)
     return amplitude, index, delta
```

### Comparing `qibocal-0.0.8/src/qibocal/protocols/characterization/utils.py` & `qibocal-0.0.9/src/qibocal/protocols/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import numpy.typing as npt
 import pandas as pd
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
 from qibolab.qubits import QubitId
 from scipy import constants
 from scipy.optimize import curve_fit
-from scipy.stats import mode
 
 from qibocal.auto.operation import Data, Results
 from qibocal.config import log
 from qibocal.fitting.classifier import run
 
 GHZ_TO_HZ = 1e9
 HZ_TO_GHZ = 1e-9
@@ -28,14 +27,18 @@
 TITLE_SIZE = 25
 EXTREME_CHI = 1e4
 KB = constants.k
 HBAR = constants.hbar
 """Chi2 output when errors list contains zero elements"""
 COLORBAND = "rgba(0,100,80,0.2)"
 COLORBAND_LINE = "rgba(255,255,255,0)"
+CONFIDENCE_INTERVAL_FIRST_MASK = 99
+"""Confidence interval used to mask flux data."""
+CONFIDENCE_INTERVAL_SECOND_MASK = 70
+"""Confidence interval used to clean outliers."""
 
 
 def effective_qubit_temperature(
     prob_0: np.array, prob_1: np.array, qubit_frequency: float, nshots: int
 ):
     """Calculates the qubit effective temperature.
 
@@ -117,39 +120,41 @@
     else:
         guess_center = frequencies[
             np.argmin(voltages)
         ]  # Argmin = Returns the indices of the minimum values along an axis.
         guess_sigma = abs(frequencies[np.argmax(voltages)] - guess_center)
         guess_amp = (np.min(voltages) - guess_offset) * guess_sigma * np.pi
 
-    model_parameters = [
+    initial_parameters = [
         guess_amp,
         guess_center,
         guess_sigma,
         guess_offset,
     ]
     # fit the model with the data and guessed parameters
     try:
         if hasattr(data, "error_signal"):
-            fit_parameters, perr = curve_fit(
-                lorentzian,
-                frequencies,
-                voltages,
-                p0=model_parameters,
-                sigma=data.error_signal,
-            )
-            perr = np.sqrt(np.diag(perr)).tolist()
-        else:
-            fit_parameters, perr = curve_fit(
-                lorentzian,
-                frequencies,
-                voltages,
-                p0=model_parameters,
-            )
-            perr = [0] * 4
+            if not np.isnan(data.error_signal).any():
+                fit_parameters, perr = curve_fit(
+                    lorentzian,
+                    frequencies,
+                    voltages,
+                    p0=initial_parameters,
+                    sigma=data.error_signal,
+                )
+                perr = np.sqrt(np.diag(perr)).tolist()
+                model_parameters = list(fit_parameters)
+                return model_parameters[1] * GHZ_TO_HZ, list(model_parameters), perr
+        fit_parameters, perr = curve_fit(
+            lorentzian,
+            frequencies,
+            voltages,
+            p0=initial_parameters,
+        )
+        perr = [0] * 4
         model_parameters = list(fit_parameters)
         return model_parameters[1] * GHZ_TO_HZ, model_parameters, perr
     except RuntimeError as e:
         log.warning(f"Lorentzian fit not successful due to {e}")
 
 
 def spectroscopy_plot(data, qubit, fit: Results = None):
@@ -160,67 +165,76 @@
         horizontal_spacing=0.1,
         vertical_spacing=0.1,
     )
     qubit_data = data[qubit]
     fitting_report = ""
     frequencies = qubit_data.freq * HZ_TO_GHZ
     signal = qubit_data.signal
-    errors_signal = qubit_data.error_signal
-    errors_phase = qubit_data.error_phase
+
     phase = qubit_data.phase
     fig.add_trace(
         go.Scatter(
             x=frequencies,
             y=signal,
             opacity=1,
             name="Frequency",
             showlegend=True,
             legendgroup="Frequency",
         ),
         row=1,
         col=1,
     )
-    fig.add_trace(
-        go.Scatter(
-            x=np.concatenate((frequencies, frequencies[::-1])),
-            y=np.concatenate((signal + errors_signal, (signal - errors_signal)[::-1])),
-            fill="toself",
-            fillcolor=COLORBAND,
-            line=dict(color=COLORBAND_LINE),
-            showlegend=True,
-            name="Signal Errors",
-        ),
-        row=1,
-        col=1,
-    )
+
     fig.add_trace(
         go.Scatter(
             x=frequencies,
             y=phase,
             opacity=1,
             name="Phase",
             showlegend=True,
             legendgroup="Phase",
         ),
         row=1,
         col=2,
     )
-    fig.add_trace(
-        go.Scatter(
-            x=np.concatenate((frequencies, frequencies[::-1])),
-            y=np.concatenate((phase + errors_phase, (phase - errors_phase)[::-1])),
-            fill="toself",
-            fillcolor=COLORBAND,
-            line=dict(color=COLORBAND_LINE),
-            showlegend=True,
-            name="Phase Errors",
-        ),
-        row=1,
-        col=2,
-    )
+
+    show_error_bars = not np.isnan(qubit_data.error_signal).any()
+    if show_error_bars:
+        errors_signal = qubit_data.error_signal
+        errors_phase = qubit_data.error_phase
+        fig.add_trace(
+            go.Scatter(
+                x=np.concatenate((frequencies, frequencies[::-1])),
+                y=np.concatenate(
+                    (signal + errors_signal, (signal - errors_signal)[::-1])
+                ),
+                fill="toself",
+                fillcolor=COLORBAND,
+                line=dict(color=COLORBAND_LINE),
+                showlegend=True,
+                name="Signal Errors",
+            ),
+            row=1,
+            col=1,
+        )
+
+        fig.add_trace(
+            go.Scatter(
+                x=np.concatenate((frequencies, frequencies[::-1])),
+                y=np.concatenate((phase + errors_phase, (phase - errors_phase)[::-1])),
+                fill="toself",
+                fillcolor=COLORBAND,
+                line=dict(color=COLORBAND_LINE),
+                showlegend=True,
+                name="Phase Errors",
+            ),
+            row=1,
+            col=2,
+        )
+
     freqrange = np.linspace(
         min(frequencies),
         max(frequencies),
         2 * len(frequencies),
     )
 
     if fit is not None:
@@ -242,48 +256,57 @@
         elif data.power_level is PowerLevel.high:
             label = "bare resonator frequency[Hz]"
             freq = fit.bare_frequency
         else:
             label = "qubit frequency[Hz]"
             freq = fit.frequency
 
-        if data.amplitudes[qubit] is not None:
-            fitting_report = table_html(
-                table_dict(
-                    qubit,
-                    [label, "amplitude", "chi2 reduced"],
-                    [
+        if data.attenuations:
+            if data.attenuations[qubit] is not None:
+                if show_error_bars:
+                    labels = [label, "amplitude", "attenuation", "chi2 reduced"]
+                    values = [
                         (
                             freq[qubit],
                             fit.error_fit_pars[qubit][1],
                         ),
                         (data.amplitudes[qubit], 0),
+                        (data.attenuations[qubit], 0),
                         fit.chi2_reduced[qubit],
-                    ],
-                    display_error=True,
+                    ]
+                else:
+                    labels = [label, "amplitude", "attenuation"]
+                    values = [
+                        freq[qubit],
+                        data.amplitudes[qubit],
+                        data.attenuations[qubit],
+                    ]
+        if data.amplitudes[qubit] is not None:
+            if show_error_bars:
+                labels = [label, "amplitude", "chi2 reduced"]
+                values = [
+                    (
+                        freq[qubit],
+                        fit.error_fit_pars[qubit][1],
+                    ),
+                    (data.amplitudes[qubit], 0),
+                    fit.chi2_reduced[qubit],
+                ]
+            else:
+                labels = [label, "amplitude"]
+                values = [freq[qubit], data.amplitudes[qubit]]
+
+            fitting_report = table_html(
+                table_dict(
+                    qubit,
+                    labels,
+                    values,
+                    display_error=show_error_bars,
                 )
             )
-        if data.attenuations:
-            if data.attenuations[qubit] is not None:
-                fitting_report = table_html(
-                    table_dict(
-                        qubit,
-                        [label, "amplitude", "attenuation", "chi2 reduced"],
-                        [
-                            (
-                                freq[qubit],
-                                fit.error_fit_pars[qubit][1],
-                            ),
-                            (data.amplitudes[qubit], 0),
-                            (data.attenuations[qubit], 0),
-                            fit.chi2_reduced[qubit],
-                        ],
-                        display_error=True,
-                    )
-                )
 
     fig.update_layout(
         showlegend=True,
         xaxis_title="Frequency [GHz]",
         yaxis_title="Signal [a.u.]",
         xaxis2_title="Frequency [GHz]",
         yaxis2_title="Phase [rad]",
@@ -324,59 +347,34 @@
 
     low_freqs = {}
     high_freqs = {}
     ro_values = {}
 
     for qubit in qubits:
         qubit_data = data[qubit]
-        freqs = np.unique(qubit_data.freq)
-        nvalues = len(np.unique(qubit_data[fit_type]))
-        nfreq = len(freqs)
-        signals = np.reshape(qubit_data.signal, (nvalues, nfreq))
+        freqs = qubit_data.freq
+        amps = getattr(qubit_data, fit_type)
+        signal = qubit_data.signal
         if data.resonator_type == "3D":
-            peak_freqs = freqs[np.argmax(signals, axis=1)]
+            mask_freq, mask_amps = extract_feature(
+                freqs, amps, signal, "max", ci_first_mask=90
+            )
         else:
-            peak_freqs = freqs[np.argmin(signals, axis=1)]
-
-        max_freq = np.max(peak_freqs)
-        min_freq = np.min(peak_freqs)
-        middle_freq = (max_freq + min_freq) / 2
-
-        freq_hp = peak_freqs[peak_freqs < middle_freq]
-        freq_lp = peak_freqs[peak_freqs >= middle_freq]
-
-        freq_hp = mode(freq_hp, keepdims=True)[0]
-        freq_lp = mode(freq_lp, keepdims=True)[0]
-
+            mask_freq, mask_amps = extract_feature(
+                freqs, amps, signal, "min", ci_first_mask=90
+            )
         if fit_type == "amp":
-            if data.resonator_type == "3D":
-                ro_val = getattr(qubit_data, fit_type)[
-                    np.argmax(
-                        qubit_data.signal[np.where(qubit_data.freq == freq_lp)[0]]
-                    )
-                ]
-            else:
-                ro_val = getattr(qubit_data, fit_type)[
-                    np.argmin(
-                        qubit_data.signal[np.where(qubit_data.freq == freq_lp)[0]]
-                    )
-                ]
+            best_freq = np.max(mask_freq)
+            bare_freq = np.min(mask_freq)
         else:
-            high_att_max = np.max(
-                getattr(qubit_data, fit_type)[np.where(qubit_data.freq == freq_hp)[0]]
-            )
-            high_att_min = np.min(
-                getattr(qubit_data, fit_type)[np.where(qubit_data.freq == freq_hp)[0]]
-            )
-
-            ro_val = round((high_att_max + high_att_min) / 2)
-            ro_val = ro_val + (ro_val % 2)
-
-        low_freqs[qubit] = freq_lp.item()
-        high_freqs[qubit] = freq_hp[0]
+            best_freq = np.min(mask_freq)
+            bare_freq = np.max(mask_freq)
+        ro_val = np.max(mask_amps[mask_freq == best_freq])
+        low_freqs[qubit] = best_freq
+        high_freqs[qubit] = bare_freq
         ro_values[qubit] = ro_val
     return [low_freqs, high_freqs, ro_values]
 
 
 def eval_magnitude(value):
     """number of non decimal digits in `value`"""
     if value == 0 or not np.isfinite(value):
@@ -731,7 +729,46 @@
 
     Return:
         str
     """
     return pd.DataFrame(data).to_html(
         classes="fitting-table", index=False, border=0, escape=False
     )
+
+
+def extract_feature(
+    x: np.ndarray,
+    y: np.ndarray,
+    z: np.ndarray,
+    feat: str,
+    ci_first_mask: float = CONFIDENCE_INTERVAL_FIRST_MASK,
+    ci_second_mask: float = CONFIDENCE_INTERVAL_SECOND_MASK,
+):
+    """Extract feature using confidence intervals.
+
+    Given a dataset of the form (x, y, z) where a spike or a valley is expected,
+    this function discriminate the points (x, y) with a signal, from the pure noise
+    and return the first ones.
+
+    A first mask is construct by looking at `ci_first_mask` confidence interval for each y bin.
+    A second mask is applied by looking at `ci_second_mask` confidence interval to remove outliers.
+    `feat` could be `min` or `max`, in the first case the function will look for valleys, otherwise
+    for peaks.
+
+    """
+
+    masks = []
+    for i in np.unique(y):
+        signal_fixed_y = z[y == i]
+        min, max = np.percentile(
+            signal_fixed_y,
+            [100 - ci_first_mask, ci_first_mask],
+        )
+        masks.append(signal_fixed_y < min if feat == "min" else signal_fixed_y > max)
+
+    first_mask = np.vstack(masks).ravel()
+    min, max = np.percentile(
+        z[first_mask],
+        [100 - ci_second_mask, ci_second_mask],
+    )
+    second_mask = z[first_mask] < max if feat == "min" else z[first_mask] > min
+    return x[first_mask][second_mask], y[first_mask][second_mask]
```

### Comparing `qibocal-0.0.8/src/qibocal/update.py` & `qibocal-0.0.9/src/qibocal/update.py`

 * *Files 9% similar despite different names*

```diff
@@ -61,14 +61,21 @@
 def drive_duration(duration: Union[int, tuple], platform: Platform, qubit: QubitId):
     """Update drive duration value in platform for specific qubit."""
     if isinstance(duration, tuple):
         duration = duration[0]
     platform.qubits[qubit].native_gates.RX.duration = int(duration)
 
 
+def crosstalk_matrix(
+    matrix_element: float, platform: Platform, qubit: QubitId, flux_qubit: QubitId
+):
+    """Update crosstalk_matrix element."""
+    platform.qubits[qubit].crosstalk_matrix[flux_qubit] = float(matrix_element)
+
+
 def iq_angle(angle: float, platform: Platform, qubit: QubitId):
     """Update iq angle value in platform for specific qubit."""
     platform.qubits[qubit].iq_angle = float(angle)
 
 
 def threshold(threshold: float, platform: Platform, qubit: QubitId):
     platform.qubits[qubit].threshold = float(threshold)
```

### Comparing `qibocal-0.0.8/src/qibocal/web/static/styles.css` & `qibocal-0.0.9/src/qibocal/web/static/styles.css`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.8/src/qibocal/web/templates/template.html` & `qibocal-0.0.9/src/qibocal/web/templates/template.html`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 <html lang="en">
 
 <head>
   <meta charset="UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1">
 
   {% if report %}
-  <title>{{ report.title }}</title>
+  <title>{{ title }}</title>
   {% else %}
-  <title>Qibocal {{version}}</title>
+  <title>Qibocal {{report.meta["versions"]["qibocal"]}}</title>
   {% endif %}
 
   <link rel="icon" type="image/x-icon" href="/_favicon.ico?v=2.6.0">
   <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.0/dist/css/bootstrap.min.css" rel="stylesheet"
     integrity="sha384-gH2yIJqKdNHPEq0n4Mqa/HGKIhSkIHeL5AyhkYV8i59U5AR6csBvApHHNl/vI1Bx" crossorigin="anonymous">
 
   <script src="https://cdnjs.cloudflare.com/ajax/libs/jspdf/1.5.3/jspdf.min.js"></script>
@@ -59,19 +59,19 @@
           </li>
           <li class="mb-1">
             <button class="btn btn-toggle d-inline-flex align-items-center rounded border-0" data-bs-toggle="collapse"
               data-bs-target="#actions-collapse" aria-expanded="true">
               Actions
             </button>
             <div class="collapse show" id="actions-collapse">
-              {% for task_uid in report.history  %}
+              {% for task_id in report.history  %}
                 <ul class="btn-toggle-nav list-unstyled fw-normal pb-1 small">
                   <ul class="btn-toggle-nav list-unstyled fw-normal pb-1 small">
                     <li><a class="link-dark d-inline-flex text-decoration-none rounded"
-                        href="#{{report.routine_name(*task_uid)}}"> {{report.routine_name(*task_uid)}}</a></li>
+                        href="#{{report.routine_name(task_id)}}"> {{report.routine_name(task_id)}}</a></li>
                   </ul>
                 </ul>
               {% endfor %}
             </div>
           </li>
           <li class="mb-1">
             <buttom class="btn btn-toggle d-inline-flex align-items-center rounded border-0" data-bs-toggle="collapse"
@@ -93,59 +93,59 @@
               data-bs-toggle="collapse" data-bs-target="#saved-reports" aria-expanded="true">
               Saved reports
             </button>
             <div class="collapse show list-group" id="saved-reports">
               <ul class="btn-toggle-nav list-unstyled fw-normal pb-1 small">
                 {% for folder in folders %}
                 <li><a id="reports" href="{{ url_for('page', path=folder) }}"
-                    class="link-dark d-inline-flex text-decoration-none rounded list-group-item {{ 'active' if folder == report.path else '' }}">{{ folder }}</a></li>
+                    class="link-dark d-inline-flex text-decoration-none rounded list-group-item {{ 'active' if folder == path else '' }}">{{ folder }}</a></li>
                 {% endfor %}
               </ul>
             </div>
           </li>
           {% endif %}
         </ul>
 
       </div>
 
     </nav>
 
     <main class="col-md-9 ms-sm-auto col-lg-10 px-md-4">
 
-      {% if report.path %}
+      {% if path %}
       <div
         class="d-flex justify-content-between flex-wrap flex-md-nowrap align-items-center pt-3 pb-2 mb-3 border-bottom">
-        <h1>{{ report.title }}</h1>
+        <h1>{{ title }}</h1>
         <button class="button-export" id="export-pdf">Export to pdf</button>
       </div>
       <p>
-        Platform: {{ report.metadata.get('platform')}}<br>
-        Run date: {{ report.metadata.get('date') }}<br>
-        Start time (UTC): {{ report.metadata.get('start-time') }}<br>
-        End time (UTC): {{ report.metadata.get('end-time') }}
+        Platform: {{ report.meta.get('platform')}}<br>
+        Run date: {{ report.meta.get('date') }}<br>
+        Start time (UTC): {{ report.meta.get('start-time') }}<br>
+        End time (UTC): {{ report.meta.get('end-time') }}
       </p>
 
       <h3 id="actions"
         class="d-flex justify-content-between flex-wrap flex-md-nowrap align-items-center pt-3 pb-2 mb-3 border-bottom">
         </h3>
 
-      {% for task_uid in report.history %}
 
-      <div id="{{report.routine_name(*task_uid)}}" style="scroll-margin-top: 4em;">
+      {% for task_id in report.history %}
+      <div id="{{report.routine_name(task_id)}}" style="scroll-margin-top: 4em;">
         <h4
           class="d-flex justify-content-between flex-wrap flex-md-nowrap align-items-center pt-3 pb-2 mb-3 border-bottom">
-          {{ report.routine_name(*task_uid) }}</h4>
-        {% for qubit in report.routine_targets(task_uid) %}
+          {{ report.routine_name(task_id) }}</h4>
+        {% for qubit in report.routine_targets(task_id) %}
         <div id="{{ routine }}-{{ iteration }}-{{ qubit }}" style="scroll-margin-top: 4em;">
             <h5
               class="d-flex justify-content-between flex-wrap flex-md-nowrap align-items-center pt-3 pb-2 mb-3 border-bottom">
               {{ header }} - Qubit {{ qubit }}</h5>
 
 
-            {% set figures, fitting_report = report.single_qubit_plot(task_uid, qubit) %}
+            {% set figures, fitting_report = report.plotter(report.history[task_id], qubit) %}
             {{ fitting_report }}
             {{ figures }}
 
             </div>
             {% endfor %}
       </div>
       {% endfor %}
@@ -163,15 +163,15 @@
           <thead>
             <tr>
               <th scope="col">Library</th>
               <th scope="col">Version</th>
             </tr>
           </thead>
           <tbody>
-            {% for library, version in report.metadata.get('versions').items() %}
+            {% for library, version in report.meta.get('versions').items() %}
             <tr>
               <td>{{ library }}</td>
               <td>{{ version }}</td>
             </tr>
             {% endfor %}
           </tbody>
         </table>
```

#### html2text {}

```diff
@@ -5,38 +5,38 @@
 {{ css_styles }} {% else %}
 {% endif %}
 _Q_i_b_o_c_a_l_ _R_e_p_o_r_t_s
     * {% if report %}
     * Home
           o _T_i_m_e_s_t_a_m_p
     * Actions
-      {% for task_uid in report.history %}
-                # _{_{_r_e_p_o_r_t_._r_o_u_t_i_n_e___n_a_m_e_(_*_t_a_s_k___u_i_d_)_}_}
+      {% for task_id in report.history %}
+                # _{_{_r_e_p_o_r_t_._r_o_u_t_i_n_e___n_a_m_e_(_t_a_s_k___i_d_)_}_}
       {% endfor %}
     * Summary
           o _V_e_r_s_i_o_n_s
     * {% endif %} {% if not is_static %}
     * Saved reports
           o {% for folder in folders %}
           o _{_{_ _f_o_l_d_e_r_ _}_}
           o {% endfor %}
     * {% endif %}
-{% if report.path %}
-************ {{{{ rreeppoorrtt..ttiittllee }}}} ************
+{% if path %}
+************ {{{{ ttiittllee }}}} ************
 Export to pdf
-Platform: {{ report.metadata.get('platform')}}
-Run date: {{ report.metadata.get('date') }}
-Start time (UTC): {{ report.metadata.get('start-time') }}
-End time (UTC): {{ report.metadata.get('end-time') }}
-{% for task_uid in report.history %}
-****** {{{{ rreeppoorrtt..rroouuttiinnee__nnaammee((**ttaasskk__uuiidd)) }}}} ******
-{% for qubit in report.routine_targets(task_uid) %}
+Platform: {{ report.meta.get('platform')}}
+Run date: {{ report.meta.get('date') }}
+Start time (UTC): {{ report.meta.get('start-time') }}
+End time (UTC): {{ report.meta.get('end-time') }}
+{% for task_id in report.history %}
+****** {{{{ rreeppoorrtt..rroouuttiinnee__nnaammee((ttaasskk__iidd)) }}}} ******
+{% for qubit in report.routine_targets(task_id) %}
 **** {{{{ hheeaaddeerr }}}} -- QQuubbiitt {{{{ qquubbiitt }}}} ****
-{% set figures, fitting_report = report.single_qubit_plot(task_uid, qubit) %} {
-{ fitting_report }} {{ figures }}
+{% set figures, fitting_report = report.plotter(report.history[task_id], qubit)
+%} {{ fitting_report }} {{ figures }}
 {% endfor %}
 {% endfor %} {% endif %}
 ******** SSuummmmaarryy ********
 In the table below we show the libraries and respective versions used in {
 { report.title }}.
 LLiibbrraarryy       VVeerrssiioonn
 {{ library }} {{ version }}
```

### Comparing `qibocal-0.0.8/PKG-INFO` & `qibocal-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qibocal
-Version: 0.0.8
+Version: 0.0.9
 Summary: Qibo's quantum calibration, characterization and validation module.
 Home-page: https://qibo.science/
 License: Apache-2.0
 Author: andrea-pasquale
 Author-email: andreapasquale97@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
@@ -23,19 +23,19 @@
 Requires-Dist: onnxruntime (>=1.14.1,<2.0.0) ; extra == "classify"
 Requires-Dist: pandas (>=1.4.3,<2.0.0)
 Requires-Dist: plotly (>=5.15.0,<6.0.0)
 Requires-Dist: pydantic (>=1.10.5,<2.0.0)
 Requires-Dist: pydot (>=1.4.2,<2.0.0) ; extra == "viz"
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: qibo (>=0.2.6,<0.3.0)
-Requires-Dist: qibolab (>=0.1.6,<0.2.0)
+Requires-Dist: qibolab (>=0.1.7,<0.2.0)
 Requires-Dist: scikit-learn (>=1.2.1,<2.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: seaborn (>=0.12.2,<0.13.0) ; extra == "classify"
-Requires-Dist: setuptools (>=67.8.0,<68.0.0)
+Requires-Dist: setuptools (>=69.1.1,<70.0.0)
 Requires-Dist: skl2onnx (>=1.14.0,<2.0.0) ; extra == "classify"
 Requires-Dist: skops (>=0.6.0,<0.7.0)
 Project-URL: Documentation, https://qibo.science/qibocal/stable/
 Project-URL: Repository, https://github.com/qiboteam/qibocal/
 Description-Content-Type: text/markdown
 
 # Qibocal
@@ -83,26 +83,25 @@
 This section shows the steps to perform a resonator spectroscopy with Qibocal.
 ### Write a runcard
 A runcard contains all the essential information to run a specific task.
 For our purposes, we can use the following:
 ```yml
 platform: tii1q
 
-qubits: [0]
+targets: [0]
 
 - id: resonator spectroscopy high power
-  priority: 0
   operation: resonator_spectroscopy
   parameters:
     freq_width: 10_000_000
     freq_step: 500_000
     amplitude: 0.4
     power_level: high
     nshots: 1024
-    relaxation_time: 0
+    relaxation_time: 5_000
 
 ```
 ### How to run protocols
 To run the protocols specified in the ```runcard```, Qibocal uses the `qq auto` command
 ```sh
 qq auto <runcard> -o <output_folder>
 ```
```

