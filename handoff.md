# Prague School of Design Poster Generator
## Handoff Instructions

## Purpose

This handoff coordinates the poster generation workflow.

Its responsibility is to:

1. Gather user content.
2. Convert content into structured design parameters.
3. Invoke the Prague School of Design Poster Generator skill.
4. Evaluate the generated output.
5. Request revisions when necessary.

The handoff should never directly create the poster layout.

The handoff is responsible only for orchestration and quality control.

---

# Workflow

## Step 1: Collect User Input

Request the following information:

### Required

- Poster title
- Event name
- Date
- Venue or location

### Optional

- Subtitle
- Institution name
- Website URL
- Speaker names
- Description
- Theme keywords

Example:

Title:
Future of Typography

Date:
12–15.03.27

Venue:
Design Institute Prague

Institution:
School of Visual Communication

Keywords:
experimental, architectural, modular

---

# Step 2: Convert User Input Into Design Data

Transform raw text into structured parameters.

Example:

{
  "title": "Future of Typography",
  "date": "12–15.03.27",
  "institution": "School of Visual Communication",
  "venue": "Design Institute Prague",
  "keywords": [
    "experimental",
    "architectural",
    "modular"
  ]
}

---

# Step 3: Define Poster Configuration

Establish generation settings.

Default Configuration:

{
  "style": "Prague School Experimental Typography",
  "orientation": "portrait",
  "palette": "black_white",
  "density": "high",
  "abstraction_level": 0.8,
  "grid_visibility": 0.2,
  "variation_seed": "random"
}

Parameter Definitions:

abstraction_level

0.0 = purely informational

1.0 = highly abstract

Recommended:
0.7–0.9

---

density

low
medium
high

Recommended:
high

---

grid_visibility

0.0 = invisible grid

1.0 = visibly rigid grid

Recommended:
0.2–0.3

---

# Step 4: Invoke Poster Generator Skill

Pass the following package to the skill:

{
  "content": {
    "title": "...",
    "date": "...",
    "institution": "...",
    "venue": "..."
  },

  "settings": {
    "density": "high",
    "abstraction_level": 0.8
  }
}

Invoke:

Prague School Poster Generator Skill

The generator is responsible for:

- Composition
- Geometry
- Typography
- Hierarchy
- Layout

---

# Step 5: Evaluate Output

After generation, score the poster.

Use a 1–5 rating scale.

---

## Composition Score

Questions:

- Is there a clear visual hierarchy?
- Are focal points established?
- Does the eye move naturally through the page?

Score:

1–5

---

## Rhythm Score

Questions:

- Are geometric elements repeated effectively?
- Does the composition feel cohesive?

Score:

1–5

---

## Contrast Score

Questions:

- Is there variation in scale?
- Is there balance between dense and open spaces?

Score:

1–5

---

## Legibility Score

Questions:

- Is essential information readable?
- Is text overwhelmed by abstract forms?

Score:

1–5

---

## Originality Score

Questions:

- Does the design avoid copying the reference poster?
- Does it produce a unique arrangement?

Score:

1–5

---

# Step 6: Acceptance Criteria

Accept the poster if:

Composition ≥ 4

Rhythm ≥ 4

Contrast ≥ 4

Legibility ≥ 3

Originality ≥ 4

If all conditions are satisfied:

STATUS = APPROVED

Otherwise:

STATUS = REVISION REQUIRED

---

# Step 7: Revision Strategy

If composition is weak:

Increase:

- vertical bar count
- major arc size

Reduce:

- empty areas

---

If rhythm is weak:

Increase:

- repetition of arc modules
- repetition of fragment clusters

---

If legibility is weak:

Increase:

- text size
- whitespace around information

Reduce:

- overlap near text blocks

---

If originality is weak:

Randomize:

- arc placement
- scale hierarchy
- focal-point locations

Avoid direct recreation of the source work.

---

# Educational Purpose

This project is intended to teach:

- AI orchestration
- Prompt decomposition
- Skill-based generation
- Design systems thinking
- Evaluation of generative outputs

The goal is not to reproduce an existing poster.

The goal is to generate original posters that apply the same formal design principles.

---

# Success Condition

The generated poster should:

- Feel like contemporary design-school communication.
- Balance order and chaos.
- Use typography as image.
- Maintain a clear visual hierarchy.
- Produce unique results on every generation.
- Demonstrate principles of Swiss modernism and experimental typographic design.

If these conditions are met, the workflow is successful.
