_______________________________________________________________________________
# Results Log: Phase Coherent Positioning of Vehicles using Array-of-Sub-Arrays
_______________________________________________________________________________

Author: Victor Pettersson, vicpett@chalmers.se

$\KaTeX$

## Phase-Coherent Objective Function

Here, I present some interesting results produced concerning the phase-coherent maximum likelihood (ML) objective function for positioning the vehicle. First, I briefly introduce the signal model used. We consider a DL vehicular positioning scenario; a basestation transmits a known reference signal using $M_\mathrm{tx}$ beams, illuminating the vehicle. The vehicle is equipped with $K$ sub-arrays for reception of the signal, each capable of making fully digital observation over $M_\mathrm{rx}$ antenna elements and $N$ subcarriers. If we assume that the sub-arrays are all phase-synchronized (coherent), then we can consider the entire vehicle as one large near-field array - however, locally at each sub-array we consider a far-field model. Consider the $k$-th sub-array, the sub-array local, vectorized signal model is 

$$
\mathbf{y}_k = \sum_{\ell = 0}^{L-1} \gamma_{k, \ell} \mathbf{c}(\bm{\psi}_{k, \ell}, \bm{\theta}_{k, \ell}, \tau_{k, \ell}) + \mathbf{z}_k \in \mathbb{C}^{M_\mathrm{tx} M_\mathrm{rx} N \times 1} \,,
$$

where the $(k, \ell)$ subscript indicates the $\ell$-th path incident on the $k$-th subarray, $\gamma_{k, \ell}$ is the corresponding complex channel gain, $\bm{\psi}_{k, \ell}$ is the angles-of-departure from the basestation, $\bm{\theta}_{k, \ell}$ is the angles-of-arrival at the receiving sub-array and $\tau_{k, \ell}$ is the delay. The vector $\mathbf{c}_{k, \ell} = \mathbf{c}(\bm{\psi}_{k, \ell}, \bm{\theta}_{k, \ell}, \tau_{k, \ell}) $ is a tall steering vector and $\mathbf{z}_k$ is AWGN for modeling thermal noise.

.gif:

![](https://github.com/vicpett/markdown-stuff/blob/main/figures/movie-20250616-0840.gif)

.png:

![](https://github.com/vicpett/markdown-stuff/blob/main/figures/9.png)

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTEwNzczNTY0ODBdfQ==
-->
