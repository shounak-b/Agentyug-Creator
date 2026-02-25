# Step 7: Save Content Brief to File

**Goal:** Create a dedicated folder for the page and save the generated content brief as a markdown file for easy access and version control.

---

## Why This Matters

Organizing content briefs in dedicated folders ensures:
- Easy retrieval and reference for content writers
- Clean file organization by page/project
- Version control and historical tracking
- Consistent file structure across all briefs

---

## Prerequisites

Ensure you have:
- **Generated content brief** (from Step 7)
- **Page Name** (from Step 1)

---

## Instructions

### A. Create Folder Structure

Create a folder inside the Briefs directory using the Page Name:

**Base directory:** `./Briefs` (relative to current working directory)

**Folder naming convention:**
- Use the Page Name from Step 1
- Replace spaces with hyphens
- Use lowercase for consistency
- Remove special characters except hyphens

**Example transformations:**
- "CHO Cell Culture Media" → `cho-cell-culture-media`
- "Bioprocessing Solutions Overview" → `bioprocessing-solutions-overview`
- "mRNA Vaccine Production" → `mrna-vaccine-production`

**Command:**
```bash
mkdir -p "./Briefs/<folder-name>"
```

The `-p` flag ensures parent directories exist and doesn't error if folder already exists.

---

### B. Generate Filename

Create a descriptive filename for the content brief:

**Filename format:** `content-brief.md`

This keeps the naming simple and consistent across all page folders.

---

### C. Save Content Brief

Write the generated content brief from Step 7 to the file:

**Full file path:**
```
./Briefs/<folder-name>/content-brief.md
```

**Content:** The complete content brief output from Step 7, including:
- Page metadata (name, client, keywords, level)
- Target word count range
- Content goal
- Meta description
- Headline structure
- Internal linking opportunities
- Notes section

---

### D. Verify File Creation

After saving, confirm the file was created successfully:

**Verification command:**
```bash
ls -lh "./Briefs/<folder-name>/content-brief.md"
```

This displays file size and confirms successful creation.

---

## Output Format

After successful save, display:

```
=== CONTENT BRIEF SAVED ===

Folder: ./Briefs/<folder-name>/
File: content-brief.md
Full path: ./Briefs/<folder-name>/content-brief.md

Status: ✓ Successfully saved

---

The content brief is now ready for the content writer to access.
```

---

## Error Handling

**Directory creation fails:**
- Check parent directory exists: `./Briefs`
- Verify write permissions on parent directory
- If Briefs folder doesn't exist, create it first: `mkdir -p ./Briefs`
- If error persists, output: "Unable to create folder - manual creation needed"

**File write fails:**
- Check folder was created successfully
- Verify write permissions on folder
- If error persists, output: "Unable to save file - manual save needed"
- Display the content brief so user can manually copy it

**Folder already exists:**
- This is OK - the `-p` flag handles this gracefully
- Existing `content-brief.md` will be overwritten with new content
- Note in output: "Folder exists - content brief updated"

---

## Quality Checks

Before completing, verify:

- [ ] Folder name follows naming convention (lowercase, hyphens, no special chars)
- [ ] Folder created at correct path: `./Briefs/<folder-name>/`
- [ ] File saved with correct name: `content-brief.md`
- [ ] File contains complete content brief from Step 7
- [ ] File creation verified with ls command
- [ ] Success message displayed to user

---

## Example Execution

**Given:**
- Page Name: "CHO Cell Culture Media"

**Steps:**

1. **Create folder:**
```bash
mkdir -p "./Briefs/cho-cell-culture-media"
```

2. **Save content brief to file:**
```
./Briefs/cho-cell-culture-media/content-brief.md
```

3. **Verify:**
```bash
ls -lh "./Briefs/cho-cell-culture-media/content-brief.md"
```

4. **Output:**
```
=== CONTENT BRIEF SAVED ===

Folder: ./Briefs/cho-cell-culture-media/
File: content-brief.md
Full path: ./Briefs/cho-cell-culture-media/content-brief.md

Status: ✓ Successfully saved

---

The content brief is now ready for the content writer to access.
```

---

## Next Step

Proceed to [Step 8: Add Writing Instructions Under Each Headline](step-8-add-instructions.md) to generate context and guidance for the content writer.
