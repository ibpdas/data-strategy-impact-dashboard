<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>ValueLine: Data Strategy Impact Dashboard - README</title>
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <style>
    :root {
      --bg: #ffffff;
      --bg-alt: #f9fafb;
      --border: #e5e7eb;
      --text-main: #111827;
      --text-muted: #4b5563;
      --accent: #2563eb;
      --accent-soft: #eff6ff;
      --badge-bg: #e0edff;
    }

    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      padding: 24px 16px 40px;
      font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
      background: var(--bg);
      color: var(--text-main);
      line-height: 1.6;
    }

    a {
      color: var(--accent);
      text-decoration: none;
    }

    a:hover {
      text-decoration: underline;
    }

    .container {
      max-width: 920px;
      margin: 0 auto;
    }

    .hero {
      text-align: center;
      margin-bottom: 24px;
    }

    .hero h1 {
      margin: 8px 0;
      font-size: 28px;
      line-height: 1.2;
    }

    .hero p {
      margin: 4px 0 0 0;
      font-size: 14px;
      color: var(--text-muted);
    }

    .badge-link {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      padding: 10px 18px;
      margin-bottom: 12px;
      border-radius: 999px;
      background: var(--accent);
      color: #ffffff;
      font-size: 13px;
      font-weight: 600;
      text-decoration: none;
    }

    .badge-link:hover {
      opacity: 0.95;
      text-decoration: none;
    }

    .badge-link span {
      margin-left: 6px;
      font-size: 12px;
      opacity: 0.9;
    }

    .toc {
      border: 1px solid var(--border);
      border-radius: 10px;
      padding: 14px 16px;
      background: var(--bg-alt);
      margin-bottom: 24px;
      font-size: 14px;
    }

    .toc-title {
      font-weight: 700;
      font-size: 13px;
      text-transform: uppercase;
      letter-spacing: 0.04em;
      color: var(--text-muted);
      margin-bottom: 4px;
    }

    .toc p {
      margin: 0 0 8px 0;
      font-size: 13px;
      color: var(--text-muted);
    }

    .toc ol {
      margin: 0;
      padding-left: 20px;
    }

    .toc li {
      margin: 2px 0;
    }

    h2 {
      margin-top: 28px;
      margin-bottom: 6px;
      font-size: 21px;
    }

    h3 {
      margin-top: 18px;
      margin-bottom: 4px;
      font-size: 16px;
    }

    p {
      margin: 6px 0;
      font-size: 14px;
    }

    ul {
      margin: 6px 0 6px 20px;
      padding: 0;
      font-size: 14px;
    }

    li {
      margin: 2px 0;
    }

    blockquote {
      margin: 10px 0;
      padding: 8px 12px;
      border-left: 3px solid var(--accent);
      background: var(--accent-soft);
      font-size: 14px;
      color: var(--text-muted);
    }

    blockquote p {
      margin: 4px 0;
    }

    .inline-badge {
      display: inline-block;
      padding: 2px 8px;
      border-radius: 999px;
      background: var(--badge-bg);
      color: var(--text-main);
      font-size: 11px;
      font-weight: 600;
      margin-left: 4px;
      vertical-align: middle;
    }

    .status-list {
      list-style: disc;
      padding-left: 20px;
    }

    .footer-talk {
      margin-top: 28px;
      text-align: center;
    }

    .footer-talk a {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      padding: 8px 14px;
      border-radius: 999px;
      border: 1px solid var(--border);
      background: #ffffff;
      font-size: 13px;
      font-weight: 500;
      text-decoration: none;
    }

    .footer-talk a:hover {
      background: var(--bg-alt);
      text-decoration: none;
    }

    .footer-talk span {
      margin-left: 6px;
      font-size: 12px;
      color: var(--text-muted);
    }

    hr {
      border: 0;
      border-top: 1px solid var(--border);
      margin: 20px 0;
    }
  </style>
</head>
<body>
  <div class="container">

    <!-- HERO -->
    <header class="hero">
      <a class="badge-link" href="https://ibpdas.github.io/data-strategy-impact-dashboard/" target="_blank" rel="noopener noreferrer">
        Open Dashboard
        <span>Live demo</span>
      </a>

      <h1>ValueLine: A Clearer Line of Sight from Data to Impact</h1>
      <p>
        A three level causal model to help public sector data leaders explain, track and demonstrate
        data strategy impact in complex or federated organisations.
      </p>
    </header>

    <!-- TOC -->
    <nav class="toc">
      <div class="toc-title">Table of contents</div>
      <p>Use this to scan the model, how it works and how to apply it.</p>
      <ol>
        <li><a href="#concept-in-30-seconds">Concept in 30 seconds</a></li>
        <li><a href="#what-the-model-solves">1. What the model solves</a></li>
        <li><a href="#caveat-scope-and-boundaries">Caveat - scope and boundaries</a></li>
        <li><a href="#regulatory-obligations-vs-strategic-value">Regulatory obligations vs strategic value</a></li>
        <li><a href="#the-three-levels-at-a-glance">2. The three levels at a glance</a></li>
        <li><a href="#leading-signal-and-lagging-indicators">3. Leading, signal and lagging indicators</a></li>
        <li><a href="#executive-decision-box">4. Executive decision box</a></li>
        <li><a href="#measurement-methods">5. Measurement methods</a></li>
        <li><a href="#why-this-model-works">6. Why this model works</a></li>
        <li><a href="#how-the-model-is-used">7. How the model is used</a></li>
        <li><a href="#repository-contents">8. Repository contents</a></li>
        <li><a href="#status">9. Status</a></li>
        <li><a href="#limitations">10. Limitations</a></li>
        <li><a href="#contributing-and-reuse">11. Contributing and reuse</a></li>
        <li><a href="#motivation-for-valueline">12. Motivation for ValueLine</a></li>
      </ol>
    </nav>

    <hr />

    <!-- SECTION: Concept -->
    <section id="concept-in-30-seconds">
      <h2>Concept in 30 seconds</h2>
      <p>
        <strong>ValueLine</strong> shows how Level 1 foundational work shapes Level 2 maturity and Level 3 outcomes.
      </p>
      <p>
        It gives leaders a clear causal chain and a reusable dashboard to compare options, understand time horizons and choose faster paths to value.
      </p>
      <p>
        It shifts conversations from <strong>"Why is value slow?"</strong> to <strong>"Which conditions and levers deliver value now, next and later?"</strong>
      </p>
    </section>

    <!-- SECTION: What the model solves -->
    <section id="what-the-model-solves">
      <h2>1. What the model solves</h2>
      <p>
        Public sector organisations often struggle to show how data strategy activity leads to maturity and outcomes.
      </p>
      <p>
        The root problem is <strong>attribution</strong> - data teams control inputs, but outcomes depend on wider system behaviour.
      </p>
      <p>
        ValueLine structures the story into three causal levels so leaders see:
      </p>
      <ul>
        <li>what delivers value quickly</li>
        <li>what takes longer</li>
        <li>which decisions accelerate progress</li>
      </ul>

      <h3>Level 1 - Build foundational enablers</h3>
      <p>
        Conditions data leaders and federated partners can shape directly. Provides early signals of progress.
      </p>

      <h3>Level 2 - Enable maturity</h3>
      <p>
        Behaviour change that emerges when Level 1 is working. Depends on adoption and leadership reinforcement.
      </p>

      <h3>Level 3 - Influence outcomes</h3>
      <p>
        Public value that becomes measurable later. Depends on system alignment, operational cycles and incentives.
      </p>

      <p>
        <strong>Causal chain:</strong> Level 1 → Level 2 → Level 3.
      </p>
    </section>

    <!-- SECTION: Caveat -->
    <section id="caveat-scope-and-boundaries">
      <h2>Caveat - scope and boundaries</h2>
      <p>
        This dashboard focuses on <strong>direct organisational outcomes</strong> from data strategy work.
      </p>
      <p>
        It is not:
      </p>
      <ul>
        <li>a data valuation framework</li>
        <li>a method for estimating broad social, environmental or economic value</li>
        <li>suited to national or sector-wide strategies with different incentives and value flows</li>
      </ul>
    </section>

    <!-- SECTION: Regulatory -->
    <section id="regulatory-obligations-vs-strategic-value">
      <h2>Regulatory obligations vs strategic value</h2>
      <p>
        Many teams manage data for compliance, audit and legal requirements. This protects integrity and reduces risk.
      </p>
      <p>
        But <strong>compliance is not the same as value</strong>.
      </p>
      <p>
        Strategic data work focuses on the conditions that enable reuse, interoperability, adoption and insight, so that maturity improves and outcomes become achievable.
      </p>
    </section>

    <!-- SECTION: Three levels at a glance -->
    <section id="the-three-levels-at-a-glance">
      <h2>2. The three levels at a glance</h2>

      <h3>Level 1 - Foundational enabler shift</h3>
      <p>Typical shifts include:</p>
      <ul>
        <li>isolated priorities → shared direction</li>
        <li>individual ownership → shared accountability</li>
        <li>fragmented fixes → common platforms and standards</li>
        <li>pockets of innovation → shared practice and reuse</li>
        <li>ad hoc conversations → structured cross functional engagement</li>
      </ul>

      <h3>Level 2 - Maturity shift</h3>
      <p>
        Describes how the organisation behaves when Level 1 foundations begin to take effect, across the six themes in the
        Data Maturity Assessment for Government (2023).
      </p>
      <ul>
        <li><strong>Uses</strong> - reactive reporting to proactive operational and strategic use</li>
        <li><strong>Data</strong> - siloed and inconsistent to coherent, reusable, governed and interoperable</li>
        <li><strong>Leadership</strong> - passive or detached to active sponsorship and expectation setting</li>
        <li><strong>Culture</strong> - sporadic and low confidence to everyday data informed decisions</li>
        <li><strong>Tools</strong> - fragmented to integrated, discoverable and self service</li>
        <li><strong>Skills</strong> - specialist pockets to widespread literacy and continuous development</li>
      </ul>

      <h3>Level 3 - Outcome shift</h3>
      <p>As Level 1 and Level 2 strengthen, public value shifts in predictable ways.</p>
      <ul>
        <li><strong>Financial savings</strong> - isolated wins to sustained, organisation wide efficiencies</li>
        <li><strong>User satisfaction</strong> - anecdotal to measurable, repeatable improvements</li>
        <li><strong>Efficiency gains</strong> - local wins to system wide improvements in core processes</li>
        <li><strong>Time savings</strong> - individual tasks to end to end workflow reductions</li>
        <li><strong>Public good impact</strong> - occasional to continuous contributions to policy and service outcomes</li>
      </ul>
    </section>

    <!-- SECTION: Indicators -->
    <section id="leading-signal-and-lagging-indicators">
      <h2>3. Leading, signal and lagging indicators</h2>
      <p>ValueLine classifies metrics so expectations stay realistic:</p>
      <ul>
        <li><strong>Leading</strong> - early signs that enablers are working (mainly Level 1)</li>
        <li><strong>Signal</strong> - system response and behaviour change (mainly Level 2)</li>
        <li><strong>Lagging</strong> - measurable outcomes and public value (mainly Level 3)</li>
      </ul>

      <blockquote>
        <p><strong>Important: different results move at different speeds</strong></p>
        <p>
          Financial savings from removing duplicate systems, rationalising platforms or tightening licensing and procurement
          can move quickly once Level 1 strategic alignment and leadership decisions are in place.
        </p>
        <p>
          Efficiency gains and time savings typically move at a medium pace as teams improve data quality, adopt shared tools
          and reuse common assets.
        </p>
        <p>
          User satisfaction tends to move more slowly because it depends on behaviour, trust and consistent adoption across many teams.
        </p>
        <p>
          Public good impact takes longest to show because it relies on whole system alignment and sustained use of evidence over time.
        </p>
        <p>
          The ValueLine model makes these pacing differences explicit so expectations stay realistic.
        </p>
      </blockquote>
    </section>

    <!-- SECTION: Exec decision box -->
    <section id="executive-decision-box">
      <h2>4. Executive decision box</h2>
      <p>
        The dashboard includes an <strong>Executive decision box</strong> that brings together what leaders need to act on, rather than just observe.
      </p>
      <p>It highlights:</p>
      <ul>
        <li>top three asks</li>
        <li>key trade offs</li>
        <li>critical dependencies</li>
        <li>confidence levels in the evidence</li>
        <li>forward look priorities</li>
      </ul>
      <p>
        This turns data strategy into specific executive decisions instead of a generic performance commentary.
      </p>
    </section>

    <!-- SECTION: Measurement methods -->
    <section id="measurement-methods">
      <h2>5. Measurement methods</h2>
      <p>
        ValueLine encourages a mixed method approach. No single metric can fully capture value or maturity, so combining
        different perspectives matters.
      </p>

      <h3>Quantitative indicators</h3>
      <ul>
        <li>monthly performance reports</li>
        <li>quarterly senior leadership updates</li>
        <li>adoption and reuse metrics for datasets, models and tools</li>
        <li>API and open data usage analytics</li>
        <li>validated cost and time savings, including Benefit Cost Ratio (BCR) and Net Present Value (NPV)</li>
        <li>CO2 impacts from compute and storage where relevant</li>
      </ul>

      <h3>Qualitative and behavioural insight</h3>
      <ul>
        <li>staff and stakeholder surveys on confidence, trust and usability</li>
        <li>user research and interviews with business teams and partners</li>
        <li>training and community participation patterns</li>
        <li>policy and standards adoption evidence</li>
        <li>case studies and reuse stories that show how data influenced decisions</li>
      </ul>

      <h3>Experimental or counterfactual evidence</h3>
      <ul>
        <li>simple A/B style pilots where appropriate</li>
        <li>before and after comparisons using agreed baselines</li>
        <li>counterfactual analysis to test whether outcomes would have happened anyway</li>
      </ul>

      <p>
        Together these methods provide a balanced view of both <strong>capability building</strong> and
        <strong>value creation</strong>.
      </p>
    </section>

    <!-- SECTION: Why this model works -->
    <section id="why-this-model-works">
      <h2>6. Why this model works</h2>
      <p>
        ValueLine is grounded in a simple systems principle: <strong>foundations shape maturity, and maturity shapes outcomes</strong>.
      </p>
      <p>This reflects how real systems behave:</p>
      <ul>
        <li>foundational and outcome changes move at different speeds</li>
        <li>system behaviour lags behind system investment</li>
        <li>maturity cannot exceed the strength of foundations</li>
        <li>outcomes cannot exceed maturity</li>
        <li>value emerges from alignment, not isolated effort</li>
        <li>progress is iterative, not linear</li>
      </ul>
      <p>
        These principles underpin the structure of the dashboard and the use of leading, signal and lagging indicators.
      </p>
    </section>

    <!-- SECTION: How model is used -->
    <section id="how-the-model-is-used">
      <h2>7. How the model is used</h2>
      <p>ValueLine helps data teams to:</p>
      <ul>
        <li>explain data strategy impact using a clear causal chain</li>
        <li>engage senior leaders with a consistent, repeatable dashboard</li>
        <li>identify where to invest next in Level 1 or Level 2</li>
        <li>align directorates or partners within federated departments</li>
      </ul>
      <p>It is particularly useful for:</p>
      <ul>
        <li>data leadership teams</li>
        <li>portfolio, PMO and governance groups</li>
        <li>strategy, policy and finance partners</li>
        <li>performance and benefits leads</li>
      </ul>
    </section>

    <!-- SECTION: Repository contents -->
    <section id="repository-contents">
      <h2>8. Repository contents</h2>
      <p>This repository provides:</p>
      <ul>
        <li>HTML conceptual dashboard</li>
        <li>methodology explanation</li>
        <li>metric catalogue</li>
        <li>theory of change view</li>
        <li>Excel input template</li>
        <li>PowerPoint generator script</li>
        <li>synthetic example datasets</li>
        <li>light architecture notes</li>
      </ul>
    </section>

    <!-- SECTION: Status -->
    <section id="status">
      <h2>9. Status</h2>
      <ul class="status-list">
        <li>HTML conceptual dashboard - complete</li>
        <li>Excel template - MVP</li>
        <li>PowerPoint generator - MVP</li>
        <li>PowerBI template - MVP</li>
        <li>Streamlit app - planned</li>
      </ul>
    </section>

    <!-- SECTION: Limitations -->
    <section id="limitations">
      <h2>10. Limitations</h2>
      <ul>
        <li>all data in the example is synthetic</li>
        <li>the dashboard is a learning and facilitation tool, not an assurance framework</li>
        <li>it is not a benchmark or official standard</li>
        <li>attribution remains approximate</li>
        <li>evidence quality can vary</li>
        <li>outcomes often lag by years</li>
        <li>maturity scores are directional, not absolute</li>
        <li>real decisions should still rely on your own evidence, governance and professional judgement</li>
      </ul>
    </section>

    <!-- SECTION: Contributing -->
    <section id="contributing-and-reuse">
      <h2>11. Contributing and reuse</h2>
      <p>You are welcome to:</p>
      <ul>
        <li>fork and customise the model</li>
        <li>propose improvements via issues or pull requests</li>
        <li>share alternative layouts or metrics for other public sector teams</li>
      </ul>
      <p>Attribution is optional but appreciated.</p>
    </section>

    <!-- SECTION: Motivation -->
    <section id="motivation-for-valueline">
      <h2>12. Motivation for ValueLine</h2>
      <p>
        ValueLine grew out of experience leading data strategy work in complex, federated environments where strong foundational work was happening,
        but was hard to explain.
      </p>
      <p>
        Across conversations with colleagues and reviews of more than fifty data strategies and business cases, the same pattern appeared:
      </p>
      <blockquote>
        <p>
          Foundational work was progressing, but the story of progress was unclear. Signals arrived late, expectations drifted, and the connection between
          foundations, maturity and outcomes was often lost.
        </p>
      </blockquote>
      <p>
        ValueLine is a practical and repeatable way to make that connection clearer. It reflects years of trial, mistakes, small breakthroughs and
        generous advice from others.
      </p>
      <p>
        If it helps even a few teams focus on what matters and explain their impact with more clarity, it has done its job.
      </p>
      <p><strong>Bandhu P. Das</strong></p>

      <div class="footer-talk">
        <a href="https://www.brighttalk.com/webcast/12405/602410" target="_blank" rel="noopener noreferrer">
          Unlocking the Value of Data
          <span>Conference talk</span>
        </a>
      </div>
    </section>

  </div>
</body>
</html>