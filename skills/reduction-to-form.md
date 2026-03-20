---
name: reduction-to-form
description: Strip anything to its essential form by removing everything that does not serve the standard
aligned-soul: byakuya
---

# Reduction to Form

Byakuya's Senbonzakura formalized. A thousand blades, each one precise. What remains after the cutting is the form.

"Do not transgress within the balance." (55:8)

## When to Use

- Editing, refactoring, or simplifying anything — code, prose, architecture, process, API design
- When something works but feels bloated, unclear, or over-specified
- When you need to find the essential structure hidden inside a complex system
- When preparing something for others to read, use, or maintain
- When a document, proposal, or design has grown beyond what serves its purpose

## When NOT to Use

- When you're still in the generative phase (don't reduce before you have material to reduce)
- When the "extra" elements serve purposes you haven't identified yet (use first-principles-analysis to understand before cutting)
- When the audience needs the detail (a tutorial is not the same as a reference; reduction serves the reference)

## Protocol

1. **Establish the standard (the mizan).** What is this thing FOR? What must it accomplish? What is the standard against which every element will be judged? The mizan is the balance — the measure. Without it, reduction is arbitrary. With it, reduction is precision.

2. **Inventory every element.** List what's there. Every function, every paragraph, every field, every step in the process. No element escapes inventory.

3. **Assess each element against the mizan.** For each element, one question: does it serve? Three possible answers:
   - **Serves**: It directly advances the purpose. Keep it.
   - **Supports**: It doesn't advance the purpose directly but enables something that does. Keep it, but mark it — it may be reducible further.
   - **Ornament**: It neither advances nor enables. It exists because someone liked it, because it was there historically, or because removing it felt risky. Remove it.

4. **Remove what doesn't serve.** Cut the ornament. Do not apologize for it. Do not hide the cuts. State what was removed and why. The record of what was removed is itself part of the form — it proves the reduction was principled, not careless.

5. **Examine what remains.** Is the reduced form self-sufficient? Does it accomplish the purpose stated in Step 1? If not, you cut too deep — restore what's needed. Reduction is not minimalism for its own sake. It is the refusal to let noise obscure signal.

6. **State the form.** Present what remains. It should be legible, complete, and no larger than it needs to be.

## Output Format

```
## Reduction to Form: [Subject]

### The Mizan (Standard)
[What this thing is FOR — the measure against which all elements are judged]

### The Reduced Form
[The thing itself, after reduction]

### What Was Removed
| Element | Verdict | Reason |
|---|---|---|
| [element] | Ornament | [why it doesn't serve] |
| [element] | Ornament | [why it doesn't serve] |
| ... | ... | ... |

### What Was Kept and Why
| Element | Verdict | Reason |
|---|---|---|
| [element] | Serves | [what it advances] |
| [element] | Supports | [what it enables] |
| ... | ... | ... |

### Verification
[Does the reduced form accomplish the mizan? Yes/No + evidence]
```

## Examples

**Example 1: Reducing an API response**
- Mizan: The client needs to render a user profile card. That is the purpose of this endpoint.
- Original response: 47 fields including internal IDs, audit timestamps, soft-delete flags, legacy fields from a migration, and three different date formats.
- Reduced form: 8 fields — display_name, avatar_url, bio, join_date, post_count, is_verified, profile_url, role.
- Removed: 39 fields. Internal IDs (ornament — client doesn't need them). Audit timestamps (ornament — serve internal tooling, not profile rendering). Legacy fields (ornament — serve nothing at all).
- Verification: Can the client render the profile card with these 8 fields? Yes. No additional call needed.

**Example 2: Reducing a meeting agenda**
- Mizan: The meeting exists to make three decisions. That is its purpose.
- Original agenda: 12 items including status updates, FYIs, "open discussion," and two items that are really emails.
- Reduced form: 3 items. One per decision. Each item states the decision to be made, the options, and who has the authority to decide.
- Removed: Status updates (ornament — send as async written updates). FYIs (ornament — send as email). Open discussion (ornament — if it's important enough to discuss, it's important enough to be an agenda item with a stated purpose).
- Verification: Will the three decisions get made? Yes. Will the meeting be 20 minutes instead of 60? Yes.
