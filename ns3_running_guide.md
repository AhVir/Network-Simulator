# Running ns-3 Simulation with Conda Environment

This guide explains how to run ns-3 simulations (example: 5 moving nodes) inside a Conda environment.

[sahmed](https://chatgpt.com/c/68a5b633-bc88-8332-af84-95e806af7aae)

---

## 1. Activate Conda Environment
```bash
conda activate ns3env
```

---

## 2. Go to ns-3 Directory
```bash
cd ~/ns-allinone-3.xx/ns-3.xx/
```
*(replace `xx` with your ns-3 version, e.g., `ns-3.41`)*

---

## 3. Build ns-3 (only needed the first time or after changes)
```bash
./ns3 build
```

---

## 4. Run Example Simulation (5 Nodes Mobility)
```bash
./ns3 run scratch/moving_nodes
```

Where `moving_nodes.cc` is your custom file inside the `scratch/` directory.

---

## 5. Open NetAnim to Visualize
```bash
netanim moving_nodes.xml
```

Make sure `moving_nodes.xml` was generated in your working directory.

---

## Notes
- Always activate the Conda environment before running simulations.
- You can create and test new `.cc` files inside the `scratch/` directory.
- Use NetAnim to visualize mobility and packet transfers.
