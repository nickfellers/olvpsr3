# OLV PSR3 - Our Lady of Victory Parish School of Religion (Grade 3)

## Overview

Data layer and planning system for 3rd grade PSR (Parish School of Religion) at **Our Lady of Victory Parish** in Columbus, Ohio. Helps Nick prepare lessons, synthesize materials, and retain planning across years.

## Curriculum

- **Program:** Finding God: Our Response to God's Gifts, Grade 3
- **Publisher:** Loyola Press
- **Guide:** Parish Catechist Guide
- **Digital Library:** https://digitallibrary.loyolapress.com/
- **Access Code:** `76D27B80`

## Project Structure

```
OLVpsr3/
├── CLAUDE.md              # This file - project context
├── datalayer/
│   ├── *.yaml             # Cleaned/structured lesson data (e.g., lesson16.yaml)
│   └── rawdata/           # Raw source documents
│       ├── *.docx         # Loyola Press interactive lesson planners
│       ├── *.pdf          # Worksheets, quizzes, workbook scans
│       └── (scans)        # Pages from physical workbook/guide
```

## Data Layer Purpose

The `datalayer/` folder serves as a **reusable knowledge base**:

1. **Raw data** (`rawdata/`) - Source materials downloaded from Loyola Press or scanned from the physical catechist guide and student workbook
2. **Cleaned data** (YAML files in `datalayer/`) - Structured lesson content extracted from raw sources, ready for synthesis and planning

This structure enables:
- Repeated use across years (same curriculum, refined approach)
- AI-assisted lesson planning and synthesis
- Consistent formatting for cross-lesson analysis

## Raw Data Sources

- **Interactive Lesson Planners** (`.docx`) - Session-by-session plans from Loyola Press (Finding God 2021 edition)
- **Reproducible Worksheets** (`.pdf`) - Student activity sheets by unit
- **Quizzes** (`.pdf`) - Session assessments
- **Workbook scans** - Pages from the physical student workbook

## YAML Data Format

Cleaned lesson files follow the pattern `lesson{N}.yaml`. Structure should capture:
- Session number and title
- Scripture references
- Key concepts and vocabulary
- Activities and discussion questions
- Prayer focus
- Take-home/family connection points

## Teaching History (2025-2026)

| Date | Sessions | Lesson Plan File |
|------|----------|------------------|
| September 28, 2025 | Session 2: Created to Be Together + Session 3: God is our Father | `datalayer/session2_3_lesson_plan.md` |
| October 5, 2025 | Session 4: Jesus is with us + Session 5: Ordinary Time | `datalayer/session4_5_lesson_plan.md` |
| January 25, 2026 | Session 8: Jesus Gathers Disciples + Session 23: Fear Not | `datalayer/session8_23_lesson_plan.md` |
| February 22, 2026 | Session 9: Jesus Dies and Rises + Session 13: The Church Prays | `datalayer/session9_13_lesson_plan.md` |
| March 8, 2026 | Stations of the Cross + Session 19: Christian Living | `datalayer/stations_session19_lesson_plan.md` |

### Activity Resources

| Session | Activity | Link |
|---------|----------|------|
| Session 2/3 | Holy Trinity stained glass coloring | [Canva](https://www.canva.com/design/DAG0FaFqfTs/mgzT2OMhQVnHqoTdgohNJg/view) |
| Session 4/5 | Joseph Trusted God coloring | [Canva](https://www.canva.com/design/DAG02T0vyFU/zwUV1aWsC81hJAd5XhKpYA/view) |
| Session 13 | Saint Carlo Acutis coloring sheet | [Gemini](https://gemini.google.com/app/39451c73f7e275ca) |

## Working With This Project

- When processing raw `.docx` or `.pdf` files, extract structured content into YAML format
- When planning a lesson, pull from both the cleaned YAML and any available raw materials
- Digital library resources at Loyola Press supplement what's stored locally
- The catechist guide (physical book) is the primary teaching reference
