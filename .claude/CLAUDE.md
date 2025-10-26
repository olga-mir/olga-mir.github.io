# Project-Specific Instructions for olga-mir.github.io

This is a GitHub Pages portfolio website showcasing public speaking engagements.

## Project Structure

- `README.md` - Main landing page with chronological list of all speaking engagements
- `Public-Speaking/` - Contains subdirectories for each conference/talk
  - Naming convention: `YYYY.MM.DD__Event-Name__Topic/`
  - Each folder contains:
    - `README.md` - Conference description, abstract, and links
    - PDF and PPTX slide files
    - Optional `img/` folder for photos

## When Adding New Conferences

1. **Folder naming**: Follow the pattern `YYYY.MM.DD__Event-Name__Topic/`
   - Use actual presentation date (not conference start date)
   - Use double underscores `__` as separators
   - Keep topic name concise but descriptive

2. **Required files**:
   - `README.md` with:
     - Conference title (h1)
     - Description/abstract (1-2 paragraphs)
     - Conference website links
     - Slides section with PDF and PPTX download links
     - Optional Photos section
   - PDF and PPTX slide files

3. **Update main README.md**:
   - Add entry under appropriate year section
   - Format: `### [Talk Title](./Public-Speaking/folder-name/) (Month YYYY)`
   - Include Event and Topics metadata
   - Maintain reverse chronological order (newest first)

## Content Guidelines

- Use Kubernetes, GKE, EKS (not k8s in formal content)
- Focus on platform engineering, SRE, and cloud-native topics
- When adding abstracts, maintain professional technical tone
- Photo references should use correct file extensions (check actual files)

## Common Tasks

- When fixing broken images: verify actual file extensions match markdown references
- When updating old pages: ensure they have title, description, and proper formatting
- Photos are typically stored in `img/` subfolder within each conference folder
