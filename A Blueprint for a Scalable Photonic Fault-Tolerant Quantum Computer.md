# A Blueprint for a Scalable Photonic Fault-Tolerant Quantum Computer - Schrödinger's Papers #1
## What could future photonic quantum computers look like?
![image](https://user-images.githubusercontent.com/73605937/176425521-1c6169f4-1aa5-4e04-90f7-a8730772603c.png)

### Welcome!
Welcome to Schrödinger's Papers #1 Issue! Through this project, I hope to help communicate the research behind existing quantum technology papers and thus help promote a scientifically oriented and accurate understanding of quantum technologies for all audiences. As a student in the Quantum field, I come through dozens of papers every week and have acquired the ability to extract the main arguments and points from such publications. Hopefully, this skill will shine through these issues and help others acquire the ability to understand deeply technical publications and apply their conclusions to practical and proof-oriented investments, research, and actions within their organizations or studies.
Before we start I would like to have two short disclaimers:
1.	I will always try my best to express the author(s)’s main arguments and logic with accuracy, nevertheless, due to the nature of certain papers and my background, I might sometimes misinterpret or paraphrase the contents of a paper, which might have specific consequences on it’s presented arguments. I will do my best to avoid these instances, but if they were ever to happen, please feel free to reach out to me as I will be happy to revise my content.
2.	I will always attach a link to discussed papers at the end of these issues, so you can always directly read the original publication and draw your own conclusions.
Now let’s begin! 

### The paper’s background
![image](https://user-images.githubusercontent.com/73605937/176425630-06b89b74-ca6f-4d3f-a7da-4fe9d4981b1c.png)
#### Authors
The “Blueprint for a Scalable Photonic Fault-Tolerant Quantum Computer” was a collaboration between no less than 8 major institutions:

    Xanadu

    The Department of Physics at the University of Toronto

    The Center for Quantum Information and Control at the University of New Mexico

    The Centre for Quantum Computation and Communication Technology at RMIT University’s School of Science

    The Perimeter Institute for Theoretical Physics

    The Institute for Quantum Computing at the University of Waterloo

    The College of Optical Sciences at the University of Arizona

    The Department of Applied Physics at the University of Tokyo

with 13 authors:

    J. Eli Bourassa: Quantum Computing Researcher, Xanadu

    Rafael N. Alexander: Vice-Chancellor's Postdoctoral Fellow, RMIT University

    Michael Vasmer: Perimeter Institute for Theoretical Physics & Institute for Quantum Computing

    Ashlesha Patil: Graduate student, The University of Arizona

    Ilan Tzitrin: Quantum Computing Researcher, Xanadu

    Takaya Matsuura: Graduate student, The University of Tokyo

    Daiqin Su: Quantum Computing Researcher, Xanadu

    Ben Q. Baragiola: Assistant Professor, at the Yukawa Institute for Theoretical Physics, Kyoto University

    Saikat Guha: Professor of Optical Sciences at The University of Arizona, and Director of the Center for Quantum Networks

    Guillaume Dauphinais: Quantum Computing Researcher, Xanadu

    Krishna K. Sabapathy: Quantum Computing Researcher, Xanadu

    Nicolas C. Menicucci: Associate Professor, RMIT University

    and Ish Dhand: current photonics quantum computing researcher at the University of Ulm, ex-head of Xanadu’s Architecture team

With collaborators ranging from industry to research, this paper gives an overview of how photonic quantum computers might be designed so they are scalable and functional for both companies and researchers.
![image](https://user-images.githubusercontent.com/73605937/176425707-ea8526ab-504b-44a0-85a6-aae349b28fff.png)

#### Publication date
This paper was published on the 2nd of February 2021, almost a year and a half before this article. Making it a relatively recent publication, that is still relevant to existing active investigation and standards.

## An overview of the paper

### Why photonics?
![image](https://user-images.githubusercontent.com/73605937/176425940-bf17fff8-925a-46e5-bc7b-9fad5118e3da.png)
Due to the existing spectrum of available photonics-based technologies, ranging from chips to network architectures, as well as the lack of need for refrigeration within some photonic quantum computer designs; photonics is a very attractive platform to build scalable quantum computers.

In this paper, the authors propose a scalable fault-tolerant quantum computer design that holds the advantages of a photonic platform, which include:

    State of light encoded qubits, that allow for less faulty and fast operations, through various error-correcting codes that utilize the temporal degrees of freedom of light.

    The existence of photonic tools that allow for an easy-to-network architecture. If we build a photonic computer, it will be intrinsically compatible -to a certain extent- with existing communication technology, as this technology is currently based on photonic hardware components. This inter-operability will enable high-fidelity connections through various platforms, therefore allowing for easy connectivity to the computer through external networks.

    Room temperature computation, opens the door to scalable fabrication and operation, as there is no need for the computer’s physical environment to be refrigerated and monitored. This allows for full miniaturization and mass manufacturing of cheap components, as well as the implementation of the computer chips into numerous existing photonic technologies available in the market, therefore allowing for rapid scalability of the architecture.
    
![image](https://user-images.githubusercontent.com/73605937/176426124-c21c328b-07ba-49de-ac22-a1aa0ebbf217.png)

### Previously proposed architectures vs the author’s proposal
At the time of publication, there were two major types of architectures proposed by academia for scalable and universal photonic quantum computing:

The first uses continuous-variable (CV) entangled resource states to implement computation on discrete-variable (DV) information.

For our non-technical audience, DVs (discrete variables) define an element, such as a qubit, that can be easily measured and defined within a certain capacity (it is defined within a measurable Hilbert space), CVs (continuous variables) on the contrary have a continuum of measurement outcomes (an infinite Hilbert space). A good way of thinking about this is to compare an apple (DV) to the concept of an apple (CV). When we think of an apple, the DV, the object, we always think of 1 fruit, but when we think of an apple, the CV, the concept, it is not a question of units, but rather of its properties.

These architectures require DV resources to be generated deterministically on-demand, meaning they require a continuous emission of equivalent photons, instead of 1 photon for the architecture to work. This requirement is very difficult to perform due to its hardware implications and seems to lead to a dead-end when we consider building these computers, according to the authors at the date of publication.

The second type of architecture involves generating entangled resource states made entirely out of bosonic qubits.

Traditional qubits are encoded in discrete two-level systems. Instead, bosonic qubits encode quantum information in complex multi-photon states of harmonic oscillators. In essence, they offer a different information storage format for basic units of quantum information (qubits). This happens to make bosonic qubits more resilient to quantum noise and decoherence, which are some of the major challenges in the development of modern quantum computers.

Although high-quality bosonic qubits allow a degree of resilience to noise, they are extremely difficult to make, making these architectures difficult to produce at scale.

![image](https://user-images.githubusercontent.com/73605937/176426227-9c32a958-8e48-4bd7-bc5b-94dc1ef218d4.png)

To account for the benefits and drawbacks of both architectures, the authors propose using CV resources to ease the burden of the preparation of bosonic qubits, whilst retaining bosonic qubit’s low-noise properties by consuming CV modes. Thus allowing for a low-noise scalable architecture. Through the paper they analyze how robustness to error depends on the concentration of bosonic qubits in the entangled state.

### GKP qubits & Squeezed vacuum states
The bosonic qubits considered in this paper were originally introduced by Gottesman, Kitaev, and Preskill, and hold the name GKP. This type of bosonic qubits was considered for 2 main reasons:
(i) An important class of computational operations and measurements on these states can be performed with Gaussian resources, which are widely available and easy to implement on photonic devices.

(ii) They are inherently robust to noise and optical losses. Whilst being available at room temperature, which makes them especially attractive for the scalable fabrication and operation of quantum computers.

Current proposals for quantum computation with optical GKP qubits rely on CV cluster states, which are entangled states of many modes of light. Measurements of CV cluster states can be used to perform Gaussian operations, but the ability to perform non-Gaussian operations is required for a fully-fledged, universal computer. Therefore CV cluster states need a counterpart component that allows for non Gaussian operations. This role is fulfilled by the GKP qubits, which allow for these.

The same issue occurs at a different layer, the optical properties of integrated photonic platforms are insufficient to provide non-Gaussian resources, but recent technological developments in photon-counting detectors can save the day at this layer.

### What happens to failed qubits?
Qubits can “fail” for various reasons: they might be lost as a consequence of quantum noise within the hardware layer, they might not have been correctly created at the output level, they might have experienced a change in their state whilst in transit, … Bits also experience these errors, but they are much easier to solve. Due to the extravagant nature of qubits, error correction within quantum systems is one of the biggest and most problematic challenges the quantum community must solve for quantum computers to become a reality. 
![image](https://user-images.githubusercontent.com/73605937/176426471-69caa2a7-5f3b-44ec-841f-c8c1dde6bc44.png)
In this work, the authors propose an architecture for measurement-based quantum computing that takes into consideration the advantages of CV-based schemes and is compatible with probabilistic GKP qubit sources. They do this by considering a hybrid CV cluster state where each mode is substituted with a GKP qubit at random.

Their approach allows them not to lose “failed” qubits, by replacing them with squeezed vacuum states. Quantum information is encoded in a qubit’s state, in this model this would correspond to GKP qubit’s state. Squeezed vacuum states, similarly to GKP states, can still encode logical information. They do not do it as efficiently and error-free as GKP states, but they present 3 advantages:

    They are Gaussian resources.

    They are easy to produce.

    They allow the model not to “lose” too many “failed” qubits and therefore enhance its fault tolerance. 

This approach makes this model more advanced than existing quantum fault tolerance methods.

### Fault-Tolerant Universal Quantum Computation
A key feature of this architecture is that it promises full scalability to a large number of qubits, which is required for fault tolerance.

Existing schemes of CV computation that use large numbers of qubits come paired with exponentially growing losses, which caps the number of qubits within quantum computers, as beyond a certain point the losses outweigh the computational power presented by the machine.

The authors address this issue by proposing a 2D chip design, that would simplify the computer’s interactions by reducing the space in which qubit’s are defined and therefore the consequences of their interactions. This would allow to minimize its losses, whilst making the architecture easier to fabricate, and therefore enhancing it’s scalability. 

![image](https://user-images.githubusercontent.com/73605937/176426597-6fd9d46a-770d-409c-bdbd-6d177fcde9b8.png)

In addition to this simplified design, the proposed architecture does not contain any particularly harsh requirements on its experimental components, it does not require any “fancy” quantum photonic parts (at least beyond quantum photonic hardware standards). Which, once again, allows for its scalability.

## Open Problems
The points made above regarding error correction, fault tolerance, chip architecture, and states are described in rigorous detail throughout the paper. This issue simply tries to highlight some of the basic concepts behind the proposed architecture, so less technical audiences might get a better insight into the technical properties that make this proposal different from previous or future quantum computer architecture designs.

Nevertheless, the authors still point towards existing open problems that could provide additional advantages to the proposed architecture over other architectures and platforms.
![image](https://user-images.githubusercontent.com/73605937/176426710-0c7897b4-d090-4d50-ab78-eab85f1a5727.png)

They divide these problems into three main categories: hardware-focused improvements to the architecture, better encoding, and better decoding strategies. I will briefly describe some of the open problems prevalent in these categories.

###Hardware-focused improvements to the architecture
    Devising a passive implementation of the hybrid architecture would allow for active and passive transformations of states. This could further simplify the computational module and thus reduce the experimental requirements.

    Reliable state preparation, particularly for high-quality GKP qubits would cause better fault-tolerant computation; but their development would come with an additional problem:

        High-quality GKP qubits would require the development of new numerical simulation techniques, as they would be too “big” to process with current techniques.

    Developing a more realistic Gaussian noise model for state preparation is also a current open problem that could improve the proposed architecture.
### Better encoding
    Future encodings could potentially provide the advantages offered by GKP qubits and overcome their shortcomings. Therefore their development can be considered an open problem.

    Exploring the viability of employing other hybrid resource states comprised of different types of bosonic encoded qubits, would also be a beneficial path of research for similar reasons.
### Better decoding strategies
    Although the presented decoder exploits the structure of the CV, there is still more information that could in principle be exploited, at other levels of the design, for example, at the level of the outer decoder.

    Better decoding strategies could also allow for a higher swap-out threshold of for the architecture. Making the swap-out threshold much higher than the era-
    sure threshold.

    Faster decoders would additionally increase the computer’s computational speed.
    
## Summary and Technological Advantages
The authors propose a scalable and concrete architecture for future photonic quantum computers. Their architecture synthesizes modern techniques in scalable entanglement resource state generation and bosonic codes, whilst proposing a novel error structure based on bosonic qubit sources. This model provides several advantages against its counterparts, which include, but are not limited to:

    a simplistic modular computational module,

    minimum temperature requirements,

    and a fast computational speed, that is a consequence of efficient use of it’s quantum resources.

Making this a state-of-the-art proposal for a photonic architecture, with current available theoretical and experimental knowledge. 

## Author’s notes & thank you
Thank you for reading the first issue of Schrödinger's Papers!

I am quite new to sub-stack and summarizing academic publications, therefore I would love to hear your feedback and thoughts on how I can improve future issues and paper summaries.

I am best to reach via LinkedIn .

## Arxiv reference
[Arxiv reference](https://arxiv.org/abs/2010.02905)
