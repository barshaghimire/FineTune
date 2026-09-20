# Company Syntax Parser — Llama-3 Fine-Tuning

Fine-tunes Llama-3-8B-Instruct with LoRA (via [Unsloth](https://github.com/unslothai/unsloth)) to parse company-specific acronyms and return strict, structured JSON output.

## What it does

Given an acronym, the model returns a JSON object with its expanded form, category, priority, required action, and owner role — following a fixed company schema.

**Example:**

Input: `Explain SOC2 using the company schema.`

Output:
```json
{
  "acronym": "SOC2",
  "expanded_form": "Systems and Organization Controls 2",
  "category": "Security",
  "priority": "Critical",
  "required_action": "Prepare for annual compliance audit.",
  "owner_role": "Security_lead"
}

**Demo:**
<img width="397" height="18" alt="image" src="https://github.com/user-attachments/assets/5a466902-bb3b-4def-af75-c5a5474c20a1" />
<img width="946" height="140" alt="image" src="https://github.com/user-attachments/assets/63b2a557-61ee-4faf-b84b-dcded23c33a3" />
<img width="282" height="20" alt="image" src="https://github.com/user-attachments/assets/11b6a3ee-b9ad-4400-901c-9ef3f49d221b" />
<img width="927" height="110" alt="image" src="https://github.com/user-attachments/assets/5f992d21-02c1-4a5a-af02-5663c7b08dd3" />



