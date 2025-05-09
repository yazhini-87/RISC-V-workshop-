# RV Day 2 - Introduction to ABI and basic verification flow
## RV-D2SK1 - Application Binary interface (ABI)
### RV_D2SK1_L1_Introduction To Application Binary Interface
 - Interface - appearance and functionality for the user 
 - There are multiple layer of software in which there is a *application binary interface(ABI)* as a layer.
   ![images/IMG-20250509-WA0020[1].jpg](https://github.com/yazhini-87/RISC-V-workshop-/blob/3e82864886096adfb7297973db42aa6cc5fe7160/images/IMG-20250509-WA0020%5B1%5D.jpg)
- ABI, also referred to as the **System Call Interface**, acts as a bridge between system calls and the ISA through the use of registers.
  - There are two categories of Instruction Set Architectures (ISA):
      - **User ISA** – managed entirely by the user space.

      - **System & User ISA** – shared control between the system (kernel) and the use
- Totally RISCV has 32 register and 8 bytes (64bits) and denoted using XLEN
   ![image](https://github.com/yazhini-87/RISC-V-workshop-/blob/421fe3970ffe91c7cc4905818e6d0b4946654f5e/images/IMG-20250509-WA0023%5B1%5D.jpg)
  

  ---

  ### RV_D2SK1_L2_Memory Allocation For Double Words
  - Double Word (64-bit) Allocation: In RISC-V RV64, a double word refers to 64-bit (8 bytes) of memory.
  - Alignment Requirement: Double words must be aligned to an 8-byte boundary in memory for efficient access.
    ![image](https://github.com/yazhini-87/RISC-V-workshop-/blob/421fe3970ffe91c7cc4905818e6d0b4946654f5e/images/IMG-20250509-WA0024%5B1%5D.jpg)

  ---
 ### RV_D2SK1_L3_Load, Add And Store Instructions With Example
**Field	Meaning**
1. ld -Load doubleword
2. x8	-Destination register (rd)
3. 16	-Immediate offset from base address
4. x23-Base address register (rs1)

**2nd case**
1. The first x8 is the desitination register (rd)
2. x24 is a source register (rs1)
3. x8 is the second sourse register (rs2)

![image](https://github.com/yazhini-87/RISC-V-workshop-/blob/421fe3970ffe91c7cc4905818e6d0b4946654f5e/images/IMG-20250509-WA0027%5B1%5D.jpg)

---

### RV_D2SK1_L4_Concluding 32-registers And Their Respective ABI Names
![i](https://github.com/yazhini-87/RISC-V-workshop-/blob/421fe3970ffe91c7cc4905818e6d0b4946654f5e/images/IMG-20250509-WA0028%5B1%5D.jpg)

---

## RV-D2SK2 - Lab work using ABI function calls
