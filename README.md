# Reliable quantum hypothesis testing: a hands-on primer

Small, checkable simulations of the core statistical questions in quantum sensing, computing and communication:

1. **Helstrom bound:** the optimal one-shot error for distinguishing two quantum states, and the measurement that achieves it.
2. **Quantum Chernoff bound:** exponential error decay with n copies; collective vs copy-by-copy measurement.
3. **Quantum relative entropy:** numerical check of the data-processing inequality over 2,000 random measurements.
4. **Quantum Fisher information:** phase estimation, the quantum Cramér–Rao bound, and a two-stage adaptive measurement that nearly reaches it.
5. **Sequential testing:** an anytime-valid likelihood-ratio test (Ville's inequality) and Wald's SPRT. Type-I error stays below α with data-dependent stopping and uses fewer copies than a fixed-sample test, while "peeking" at a fixed-sample test inflates false alarms.
6. **Qiskit validation:** the Helstrom measurement as a circuit, checked against theory on AerSimulator.

## Run

```bash
pip install -r requirements.txt
jupyter notebook quantum_hypothesis_testing_primer.ipynb
```

Parts 1–5 need only NumPy, SciPy and Matplotlib. Part 6 needs Qiskit.
