# Citation Verification Log — Supporting Appendix

Compiled from primary-source fetches performed against www.bahai.org and
reference.bahai.org during manuscript review. Each row records: the quotation as it
appears in the manuscript, the citation given, the primary source fetched, and the
verification outcome. This log is the evidentiary basis for the "Citation and reference
verification" section of the AI Disclosure Statement — every claim there should trace to
a row here.

## Verified — exact match, location confirmed

| # | Quotation (manuscript) | Citation given | Source fetched | Outcome |
|---|---|---|---|---|
| 1 | "Religion and science are the two wings upon which man's intelligence can soar into the heights, with which the human soul can progress" | Paris Talks, p.143 | reference.bahai.org/en/t/ab/PT/pt-45.html (page titled "Pages 141-146"), re-fetched and re-checked directly | Verbatim match; page marker "143" appears in the source text in the same paragraph shortly before the quote. Confirmed. |
| 2 | "All created things are expressions of the affinity and cohesion..." | PUP, Talk 48 | bahai.org PUP .docx | Verbatim match (one elided middle sentence, properly marked); talk marker "48" confirmed. |
| 3 | "Spirit, mind, soul, and the powers of sight and hearing are but one single reality..." | Summons of the Lord of Hosts, para. 35 | reference.bahai.org/en/t/b/SLH/slh-10.html | Verbatim match; paragraph marker "35" immediately precedes quote. Confirmed. |
| 4 | "The world of existence came into being through the heat generated..." | Tablets of Bahá'u'lláh, p.140 | reference.bahai.org/en/t/b/TB/tb-10.html | Verbatim match; page marker "140" is the last page marker before the quote (~1 paragraph of intervening text, no "141" marker). Confirmed. |
| 5 | "I loved thy creation, hence I created thee..." | Hidden Words, Arabic no. 4 | bahai.org Hidden Words .docx | Verbatim match; numbered marker "4" immediately precedes it. Confirmed. |
| 6 | "Within thee have I placed the essence of My light" | Hidden Words, Arabic no. 12 | bahai.org Hidden Words .docx | Verbatim match; numbered marker "12" immediately precedes it. Confirmed. |
| 7 | "For I have created thee rich..." (used unquoted as "was created rich") | Hidden Words (no verse given) | bahai.org Hidden Words .docx | Verbatim match, Arabic no. 13 (marker "13" immediately precedes it; "12" precedes the *previous* verse, not this one). Confirmed. |
| 8 | "All created things are connected one to another by a linkage complete and perfect..." | Selections from the Writings of 'Abdu'l-Bahá, §21 | bahai.org Selections .docx | Verbatim match; section marker "21.6" immediately precedes quote. Confirmed. |
| 9 | "The soul is not a combination of elements, it is not composed of many atoms..." | Paris Talks, p.91 (corrected from original SAQ misattribution) | reference.bahai.org/en/t/ab/PT/pt-29.html + bahai.org Paris Talks .docx | NOT found anywhere in Some Answered Questions (confirmed by full-text search: zero hits for 5 variant phrasings). Found verbatim in Paris Talks; page marker "91" confirmed. Citation corrected in pub3 and book. |
| 10 | "...has a connection with the body like that of the sun with this mirror..." | SAQ, Ch. 68 | bahai.org SAQ .docx | Near-verbatim match ("occupies no place within" vs. manuscript's "is not within" — same substance, minor paraphrase). Confirmed accurate as cited. |

## Corrected — fabricated or inaccurate quote content found and fixed

| # | Manuscript's original wording | Citation given | Verification finding | Fix applied |
|---|---|---|---|---|
| 11 | "...Motion is life...All energy is contingent upon motion." | PUP, Talk 52 | Talk 52 heading confirmed correct; opening sentences verbatim; but "All energy is contingent upon motion" does NOT appear anywhere in PUP (checked 2 variant phrasings, both -1). Real continuation: "...The universal energy is dynamic. Nothing is stationary..." | Quote ending replaced with verified text in pub3 (2 occurrences) **and, discovered later, in the book — which repeated the identical fabricated phrase 6 times across 3 chapters** (confirmed directly from the fix commit's diff): ch.III — 1 instance (quote block); ch.VI — 2 instances (the quote block, and a standalone analytical sentence that quotes the fabricated phrase inline and discusses it); ch.XII — 3 instances (a quote block, a second inline analytical quotation of the phrase in the same paragraph, and a second, separate quote block later in the chapter). All 6 instances corrected to the verified wording; the analytical prose built directly on the fabricated phrase (in ch.VI and ch.XII) was rewritten to interpret the real text instead. |
| 12 | "...The constituent parts...separate, and the form perishes." | PUP, Talk 41 | Talk 41 marker confirmed correct; opening clause ("when dissension and repulsion arise...disintegration follows") verbatim; but "the form perishes" and "constituent parts...separate" do NOT appear in PUP (both -1). | Quote trimmed to end at the verified "...disintegration follows" in both pub3 occurrences. |
| 13 | "total annihilation is impossible" | PUP, Talk 38 | Talk 38 marker confirmed correct; but exact source wording is "total annihilation is **an** impossibility" (found twice in PUP), not "is impossible." | Corrected to exact wording in pub3. |
| 14 | (Book only) "The soul is not a combination of elements...for then it would be made subject to disintegration and its existence would be contingent and not essential" | SAQ, Ch. 66 | Searched SAQ full text for "made subject to disintegration," "contingent and not essential" — both -1, not found. This is a *different* fabricated continuation than pub3's version (#9 above), attached to the same real opening clause, in the book manuscript only. | Corrected to the verified Paris Talks wording (same source as #9) in book, 2 occurrences. |

## Placeholder source replaced (not a quote-accuracy issue, but a citability issue)

| # | Issue | Resolution |
|---|---|---|
| 15 | `BSW` ("Bahá'í Sacred Writings", a generic 1983 anthology) used as a bibliography entry across pub2, pub3, and the book — no such identifiable single-volume source exists under this title. | Replaced with the two specific, verified primary sources the quotes actually trace to: `TabletsBahaullah` (Tablet of Wisdom, p.140 — item #4 above) and `SummonsLordHosts` (para. 35 — item #3 above), in all three documents. |

## Explicitly NOT independently re-verified (flagged, not fixed)

| # | Item | Reason not verified | Status |
|---|---|---|---|
| 16 | "each kingdom able to apprehend the kingdoms beneath it but not the kingdom above it" — SAQ, Part 4 (hierarchy of comprehension) | Paraphrase, not verbatim quotation; judged lower priority than direct quotes at the time | Attempted this session — searched SAQ full text for multiple phrasings of the graded-comprehension-hierarchy claim; none matched. Inconclusive: the general theme (differentiated comprehension across kingdoms) is a recurring SAQ motif, but I could not confirm the "Part 4" location or locate the specific passage in the time available. **Needs author or closer manual check before submission.** |
| 17 | "the attributes of God" (book, non-composite-soul context) — SelectionsAbdul, no locator given | Short quoted phrase, general/thematic citation | Checked this session — phrase not found verbatim in Selections from the Writings of 'Abdu'l-Bahá. **Unresolved; needs author check or removal of quotation marks if it's meant as paraphrase.** |

## What this log supports

Every specific correction named in the manuscript's "Declaration of AI-Assisted
Technologies" (main.tex) and in `AI_DISCLOSURE_STATEMENT.md` traces to rows 9, 11, 12,
13, 14, and 15 above. Rows 16–17 are the concrete instances behind that declaration's
caveat that "some ... citations were judged lower risk and not independently
re-verified" — they are not paraphrase citations in general, but these two specific,
named, still-open items.


## Note on this log's own provenance

Item 11's book-wide scope was NOT caught during the original book review pass earlier
in this session — only pub3's two occurrences were found and fixed at that time. It was
caught during compilation of this log, when a routine cross-check ("does the book use
this quote too?") turned up six more instances across three chapters, all carrying the
identical fabricated ending. This is disclosed here rather than silently absorbed into the "verified" count,
because it is itself evidence of the failure mode this log exists to guard against: a
plausible-sounding continuation of a real quotation is easy to miss on a first pass, and
duplicated instances of the same error compound the risk. All six book instances were
corrected before this log was finalized; see `book-physics-of-love` commit history for
the fix.
