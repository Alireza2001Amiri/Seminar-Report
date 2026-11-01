# Strict thesis editorial audit — Persian and English

Source: `main(10).pdf` — 180 A4 PDF pages; printed main-text page generally equals PDF page minus 16.

This is an evidence-based defect register, **not a certification of error-free Persian copy**. PDF text extraction has corrupted Persian Unicode mappings, so many native-line writing checks require the LaTeX/Word source. Visual sample/overview and full bibliography inspection were used. All bibliography items below are verifiable locations; for language problems, confirm original publication title before changing a quoted article title.

**Total registered findings:** 118 (47 Must fix; 71 Should fix). In addition, the complete source should be proofread word-by-word for Persian grammar and zero-width joiners.

**Location convention:** PDF page = one-based physical page. “PDF text line” = one-based line of extracted PDF text (not typesetting source line); exact quoted fragment/reference number anchors the finding where RTL extraction is unstable. Figure entries use figure numbers instead of invented source-code line numbers.

## Priority corrections

- **E-032:** PDF p. 165, Ref. [66]: Reference contains "Bibliographic metadata reconstructed from the corresponding Obsidian paper note."
- **E-031:** PDF p. 165, Ref. [64]: Multiple authors are inverted into nonsensical fields: "CMM, van Lierop, JW, Jansen ... AJA, Vandenput".
- **E-017:** PDF p. 168, References — final page: References page carries the Chapter 5 running header rather than a References header.
- **E-003:** PDF p. 180, English cover — supervisor: No space after title abbreviation.
- **E-001:** PDF p. 180, English title: Missing indefinite article before the singular count-noun phrase "magnetically levitated planar motor system".
- **E-026:** PDF p. 159, Ref. [3]: The page interval contains two en dashes: "114––117".
- **E-034:** PDF p. 159, Ref. [5]: "Thesis, [year]" does not identify awarding institution or degree; reader cannot reliably retrieve work.
- **E-035:** PDF p. 160, Ref. [11]: "Thesis, [year]" does not identify awarding institution or degree; reader cannot reliably retrieve work.
- **E-036:** PDF p. 160, Ref. [12]: "Thesis, [year]" does not identify awarding institution or degree; reader cannot reliably retrieve work.
- **E-037:** PDF p. 165, Ref. [71]: Entry contains author, title, and year only; thesis/report type and awarding institution are missing.
- **E-015:** PDF p. 101, Chapter 3 — final lines of §3.14: Only two lines of body text appear on an otherwise empty final chapter page. The following page is blank to start Chapter 4 on the next recto.
- **E-016:** PDF p. 149, Chapter 4 — final paragraph of §4.8: A three-line continuation occupies an otherwise empty final chapter page, followed by a blank verso.
- **E-022:** PDF p. 129, §4.4.2 / model comparison — Figure 4.23: Eighteen heat-map panels and colorbars on one A4 page; axis and colorbar numerals are close to illegible at normal print size.

## Full location-specific defect register

### E-001 — Must fix — Academic English

**Address:** English back matter; English title; PDF p. 180; printed p. —; PDF-text line 6.

**Source anchor:** Design and Implementation of a Simulator for Magnetically Levitated Planar Motor System

**Fault:** Missing indefinite article before the singular count-noun phrase "magnetically levitated planar motor system".

**Correction:** Design and Implementation of a Simulator for a Magnetically Levitated Planar Motor System

### E-002 — Must fix — Punctuation / spacing

**Address:** English back matter; English cover — faculty affiliation; PDF p. 180; printed p. —; PDF-text line 2.

**Source anchor:** Faculty of Electrical Engineering- Mechatronics Group

**Fault:** Hyphen has no space before it and a space after it; dash used inconsistently as departmental separator.

**Correction:** Use an en dash with surrounding spaces: Faculty of Electrical Engineering – Mechatronics Group; confirm the official unit name.

### E-003 — Must fix — Punctuation / spacing

**Address:** English back matter; English cover — supervisor; PDF p. 180; printed p. —; PDF-text line 12.

**Source anchor:** Dr.Mahdi Aliyari Shooredeli

**Fault:** No space after title abbreviation.

**Correction:** Dr. Mahdi Aliyari Shooredeli

### E-004 — Should fix — PDF metadata

**Address:** PDF metadata; Document properties — Author; PDF p. Metadata; printed p. —; PDF-text line Metadata field.

**Source anchor:** AlirezaAmiri

**Fault:** Author metadata concatenates the given name and surname.

**Correction:** Set PDF /Author to "Alireza Amiri".

### E-005 — Should fix — PDF text layer

**Address:** Front matter; University and faculty text; PDF p. 1; printed p. —; PDF-text line 1–2.

**Source anchor:** Text extraction contains non-Persian script characters in the Persian university/faculty lines

**Fault:** PDF glyph-to-Unicode mapping is corrupt in the first two cover lines; screen readers and copy/paste will output unrelated characters. The visible print rendering is not the error.

**Correction:** Regenerate/re-embed Persian font ToUnicode mappings and validate copied text and full-text search; do not replace the visible institution name.

### E-006 — Should fix — PDF text layer

**Address:** Front matter; Persian abstract; PDF p. 3; printed p. —; PDF-text line 2–16.

**Source anchor:** Visible Persian words become presentation forms/concatenated tokens when extracted

**Fault:** Machine-readable Persian text has unstable word spacing and presentation-form encoding; a high-fidelity digital thesis should allow clean copying, searching and accessibility.

**Correction:** Test full-text extraction/search for Arabic-script content after rebuilding PDF with correct text-layer/ToUnicode mappings.

### E-007 — Should fix — Persian orthography

**Address:** Front matter; Persian cover; PDF p. 1; printed p. —; PDF-text line 6.

**Source anchor:** پیاده سازی

**Fault:** Full word-space used where Persian standard typography normally requires a half-space (ZWNJ): compound word.

**Correction:** Use «پیاده‌سازی» and apply the same orthographic convention in the body and the table of contents.

**Qualification:** Visually verified; check source ZWNJ encoding

### E-008 — Should fix — Persian orthography

**Address:** Front matter; Persian cover; PDF p. 1; printed p. —; PDF-text line 6.

**Source anchor:** شبیه ساز

**Fault:** Full word-space used where Persian standard typography normally requires a half-space (ZWNJ): compound word.

**Correction:** Use «شبیه‌ساز» and apply the same orthographic convention in the body and the table of contents.

**Qualification:** Visually verified; check source ZWNJ encoding

### E-009 — Should fix — Persian orthography

**Address:** Front matter; Persian cover; PDF p. 1; printed p. —; PDF-text line 7.

**Source anchor:** صفحه ای

**Fault:** Full word-space used where Persian standard typography normally requires a half-space (ZWNJ): compound adjective.

**Correction:** Use «صفحه‌ای» and apply the same orthographic convention in the body and the table of contents.

**Qualification:** Visually verified; check source ZWNJ encoding

### E-010 — Should fix — Persian orthography

**Address:** Front matter; Persian cover; PDF p. 1; printed p. —; PDF-text line 3.

**Source anchor:** پایان نامه

**Fault:** Full word-space used where Persian standard typography normally requires a half-space (ZWNJ): compound word.

**Correction:** Use «پایان‌نامه» and apply the same orthographic convention in the body and the table of contents.

**Qualification:** Visually verified; check source ZWNJ encoding

### E-011 — Should fix — Persian terminology

**Address:** Front matter; Abstract; PDF p. 3; printed p. —; PDF-text line 3.

**Source anchor:** اجرای جریان

**Fault:** "اجرای جریان" is less idiomatic than "اعمال جریان" for electrical current; the expression is repeated near the end of the abstract.

**Correction:** Use «اعمال جریان» if the intended meaning is actuation by current; align wording across Persian abstract and Chapter 3.

**Qualification:** Editorial suggestion

### E-012 — Should fix — Keyword formatting

**Address:** English back matter; English abstract — Keywords; PDF p. 178; printed p. —; PDF-text line 24.

**Source anchor:** Keywords    Magnetically levitated planar motor, ...

**Fault:** Keyword label has no punctuation separator from the keywords, unlike most formal English thesis styles; acceptable only if prescribed by template.

**Correction:** If the university guide does not prescribe this layout, use "Keywords:" and a consistent hanging or separate-line style.

**Qualification:** Style-dependent

### E-013 — Should fix — Cross-document terminology

**Address:** Front matter; Table of contents — §4.1 and §3.4.2; PDF p. 9; printed p. —; PDF-text line 17.

**Source anchor:** کنترلر / کنترل‌کننده

**Fault:** The text alternates between synonymous but stylistically different controller terms in formal headings.

**Correction:** Choose «کنترل‌کننده» or «کنترلر» for section titles and running text, except fixed source titles.

**Qualification:** Style-dependent

### E-014 — Should fix — Cross-document terminology

**Address:** Front matter; Table of contents — §3.12 and Fig. 3.15 listing; PDF p. 9; printed p. —; PDF-text line 14.

**Source anchor:** رابط کاربر / رابط کاربری

**Fault:** UI terminology is inconsistent between section title and figure caption.

**Correction:** Standardize on «رابط کاربری» unless specific technical distinction is intended.

**Qualification:** Style-dependent

### E-015 — Should fix — Pagination

**Address:** Ch. 3; Chapter 3 — final lines of §3.14; PDF p. 101; printed p. 85; PDF-text line 2.

**Source anchor:** فیزیکی. هرجا داده‌ی حلقه‌بسته‌ی فیزیکی موجود نباشد ...

**Fault:** Only two lines of body text appear on an otherwise empty final chapter page. The following page is blank to start Chapter 4 on the next recto.

**Correction:** Adjust preceding paragraph/section spacing or copyfit slightly so the two lines fit on PDF p.100, without changing legitimate recto chapter starts.

### E-016 — Should fix — Pagination

**Address:** Ch. 4; Chapter 4 — final paragraph of §4.8; PDF p. 149; printed p. 133; PDF-text line 2.

**Source anchor:** این نتایج در کنار ارزیابی مرجع شبیه‌سازی ...

**Fault:** A three-line continuation occupies an otherwise empty final chapter page, followed by a blank verso.

**Correction:** Avoid the runover by copyfitting the final section on p.148 or restructuring the preceding page without degrading typography.

### E-017 — Must fix — Running header

**Address:** References; References — final page; PDF p. 168; printed p. 152; PDF-text line 1.

**Source anchor:** فصل ۵: نتیجه‌گیری و پیشنهادها

**Fault:** References page carries the Chapter 5 running header rather than a References header.

**Correction:** Set bibliography running mark to «مراجع» (or omit the header consistently throughout bibliography).

### E-018 — Should fix — Bibliography pagination

**Address:** References; References — Ref. [81] continued on PDF p.167; PDF p. 166; printed p. 150; PDF-text line 30.

**Source anchor:** [81] ... based on beetle / algorithm. in 2024 ...

**Fault:** A single bibliography entry is split across pages 166–167, leaving a mid-sentence fragment at the start of the next page.

**Correction:** Use a keep-together policy for bibliography entries (e.g., \interlinepenalty or appropriate bibliography-environment setting) while preventing large page gaps.

### E-019 — Should fix — Figure legibility / layout

**Address:** Ch. 3; §3.2 / simulation architecture — Figure 3.1; PDF p. 63; printed p. 47; PDF-text line figure and caption.

**Source anchor:** Figure 3.1

**Fault:** Diagram and caption are rotated 90° while the PDF page stays portrait; labels are very small in upright print view.

**Correction:** Make the page a properly tagged/oriented landscape page or redraw the diagram at a readable scale; keep caption orientation consistent.

### E-020 — Should fix — Figure legibility / layout

**Address:** Ch. 3; §3.6 / physical prototype flow — Figure 3.7; PDF p. 81; printed p. 65; PDF-text line figure and caption.

**Source anchor:** Figure 3.7

**Fault:** Repeated rotated full-page diagram with small labels; not directly readable without physically rotating the page.

**Correction:** Use a true landscape page and larger diagram typography, avoiding screenshots embedded in the architecture at unreadable size.

### E-021 — Should fix — Figure legibility / layout

**Address:** Ch. 4; §4.1.5 / wrench outputs — Figure 4.9; PDF p. 113; printed p. 97; PDF-text line figure and caption.

**Source anchor:** Figure 4.9

**Fault:** Twelve narrow subplots; tick labels, legends and units are too small relative to thesis body text.

**Correction:** Enlarge axes type and split into multiple larger figures or move supplementary panels to an appendix.

### E-022 — Should fix — Figure legibility / layout

**Address:** Ch. 4; §4.4.2 / model comparison — Figure 4.23; PDF p. 129; printed p. 113; PDF-text line figure and caption.

**Source anchor:** Figure 4.23

**Fault:** Eighteen heat-map panels and colorbars on one A4 page; axis and colorbar numerals are close to illegible at normal print size.

**Correction:** Split force and torque matrices, enlarge panels, and use consistent accessible label size.

### E-023 — Should fix — Figure legibility / layout

**Address:** Ch. 4; §4.5.1 / sensor noise — Figure 4.24; PDF p. 131; printed p. 115; PDF-text line figure and caption.

**Source anchor:** Figure 4.24

**Fault:** Multiple dense noise plots, tiny annotations and axes.

**Correction:** Increase panel/label size or separate distributions from time-series plots.

### E-024 — Should fix — Figure legibility / layout

**Address:** Ch. 4; §4.6.7 / six-coordinate test — Figure 4.34; PDF p. 143; printed p. 127; PDF-text line figure and caption.

**Source anchor:** Figure 4.34

**Fault:** Twelve panels on one page; labels and the small English plot titles are materially smaller than surrounding text.

**Correction:** Regenerate vector plots at the intended print size, with larger labels, matching notation and readable legends.

### E-025 — Should fix — Figure legibility / layout

**Address:** Ch. 4; §4.6.7 / current allocation — Figure 4.35; PDF p. 144; printed p. 128; PDF-text line figure and caption.

**Source anchor:** Figure 4.35

**Fault:** Grouped six-coordinate plots have small axis labels and legends at print size.

**Correction:** Increase plot fonts, label size and line/key readability; split panels if necessary.

### E-026 — Must fix — Number range punctuation

**Address:** References; Ref. [3]; PDF p. 159; printed p. 143; PDF-text line 10 (entry begins at 9 on PDF p. 159).

**Source anchor:** Browne, Jim J, Dubois, Didier, Rathmill, Keith, Sethi, Suresh, and Stecke, Kathrin. Classifi- cation of flexible manufacturing systems. The FMS magazine, 2(2):114––117, 1984.

**Fault:** The page interval contains two en dashes: "114––117".

**Correction:** Replace with the single range dash "114–117".

### E-027 — Must fix — Bibliographic punctuation

**Address:** References; Ref. [5]; PDF p. 159; printed p. 143; PDF-text line 14 (entry begins at 14 on PDF p. 159).

**Source anchor:** Jansen, J. W. Magnetically levitated planar actuator with moving magnets : electromechan- ical analysis and design. Thesis, 2007.

**Fault:** Unwanted space before colon in article/thesis title: "magnets : electromechanical".

**Correction:** Use "magnets: electromechanical" unless source title differs.

### E-028 — Must fix — Bibliographic punctuation

**Address:** References; Ref. [12]; PDF p. 160; printed p. 144; PDF-text line 11 (entry begins at 10 on PDF p. 160).

**Source anchor:** Mao, Simone. Studio dinamico di una catenaria a passo e valutazione dell’introduzione di motori planari a levitazione magnetica= Study on the dynamics of a catenary conveyor and evaluation o…

**Fault:** Bilingual title uses a bare equals sign glued to Italian title ("magnetica= Study").

**Correction:** Format translation with a clean separator according to citation style (e.g., space-colon-space or square brackets). Verify title exactness.

### E-029 — Must fix — Author presentation

**Address:** References; Ref. [30]; PDF p. 162; printed p. 146; PDF-text line 1 (entry begins at 1 on PDF p. 162).

**Source anchor:** Jeroen de Boeij, Elena Lomonova and Vandenput, Andr´e J.A. Look-up table based real- time commutation of 6-dof planar actuators. 16th IEEE International Conference on Control Applications Pa…

**Fault:** Entry mixes direct-name ordering with surname-first ordering, including "Jeroen de Boeij, Elena Lomonova and Vandenput, André".

**Correction:** Rewrite all authors in the same citation style, ensuring particles and accents are represented correctly.

### E-030 — Should fix — Unicode / diacritics

**Address:** References; Ref. [30]; PDF p. 162; printed p. 146; PDF-text line 1 (entry begins at 1 on PDF p. 162).

**Source anchor:** Jeroen de Boeij, Elena Lomonova and Vandenput, Andr´e J.A. Look-up table based real- time commutation of 6-dof planar actuators. 16th IEEE International Conference on Control Applications Pa…

**Fault:** The accented first name is extracted as "Andr´e", indicating an incorrectly encoded diacritic.

**Correction:** Re-enter name as Unicode "André" (or a correct LaTeX accent command), and verify rendering and copy/paste.

### E-031 — Must fix — Bibliography author parsing

**Address:** References; Ref. [64]; PDF p. 165; printed p. 149; PDF-text line 7 (entry begins at 7 on PDF p. 165).

**Source anchor:** CMM, van Lierop, JW, Jansen, EA, Lomonova, AAH, Damen, PPJ, van den Bosch, and AJA, Vandenput. Commutation of a magnetically levitated planar actuator with moving-magnets. IEEJ Transactions …

**Fault:** Multiple authors are inverted into nonsensical fields: "CMM, van Lierop, JW, Jansen ... AJA, Vandenput".

**Correction:** Repair original BibTeX/CSL author metadata using family names and properly punctuated initials; regenerate the entry.

### E-032 — Must fix — Working-note leakage

**Address:** References; Ref. [66]; PDF p. 165; printed p. 149; PDF-text line 14 (entry begins at 13 on PDF p. 165).

**Source anchor:** Xu, Zhiyuan, Gu, Yajie, Xu, Rongqing, and Qin, Yaohong. Design, implementation, and control of a maglev planar motor with 6-dof current-sharing, 2024. Bibliographic metadata reconstructed fr…

**Fault:** Reference contains "Bibliographic metadata reconstructed from the corresponding Obsidian paper note."

**Correction:** Delete the internal source-management note. Verify complete bibliographic metadata against the original publication before submission.

### E-033 — Must fix — Reference completeness

**Address:** References; Ref. [16]; PDF p. 160; printed p. 144; PDF-text line 23 (entry begins at 23 on PDF p. 160).

**Source anchor:** Pelta, Edmond R. Two-axis sawyer motor for motion systems. 1987.

**Fault:** Citation consists only of author, title and 1987; publication medium and bibliographic identification are absent.

**Correction:** Supply actual patent/report/publication type, organization or identifier, and year after verification.

### E-034 — Must fix — Reference completeness

**Address:** References; Ref. [5]; PDF p. 159; printed p. 143; PDF-text line 15 (entry begins at 14 on PDF p. 159).

**Source anchor:** Jansen, J. W. Magnetically levitated planar actuator with moving magnets : electromechan- ical analysis and design. Thesis, 2007.

**Fault:** "Thesis, [year]" does not identify awarding institution or degree; reader cannot reliably retrieve work.

**Correction:** Supply thesis type/degree, university, repository/identifier where appropriate; preserve standard bibliography formatting.

### E-035 — Must fix — Reference completeness

**Address:** References; Ref. [11]; PDF p. 160; printed p. 144; PDF-text line 8 (entry begins at 8 on PDF p. 160).

**Source anchor:** Stewart, Curtis. Implementation of a Modular Magnetic Levitation Planar Motor. Thesis, 2023.

**Fault:** "Thesis, [year]" does not identify awarding institution or degree; reader cannot reliably retrieve work.

**Correction:** Supply thesis type/degree, university, repository/identifier where appropriate; preserve standard bibliography formatting.

### E-036 — Must fix — Reference completeness

**Address:** References; Ref. [12]; PDF p. 160; printed p. 144; PDF-text line 12 (entry begins at 10 on PDF p. 160).

**Source anchor:** Mao, Simone. Studio dinamico di una catenaria a passo e valutazione dell’introduzione di motori planari a levitazione magnetica= Study on the dynamics of a catenary conveyor and evaluation o…

**Fault:** "Thesis, [year]" does not identify awarding institution or degree; reader cannot reliably retrieve work.

**Correction:** Supply thesis type/degree, university, repository/identifier where appropriate; preserve standard bibliography formatting.

### E-037 — Must fix — Reference completeness

**Address:** References; Ref. [71]; PDF p. 165; printed p. 149; PDF-text line 30 (entry begins at 30 on PDF p. 165).

**Source anchor:** Broens, Yorick Leonardus Catharina. Precision control of position dependent dynamics of moving-magnet planar actuators. 2024.

**Fault:** Entry contains author, title, and year only; thesis/report type and awarding institution are missing.

**Correction:** Identify source type, institution and retrieval metadata.

### E-038 — Should fix — Reference completeness

**Address:** References; Ref. [1]; PDF p. 159; printed p. 143; PDF-text line 4 (entry begins at 2 on PDF p. 159).

**Source anchor:** Xu, Zhenchuan, Trakarnchaiyo, Chanuphon, Stewart, Curtis, and Khamesee, Mir Behrad. Modular maglev: Design and implementation of a modular magnetic levitation system to levitate a 2d halbach…

**Fault:** Journal volume and year appear without article number/page span ("Mechatronics, 99, 2024").

**Correction:** Verify and add volume-specific article number/page span or persistent identifier.

### E-039 — Should fix — Reference completeness

**Address:** References; Ref. [7]; PDF p. 159; printed p. 143; PDF-text line 21 (entry begins at 19 on PDF p. 159).

**Source anchor:** Sun, Tao, Zhang, Youpan, Zhang, Hui, Wang, Pei, Zhao, Yongguo, and Liu, Guangliang. Three-wheel driven omnidirectional reconfigurable conveyor belt design. in 2019 Chinese Automation Congres…

**Fault:** Conference title contains 2019 but a separate publication year is not present at the end of the entry.

**Correction:** Add explicit bibliographic year and normalize publisher/venue ordering.

### E-040 — Should fix — Reference completeness

**Address:** References; Ref. [30]; PDF p. 162; printed p. 146; PDF-text line 2 (entry begins at 1 on PDF p. 162).

**Source anchor:** Jeroen de Boeij, Elena Lomonova and Vandenput, Andr´e J.A. Look-up table based real- time commutation of 6-dof planar actuators. 16th IEEE International Conference on Control Applications Pa…

**Fault:** Conference entry has no page numbers and venue/location are run together.

**Correction:** Verify the formal conference name, dates, location and proceedings/page identifier as available.

### E-041 — Must fix — Wrong source type/venue format

**Address:** References; Ref. [41]; PDF p. 163; printed p. 147; PDF-text line 3 (entry begins at 1 on PDF p. 163).

**Source anchor:** Zhang, Han, He, Jiawen, Xu, Xianze, Wang, Rui, Xu, Manman, and Xu, Fengqiu. Numerical modeling and structure optimization for magnetic levitation planar machine using pcb coils. in Actuators…

**Fault:** "in Actuators, vol. ..., p. ... MDPI" formats a journal article as a proceedings contribution. The entry also omits a standard year field.

**Correction:** Treat Actuators as a journal, format with volume/issue/article number and publication year after checking source metadata.

### E-042 — Must fix — Wrong source type/venue format

**Address:** References; Ref. [48]; PDF p. 163; printed p. 147; PDF-text line 26 (entry begins at 24 on PDF p. 163).

**Source anchor:** Mu, Junren and Zhang, He. Design and optimization of a large-air-gap voice coil motor with enhanced thermal management for magnetic levitation vibration isolation in a vacuum. in Actuators, …

**Fault:** "in Actuators, vol. ..., p. ... MDPI" formats a journal article as a proceedings contribution. The entry also omits a standard year field.

**Correction:** Treat Actuators as a journal, format with volume/issue/article number and publication year after checking source metadata.

### E-043 — Must fix — Wrong source type/venue format

**Address:** References; Ref. [90]; PDF p. 167; printed p. 151; PDF-text line 33 (entry begins at 31 on PDF p. 167).

**Source anchor:** Du, Chaofan, Ming, Zhengfeng, Liu, Ding, and Cai, Luyang. Double event-triggered global terminal sliding-mode control with disturbance observation for maglev planar motors. in Actuators, vol…

**Fault:** "in Actuators, vol. ..., p. ... MDPI" formats a journal article as a proceedings contribution. The entry also omits a standard year field.

**Correction:** Treat Actuators as a journal, format with volume/issue/article number and publication year after checking source metadata.

### E-044 — Must fix — Reference completeness

**Address:** References; Ref. [50]; PDF p. 163; printed p. 147; PDF-text line 31 (entry begins at 30 on PDF p. 163).

**Source anchor:** De Boeij, J, Lomonova, E, and Vandenput, AJ. Modeling of ironless permanent magnet planar motor structures. in INTERMAG 2006-IEEE International Magnetics Conference.

**Fault:** Conference reference gives a title and conference name, with no distinct publication year, pages or paper ID.

**Correction:** Add verifiable year and proceedings/paper identification, consistently formatted.

### E-045 — Should fix — Bibliographic pagination

**Address:** References; Ref. [40]; PDF p. 162; printed p. 146; PDF-text line 29 (entry begins at 27 on PDF p. 162).

**Source anchor:** Hu, Wei-Feng, Hu, Hong-Jin, Cao, Guang-Zhong, and Liang, De-Liang. Comparative analy- sis of wire-wound and pcb coil magnetically levitation moving-magnet planar motor. in 2025 15th Internat…

**Fault:** Page interval "p. 1–1" is a suspicious placeholder rather than a useful page range.

**Correction:** Verify official pagination or paper/article identifier; do not retain placeholder pagination.

### E-046 — Should fix — Bibliographic pagination

**Address:** References; Ref. [94]; PDF p. 168; printed p. 152; PDF-text line 15 (entry begins at 13 on PDF p. 168).

**Source anchor:** Song, Fazhi, Liu, Yang, Dong, Yue, Chen, Xinkai, and Tan, Jiubin. Motion control of wafer scanners in lithography systems: From setpoint generation to multi-stage coordination. IEEE Transact…

**Fault:** Journal volume/pages "PP:1–1" is an online-early placeholder in a final thesis.

**Correction:** Update to the latest confirmed volume/issue/pages or explicitly format as Early Access if still applicable.

### E-047 — Should fix — Venue naming

**Address:** References; Ref. [88]; PDF p. 167; printed p. 151; PDF-text line 25 (entry begins at 23 on PDF p. 167).

**Source anchor:** Wang, Chao, Li, Hong-Li, Hu, Hong-Jin, Huang, Su-Dan, and Cao, Guang-Zhong. A lstm- nn-based reference trajectory compensation algorithm for the maglev planar motor control system. in 2025 I…

**Fault:** Venue text "IEEE Energy Conversion Conference Congress and Exposition" includes contradictory/repeated event nouns.

**Correction:** Check the official event title and correct the proceedings field.

### E-048 — Should fix — Author-name styling

**Address:** References; Ref. [3]; PDF p. 159; printed p. 143; PDF-text line 9 (entry begins at 9 on PDF p. 159).

**Source anchor:** Browne, Jim J, Dubois, Didier, Rathmill, Keith, Sethi, Suresh, and Stecke, Kathrin. Classifi- cation of flexible manufacturing systems. The FMS magazine, 2(2):114––117, 1984.

**Fault:** Initial formatting "Jim J" is inconsistent with dotted initials used in neighboring entries (e.g., J. W.).

**Correction:** Standardize first-name initials, punctuation and spacing under the chosen citation style; repair the author fields in the bibliography database.

### E-049 — Should fix — Author-name styling

**Address:** References; Ref. [32]; PDF p. 162; printed p. 146; PDF-text line 5 (entry begins at 5 on PDF p. 162).

**Source anchor:** Kuijpers, BJA, Jansen, JW, and Lomonova, EA. Coil design for a moving-magnet planar motor using the stream-function method. IEEE Transactions on Magnetics, 61(9):1–5, 2025.

**Fault:** Initial formatting "BJA" is inconsistent with dotted initials used in neighboring entries (e.g., J. W.).

**Correction:** Standardize first-name initials, punctuation and spacing under the chosen citation style; repair the author fields in the bibliography database.

### E-050 — Should fix — Author-name styling

**Address:** References; Ref. [42]; PDF p. 163; printed p. 147; PDF-text line 4 (entry begins at 4 on PDF p. 163).

**Source anchor:** Rovers, JMM, Jansen, JW, and Lomonova, EA. Design and measurements of the double layer planar motor. in 2013 International Electric Machines & Drives Conference, p. 204– 211. IEEE.

**Fault:** Initial formatting "JMM" is inconsistent with dotted initials used in neighboring entries (e.g., J. W.).

**Correction:** Standardize first-name initials, punctuation and spacing under the chosen citation style; repair the author fields in the bibliography database.

### E-051 — Should fix — Author-name styling

**Address:** References; Ref. [50]; PDF p. 163; printed p. 147; PDF-text line 30 (entry begins at 30 on PDF p. 163).

**Source anchor:** De Boeij, J, Lomonova, E, and Vandenput, AJ. Modeling of ironless permanent magnet planar motor structures. in INTERMAG 2006-IEEE International Magnetics Conference.

**Fault:** Initial formatting "De Boeij, J" is inconsistent with dotted initials used in neighboring entries (e.g., J. W.).

**Correction:** Standardize first-name initials, punctuation and spacing under the chosen citation style; repair the author fields in the bibliography database.

### E-052 — Should fix — Author-name styling

**Address:** References; Ref. [76]; PDF p. 166; printed p. 150; PDF-text line 14 (entry begins at 14 on PDF p. 166).

**Source anchor:** Sayed, BM and Eltawil, Alaaeldin A. Automatic density measurement of small-size material via magnetic levitation & machine vision techniques. IEEE Transactions on Instrumentation and Measure…

**Fault:** Initial formatting "Sayed, BM" is inconsistent with dotted initials used in neighboring entries (e.g., J. W.).

**Correction:** Standardize first-name initials, punctuation and spacing under the chosen citation style; repair the author fields in the bibliography database.

### E-053 — Must fix — Journal title capitalization

**Address:** References; Ref. [3]; PDF p. 159; printed p. 143; PDF-text line 10 (entry begins at 9 on PDF p. 159).

**Source anchor:** Browne, Jim J, Dubois, Didier, Rathmill, Keith, Sethi, Suresh, and Stecke, Kathrin. Classifi- cation of flexible manufacturing systems. The FMS magazine, 2(2):114––117, 1984.

**Fault:** Journal title appears as "The FMS magazine"; proper publication title capitalization is not preserved.

**Correction:** Use "The FMS Magazine" consistently.

### E-054 — Must fix — Journal title capitalization

**Address:** References; Ref. [21]; PDF p. 161; printed p. 145; PDF-text line 4 (entry begins at 4 on PDF p. 161).

**Source anchor:** Lu, Xiaodong. 6d direct-drive technology for planar motion stages. CIRP annals, 61(1):359– 362, 2012.

**Fault:** Journal title appears as "CIRP annals"; proper publication title capitalization is not preserved.

**Correction:** Use "CIRP Annals" consistently.

### E-055 — Must fix — Journal title capitalization

**Address:** References; Ref. [51]; PDF p. 163; printed p. 147; PDF-text line 33 (entry begins at 32 on PDF p. 163).

**Source anchor:** Akoun, Gilles and Yonnet, J-P. 3d analytical calculation of the forces exerted between two cuboidal magnets. IEEE Transactions on magnetics, 20(5):1962–1964, 1984.

**Fault:** Journal title appears as "IEEE Transactions on magnetics"; proper publication title capitalization is not preserved.

**Correction:** Use "IEEE Transactions on Magnetics" consistently.

### E-056 — Must fix — Journal title capitalization

**Address:** References; Ref. [82]; PDF p. 167; printed p. 151; PDF-text line 5 (entry begins at 3 on PDF p. 167).

**Source anchor:** Lee, Hojin, Kim, Gwanyeon, Lee, Youngwoo, Tomitzuka, Masayoshi, and Kim, Wonhee. Performance enhancement using vertex simplification based on linear parameter varying syn- thesis in planar s…

**Fault:** Journal title appears as "ISA transactions"; proper publication title capitalization is not preserved.

**Correction:** Use "ISA Transactions" consistently.

### E-057 — Should fix — Proper-noun / acronym capitalization

**Address:** References; Ref. [1]; PDF p. 159; printed p. 143; PDF-text line 4 (entry begins at 2 on PDF p. 159).

**Source anchor:** Xu, Zhenchuan, Trakarnchaiyo, Chanuphon, Stewart, Curtis, and Khamesee, Mir Behrad. Modular maglev: Design and implementation of a modular magnetic levitation system to levitate a 2d halbach…

**Fault:** Unprotected technical name or acronym "2d" appears with incorrect lowercase/casing in citation title.

**Correction:** Verify the published title, protect correct acronym/proper name capitalization in the bibliography source, and render as "2D".

**Qualification:** Confirmed text; verify original publication title

### E-058 — Should fix — Proper-noun / acronym capitalization

**Address:** References; Ref. [1]; PDF p. 159; printed p. 143; PDF-text line 4 (entry begins at 2 on PDF p. 159).

**Source anchor:** Xu, Zhenchuan, Trakarnchaiyo, Chanuphon, Stewart, Curtis, and Khamesee, Mir Behrad. Modular maglev: Design and implementation of a modular magnetic levitation system to levitate a 2d halbach…

**Fault:** Unprotected technical name or acronym "halbach" appears with incorrect lowercase/casing in citation title.

**Correction:** Verify the published title, protect correct acronym/proper name capitalization in the bibliography source, and render as "Halbach".

**Qualification:** Confirmed text; verify original publication title

### E-059 — Should fix — Proper-noun / acronym capitalization

**Address:** References; Ref. [9]; PDF p. 160; printed p. 144; PDF-text line 1 (entry begins at 1 on PDF p. 160).

**Source anchor:** Hu, Chuxiong, Fu, Hong, Zhu, Yu, and Zhang, Ming. A 6-dof extended unified wrench model for maglev planar motor. IEEE/ASME Transactions on Mechatronics, 29(5):3579– 3589, 2024.

**Fault:** Unprotected technical name or acronym "6-dof" appears with incorrect lowercase/casing in citation title.

**Correction:** Verify the published title, protect correct acronym/proper name capitalization in the bibliography source, and render as "6-DOF".

**Qualification:** Confirmed text; verify original publication title

### E-060 — Should fix — Proper-noun / acronym capitalization

**Address:** References; Ref. [10]; PDF p. 160; printed p. 144; PDF-text line 5 (entry begins at 4 on PDF p. 160).

**Source anchor:** Nakata, Keigo, Ohnishi, Wataru, Koseki, Takafumi, Nakamura, Yuichiro, Takahashi, Kenji, and Sekiguchi, Hiroyuki. Compensation of fem based wrench-current vector for precise lev- itation cont…

**Fault:** Unprotected technical name or acronym "fem" appears with incorrect lowercase/casing in citation title.

**Correction:** Verify the published title, protect correct acronym/proper name capitalization in the bibliography source, and render as "FEM".

**Qualification:** Confirmed text; verify original publication title

### E-061 — Should fix — Proper-noun / acronym capitalization

**Address:** References; Ref. [18]; PDF p. 160; printed p. 144; PDF-text line 27 (entry begins at 27 on PDF p. 160).

**Source anchor:** Li, Shangqiu. Non-levitative electromagnet robot propulsion method for 2-d material han- dling. IEEE Access, 2025.

**Fault:** Unprotected technical name or acronym "2-d" appears with incorrect lowercase/casing in citation title.

**Correction:** Verify the published title, protect correct acronym/proper name capitalization in the bibliography source, and render as "2-D / 2D, consistently".

**Qualification:** Confirmed text; verify original publication title

### E-062 — Should fix — Proper-noun / acronym capitalization

**Address:** References; Ref. [19]; PDF p. 160; printed p. 144; PDF-text line 30 (entry begins at 29 on PDF p. 160).

**Source anchor:** Li, J., Wang, M., Liu, M., Zhang, C., and Li, L. High-precision triaxial contouring control for magnetic levitation planar motor based on online enhanced newton-robust repetitive learning co…

**Fault:** Unprotected technical name or acronym "newton" appears with incorrect lowercase/casing in citation title.

**Correction:** Verify the published title, protect correct acronym/proper name capitalization in the bibliography source, and render as "Newton".

**Qualification:** Confirmed text; verify original publication title

### E-063 — Should fix — Proper-noun / acronym capitalization

**Address:** References; Ref. [20]; PDF p. 161; printed p. 145; PDF-text line 2 (entry begins at 1 on PDF p. 161).

**Source anchor:** Xu, Zhenchuan, Wang, Yang, Wang, Jie, and Khamesee, Mir Behrad. Predictor-based model predictive control for maglev planar motor with a 2d halbach array mover. Control Engineer- ing Practice…

**Fault:** Unprotected technical name or acronym "2d" appears with incorrect lowercase/casing in citation title.

**Correction:** Verify the published title, protect correct acronym/proper name capitalization in the bibliography source, and render as "2D".

**Qualification:** Confirmed text; verify original publication title

### E-064 — Should fix — Proper-noun / acronym capitalization

**Address:** References; Ref. [20]; PDF p. 161; printed p. 145; PDF-text line 2 (entry begins at 1 on PDF p. 161).

**Source anchor:** Xu, Zhenchuan, Wang, Yang, Wang, Jie, and Khamesee, Mir Behrad. Predictor-based model predictive control for maglev planar motor with a 2d halbach array mover. Control Engineer- ing Practice…

**Fault:** Unprotected technical name or acronym "halbach" appears with incorrect lowercase/casing in citation title.

**Correction:** Verify the published title, protect correct acronym/proper name capitalization in the bibliography source, and render as "Halbach".

**Qualification:** Confirmed text; verify original publication title

### E-065 — Should fix — Proper-noun / acronym capitalization

**Address:** References; Ref. [23]; PDF p. 161; printed p. 145; PDF-text line 10 (entry begins at 9 on PDF p. 161).

**Source anchor:** Wang, Yixing, Yan, Jianhu, Zhang, Long, and Yuan, Liming. Three-dimensional electromag- netic analytical model of 6-dof maglev planar motor with passive halbach pm mover. IEEE Transactions o…

**Fault:** Unprotected technical name or acronym "6-dof" appears with incorrect lowercase/casing in citation title.

**Correction:** Verify the published title, protect correct acronym/proper name capitalization in the bibliography source, and render as "6-DOF".

**Qualification:** Confirmed text; verify original publication title

### E-066 — Should fix — Proper-noun / acronym capitalization

**Address:** References; Ref. [23]; PDF p. 161; printed p. 145; PDF-text line 10 (entry begins at 9 on PDF p. 161).

**Source anchor:** Wang, Yixing, Yan, Jianhu, Zhang, Long, and Yuan, Liming. Three-dimensional electromag- netic analytical model of 6-dof maglev planar motor with passive halbach pm mover. IEEE Transactions o…

**Fault:** Unprotected technical name or acronym "halbach" appears with incorrect lowercase/casing in citation title.

**Correction:** Verify the published title, protect correct acronym/proper name capitalization in the bibliography source, and render as "Halbach".

**Qualification:** Confirmed text; verify original publication title

### E-067 — Should fix — Proper-noun / acronym capitalization

**Address:** References; Ref. [26]; PDF p. 161; printed p. 145; PDF-text line 21 (entry begins at 19 on PDF p. 161).

**Source anchor:** Wang, Ronglu, Zhang, Lu, Shi, Chenyang, Zhao, Chunqiu, and Yang, Kai. Analysis and optimization of a moving magnet permanent magnet synchronous planar motor with split halbach arrays. Energi…

**Fault:** Unprotected technical name or acronym "halbach" appears with incorrect lowercase/casing in citation title.

**Correction:** Verify the published title, protect correct acronym/proper name capitalization in the bibliography source, and render as "Halbach".

**Qualification:** Confirmed text; verify original publication title

### E-068 — Should fix — Proper-noun / acronym capitalization

**Address:** References; Ref. [30]; PDF p. 162; printed p. 146; PDF-text line 2 (entry begins at 1 on PDF p. 162).

**Source anchor:** Jeroen de Boeij, Elena Lomonova and Vandenput, Andr´e J.A. Look-up table based real- time commutation of 6-dof planar actuators. 16th IEEE International Conference on Control Applications Pa…

**Fault:** Unprotected technical name or acronym "6-dof" appears with incorrect lowercase/casing in citation title.

**Correction:** Verify the published title, protect correct acronym/proper name capitalization in the bibliography source, and render as "6-DOF".

**Qualification:** Confirmed text; verify original publication title

### E-069 — Should fix — Proper-noun / acronym capitalization

**Address:** References; Ref. [33]; PDF p. 162; printed p. 146; PDF-text line 7 (entry begins at 7 on PDF p. 162).

**Source anchor:** Peng, Junrong and Zhou, Yunfei. Modeling and analysis of a new 2-d halbach array for magnetically levitated planar motor. IEEE Transactions on Magnetics, 49(1):618–627, 2012.

**Fault:** Unprotected technical name or acronym "2-d" appears with incorrect lowercase/casing in citation title.

**Correction:** Verify the published title, protect correct acronym/proper name capitalization in the bibliography source, and render as "2-D / 2D, consistently".

**Qualification:** Confirmed text; verify original publication title

### E-070 — Should fix — Proper-noun / acronym capitalization

**Address:** References; Ref. [33]; PDF p. 162; printed p. 146; PDF-text line 7 (entry begins at 7 on PDF p. 162).

**Source anchor:** Peng, Junrong and Zhou, Yunfei. Modeling and analysis of a new 2-d halbach array for magnetically levitated planar motor. IEEE Transactions on Magnetics, 49(1):618–627, 2012.

**Fault:** Unprotected technical name or acronym "halbach" appears with incorrect lowercase/casing in citation title.

**Correction:** Verify the published title, protect correct acronym/proper name capitalization in the bibliography source, and render as "Halbach".

**Qualification:** Confirmed text; verify original publication title

### E-071 — Should fix — Proper-noun / acronym capitalization

**Address:** References; Ref. [35]; PDF p. 162; printed p. 146; PDF-text line 13 (entry begins at 12 on PDF p. 162).

**Source anchor:** Wang, Yibo, Liu, Chun, Huang, Zhiwei, Xu, Xianze, and Xu, Fengqiu. Hall-array-based po- sition and posture measurement of mover in mlpm with extendable stroke. IEEE Transactions on Instrumen…

**Fault:** Unprotected technical name or acronym "mlpm" appears with incorrect lowercase/casing in citation title.

**Correction:** Verify the published title, protect correct acronym/proper name capitalization in the bibliography source, and render as "MLPM".

**Qualification:** Confirmed text; verify original publication title

### E-072 — Should fix — Proper-noun / acronym capitalization

**Address:** References; Ref. [36]; PDF p. 162; printed p. 146; PDF-text line 15 (entry begins at 15 on PDF p. 162).

**Source anchor:** Yu, Xuyang, Liu, Enshuo, Fan, Chunguang, Zhao, Bo, and Tan, Jiubin. Honeycomb halbach flexible permanent magnet array for magnetically levitated planar motor. IEEE Transactions on Magnetics,…

**Fault:** Unprotected technical name or acronym "halbach" appears with incorrect lowercase/casing in citation title.

**Correction:** Verify the published title, protect correct acronym/proper name capitalization in the bibliography source, and render as "Halbach".

**Qualification:** Confirmed text; verify original publication title

### E-073 — Should fix — Proper-noun / acronym capitalization

**Address:** References; Ref. [39]; PDF p. 162; printed p. 146; PDF-text line 24 (entry begins at 24 on PDF p. 162).

**Source anchor:** Yang, Runze and Zhang, He. Design of 200n magnetic levitation single-sided voice coil motor. in 2024 IEEE 7th International Electrical and Energy Conference (CIEEC), p. 4976– 4981. IEEE.

**Fault:** Unprotected technical name or acronym "200n" appears with incorrect lowercase/casing in citation title.

**Correction:** Verify the published title, protect correct acronym/proper name capitalization in the bibliography source, and render as "200 N".

**Qualification:** Confirmed text; verify original publication title

### E-074 — Should fix — Proper-noun / acronym capitalization

**Address:** References; Ref. [40]; PDF p. 162; printed p. 146; PDF-text line 28 (entry begins at 27 on PDF p. 162).

**Source anchor:** Hu, Wei-Feng, Hu, Hong-Jin, Cao, Guang-Zhong, and Liang, De-Liang. Comparative analy- sis of wire-wound and pcb coil magnetically levitation moving-magnet planar motor. in 2025 15th Internat…

**Fault:** Unprotected technical name or acronym "pcb" appears with incorrect lowercase/casing in citation title.

**Correction:** Verify the published title, protect correct acronym/proper name capitalization in the bibliography source, and render as "PCB".

**Qualification:** Confirmed text; verify original publication title

### E-075 — Should fix — Proper-noun / acronym capitalization

**Address:** References; Ref. [41]; PDF p. 163; printed p. 147; PDF-text line 2 (entry begins at 1 on PDF p. 163).

**Source anchor:** Zhang, Han, He, Jiawen, Xu, Xianze, Wang, Rui, Xu, Manman, and Xu, Fengqiu. Numerical modeling and structure optimization for magnetic levitation planar machine using pcb coils. in Actuators…

**Fault:** Unprotected technical name or acronym "pcb" appears with incorrect lowercase/casing in citation title.

**Correction:** Verify the published title, protect correct acronym/proper name capitalization in the bibliography source, and render as "PCB".

**Qualification:** Confirmed text; verify original publication title

### E-076 — Should fix — Proper-noun / acronym capitalization

**Address:** References; Ref. [46]; PDF p. 163; printed p. 147; PDF-text line 18 (entry begins at 17 on PDF p. 163).

**Source anchor:** Huang, Zhiwei, Wang, Yibo, Xu, Xianze, and Xu, Fengqiu. A low-cost and high-efficiency magnetic levitation stage based on hall sensors. Measurement Science and Technology, 37(4):045002, 2026…

**Fault:** Unprotected technical name or acronym "hall" appears with incorrect lowercase/casing in citation title.

**Correction:** Verify the published title, protect correct acronym/proper name capitalization in the bibliography source, and render as "Hall".

**Qualification:** Confirmed text; verify original publication title

### E-077 — Should fix — Proper-noun / acronym capitalization

**Address:** References; Ref. [49]; PDF p. 163; printed p. 147; PDF-text line 28 (entry begins at 27 on PDF p. 163).

**Source anchor:** Jiang, Peng, Wang, Qianglong, Yang, Jinhe, Guo, Tongjian, Liu, Ruiqi, and Liu, Zhenyu. Simultaneous magnetization and shape optimization for lorentz motors with low force ripple and parasiti…

**Fault:** Unprotected technical name or acronym "lorentz" appears with incorrect lowercase/casing in citation title.

**Correction:** Verify the published title, protect correct acronym/proper name capitalization in the bibliography source, and render as "Lorentz".

**Qualification:** Confirmed text; verify original publication title

### E-078 — Should fix — Proper-noun / acronym capitalization

**Address:** References; Ref. [55]; PDF p. 164; printed p. 148; PDF-text line 10 (entry begins at 10 on PDF p. 164).

**Source anchor:** Ortner, Michael and Bandeira, Lucas Gabriel Coliado. Magpylib: A free python package for magnetic field computation. SoftwareX, 11:100466, 2020.

**Fault:** Unprotected technical name or acronym "python" appears with incorrect lowercase/casing in citation title.

**Correction:** Verify the published title, protect correct acronym/proper name capitalization in the bibliography source, and render as "Python".

**Qualification:** Confirmed text; verify original publication title

### E-079 — Should fix — Proper-noun / acronym capitalization

**Address:** References; Ref. [56]; PDF p. 164; printed p. 148; PDF-text line 13 (entry begins at 12 on PDF p. 164).

**Source anchor:** Ospanova, Aigerim, Konysbekov, Alisher, Pruchnik, Bartosz, Putek, Piotr, Gotszalk, Teodor, Dziedzic, Andrzej, Ellis, Grant, and Skrzypacz, Piotr. Magnetic field sensing of 3d printed halbach…

**Fault:** Unprotected technical name or acronym "3d" appears with incorrect lowercase/casing in citation title.

**Correction:** Verify the published title, protect correct acronym/proper name capitalization in the bibliography source, and render as "3D".

**Qualification:** Confirmed text; verify original publication title

### E-080 — Should fix — Proper-noun / acronym capitalization

**Address:** References; Ref. [56]; PDF p. 164; printed p. 148; PDF-text line 14 (entry begins at 12 on PDF p. 164).

**Source anchor:** Ospanova, Aigerim, Konysbekov, Alisher, Pruchnik, Bartosz, Putek, Piotr, Gotszalk, Teodor, Dziedzic, Andrzej, Ellis, Grant, and Skrzypacz, Piotr. Magnetic field sensing of 3d printed halbach…

**Fault:** Unprotected technical name or acronym "halbach" appears with incorrect lowercase/casing in citation title.

**Correction:** Verify the published title, protect correct acronym/proper name capitalization in the bibliography source, and render as "Halbach".

**Qualification:** Confirmed text; verify original publication title

### E-081 — Should fix — Proper-noun / acronym capitalization

**Address:** References; Ref. [63]; PDF p. 165; printed p. 149; PDF-text line 5 (entry begins at 4 on PDF p. 165).

**Source anchor:** Wang, Chao, Cao, Guang-Zhong, Hu, Hong-Jin, and Huang, Su-Dan. A data-driven magnetic field model for the halbach arrays of the magnetically levitated planar motor with variable harmonic coe…

**Fault:** Unprotected technical name or acronym "halbach" appears with incorrect lowercase/casing in citation title.

**Correction:** Verify the published title, protect correct acronym/proper name capitalization in the bibliography source, and render as "Halbach".

**Qualification:** Confirmed text; verify original publication title

### E-082 — Should fix — Proper-noun / acronym capitalization

**Address:** References; Ref. [65]; PDF p. 165; printed p. 149; PDF-text line 11 (entry begins at 10 on PDF p. 165).

**Source anchor:** Wang, Xiusen, Zhong, Zaimin, Wang, Yeqin, Jiang, Bowen, and Chen, Wei. Magnetic levi- tation control of doubly fed linear motor with multiphase ac excited mover. IEEE Journal of Emerging and…

**Fault:** Unprotected technical name or acronym "ac" appears with incorrect lowercase/casing in citation title.

**Correction:** Verify the published title, protect correct acronym/proper name capitalization in the bibliography source, and render as "AC".

**Qualification:** Confirmed text; verify original publication title

### E-083 — Should fix — Proper-noun / acronym capitalization

**Address:** References; Ref. [66]; PDF p. 165; printed p. 149; PDF-text line 14 (entry begins at 13 on PDF p. 165).

**Source anchor:** Xu, Zhiyuan, Gu, Yajie, Xu, Rongqing, and Qin, Yaohong. Design, implementation, and control of a maglev planar motor with 6-dof current-sharing, 2024. Bibliographic metadata reconstructed fr…

**Fault:** Unprotected technical name or acronym "6-dof" appears with incorrect lowercase/casing in citation title.

**Correction:** Verify the published title, protect correct acronym/proper name capitalization in the bibliography source, and render as "6-DOF".

**Qualification:** Confirmed text; verify original publication title

### E-084 — Should fix — Proper-noun / acronym capitalization

**Address:** References; Ref. [67]; PDF p. 165; printed p. 149; PDF-text line 17 (entry begins at 16 on PDF p. 165).

**Source anchor:** Ran, Ming, Ma, Jun, Fan, Chunguang, and Zhao, Bo. Drive-augmented model predictive control with kalman state observer for long-stroke maglev planar motor. in IET Conference Proceedings CP936…

**Fault:** Unprotected technical name or acronym "kalman" appears with incorrect lowercase/casing in citation title.

**Correction:** Verify the published title, protect correct acronym/proper name capitalization in the bibliography source, and render as "Kalman".

**Qualification:** Confirmed text; verify original publication title

### E-085 — Should fix — Proper-noun / acronym capitalization

**Address:** References; Ref. [69]; PDF p. 165; printed p. 149; PDF-text line 24 (entry begins at 23 on PDF p. 165).

**Source anchor:** Zhou, Shun, Shi, Yuan, Zou, Menglong, Xu, Fengqiu, and Xu, Xianze. Tracking error sup- pression of maglev planar actuator with fpga-based mpc. IEEE Transactions on Instrumen- tation and Meas…

**Fault:** Unprotected technical name or acronym "fpga" appears with incorrect lowercase/casing in citation title.

**Correction:** Verify the published title, protect correct acronym/proper name capitalization in the bibliography source, and render as "FPGA".

**Qualification:** Confirmed text; verify original publication title

### E-086 — Should fix — Proper-noun / acronym capitalization

**Address:** References; Ref. [69]; PDF p. 165; printed p. 149; PDF-text line 24 (entry begins at 23 on PDF p. 165).

**Source anchor:** Zhou, Shun, Shi, Yuan, Zou, Menglong, Xu, Fengqiu, and Xu, Xianze. Tracking error sup- pression of maglev planar actuator with fpga-based mpc. IEEE Transactions on Instrumen- tation and Meas…

**Fault:** Unprotected technical name or acronym "mpc" appears with incorrect lowercase/casing in citation title.

**Correction:** Verify the published title, protect correct acronym/proper name capitalization in the bibliography source, and render as "MPC".

**Qualification:** Confirmed text; verify original publication title

### E-087 — Should fix — Proper-noun / acronym capitalization

**Address:** References; Ref. [75]; PDF p. 166; printed p. 150; PDF-text line 12 (entry begins at 11 on PDF p. 166).

**Source anchor:** Yan, Jianhu, Wang, Yixing, Zhang, Long, and Lin, Heyun. Passive mover pose detection of maglev planar motor with hall sensor array based on bp neural network. IEEE Sensors Journal, 2025.

**Fault:** Unprotected technical name or acronym "hall" appears with incorrect lowercase/casing in citation title.

**Correction:** Verify the published title, protect correct acronym/proper name capitalization in the bibliography source, and render as "Hall".

**Qualification:** Confirmed text; verify original publication title

### E-088 — Should fix — Proper-noun / acronym capitalization

**Address:** References; Ref. [75]; PDF p. 166; printed p. 150; PDF-text line 12 (entry begins at 11 on PDF p. 166).

**Source anchor:** Yan, Jianhu, Wang, Yixing, Zhang, Long, and Lin, Heyun. Passive mover pose detection of maglev planar motor with hall sensor array based on bp neural network. IEEE Sensors Journal, 2025.

**Fault:** Unprotected technical name or acronym "bp" appears with incorrect lowercase/casing in citation title.

**Correction:** Verify the published title, protect correct acronym/proper name capitalization in the bibliography source, and render as "BP".

**Qualification:** Confirmed text; verify original publication title

### E-089 — Should fix — Proper-noun / acronym capitalization

**Address:** References; Ref. [77]; PDF p. 166; printed p. 150; PDF-text line 18 (entry begins at 17 on PDF p. 166).

**Source anchor:** Yu, Chenglong, Fan, Chunguang, Li, Tianyi, Li, Na, Zhao, Bo, and Tan, Jiubin. Research on electromagnetic drive modeling and precision hall measurement of maglev platform. in 2024 Academic C…

**Fault:** Unprotected technical name or acronym "hall" appears with incorrect lowercase/casing in citation title.

**Correction:** Verify the published title, protect correct acronym/proper name capitalization in the bibliography source, and render as "Hall".

**Qualification:** Confirmed text; verify original publication title

### E-090 — Should fix — Proper-noun / acronym capitalization

**Address:** References; Ref. [80]; PDF p. 166; printed p. 150; PDF-text line 27 (entry begins at 26 on PDF p. 166).

**Source anchor:** Bizuneh, Ambachew, Mitiku, Hunachew, Salau, Ayodeji Olalekan, and Chandran, Karthic. Performance analysis of an optimized pid-p controller for the position control of a magnetic levitation s…

**Fault:** Unprotected technical name or acronym "pid" appears with incorrect lowercase/casing in citation title.

**Correction:** Verify the published title, protect correct acronym/proper name capitalization in the bibliography source, and render as "PID".

**Qualification:** Confirmed text; verify original publication title

### E-091 — Should fix — Proper-noun / acronym capitalization

**Address:** References; Ref. [85]; PDF p. 167; printed p. 151; PDF-text line 14 (entry begins at 13 on PDF p. 167).

**Source anchor:** Liu, Minghong, Wang, Mingyi, Li, Junchi, Sun, Qinwei, Zhang, Chengming, and Li, Liyi. Hybrid harmonic and rbfnn-based disturbance estimation and feedforward compensation for multiaxis maglev…

**Fault:** Unprotected technical name or acronym "rbfnn" appears with incorrect lowercase/casing in citation title.

**Correction:** Verify the published title, protect correct acronym/proper name capitalization in the bibliography source, and render as "RBFNN".

**Qualification:** Confirmed text; verify original publication title

### E-092 — Should fix — Proper-noun / acronym capitalization

**Address:** References; Ref. [88]; PDF p. 167; printed p. 151; PDF-text line 23 (entry begins at 23 on PDF p. 167).

**Source anchor:** Wang, Chao, Li, Hong-Li, Hu, Hong-Jin, Huang, Su-Dan, and Cao, Guang-Zhong. A lstm- nn-based reference trajectory compensation algorithm for the maglev planar motor control system. in 2025 I…

**Fault:** Unprotected technical name or acronym "lstm" appears with incorrect lowercase/casing in citation title.

**Correction:** Verify the published title, protect correct acronym/proper name capitalization in the bibliography source, and render as "LSTM".

**Qualification:** Confirmed text; verify original publication title

### E-093 — Should fix — Proper-noun / acronym capitalization

**Address:** References; Ref. [91]; PDF p. 168; printed p. 152; PDF-text line 2 (entry begins at 2 on PDF p. 168).

**Source anchor:** Chen, Xiang, Na, Tuopu, Ma, Chenglong, Ning, Lei, and Zhao, Bo. The robust pi control of a magnetically levitated planar motor with output constrains. in 2024 3rd Conference on Fully Actuate…

**Fault:** Unprotected technical name or acronym "pi" appears with incorrect lowercase/casing in citation title.

**Correction:** Verify the published title, protect correct acronym/proper name capitalization in the bibliography source, and render as "PI".

**Qualification:** Confirmed text; verify original publication title

### E-094 — Should fix — Proper-noun / acronym capitalization

**Address:** References; Ref. [92]; PDF p. 168; printed p. 152; PDF-text line 7 (entry begins at 5 on PDF p. 168).

**Source anchor:** Hartmann, Philipp, Stranghöner, Jannick, and Neumann, Klaus. End-to-end low-level neural control of an industrial-grade 6d magnetic levitation system. arXiv preprint arXiv:2509.01388, 2025.

**Fault:** Unprotected technical name or acronym "6d" appears with incorrect lowercase/casing in citation title.

**Correction:** Verify the published title, protect correct acronym/proper name capitalization in the bibliography source, and render as "6D".

**Qualification:** Confirmed text; verify original publication title

### E-095 — Must fix — Reference sentence capitalization

**Address:** References; Ref. [7]; PDF p. 159; printed p. 143; PDF-text line 20 (entry begins at 19 on PDF p. 159).

**Source anchor:** Sun, Tao, Zhang, Youpan, Zhang, Hui, Wang, Pei, Zhao, Yongguo, and Liu, Guangliang. Three-wheel driven omnidirectional reconfigurable conveyor belt design. in 2019 Chinese Automation Congres…

**Fault:** Conference/proceedings introducer is lowercased after an end-of-sentence period (". in ...").

**Correction:** Capitalize as "In:" or "In" according to the bibliography style; repair the `.bib` entry type/format so the change is generated automatically.

### E-096 — Must fix — Reference sentence capitalization

**Address:** References; Ref. [10]; PDF p. 160; printed p. 144; PDF-text line 6 (entry begins at 4 on PDF p. 160).

**Source anchor:** Nakata, Keigo, Ohnishi, Wataru, Koseki, Takafumi, Nakamura, Yuichiro, Takahashi, Kenji, and Sekiguchi, Hiroyuki. Compensation of fem based wrench-current vector for precise lev- itation cont…

**Fault:** Conference/proceedings introducer is lowercased after an end-of-sentence period (". in ...").

**Correction:** Capitalize as "In:" or "In" according to the bibliography style; repair the `.bib` entry type/format so the change is generated automatically.

### E-097 — Must fix — Reference sentence capitalization

**Address:** References; Ref. [24]; PDF p. 161; printed p. 145; PDF-text line 14 (entry begins at 12 on PDF p. 161).

**Source anchor:** Wang, Chao and Cao, Guang-Zhong. A novel algorithm of force distribution to reduce force coupling for the six-degree-of-freedom maglev planar motor. in 2025 15th International Symposium on L…

**Fault:** Conference/proceedings introducer is lowercased after an end-of-sentence period (". in ...").

**Correction:** Capitalize as "In:" or "In" according to the bibliography style; repair the `.bib` entry type/format so the change is generated automatically.

### E-098 — Must fix — Reference sentence capitalization

**Address:** References; Ref. [29]; PDF p. 161; printed p. 145; PDF-text line 30 (entry begins at 28 on PDF p. 161).

**Source anchor:** Nakata, Keigo, Ohnishi, Wataru, Koseki, Takafumi, Nakamura, Yuichiro, Takahashi, Kenji, and Sekiguchi, Hiroyuki. Drive stabilization of multi-degree-of-freedom maglev planar mo- tor based on…

**Fault:** Conference/proceedings introducer is lowercased after an end-of-sentence period (". in ...").

**Correction:** Capitalize as "In:" or "In" according to the bibliography style; repair the `.bib` entry type/format so the change is generated automatically.

### E-099 — Must fix — Reference sentence capitalization

**Address:** References; Ref. [39]; PDF p. 162; printed p. 146; PDF-text line 25 (entry begins at 24 on PDF p. 162).

**Source anchor:** Yang, Runze and Zhang, He. Design of 200n magnetic levitation single-sided voice coil motor. in 2024 IEEE 7th International Electrical and Energy Conference (CIEEC), p. 4976– 4981. IEEE.

**Fault:** Conference/proceedings introducer is lowercased after an end-of-sentence period (". in ...").

**Correction:** Capitalize as "In:" or "In" according to the bibliography style; repair the `.bib` entry type/format so the change is generated automatically.

### E-100 — Must fix — Reference sentence capitalization

**Address:** References; Ref. [40]; PDF p. 162; printed p. 146; PDF-text line 28 (entry begins at 27 on PDF p. 162).

**Source anchor:** Hu, Wei-Feng, Hu, Hong-Jin, Cao, Guang-Zhong, and Liang, De-Liang. Comparative analy- sis of wire-wound and pcb coil magnetically levitation moving-magnet planar motor. in 2025 15th Internat…

**Fault:** Conference/proceedings introducer is lowercased after an end-of-sentence period (". in ...").

**Correction:** Capitalize as "In:" or "In" according to the bibliography style; repair the `.bib` entry type/format so the change is generated automatically.

### E-101 — Must fix — Reference sentence capitalization

**Address:** References; Ref. [42]; PDF p. 163; printed p. 147; PDF-text line 5 (entry begins at 4 on PDF p. 163).

**Source anchor:** Rovers, JMM, Jansen, JW, and Lomonova, EA. Design and measurements of the double layer planar motor. in 2013 International Electric Machines & Drives Conference, p. 204– 211. IEEE.

**Fault:** Conference/proceedings introducer is lowercased after an end-of-sentence period (". in ...").

**Correction:** Capitalize as "In:" or "In" according to the bibliography style; repair the `.bib` entry type/format so the change is generated automatically.

### E-102 — Must fix — Reference sentence capitalization

**Address:** References; Ref. [43]; PDF p. 163; printed p. 147; PDF-text line 9 (entry begins at 7 on PDF p. 163).

**Source anchor:** Liu, Kai, Chen, Fuxiang, Wu, Yingtong, Hu, Aoqi, Wei, Xinpeng, and Zeng, Lizhan. Analy- sis of electromagnetic force and power consumption in magnetic levitation planar motor with dual-layer…

**Fault:** Conference/proceedings introducer is lowercased after an end-of-sentence period (". in ...").

**Correction:** Capitalize as "In:" or "In" according to the bibliography style; repair the `.bib` entry type/format so the change is generated automatically.

### E-103 — Must fix — Reference sentence capitalization

**Address:** References; Ref. [50]; PDF p. 163; printed p. 147; PDF-text line 31 (entry begins at 30 on PDF p. 163).

**Source anchor:** De Boeij, J, Lomonova, E, and Vandenput, AJ. Modeling of ironless permanent magnet planar motor structures. in INTERMAG 2006-IEEE International Magnetics Conference.

**Fault:** Conference/proceedings introducer is lowercased after an end-of-sentence period (". in ...").

**Correction:** Capitalize as "In:" or "In" according to the bibliography style; repair the `.bib` entry type/format so the change is generated automatically.

### E-104 — Must fix — Reference sentence capitalization

**Address:** References; Ref. [57]; PDF p. 164; printed p. 148; PDF-text line 17 (entry begins at 15 on PDF p. 164).

**Source anchor:** Li, Hanyu, Zhang, Shengguo, Zhu, Jiaran, Zhu, Binrong, and Ma, Jiayu. Finite element modeling of electromagnetic forces in square coils of magnetically levitated planar motors. in 2025 IEEE …

**Fault:** Conference/proceedings introducer is lowercased after an end-of-sentence period (". in ...").

**Correction:** Capitalize as "In:" or "In" according to the bibliography style; repair the `.bib` entry type/format so the change is generated automatically.

### E-105 — Must fix — Reference sentence capitalization

**Address:** References; Ref. [60]; PDF p. 164; printed p. 148; PDF-text line 26 (entry begins at 25 on PDF p. 164).

**Source anchor:** Zhu, Mingxun, Wang, Xiaolin, Bao, Xucong, and Zhou, Haoying. Decoupling control strat- egy for maglev planar motors based on virtual current coordinate system. in 2025 28th Inter- national C…

**Fault:** Conference/proceedings introducer is lowercased after an end-of-sentence period (". in ...").

**Correction:** Capitalize as "In:" or "In" according to the bibliography style; repair the `.bib` entry type/format so the change is generated automatically.

### E-106 — Must fix — Reference sentence capitalization

**Address:** References; Ref. [61]; PDF p. 164; printed p. 148; PDF-text line 28 (entry begins at 28 on PDF p. 164).

**Source anchor:** Hareer, Sarah and Shary, Diyah Kammel. Analytical review of linear reluctance motors. in 2026 13th International Conference on Electrical and Electronics Engineering (ICEEE), p. 147–152. IEE…

**Fault:** Conference/proceedings introducer is lowercased after an end-of-sentence period (". in ...").

**Correction:** Capitalize as "In:" or "In" according to the bibliography style; repair the `.bib` entry type/format so the change is generated automatically.

### E-107 — Must fix — Reference sentence capitalization

**Address:** References; Ref. [62]; PDF p. 165; printed p. 149; PDF-text line 2 (entry begins at 1 on PDF p. 165).

**Source anchor:** Liu, Kai, Chen, Fuxiang, and Zeng, Lizhan. Fluctuation analysis of electromagnetic force in magnetic levitation planar motor. in 2024 10th International Conference on Control, Au- tomation a…

**Fault:** Conference/proceedings introducer is lowercased after an end-of-sentence period (". in ...").

**Correction:** Capitalize as "In:" or "In" according to the bibliography style; repair the `.bib` entry type/format so the change is generated automatically.

### E-108 — Must fix — Reference sentence capitalization

**Address:** References; Ref. [67]; PDF p. 165; printed p. 149; PDF-text line 17 (entry begins at 16 on PDF p. 165).

**Source anchor:** Ran, Ming, Ma, Jun, Fan, Chunguang, and Zhao, Bo. Drive-augmented model predictive control with kalman state observer for long-stroke maglev planar motor. in IET Conference Proceedings CP936…

**Fault:** Conference/proceedings introducer is lowercased after an end-of-sentence period (". in ...").

**Correction:** Capitalize as "In:" or "In" according to the bibliography style; repair the `.bib` entry type/format so the change is generated automatically.

### E-109 — Must fix — Reference sentence capitalization

**Address:** References; Ref. [68]; PDF p. 165; printed p. 149; PDF-text line 21 (entry begins at 19 on PDF p. 165).

**Source anchor:** Nakata, Keigo, Ohnishi, Wataru, Koseki, Takafumi, Nakamura, Yuichiro, Takahashi, Kenji, and Sekiguchi, Hiroyuki. Highly responsive drive of a repulsive multi-degree-of-freedom magnetic levit…

**Fault:** Conference/proceedings introducer is lowercased after an end-of-sentence period (". in ...").

**Correction:** Capitalize as "In:" or "In" according to the bibliography style; repair the `.bib` entry type/format so the change is generated automatically.

### E-110 — Must fix — Reference sentence capitalization

**Address:** References; Ref. [70]; PDF p. 165; printed p. 149; PDF-text line 28 (entry begins at 26 on PDF p. 165).

**Source anchor:** Chen, Fuxiang, Liu, Kai, Wu, Yingtong, Hu, Aoqi, Wei, Xinpeng, Hong, Cailin, and Zeng, Lizhan. Model calibration of inconsistent coils shape driven by coupling effect of magnetic levitation …

**Fault:** Conference/proceedings introducer is lowercased after an end-of-sentence period (". in ...").

**Correction:** Capitalize as "In:" or "In" according to the bibliography style; repair the `.bib` entry type/format so the change is generated automatically.

### E-111 — Must fix — Reference sentence capitalization

**Address:** References; Ref. [73]; PDF p. 166; printed p. 150; PDF-text line 6 (entry begins at 4 on PDF p. 166).

**Source anchor:** Mitsui, Shota, Konishi, Akito, Kondo, Ken-ichi, and Ohashi, Shunsuke. Study of pitch- ing suppression in a propulsion and levitation integrated conveyance system using the linear stepper mot…

**Fault:** Conference/proceedings introducer is lowercased after an end-of-sentence period (". in ...").

**Correction:** Capitalize as "In:" or "In" according to the bibliography style; repair the `.bib` entry type/format so the change is generated automatically.

### E-112 — Must fix — Reference sentence capitalization

**Address:** References; Ref. [77]; PDF p. 166; printed p. 150; PDF-text line 18 (entry begins at 17 on PDF p. 166).

**Source anchor:** Yu, Chenglong, Fan, Chunguang, Li, Tianyi, Li, Na, Zhao, Bo, and Tan, Jiubin. Research on electromagnetic drive modeling and precision hall measurement of maglev platform. in 2024 Academic C…

**Fault:** Conference/proceedings introducer is lowercased after an end-of-sentence period (". in ...").

**Correction:** Capitalize as "In:" or "In" according to the bibliography style; repair the `.bib` entry type/format so the change is generated automatically.

### E-113 — Must fix — Reference sentence capitalization

**Address:** References; Ref. [78]; PDF p. 166; printed p. 150; PDF-text line 21 (entry begins at 20 on PDF p. 166).

**Source anchor:** Yu, Xuyang, Fan, Chunguang, Ran, Ming, Ma, Jun, and Yu, Chenglong. Research on key technology of motion decoupling of maglev robot based on perturbation theory. in 2024 IEEE International Co…

**Fault:** Conference/proceedings introducer is lowercased after an end-of-sentence period (". in ...").

**Correction:** Capitalize as "In:" or "In" according to the bibliography style; repair the `.bib` entry type/format so the change is generated automatically.

### E-114 — Must fix — Reference sentence capitalization

**Address:** References; Ref. [79]; PDF p. 166; printed p. 150; PDF-text line 23 (entry begins at 23 on PDF p. 166).

**Source anchor:** Wang, John and Olson, Edwin. Apriltag 2: Efficient and robust fiducial detection. in 2016 IEEE/RSJ international conference on intelligent robots and systems (IROS), p. 4193–4198. IEEE.

**Fault:** Conference/proceedings introducer is lowercased after an end-of-sentence period (". in ...").

**Correction:** Capitalize as "In:" or "In" according to the bibliography style; repair the `.bib` entry type/format so the change is generated automatically.

### E-115 — Must fix — Reference sentence capitalization

**Address:** References; Ref. [81]; PDF p. 167; printed p. 151; PDF-text line 1 (entry begins at 30 on PDF p. 166).

**Source anchor:** Ma, ZhanChao, Yang, DongSheng, Zhu, YeSheng, Wang, Xin, and Gao, XiaoTing. An un- balance compensation method for rotor system of magnetic levitation motors based on beetle algorithm. in 202…

**Fault:** Conference/proceedings introducer is lowercased after an end-of-sentence period (". in ...").

**Correction:** Capitalize as "In:" or "In" according to the bibliography style; repair the `.bib` entry type/format so the change is generated automatically.

### E-116 — Must fix — Reference sentence capitalization

**Address:** References; Ref. [84]; PDF p. 167; printed p. 151; PDF-text line 11 (entry begins at 9 on PDF p. 167).

**Source anchor:** Liu, Minghong, Wang, Mingyi, Li, Junchi, Sun, Qinwei, Zhang, Chengming, and Li, Liyi. Adaptive feedforward control based on recursive least squares algorithm for the biaxial ma- glev planar-…

**Fault:** Conference/proceedings introducer is lowercased after an end-of-sentence period (". in ...").

**Correction:** Capitalize as "In:" or "In" according to the bibliography style; repair the `.bib` entry type/format so the change is generated automatically.

### E-117 — Must fix — Reference sentence capitalization

**Address:** References; Ref. [88]; PDF p. 167; printed p. 151; PDF-text line 25 (entry begins at 23 on PDF p. 167).

**Source anchor:** Wang, Chao, Li, Hong-Li, Hu, Hong-Jin, Huang, Su-Dan, and Cao, Guang-Zhong. A lstm- nn-based reference trajectory compensation algorithm for the maglev planar motor control system. in 2025 I…

**Fault:** Conference/proceedings introducer is lowercased after an end-of-sentence period (". in ...").

**Correction:** Capitalize as "In:" or "In" according to the bibliography style; repair the `.bib` entry type/format so the change is generated automatically.

### E-118 — Must fix — Reference sentence capitalization

**Address:** References; Ref. [91]; PDF p. 168; printed p. 152; PDF-text line 3 (entry begins at 2 on PDF p. 168).

**Source anchor:** Chen, Xiang, Na, Tuopu, Ma, Chenglong, Ning, Lei, and Zhao, Bo. The robust pi control of a magnetically levitated planar motor with output constrains. in 2024 3rd Conference on Fully Actuate…

**Fault:** Conference/proceedings introducer is lowercased after an end-of-sentence period (". in ...").

**Correction:** Capitalize as "In:" or "In" according to the bibliography style; repair the `.bib` entry type/format so the change is generated automatically.

## Assessment limitations

The rendered 180-page PDF and extracted bibliography were examined. The PDF contains no usable native text-line mapping to LaTeX source, and the first Persian lines are demonstrably corrupt when copied. Accurate complete Farsi spellcheck/spacing audit and template-specific compliance therefore require the original `.tex`/`.docx` plus the faculty stylesheet. Do not assume all unlisted passages have been exhaustively line-edited. 
