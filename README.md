# Welcome to Q^3 Qompute 2025!
All Challenges are provided by IBM Quantum and to be completed with Qiskit. 

> [!IMPORTANT]
**Please note that in-person attendees must check in on 9/12 and 9/14, contact qee@usc.edu for any concerns**

- [Overview](#overview)
- [How to Start Qomputing](#how-to-start-qomputing)
- [Final Submission Due Date](#final-submission)
- [Juding Criteria](#judging-criteria)
- [Submission Details and Challenges](#submission-details-and-challenges)
- [Winners](#🏆_winners_🏆)
------

## **Overview**

There are multiple challenge tracks, but it is up to you and your teammates to work on one or multiples to present a project in alignment with the judging criteria.

The convergence of quantum science and global sustainability efforts is unlocking a new horizon of possibility. Quantum computing provides a transformative toolkit to achieve the ambitious vision of the UN's Sustainable Development Goals, offering powerful new approaches to problems in simulation, optimization, and foundational computation itself. [1]

This Q3 USC hackathon, supported by IBM, is structured as a direct inquiry into quantum's potential, presenting a series of challenges across critical domains:
- Reversible computing: Probing the principles of reversible computing to address the fundamental energy cost of information processing
- Complex optimization problem: Untangling intractable logistical and energy-grid puzzles
- Natural Simulations: Modeling the very building blocks of nature to accelerate the discovery of new medicines and materials.

Your goal is to engage with one of these core challenges. Beyond simply implementing an algorithm, you are challenged to consider the deeper questions of real-world application and the broader social context of your work.

## **How to Start Qomputing**

Please visit [IBM Setup Guide](https://docs.google.com/document/d/12Be_4zIUcz8xkC1jnlbSwCfLch4eiJhVqtn0Syusv70/edit?usp=sharing) for an overview of installing Qiskit, accessing the online environment, and using the backend computing tools.

### Access to IBM Hardware
Whether you will work locally or in a cloud environment, the first step for all users is to install Qiskit. Please visit [IBM Qiskit install guide](https://quantum.cloud.ibm.com/docs/en/guides/install-qiskit) to learn about how to install Qiskit and set up the Python environment.

Also, you can visit this YouTube videos: [How to Install Qiskit | Coding with Qiskit 1.x | Programming on Quantum Computers](https://youtu.be/dZWz4Gs_BuI?si=um36GxYPqrcAaZC_)


### Using an Online Environment
To ensure an easy and consistent experience for all participants—especially those on Windows — we can try [qBraid](https://www.qbraid.com/), one of the supported online environments, to provide a pre-configured, ready-to-use environment to use Qiskit. You can follow these steps to launch the lab notebooks on qBraid.

You can find [detailed instructions](https://docs.qbraid.com/lab/user-guide/getting-started) on qBraid.

📎 Learn more and get started here: [IBM Quantum Online Lab Environments Guide](https://quantum.cloud.ibm.com/docs/en/guides/online-lab-environments)

## Final Submission Due Date

> [!IMPORTANT]
Submission Due: 11:59AM PST, 13th Sep (Saturday)</br>
Link will expires after due.

## Judging Criteria

1. **Technical Content - 30%** : 
2. **Societal Impacts - 20%** : How does the challenge support [Quantum for Good](https://aiforgood.itu.int/quantum-for-good/) by the UN? (Prompt motivation)
  - Did you consider the potential harm or danger of this technology?
  - Does your project have a clearn and positive impact? 
3. **Presentation - 20%** : Comprehension, aesthetics, and delivery style. Clear communication is crucial in innovative fields of emerging tech, a good idea that cannot be shared cannot make an impact.
4. **Originality - 15%** : Creativity and problem solving (applications to real world problems). Is the project and solution well researched?
5. **Submitting correct and clean files and attendance/communication - 5%** :
  - Easy to follow and clean formatting on GitHub
  - Sources and references are included
  - *For in-person attendees only* You are responsible for your attendance, if someone from your team cannot come they should communicate with the organizers AND teammates


## **Submission Details and Challenges**

The final submission for this hackathon is a 5-10 minute presentation in any chosen format and your GitHub Repository. Please fill out [this google form](https://forms.gle/PBY8KsTmg4SdrbaeA) to upload all necessary information and documents. Only ONE team member has to submit, please do not duplicate submissions!

## Track 1: Feynman's dream - Reversible computing

This track is your conceptual entry point into the quantum world, starting with a foundational question that puzzled the pioneers of computing: Can we compute reversibly?

### Reversible computing

In classical computers, most logic gates are `irreversible`. For example, and AND gate outputs `0` for three different inputs (`00`, `01`, `10`). If you only have the output, you can't know the input - information has been lost. According to Landauer's Principles, this act of erasing information fundamentally s energy dissipation, making computation inherently inefficient. A **reversible computation**, in contrast, is one where you can always reverse the process to find the original input from the output, meaning no information is lost. [2]

The idea of reversible computing was advanced significantly by Charles Bennett, who showed that any classical computation could be performed in a logically reversible manner. Building on this, Richard Feynman noted that the laws of quantum mechanics are themselves inherently reversible and thus proposed that a computer built on quantum principles could be the ideal physical implementation of a reversible computer.[3] [4]

### Your Challenge

Your challenge is to explore Feynman's vision. Using Qiskit, design and demonstrate a non-trivial computation that is fully reversible. Take a simple classical process that is normally irreversible, like the `AND` operation previously mentioned, and show how it can be constructed using only reversible quantum gates. Your goal is not only to build a working circuit but also to understand and explain why your quantum implementation is fundamentally reversible. Plus point if you run your circuit at the real QPU and analyze it.

### Start from here
- The Reversible Quantum Calculator: Could you build a circuit that performs binary addition where the original input number can be fully recovered from the output state?
- The Quantum Game: Could you design a simple game where every move is reversible? This can be a `rock-paper-scissor`, `tic-tac-toe` or a `guessing game`.
- Reversible Data Processing: Could you design a circuit that checks if a binary string is a palindrome (`1001`) without erasing any of the intermediate steps?


[1] World Economic Forum. 2024. Quantum for Society: Meeting the Ambition of the SDGs. Geneva, Switzerland: World Economic Forum.

[2] Landauer, Rolf. 1961. “Irreversibility and Heat Generation in the Computing Process.” IBM Journal of Research and Development 5 (3): 183–91.

[3] Feynman, Richard P. 1982. “Simulating Physics with Computers.” International Journal of Theoretical Physics 21 (6/7): 467–88.

[4] Bennett, Charles H. 1973. “Logical Reversibility of Computation.” IBM Journal of Research and Development 17 (6): 525–32.

## Track 2: Quantum Optimization for Impact

This track is for participants ready to explore one of the most promising near-term applications of quantum computers: solving complex optimization problems.

### Quantum for Optimization Problem

Many real-world problems—from logistics and finance to drug development—are fundamentally optimization problems. The challenge is that as the number of variables increases, the number of possible solutions can grow exponentially, becoming too vast for even the most powerful supercomputers to search exhaustively. This is where quantum computers offer a new approach. By leveraging principles like superposition and interference, a quantum algorithm can explore a huge number of potential solutions simultaneously, finding high-quality approximate solutions to problems that are otherwise intractable.


### Your Challenge: Solve Real-World Optimization Problem

A single quantum algorithm, like the `Quantum Approximate Optimization Algorithm (QAOA)`, can be adapted to solve a wide range of problems [1], [2], [3]. Your challenge is to choose one of the following classic optimization problems, frame it as a real-world issue, and use Qiskit to find an approximate solution.

### Start from here:

- The Traveling Salesperson (TSP) - Efficient Logistics: This challenge addresses Climate Action by minimizing fuel consumption and carbon emissions in transportation and logistics. Try to model a scenario where a vehicle must find the most efficient route to visit a small number of cities (e.g., 3-4) and return home.

- The Max-Cut Problem - Uncovering Network Structures: This challenge can be applied to Sustainable Cities by optimizing community planning or to Peace and Justice by identifying polarized groups in social networks. Try to model a graph of nodes (e.g., people, locations) and find the optimal way to divide them into two distinct groups to maximize the connections (or disagreements) between them.
- The Knapsack Problem - Strategic Resource Allocation: This challenge addresses numerous real-world problems by finding the best way to allocate limited resources, such as distributing a budget across non-profit projects to maximize social impact. Try to model a scenario where you have a set of items, each with a cost and a value (e.g., projects with a budget and an impact score). Your goal is to choose the combination of items that provides the maximum possible value without exceeding a total budget.[3]


[1] Barkoutsos, Panagiotis Kl., Giacomo Nannicini, Antonis Robert, Ivano Tavernelli, and Stefan Woerner. 2020. “Improving the Quantum Optimization Algorithm for the Knapsack Problem.” Physical Review A 102 (3): 032415.

[2] Farhi, Edward, Jeffrey Goldstone, and Sam Gutmann. 2014. “A Quantum Approximate Optimization Algorithm.” arXiv preprint arXiv:1411.4028.

[3] Hadfield, Stuart, Zhihui Wang, Bryan O’Gorman, Eleanor G. Rieffel, Davide Venturelli, and Jarrod Biamonte. 2019. “From the Quantum Approximate Optimization Algorithm to a Quantum Alternating Operator Ansatz.” Algorithms 12 (2): 34.

## Track 3: Quantum Chemistry for Sustainable Technologies

The global transition to a sustainable future depends on the discovery of novel materials. Whether for next-generation batteries, efficient carbon capture, or green catalysts, the key lies in understanding and predicting the complex quantum interactions within molecules. Simulating these properties accurately is a profound challenge where quantum computers are expected to provide a significant advantage.

### Your challenge: Apply an advanced quantum chemistry algorithm to a molecule of your choice

You should use methods that go beyond standard ground state calculations, such as advanced solvers for computing specific molecular properties. This includes techniques like `Quantum Subspace Diagonalization (QSD)`, `Sampling-based Quantum Diagonalization (SQD)` for analyzing molecular behavior. Your goal is to:

1. Select a molecule that interests you.
2. Identify a key chemical property to investigate (e.g., excited state energies, dipole moment, etc.).
3. Implement the simulation using Qiskit and appropriate classical chemistry software.
4. Interpret your results in the context of the molecule's potential application.

**Bonus Points:**  Teams that choose to simulate a molecule directly relevant to a sustainability challenge will receive bonus points. Examples include, but are not limited to:
- A component of a next-generation battery (e.g., a simple electrolyte or cathode molecule).
- A molecule involved in carbon capture or catalysis.
- A molecule relevant to understanding environmental pollutants.


[1] Doney, Kirstin D., Joshua A. Job, William S. Friend, and Gavin O. Jones, et al. 2025. “Quantum-Centric Computational Study of Methylene Singlet and Triplet States.” Journal of Chemical Theory and Computation. https://doi.org/10.1021/acs.jctc.5c00075.

[2] Pelaez, D., et al. 2025. “Quantum-Centric Supercomputing: A New Computational Framework for Chemistry.” Paper presented at the American Chemical Society (ACS) Spring Meeting.

[3] Robledo-Moreno, J., M. Motta, H. Haas, A. Javadi-Abhari, P. Jurcevic, W. Kirby, S. Martiel, et al. 2024. “Chemistry beyond the Scale of Exact Diagonalization on a Quantum-Centric Supercomputer.” Science Advances 10 (25). https://doi.org/10.1126/sciadv.adu9991.

## 🏆 Winners 🏆

Congratulations to all winners and thank you everyone who competed!

<h2> 🥇 1st Place </h2>

**Team BLANK**: "Title"
- Repo Link
- Members:
  - [Name](https://github.com/NAME)

<h2>🥈 2nd Place </h2>

**Team BLANK**: "Title"
- Repo Link
- Members:
  - [Name](https://github.com/NAME)


<h2>🥉 3rd Place </h2>

**Team BLANK**: "Title"
- Repo Link
- Members:
  - [Name](https://github.com/NAME)
 
 <h2>🏅 4th Place </h2>

**Team BLANK**: "Title"
- Repo Link
- Members:
  - [Name](https://github.com/NAME)


---


## How to start Qomputing

[Start Here: How to Install Qiskit and Make Yourself ready for this Hackathon](put-your-drive-document-link-here)

[Quantum Learning Resources](put-your-drive-document-link-here)

---

## Winners and Awards

Winners: TBA

- Winners will receive a digital certificate and prizes will range from a final round interview with WISER for a paid fellowship, two cash prizes, and a one-time mentorship sesssion with IBM Quantum. The top winners will pick their prize first and the following winning teams will pick their prizes afterwards in order of ranking!


### Useful Resources

- [Qiskit Youtubes](https://www.youtube.com/Qiskit)

## Feedbacks

Your opinions matter and we take them seriously to improve QEE events! Please complete this end-of-event survery to tell us your experience at Q^3 Qompute 2025 and if you would like to attennd more events like this in the future. 

