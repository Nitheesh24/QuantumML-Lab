# Quantum ML Lab

Welcome to the Quantum ML Lab! This repository contains beginner-friendly projects that leverage quantum machine learning techniques using IBM's Qiskit framework. Below are the instructions for setup, configuring IBM Quantum token, and how you can run these projects both on simulators and IBM hardware.

## Setup
1. Clone this repository:
   ```bash
   git clone https://github.com/Nitheesh24/QuantumML-Lab.git
   cd QuantumML-Lab
   ```
2. Create a virtual environment and activate it:
   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```
3. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

## IBM Quantum Token Configuration
- Create an IBM Quantum account if you haven’t already. Go to [IBM Quantum](https://quantum-computing.ibm.com/) and create a free account.
- After creating the account, navigate to your account settings and copy your API token.
- Set your token using:
   ```bash
   export IBM_QISKIT_API_TOKEN='Your_API_Token_Here'
   ```
- You can also configure it in your script via Qiskit:
   ```python
   from qiskit import IBMQ
   IBMQ.save_account('Your_API_Token_Here')
   ```

## Running the Projects
- To run the projects locally using simulators, simply navigate to the project directory and execute the notebook or the run.py script:
   ```bash
   cd projects/01-quantum-kernel-qsvm
   jupyter notebook
   ```
- To run on IBM hardware, ensure your token is configured as mentioned above, and follow the instructions in each project's README.md.

## Projects
1. [Quantum Kernel QSVN](projects/01-quantum-kernel-qsvm/README.md)
2. [Variational Quantum Classifier](projects/02-vqc-classifier/README.md)
3. [Variational Quantum Regression](projects/03-vqr-regression/README.md)