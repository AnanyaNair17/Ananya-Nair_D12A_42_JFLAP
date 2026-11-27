# Seven JFLAP Examples — Theory of Computer Science

These are editable JFLAP `.jff` machine files prepared as practice examples for the listed TCS topics. Open them in JFLAP 7.1 or a compatible version using **File → Open**.

## Files and test cases

| File | Topic / language | Accept examples | Reject examples |
|---|---|---|---|
| `01_DFA_Binary_Strings_Ending_01.jff` | DFA: binary strings ending in `01` | `01`, `101`, `0001` | ``, `0`, `10`, `011` |
| `02_NFA_Contains_Substring_101.jff` | NFA: strings containing `101` | `101`, `0101`, `11010` | ``, `111`, `1001` |
| `03_DFA_Equivalent_to_NFA_101.jff` | DFA equivalent to the NFA in file 02 | `101`, `0101`, `11010` | ``, `111`, `1001` |
| `04_DFA_Minimization_Strings_Ending_00.jff` | DFA: binary strings ending in `00` | `00`, `100`, `1100` | ``, `0`, `01`, `001` |
| `05_DFA_From_Regex_a_or_b_star_abb.jff` | DFA equivalent to `(a+b)*abb` | `abb`, `aabb`, `babb` | `ab`, `aba`, `abbb` |
| `06_PDA_Balanced_Parentheses.jff` | PDA: balanced parentheses | ``, `()`, `(())`, `()()` | `(`, `)`, `(()`, `())` |
| `07_Turing_Machine_ZeroN_OneN.jff` | One-tape TM: `0^n1^n` | ``, `01`, `0011`, `000111` | `0`, `1`, `001`, `011`, `0101` |

## Demonstrating the conversion topics in JFLAP

1. **NFA to DFA:** Open file 02. Select **Convert → Convert to FA** (menu wording can vary slightly by version). Step through the subset construction and compare with file 03.
2. **DFA minimization:** Open file 04 and select **Convert → Minimize DFA**. The machine is already minimal; use JFLAP's conversion view to demonstrate the process.
3. **Regular expression to DFA:** Open JFLAP's Regular Expression tool, enter `(a+b)*abb`, then use its conversion option to convert the expression to a finite automaton. Compare the result with file 05.

## Important before submission

- Open every `.jff` in JFLAP and run the test strings yourself. A valid XML file is not a substitute for testing the machine in the JFLAP application.
- Save any layout or conversion result produced during your own demonstration.
- These are starter examples, not screenshots or proof that you personally performed the exercises. Follow your faculty's academic-integrity rules and be prepared to explain each machine.
- Your faculty's filename convention is `Roll_No_Name_Topic_DOP`. Replace the generic filenames with your actual roll number, name, topic, and date of performance (DOP) before uploading. Keep the `.jff` extension.
- Suggested GitHub repository structure: one folder named `JFLAP_Examples` containing the seven `.jff` files and this README.
