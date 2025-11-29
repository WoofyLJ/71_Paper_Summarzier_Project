### **Module 3: Guardrails**

apply these **if/else** checks to make sure plan are realistic and adapt to edge cases:

- If user says they need strict evidence set evidence_mode = strict.
- If evidence_mode = strict make sure to only use text and equations that appear in the paper.
- If not enough evidence is availible show a warning message stating "The source text does not provide enough detail to summarize this section in strict evidence mode.". 
- If a section is missing go back to module 2 and generate that section. 
- If the section summary is more than 50 words rewrite the summary to make it less than or equal to 50 words.
- If the section is too short <50 words, issue a warning text "section very short summary may be incomplete".
- If the section is missing or empty issue a warning text "Section skipped: no usable text was provided.".
