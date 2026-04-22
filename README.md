# SNN Roadmap with Brian2

A systematic exploration of **Spiking Neural Networks (SNNs)** and **Neuromorphic Computing** using the Brian2 simulator. This repository documents the transition from fundamental biological neuron modeling to complex spike-based learning patterns.

## Overview

This project serves as a technical roadmap for implementing SNNs. Unlike traditional rate-based neural networks, these models focus on the precise timing of spikes to process information, utilizing the **Brian2** library to define neuron behavior through differential equations.

## Core Concepts

The notebooks in this repository cover:
* **LIF Modeling:** Implementing Leaky Integrate-and-Fire neuron dynamics.
* **STDP (Spike-Timing-Dependent Plasticity):** Exploring how synaptic weights ($w$) evolve based on the millisecond-level latency between pre- and post-synaptic events.
* **Temporal Encoding:** Shifting from rate-coded inputs to time-coded information processing.
* _More to come_

## Repository Structure

### 1. Single Synapse Toy Network
* **Focus:** The "Hello World" of STDP.
* **Objective:** Visualizing the weight change curve ($Δw$). It demonstrates how a synapse strengthens when a presynaptic spike precedes a postsynaptic spike (LTP) and weakens in the reverse scenario (LTD).

### 2. STDP Learning from Temporal Encoding
* **Focus:** Pattern Recognition.
* **Objective:** Scaling the network to recognize distinct input patterns. This notebook implements a functional architecture where the SNN learns to classify or differentiate signals based solely on the temporal distribution of spikes.

#### SNN Practice & Scratchpad
* **Focus:** Prototyping.
* **Objective:** Experimental code for testing equation-based neuron definitions, threshold resets, and Brian2's `StateMonitor` and `SpikeMonitor` functionalities.

## Prerequisites

To run these notebooks, you will need:
* Python 3.x
* Brian2
* Jupyter / Matplotlib / NumPy

```bash
pip install brian2 matplotlib jupyter
```

## Learning Journey
This repository is a live documentation of progress in neuromorphic engineering. Each notebook builds upon the last, moving from the microscopic view of a single synapse to the macroscopic behavior of learning networks.
