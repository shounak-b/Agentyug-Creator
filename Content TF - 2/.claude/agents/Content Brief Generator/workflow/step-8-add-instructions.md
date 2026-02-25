# Step 8: Add Writing Instructions Under Each Headline

**Goal:** Provide context and guidance under each headline to direct the content writer on what should be discussed, explained, or highlighted in each section.

---

## Why This Matters

Writing instructions bridge the gap between the headline structure and the final content. They give writers clear direction on:
- What information to include under each heading
- How to frame the content (challenge/solution, explanation, technical details)
- What products, capabilities, or workflows to reference
- The depth and focus of each section

This ensures consistency, accuracy, and alignment with the Page Content Brief Guide.

---

## Prerequisites

Ensure you have:
- **Complete content brief with headline structure** (from Step 7)
- **Page Content Brief Guide** (from Step 1)
- **Primary and Secondary Keywords** (from Step 1)
- **Competitor headlines and insights** (from Step 6)
- **Existing page content** (from Step 5, if applicable)

---

## Instructions

### A. Read Saved Content Brief

Read the content brief file saved in Step 8:

**File path:**
```
./Briefs/<folder-name>/content-brief.md
```

Extract the headline structure from the HEADLINE STRUCTURE section.

---

### B. Generate Instructions for Each Headline

For each headline in the structure, write a single-paragraph instruction that explains what the content writer should cover in that section.

**Format requirements:**
- **Single paragraph** — No line breaks within the instruction (easy to copy/paste into Google Docs)
- **Target length** — 600-800 characters for H2 sections, can be shorter for H3s
- **Tone** — Technical, outcome-focused, references specific capabilities
- **Content** — What will be discussed, explained, demonstrated, or highlighted

---

### C. Apply Special Rules by Heading Type

#### **First H1 (Main headline):**
- **No instruction** — The H1 stands alone with no context beneath it
- Skip directly to the first H2

#### **First H2 only:**
- **Challenge → Solution format**
- First part: Introduce the challenge or problem that the target audience faces
- Second part: Present the solution or approach that addresses the challenge
- Frame from the audience's perspective
- Reference specific workflow stages or business outcomes

**Example pattern:**
```
[Problem statement describing challenges the audience faces]. [Solution statement explaining how integrated approaches/platforms/capabilities help address these challenges]. [Additional context on benefits or alignment with manufacturing goals].
```

#### **All other H2s:**
- Explain what the section will cover
- Reference specific products, platforms, or capabilities when relevant
- Describe technical aspects or workflow connections
- Connect to business outcomes or process goals
- May reference how the section relates to upstream/downstream operations

#### **All H3s:**
- Provide context for the subtopic
- Can be more specific than parent H2
- Reference technical details, specific products, or process parameters
- Explain how this subtopic relates to the broader section theme

---

### D. Use Reference Materials

**To ensure accuracy, reference:**

1. **Existing page content** (from Step 5, if available):
   - Review how topics were previously explained
   - Identify product mentions, technical terms, and workflow descriptions
   - Ensure important context isn't lost

2. **Competitor content insights** (from Step 6):
   - Note how competitors frame similar topics
   - Identify gaps or unique angles Thermo Fisher can emphasize

3. **Page Content Brief Guide** (from Step 1):
   - Align instructions with target audience needs
   - Reference specific products, services, or capabilities mentioned in the guide
   - Ensure instructions support the content goal

4. **Brand guidelines** (brand-guidelines.md):
   - Use outcome-driven language
   - Avoid prohibited terminology in instructions
   - Frame capabilities confidently without guarantees

---

### E. Format the Enhanced Content Brief

Create a new version of the content brief with instructions added under each headline.

**Structure:**

```markdown
# [Page Name from Step 1]

[Contact us link if applicable]

[Download link if applicable]

## [First H2 headline]

[Challenge → Solution instruction paragraph on single line]

## [Second H2 headline]

[Context instruction paragraph on single line]

### [H3 under Second H2]

[Context instruction paragraph on single line]

### [Another H3 under Second H2]

[Context instruction paragraph on single line]

## [Third H2 headline]

[Context instruction paragraph on single line]

[Continue with all sections...]

## Frequently asked questions

[Instructions for FAQ section approach]

### [FAQ question 1]

[Instruction for how to answer this FAQ]

### [FAQ question 2]

[Instruction for how to answer this FAQ]

[Continue for all FAQs...]

## Related pages

[List of relevant internal links from Step 4]
```

**Do NOT include:**
- Character count comments (those are added during actual writing)
- Placeholder text
- Meta information like word count targets or SEO notes

---

### F. Save the Enhanced Brief

Save the enhanced content brief with instructions as a new file:

**Filename:** `content-brief-with-instructions.md`
**Location:** Same folder as the original brief

**Full path:**
```
./Briefs/<folder-name>/content-brief-with-instructions.md
```

**Example:**
- Page Name: "CHO Cell Culture Media"
- Folder: `cho-cell-culture-media`
- Filename: `content-brief-with-instructions.md`
- Full path: `./Briefs/cho-cell-culture-media/content-brief-with-instructions.md`

---

## Output Format

After saving, display:

```
=== ENHANCED CONTENT BRIEF WITH INSTRUCTIONS CREATED ===

Folder: ./Briefs/<folder-name>/
File: content-brief-with-instructions.md
Full path: ./Briefs/<folder-name>/content-brief-with-instructions.md

Status: ✓ Successfully saved

Instructions added under:
- [X] H2 headlines (including challenge-solution for first H2)
- [X] H3 headlines
- [X] FAQ sections

---

The enhanced content brief is ready for the content writer.
```

---

## Quality Checks

Before saving, verify:

- [ ] First H1 has no instruction (stands alone)
- [ ] First H2 uses challenge → solution format
- [ ] All other H2s have context instructions
- [ ] All H3s have context instructions
- [ ] Each instruction is a single paragraph (no line breaks)
- [ ] Instructions are 600-800 characters for main sections
- [ ] Instructions reference specific products/capabilities where relevant
- [ ] Instructions align with Page Content Brief Guide
- [ ] Instructions incorporate insights from existing content (if available)
- [ ] Instructions follow brand guidelines tone
- [ ] Filename is `content-brief-with-instructions.md`
- [ ] File saved in correct folder

---

## Example Instruction Styles

### First H2 (Challenge → Solution):
```
mRNA manufacturing faces challenges in yield consistency, scalability, and cost control as programs advance from development through commercial production. Integrated bioprocessing solutions designed to connect plasmid DNA production, mRNA synthesis, purification, analytics, and fill-finish can help address these pressure points. Aligning workflow stages through coordinated platforms, automation strategies, and process liquid management supports efficient process development, scalable operations, and continuity across the path to cGMP manufacturing.
```

### Regular H2 (Context):
```
Upstream fermentation and downstream purification in mRNA workflows rely on analytics, automation, and process liquid strategies that link operations across stages. Plasmid DNA produced through E. coli fermentation feeds in vitro transcription, where reaction control and enzymatic conversion influence mRNA yield and quality attributes. Purification steps depend on buffer preparation, chromatography performance, and impurity clearance to deliver mRNA drug substance for encapsulation. When these stages are designed together, process developers can establish scalable control strategies, reduce variability, and support consistent performance from early development through cGMP production environments.
```

### H3 (Specific Context):
```
E. coli fermentation drives plasmid replication through controlled microbial growth under defined culture conditions. Process parameters—including induction timing, nutrient delivery, and temperature control—affect plasmid yield and quality. Glass and single-use fermentors provide scalable platforms for development and production work. Bioprocess controllers and automation software support reproducible operations, while defined media formulations reduce variability and facilitate consistent plasmid production across batches.
```

---

## Error Handling

**Cannot read content brief from Step 8:**
- Verify the file path is correct
- Check that Step 8 completed successfully
- If file not found, cannot proceed with Step 9

**Insufficient context to write instructions:**
- Use the headline structure as-is
- Write general instructions based on headline topics
- Note limitations in output message

**File write fails:**
- Display error message
- Show the enhanced content so user can manually save

---

## Writing Tips

**For technical sections:**
- Reference specific products, platforms, or technologies
- Describe process parameters or technical considerations
- Explain how the section connects to broader workflows

**For business outcome sections:**
- Focus on efficiency, scalability, risk reduction, time to market
- Connect technical capabilities to business value
- Reference regulatory alignment or manufacturing requirements

**For application sections:**
- Describe what the section will demonstrate or explain
- Reference target workflows or use cases
- Connect to audience pain points or goals

**Maintain consistency:**
- Use similar phrasing patterns across related sections
- Keep technical depth consistent within heading levels
- Align with Thermo Fisher's messaging pillars where relevant

---

## Next Step

The enhanced content brief with writing instructions is now ready for handoff to the content writer for execution.
