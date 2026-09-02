# Finite-Science

**A deterministic, discrete-geometry natural science model where physical laws and cosmological structures are enforced at compile time over natural and exact rational numbers.**

[![Idris2](https://img.shields.io/badge/Idris2-QTT_Nat_Types-blue.svg)](https://github.com/idris-lang/Idris2)
[![Verification](https://img.shields.io/badge/Witnesses-171_passing-green.svg)]()
[![License](https://img.shields.io/badge/License-MIT-purple.svg)]()

---

## Significance & Core Vision

**Finite-Science** models the physical universe as a discrete, scale-invariant combinatorial engine built on finitist multiset mathematics. By representing coordinates, fields, and states as exact multisets over integers (`BoxInt`) and exact unixel fractions (`UnixelFraction`), physical properties—from elementary particle confinement to molecular bonds, biological folds, and galactic rotation curves—emerge as exact algebraic invariants.

This framework bypasses continuous infinite fields and floating-point approximations:
* **Exact Constructivist Arithmetic**: Uses cross-multiplication, geometric quadrances, and rational spreads to guarantee total termination (`%default total`) without floating-point drift.
* **Automatic Physical Conservation**: Evaluates state transitions via Quantitative Type Theory (QTT) linear multiset operations (`addMultiset`, `lfoldl`, `lmap`), guaranteeing exact conservation of energy, momentum, charge, and information.
* **Elaborator Reflection Macro Audits**: All physical invariants are verified at compile time using `%macro` elaboration tactics.

---

## Emergence of the Universe (Layer-by-Layer Progression)

The universe builds up systematically across 7 distinct constructivist layers:

```
  Layer 6: Universe Engine & Verification  ← (Idris2-Universe, Idris2-Universe-Wiki)
                     ▲
  Layer 5: Chemistry & Biological Systems  ← (Idris2-Chemistry, Idris2-Biology)
                     ▲
  Layer 4: Physical Laws & Hadron Algebra  ← (Idris2-Physics, Idris2-Hadron)
                     ▲
  Layer 3: 4-Metric Spacetime Geometry     ← (Idris2-Geometry)
                     ▲
  Layer 2: Binary & Ternary State Fields   ← (Idris2-Multiset-Binary, Idris2-Multiset-Ternary)
                     ▲
  Layer 1: Multiset Tensor Transforms      ← (Idris2-Multiset-Transform)
                     ▲
  Layer 0: Ground Multiset Memory Kernel   ← (Idris2-Multiset-Core)
```

1. **Layer 0: Ground Multiset Kernel**
   Foundational memory data structures: Run-Length Encoded (RLE) multisets, `BoxInt` bounded integers, `UnixelFraction`, QTT linear multisets (`LMultiset`), and type-indexed dependent multisets (`DepMultiset`).
2. **Layer 1: Multiset Tensor Transforms**
   2-Category tensor state machines (`VexelMaxel`, `TransformMultiset`) and $O(\log N)$ parallelized multiset trees (`MultisetTree`).
3. **Layer 2: Binary & Ternary Logic Fields**
   Binary state logic ($\mathbb{F}_2 = \{0, 1\}$) with Mobius transforms (`Idris2-Multiset-Binary`) and balanced ternary spacetime geometry ($\mathbb{F}_3 = \{-1, 0, 1\}$) with Narayana polynomials (`Idris2-Multiset-Ternary`).
4. **Layer 3: 4-Metric Spacetime Geometry**
   The 4 fundamental geometries (Elliptic 27, Hyperbolic 128, Parabolic 55, Substrate 210 master budget) achieving global Helmholtz free energy minimization ($F = -1320$).
5. **Layer 4: Physical Laws & Hadron Confinement**
   69 fundamental physical laws and conservation theorems (`Idris2-Physics`) alongside quark-hadron-meson confinement algebra (`Idris2-Hadron`).
6. **Layer 5: Chemistry & Biological Systems**
   Chemical bonds, aqueous solvation, base pairing, and nucleosynthesis (`Idris2-Chemistry`), progressing to enzyme kinetics, Hodgkin-Huxley action potentials, ribosomal translation, and active inference neural networks (`Idris2-Biology`).
7. **Layer 6: Universe Engine & Verification Suite**
   The master QTT cosmological state engine (`Idris2-Universe`) and the literate verification test suite (`Idris2-Universe-Wiki`) executing 171 automated proof witnesses (`universe-verify`).

---

## Repository Catalog

The project is structured as a modular ecosystem of 11 domain-specific Idris 2 libraries:

| Layer | Repository | Package Name | Scope & Key Modules | GitHub Link |
| :--- | :--- | :--- | :--- | :--- |
| **Layer 0** | **`Idris2-Multiset-Core`** | `Idris2-Multiset-Core` | Ground QTT memory kernel, `BoxInt`, `UnixelFraction`, `DepMultiset`, `LMultiset` | [justinkelly-ie/Idris2-Multiset-Core](https://github.com/justinkelly-ie/Idris2-Multiset-Core) |
| **Layer 1** | **`Idris2-Multiset-Transform`** | `Idris2-Multiset-Transform` | 2-Category tensor transforms, `VexelMaxel`, `TransformMultiset`, `MultisetTree` | [justinkelly-ie/Idris2-Multiset-Transform](https://github.com/justinkelly-ie/Idris2-Multiset-Transform) |
| **Layer 2a** | **`Idris2-Multiset-Binary`** | `Idris2-Multiset-Binary` | Modulo-2 binary logic (F_2 = {0, 1}), Mobius transforms, circuit resolution | [justinkelly-ie/Idris2-Multiset-Binary](https://github.com/justinkelly-ie/Idris2-Multiset-Binary) |
| **Layer 2b** | **`Idris2-Multiset-Ternary`** | `Idris2-Multiset-Ternary` | Balanced ternary geometry (F_3 = {-1, 0, 1}), Narayana combinatorial polynomials | [justinkelly-ie/Idris2-Multiset-Ternary](https://github.com/justinkelly-ie/Idris2-Multiset-Ternary) |
| **Layer 3** | **`Idris2-Geometry`** | `Idris2-Geometry` | 4-Metric Spacetime Geometry (Elliptic 27, Hyperbolic 128, Parabolic 55, Substrate 210) | [justinkelly-ie/Idris2-Geometry](https://github.com/justinkelly-ie/Idris2-Geometry) |
| **Layer 4a** | **`Idris2-Physics`** | `Idris2-Physics` | 69 Fundamental Physical Laws, Landauer bound, Page curve, Jarzynski equality | [justinkelly-ie/Idris2-Physics](https://github.com/justinkelly-ie/Idris2-Physics) |
| **Layer 4b** | **`Idris2-Hadron`** | `Idris2-Hadron` | Quark-hadron algebra, multiquark & heavy meson confinement | [justinkelly-ie/Idris2-Hadron](https://github.com/justinkelly-ie/Idris2-Hadron) |
| **Layer 5a** | **`Idris2-Chemistry`** | `Idris2-Chemistry` | Molecular bonding, hydrogen bonding, Watson-Crick base pairing, nucleosynthesis | [justinkelly-ie/Idris2-Chemistry](https://github.com/justinkelly-ie/Idris2-Chemistry) |
| **Layer 5b** | **`Idris2-Biology`** | `Idris2-Biology` | Enzyme kinetics, action potentials, allostery, ribosomal translation, neural networks | [justinkelly-ie/Idris2-Biology](https://github.com/justinkelly-ie/Idris2-Biology) |
| **Layer 6a** | **`Idris2-Universe`** | `Idris2-Universe` | Master QTT Cosmological State Machine & Elaborator Reflection Suite | [justinkelly-ie/Idris2-Universe](https://github.com/justinkelly-ie/Idris2-Universe) |
| **Layer 6b** | **`Idris2-Universe-Wiki`** | `Idris2-Universe-Wiki` | Literate Verification Test Suite (`universe-verify`) | [justinkelly-ie/Idris2-Universe-Wiki](https://github.com/justinkelly-ie/Idris2-Universe-Wiki) |

---

## Building & Verification

### Prerequisites
The stack requires **[Idris 2](https://github.com/idris-lang/Idris2)** and **[pack](https://github.com/stefan-hoeck/idris2-pack)**.

### Building the Entire Stack
To build all 11 libraries in dependency sequence:
```bash
# Inside fedora-toolbox-44 or native shell:
toolbox run -c fedora-toolbox-44 /var/home/justin/.local/bin/pack build  # inside Idris2-Universe-Wiki
```

### Running the Verification Suite (`universe-verify`)
To execute all **171 compile-time and runtime proof witnesses**:
```bash
toolbox run -c fedora-toolbox-44 /var/home/justin/.local/bin/pack run    # inside Idris2-Universe-Wiki
```

Expected Output:
```text
========================================================
   Idris2-Universe Verification & Cosmological Suite   
   (Pure Elaborator Reflection + QTT Architecture)      
========================================================

Executing 171 Verification Witness Checks...

  [TEST 1] Law 1: Discrete Conservation of Energy: PASSED ✅
  ...
  [TEST 171] Planck 2018 Primordial Inflation n_s = 0.965 Confidence Interval: PASSED ✅

All Cosmological Proof Witnesses & Literate Invariants Verified!
  ⚡ Total Runtime Evidence Benchmark: duration: 0s 2189410ns
========================================================
```

---

## Interactive 3D Visualizer

The `visualizer/` folder contains an interactive 3D laboratory built with Vite, React, and Three.js, powered directly by the compiled Idris 2 JavaScript web assembly target:

```bash
cd visualizer
npm install
npm run dev
```

---

&copy; Justin Kelly. All rights reserved. Formalized in pair-programming collaboration with Google Antigravity.
