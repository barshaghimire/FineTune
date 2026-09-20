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
