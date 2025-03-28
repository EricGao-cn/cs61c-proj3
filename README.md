# CS61CPU

Look here, I made a CPU! This project is based on the [*Project 3: CS61CPU*](https://web.archive.org/web/20241214075649/https://cs61c.org/fa24/projects/proj3/) of Course CS61C, UC Berkeley. Here's what I did:

- Implement the R, I, S, B, U, J formats on the CPU
- Implement a 2-stage pipeline in my CPU, including **Instruction Fetch** and **Execute**

**Details**:
- 5 stages: IF, ID, EX, MEM, WB
- Components I have made: PC, ALU, RegFile, Control Unit, Immediate Generator, Branch Comparator  
- Construct the Datapath for all the formats

**How to run code on this CPU**:
1. Clone this repository and make sure you have Python 3 and Java installed.
2. Write your RISC-V assembly code in a file in `tests/intergration-custom/in` folder and with the `.s` extension.
3. Run following code to get the register information during the execution.
```shell
bash test.sh test_custom
bash test.sh format tests/intergration-custom/out/filename.out
```

**How to look into my CPU**:
1. Clone this repository and make sure you have Python 3 and Java installed.
2. Run the following code to open the **Logisim**:
```shell
bash tools/download_tools.sh # download the logisim first
java -jar tools/logisim-evolution.jar
```
3. When you have the **Logisim** opened, you can open the `cpu.circ` file in the `cpu` folder in the top left corner of logisim.
