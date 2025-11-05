---
layout: default
title: Physics
# (Just the Docs extra, if you want sidebar ordering)
nav_order: 1
parent: External Revision
---


# Standard Model for Dummies

The standard model is the best current theory describing the fundamental building blocks of matter and three of the four known fundamental forces: the strong force, the weak force, and electromagnetism. It classifies all known elementary particles into matter particles (quarks and leptons) and force carrier particles (bosons). Gravity is not included in this model. 

## Matter Particles

Matter consists of elementary fermions, divided into quarks and leptons: 
- 6 Types of Quarks: up, down, charm, strange, top, bottom
	- They combine to form hadrons:
		- Baryons are composed of 3 quarks, (e.g. protons and neutrons)
		- Mesons are composed of quark + antiquark

- 6 Types of Leptons: electron, muon, tau, and their associated neutrinos (electron neutrino, muon neutrino, tau neutrino)
	- Unlike quarks, leptons do not experience the strong force

Each of these particles has a corresponding antiparticle with opposite charge.

Quarks, including baryons and mesons, experience the strong force, the weak force, and the electromagnetic force.

Leptons, experience the weak and electromagnetic forces.

## Force Carrying Bosons

The exchange of bosons mediates the forces between particles:
- Photon mediates the electromagnetic force
- Gluons mediate the strong nuclear force, binding quarks together
- W$^\pm$ and Z bosons mediate the weak nuclear force, enabling processes like beta decay
- Higgs boson gives particles mass through interaction with the Higgs field, but it is not a force mediator

The W$^\pm$ bosons have either a positive or negative electric charge of 1 elementary charge and are each other's antiparticles. The Z$^0$ boson is electrically neutral and is its own antiparticle. 

The photon is also its own antiparticle.

The summary of the standard model is shown here:
![Alt text]({{ '/assets/images/Pasted image 20250830114517.png' | relative_url }})

## Quick summary:

- All particles with electric charge experience force due to the electromagnetic interaction.
- Quarks and leptons have flavour and experience the weak interaction
- The neutrinos have no electrical charge
- The gauge bosons that act as the mediating particles are gluons for the quarks, W$^+$, W$^-$, and Z for the weak force, and photons for the electromagnetic force. 

# Feynman Diagrams

A Feynman diagram is a graphical way of representing particle interactions. It shows hows particles move through space (vertical axis) and time (horizontal axis) and how they exchange force carrying particles. 

## Conventions for drawing:
1. Axis
	- Time runs left to right
	- Space runs up and down
2. Particles
	- Drawn as straight lines with arrows pointing forward in time
3. Antiparticles
	- Shown as arrows pointing backwards in time
4. Gauge bosons
	- Photons ($\gamma$) as wiggly lines  
	 - Z and W bosons as wiggly lines
	 - Gluons as a curly loop (not assessable)
5. Vertices (interaction points)
	- A vertex is where lines meet (particles interact)
	- Each vertex always has 3 lines:
		- 1 boson (wiggly line)
		- 2 fermions (straight arrows, one in, one out)


## Conservation Laws

Every diagram must obey conservation of:
- Charge (total electric charge stays constant)
- Lepton number (e.g., electrons & neutrinos)
- Baryon number (protons, neutrons, etc.)

## Common examples (The exam WILL have ONE of these)

### Electron-electron scattering (Møller scattering)
Two electrons repel, exchanging a photon. Diagram: two straight lines (e⁻, e⁻) with a photon line (γ) between them.

The diagram will look like this:
![Alt text]({{ '/assets/images/Pasted image 20250830130802.png' | relative_url }})

### Electron-positron annihilation
An electron and a positron meet, annihilate, and produce photons. Diagram: e⁻ and e⁺ lines meet at a vertex, with photons emitted.

The diagram will look like this:
![Alt text]({{ '/assets/images/Pasted image 20250830130932.png' | relative_url }})

### Beta decay (neutron → proton)
A down quark changes into an up quark by emitting a W$^-$ boson, which then decays into an electron and an antineutrino. Diagram: d → u + W⁻, followed by W⁻ → e⁻ + ν̄ₑ.

The diagram will look like this:
![Alt text]({{ '/assets/images/Pasted image 20250830131007.png' | relative_url }})



# Atomic Spectra
![Alt text]({{ '/assets/images/Pasted image 20250831104835.png' | relative_url }})
Above is an energy level/atomic spectra diagram for hydrogen.

The equations relevant to this topic:
$\Delta E=hf$
$c=\lambda f$
$f=\frac{c}{\lambda}$

Where $c$ is the speed of light $3\times10^{8}\;\mathrm{m/s}$

This equation will be on the exam (not on formula book):
$\Delta E=\frac{hc}{\lambda}$

**Absorption Spectrum** indicates moving from a low energy state to a higher energy state
**Emission Spectrum** indicates moving from a high energy state to a lower energy state

## Some other stuff

$E_k=hf-W$
If asked to find the work function, $E_k=Vq$ and then substitute in:

$Vq=\frac{hc}{\lambda}-W$
Solve for W, the answer will be in electron-volts (eV).

# Photoelectric Effect

The Photoelectric effect is the emission of electrons (or other free carriers) when light shines on a material.

Threshold frequency is the minimum frequency of a photon required to eject a photoelectron from the surface of a metal. 

Photons with frequencies equal to or greater than the threshold frequency will eject photoelectrons from the surface of the metal, while photons with a lower frequency will scatter off the metal’s surface.

From the textbook:
## Experiment 1: Varying the frequency
Lenard shone light on the metal in the cathode ray tube and varied the frequency. Nothing
happened until the frequency was in the ultraviolet region, then a current started to flow. The
UV light had caused electrons to be ejected from the metal and pass through the vacuum to
the anode. He called this the threshold frequency, $f_0$. As he increased the frequency past
this minimum, the electrons became faster and faster with more and more kinetic energy.
Lenard then repeated the experiment with increased intensity (brightness). Again, nothing
happened until he reached the threshold frequency. However, once the threshold was reached,
the more intense the light the bigger the current. He then tried different metals and found
different threshold frequencies for each. 

This is a summary of his findings:<br>
• Electrons were ejected from the metal only if the frequency of the incident light exceeded
a minimum value called the threshold frequency, $f_0$<br>
• The threshold frequency was different for various metals.<br>
• If the frequency was below the threshold value, electrons were not ejected and there was
no flow of photocurrent, not even when very intense light was used.<br>
• Once a photocurrent is registered, increasing the incident light intensity increased the
amount of photocurrent flowing.<br>
• Light of a frequency higher than the threshold increased the kinetic energy of the ejected
electrons.<br>

## Experiment 2: Varying the voltage
Lenard then experimented with the voltage. He left the light shining on the tube at a
frequency greater than threshold so that a current was flowing. When he increased the
voltage, V, the current didn’t change. He reversed the battery and made the anode negative
with respect to the cathode. Thus, the voltage was now negative. This was causing the
cathode to repel the ejected electrons. 

Lenard kept increasing the voltage in the negative
direction and noticed that the current decreased. At a certain voltage the current reached
zero. The reverse voltage was now large enough to stop the photocurrent completely. He
called this the stopping potential, also known as the reverse cut-off voltage, Vc
form: V = −Vc. This behaviour is shown in Figure 4a.

$E_k=hf-W$ <br>
$E_k=hf-hf_0$<br>
$E_k=qV_c$<br>
$\frac{1}{2}mv^2=hf-hf_0$<br>
$\frac{1}{2}mv^2=qV_c$<br>

# Faraday’s Law & Lenz’s Law

Lenz’s law is one expression of a fundamental law of nature: the law of conservation of energy. Lenz’s law states that the direction of an induced electric current is such that it produces a current whose magnetic field opposes the change in the circuit or in the magnetic field that produces it.

Faraday’s law states that the induced electromotive force (emf) in a circuit is equal to the negative rate of change of magnetic flux through the circuit.

$$\mathrm{emf}=-n\frac{\Delta \phi}{\Delta t}$$  &nbsp;  $$\mathrm{emf}=-\frac{n\Delta(BA_\perp)}{\Delta t}$$
- $n$ = number of turns in the coil
- $B$ = magnetic field strength (tesla)
- $A_\perp$= perpendicular area to the field (m²)
- $\Delta (BA_\perp)$ = change in magnetic flux
- $\Delta t$ = time interval
- $\phi$ = single-turn magnetic flux
- The minus sign is **Lenz’s law** (emf opposes the change)

## Transformer Equations

$$I_pV_p=I_sV_s$$  &nbsp;   $$\frac{V_p}{V_s}=\frac{n_p}{n_s}$$

Where $V_p$ and $V_s$ are primary/secondary voltages, and $n_p$ and $n_s$ are number of turns.

# Coulomb’s Law

$$F=\frac{1}{4\pi\epsilon_0}\frac{Qq}{r^2}$$ <br>
Where $\frac{1}{4\pi\epsilon_0}$ is Coulomb’s constant (value in the formula booklet). The questions on this topic will be mostly calculating something using this formula or another one from the formula sheet.
# Special Relativity

Moving clocks run slow. 

$$t=\frac{t_0}{\sqrt{1-\frac{v^2}{c^2}}}$$ <br>
Where $t$ is the time measured by the stationary observer in their own reference frame, and $t_0$ is the proper time, which is the time measured by the observer moving with the clock or event.


# Black bodies

**Key idea**
A blackbody is a body that absorbs 100% of all electromagnetic radiation AND emits 100% of all electromagnetic radiation.

$W=NkT$   &nbsp; $N = \text{number of particles}$   &nbsp; $kT = \text{on average energy}$ <br>
Some particles have much higher energy than others

## Planck
In order to obtain agreement with the experimental curves, Planck assumed that each atomic oscillator could only have have discrete values of energy (E). 

i.e. $E=0$, &nbsp; $E=hf$ &nbsp; $E=2hf$  &nbsp; $E=3hf$ <br>
$E=nhf$

Conservation of energy requires tht the energy carried off by the radiated EM waves = energy lost by the atomic oscillator. There are not many particles with high frequencies (or low wavelengths) and each particle has a discret amount of energy. The radiation curve decreases for $\lambda > \lambda_{\text{max}}$.

$E=\frac{8\pi hc}{\lambda^{5}\times}\frac{1}{}$    (SECTION INCOMPLETE)
## Rayleigh-Jeans Law

$I=\frac{2ckT}{\lambda^4}$

Bohr model only applies when ONE electron orbits the nucleus.


# Symmetries
## Parity - Mirror image copy
Left handed neutrino gets turned into right handed neutrino
Right handed neutrinos don't exist

## Charge symmetry
Neutrino becomes anti neutrino.
Left handed anti neutrinos don't exist

The universe holds under symmetry apart from neutrinos. If you apply both parity and charge then the neutrinos fix themselves again.


# Formulae

$v=u+at$
$s=u+\frac{1}{2}at^2$
$v^2=u^2+2as$
$F=ma$
$v=\frac{2\pi r}{T}$
$a_c=\frac{v^2}{r}$
$F_{net}=\frac{mv^2}{r}$
$F_g=\frac{GMm}{r}$
$g=\frac{F}{m}=\frac{GM}{r}$
$\frac{T^2}{r^3}=\frac{4\pi^2}{GM}$ 
$F=\frac{1}{4\pi\epsilon_0}\frac{Qq}{r^2}$
$E=\frac{F}{Q}=\frac{1}{4\pi\epsilon_0}\frac{q}{r^2}$
$V=\frac{\Delta U}{q}$
$B=\frac{\mu}{2\pi}\times\frac{I}{r}$
$B=\mu n I$
$F=BIL\sin\theta$
$F=qvB\sin\theta$



# Textbook Chapter Completion

## Chapter 0
- [x] 0.1 ✅ 2025-09-18
- [x] 0.2 ✅ 2025-09-18
- [x] 03 ✅ 2025-09-18
- [x] 0.4 ✅ 2025-09-18
- [x] 0.5 ✅ 2025-09-18
- [x] 0.6 ✅ 2025-09-18
- [x] 0.7 ✅ 2025-09-18
- [ ] Chapter 0 Review

## Chapter 1
- [x] 1.1 ✅ 2025-09-18
- [x] 1.2 ✅ 2025-09-18
- [ ] 1.3
- [ ] Chapter 1 Review

## Chapter 2
- [ ] 2.1
- [ ] 2.2
- [ ] 2.3
- [ ] Chapter 2 Review

## Chapter 3
- [ ] 3.1
- [ ] 3.2
- [ ] 3.3
- [ ] Chapter 3 Review

## Chapter 4
- [ ] 4.1
- [ ] 4.2
- [ ] 4.3
- [ ] Chapter 4 Review

## Chapter 5
- [ ] 5.1
- [ ] 5.2
- [ ] 5.3
- [ ] Chapter 5 Review

## Chapter 6
- [x] 6.1 ✅ 2025-09-23
- [x] 6.2 ✅ 2025-09-23
- [x] 6.3 ✅ 2025-09-23
- [ ] Chapter 6 Review

## Chapter 7
- [x] 7.1 ✅ 2025-10-7
- [ ] 7.2
- [ ] 7.3
- [ ] 7.4
- [ ] 7.5
- [ ] Chapter 7 Review

## Chapter 8
- [ ] 8.1
- [ ] 8.2
- [ ] 8.3
- [ ] 8.4
- [ ] 8.5
- [ ] 8.6
- [ ] Chapter 8 Review
 
## Chapter 9
- [ ] 9.1
- [ ] 9.2
- [ ] 9.3
- [ ] 9.4
- [ ] Chapter 9 Review

## Chapter 10
- [ ] 10.1
- [ ] 10.2
- [ ] 10.3
- [ ] 10.4
- [ ] 10.5
- [ ] Chapter 10 Review

## Chapter 11
- [ ] 11.1
- [ ] 11.2
- [ ] 11.3
- [ ] 11.4
- [ ] 11.5
- [ ] 11.6
- [ ] Chapter 11 Review

## Chapter 12
- [ ] 12.1
- [ ] 12.2
- [ ] 12.3
- [ ] Chapter 12 Review

## Chapter 13
- [ ] 13.1
- [ ] 13.2
- [ ] 13.3
- [ ] Chapter 13 Review

## Chapter 14
- [ ] 14.1
- [ ] 14.2
- [ ] 14.3
- [ ] 14.4
- [ ] Chapter 14 Review


## Practice Exams
- [ ] 2024 External
- [ ] 2023 External
- [ ] 2022 External
- [ ] 2021 External
