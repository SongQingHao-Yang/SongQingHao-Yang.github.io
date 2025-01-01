---
layout: project
title: 'Integrated Quantum Photonics with Semiconductor Single Photon Sources'
# author: peteryang
tags: [projects]
img: qd.jpeg
display-order: 1
description: >
---

Supervisor: Mete Atature (Professor of Physics, Fellow, Director of Studies and Tutor at St. John’s College)
 
# Abstract

The utilization of classical integrated photonic technologies and devices in quantum applications is known as integrated quantum photonics. Single photon sources with high purity have been demonstrated using semiconductor quantum dots as a confinement for exciton generation, as well as advanced nanofabrication techniques. Optical cavity and waveguides embedded with quantum dots are popular methods for manipulating quantum state. One of the current challenges in universal quantum computation is verifying quantumness, which can be accomplished through Boson sampling. This computational task is believed to be difficult for classical computers, but can be efficiently solved by orchestrated Bosonic interference in a specialized quantum computer. Near-unity efficient single photon sources have made these experiments possible by the production of indistinguishable photons. This review of solid-state quantum optics research will provide a deeper understanding of its near-term applications.


# Introduction

Integrated quantum photonics (IQP) has emerged as a promising platform for the generation, manipulation, and detection of single photons. With the rapid advancements in nanofabrication techniques, researchers have been able to integrate various quantum photonic components onto a single chip, enabling precise control over the generation and manipulation of individual photons. Among the crucial components in integrated quantum photonics is the single photon source, which plays a fundamental role in applications such as Boson sampling.

Traditionally, single photon sources were realized using bulk optics setups, which are complex and challenging to miniaturize. However, by leveraging the principles of integrated photonics, as with integrated electronics, researchers have made significant strides in developing compact and efficient single photon sources that can be seamlessly integrated into chip-scale devices. These integrated single photon sources offer several advantages over their bulk counterparts, including enhanced stability, scalability, and compatibility with on-chip quantum circuits.

![](/public/img/qd_img/klm.jpeg)

One approach to realizing single photon sources in IQP is through the use of quantum emitters embedded in photonic waveguides or cavities. Quantum dots (QD), for example, have been extensively studied as solid-state emitters capable of emitting single photons on demand. By integrating quantum dots with photonic structures, such as nanowires or photonic crystal cavities, researchers have achieved high-efficiency single photon emission with precise control over the emission wavelength and polarization.

In this paper, we review the recent advancements in GaAs based single photon sources using integrated quantum photonics. We discuss the background of light matter interaction in QD (section 2), different approaches (section 3), and fabrications (section 4). Furthermore, we explore the applications and future prospects of integrated single photon sources in the context of Boson sampling (section 5) and other emerging quantum technologies.

![](/public/img/qd_img/qd.png)

Quantum dots are materials that have dimensions and atom numbers falling between the atomic-molecular level and bulk materials, and their band-gap depends on a variety of factors in a complex manner. For instance, the band gap of InAs quantum dots sandwiched between GaAs layers is much larger at 1.25 eV, as opposed to the bulk InAs value of $\sim$ 0.4eV. Isolated single atoms exhibit sharp and narrow luminescent emission peaks, while nanoparticles consisting of 100-1000 atoms display different narrow optical lines. The most critical feature of quantum dots is their quantum confinement, which imparts a $\delta$-function-like density of states as in Figure 2.

Quantum confinement arises when electrons are confined to a region comparable in size to their de Broglie wavelength, and the energy level spacing of the nanocrystal exceeds $k_bT$. When electrons are excited across the band-gap, interesting properties emerge as they interact with the valence band hole, resulting in single or multiple excitons populating the quantum dot.


## Excitons in quantum dots
Dominated by quantum confinement, electrons and holes in QD behaves like a two-level system, where the lowest-energy electronic excitation (heavy-hole exciton, $\mathbf{X}$) involves one electron in the conduction band and one hole in the valence band as shown in Figure 4. Within high energy scale, biexciton and multiexcitons are possible with coulomb interactions. 

Usually the the heavy-hole–light-hole degeneracy is lifted in a self-assembled QD by the difference in effective masses of valence band and the asymmetric shape of the confinement, which has aspect ratio larger than unity with the dominant quantization axis being the growth direction. Most researches dealt with heavy holes because they are energetically above light ones thus a higher density of states.

## Bright and Dark excitons

Single photons are generated when an electron-heavy-hole pair has anti-parallel spins, which is referred to as a bright exciton. Conversely, when the electron and hole spins are parallel to one another, a dark exciton is produced. The exchange interaction between the pair leads to energy splitting, known as fine structure splitting (FSS), between the bright and dark states.

![](/public/img/qd_img/img/split.png)

The bright exciton preferentially decays through radiative recombination channel while dark exciton decay through non-radiative channels. Although this means that the dark exciton has much longer lifetime, we need bright excitons as the photon source. Interestingly, by engineering the spin-flip, dark exciton undergoes a transition into a bright exciton.


![](/public/img/qd_img/img/hv.png)

![](/public/img/qd_img/img/sum_exciton.png)

## Exciton exciton interaction

Having considered the aforementioned points, we can now establish the requirement for generating a pair of polarization-entangled photons from biexcitons. Each photon can exhibit one of two mutually complementary polarizations, denoted as horizontal (H) and vertical (V) in reference to the asymmetry axis of the quantum dot (QD), as depicted in Figure 3. We can then write out the state as:


$$\begin{equation}
    \ket{\psi} = \frac{1}{\sqrt{2}} ( \ket{H_{XX}} \ket{H_{X}}  +  \ket{V_{XX}} \ket{V_{X}} )
\end{equation}
$$

To achieve entanglement, two conditions must be met: the intermediate exciton states should be degenerate, and the final state of the quantum dot (QD) must be unaffected by the decay path. Suppression of Fine Structure Splitting (FSS) is crucial as it allows the biexciton to decay into two bright excitons with opposite circular polarizations. In order to generate an entangled pair of excitons, the FSS value must be smaller than the exciton linewidth to ensure that the decay process is indistinguishable. The state of art fidelity of entanglement generation has already exceeded 97%.

![](/public/img/qd_img/img/intensity_ex.png)

# Photonic Structure
## Cavity

Another way to create indistinguishable photon is by employing single photon source.
A high-quality single-photon source produces photons with a well-defined quantum state, which ensures that each emitted photon has consistent properties, such as narrow temporal emission profiles, polarization, and spatial mode. But typically, such device suffer from poor performance as photons are emitted randomly in space, and dephasing mechanisms are strong. However, the use of a quantum emitter embedded in a cavity with a high Q factor and a small mode volume can improve photon's indistinguishability. This is achieved by reducing photon's spectral linewidth. Cavity acts as a filter, only allowing photons of a certain frequency to pass through. By choosing the appropriate cavity parameters, the spectral linewidth of the emitted photons can be narrowed, leading to indistinguishable photons. The efficiency can be enhanced by increasing the spontaneous emission rate of the emitter relative to its value in bulk or free space, through coupling it to the cavity mode, a phenomenon known as the Purcell effect. Consequently, the fraction of photons coupled to the cavity mode that are redirected towards a specific output increases, thus improving the external out-coupling efficiency. Furthermore, the Purcell effect significantly reduces the radiative lifetime below the dephasing time, resulting in increased purification of emitted photons and a higher possible repetition rate of the source.
% Single-photon efficiency and indistinguishability are normally poor because photons are emitted in random directions in space, and dephasing mechanisms are strong. However, both efficiency and indistinguishability can be improved by embedding a quantum emitter into a cavity that has a high Q factor and a small mode volume, enhancing the spontaneous emission rate of the emitter relative to its value in bulk (or free space) as a result of its coupling to the cavity mode (known as the Purcell effect). In this case, the external out-coupling efficiency is improved by increasing the fraction of photons coupled to the cavity mode that are redirected towards a particular output where they can be collected. In addition, as a result of the Purcell effect, the radiative lifetime is reduced significantly below the dephasing time, increasing the indistinguishability of emitted photons and the possible repetition rate of the source. 

Two decisive parameters for cavity-QED are quality factor Q and effective mode volume V, represented as:
$$
\begin{equation}
    F_{p} = \frac{\Gamma_{cav}}{\Gamma_{bulk}} = \frac{3}{4\pi^{2}} (\frac{\lambda}{n})^{3} \frac{Q}{V_{eff}}
\end{equation}
$$

where $\Gamma_{cav}$ means the decay into the targeted mode while $\Gamma_{bulk}$ is the one in the whole bulk materials.

Note that in this context, F represents the maximum achievable value of the Purcell factor. Since the mode volume of nanophotonic cavities is not easily measurable, the Purcell factor experienced by a quantum emitter when resonating with the cavity is often used as a metric. To achieve a large F, it is important to ensure deterministic photon emission into a single optical mode and the efficiency, $\beta$ (equation 3), is defined as the ratio of the emission into the target mode compared to all modes.
% Note here the F means the maximum value Purcell factor can achieve. Because the mode volume is not a readily measurable quantity for nanophotonic cavities, we normally choose instead to specify the Purcell factor that a quantum emitter in the cavity experiences when being resonant with the cavity. To get a large F, we need to ensure a deterministic photon emission into a single optical mode can be achieved with an efficiency close to unity for a very large F, for example, QD strongly coupled to cavity. The effciency $\beta$ is defined as fowlloing. With higher beta, the more emission is enhanced at a specific target mode.

$$
\begin{equation}
    \beta = \frac{F_{p}}{F_{p}+1} = \frac{\Gamma_{mode}}{\Gamma_{mode}+\Gamma_{others}}
\end{equation}
$$

However, in practical photonic cavities, it is highly probable that the resonance is slightly offset due to imperfections in growth and processing. Achieving nanometer-scale accuracy for a photon with a specific wavelength becomes an exceedingly challenging task. Although cavities can yield significantly higher Purcell factors compared to methods like waveguides, this advantage comes at a cost. When the enhanced mode of the cavity exhibits a slightly detuned wavelength, emitted photons may become trapped within the cavity instead of being emitted outward. To overcome this obstacle, precise engineering of the cavity is necessary, ensuring that its reflectivity is low enough to allow photon emission while maintaining a sufficiently high quality factor. Several studies have been conducted to solve these issues, such as adjusting the temperature, as the electronic band and refractive index have different dependencies. However, increasing the temperature increases the decoherence associated with photons. Other post-growth tuning mechanisms, such as the application of external magnetic fields or strain, are experimentally more challenging.

## Micropillar cavities

Micropillar cavities are a popular choice for High-Q cavities and are typically fabricated using alternating layers of different refractive indices grown epitaxially. Each layer has a thickness of $\lambda=4n_i$ (where i=1,2) and forms a Bragg mirror with reflectivity controlled by the number of layers. The height of the micropillar is typically around 10 $\mu$m, with a diameter of a few microns. However, there is a trade-off between volume size and quality factor, as smaller cavities have a restricted lateral extension of the guided mode but are also more sensitive to sidewall roughness. The Bragg mirror is grown to allow one side of the cavity to be highly reflective while the other is optimized for photon transmission. High-Q factors can be observed in micropillar resonators up to 250,000, making them ideal for vertical-emitting single-photon sources. While out-of-plane confinement relies on total internal reflection at the membrane-air interface, air holes are drilled in a lattice geometry of semiconductor material, to achieve in-plane confinement by introducing a photonic band gap.  Micropillar cavities with embedded QDs have been shown to generate single photons with high efficiency and an indistinguishability of 90\% was recently reported.

![](/public/img/qd_img/img/cav.png)

## Photonic-crystal cavity

When light is confined in a very small cavity, it consists of numerous plane wave components with wavevectors k of various magnitudes and directions. This makes it difficult to achieve Bragg reflection condition. A better approach is to use structures having a two-dimensional periodic change of refractive index on the scale of the light wavelength, which are known as photonic crystals.

A promising approach is a 2D photonic-crystal slab with a thickness of the order of the light wavelength, as it provides strong optical in-plane confinement. Light is trapped in the plane and can only escape through the vertical direction. The oscillations in the 2D crystal lead to a preferential angle of emission close to the surface of the plane, making it easy to collect the photon. By displacing the holes at each end of the cavity by just a fraction of a lattice constant, the Q factor can be boosted, and the leakage of radiation modes is greatly suppressed.

% The L3 cavity is one of the most successful and important designs obtained from a 2D triangular lattice in a photonic-crystal membrane by leaving out three holes. It has a mode volume of less than $(\frac{\lambda}{n})^{3}$ with a Q factor of $3x10^{4}$. Recently, a modified L3 cavity in silicon at a wavelength of 1.55$\mu$m was experimentally observed to have a cavity Q factor of $2x10^{6}$.

## Waveguides

Waveguides have the advantage over cavities as quantum emitter in the open system can be channelled directly into propagating mode as flying qubit. In contrast, cavity needs localized modes. If the waveguide mode has slow group velocity and a tight confinement of the mode, the photon matter coupling is enhanced. This can be seen from the equation:

$$
\begin{equation}
    F_{p}^{max}(\omega) = (\frac{3}{4n\pi} \frac{\lambda^2/n^2}{V_{eff}/a}) n_g(\omega)
\end{equation}
$$

where n is the group index $\frac{c}{v_g}$ that specifies the slow-down factor of the waveguide. In fabrication, the structural dispersion of the Bloch modes gives rise to slow light and the mode is tightly confined to the diffraction-limited defect area. In plasmonic nanowires, Figure 7, subwavelength confinement combined with the slow propagation of the lowest-order guided mode leads to potentially large Purcell factors.

![](/public/img/qd_img/img/nano.png)

Waveguides rely on spontaneous-emission inhibition in all modes except one, known as mode matching. To collect photons in one direction only, tapered fibre is introduced as conventional waveguides and a metallic mirror spaced by a dielectric layer is placed at the end of nanowires. Another advantage over cavity is that waveguides have higher tolerance of deviation. A range of wavelength can propagate in the plane and the efficiency of photon collection is greater than cavity subjecting to the similar detuning.

$$
\begin{equation}
    \beta(\omega) = \frac{\gamma_{wg}}{\gamma_{wg} +\gamma_{ng} +\gamma_{nrad}}
\end{equation}
$$

where $\gamma_{ng}$ is the loss rate of coupling to all nonguided modes and $\gamma_{nrad}$ is the rate of intrinsic nonradiative recombination in the quantum dot. The near unit beta stems from the fact that the 2D photonic band gap suppresses $\gamma_{ng}$, i.e., the leakage to unwanted modes is strongly inhibited.

However, waveguides like photonic crystal suffer from imperfections as well: the backscattering of the propagating mode into the counter-propagating direction in the waveguide and out-of-plane scattering due to coupling to leaky modes that are above the light line. The former (latter) is characterized by an average length $l_{back}$ $(l_{leak})$ leading to a total extinction length $\frac{1}{l_{ext}} = \frac{1}{l_{back}} + \frac{1}{l_{leak}}$ that determines how the average intensity decays along the waveguide.

# Fabrication
## Growth of semiconductor QD

The progress in quantum nanophotonics over the past few decades has largely relied on a generic nanofabrication platform that combines crystal-growth procedures with semiconductor processing methods, such as electron-beam lithography, etching, and deposition.

In this context, we will provide an overview of two major fabrication methods in quantum dot technology.

## Stranski-Krastanov

Stranski-Krastanov method for InGaAs QD is most extensively studied in QD materials like InAs and InGaAs in GaAs matrices. The huge difference in band-gap energies between InAs (0.422eV) and GaAs (1.522eV) at 4 K and the three-dimensional quantum confinement makes it possible to tune the QD emission in a very large spectral window - from almost 850 nm up to 1400 nm - by adjusting the QD dimensions.

The lattice mismatch between InAs and GaAs creates strain during deposition: The growth of InAs on a GaAs (100) surface initially results in a thin two-dimensional (2D) wetting layer (WL), this is when more than 1.7 monolayers of InAs is deposited on GaAs. Due to the lattice-mismatch, the 2D growth mode turns into a three-dimensional (3D) growth after deposition of a few monolayers, resulting in the creation of randomly positioned QDs with a pyramidal shape (shown in Figure 8 (a)). A capping layer of GaAs is added to prevent oxidation and the intermixing results in a truncated pyramid. As crystal growth proceeds, the accumulated strain energy increases, a transition occurs and the total energy is minimized by creating InAs islands form coherent islands of InGaAs on GaAs surfaces. By stopping the growth right after this transition, the islands are typically 10–30 nm lateral size in the in-plane directions and 2–5 nm out of plane.

![](/public/img/qd_img/img/sk.png)

## Droplet epitaxy
A sometime undesired feature of the SK QDs is the unavoidable presence of the WL at the base of the dots, which generates bidimensional electronic states interconnecting the dots. This affects the QD optical properties and carrier kinetics. The WL is also detrimental in device performances, since it represents a channel for carrier escape out of the QDs. But this can be avoided by droplet epitaxy (DE).

![](/public/img/qd_img/img/DE.png)

Droplet epitaxy is a new technique where gallium droplets saturated with arsenic create large, low-density GaAs quantum dots in AlGaAs without a lattice-mismatch. First group-III atoms are deposited on the surface, then group-V flux is supplied to the surface to crystallize the droplets as in Figure 9. Post-growth annealing with a relatively high temperature is needed to make them optically active, which means the demonstrated quantum efficiency cannot yet compete with Stranski-Krastanov, but this method can grow large QDs in dimension and is strain-free.
% Droplet epitaxy is an emerging growth technique, where droplets of gallium are saturated with arsenic, resulting in relatively large and low-density GaAs quantum dots in AlGaAs. This relies on the affinity of some group-III elements on a semiconductor surface and has the advantage that it does not require a lattice-mismatch between the involved materials. Since the AlGaAs capping layer is often grown at low temperatures, a high-temperature post-growth annealing is required to make them optically active and the demonstrated quantum efficiency cannot yet compete with Stranski-Krastanov quantum dots, but this method can grow large QD in dimension and is strain free.

# Application

The extent to which the results of a quantum hardware can be certified is an open problem, despite the potential power of quantum algorithms. A significant area of research has focused on verifying the quantum advantage over classical computers, and Boson sampling is a useful benchmark for testing different validation methods. Boson sampling involves inputting n Bosons in different modes of an m-mode linear interferometer, sampling events from the distribution of Bosons at the output modes, and testing the obtained calculation. So now we can see the importance of indistinguishable photons, to create interference effects when multiple indistinguishable particles are superposed or overlapped. 

For example, consider N single photon Fock state:

$$
\begin{equation}
    \ket{\psi} = \ket{m_1, m_2,...,m_N}
\end{equation}
$$

composed of $\sum_{n=i}^{\infty} m_i$ photons, incident on an N-mode linear interferometer. Therefore, the probability of detecting $n_j$ photons at the jth output mode is given by:

$$
\begin{equation}
    \bra{n_1, n_2,...,n_N} U \ket{\psi} = \frac{|Per(U_{st})|^2}{m_1!m_2!...m_N!n_1!n_2!...n_N!}
\end{equation}
$$

where the left hand side is the sampled single photon probability distribution and the right is the permanent of a submatrix of the interferometer unitary, dependent upon the input and output Fock states.

The calculation of permanent, which belongs to the computational complexity class of \#P-Hard problems, implies that this is an exponentially hard task for classical computers.

Boson sampling has been experimentally demonstrated with three photons, and scalability in imperfect conditions, such as partial distinguishability has been investigated. Scattershot Boson Sampling (SBS) is an improved method, which uses spontaneous parametric down-conversion (SPDC) to reduce the experimental difficulty of emitting multiple photons by inputting a set of coherent random input photon state. This is a nonlinear process that using a pulsed pump laser with a high repetition rate to generates a separate set of entangled photon pairs and then feed them into an interferometer. The scattershot technique allows for the injection of multiple photons into the interferometer simultaneously as in Figure 10 right, resulting in more efficient sampling. Inside the interferometer, the signal photons interfere with each other, generating complex interference patterns. The output of the interferometer is then measured using photon detectors placed at the output ports, which provide information about the correlations between the input photons.

![](/public/img/qd_img/boson.png)

# Conclusion

IQP has made significant progress in developing single photon sources, crucial for quantum photonic applications. Elshaari proposed seven fundamental components for a quantum photonic circuit, including for example, quantum memories for information storage. However, no single material system can perform all necessary tasks. Thus, hybrid integrated quantum circuits are necessary. While this may seem impractical, recent advances in semiconductor IQP devices demonstrate the feasibility of hybrid integration, with QD as single photon source. Additionally, photonic-based Boson sampling highlights the potential of quantum technologies to achieve quantum supremacy and solve computationally challenging problems paving the way for practical quantum information processing. 

Download the full version [here]({{ site.url }}/public/assets/Integrated_Quantum_Photonics_with_Semiconductor_Single_Photon_Sources.pdf)

Besides the review, I have worked with Dr.Christian Schimpf on optimizing the wavelength fitting of cavity diode with DBR implemented. First I tried to fit the Poisson solution with the data we have:

At 50K:

![](../public/img/50_1.png)
![](../public/img/50_2.png)

At room temperature:

![](../public/img/300_1.png)
![](../public/img/300_2.png)

The doping currently only affects our electronic properties (the function of the diode), as we do not (yet) consider light absorption in our structure. So the general rule of thumb will be that there should be a node of the light electric field in the doped layer AND the doping regions should be as small as possible, but as large as necessary, in order to minimize absorption in the real structure.

The structure of the diode is shown below:

![](../public/img/layer.png)

and the fitting waves:

![](../public/img/mirror.png)