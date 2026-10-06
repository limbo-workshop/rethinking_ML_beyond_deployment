+++
title = "LiMBo: Living Clinical Models @ ICLR 2027"
+++

<style>
.topic-grid,
.track-grid,
.people-grid,
.advisor-grid,
.award-grid,
.sponsor-grid,
.proceedings-grid {
    display: grid;
    grid-template-columns: 1fr;
    gap: 1rem;
    margin: 1.5rem 0 2rem;
}

.topic-card,
.track-card,
.person-card,
.advisor-card,
.award-card,
.sponsor-card,
.proceedings-card {
    background: rgba(255, 255, 255, 0.62);
    border: 1px solid rgba(0, 0, 0, 0.08);
    border-radius: 8px;
    padding: 1rem;
}

.topic-card h4,
.track-card h4,
.person-card h4,
.advisor-card h4,
.award-card h4,
.sponsor-card h4,
.proceedings-card h4 {
    margin: 0 0 0.35rem;
}

.topic-card p,
.track-card p,
.person-card p,
.advisor-card p,
.award-card p,
.sponsor-card p,
.proceedings-card p {
    margin: 0;
}

.person-role,
.person-affiliation,
.advisor-affiliation,
.award-status,
.sponsor-note,
.proceedings-note {
    color: #666;
    font-size: 0.92rem;
    line-height: 1.45;
}

.speaker-grid {
    gap: 2.5rem 1.5rem;
}

.advisor-photo-grid {
    gap: 2rem 1.5rem;
}

.organizer-photo-grid {
    gap: 2rem 1.5rem;
}

.speaker-grid .person-card {
    background: transparent;
    border: 0;
    padding: 0.5rem;
    text-align: center;
}

.organizer-photo-grid .person-card {
    text-align: center;
}

.advisor-photo-grid .advisor-card {
    background: transparent;
    border: 0;
    padding: 0.5rem;
    text-align: center;
}

.speaker-photo,
.organizer-photo,
.advisor-photo {
    width: min(220px, 64vw);
    aspect-ratio: 1;
    border-radius: 50%;
    object-fit: cover;
    display: block;
    margin: 0 auto 1rem;
}

.organizer-photo {
    width: min(180px, 58vw);
}

.advisor-photo {
    width: min(190px, 58vw);
}

.speaker-grid .person-card h4 {
    font-size: clamp(1.45rem, 4.8vw, 2rem);
    margin-bottom: 0.6rem;
}

.advisor-photo-grid .advisor-card h4 {
    font-size: clamp(1.25rem, 4vw, 1.65rem);
    margin-bottom: 0.45rem;
}

.organizer-photo-grid .person-card h4 {
    font-size: clamp(1.2rem, 4vw, 1.55rem);
    margin-bottom: 0.45rem;
}

.speaker-grid .person-affiliation {
    color: #333;
    font-size: 1rem;
}

.advisor-photo-grid .advisor-affiliation {
    color: #333;
    font-size: 0.96rem;
}

#schedule table td:first-child,
#schedule table th:first-child {
    white-space: nowrap;
    width: 1%;
}

.pc-grid {
    column-count: 1;
    column-gap: 3rem;
    margin-top: 1.5rem;
}

.pc-member {
    break-inside: avoid;
    margin-bottom: 0.4rem;
}

.pc-affiliation {
    color: #666;
}

.award-card {
    text-align: center;
}

.award-card h4 {
    font-size: clamp(1.15rem, 3.5vw, 1.45rem);
}

.award-status {
    margin-top: 0.75rem;
    font-style: italic;
}

.sponsor-card {
    text-align: center;
}

.sponsor-logo {
    display: block;
    max-width: min(220px, 64vw);
    max-height: 120px;
    object-fit: contain;
    margin: 0 auto 1rem;
}

.proceedings-logo {
    display: block;
    max-width: min(220px, 64vw);
    max-height: 120px;
    object-fit: contain;
    margin: 0 auto 1rem;
}

.proceedings-mark {
    align-items: center;
    border: 1px solid rgba(0, 0, 0, 0.1);
    border-radius: 8px;
    display: inline-flex;
    font-size: 1.4rem;
    font-weight: 700;
    justify-content: center;
    margin-bottom: 0.9rem;
    min-height: 4rem;
    min-width: 8rem;
    padding: 0.5rem 1rem;
}

@media (min-width: 760px) {
    .topic-grid,
    .track-grid,
    .people-grid,
    .advisor-grid,
    .award-grid,
    .sponsor-grid,
    .proceedings-grid {
        grid-template-columns: repeat(2, 1fr);
    }
}

@media (min-width: 1000px) {
    .topic-grid,
    .people-grid {
        grid-template-columns: repeat(3, 1fr);
    }

    .organizer-photo-grid {
        grid-template-columns: repeat(2, 1fr);
    }

    .pc-grid {
        column-count: 2;
    }
}
</style>

---

<section id="about">

## About {#about}

Standard ML evaluation assumes a stationary world: a fixed test distribution, a fixed dataset, and a fixed notion of correctness. Deployed clinical systems violate all three. Patient populations drift, hardware and protocols evolve, individual records may need to be removed, and clinician feedback continually reshapes what counts as a correct prediction.

LiMBo brings together researchers working on adaptable, maintainable, and interactive machine learning systems for healthcare. We focus on post-deployment behavior: models that can adapt under distribution shift, support verifiable unlearning, expose uncertainty, and be audited or corrected through human feedback without destabilizing learned behavior.

Our goal is to build shared problem formulations, evaluation protocols, and benchmarks for healthcare ML systems that change over time. The workshop is method-first, with healthcare as the stress test: data scarcity, privacy withdrawal, clinical oversight, safety constraints, and regulation make post-deployment reliability unavoidable.

### Topics

<div class="topic-grid">
<div class="topic-card"><h4>Continual and Test-Time Adaptation</h4><p>Methods for models that update under changing patient populations, clinical workflows, hardware, and acquisition protocols.</p></div>
<div class="topic-card"><h4>Machine Unlearning</h4><p>Privacy-compliant removal of patient data, auditability, and verifiable guarantees under limited clinical data.</p></div>
<div class="topic-card"><h4>Interactive Model Steering</h4><p>Clinician feedback, preference-based updates, counterfactual interventions, and concept-level control.</p></div>
<div class="topic-card"><h4>Post-Deployment Evaluation</h4><p>Benchmarks and protocols for distribution shift, continual adaptation, unlearning audits, and human-in-the-loop systems.</p></div>
<div class="topic-card"><h4>Trustworthy Clinical Deployment</h4><p>Robustness, calibrated uncertainty, monitoring, regulatory constraints, and safe lifecycle management.</p></div>
<div class="topic-card"><h4>Clinical Translation</h4><p>Work that connects core ML methods with real-world clinical settings, deployment constraints, and clinician oversight.</p></div>
</div>

</section>

---

<section id="key-info">

## Key Info {#key-info}

### Important Dates

Please note that all deadlines are Anywhere on Earth (AOE).

- **Call for papers and OpenReview submission portal open:** December 7, 2026
- **Submission deadline:** February 1, 2027
- **Author notification:** February 22, 2027
- **Camera-ready deadline:** March 19, 2027
- **Talk titles and full schedule public:** March 26, 2027
- **Workshop date:** April 29 or 30, 2027, at ICLR 2027 in San Francisco (exact day to be announced)

### Format

The workshop will feature invited talks, selected spotlight talks, Tiny Papers lightning talks, two poster sessions, a moderated panel, an open Q&A discussion, and closing awards. Reviewing will be double-blind via OpenReview, with at least three reviews per submission and conflict-of-interest handling at both organizer and reviewer levels.

</section>

---

<section id="call-for-papers">

## Call for Papers {#call-for-papers}

We invite submissions on machine learning methods and clinical translations for systems that must remain reliable after deployment. Relevant topics include, but are not limited to:

- Continual and lifelong learning for evolving clinical populations
- Test-time adaptation and domain adaptation in healthcare
- Machine unlearning for privacy-compliant patient withdrawal
- Robustness to hardware, site, protocol, and population shifts
- Clinician-in-the-loop model steering and auditing
- Counterfactual reasoning and concept-level interventions
- Post-deployment monitoring, uncertainty, and lifecycle evaluation
- Benchmarks for adaptation, unlearning, steering, and clinical drift

### Submission Tracks

<div class="track-grid">
<div class="track-card"><h4>Tiny Papers</h4><p>Up to 4 pages for early-stage ideas, negative results, position pieces, and focused technical contributions, with priority for emerging and under-represented authors.</p></div>
<div class="track-card"><h4>Proceedings Track</h4><p>Up to 8 pages for full, unpublished work forming the core scientific program through posters and selected spotlights.</p></div>
<div class="track-card"><h4>Datasets & Benchmarks Track</h4><p>Up to 8 pages for curated datasets, standardized post-deployment evaluation protocols, reproducible benchmarks, and baselines.</p></div>
</div>

Proceedings-track and Datasets & Benchmarks papers are planned for a dedicated PMLR workshop volume. We are also exploring an editorial summarizing the scientific outcomes and research agenda of the workshop.

### Review

- **Review model:** Double-blind
- **Platform:** OpenReview
- **Anonymization:** Required for all submissions
- **Reviews:** At least three reviews per submission
- **Conflicts:** Organizers and reviewers will recuse themselves from conflicted submissions

</section>

---

<section id="accepted-papers">

## Accepted Papers {#accepted-papers}

</section>

---

<section id="proceedings">

## Proceedings {#proceedings}

Accepted papers in the Proceedings Track and the Datasets & Benchmarks Track will be included in a dedicated PMLR workshop volume. The volume will include a distinct Datasets & Benchmarks section for curated datasets, standardized post-deployment evaluation protocols, reproducible benchmarks, and baselines.

We are also in discussion with TMLR for an editorial that summarizes the scientific outcomes of the workshop and the research agenda it sets for adaptable, auditable, and interactive machine learning in healthcare.

<div class="proceedings-grid">
<div class="proceedings-card"><img class="proceedings-logo" src="img/proceedings/logo-pmlr.svg" alt="PMLR logo"><h4>Dedicated Workshop Volume</h4><p class="proceedings-note">Confirmed for Proceedings Track papers and a distinct Datasets & Benchmarks section.</p></div>
<div class="proceedings-card"><img class="proceedings-logo" src="img/proceedings/tmlr.jpg" alt="TMLR logo"><h4>Editorial Discussion</h4><p class="proceedings-note">Potential editorial summarizing workshop outcomes and the resulting research agenda.</p></div>
</div>

</section>

---

<section id="awards">

## Awards {#awards}

We plan to recognize outstanding contributions and reviewing through the following awards. Awardees will be announced after the workshop review and presentation process.

<div class="award-grid">
<div class="award-card"><h4>Best Paper Award (600 USD)</h4><p>Recognizing the strongest accepted contribution to post-deployment machine learning for healthcare.</p><p class="award-status">Awardee to be announced.</p></div>
<div class="award-card"><h4>Best Presentation Award (400 USD)</h4><p>Recognizing the clearest and most engaging spotlight or lightning talk presented at the workshop.</p><p class="award-status">Awardee to be announced.</p></div>
<div class="award-card"><h4>Best Presentation Runner-Up (350 USD)</h4><p>Recognizing an additional outstanding talk from the workshop program.</p><p class="award-status">Awardee to be announced.</p></div>
<div class="award-card"><h4>Best Poster Award (300 USD)</h4><p>Recognizing the most compelling poster presented during the poster sessions.</p><p class="award-status">Awardee to be announced.</p></div>
<div class="award-card"><h4>Best Poster Runner-Up (225 USD)</h4><p>Recognizing an additional outstanding poster from the poster sessions.</p><p class="award-status">Awardee to be announced.</p></div>
<div class="award-card"><h4>Best Reviewer Award (75 USD)</h4><p>Recognizing exceptional reviewing quality, constructiveness, and service to the double-blind review process.</p><p class="award-status">Awardee to be announced.</p></div>
<div class="award-card"><h4>Best Reviewer Runner-Up (50 USD)</h4><p>Recognizing an additional reviewer whose feedback substantially supports authors and the program committee.</p><p class="award-status">Awardee to be announced.</p></div>
</div>

Awards total 2,000 USD. In addition, we will offer travel and registration support to 10-15 students and early-career researchers with financial need, prioritizing applicants from underrepresented or under-resourced backgrounds.

</section>

---

<section id="schedule">

## Schedule {#schedule}

| Time | Theme / Session | Lead / Speaker |
| --- | --- | --- |
| 09:00-09:15 | Opening Remarks | Organizers |
| 09:15-10:30 | ML adaptation & uncertainty | Theme block |
| 09:15-09:35 | Invited Talk I | Razvan Pascanu |
| 09:40-10:00 | Invited Talk II | Yarin Gal |
| 10:00-10:15 | Spotlight Talk I - Selected Submission | Presenter 1 |
| 10:15-10:30 | Spotlight Talk II - Selected Submission | Presenter 2 |
| 10:30-11:15 | Coffee Break & Poster Session I | Poster Presenters |
| 11:15-12:50 | Clinical deployment under shift | Theme block |
| 11:15-11:35 | Invited Talk III | Enzo Ferrante |
| 11:40-12:00 | Invited Talk IV | Olivier Salvado |
| 12:05-12:50 | Panel Discussion | Moderators / Panelists |
| 12:50-14:00 | Lunch & Networking | - |
| 14:00-15:15 | Auditing dynamic clinical ML | Theme block |
| 14:00-14:20 | Invited Talk V | Irene Chen |
| 14:25-14:40 | Spotlight Talk III - Selected Submission | Presenter 3 |
| 14:40-14:55 | Spotlight Talk IV - Selected Submission | Presenter 4 |
| 14:55-15:15 | Tiny Papers Lightning Talks | Tiny Papers Presenters |
| 15:15-16:00 | Coffee Break & Poster Session II | Poster Presenters |
| 16:00-16:15 | Open Q&A and Discussion | Session Chair |
| 16:15-16:30 | Closing Remarks & Awards | Organizers |

</section>

---

<section id="speakers">

## Confirmed Speakers {#confirmed-speakers}

<div class="people-grid speaker-grid">
<div class="person-card"><img class="speaker-photo" src="img/speakers/irene-chen.jpeg" alt="Irene Chen"><h4>Irene Chen</h4><p class="person-affiliation">UC Berkeley, US</p><p class="person-role">Speaker & Panelist</p></div>
<div class="person-card"><img class="speaker-photo" src="img/speakers/enzo-ferrante-centered.jpeg" alt="Enzo Ferrante"><h4>Enzo Ferrante</h4><p class="person-affiliation">Universidad de Buenos Aires, AR</p><p class="person-role">Speaker & Panelist</p></div>
<div class="person-card"><img class="speaker-photo" src="img/speakers/razvan-pascanu.jpeg" alt="Razvan Pascanu"><h4>Razvan Pascanu</h4><p class="person-affiliation">Google DeepMind and Mila, Canada</p><p class="person-role">Speaker & Panelist</p></div>
<div class="person-card"><img class="speaker-photo" src="img/speakers/olivier-salvado.jpeg" alt="Olivier Salvado"><h4>Olivier Salvado</h4><p class="person-affiliation">Queensland University of Technology, AU</p><p class="person-role">Speaker & Panelist</p></div>
<div class="person-card"><img class="speaker-photo" src="img/speakers/yarin-gal.jpeg" alt="Yarin Gal"><h4>Yarin Gal</h4><p class="person-affiliation">University of Oxford, UK</p><p class="person-role">Speaker & Panelist</p></div>
</div>

</section>

---

<section id="organizers">

## Organizers {#organizers}

<div class="people-grid organizer-photo-grid">
<div class="person-card"><img class="organizer-photo" src="img/organizers/samuel-ruiperez-campillo.jpeg" alt="Samuel Ruiperez-Campillo"><h4>Samuel Ruiperez-Campillo</h4><p class="person-affiliation">Massachusetts Institute of Technology, US</p><p class="person-role">Executive Co-Chair & Scientific Co-Chair</p></div>
<div class="person-card"><img class="organizer-photo" src="img/organizers/silke-muehlstedt.jpeg" alt="Silke Muehlstedt"><h4>Silke Muehlstedt</h4><p class="person-affiliation">ETH Zurich, CH</p><p class="person-role">Executive Co-Chair & Scientific Co-Chair</p></div>
<div class="person-card"><img class="organizer-photo" src="img/organizers/cristina-almagro-perez.jpeg" alt="Cristina Almagro-Perez"><h4>Cristina Almagro-Perez</h4><p class="person-affiliation">Harvard-MIT HST and Brigham and Women's Hospital, US</p><p class="person-role">Operations & Program Delivery Chair</p></div>
<div class="person-card"><img class="organizer-photo" src="img/organizers/sonia-laguna.jpeg" alt="Sonia Laguna"><h4>Sonia Laguna</h4><p class="person-affiliation">Apple, FR</p><p class="person-role">Program Committee & External Relations Chair</p></div>
</div>

### Senior Advisory Board

<div class="advisor-grid advisor-photo-grid">
<div class="advisor-card"><img class="advisor-photo" src="img/advisors/joelle-barral.jpeg" alt="Joelle Barral"><h4>Joelle Barral</h4><p class="advisor-affiliation">Senior Director of Research & Engineering, Google DeepMind, FR</p></div>
<div class="advisor-card"><img class="advisor-photo" src="img/advisors/yun-sing-koh.jpeg" alt="Yun Sing Koh"><h4>Yun Sing Koh</h4><p class="advisor-affiliation">Professor, University of Auckland, NZ</p></div>
<div class="advisor-card"><img class="advisor-photo" src="img/advisors/rajesh-ranganath-centered.jpeg" alt="Rajesh Ranganath"><h4>Rajesh Ranganath</h4><p class="advisor-affiliation">Professor, New York University, US</p></div>
<div class="advisor-card"><img class="advisor-photo" src="img/advisors/julia-vogt.jpeg" alt="Julia Vogt"><h4>Julia Vogt</h4><p class="advisor-affiliation">Associate Professor, ETH Zurich, CH</p></div>
</div>

</section>

---

<section id="program-committee">

## Program Committee Members {#program-committee}

To be included after double-blind review.

</section>

---

<section id="contact">

## Contact {#contact}

- General inquiries: <calmagroperez@hst.harvard.edu>

</section>

---

<section id="sponsors">

## Sponsors {#sponsors}

We gratefully acknowledge the support of our sponsors. Sponsor funds will go directly toward workshop awards and participant support.

<div class="sponsor-grid">
<div class="sponsor-card"><img class="sponsor-logo" src="img/quantco_logo.png" alt="QuantCo logo"><h4>QuantCo</h4><p class="sponsor-note">Confirmed sponsor supporting awards and participant support.</p></div>
<div class="sponsor-card"><h4>Additional Sponsorship</h4><p class="sponsor-note">Additional support is under discussion and will be added here once confirmed.</p></div>
</div>

</section>
