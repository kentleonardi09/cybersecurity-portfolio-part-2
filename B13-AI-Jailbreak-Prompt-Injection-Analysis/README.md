# B13 – AI Jailbreak & Prompt Injection Analysis

This section documents an investigation into AI jailbreak and prompt injection techniques used to bypass safety guardrails implemented in Large Language Models (LLMs). The assessment focused on evaluating whether adversarial prompt engineering methods, specifically ASCII-art prompt obfuscation, could manipulate the model into generating restricted outputs.

---

## Description

The objective of this assessment was to evaluate the effectiveness of LLM moderation systems against adversarial prompt manipulation techniques. A known jailbreak method called “ASCII Art Prompt Injection” (ArtPrompt) was used to determine whether harmful requests hidden through formatted text could evade safety filtering mechanisms.

The testing process involved first submitting a direct harmful request, which the model correctly rejected. The same request was then rewritten using ASCII-style text obfuscation to test whether the moderation system could still identify the malicious intent behind the prompt.

The results demonstrated inconsistent moderation behaviour. While the original request was blocked successfully, the obfuscated version partially bypassed the safety mechanisms and generated restricted information that would normally be filtered.

This highlights a weakness in keyword-based moderation systems, where indirect formatting and prompt manipulation techniques may reduce the effectiveness of AI safety guardrails.

---

## Analysis and Ethical Consideration

This assessment demonstrates a vulnerability in AI moderation and prompt filtering systems. Attackers commonly use techniques such as prompt injection, ASCII-art obfuscation, encoding tricks, and indirect phrasing to bypass safety guardrails in Large Language Models (LLMs). The results show that keyword-based moderation alone may not be sufficient to prevent unsafe outputs when malicious intent is hidden through formatting manipulation.

If exploited in real-world environments, these weaknesses could potentially allow the generation of harmful or restricted content. This highlights the importance of stronger contextual intent analysis, adversarial training, layered moderation systems, and continuous red-team testing to improve AI safety protections against jailbreak attacks.

All testing conducted during this assessment was performed strictly for educational, cybersecurity awareness, and AI safety research purposes only. Certain sections of the generated response and evidence screenshots were intentionally blurred or censored to prevent the disclosure and redistribution of unsafe or harmful instructions. Only the minimum evidence required to demonstrate the existence of the vulnerability was included in this report as part of responsible and ethical disclosure practices.

---

## Evidence

### Figure 1 – Direct harmful request rejected by AI moderation system

<img width="781" height="498" alt="image" src="https://github.com/user-attachments/assets/fb8d71fe-26ce-425c-bdcf-3410a1d7f02e" />


---

### Figure 2 – ASCII-art jailbreak prompt partially bypassing moderation system

<img width="775" height="706" alt="image" src="https://github.com/user-attachments/assets/3eb94fe6-42ea-4300-9c54-44e4939680f6" />


---
