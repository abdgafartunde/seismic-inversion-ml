# Seismic Inversion ML

End-to-end learned seismic full-waveform inversion using the OpenFWI benchmark
dataset.

**Status:** Under development.

## Planned

- End-to-end velocity model building with neural networks trained on OpenFWI
  synthetic acoustic data
- Encoder-decoder architectures (InversionNet, SeisInvNet) for mapping
  seismograms directly to velocity models
- Physics-informed augmentation: combining data-driven predictions with
  adjoint-state FWI refinement
- Benchmark evaluation on OpenFWI FlatVel-A, CurveVel-A, and Style-A subsets

## Motivation

The OpenFWI dataset provides large-scale, diverse synthetic seismic data that
enables supervised end-to-end learning for full-waveform inversion. Unlike
classical FWI, which iteratively minimises waveform misfit and is prone to
cycle-skipping, learned approaches can produce velocity models in a single
forward pass when trained on sufficient data. This project implements and
benchmarks several neural architectures on OpenFWI, with the goal of
understanding when end-to-end learning outperforms classical inversion and when
hybrid strategies are needed.

## References

- Deng, C. et al. (2022). OpenFWI: large-scale multi-structural benchmark
  datasets for full waveform inversion. *Advances in Neural Information
  Processing Systems*, 35, 6007--6020.
- Li, S. et al. (2021). InversionNet: an efficient and accurate data-driven
  full waveform inversion. *IEEE Transactions on Geoscience and Remote
  Sensing*, 60, 1--12.

