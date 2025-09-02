# Welcome to Q^3 Qompute 2025!
All Challenges are provided by IBM Quantum. 

> [!IMPORTANT]
**Please note that in-person attendees must check in on 9/14**

- [Overview](#overview)
- [Challenges and Submission Details](#challengesAndSubmissionDetails)
- [Final Teams](#final-teams)
- [Winners](#-winners-)
------

Preparation

- [Requirement](#requirement)
  - [Access to IBM Hardware](#access-to-ibm-hardware)
  - [Working on qBraid Lab](#working-on-qbraid-lab)
  - [Working on IBM Quantum Lab](#working-on-ibm-quantum-lab)
  - [Working on Locally](#working-on-locally)
- [Submitting the tasks](#submitting-the-tasks)
- [Judging Criteria](#judging-criteria)
- [Winners and Awards](#winners-and-awards)
- [Resources](#resources)
  - [Learning Materials](#learning-materials)
    - [Quantum Computing and Algorithms](#quantum-computing-and-algorithms)
    - [Workflow Example Tutorials](#workflow-example-tutorials)
  - [API Reference](#api-reference)
  - [Useful Resources](#useful-resources)
- [Tips](#tips)
- [Feedbacks and Discussions](#feedbacks-and-discussions)

## **Overview**

The convergence of quantum science and global sustainability efforts is unlocking a new horizon of possibility. Quantum computing provides a transformative toolkit to achieve the ambitious vision of the UN's Sustainable Development Goals, offering powerful new approaches to problems in simulation, optimization, and foundational computation itself. [1]

This Q3 USC hackathon, supported by IBM, is structured as a direct inquiry into quantum's potential, presenting a series of challenges across critical domains:
- Reversible computing: Probing the principles of reversible computing to address the fundamental energy cost of information processing
- Complex optimization problem: Untangling intractable logistical and energy-grid puzzles
- Natural Simulations: Modeling the very building blocks of nature to accelerate the discovery of new medicines and materials.

Your goal is to engage with one of these core challenges. Beyond simply implementing an algorithm, you are challenged to consider the deeper questions of real-world application and the broader social context of your work.

## **Challenges and Submission Details**

The final submission for this hackathon is a 5-10 minute presentation in any chosen format and your GitHub Repository. 

## Track 1: Feynman's dream - Reversible computing

This track is your conceptual entry point into the quantum world, starting with a foundational question that puzzled the pioneers of computing: Can we compute reversibly?

### Reversible computing

In classical computers, most logic gates are `irreversible`. For example, and AND gate outputs `0` for three different inputs (`00`, `01`, `10`). If you only have the output, you can't know the input - information has been lost. According to Landauer's Principles, this act of erasing information fundamentally requires energy dissipation, making computation inherently inefficient. A **reversible computation**, in contrast, is one where you can always reverse the process to find the original input from the output, meaning no information is lost. [2]

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



## HERE

> [!NOTE]
The idea is that it serves a practical use case and can be accessed by anyone without special tooling that is not already included in a typical computer installation (or minimal installation)

## Final Teams
Thank you for choosing IBM Quantum Challenge!

- hyperposition: [Repository](https://github.com/GeorgeHolm/ALQORITHM)
- Bulldogs: [Repository](https://github.com/shannenespinosa/iquhack24)
- Stockfish: [Repository](https://github.com/aace217/iQuHACK2024)
- team-7: [Repository](https://github.com/grid-rider/team-7-iQuHACK)
- mass2024: [Repository](https://github.com/quargsgreene/ibmgamechallenge)
- [B]Alde's Gate: [Repository](https://github.com/coderalde/iQuHack-2024-B-Alde-s-Gate/tree/main)

## 🏆 Winners 🏆

Congratulations to all winners!

<h2> 🥇 1st Place </h2>

**Team Bulldogs**: "Organ Donation QuAllocation
Quantum Approximate Optimization Algorithm for Organ Donor and Patient Matching" 
- https://github.com/shannenespinosa/iquhack24
- Members:
  - [Shannen Espinosa](https://www.linkedin.com/in/shannenespinosa/)
  - [Siona Tagare](https://www.linkedin.com/in/siona-tagare-2aa71a2a6/)
  - [Alma Alex](http://www.linkedin.com/in/alma-alex-b41596236)
  - [Annli Zhu](https://www.linkedin.com/in/annli-zhu-214016184/)

<h2>🥈 2nd Place </h2>

**Team team-7**: "MITqute" 
- https://github.com/grid-rider/team-7-iQuHACK
- Members:
  - [Liam Kronman](https://www.linkedin.com/in/liam-kronman/)
  - [Maggie Bao](@maggie-bao202)
  - [Nicole Shen](https://www.linkedin.com/in/nicole-shen-38b81b293/)
  - [Armin Ulrich](https://www.linkedin.com/in/arminulrich/)
  - [Sierra Romo](https://www.linkedin.com/in/sierra-romo-568002253/)


<h2>🥉 3rd Place </h2>

**Team hyperposition**: "ALQORITHM: A novel, quantum signal processing-based algorithm builder"
- https://github.com/GeorgeHolm/ALQORITHM
- Members:
  - [Brennan Lagasse](https://github.com/BrennanLagasse)
  - [Frank Wong](https://github.com/frank-cywong)
  - [Pranet Sharma](https://github.com/pranetksharma)
  - [George Holm](https://github.com/GeorgeHolm)
  - [Diya Naik](https://github.com/diyamagnetism)
---

## **Requirement**

### Access to IBM Hardware
In order to gain access to IBM Quantum hardware for working on qBraid Lab or Locally:

1. Login to https://quantum.ibm.com/. If you don't have your IBMid, please signin first. 
2. After login, please copy your "API Token" by clicking double square butten at the top right and save it for the aBraid Quantum Lab
<img src="./img/apitoken.png" width=100%>

### Working on qBraid Lab
[<img src="https://qbraid-static.s3.amazonaws.com/logos/Launch_on_qBraid_white.png" width="150">](https://account.qbraid.com/?gitHubUrl=https://github.com/iQuHACK/2024_IBM.git)


1. If you're working on qBraid, first fork this repository and click the above `Launch on qBraid` button. It will take you to your qBraid Lab with the repository cloned.
   
2. Use the default environment to use the latest Qiskit.

<img width="287" alt="image" src="./img/default_env.png">

3. [This tutorial](https://github.com/qBraid/qbraid-lab-demo/blob/main/qbraid_sdk/ibm_quantum_jobs_with_runtime.ipynb) will give you a guideline on how to use your own IBM Quantum Credential. You can find it through qBraid Lab under the "qbraid_sdk" folder as well. 

### Working on IBM Quantum Lab

You can also work on the [IBM Quantum Platform](https://quantum.ibm.com/), by using [IBM Quantum Lab](https://quantum.ibm.com/lab). In Quantum Lab, you can write scripts that combine Qiskit code, equations, visualizations, and narrative text in a customized Jupyter Notebook environment — no installation required. Run code on real quantum hardware(opens in a new tab) or simulators(opens in a new tab). Store, access, and manage your files from anywhere.

> [!IMPORTANT]
While you are using IBM Quantum Lab, you don't need to select a channel or save tokens.

### Working on Locally
If you will work locally or in a cloud environment, all users' first step is installing Qiskit. 

Please follow [this installation tutorial](https://docs.quantum.ibm.com/start/install). After installing the latest Qiskit, You can access IBM Quantum systems by using the `IBM Quantum Platform` or `IBM Cloud` channel. Channel is the term used to describe the method you use to access IBM Quantum services, and for this challenge, we suggest you use the `IBM Quantum Platform` channel and follow this [instruction](https://docs.quantum.ibm.com/start/setup-channel#set-up-to-use-ibm-quantum-platform) to set up a channel for your project.


## Submitting the tasks

> [!IMPORTANT]
Submission Due: 10am ET, 4th Feb (Sunday)</br>
Link will expires after due.

Submission: Thank you so much for choosing IBM Quantum Challenge!

## **Judging Criteria**

1. **Technical Aspects (30%)** : This category includes the following subcategories:
    - Quantum Complexity : How complex is the quantum algorithm? How optimized is it?
    - Architecture : Does the architecture leverage cloud technologies to optimize cost? Can the architecture serve users at a reasonable scale?
    - Accessibility/User Experience : How accessible is the end user application? Is it easy to use and intuitive for end users?
2. **Originality and Uniqueness (25%)** : How unique is this project compared to others? How interesting is it? Did the team attempt something new or difficult?
3. **Usefulness and Complexity (25%)** : How useful is the project and how well-designed is it? How functional is it at the time of judging? Can it be used in real-world business applications or serve as a valuable tool for individuals?
4. **Presentation (20%)** : How well did the team present their project? Were they able to explain their decisions? Did the entire team have a chance to speak?

## Winners and Awards

Winners: TBA

- Winners will receive a digital certificate and can get a [Tier 1](https://github.com/qiskit-advocate/application-guide) score when they apply for the Qiskit Advocate. 
- The number of total winners might depend on the number of applications.

## Resources

### Learning Materials

#### Quantum Computing and Algorithms

- [Basics of quantum information](https://learning.quantum.ibm.com/course/basics-of-quantum-information) by John Watrous (Award Badge Available)
- [Fundamentals of quantum algorithms](https://learning.quantum.ibm.com/course/fundamentals-of-quantum-algorithms) by John Watrous
- [Variational algorithm design](https://learning.quantum.ibm.com/course/variational-algorithm-design)

#### Workflow Example Tutorials

- [Qiskit Runtime Lab](https://github.com/JavaFXpert/qiskit-runtime-lab) by [James Weaver](https://github.com/JavaFXpert)
- [Variational quantum eigensolver](https://learning.quantum.ibm.com/tutorial/variational-quantum-eigensolver)
- [Quantum approximate optimization algorithm](https://learning.quantum.ibm.com/tutorial/quantum-approximate-optimization-algorithm)
- [CHSH inequality](https://learning.quantum.ibm.com/tutorial/chsh-inequality)
- [Max-Cut](https://learning.quantum.ibm.com/tutorial/max-cut)
- [Heisenberg chain](https://learning.quantum.ibm.com/tutorial/heisenberg-chain)
- [And More!](https://learning.quantum.ibm.com/catalog/tutorials)


### API Reference

- [Qiskit](https://docs.quantum.ibm.com/api/qiskit)
- [Qiskit Runtime IBM Client](https://docs.quantum.ibm.com/api/qiskit-ibm-runtime)
- [Qiskit IBM Runtime REST API](https://docs.quantum.ibm.com/api/runtime/tags/jobs)
- [Qiskit IBM Provider](https://docs.quantum.ibm.com/api/qiskit-ibm-provider)

### Useful Resources

- [Qiskit Youtubes](https://www.youtube.com/Qiskit)
- [IBM Quantum Blogs](https://www.ibm.com/quantum/blog)
- [Qiskit Slack](https://qisk.it/join-slack): Meet the community!


## Tips
This year’s iQuHACK challenges require a write-up/documentation portion that is heavily considered during
judging. The write-up is a chance for you to be creative in describing your approach and describing
your process. It can be in the form of a blog post, a short YouTube video or any form of
social media. It should clearly explain the problem, the approach you used, your implementation with results
from simulation and hardware, and how you accessed the quantum hardware (total number of shots used, 
backends used, etc.).

Make sure to clearly link the documentation into the `README.md` and to include a link to the original challenge 
repository from the documentation.

## Feedbacks and Discussions

Your opinions matter! Place to share your feedback on Qiskit [here](https://github.com/Qiskit/feedback
); stay up to date with release planning and DemoDays; and find out where to get support.
