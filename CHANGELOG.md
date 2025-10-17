<!-- Entries in each category are sorted by merge time, with the latest PRs appearing first. -->

# Changelog

All notable changes to this project will be documented in this file.

The format is based on a mixture of [Keep a Changelog](https://keepachangelog.com/en/1.1.0/) and [Common Changelog](https://common-changelog.org).
This project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html), with the exception that minor releases may include breaking changes.

## [Unreleased]

### Added

- 👷 Enable testing on Python 3.14 ([#705]) ([**@denialhaag**])

### Changed

- 🐛 Fix layout preservation and ensure native gate compliance for mirror circuit generation ([#708]) ([**@soroushfathi**])


### Removed

- 🔥 Drop support for Python 3.9 ([#671]) ([**@denialhaag**])

## [2.0.1] - 2025-07-28

### Changed

- 🎨 Rename CLI from `mqt.bench.cli` to `mqt-bench` ([#625]) ([**@burgholzer**], [**@nquetschlich**])
- 📝 Rewrite the usage documentation to include the CLI ([#625]) ([**@burgholzer**], [**@nquetschlich**])

## [2.0.0] - 2025-06-24

_If you are upgrading: please see [`UPGRADING.md`](UPGRADING.md#200)._

### Added

- ✨ Add mirror circuit option for all benchmarks ([#577], [#603]) ([**@CreativeBinBag**], [**@burgholzer**], [**@nquetschlich**])
- ✨ Add arithmetic benchmarks ([#586]) ([**@simon1hofmann**], [**@burgholzer**])
- ✨ Add registry for benchmarks, devices, and native gatesets ([#585], [#572]) ([**@simon1hofmann**], [**@burgholzer**])
- ✨ Add symbolic parameters for variational benchmarks ([#581]) ([**@nquetschlich**], [**@burgholzer**])
- ✨ Add distinct `get_benchmark` function per level ([#571]) ([**@simon1hofmann**], [**@burgholzer**])
- ✨ Add HHL algorithm ([#582]) ([**@nquetschlich**], [**@burgholzer**])
- ✨ Add support for compiling to the Clifford+T gateset ([#555]) ([**@simon1hofmann**], [**@burgholzer**], [**@nquetschlich**])
- ✨ Add two benchmarks from BMW's QUARK framework ([#541]) ([**@fkiwit**])
- ✨ Add support for exporting to OpenQASM 3 ([#518]) ([**@simon1hofmann**], [**@burgholzer**], [**@nquetschlich**])
- ✨ Add support for exporting to Qiskit's QPY ([#518]) ([**@simon1hofmann**], [**@burgholzer**], [**@nquetschlich**])
- ✨ Add Bernstein-Vazirani algorithm ([#505]) ([**@simon1hofmann**], [**@burgholzer**], [**@nquetschlich**])

### Changed

- ✨ Call `transpile` for optimization at the target-independent level ([#580]) ([**@simon1hofmann**], [**@burgholzer**])
- 🎨 Adjust supported IonQ Devices and update all Calibration Data ([#570]) ([**@nquetschlich**], [**@burgholzer**])
- 🎨 Correct the Rigetti gateset to only support RX gate with specific and not arbitrary angles and updated the calibration data ([#570]) ([**@nquetschlich**], [**@burgholzer**])
- ✨ Switch device and gateset representation to Qiskit's Target ([#560]) ([**@burgholzer**], [**@nquetschlich**])
- 📝 Update and modernize project documentation ([#566]) ([**@simon1hofmann**])
- 📝 Add CHANGELOG and UPGRADING info ([#567]) ([**@simon1hofmann**])
- 🎨 Shorten and improve the generation logic of the Shor benchmark ([#548]) ([**@simon1hofmann**])
- 🚚 Rebrand and move to MQT GitHub organization ([#544]) ([**@simon1hofmann**])
- ✨ Re-add Python 3.9 support ([#531]) ([**@simon1hofmann**])
- 🎨 Rename random circuit and VQE ansatz circuit benchmarks ([#508]) ([**@simon1hofmann**], [**@nquetschlich**])
- 🎨 Re-implement amplitude estimation without Qiskit Application modules ([#506]) ([**@simon1hofmann**], [**@burgholzer**], [**@nquetschlich**])

### Removed

- 🔥 Remove Generation Logic for Webpage ([#538]) ([**@nquetschlich**])
- 🔥 Remove TKET-related functionality ([#519], [#510]) ([**@simon1hofmann**])
- 🔥 Remove Qiskit Application-based benchmarks ([#507]) ([**@simon1hofmann**], [**@nquetschlich**])
- 🔥 Remove `benchviewer` and `evaluation` modules ([#504]) ([**@burgholzer**], [**@nquetschlich**])

## [1.1.9] - 2024-12-01

_📚 Refer to the [GitHub Release Notes] for previous changelogs._

<!-- Version links -->

[unreleased]: https://github.com/munich-quantum-toolkit/bench/compare/v2.0.1...HEAD
[2.0.1]: https://github.com/munich-quantum-toolkit/bench/releases/tag/v2.0.1
[2.0.0]: https://github.com/munich-quantum-toolkit/bench/releases/tag/v2.0.0
[1.1.9]: https://github.com/munich-quantum-toolkit/bench/releases/tag/v1.1.9

<!-- PR links -->

[#705]: https://github.com/munich-quantum-toolkit/bench/pull/705
[#671]: https://github.com/munich-quantum-toolkit/bench/pull/671
[#666]: https://github.com/munich-quantum-toolkit/bench/pull/666
[#625]: https://github.com/munich-quantum-toolkit/bench/pull/625
[#603]: https://github.com/munich-quantum-toolkit/bench/pull/603
[#586]: https://github.com/munich-quantum-toolkit/bench/pull/586
[#585]: https://github.com/munich-quantum-toolkit/bench/pull/585
[#582]: https://github.com/munich-quantum-toolkit/bench/pull/582
[#581]: https://github.com/munich-quantum-toolkit/bench/pull/581
[#580]: https://github.com/munich-quantum-toolkit/bench/pull/580
[#577]: https://github.com/munich-quantum-toolkit/bench/pull/577
[#572]: https://github.com/munich-quantum-toolkit/bench/pull/572
[#571]: https://github.com/munich-quantum-toolkit/bench/pull/571
[#570]: https://github.com/munich-quantum-toolkit/bench/pull/570
[#567]: https://github.com/munich-quantum-toolkit/bench/pull/567
[#566]: https://github.com/munich-quantum-toolkit/bench/pull/566
[#560]: https://github.com/munich-quantum-toolkit/bench/pull/560
[#555]: https://github.com/munich-quantum-toolkit/bench/pull/555
[#548]: https://github.com/munich-quantum-toolkit/bench/pull/548
[#544]: https://github.com/munich-quantum-toolkit/bench/pull/544
[#541]: https://github.com/munich-quantum-toolkit/bench/pull/541
[#538]: https://github.com/munich-quantum-toolkit/bench/pull/538
[#531]: https://github.com/munich-quantum-toolkit/bench/pull/531
[#519]: https://github.com/munich-quantum-toolkit/bench/pull/519
[#518]: https://github.com/munich-quantum-toolkit/bench/pull/518
[#510]: https://github.com/munich-quantum-toolkit/bench/pull/510
[#508]: https://github.com/munich-quantum-toolkit/bench/pull/508
[#507]: https://github.com/munich-quantum-toolkit/bench/pull/507
[#506]: https://github.com/munich-quantum-toolkit/bench/pull/506
[#505]: https://github.com/munich-quantum-toolkit/bench/pull/505
[#504]: https://github.com/munich-quantum-toolkit/bench/pull/504

<!-- Contributor -->

[**@burgholzer**]: https://github.com/burgholzer
[**@simon1hofmann**]: https://github.com/simon1hofmann
[**@nquetschlich**]: https://github.com/nquetschlich
[**@fkiwit**]: https://github.com/fkiwit
[**@CreativeBinBag**]: https://github.com/CreativeBinBag
[**@denialhaag**]: https://github.com/denialhaag

<!-- General links -->

[Keep a Changelog]: https://keepachangelog.com/en/1.1.0/
[Common Changelog]: https://common-changelog.org
[Semantic Versioning]: https://semver.org/spec/v2.0.0.html
[GitHub Release Notes]: https://github.com/munich-quantum-toolkit/bench/releases
