# THEORY OF COMPUTER SCIENCE
## JFLAP – SELF LEARNING ASSIGNMENT

**Department:** Computer Engineering  
**Academic Year:** 2026–2027  
**Course:** Theory of Computer Science  
**Year/Semester/Division:** T.E. / Semester V / D12A  
**Subject Code:** 26CMPC51  
**Faculty In-charge:** Mr. Sanjay Mirchandani  

---

## 1. Introduction

JFLAP (Java Formal Languages and Automata Package) is an educational software tool used to design, simulate and experiment with concepts of Theory of Computer Science. It provides a graphical interface for constructing and testing finite automata, pushdown automata, Turing machines, regular expressions and grammars.

This assignment demonstrates seven important concepts of automata theory using JFLAP. Each example illustrates the construction and working of a computational model through state diagrams and input-string testing.

## 2. Objectives

1. To understand the construction and working of Deterministic Finite Automata (DFA).
2. To understand Nondeterministic Finite Automata (NFA).
3. To study the conversion of NFA into DFA.
4. To understand DFA minimization.
5. To explore the relationship between regular expressions and finite automata.
6. To understand Pushdown Automata and stack operations.
7. To study the working of a single-tape Turing Machine.

## 3. JFLAP Experiments

### Experiment 1: Deterministic Finite Automata (DFA)

**Aim:** To construct a DFA that accepts binary strings ending with `01`.

**Description:** The automaton uses three states to track the last two relevant input symbols. It accepts a string only when its final two symbols are `01`.

**Sample Test Cases:**
- Accepted: `01`, `101`, `0001`
- Rejected: `0`, `10`, `011`

### Experiment 2: Nondeterministic Finite Automata (NFA)

**Aim:** To construct an NFA that accepts strings containing the substring `101`.

**Description:** The automaton nondeterministically guesses the beginning of the required substring. Once the sequence `101` is identified, it remains in the final state for the remaining input symbols.

**Sample Test Cases:**
- Accepted: `101`, `0101`, `11010`
- Rejected: `111`, `1001`

### Experiment 3: NFA to DFA Conversion

**Aim:** To convert an NFA into an equivalent DFA.

**Description:** The subset construction method is used to convert a nondeterministic finite automaton into a deterministic finite automaton. The resulting DFA recognizes the same language as the original NFA.

**Sample Test Cases:**
- Accepted: `101`, `0101`, `11010`
- Rejected: `111`, `1001`

### Experiment 4: DFA Minimization

**Aim:** To construct and minimize a DFA that accepts binary strings ending with `00`.

**Description:** DFA minimization reduces the number of states without changing the language accepted by the automaton. The example uses three states to distinguish strings based on their ending symbols.

**Sample Test Cases:**
- Accepted: `00`, `100`, `1100`
- Rejected: `0`, `01`, `001`

### Experiment 5: Regular Expression to DFA Conversion

**Aim:** To construct a DFA equivalent to the regular expression `(a+b)*abb`.

**Description:** The regular expression represents all strings over the alphabet `{a,b}` that end with `abb`. The equivalent DFA tracks the progress of matching the required suffix.

**Sample Test Cases:**
- Accepted: `abb`, `aabb`, `babb`
- Rejected: `ab`, `aba`, `abbb`

### Experiment 6: Pushdown Automata (PDA)

**Aim:** To construct a Pushdown Automaton that accepts balanced parentheses.

**Description:** A PDA uses a stack to keep track of opening parentheses. An opening parenthesis pushes a symbol onto the stack, while a closing parenthesis removes one. A string is accepted when all parentheses are correctly matched.

**Sample Test Cases:**
- Accepted: `()`, `(())`, `()()`
- Rejected: `(`, `)`, `(()`, `())`

### Experiment 7: One-Tape Turing Machine

**Aim:** To construct a single-tape Turing Machine that accepts strings of the form `0ⁿ1ⁿ`.

**Description:** The Turing Machine marks each unprocessed `0` and matches it with an unprocessed `1`. The machine accepts when all symbols are successfully matched in the required order.

**Sample Test Cases:**
- Accepted: `01`, `0011`, `000111`
- Rejected: `0`, `1`, `001`, `011`, `0101`

## 4. Software Requirements

- **Software:** JFLAP
- **Version:** JFLAP 7.1 or compatible version
- **Programming Language:** Java (JFLAP runtime)
- **File Format:** `.jff` (JFLAP file format)
- **Operating System:** Windows / Linux / macOS

## 5. Conclusion

Through these seven experiments, fundamental concepts of Theory of Computer Science were explored using JFLAP. The exercises demonstrate the construction and simulation of finite automata, conversion between automata, DFA minimization, regular expression representation, stack-based computation and Turing machine operations.

JFLAP provides an effective visual learning environment for understanding abstract computational models and their applications in formal language theory.

## 6. References

1. JFLAP Official Website: https://www.jflap.org/
2. JFLAP Modules: https://www.jflap.org/modules/
3. JFLAP GitHub Repository: https://github.com/NHK2012/JFLAP
4. Hopcroft, Motwani and Ullman, *Introduction to Automata Theory, Languages, and Computation*.
