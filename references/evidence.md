# Evidence behind the rules

Read this only when you need to justify a choice, explain why the skill behaves as it does, or decide between two rules that conflict. Labels: **Supported** = meta-analyses or randomized trials in a relevant population. **Promising** = real but limited evidence, or evidence from other settings. **Heuristic** = design practice, expert guidance or theory without direct outcome tests.

The most important limit: no study has tested this way of writing explanations, with an AI, for people with ADHD. Every rule below is an extrapolation from research on ADHD cognition, general learning science, accessibility guidance or AI tutoring. Do not tell users the skill is clinically validated.

## What the research says about ADHD (why the skill adapts instead of assuming)

- Group differences are real but moderate: across 34 meta-analyses, mean d = 0.45; working memory about 0.54. https://pubmed.ncbi.nlm.nih.gov/29106438/
- Individuals vary widely: no single neurocognitive measure was impaired in more than half of ADHD cases (Nigg et al. 2005, summarized by Doyle 2006). https://psychiatrist.com/read-pdf/6907
- Memory difficulties in adults arise mostly at encoding, not retrieval. https://journals.sagepub.com/doi/10.1177/1087054713510561
- Readers with ADHD recalled fewer central ideas although they judged centrality correctly. https://cris.biu.ac.il/en/publications/the-origin-of-the-centrality-deficit-in-individuals-with-attentio-4/
- Spontaneous mind wandering is strongly linked to ADHD symptoms. https://featuredcontent.psychonomic.org/not-all-minds-that-wander-are-lost-adhd-and-the-types-of-mind-wandering
- Inattention predicts procrastination (small non-clinical sample). https://www.epanlab.nl/wp-content/uploads/2017/05/Niermann-Scheres-2014.pdf
- Emotion dysregulation is large in adult ADHD (g = 1.17). https://doaj.org/article/559c71e475cc4cd2a6228b2e9c2f75a8

## Rule-by-rule evidence

| Rule in SKILL.md | Evidence | Key source |
| --- | --- | --- |
| Answer first | Heuristic | NN/g scanning research https://nngroup.com/articles/f-shaped-pattern-reading-web-content/ ; centrality-deficit data above |
| One idea per segment, labeled by its point | Supported (general), Heuristic (ADHD) | Segmenting meta-analysis https://is.tuebingen.mpg.de/publications/rey2018segmenting ; signaling d = .38 https://rex.libraries.wsu.edu/esploro/outputs/journalArticle/A-meta-analysis-of-signaling-principle-in/99900601052901842 |
| Cut what does not explain | Supported | Seductive details, 58 studies https://news.wsu.edu/2020/03/19/seductive-details-inhibit-learning/ ; overview of 29 reviews https://acuresearchbank.acu.edu.au/item/8zqy4/multimedia-design-for-learning-an-overview-of-reviews-with-meta-meta-analysis |
| Name parts before the mechanism | Supported (few tests) | Pre-training principle, median d = 0.85 https://www.cambridge.org/core/books/abs/multimedia-learning/pretraining-principle/01791D57F5D4164251269E6DF56A8BF1 |
| Hold it on the page | Heuristic, grounded in working-memory data | https://pubmed.ncbi.nlm.nih.gov/15782085/ ; W3C COGA https://www.w3.org/TR/coga-usable/ |
| Match the user's level; skip basics for experts | Supported | Expertise reversal https://www.uky.edu/~gmswan3/EDC608/Kalyuga2007_Article_ExpertiseReversalEffectAndItsI.pdf |
| Start mode: one small step, no roadmap | Heuristic | Procrastination correlates https://prism.ucalgary.ca/items/d0dea740-4751-4e9a-84da-2d8ad446830d/full ; CBT task chunking https://pmc.ncbi.nlm.nih.gov/articles/PMC3874265 ; NICE NG87 https://www.nice.org.uk/guidance/ng87 |
| One concrete next step | Supported (general), fragile in ADHD lab work | If-then plans d = .65 https://kops.uni-konstanz.de/entities/publication/2e749bfb-8533-437c-8203-7e788c910c5f ; ADHD study https://www.socmot.uni-konstanz.de/sites/default/files/08_Gawrilow_Gollwitzer_Implementation_intentions_facilit.pdf |
| Recommend one option | Promising | Choice overload moderators https://www.kellogg.northwestern.edu/academics-research/research/detail/2015/when-product-assortment-leads-to-choice-overload-a-conceptual/ |
| Worked examples, then fading | Supported | Math g = 0.48 https://oaks.kent.edu/hcri/meta-analysis-worked-examples-effect-mathematics-performance ; subgoal labels https://scholarworks.gsu.edu/ltd_facpub/3 |
| Concrete before abstract | Promising | https://learningscientists.org/blog/2018/2/1-1 |
| Analogies with stated limits | Heuristic | Teaching-With-Analogies https://www.csun.edu/~vceed002/books/sourcebook/chapters/10-analogies/teaching-analogies.html |
| Recall questions in Practice and multi-session work | Supported, including college students with ADHD | https://www.psychologicalscience.org/journals/clinical/2167702614565175/ ; https://www.frontiersin.org/journals/psychology/articles/10.3389/fpsyg.2023.1186566/full |
| Spaced review across sessions | Supported | https://www.evullab.org/pdf/CepedaPashlerVulWixtedRohrer-PB-2006.pdf |
| Self-explanation as an option | Supported (g = 0.55) | https://bps.org.uk/research-digest/self-explanation-powerful-learning-technique-according-meta-analysis-64-studies |
| Interleave only to tell similar types apart | Promising | https://www.psychologie.uni-wuerzburg.de/fileadmin/06020400/2019/Brunmair_Richter_in_press__2019_META-ANALYSIS_OF_INTERLEAVED_LEARNING.pdf |
| Refute misconceptions explicitly | Supported (g = 0.41; 0.28 bias-adjusted) | https://link.springer.com/article/10.1007/s10648-021-09656-z |
| No "Does that make sense?" | Supported (feeling of learning misleads) | https://openlab.citytech.cuny.edu/gamelab/files/2023/01/Deslauriersa-et-al-2019.pdf |
| Specific, neutral feedback; no praise inflation | Supported (d = 0.99 vs 0.24) | https://www.frontiersin.org/articles/10.3389/fpsyg.2019.03087/full |
| Resume with explicit state | Promising | Resumption cues https://interruptions.net/literature/Trafton-IJHCS03.pdf ; tendency to resume https://ideas.repec.org/a/pal/palcom/v12y2025i1d10.1057_s41599-025-05000-w.html |
| Scaffold when learning is the goal; answer when an answer is needed | Supported | Unrestricted AI hurt later exams https://ideas.repec.org/a/nas/journl/v122y2025pe2422633122.html ; structured AI tutor RCT https://pmc.ncbi.nlm.nih.gov/articles/PMC12179260/ |
| Problem-first challenge only for engaged learners | Promising | https://futurity.org/?p=2629782 |
| Causal story framing for history | Promising | https://www.aft.org/periodical/american-educator/summer-2004/ask-cognitive-scientist |
| Action-first procedures with error recovery | Promising (older usability studies) | https://www.psy.gla.ac.uk/~steve/MinMan2.html |

## Known gaps

- No trials of explanation formats for ADHD readers, in text or chat.
- Multimedia findings come mostly from short lab lessons with non-ADHD students and narrated animations.
- AI tutoring trials used general student populations and specific, carefully built tutors.
- ADHD generative-AI research so far is design studies, not efficacy trials.
- Hyperfocus, "interest-based" motivation and similar popular ideas have little controlled research; the skill does not rely on them.
