# LLM “Deep Fake” Interview Project

> **One-minute AI reporter video** summarizing Syracuse Women’s Lacrosse performance using verified stats and Task 05 analysis. Generated with **HeyGen** (avatar presenter) and cross-checked with **NotebookLM** (upload: *2025 Syracuse University Lacrosse Statistics*).

---

## 1. Background
In earlier periods (Task 05), I built data summaries from a **32-player** Syracuse Women’s Lacrosse dataset (G, A, SH, SH%, SOG%, GB, CT, DC, Fouls, GP–GS) and validated insights with Python.  
This period extends that narrative into an **AI “deep fake” interview**—a broadcast-style stand-up where a reporter explains the key findings on camera.  
To keep the video **data-grounded**, I reused numbers from **SU_RA_Task_05_Descriptive_Stats** and cross-referenced wording with **NotebookLM** (source: *2025 Syracuse University Lacrosse Statistics*).

---

## 2. Process
1. **Lock ground truth** from Task 05 and dataset:
   - Top goals: **Emma Muchnick — 34 G**  
   - Most assists & total contribution: **Emma Ward — 46 A; 76 (G+A)**  
   - Per-game standout: **Olivia Adamson — 10 G, 6 A in 3 GP (~3.33 GPG; ~5.33 contrib/game)**  
   - Accuracy leaders: **Mackenzie Rich — 100% SH%**, **Bri Peters — 100% SOG%**  
   - GB leader: **Kaci Benoit — 34 GB**  
   - Top defensive impact (GB+CT+DC): **Meghan Rode — 76**  
   - Shots ↔ Goals correlation: **r ≈ 0.99**
2. **Write the on-air script** (stadium stand-up; short lines; numeric callouts).
3. **Generate video in HeyGen** (script → avatar; 16:9; subtitles; light music).
4. **Review & trim** (timing, overlays, lip-sync, stat alignment).
5. **Export MP4** and store the **public share link**.
6. **Document** everything here for reproducibility.

---

## 3. Tools Explored
- **HeyGen** — text/script → human presenter video (used for final export).
- **NotebookLM** — summarized and cross-checked phrasing against *2025 Syracuse University Lacrosse Statistics*.
- *(Considered for future)* Colossyan (two-presenter scenes), Lumen5/Kapwing (prompt→b-roll montage).

---

## 4. Workflow Strategy
- **Data-first**: never invent numbers; reuse Task 05 outputs.  
- **Broadcast craft**: 1–2 sentences per beat; **big numeric overlays**; subtitles on.  
- **Design system**: 16:9, high-contrast captions, accent **#F76900** for numbers.  
- **Auditability**: keep script + sources + video together; note tool settings.  
- **Disclosure**: tag as **“AI-generated interview.”**

---

## 5. Reflections
- **What worked**: concise script reads naturally; numeric badges clarify takeaways; NotebookLM prevented wording drift.  
- **To improve**: try a **two-human interview** (Reporter + Analyst), add **b-roll charts** (scatter for *r ≈ 0.99*), export an **SRT** caption file for accessibility.  
- **Lesson**: credible “deep fake” storytelling requires **LLM narration + verified analytics**.

---

## 6. Outputs
- **Final Video (HeyGen)**  
  - Video link: https://app.heygen.com/videos/5b77a0288e224ec19ff78bb86d8906e1
- **NotebookLM**
  - Video link: https://notebooklm.google.com/notebook/ba46a835-ace6-4902-9b6d-4cf337e63cab?artifactId=de7b97ff-66c7-4939-a79f-8a50eacad222
- **Script Used (Reporter stand-up, ~60s)**

Live from the dome, we’re spotlighting Syracuse women’s lacrosse through the lens of data.
Our dataset covers 32 players with goals, assists, shots and shooting rates, shots-on-goal,
ground balls, caused turnovers, draw controls, fouls, and GP–GS.Up front, the headline is finishing. Emma Muchnick led scoring with 34 goals.
Playmaking? That’s Emma Ward—46 assists and a team-high 76 combined goals plus assists.Per-game impact belongs to Olivia Adamson: 10 goals, 6 assists in just 3 games—
about 3.33 goals per game and 5.33 contributions per game. Limited minutes, massive returns.Accuracy leaders: Mackenzie Rich hit a perfect 100% shooting,
and Bri Peters delivered 100% shots-on-goal—every attempt on frame.Possession and defense matter too. Kaci Benoit owned the ground game with 34 ground balls,
while Meghan Rode posted the top defensive impact at 76 using GB plus CT plus DC.And the big trend: shots strongly predict goals—correlation around 0.99.
Volume matters, but paired with efficiency, it wins you games.For Syracuse, the numbers tell a clear story—finishers, creators, and ball-winners driving results.
Full breakdown and code are linked in the description.


- **Data & Arifacts**
- Task 05 notebook/code: `playerperformance.ipynb`, `data/Player_Stats.csv`
- LLM prompt history: `LLMResponses.docx`
- NotebookLM source: *2025 Syracuse University Lacrosse Statistics* (uploaded)

---

## 7. Conclusion
This project shows how to **convert verified analytics into an on-camera AI interview**. Grounding the script in Task 05 outputs and validating phrasing with NotebookLM produced a video that’s both **engaging and trustworthy**.  
**Next steps**: two-presenter stadium interview, b-roll data charts, SRT captions, and prompt A/B tests for different broadcast tones.

---

### Repro Steps (Quick)
1. Confirm stats from Task 05 / source doc.  
2. Paste script into **HeyGen** → choose presenter + stadium background → subtitles on.  
3. Generate, review pacing/overlays, and **export 16:9 MP4**.  
4. Add the **share link** and files to the repo.  
5. Keep this README, script, and data together for traceability.

---
