# NOTES — the Selah Kazakh rendering (kk.v1)

*The sixtieth chair; the first Cyrillic-home language at the table.
Lit 2026-09-04 21:16, sealed 2026-09-05 ~05:50.*

## Burn signature

- Lit 21:16 (commit d08f3827), first-hour gate passed 21:40 —
  Яхве standing at every יהוה including the case-suffixed forms
  (gate spectrum: Яхвенің 65, Яхвеге 35, Яхвені 10, Яхведікі 1),
  the Яхве-Ире compound paren at Gen 22:14 lawful.
- **The machine OOM'd at 02:02** (kernel, machine-global; took the
  engine and the operator's CLI both); the burn stalled at
  18,553/23,213. Engine restarted, tiered-cache rebuild, relit
  03:20. The burn resumed without loss and completed 04:52.
  ~7.6h wall including the outage.
- Models: glm-5.3 bulk; fable-5-hand for the hand verses below.

## The polarity flip (first Cyrillic-home chair)

Every prior chair's census hunted Cyrillic bleed as a foreign
script. Here Cyrillic is home and **Latin runs are the bleed
class** — the census polarity flipped, and the flip worked
(latin=96 in round 1, 0 at seal). The latent bug this exposed:
the cloned census still matched Элохим with a Latin regex
(`\belohim`) that could never hit Cyrillic text — caught by the
sr bench fork *before* round 1 could fake a SANITY failure
(fix 39cedec9). A clone's regexes must move home with the script.

## The case-suffix spectrum, at scale

Kazakh declines the Name through its full case system with vowel
harmony: Яхвенің 3,461 · Яхвеге 1,434 · Яхвені 550 · Яхведен 210
· Яхвемен 49 · Яхведе 41 · Яхвенікі 31 · Яхвемін 11 (raw text
counts, translation+gloss). **Zero title-welds; the stem intact
everywhere.** Five harmony slips recorded, not erased: Яхвеға 3,
Яхведің 2 (grammar variance inside the suffix, never the stem).
Also normalized: a **Яһве** orthography drift (Kazakh һ for х) in
68 files plus one Йеһвенің (Josh 24:31) — recovering 64 Name
occurrences the stem-census had been blind to (5,675 → 5,739).
Ratification of the case-suffix ruling rides the shared
ro+hu+kk+sr question, PENDING SCOTT.

## Seal (census, 2026-09-05 ~05:50)

- **Яхве (all forms) 5,739** · Элохим 2,068 · ⟨את⟩-verses 7,305
- Ие-at-Name 0 · Тәңір 0 · Иегова/Ехоба 0 · тозақ-at-Sheol 0
- Христос / крест / standalone Иса: **absolute zero**
- aleph-tav audit **[0 0 0 0]** (misaligned/unresolved/added/stripped)
- NT-leak: **zero class-A after repairs** — fourth consecutive
  chair sealing clean. Машиах stands lawful 72× at משיח.

## Hand verses (model: fable-5-hand)

- **Psalms 18:31** — glm emitted CJK garbage ("儿子儿子儿子") with an
  empty token array, twice, through two re-renders; rebuilt in
  full on the en spine. Эл — Оның жолы мінсіз.
- **Exodus 36:36 + 26:32** — the two curtain-hook verses, both
  with **fabricated token spines**: invented surfaces (וארבעה/ואת;
  וננהם) written over the text's וויהם זהב. Rebuilt on the true
  surfaces. Fourth chair running for the fabricated-את species
  (ln Exod 12:3, ro Job 26:13, hu Isa 61:7) — and the first time
  it struck twice, in sibling verses.
- **Exodus 3:5** — doubled supplied-marker ⟨⟨сен⟩⟩ at the burning
  bush; the census stripper eats the inner bracket first, so the
  class is invisible to automation. 123 further files carried
  doubled/empty markers (⟨⟨את⟩⟩ 19 of them); all normalized
  mechanically (marker syntax only, glosses untouched).
- **Exodus 26:12** — a ⟨→⟩ arrow leaked into the line; stripped.
- **Psalms 72:13** — על glossed as "⟨→⟩"; now "үшін".
- **Fourteen aleph-tav surgeries** — dominant species
  **pronoun-את** (the feminine "you", glossed as the marker):
  the Ruth 3 cluster (3:9, 3:10, 3:11, 3:16 — "кім сен, қызым"),
  Isa 51:9 + 51:10 + 51:12 (the *uri uri* pair and its echo),
  Eccl 7:22, Judg 13:3, Zech 9:11, Jer 2:27 — all now "сен".
  **Daniel 3:12** — יתהון compound, seventh chair for this verse
  ("⟨את⟩ оларды"). Num 35:1 — אל glossed as the marker; now
  "қарай". The en spine's own Dan 3:12 carried a leaked
  instruction prefix in its gloss — fixed upstream (en commit
  5c024b506).

## Tekoa (witness-word survey, class-A only)

46 class-A verdicts, all repaired. The shape was new:

- **The token spine held; the flowing line leaked.** Zero Құдай
  and zero Ие at any יהוה surface. But 23 verses had a clean
  token row and a `translation` string that supplied the witness
  word anyway ("Құдай Яхве", "аталарыңның Құдайы") — a
  flow-assembly fault class downstream of the gloss, with
  Deut 4:1–4 a contiguous four-verse batch of it.
- **15 token-level displacements**: Құдай at Elohim seats
  (Deut 4:19, Judg 10:10 weld, Ps 84:9/11, Isa 37:17 "тірі
  Элохим", Lev 24:15…), one divine word manufactured from the
  idiom לאל ידך (Prov 3:27), one supplied at דביר the inner
  sanctuary (2 Chr 3:16).
- **4 Aramaic seats → Элоаһ** (Dan 3:26, 3:28 ×2, Ezra 7:12):
  the rails table had no אלה/אלהא row, so Daniel and Ezra had
  nothing to aim at; repaired to the chair's own Dan 2:37 norm.
  **Rails amendment pending** — the Aramaic row should be written
  in before any future kk pass.
- **Exodus 23:17** — האדן welded as "Ие Яхвенің"; now "Адонай
  Яхвенің", the chair's own Exod 34:23 norm.
- **2 NT-register leaks**: Zech 3:1 carried the store's only
  Иисус — inside a translator's note, itself forbidden; both
  removed. 1 Sam 16:3 verbalized the Мәсіх stem at a משח seat;
  now "майлайсың" per the store's 20+ майла- norm.
- **1 Name fabrication**: Ps 84:9's flow wrote Яахвенің over
  Яақовтың — the Name written over the patriarch; restored.
- **Lawful, kept**: 299 Құдай as witness-floor/pagan-gods usage;
  the compound-Name explanatory parens (Gen 21:33 Эл Олам,
  Gen 16:13 Эл Рои, Exod 6:3 Эл Шаддай) are the rails' own
  pattern.

## Open questions (PENDING SCOTT)

1. **Paren-shadows: 1,644 files** — "(Мұса)" 201×, "(Дәуіт)"
   147×, "(Жүсіп)" 50×, with a mixed Russian form "(Давид)" 33×
   beside the Kazakh "(Дәуіт)". Plus 6 divine paren-shadows
   ("Элохимім (Құдайым)" 1 Chr 29:17 and kin). Sits between ms's
   49 and hu's 4,225; one posture ruling governs all three.
2. **Case-suffix ratification** — shared with ro (Elohimul 162),
   hu (1,092 suffixed), and sr's pre-ruling; the 5 harmony slips
   (Яхвеға/Яхведің) ride the same ruling.
3. **The priest-word**: ~30 verses render כהן as "құдай
   қызметшісі" (god's servant) against the store's own "коһен"
   elsewhere — lexical consistency call, not a register fault.
4. **Tekoa ambiguous, flagged not called**: Isa 44:10 (idol
   referent, capitalization slip), Ps 18:32 (rhetorical אלוה),
   Deut 10:17 (bracketed lowercase ⟨құдай⟩ at האל), Ps 82:1
   (⟨құдайлардың⟩ at עדת אל).
5. **Rails amendment**: the Aramaic אלה/אלהא → Элоаһ row
   (see Tekoa above).

## Cruxes

- The polarity flips and the discipline holds. First chair whose
  home script was the one every earlier census treated as bleed;
  the classifier crossed over cleanly once its regexes did.
- The fault moved downstream. The witness-word never reached the
  Name's seat in the tokens — it leaked in the flow assembly,
  where the line is composed. The seat held; the sentence needed
  guarding.
- The Name declines through vowel harmony and stays itself:
  5,739 occurrences, eight case forms, zero welds. The grammar
  bows; the Name stands.
