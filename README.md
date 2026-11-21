This repository contains the source of the **O7** Cosmochrony paper  
*Projective Capacity and the Continuum Limit of Admissible Redundancy*.

This work completes the **spectral redundancy programme** by resolving the
obstruction identified in O6: the impossibility of extracting the cascade
exponent from fixed finite-dimensional representations due to bounded
saturation depth.

While **O5–O6** establish that all static fingerprints necessarily saturate,
they leave open a fundamental question: how can redundancy still produce a
non-trivial scaling law along the cascade?

The present work introduces a **coarse-grained notion of projective capacity**
that captures the residual novelty of admissible paths beyond exact linear
independence.

# Core Idea

Instead of measuring redundancy through exact span growth, we define a
mesoscopic quantity:

- **Projective capacity** $\Sigma_n(x)$: accumulated residual novelty of
  $k$-step path fingerprints within coarse-grained cells

This leads to a natural notion of **projective occupancy**:

- $\eta_n(x) = |\psi_n(x)|^2 / \Sigma_n(x)$

The admissible frontier is then governed by a **state equation**:

- $R_n^{(k)}(x) \approx \Phi(\eta_n(x))$

where $\Phi$ is a monotone decreasing function with:

- $\Phi(0) = 1$ (unsaturated regime)
- $\Phi(1) = 1/\sqrt{2}$ (half-occupancy scale)

# Main Results

- Introduction of a **coarse-grained capacity field** $\Sigma_n(x)$ derived
  from path fingerprints
- Establishment of a **monotone state law** linking redundancy to projective
  occupancy
- Reinterpretation of the cascade exponent $\beta$ as the growth exponent of
  projective capacity
- Structural bridge between discrete redundancy (O5–O6) and the continuous
  nonlinear dynamics derived in §B.14 of the white paper

# Physical Interpretation

The nonlinear term appearing in the effective Schrödinger equation:

$$
i\hbar_{\mathrm{eff}}\,\partial_t \psi
= \hat{H}_{\mathrm{eff}} \psi + \frac{\gamma}{\Sigma(x,t)} |\psi|^2 \psi
$$

is interpreted as the **macroscopic manifestation of finite projective capacity**.

In this picture:

- redundancy → capacity depletion
- capacity depletion → increased effective coupling
- increased coupling → nonlinear saturation dynamics

# Position in the Programme

- **O4**: no bound on $\beta$ follows from the bounded-flux and Cheeger argument (candidate open)
- **O5**: vertex-level saturation obstruction
- **O6**: Steinberg-matrix span of dimension $q^2$, filled within a few BFS radii (no general no-go)
- **O7**: emergence of a **capacity-driven continuum description**

O7 shows that the obstruction is not a dead end, but a signal that the
correct observable is not exact redundancy, but its coarse-grained capacity.

# Outlook

The framework opens several directions:

- Rigorous discrete-to-continuum limit $\Sigma_n(x) \to \Sigma(x,t)$
- Determination of the state function $\Phi$ for $k \geq 2$
- Extension to higher-order fingerprints ($k=3$ and beyond)
- Numerical extraction of capacity growth exponents

O7 establishes the first consistent bridge between the discrete spectral
programme and emergent nonlinear quantum dynamics.
