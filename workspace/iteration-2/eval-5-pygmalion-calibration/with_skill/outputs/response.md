Short answer: "real and well-established" is stronger than the evidence supports, and "Rosenthal and Jacobson proved it" is wrong in the technical sense. There is a real but small effect hiding behind a famous-but-methodologically-troubled original study. Let me unpack.

## Claims I'm parsing

1. **The Pygmalion effect is real** (teacher expectations causally shift student performance).
2. **It is well-established.**
3. **The 1968 Rosenthal & Jacobson "Pygmalion in the Classroom" study proved it.**

These are not the same claim, and they do not all survive scrutiny equally.

## Evidence, per claim

**Claim 3 — "Rosenthal and Jacobson proved it": weak.**
The original 1968 study (random subset of elementary students labeled "intellectual bloomers," teachers told to expect a growth spurt, IQ gains compared to controls) has serious methodological problems that were raised almost immediately and have never really been answered:

- **IQ test artifacts.** Robert Thorndike's 1968 review of the study pointed out that the Flanagan TOGA test was being used outside its normed range; mean "reasoning IQ" in some control classrooms fell into the intellectually-disabled range, which is facially implausible. His line — roughly, "when the clock strikes thirteen, it casts doubt on all the previous strikes" — is the canonical critique.
- **Regression to the mean.** The biggest "gains" were in the youngest children and lowest-scoring classrooms, which is exactly what you'd expect from measurement error on a noisy instrument regardless of any expectancy effect.
- **Reporting problems.** Snow (1969) and others documented inconsistencies between tables and text, incomplete analyses, and overclaimed conclusions.
- **Failure to replicate cleanly.** Early attempts at direct replication mostly didn't find the effect, or found it much smaller.

So "Rosenthal and Jacobson proved it" is not how the literature reads. It's how the *textbook summary* reads.

**Claim 1 — "The effect is real": qualified yes, but small and narrower than the myth.**
This is where the picture gets more interesting, and where I'd push back on anyone who says the whole thing is bunk.

- **Raudenbush (1984)** meta-analyzed 18 randomized teacher-expectancy experiments. Key finding: the effect on pupil IQ depended heavily on *when* the expectancy was induced. When teachers had known the students for **two weeks or more before the manipulation**, the effect was ~zero. When the manipulation hit in the first two weeks (teachers still forming impressions), there was a real effect. Mechanistically that makes sense — a false label can't override two weeks of direct observation. It also means the Rosenthal-style "tell teachers a random kid is a bloomer" design only works in a narrow window.
- **Jussim & Harber (2005)**, *Personality and Social Psychology Review*, reviewed ~35 years of research. Their summary, which is now the mainstream position among researchers who work on this directly: self-fulfilling prophecies in classrooms *do* occur, but effect sizes are typically small (roughly r = .1-.2, d ≈ .3), they do *not* accumulate across teachers or years (if anything they dissipate), and the correlation between teacher expectations and student outcomes is mostly explained by teacher expectations being **accurate** (teachers correctly perceiving which students are struggling), not by expectations *causing* the outcomes. Roughly 40% shared variance between teacher judgments and actual achievement is accuracy, not prophecy.
- **de Boer, Timmermans & van der Werf (2018)**, *Educational Research and Evaluation*, meta-analyzed 19 teacher-expectation *intervention* studies. Hedges' g ≈ 0.38 on teacher expectations and ≈ 0.30 on student achievement. Small-to-moderate, real, but nowhere near the "24.8 IQ points" framing from the original.
- **One genuinely important caveat** Jussim & Harber flag: effects may be **larger for students from stigmatized groups** (low-SES, racial minorities, students with prior low achievement). This is the live research question. It matters for policy even if the average effect is small, because averages hide where the effect concentrates.

**Claim 2 — "Well-established": depends what you mean.**
- The *cultural* Pygmalion effect — "high teacher expectations dramatically transform student IQ" — is folklore, not science. It's a textbook simplification of a contested study.
- The *actual* finding — "teacher expectations exert a small causal influence on student outcomes, mostly at the start of the teacher-student relationship, possibly larger for stigmatized students, but most of the expectation-outcome correlation reflects accurate teacher perception" — is reasonably well-established.

## Steelman of your position

The strongest defense of "real and well-established": the original study, whatever its flaws, launched a legitimate research program. Fifty years later, with better designs and meta-analysis, we still find non-zero effects in the direction Rosenthal predicted. The de Boer et al. meta-analysis of *intervention* studies (which is the causally cleanest design) gives g ≈ 0.30 on achievement, which is not trivial in education-research terms. Raudenbush's moderator finding — effect present in the first two weeks — isn't a refutation; it's a mechanism. And Jussim, who is among the most skeptical voices on self-fulfilling prophecies generally, *still* concludes the effect is real, just modest. On that reading, "real" is correct; "well-established" is defensible; only "Rosenthal and Jacobson proved it" is clearly overstated.

I think this steelman is partly right — specifically on "real." I don't think it rescues "well-established" at the strength the original framing suggests, and it doesn't rescue the original study.

## Verdict

**Calibrated:**
- "Teacher expectations have some causal effect on student outcomes" — **yes, with small effect sizes (d ≈ 0.2-0.3)**. Evidence level: multiple meta-analyses of RCT-style interventions. Reasonably established.
- "The Pygmalion effect as popularly described — big, reliable transformations of student IQ from teacher expectancy alone" — **no, that's not what the evidence shows.** The effect is small, conditional on timing, and most of the teacher-expectation / student-outcome correlation is explained by teacher accuracy rather than prophecy.
- "Rosenthal and Jacobson proved it" — **no.** The 1968 study has well-documented methodological problems (IQ-test misuse, regression to the mean, reporting issues) and failed direct replications. The *concept* survived; *that particular study* did not earn the canonical status it has in textbooks.

The most interesting live question in the current literature isn't "does it exist" but "is it concentrated in stigmatized-group students?" — where some evidence suggests effects may be considerably larger than the average, though this is still being worked out.

## What would change my verdict

- A well-powered pre-registered replication of the original Pygmalion design finding the large effect Rosenthal claimed — would upgrade the original study's standing. (This basically hasn't happened in 50+ years.)
- A meta-analysis restricted to pre-registered, low-risk-of-bias studies showing d substantially larger than 0.3 — would upgrade "real but small" to "real and substantial."
- Strong longitudinal evidence that small per-year effects *accumulate* across grades into large cumulative effects — would change the policy significance even if the annual effect stays small. Jussim & Harber currently argue against this; a well-designed study reversing them would matter.
- Evidence that the stigmatized-group moderator is robust and large — would change the distributional interpretation even if the population average stays small.

## Sources

- Rosenthal, R., & Jacobson, L. (1968). *Pygmalion in the Classroom*. [Wikipedia overview](https://en.wikipedia.org/wiki/Pygmalion_in_the_Classroom)
- Thorndike, R. L. (1968). Review of *Pygmalion in the Classroom*. *American Educational Research Journal* — critique of IQ test use. See [Spitz (1999) historical review](https://gwern.net/doc/iq/1999-spitz.pdf) for the controversy.
- Snow, R. E. (1969). [A Case Study in Statistical Inference](https://files.eric.ed.gov/fulltext/ED046892.pdf) — methodological critique.
- Raudenbush, S. W. (1984). Magnitude of teacher expectancy effects on pupil IQ as a function of the credibility of expectancy induction. [Meta-analysis PDF](https://gwern.net/doc/statistics/bias/1984-raudenbush.pdf).
- Jussim, L., & Harber, K. D. (2005). Teacher Expectations and Self-Fulfilling Prophecies. *Personality and Social Psychology Review*, 9, 131-155. [PDF](http://nwkpsych.rutgers.edu/~kharber/publications/Jussim.&.Harber.2005.%20Teacher%20Expectations%20and%20Self-Fulfilling%20Prophesies.pdf) / [PubMed](https://pubmed.ncbi.nlm.nih.gov/15869379/).
- de Boer, H., Timmermans, A. C., & van der Werf, M. P. C. (2018). [The effects of teacher expectation interventions on teachers' expectations and student achievement: narrative review and meta-analysis](https://www.tandfonline.com/doi/full/10.1080/13803611.2018.1550834). *Educational Research and Evaluation*, 24(3-5).
- [Cumming, "We've Been Here Before: The Replication Crisis over the Pygmalion Effect"](https://thenewstatistics.com/itns/2018/04/03/weve-been-here-before-the-replication-crisis-over-the-pygmalion-effect/) — accessible summary of the replication history.
