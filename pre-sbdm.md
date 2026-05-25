---
layout: no-header
title: 
permalink: "/pre-sbdm"
nav: false
---

<style>
  @import url('https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,600;1,400&family=Source+Serif+4:wght@300;400;600&display=swap');

  :root {
    --moss:       #3B6D11;
    --moss-lt:    #EAF3DE;
    --moss-md:    #639922;
    --bark:       #633806;
    --bark-lt:    #FAEEDA;
    --bark-md:    #BA7517;
    --soil:       #4A2F1A;
    --cream-dk:   #F0EBE1;
    --sand:       #E8DFD0;
    --text:       #2C2218;
    --text-muted: #6B5B4B;
    --border:     rgba(99,56,6,0.15);
  }

  body { background: #ffffff !important; }

  .conf-wrap {
    font-family: 'Source Serif 4', Georgia, serif;
    color: var(--text);
    max-width: 760px;
    margin: 0 auto;
    padding: 0 1.5rem 4rem;
  }

  /* POSTER */
  .poster-wrap { margin: 2rem 0 0; }
  .poster-wrap img { width: 100%; border-radius: 4px; display: block; }

  /* HERO */
  .hero {
    padding: 3rem 0 2.5rem;
    border-bottom: 1.5px solid var(--border);
    margin-bottom: 3rem;
  }
  .hero-eyebrow {
    font-family: 'Source Serif 4', serif;
    font-weight: 300;
    font-size: 0.85rem;
    letter-spacing: 0.14em;
    text-transform: uppercase;
    color: var(--moss);
    margin: 0 0 1rem;
  }
  .hero h1 {
    font-family: 'Playfair Display', Georgia, serif;
    font-size: clamp(2rem, 5vw, 2.9rem);
    font-weight: 600;
    line-height: 1.2;
    margin: 0 0 1.5rem;
    color: var(--soil);
  }
  .hero h1 em { font-style: italic; color: var(--moss); }

  .meta-row { display: flex; flex-wrap: wrap; gap: 1.2rem 2rem; margin-top: 1.5rem; }
  .meta-pill { display: flex; align-items: flex-start; gap: 0.55rem; font-size: 0.92rem; }
  .meta-pill .icon { width: 18px; height: 18px; flex-shrink: 0; margin-top: 2px; color: var(--moss); }
  .meta-pill strong { display: block; font-weight: 600; color: var(--soil); line-height: 1.3; }
  .meta-pill span { color: var(--text-muted); font-weight: 300; font-size: 0.88rem; }

  /* DESCRIPTION */
  .desc {
    font-size: 1.05rem;
    line-height: 1.75;
    color: var(--text);
    font-weight: 300;
    margin-bottom: 2.5rem;
    padding-left: 1.2rem;
    border-left: 3px solid var(--moss-lt);
  }
  .desc p { margin: 0 0 0.8rem; }
  .desc p:last-child { margin: 0; }

  /* REGISTER BUTTON */
  .register-btn {
    display: inline-flex;
    align-items: center;
    gap: 0.5rem;
    background: var(--moss);
    color: #fff !important;
    text-decoration: none !important;
    font-family: 'Source Serif 4', serif;
    font-weight: 600;
    font-size: 0.9rem;
    letter-spacing: 0.04em;
    padding: 0.65rem 1.4rem;
    border-radius: 3px;
    transition: background 0.2s;
    margin-bottom: 3rem;
  }
  .register-btn:hover { background: #27500A; }

  /* SECTION LABELS */
  .section-label {
    font-family: 'Source Serif 4', serif;
    font-weight: 300;
    font-size: 0.75rem;
    letter-spacing: 0.16em;
    text-transform: uppercase;
    color: var(--moss-md);
    margin: 0 0 1.2rem;
  }
  h2.section-title {
    font-family: 'Playfair Display', Georgia, serif;
    font-size: 1.55rem;
    font-weight: 600;
    color: var(--soil);
    margin: 0 0 1.5rem;
    padding-bottom: 0.6rem;
    border-bottom: 1px solid var(--border);
  }

  /* PROGRAM */
  .program { margin-bottom: 3.5rem; }
  .program-block { margin-bottom: 2.4rem; }
  .program-block-title {
    font-family: 'Source Serif 4', serif;
    font-weight: 600;
    font-size: 0.78rem;
    letter-spacing: 0.13em;
    text-transform: uppercase;
    color: var(--bark-md);
    margin: 0 0 0.9rem;
    display: flex;
    align-items: center;
    gap: 0.6rem;
  }
  .program-block-title::after {
    content: '';
    flex: 1;
    height: 1px;
    background: var(--sand);
  }

  /* TABLE-BASED ROWS */
  .prog-table {
    width: 100%;
    border-collapse: collapse;
  }
  .prog-table tr td {
    padding: 0.85rem 0;
    border-bottom: 1px solid var(--cream-dk);
    vertical-align: top;
  }
  .prog-table tr:last-child td { border-bottom: none; }
  .prog-table .t-time {
    font-size: 0.78rem;
    font-weight: 600;
    color: var(--text-muted);
    letter-spacing: 0.04em;
    line-height: 1.5;
    white-space: nowrap;
    width: 80px;
    padding-right: 1rem;
  }
  .prog-table .t-time.break { color: var(--sand); }

  .t-speaker {
    font-family: 'Playfair Display', Georgia, serif;
    font-size: 1rem;
    font-weight: 600;
    color: var(--soil);
    margin: 0 0 0.18rem;
    line-height: 1.35;
  }
  .t-speaker em {
    font-style: normal;
    font-size: 0.78rem;
    font-weight: 400;
    font-family: 'Source Serif 4', serif;
    color: var(--text-muted);
    margin-left: 0.5em;
  }
  .t-title {
    font-size: 0.88rem;
    font-weight: 600;
    color: var(--moss);
    margin: 0 0 0.4rem;
    line-height: 1.45;
  }
  .t-break-label {
    font-size: 0.78rem;
    font-style: italic;
    color: var(--sand);
    letter-spacing: 0.02em;
  }

  details summary {
    cursor: pointer;
    color: var(--moss-md);
    font-weight: 600;
    font-size: 0.78rem;
    letter-spacing: 0.03em;
    list-style: none;
    display: inline-flex;
    align-items: center;
    gap: 0.3em;
    margin-top: 0.3rem;
  }
  details summary::-webkit-details-marker { display: none; }
  details summary::before { content: '▸ '; }
  details[open] summary::before { content: '▾ '; }
  details p {
    font-size: 0.82rem;
    font-weight: 300;
    color: var(--text-muted);
    line-height: 1.65;
    margin: 0.5rem 0 0;
    padding: 0.6rem 0.8rem;
    background: #f7f4f0;
    border-left: 2.5px solid var(--moss-lt);
    border-radius: 0 3px 3px 0;
  }

  /* PARTICIPANTS */
  .participants { margin-bottom: 3.5rem; }
  .participant-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
    gap: 0.75rem;
    margin-bottom: 2rem;
  }
  .participant-card {
    background: #f7f4f0;
    border: 1px solid var(--border);
    border-radius: 4px;
    padding: 0.75rem 1rem;
  }
  .participant-card .p-name {
    font-family: 'Playfair Display', serif;
    font-weight: 600;
    font-size: 0.93rem;
    color: var(--soil);
    margin: 0 0 0.18rem;
    line-height: 1.3;
  }
  .participant-card .p-affil {
    font-size: 0.75rem;
    font-weight: 300;
    color: var(--text-muted);
    line-height: 1.4;
    margin: 0;
  }

  /* ORGANIZERS */
  .organizers { margin-bottom: 3rem; }
  .org-list { display: flex; flex-wrap: wrap; gap: 0.6rem 1.8rem; list-style: none; padding: 0; margin: 0; }
  .org-list li { font-size: 0.9rem; font-weight: 300; color: var(--text-muted); }
  .org-list li a { color: var(--moss); text-decoration: none; border-bottom: 1px solid var(--moss-lt); transition: border-color 0.15s; }
  .org-list li a:hover { border-color: var(--moss); }

  /* FOOTER */
  .footer-note {
    font-size: 0.8rem;
    font-weight: 300;
    color: var(--text-muted);
    border-top: 1px solid var(--border);
    padding-top: 1.2rem;
    line-height: 1.6;
  }
  .footer-note a { color: var(--moss); }

  @media (max-width: 520px) {
    .prog-table .t-time { width: 56px; padding-right: 0.6rem; }
    .participant-grid { grid-template-columns: 1fr 1fr; }
  }
</style>

<div class="conf-wrap">

<div class="poster-wrap">
  <img src="other/Poster_CogSciClimate2026.pdf" alt="Conference poster">
</div>

<header class="hero">
  <p class="hero-eyebrow">Pre-conference seminar · SBDM 2026</p>
  <div class="meta-row">
    <div class="meta-pill">
      <svg class="icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><rect x="3" y="4" width="18" height="18" rx="2"/><line x1="16" y1="2" x2="16" y2="6"/><line x1="8" y1="2" x2="8" y2="6"/><line x1="3" y1="10" x2="21" y2="10"/></svg>
      <div><strong>Tuesday, 26 May 2026</strong><span>9:00 – 17:00</span></div>
    </div>
    <div class="meta-pill">
      <svg class="icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><path d="M12 21C12 21 5 14 5 9a7 7 0 0114 0c0 5-7 12-7 12z"/><circle cx="12" cy="9" r="2.5"/></svg>
      <div><strong>École Normale Supérieure</strong><span>Salle Doussane · 45 rue d'Ulm, Paris</span></div>
    </div>
  </div>
</header>

<section>
  <p class="section-label">About the seminar</p>
  <div class="desc">
    <p>This one-day seminar brings together researchers from cognitive (neuro)science, social psychology, behavioral science, and computational modelling to explore how cognitively informed models of decision-making can advance sustainability and climate action.</p>
    <p>The program features keynote talks in the morning, followed by flash talks and facilitated group discussions in the afternoon designed to spark collaborations and build connections across disciplines. If you're interested in participating in the afternoon panel, please contact the organisers.</p>
    <p>This meeting is a pre-conference seminar in relation to <a href="https://sbdm2026.sciencesconf.org" style="color:var(--moss);">SBDM 2026</a>.</p>
  </div>
  <a class="register-btn" href="https://www.eventbrite.com/e/billets-decision-making-science-for-climate-change-and-sustainability-1983064682849?aff=oddtdtcreator">Register — free admission ↗</a>
</section>

<section class="program">
  <p class="section-label">Programme</p>
  <h2 class="section-title">Tuesday 26 May 2026</h2>

  <div class="program-block">
    <p class="program-block-title">Welcome</p>
    <table class="prog-table"><tbody>
      <tr>
        <td class="t-time">9:00</td>
        <td><p class="t-speaker">Walk-in with coffee</p></td>
      </tr>
      <tr>
        <td class="t-time">9:30</td>
        <td>
          <p class="t-speaker">Anne Urai <em>Leiden University</em></p>
          <p class="t-title">Introduction &amp; Welcome</p>
        </td>
      </tr>
    </tbody></table>
  </div>

  <div class="program-block">
    <p class="program-block-title">Individual decision-making</p>
    <table class="prog-table"><tbody>
      <tr>
        <td class="t-time">9:40–10:10</td>
        <td>
          <p class="t-speaker">Stefano Palminteri <em>ENS Paris</em></p>
          <p class="t-title">Correcting misconceptions and shaping preferences about energy with reinforcement learning</p>
          <details><summary>Read abstract</summary><p><em>Abstract coming soon.</em></p></details>
        </td>
      </tr>
      <tr>
        <td class="t-time">10:10–10:40</td>
        <td>
          <p class="t-speaker">Aurore Grandin <em>ENS Paris</em></p>
          <p class="t-title">Time discounting and environmental engagement</p>
          <details><summary>Read abstract</summary><p>Climate change and other environmental issues represent resource dilemmas that combine social and temporal dimensions. Addressing these challenges requires understanding how individuals balance present needs with future consequences. Research in psychology and behavioural economics has focused on how people value the future through concepts like time preferences, time discounting, and psychological distance. A consistent finding is that a greater orientation towards the future is positively associated with pro-environmental attitudes and behaviours. Investigating the determinants of time preferences could therefore shed light on factors that also influence environmental engagement. I will review existing literature and present findings from my doctoral research, which focused on socioeconomic predictors of time preferences. </p></details>
        </td>
      </tr>
      <tr>
        <td class="t-time">10:40–10:50</td>
        <td>
          <p class="t-speaker">Ali Shiravand <em>ENS Paris</em></p>
          <p class="t-title">NORMARL: A Multi-Agent Reinforcement Learning Framework for Adaptive Social Norms in Resource Sustainability</p>
          <details><summary>Read abstract</summary><p>Human behavior plays a crucial role in determining the sustainability of common-pool resources, where the misalignment of individual actions and collective goals often leads to overexploitation and resource depletion. Traditional methods, such as taxation and cost-based interventions, typically overlook cognitive mechanisms underlying individual decisions, limiting their effectiveness. We introduce the Norm-ORiented Multi-Agent Reinforcement Learning (NORMARL) framework, integrating psychologically plausible parameters (norm internalization and adaptive learning) to explore resource exploitation dynamics. Our model simulates agents interacting with a shared resource, adapting their behaviors based on feedback regarding normative consumption. Agents optimize their utility by balancing individual and social costs, influencing collective resource dynamics. We demonstrate that increased norm internalization and adaptive learning substantially enhance cooperation, resilience to environmental shocks, and resource sustainability. NORMARL highlights how incorporating cognitive mechanisms into computational models can reveal the potential of educational and behavioral interventions, complementing economic policies to promote sustainable behavior. </p></details>
        </td>
      </tr>
      <tr>
        <td class="t-time break">10:50–11:05</td>
        <td><p class="t-break-label">Coffee break</p></td>
      </tr>
    </tbody></table>
  </div>

  <div class="program-block">
    <p class="program-block-title">Collective behaviour</p>
    <table class="prog-table"><tbody>
      <tr>
        <td class="t-time">11:05–11:35</td>
        <td>
          <p class="t-speaker">Amaury Lambert <em>ENS Paris</em></p>
          <p class="t-title">Modelling social dynamics of sustainable behaviors: The consumption-judgement-reputation game</p>
          <details><summary>Read abstract</summary><p>The environmental transition partly depends on the collective adoption of sustainable behaviors (e.g., eating less red meat). Behaving sustainably is moral but individually costly, with a much delayed payoff, thereby incentivizing free-riding.  We wish to study how social norms (prescriptive and descriptive) emerge from social interactions and whether these internal dynamics are sufficient to promote collective moral behavior in this context. We propose a model where each agent has her own internal moral norm (b as in belief), and her own consumption behavior (a as in action). At each round, some agents optimize their utility, which is a weighted combination of their material interest, their social reputation and their moral influence. Roughly, agent (a,b) receives a benefit from passively disapproving agents who consume a' > b and reciprocally pays a reputation cost to individuals who actively disapprove a > b'. The amount of these transactions depends on how much the moral agent is credible (a<b). Our results show that the population spontaneously breaks into well-defined clusters of agents following the same norm (a,b), different from the norm of other clusters, even when all agents are interchangeable. The most generic pattern is that of two subpopulations, one consuming a lot and the other consuming less but receiving a larger utility from passive disapproval. </p></details>
        </td>
      </tr>
      <tr>
        <td class="t-time">11:35–12:05</td>
        <td>
          <p class="t-speaker">Lucia Bosone <em>Université Gustave Eiffel &amp; Paris Cité</em></p>
          <p class="t-title">Thinking Beyond Crisis: Positive Future Societies and Environmental Engagement</p>
          <details><summary>Read abstract</summary><p>Climate change and other environmental crises require not only individual behavioural changes, but also large-scale collective and societal transformations. Understanding what motivates individuals to support such changes is therefore a major challenge for environmental psychology. Recent research suggests that the ability to imagine positive collective futures, referred to as environmental cognitive alternatives, may represent an important lever for environmental engagement. Environmental cognitive alternatives describe individuals’ perceived ability to envision a future society organised around more sustainable ways of living and interacting with the natural environment. In this talk, I will present theoretical perspectives linking future envisioning, collective efficacy, and behavioural change, and discuss how positive visions of society may help overcome social and temporal dilemmas associated with climate action. I will then present findings from a cross-cultural study conducted in China, the United States, France, and Germany, as well as results from an experimental study comparing the effects of utopian versus dystopian future scenarios on environmental attitudes and intentions.</p></details>
        </td>
      </tr>
      <tr>
        <td class="t-time">12:05–12:15</td>
        <td>
          <p class="t-speaker">Magdalena Sabat <em>Leiden &amp; Amsterdam University</em></p>
          <p class="t-title">Early predictors of social tipping points and the opportunity as intervention targets</p>
          <details><summary>Read abstract</summary><p>Large-scale behavioral change is central to climate change mitigation, yet most policy interventions targeting knowledge, attitudes, and beliefs show negligible to small effects on pro-environmental behavior. Emerging evidence points instead to social cognition as offering more consistently effective levers (i.e. collective action and social norms) suggesting that addressing social dynamics may be a more productive intervention target than individual-level persuasion.
          Social tipping points - the nonlinear transitions by which a minority behavior comes to dominate a population - have become promising mechanisms to facilitate large-scale change. Evidence suggests that once a critical mass of adopters is reached, behaviors can spread through a network without additional intervention. This makes early detection of tipping dynamics an attractive point of leverage: interventions need not reach an entire population to catalyze system-wide change. Yet the cognitive mechanisms underlying these transitions remain poorly understood. In particular, rapid norm change confronts individuals with the need to reconsider established beliefs and prior behaviors, increasing cognitive load, decision uncertainty, and social friction with early adopters. Characterizing the temporal dynamics of this conflict - and designing interventions to alleviate it -  is therefore crucial to facilitating harmonious social change.
          Using an established experimental paradigm designed to elicit social tipping points, a coordination game in which a committed minority gradually challenges an established convention, we measure response times as an implicit measure of decision uncertainty. Preliminary results indicate that decisional conflict increases prior to the tipping point, suggesting that participants register normative ambiguity before updating their choices. A computational model incorporating trend-seeking, coordination, and inertia further reveals that trend-seeking specifically precedes the onset of nonlinear diffusion, mirroring the temporal profile of the response time signal.
          Together, these findings establish a cognitive signature of the pre-tipping window and open new directions for intervention design, including which strategies may reduce social friction at moments of collective transition.</p></details>
        </td>
      </tr>
      <tr>
        <td class="t-time">12:15–12:30</td>
        <td><p class="t-speaker">Conclusions</p></td>
      </tr>
      <tr>
        <td class="t-time break">12:30–14:30</td>
        <td><p class="t-break-label">Lunch break</p></td>
      </tr>
    </tbody></table>
  </div>

  <div class="program-block">
    <p class="program-block-title">Afternoon panel</p>
    <table class="prog-table"><tbody>
      <tr>
        <td class="t-time">14:30–17:00</td>
        <td>
          <p class="t-speaker">Closed working group</p>
          <p style="font-size:0.82rem;font-weight:300;color:var(--text-muted);margin:0.2rem 0 0;">The afternoon panel is closed. If you're interested in participating, please contact the organisers.</p>
        </td>
      </tr>
    </tbody></table>
  </div>
</section>



<section class="organizers">
  <p class="section-label">Organising committee</p>
  <ul class="org-list">
    <li><a href="https://magdalenasabat.github.io">Magdalena Sabat</a> — University of Leiden &amp; University of Amsterdam</li>
    <li>Ali Shiravand — ENS</li>
    <li><a href="https://anneurai.net">Anne Urai</a> — University of Leiden</li>
    <li><a href="https://sites.google.com/site/stefanopalminteri/">Stefano Palminteri</a> — ENS</li>
  </ul>
</section>

<p class="footer-note">The event is free. <a href="https://www.eventbrite.com/e/billets-decision-making-science-for-climate-change-and-sustainability-1983064682849?aff=oddtdtcreator">Registration via Eventbrite</a> is appreciated. · Pre-conference seminar of <a href="https://sbdm2026.sciencesconf.org">SBDM 2026</a>.</p>

</div>