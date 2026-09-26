# OLV PSR3 - Our Lady of Victory Parish School of Religion (Grade 3)

## Overview

Data layer and planning system for 3rd grade PSR (Parish School of Religion) at **Our Lady of Victory Parish** in Columbus, Ohio. Helps Nick prepare lessons, synthesize materials, and retain planning across years.

## Where I Am: Year 2 (2026-2027)

As of **September 26, 2026**, Nick is starting his **second year** teaching this class. First class is **Sunday, September 27, 2026**. Same curriculum, same book — much of Year 1 (2025-2026) should be reusable.

**Default workflow for any Year 2 session:** check the reuse map below first. If Year 1 material exists, start from it and refine (what worked, what to cut, what to add) rather than rebuilding. Only build from the raw planner/book when the "Year 1 material" column is empty. After each class, log it in the Year 2 Teaching Log.

Full syllabus transcription (logistics, pageant, reconciliation, standing instructions): `datalayer/syllabus_2026_2027.md`. Photos: `datalayer/rawdata/syllabus_2026-2027_p*.jpg`.

### Year 2 schedule → Year 1 reuse map

| Date | Year 2 content (per coordinator syllabus) | Year 1 material to reuse |
|------|-------------------------------------------|--------------------------|
| Sep 27 | Unit 1 Opener (St. Ignatius) + Session 1 Created to Be Happy | **None built** — raw planner only (`rawdata/..._Session_1_GP.docx`) |
| Oct 4 | Session 2 Created to Be Together | `session2_3_lesson_plan.md` (taught 2+3 together in Y1) + Trinity coloring |
| Oct 11 | Session 3 God is our Father | `session2_3_lesson_plan.md` |
| Oct 25 | Sessions 4 + 5 (Jesus is with Us, Ordinary Time) | `session4_5_lesson_plan.md` — same pairing as Y1 + Joseph coloring |
| Nov 1 | All Saints / All Souls pp. 237-240 | None |
| Nov 8 | Session 10 Celebrating Advent | Raw planner + `rawdata/session10quiz.pdf` only |
| Nov 15 | Session 14 Mary is Holy | None |
| Nov 22 | Session 15 Celebrating Christmas | None |
| Dec 6 | Christmas Play | — |
| Jan 10 | Baptism of the Lord + Session 16 Sacraments of Initiation + chalk blessing | Raw Unit 4 planner/worksheets only (`lesson16.yaml` is empty) |
| Jan 24 | Session 18 Celebrating Jesus + Celebrating the Lord's Day pp. 254-259 | Raw Unit 4 planner only |
| Jan 31 | Session 17 Reconciliation + Session 22 Making Good Choices | Raw Unit 4 planner (17) only |
| Feb 7 | Reconciliation in church + The Bible and You | None |
| Feb 21 | Session 20 Lent and Holy Week + Lent pp. 221-224 | `lesson20.yaml`, `lesson20_session_prompt.md`, `rawdata/lesson20bookscan.pdf` (built Feb 2026; not in Y1 teaching log) |
| Feb 28 | Session 8 + Session 23 | `session8_23_lesson_plan.md` — same pairing as Y1 + workbook scans |
| Mar 14 | Session 25 Easter + Last Supper pages + Session 9 | `lesson25.yaml`, `session25_easter_jeopardy.md`; `lesson9.yaml`, `session9_13_lesson_plan.md`, `session9_13_jeopardy.md` |
| Apr 11 | All Life is Sacred pp. 197-204 (Session 24) | Raw planner only (`..._Session_24.docx`) |
| Apr 18 | Holy Spirit + Pentecost pp. 233-236 | `session_11_data_layer.md` — ⚠️ syllabus says "Session 12, pp. 97-104"; Y1 book data says Session 11, pp. 89-96. Verify. |
| Apr 25 | Last day / fun / food drive | `final_year_review_jeopardy.md` |

No class: Oct 18, Nov 29, Dec 13–Jan 3, Jan 17, Feb 14, Mar 7, Mar 21–Apr 4.

**Year 1 material not on this year's syllabus** (available if a slot opens): Session 13 The Church Prays (`lesson13.yaml`), Session 19 Christian Living (`lesson19.yaml`), Stations of the Cross (`stations_of_the_cross.yaml`, `stations_session19_*`), Carlo Acutis coloring.

### Year 2 Teaching Log (2026-2027)

| Date | Sessions | Lesson Plan File | Reused from Y1? / Notes |
|------|----------|------------------|-------------------------|
| | | | |

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
│   ├── session*_lesson_plan.md / *_jeopardy.md   # Year 1 lesson plans + review games
│   ├── syllabus_2026_2027.md  # Year 2 coordinator syllabus (transcribed)
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

## Year 1 Teaching History (2025-2026)

| Date | Sessions | Lesson Plan File |
|------|----------|------------------|
| September 28, 2025 | Session 2: Created to Be Together + Session 3: God is our Father | `datalayer/session2_3_lesson_plan.md` |
| October 5, 2025 | Session 4: Jesus is with us + Session 5: Ordinary Time | `datalayer/session4_5_lesson_plan.md` |
| January 25, 2026 | Session 8: Jesus Gathers Disciples + Session 23: Fear Not | `datalayer/session8_23_lesson_plan.md` |
| February 22, 2026 | Session 9: Jesus Dies and Rises + Session 13: The Church Prays | `datalayer/session9_13_lesson_plan.md` |
| March 8, 2026 | Stations of the Cross + Session 19: Christian Living | `datalayer/stations_session19_lesson_plan.md` |
| ~March 2026 (date not recorded) | Session 25: Celebrating Easter (Jeopardy) | `datalayer/lesson25.yaml`, `datalayer/session25_easter_jeopardy.md` |
| ~April 19, 2026 (inferred from file date) | Session 11: Jesus Sends the Holy Spirit + Pentecost | `datalayer/session_11_data_layer.md` |
| ~April 26, 2026 (inferred from file date) | Last class: year-end review Jeopardy | `datalayer/final_year_review_jeopardy.md` |

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
