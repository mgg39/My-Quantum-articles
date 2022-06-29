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

###GKP qubits & Squeezed vacuum states
