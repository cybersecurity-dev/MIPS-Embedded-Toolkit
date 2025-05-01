# MIPS based Embedded Device Toolkit

The **MIPS** (_Microprocessor without Interlocked Pipeline Stages_) architecture is a RISC (_Reduced Instruction Set Computer_) instruction set architecture (ISA) initially developed by MIPS Computer Systems in the early 1980s. It's known for its clean, simple design and has been influential in computer architecture education.

<details>

<summary>Install required tools on Linux</summary>

### For Ubuntu 18.04, 20.04, 22.04

```bash
sudo apt-get update
```
</details>


<details>

<summary>Install required python libs</summary>

### pip install
```bash
pip install -r requirements.txt
python3 setup.py install
```

### conda install
```bash
conda config --add channels conda-forge
conda install --file requirements_conda.txt
python3 setup.py install
```

</details>

| Feature             | MIPS (Microprocessor without Interlocked Pipeline Stages) | ARM (Advanced RISC Machines) |
|----------------------|---------------------------------------------------------|-----------------------------|
| **Instruction Set** | Primarily 32-bit fixed length, load-store architecture | Variable length (mostly 32-bit, with 16-bit Thumb) |
| **Instruction Format**| Fewer formats (R, I, J types)                          | More complex and numerous formats |
| **Registers** | 32 general-purpose registers                           | Up to 32 general-purpose registers (32-bit or 64-bit) |
| **Addressing Modes** | Simpler addressing modes                               | More complex and flexible addressing modes |
| **Execution** | Focus on single-cycle execution for most instructions   | Emphasis on low power consumption and efficiency |
| **Branching** | Delayed branches                                        | Conditional execution of many instructions |
| **Data Alignment** | Strict data alignment requirements                      | More flexible data alignment |
| **Endianness** | Configurable (Big or Little Endian)                     | Bi-endian (configurable, often Little Endian by default) |
| **History & Usage** | Historically used in embedded systems, networking, workstations; popular for teaching RISC concepts | Dominant in mobile devices, embedded systems, and increasingly in servers and desktops |
| **SIMD Extensions** | MIPS-3D, MDMX                                           | NEON, SVE, SVE2               |
| **Power Consumption** | Generally higher                                        | Generally lower                 |
| **Complexity** | Simpler instruction set and architecture               | More complex instruction set and architecture |
