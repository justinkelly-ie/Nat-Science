# Finite-Science

**A constructive, discrete-mathematical framework for physical law verification, enforcing conservation laws and cosmological structures at compile time in Idris 2.**

[![Idris2](https://img.shields.io/badge/Idris2-QTT_Nat_Types-blue.svg)](https://github.com/idris-lang/Idris2)
[![Verification](https://img.shields.io/badge/Witnesses-172_passing-green.svg)]()
[![License](https://img.shields.io/badge/License-MIT-purple.svg)](LICENSE)

---

## Significance & Integration with Modern Physics

**Finite-Science** complements continuous differential models in modern physics by providing a constructive, exact discrete mathematical engine built on Quantitative Type Theory (QTT) and multiset algebra. Expressing physical laws over exact rational numbers (`UnixelFraction`) and signed integer multiset tokens (`BoxInt`) enables automated, type-safe verification of physical conservation laws without numerical floating-point drift.

This framework integrates directly with established modern physical principles:
* **Constructive Arithmetic & Rational Trigonometry**: Utilizes Wildberger rational spreads, cross-multiplication, and exact metric quadrances to ensure total termination (`%default total`) and exact algebraic equivalence.
* **Exact Conservation Theorems**: Evaluates state evolution via Quantitative Type Theory (QTT) linear multiset operations (`addMultiset`, `lfoldl`), guaranteeing exact compile-time preservation of energy, momentum, charge, and information.
* **Elaborator Reflection Proofs**: Physical invariants, conservation theorems, and geometric classifications are verified at compile time using `%macro` elaboration tactics in Idris 2.

---

## Constructivist 7-Layer Architecture

The physical pipeline builds up systematically across 7 constructivist domain layers:

```text
  Layer 6: Cosmological Master Engine      ← (Idris2-Universe, Idris2-Universe-Wiki)
                     ▲
  Layer 5: Chemistry & Biological Systems  ← (Idris2-Chemistry, Idris2-Biology)
                     ▲
  Layer 4: Physical Laws & Hadron Algebra  ← (Idris2-Physics, Idris2-Hadron)
                     ▲
  Layer 3: 4-Metric Spacetime Geometry     ← (Idris2-Geometry)
                     ▲
  Layer 2: Binary & Ternary Logic Fields   ← (Idris2-Multiset-Binary, Idris2-Multiset-Ternary)
                     ▲
  Layer 1: Multiset Tensor Transforms      ← (Idris2-Multiset-Transform)
                     ▲
  Layer 0: Ground Multiset Memory Kernel   ← (Idris2-Multiset-Core)
```

1. **Layer 0: Ground Multiset Kernel**
   Foundational memory data structures: `BoxInt` signed integer boxes, `Bit` singletons (`Zero`/`One`), QTT linear multisets (`LMultiset`), and type-indexed dependent multisets (`DepMultiset`).
2. **Layer 1: Multiset Tensor Transforms**
   2-Category tensor state machines (`VexelMaxel`, `TransformMultiset`) and $O(\log N)$ parallelized multiset trees (`MultisetTree`).
3. **Layer 2: Binary & Ternary Logic Fields**
   Binary state logic ($\mathbb{F}_2 = \{0, 1\}$) with Möbius transforms (`Idris2-Multiset-Binary`) and balanced ternary spacetime geometry ($\mathbb{F}_3 = \{-1, 0, 1\}$) with Narayana polynomials (`Idris2-Multiset-Ternary`).
4. **Layer 3: 4-Metric Spacetime Geometry**
   The 4 fundamental metrics (Elliptic 27, Hyperbolic 128, Parabolic 55, Substrate 210 master budget) achieving global Helmholtz free energy minimization ($F = -1320$).
5. **Layer 4: Physical Laws & Hadron Confinement**
   44 fundamental constructive physical laws (`Idris2-Physics`) alongside quark-hadron-meson confinement algebra (`Idris2-Hadron`).
6. **Layer 5: Chemistry & Biological Systems**
   Covalent molecular bonding, enzyme Michaelis-Menten kinetics, nucleosynthesis (`Idris2-Chemistry`), progressing to 7-phase matter ascent, ribosomal translation, Hodgkin-Huxley action potentials, and active inference neural networks (`Idris2-Biology`).
7. **Layer 6: Master Engine & Verification Suite**
   The master QTT cosmological state engine (`Idris2-Universe`) and the literate verification test suite (`Idris2-Universe-Wiki`) executing 172 automated proof witnesses (`universe-verify`).

---

## Ecosystem Repository Catalog

The project is organized as a modular ecosystem of 20 domain-specific Idris 2 libraries and verification suites:

| Layer | Domain Library | Verification & Wiki Suite | Core Scope & Key Modules |
| :--- | :--- | :--- | :--- |
| **Layer 0** | [`Idris2-Multiset-Core`](https://github.com/justinkelly-ie/Idris2-Multiset-Core) | [`Idris2-Multiset-Core-Wiki`](https://github.com/justinkelly-ie/Idris2-Multiset-Core-Wiki) | Ground QTT kernel, `BoxInt`, `Bit` singletons (`Zero`/`One`), `DepMultiset` |
| **Layer 1** | [`Idris2-Multiset-Transform`](https://github.com/justinkelly-ie/Idris2-Multiset-Transform) | [`Idris2-Multiset-Transform-Wiki`](https://github.com/justinkelly-ie/Idris2-Multiset-Transform-Wiki) | 2-Category tensor transforms, `VexelMaxel`, `UnixelFraction`, $O(\log N)$ `MultisetTree` |
| **Layer 2a** | [`Idris2-Multiset-Binary`](https://github.com/justinkelly-ie/Idris2-Multiset-Binary) | [`Idris2-Multiset-Binary-Wiki`](https://github.com/justinkelly-ie/Idris2-Multiset-Binary-Wiki) | Binary logic ($\mathbb{F}_2$), Möbius transforms, circuit resolution, functional probability |
| **Layer 2b** | [`Idris2-Multiset-Ternary`](https://github.com/justinkelly-ie/Idris2-Multiset-Ternary) | [`Idris2-Multiset-Ternary-Wiki`](https://github.com/justinkelly-ie/Idris2-Multiset-Ternary-Wiki) | Balanced ternary geometry ($\mathbb{F}_3$), Narayana combinatorial polynomials, tri-state logic |
| **Layer 3** | [`Idris2-Geometry`](https://github.com/justinkelly-ie/Idris2-Geometry) | [`Idris2-Geometry-Wiki`](https://github.com/justinkelly-ie/Idris2-Geometry-Wiki) | 4-Metric Spacetime Geometry (Elliptic 27, Hyperbolic 128, Parabolic 55, Substrate 210) |
| **Layer 4a** | [`Idris2-Physics`](https://github.com/justinkelly-ie/Idris2-Physics) | [`Idris2-Physics-Wiki`](https://github.com/justinkelly-ie/Idris2-Physics-Wiki) | 44 Constructive Physical Laws, Action principle, Page curve, Jarzynski equality |
| **Layer 4b** | [`Idris2-Hadron`](https://github.com/justinkelly-ie/Idris2-Hadron) | [`Idris2-Hadron-Wiki`](https://github.com/justinkelly-ie/Idris2-Hadron-Wiki) | Quark-hadron algebra, Standard Model catalog, multiquark & heavy meson confinement |
| **Layer 5a** | [`Idris2-Chemistry`](https://github.com/justinkelly-ie/Idris2-Chemistry) | [`Idris2-Chemistry-Wiki`](https://github.com/justinkelly-ie/Idris2-Chemistry-Wiki) | Covalent bonding Maxels, substrate-enzyme Michaelis-Menten kinetics, nucleosynthesis |
| **Layer 5b** | [`Idris2-Biology`](https://github.com/justinkelly-ie/Idris2-Biology) | [`Idris2-Biology-Wiki`](https://github.com/justinkelly-ie/Idris2-Biology-Wiki) | 7-phase matter ascent, TRS soundness, ribosomal translation, action potentials, neural networks |
| **Layer 6** | [`Idris2-Universe`](https://github.com/justinkelly-ie/Idris2-Universe) | [`Idris2-Universe-Wiki`](https://github.com/justinkelly-ie/Idris2-Universe-Wiki) | Master QTT Cosmological State Engine & 172-Witness Executable (`universe-verify`) |

---

## Building & Verification Suite

### Prerequisites
Requires **[Idris 2](https://github.com/idris-lang/Idris2)** (`0.8.0` or higher).

### Ecosystem Build Script
To compile and install all 20 packages in dependency sequence:

```bash
./build-all.sh
```

### Running the Verification Binary (`universe-verify`)
To execute all **172 compile-time and runtime proof witnesses**:

```bash
./Idris2-Universe-Wiki/build/exec/universe-verify
```

Expected Output:
```text
========================================================
  IDRIS 2 COSMOLOGICAL UNIVERSE VERIFICATION SUITE
========================================================

Executing Verification Witness Checks...

  [TEST 1] Law 1: Discrete Conservation of Energy: PASSED ✅
  ...
  [TEST 172] Inverted Open Universe Scale Transform Architecture: PASSED ✅

All 172 Cosmological Proof Witnesses & Literate Invariants Verified!
========================================================
```

---

## Interactive 3D Visualizer

The `visualizer/` folder contains an interactive 3D laboratory built with Vite, React, and Three.js, powered by compiled Idris 2 JavaScript code targets:

```bash
cd visualizer
npm install
npm run dev
```

---

&copy; Justin Kelly. Formalized in pair-programming collaboration with Google Antigravity.
