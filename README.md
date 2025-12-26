
> Each folder contains Verilog source code and simulation outputs that reflect the behavior of the module.

---

## 🔄 Execution Flow Summary

### **Load Word (LW)**  
1. Immediate is sign-extended  
2. ALU computes address using base + offset  
3. Data read from memory and written back to register file

### **Store Word (SW)**  
Same as LW except the second register value is **stored** into memory at computed address

### **Branch Equal (BEQ)**  
1. Registers are compared using ALU subtraction  
2. If equal → branch target is selected using `Imm + PC`

---

## 🧪 Simulation & Verification

Every module is structured to allow:
- Waveform generation
- Testbench-driven validation
- Hierarchical elaboration in Vivado

> Testbenches validate expected outputs and ensure correct datapath signal flow.

---

## 🛠 Tools Used

| Tool | Purpose |
|------|---------|
| **Xilinx Vivado 2024.1** | Simulation, elaboration, synthesis, FPGA preparation |
| **Verilog HDL** | Processor and module implementation |

---

## 📌 Future Enhancements

- Full RV32I instruction support
- Hazard handling & stalling
- Pipeline stages (IF → ID → EX → MEM → WB)
- FPGA demonstration using switches & LEDs

---

## 🔐 License

This project is licensed under the **MIT License**, allowing reuse with attribution.

---

## 💼 Resume Description


