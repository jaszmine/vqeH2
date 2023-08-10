# vqeH2

The field of quantum physics and computing is one of the most interesting and promising endeavors in our day and age. From developing faster and more secure communication networks, to unlocking the protein folding problem, there’s immense potential in quantum algorithms and applications. A specific algorithm of interest is the Variational Quantum Eigensolver, or VQE, a hybrid classical-quantum algorithm used for solving optimization problems. 

An application of interest for such an algorithm includes calculating the energy of molecular Hydrogen (H2), one of the current most popular alternatives to methane. However, this is only one example of a molecule we can utilize VQE to understand. We can extend this tool to understand molecules involved across the energy sector including in solar cell materials, battery components, carbon capture, hydrogen storage, and virtually any chemical application, saving time, money, and resources. Here we can see an example of VQE finding the electronic structure of H2 with varying Angstrom distances between atoms.

### Steps Overview
1. Convert a molecule into a ‘QMolecule’ with varying distances between the H atoms.
2. Define a tunable circuit using ‘EfficientSU2’, mapping atoms to qubits where each qubit represents the state of an atom or particle.
   We also use the classical optimizer algorithm ‘COBYLA’ that employs linear approximations to objective and constraint functions.
3. Find the total energy through both VQE and an exact solver (to verify results) in addition to calculating percent error.

<br>

Tunable Circuit

<img width="433" alt="Screenshot 2023-08-10 at 7 26 22 AM" src="https://github.com/jaszmine/vqeH2/assets/52623824/a736afbf-6196-4cb5-8185-ecfef3ef9b97">

<br>
<br>

Total energies using vqe and exact solver w/percent error

<img width="600" alt="Screenshot 2023-08-10 at 7 28 50 AM" src="https://github.com/jaszmine/vqeH2/assets/52623824/6319144e-b5a8-47cc-91ba-aef098d59e29">

<br>
<br>

<img width="600" alt="Screenshot 2023-08-10 at 2 38 29 PM" src="https://github.com/jaszmine/vqeH2/assets/52623824/cb09015b-2b02-42d7-a893-585aa230e010">

<img width="600" alt="Screenshot 2023-08-10 at 2 38 41 PM" src="https://github.com/jaszmine/vqeH2/assets/52623824/fc86382c-dff3-40c5-9012-97a85231bad3">


<br>
<br>
<br>

Visualization of Exact Solver vs. VQE methods 

<img width="576" alt="Screenshot 2023-08-10 at 2 28 32 PM" src="https://github.com/jaszmine/vqeH2/assets/52623824/96c801f2-bc34-4cc2-b277-8e16f5f0d30a">

<br>
<br>

Through analysis of the results shown above, we can see the relative accuracy and time it takes for VQE to reach the optimal solution/energy compared to the exact solver. Now imagine using this method with much more complicated molecules with far more atoms than H2.

While VQE has shown immense promise, there are some limitations we have to consider such as available quantum resources, circuit complexity, error mitigation, and scalability. However, as we begin to improve both quality and quantity regarding quantum hardware, the prospects of VQE continue to grow. 

By finding the ground state of a molecule, we’re able to gain a better understanding of its behaviors and properties, allowing us to make informed decisions when creating applications of interest. This not only applies to the energy sector but also to industries such as pharmaceutical development, material science, and so much more, furthering our understanding of the world around us. 
