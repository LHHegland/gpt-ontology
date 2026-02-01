# File Header

- **Name**: GPT RBI Humanity OODA 
- **Version**: 2026-01-31 06:01 UTC by LHH
- **Purpose**: TBD 
- **Features**
  - TBD
- **Scope**
  - TBD
- **Use Cases**
  - **Supported**
    - TBD
  - **Not Supported**
    - TBD


# Relevant Background Information


## Index

Common human topic references mapped to canonical handles (i.e., IDs and namespaced tags). Use canonical tags in prompts (e.g., [[HUMANITY:RESOURCES]]).
- Processing (OODA: Observe → Orient → Decide →  Act) → HUMANITY.ELEMENTS.OODA → [[HUMANITY:OODA]]
- Observe → HUMANITY.ELEMENTS.OODA.OBSERVE → [[HUMANITY:OBSERVE]] 
- Senses → HUMANITY.ELEMENTS.OODA.OBSERVE.SENSES → [[HUMANITY:SENSES]]
- Orient → HUMANITY.ELEMENTS.OODA.ORIENT → [[HUMANITY:ORIENT]]
- Decide → HUMANITY.ELEMENTS.OODA.DECIDE →  [[HUMANITY:DECIDE]]


### Primary File Index

Common human topic reference and canonical handle (i.e., ID and namespaced tag) mapped to primary knowledge file:
- 'GPT RBI Humanity 202601310149.md' → Humanity  → HUMANITY → [[HUMANITY:ROOT]]


## Humanity


### Elements


#### Processing (OODA: Observe → Orient → Decide →  Act)

ID: HUMANITY.ELEMENTS.OODA
TAGS: [[HUMANITY:OODA]] [[OODA]]

**Processing (OODA)** is a repeating control loop that converts **current signals** into a **next action** and then updates based on results.
- **Examples**
  - **Driving in traffic (seconds loop):** You observe brake lights → orient (rain + merge) → decide (slow + increase following distance) → act (ease off gas) → observe again.
  - **Grocery shopping on a budget (minutes loop):** You observe prices + pantry state → orient (payday timing; cash limits) → decide (swap to store brands; prioritize staples) → act (change items; track total) → observe again.
  - **Work message that feels rude (minutes loop):** You observe wording + tone cues → orient (intent unclear; stress possible) → decide (clarify, do not escalate) → act (ask one neutral question; delay reply if needed) → observe again.
  - **Caregiving during a kid’s public meltdown (minutes loop):** You observe cues (tired/hungry/overstimulated) → orient (safety + regulation first) → decide (step outside + snack/water) → act (move to quiet place; offer water) → observe again.
  - **Severe weather alert (hours loop):** You observe warnings → orient (your location; timing; risk) → decide (charge phones; alter travel; shelter plan) → act (prepare kit; leave early/relocate if needed) → observe again.
- **Inputs (MUST define or approximate):**
  - **Stimuli:** external signals (environment, other people, systems) + internal signals (body, emotions, thoughts).
  - **Constraints:** [[HUMANITY:RESOURCES]], [[HUMANITY:FALLIBILITY]].
  - **Aims:** [[HUMANITY:NEEDS]] being protected/satisfied + [[HUMANITY:VALUES]] guiding tradeoffs + [[HUMANITY:MISSION]] performed adequately and efficiently to contribute to [[HUMANITY:VISION]].
- **Procedure**
  - **Inputs**
    - 3–7 concrete stimuli
    - 1–3 aims (needs/values/mission priorities).
    - Key constraints (time, energy, money, safety, social/reputation risk).
  - **Actions**
    1. **[[HUMANITY:OBSERVE]]:** List signals; label unknowns explicitly.
    2. **[[HUMANITY:ORIENT]]:** Build a working model (most likely + 1–2 alternatives); list assumptions.
    3. **[[HUMANITY:DECIDE]]:** Choose the next smallest safe step; set a stop/adjust condition.
    4. **[[HUMANITY:ACT]]:** Execute (do/say/stop/ask/leave/defer); prefer reversible actions under uncertainty.
    5. **Repeat:** [[HUMANITY:OBSERVE]] outcomes; update model; optionally record one [[HUMANITY:LESSONS]] item.
  - **Outputs (MUST produce at least one):**
    - **Action:** a concrete behavior/communication change (do, say, stop, ask, leave, defer) (e.g., [[HUMANITY:ACTIVITIES]]).
    - **Updated model:** revised understanding of what is happening ([[HUMANITY:ORIENT]]) and what to do next.
    - **Optionally:** a captured [[HUMANITY:LESSONS]] note/checklist to improve future loops.
- **Boundaries / Scope**
  - **Includes:** rapid micro-loops (seconds) and slower loops (hours/days) as long as the sequence remains: [[HUMANITY:OBSERVE]] → [[HUMANITY:ORIENT]] → [[HUMANITY:DECIDE]] → [[HUMANITY:ACT]] → repeat ([[HUMANITY:OBSERVE]] again)
  - **Excludes:** one-time plans that do not update from feedback; purely “thinking” without an action; “acting” without any attempt to notice outcomes (no re-observation and no updated model); endless re-analysis that prevents a safe next step.
  - **Primary purpose:** reduce avoidable harm and wasted effort by enforcing structured sense-making and response under changing conditions.
- **Decision Rules**
  - **If observations are low-quality or contradictory, THEN** return to [[HUMANITY:OBSERVE]] and gather at least one more data point before deciding.
  - **If stakes are high (safety, major money, reputation, relationships), THEN** slow the loop: add verification, add a pause, and seek a second perspective ([[HUMANITY:INTERDEPENDENCE]]).
  - **If you feel strong urgency/anger/fear, THEN** insert a regulation pause (breathe, draft-not-send) before Decide/Act.
  - **If you cannot act now, THEN** act by choosing a safe placeholder (pause, ask for clarification, exit unsafe situation) and schedule the next loop.
  - **If outcomes differ from expectation, THEN** treat that as new input and re-orient; do not defend the old plan.
- **Ontological Relationships**
  - **Includes/Excludes**
    - **Includes:** [[HUMANITY:OBSERVE]], [[HUMANITY:ORIENT]], [[HUMANITY:DECIDE]], and [[HUMANITY:ACT]] (in that order).
    - **Excludes:** static planning without feedback; action without re-observation; thinking without action.
  - **Related to:** [[HUMANITY:THINKING]], [[HUMANITY:VALUES]], [[HUMANITY:REGULATION]], [[HUMANITY:INTERDEPENDENCE]].
  - **Requires / Required by**
    - **Requires:** [[HUMANITY:RESOURCES]] (at minimum time + energy) to run the loop; [[HUMANITY:THINKING]] to reduce inference errors.
    - **Required by:** reliable performance of [[HUMANITY:ACTIVITIES]] under changing conditions.
  - **Affects / Affected by**
    - **Affects:** quality of performed [[HUMANITY:ACTIVITIES]] and therefore likelihood of satisfying [[HUMANITY:NEEDS]].
    - **Affected by:** depletion (low time/energy), stress, and poor signal quality.
  - **Vulnerable to / Creates Vulnerabilities for**
    - **Vulnerable to:** [[HUMANITY:FALLIBILITY]] and [[HUMANITY:TEMPTATIONS]] (especially when [[HUMANITY:RESOURCES]] are low).
    - **Creates vulnerabilities for:** overconfidence if [[HUMANITY:ORIENT]] is treated as certainty; paralysis if action is avoided.
  - **Reduces Risks for / Risks Reduced by**
    - **Risk reduction (SHOULD):** align decisions/actions with intentional and consistent practice of [[HUMANITY:VALUES]]; use [[HUMANITY:INTERDEPENDENCE]] for high-stakes loops to reduce avoidable harm and escalation risk.
    - **Risks reduced by:** stronger observation quality, verification, regulation pauses, and feedback-based updating.
- Examples of [[HUMANITY:FALLIBILITY]]
  - **Observe error (missing/distorted input):** You skim a headline while tired and “observe” a false claim; every later step inherits the error.
  - **Orient error (assumption/bias):** You interpret a stranger’s neutral face as hostile and orient toward threat; you escalate needlessly.
  - **Decide error (stress impulsivity):** You feel anxious and decide too fast (send the angry text; accept a bad deal) to reduce discomfort.
  - **Act error (execution failure):** You choose the right action (pay bill, take meds) but forget because attention/energy are depleted.
  - **Update failure (stuck loop):** New evidence shows your approach is not working, but pride/fatigue keeps you repeating the same action.
- Examples of Using [[HUMANITY:VALUES]]
  - **Add a deliberate pause before Decide/Act (SHOULD):** Use one breath, a 10-second rule, or “draft but don’t send” for charged messages to reduce impulsive harm ([[HUMANITY:REGULATION]]; [[HUMANITY:TEMPERANCE]]).
  - **Run an orientation humility check (SHOULD):** Ask: “What else could be true?” and “What evidence would change my mind?” to counter assumption-lock ([[HUMANITY:HUMILITY]]; [[HUMANITY:OPEN_MINDEDNESS]]).
  - **Use basic verification for important choices (SHOULD):** Confirm time/place/amount; check original sources; separate “observed” from “inferred” ([[HUMANITY:THINKING]]).
  - **Close the loop with a micro after-action review (MAY):** “What happened? What did I miss? What will I change next time?” and capture one [[HUMANITY:LESSONS]] item (a checklist or rule).
  - **Use [[HUMANITY:INTERDEPENDENCE]] for high-stakes decisions (SHOULD):** Ask a trusted person to sanity-check your Observe/Orient/Decide before acting; treat feedback as new observation ([[HUMANITY:INTERDEPENDENCE]]; [[HUMANITY:WISDOM]]).


##### Observe

ID: HUMANITY.ELEMENTS.OODA.OBSERVE
TAGS: [[HUMANITY:OBSERVE]] [[OBSERVE]]

**Observe** is the repeating practice of **noticing and gathering information** about what is happening **outside you** (environment, people, systems) and **inside you** (body state, emotions, thoughts) using [[HUMANITY:SENSES]]. The purpose is to produce **reliable inputs** for [[HUMANITY:ORIENT]] and the rest of [[HUMANITY:OODA]]. Because of [[HUMANITY:FALLIBILITY]], observation MUST include basic error-checking (missing, distorted, or biased signals).
- **Examples**
  - **Driving/commuting (seconds):** You notice brake lights, lane changes, road slickness, and your own fatigue level.
  - **Doctor visit / caregiving (minutes):** You track symptoms (pain, fever, mood), note what changed since yesterday, and notice side effects after medication.
  - **Work or shift job (minutes):** You scan the task list, watch incoming messages, notice bottlenecks, and catch small errors before they compound.
  - **Online shopping / budgeting (minutes):** You check total price, shipping time, return policy, and your bank balance, and you notice an impulse to overspend.
  - **Kids / classroom / caregiving (minutes):** You notice tone of voice, hunger/tired cues, escalating frustration, and your own stress level.
- **Procedure**
  - **Inputs (MUST define or approximate):**
    - **External signals:** what you can directly see/hear/measure (traffic, messages, numbers, alerts, behavior, weather).
    - **Internal signals:** body state (sleep, hunger, pain), emotions, urges, attention level.
    - **Context constraints:** time available, safety risk, cost/reputation risk, cognitive load ([[HUMANITY:RESOURCES]]).
    - **Uncertainty markers:** what you do not know; what might be wrong or incomplete ([[HUMANITY:FALLIBILITY]]).
  - **Actions (DO in order):**
    1. **Collect signals:** Write 3–7 concrete observations as facts (no interpretation words like “obvious,” “rude,” “safe”).
    2. **Label unknowns:** List 1–3 unknowns explicitly (missing data, unclear intent, unverified numbers).
    3. **Separate observed vs inferred:** Mark what you directly perceived vs what you are guessing.
    4. **Check for distortion:** Identify one likely error source (fatigue, stress, distractions, prior beliefs, low-quality media).
    5. **Improve signal quality (as needed):**
       - If low stakes: gather one more data point OR proceed with a reversible step.
       - If high stakes: verify one critical fact (time, amount, source, location, safety condition).
    6. **Hand off to [[HUMANITY:ORIENT]]:** Provide the observation list + uncertainty markers.
  - **Outputs (MUST produce at least one):**
    - **Observation set:** a short list of concrete signals (facts) + labeled unknowns.
    - **Reliability notes:** at least one flagged distortion risk (e.g., “tired,” “angry,” “unverified source”).
    - **Optional:** a captured [[HUMANITY:LESSONS]] note (e.g., “verify totals before checkout”).
- **Boundaries / Scope**
  - **Includes:** internal + external sensing; quick scans and careful checks; re-observation after new events.
  - **Excludes:** interpretation-only narratives (“they hate me”); conclusions without signals; “research” that never results in a usable observation set.
  - **Primary purpose:** produce **higher-quality inputs** for [[HUMANITY:ORIENT]] and reduce downstream error in the [[HUMANITY:OODA]] loop.
- **Constraints**
  - Observation quality is limited by [[HUMANITY:RESOURCES]] (time, energy, attention) and [[HUMANITY:FALLIBILITY]].
  - Under stress, you SHOULD assume you are missing something and gather at least one additional signal before committing to a high-impact action.
  - Observation MUST remain grounded in what is available now; do not invent data to “complete the picture.”
- **Decision Rules (IF/THEN)**
  - **IF** you cannot list at least 3 concrete observations, **THEN** return to collecting signals before proceeding.
  - **IF** sources conflict or key facts are unverified, **THEN** gather one more data point or verify the most important fact.
  - **IF** stakes are high (health, safety, major money, legal, relationship rupture), **THEN** slow down: verify, document, and consider a second set of eyes ([[HUMANITY:INTERDEPENDENCE]]).
  - **IF** you notice strong emotion (anger, panic, shame), **THEN** add a regulation step (pause/breathe) before trusting your observations.
  - **IF** new evidence appears, **THEN** treat it as higher-priority input and update the observation set immediately.
- **Ontological Relationships**
  - **Includes/Excludes**
    - **Includes:** sensing + recording signals + labeling uncertainty.
    - **Excludes:** orientation, judgment, and action selection (these belong to [[HUMANITY:ORIENT]] / [[HUMANITY:DECIDE]]).
  - **Related to:** [[HUMANITY:SENSES]] (signal acquisition), [[HUMANITY:THINKING]] (verification and inference control), [[HUMANITY:REGULATION]] (reduces distortion under stress).
  - **Requires / Required by**
    - **Requires:** [[HUMANITY:SENSES]] and minimal [[HUMANITY:RESOURCES]] (attention/time).
    - **Required by:** [[HUMANITY:ORIENT]] (needs observation inputs); overall [[HUMANITY:OODA]] quality.
  - **Affects / Affected by**
    - **Affects:** accuracy of [[HUMANITY:ORIENT]] and quality of downstream decisions/actions.
    - **Affected by:** fatigue, distraction, emotional arousal, misinformation exposure, time pressure ([[HUMANITY:FALLIBILITY]]).
  - **Vulnerable to / Creates Vulnerabilities for**
    - **Vulnerable to:** attentional lapses, bias, misperception, misleading inputs, bodily depletion.
    - **Creates vulnerabilities for:** overconfidence if uncertainty is not labeled; cascading errors if bad observations feed later steps.
  - **Reduces Risks for / Risks Reduced by**
    - **Reduces risks for:** preventable mistakes from missing/false inputs; escalation from misread cues.
    - **Risks reduced by:** verification, clear “observed vs inferred” separation, and use of [[HUMANITY:INTERDEPENDENCE]] for high-stakes checks.
- **Examples of [[HUMANITY:FALLIBILITY]]**
  - **Attention gaps:** You multitask (work + texts + kids) and miss a key detail (appointment time, stop sign, dosage).
  - **Stress distortion:** When anxious, you notice only threats/insults and overlook neutral facts.
  - **Low-quality inputs:** You treat a viral clip or headline as the full story and stop observing.
  - **Confirmation filtering:** You notice “supporting” evidence and ignore signals that contradict your belief.
  - **Body-state blind spots:** Hunger, poor sleep, pain, or burnout makes internal observation unreliable (“I’m fine” when you are not).
- **Examples of Using [[HUMANITY:VALUES]]**
  - **[[HUMANITY:INTEGRITY]] (reliability over convenience):** You use checklists, reminders, and “review before send” to reduce missed observations.
  - **[[HUMANITY:HUMILITY]] (assumption-audit):** You ask “What might I be missing?” and actively look for one disconfirming signal.
  - **[[HUMANITY:WISDOM]] (long-term consequences):** You slow down for high-stakes situations (sleep on it, re-check, get one more data point).
  - **[[HUMANITY:INTERDEPENDENCE]] (shared verification):** You ask a trusted person to sanity-check numbers, tone, or risk signals before acting.
  - **[[HUMANITY:TEMPERANCE]] + [[HUMANITY:REGULATION]] (impulse control):** You pause when angry or afraid, then re-observe before concluding.


##### Senses

ID: HUMANITY.ELEMENTS.OODA.OBSERVE.SENSES
TAGS: [[HUMANITY:SENSES]] [[SENSES]]

**Senses** are the body’s **signal detectors** that convert **stimuli** (outside the body and inside the body) into **perceptual signals** the brain can interpret. Senses are a primary input to [[HUMANITY:OBSERVE]]. Because of [[HUMANITY:FALLIBILITY]], sensed signals are not automatically reliable; they SHOULD be checked and calibrated during [[HUMANITY:ORIENT]].
- **Examples**
  - **Cooking at home:** You smell something burning, hear a timer, feel heat from the oven, and notice hunger or nausea.
  - **Driving/commuting:** You see brake lights, hear a siren, feel vibration in the steering wheel, and sense dizziness or fatigue.
  - **Crowded store or event:** You hear loud noises, feel jostling, smell strong perfumes, and notice rising anxiety or overstimulation.
  - **Exercise or physical work:** You feel muscle strain, joint position, balance shifts, breathing effort, thirst, and heartbeat changes.
  - **Illness or recovery:** You sense fever/chills, pain location/intensity, appetite loss, shortness of breath, and light sensitivity.
- **Procedure**
  - **Inputs (MUST define or approximate):**
    - **Stimulus source:** external environment OR internal body state (or both).
    - **Sense channel(s):** which detectors are engaged (vision, hearing, touch, etc.).
    - **Context:** lighting, noise, movement, temperature, substances (smoke/chemicals), stress level, fatigue, hydration.
    - **Uncertainty markers:** anything that could distort sensing (low light, loud noise, strong emotion, intoxication, illness).
  - **Actions (DO in order):**
    1. **Identify channel(s):** Name which sense(s) produced the signal (e.g., vision + interoception).
    2. **Describe the raw signal:** State the perception in concrete terms (what you saw/heard/felt), avoiding interpretations (“dangerous,” “rude,” “fine”).
    3. **Check for distortion:** Flag likely error sources (fatigue, stress, distraction, poor conditions, prior expectations).
    4. **Cross-check (SHOULD):** Use a second channel or tool when available:
       - Look again in better light; reduce noise; move closer/farther.
       - Use a measurement tool (thermometer, timer, blood pressure cuff, receipt total, map).
       - Ask another person to confirm in high-stakes contexts ([[HUMANITY:INTERDEPENDENCE]]).
    5. **Hand off to [[HUMANITY:ORIENT]]:** Provide the signal + distortion flags + cross-check results.
  - **Outputs (MUST produce at least one):**
    - **Perceptual signal statement:** “I saw/heard/felt ____.”
    - **Channel label(s):** which senses generated the signal.
    - **Reliability note:** one short flag about conditions/distortion risk.
    - **Optional:** cross-check result or planned verification step.
- **Boundaries / Scope**
  - **Includes:** all sensory channels that generate inputs for [[HUMANITY:OBSERVE]] (external, internal, balance/position).
  - **Excludes:** meaning-making, threat assessment, and action selection (these belong to [[HUMANITY:ORIENT]] / [[HUMANITY:DECIDE]]).
  - **Primary purpose:** provide **raw inputs** for [[HUMANITY:OBSERVE]]; improve downstream accuracy by making channels and reliability explicit.
- **Constraints**
  - Senses can be inaccurate due to environment (noise, low light), body state (fatigue, illness), and cognition/emotion (stress, expectation) ([[HUMANITY:FALLIBILITY]]).
  - Senses provide **signals**, not guarantees. You MUST treat high-stakes perceptions as provisional until verified when feasible.
  - Internal sensing (interoception) varies widely across people and situations; you SHOULD avoid over-trusting a single internal cue when safety is at risk.
* **Decision Rules (IF/THEN)**
  - **IF** the environment is degraded (dark, loud, chaotic), **THEN** increase cross-checking (re-check, change position, use tools).
  - **IF** you feel strong emotion, fatigue, intoxication, or illness, **THEN** treat sensory certainty as lower and slow the loop.
  - **IF** the perception implies immediate safety risk (smoke smell, severe pain, dizziness while driving), **THEN** take a safe stabilizing action first (stop, move away, seek help) and verify after.
  - **IF** another channel conflicts (you smell smoke but see none), **THEN** gather one more data point before concluding (check appliances, ask someone, verify source).
  - **IF** you cannot verify now, **THEN** label it as uncertain and choose a reversible or protective next step.
- **Ontological Relationships**
  - **Includes/Excludes**
    - **Includes:** exteroception, proprioception, vestibular sensing, interoception as signal sources.
    - **Excludes:** [[HUMANITY:ORIENT]] judgments and decisions; those are downstream processes.
  - **Related to:** [[HUMANITY:OBSERVE]] (uses senses), [[HUMANITY:ORIENT]] (evaluates and corrects), [[HUMANITY:FALLIBILITY]] (distortion risk), [[HUMANITY:THINKING]] (verification).
  - **Requires / Required by**
    - **Requires:** functioning sensory channels and minimal attention/time ([[HUMANITY:RESOURCES]]).
    - **Required by:** [[HUMANITY:OBSERVE]] (primary signal acquisition).
  - **Affects / Affected by**
    - **Affects:** [[HUMANITY:OBSERVE]] accuracy; downstream model quality and decisions.
    - **Affected by:** environment conditions, stress, fatigue, substances, illness, and cognitive expectations.
  - **Vulnerable to / Creates Vulnerabilities for**
    - **Vulnerable to:** illusions, misperception, noise, masking, attentional limits, and biased interpretation.
    - **Creates vulnerabilities for:** downstream errors if raw signals are treated as certain facts without calibration.
  - **Reduces Risks for / Risks Reduced by**
    - **Reduces risks for:** missed hazards when channels are actively monitored and cross-checked.
    - **Risks reduced by:** redundancy (multiple channels), tools/measurement, and second-person confirmation in high stakes.
- Examples of [[HUMANITY:FALLIBILITY]]
  - **Low-light error:** You misread a label or medication bottle at night and take the wrong item.
  - **Noise masking:** You miss an announcement or warning because of loud music or crowded space.
  - **Expectation bias:** You “hear attitude” in a neutral tone because you expect conflict.
  - **Stress body misread:** Anxiety feels like a heart problem (or you dismiss real symptoms as “just stress”).
  - **Motion/balance distortion:** You feel dizzy and misjudge stability, increasing fall or driving risk.
- Examples of Using [[HUMANITY:VALUES]]
  - **[[HUMANITY:HUMILITY]]:** You treat first impressions as provisional and actively look for disconfirming signals.
  - **[[HUMANITY:WISDOM]]:** You slow down and verify when the consequence is high (health, safety, major money).
  - **[[HUMANITY:INTEGRITY]]:** You use checklists/tools (labels, timers, measurements) instead of relying on “I’m sure.”
  - **[[HUMANITY:INTERDEPENDENCE]]:** You ask someone else to confirm what you sensed when it matters (smoke source, child fever, confusing instructions).
  - **[[HUMANITY:TEMPERANCE]] + [[HUMANITY:REGULATION]]:** You pause when overstimulated, reduce inputs (quiet/dim), then re-check signals before acting.


##### Orient

ID: HUMANITY.ELEMENTS.OODA.ORIENT
TAGS: [[HUMANITY:ORIENT]] [[ORIENT]]

**Orient** is the repeating step where you **interpret what you [[HUMANITY:OBSERVE]]** by fitting it into context (goals/needs, prior experience, culture, incentives, constraints, emotions, assumptions, and mental models). The purpose is to produce a **working model** of “what is happening” and “what it likely means” that is good enough to support [[HUMANITY:DECIDE]]. Because of [[HUMANITY:FALLIBILITY]], orientation MUST treat interpretations as **hypotheses**, not facts, and SHOULD use [[HUMANITY:VALUES]] (especially [[HUMANITY:THINKING]], [[HUMANITY:HUMILITY]], [[HUMANITY:PERSPECTIVE]], [[HUMANITY:WISDOM]]) to reduce error and harm.
- **Examples**
  - **Short text from a friend (minutes):** You orient by considering context (history, timing, typical tone) before assuming they are upset.
  - **Work feedback/performance review (minutes-hours):** You orient by separating what was said from what it implies about expectations, incentives, and your goals.
  - **Health symptoms (minutes):** You orient by linking symptoms to patterns (sleep, stress, new meds) and deciding what seems urgent vs. monitor.
  - **Family conflict about money (hours):** You orient by identifying underlying needs (security, fairness, respect) and the tradeoffs driving each stance.
  - **News/social media clip (minutes):** You orient by checking what is missing (source, timeline, base rate) and whether the clip is representative.
- **Procedure**
  - **Inputs (MUST define or approximate):**
    - **Observation set:** 3–10 concrete signals from [[HUMANITY:OBSERVE]] (facts + unknowns).
    - **Aims:** relevant [[HUMANITY:NEEDS]] at stake; [[HUMANITY:VALUES]] guiding tradeoffs; any [[HUMANITY:MISSION]] requirement.
    - **Context:** incentives, roles, power dynamics, norms, culture, timeline, prior history, environment constraints.
    - **State flags:** your body/emotion state (stress, fatigue, anger), which can distort interpretation ([[HUMANITY:REGULATION]]).
    - **Risk level:** safety, money, legal, reputation, relationship impact.
  - **Actions (DO in order):**
    1. **Restate observations:** Repeat the key facts in neutral language; keep interpretation separate.
    2. **Generate a primary hypothesis:** Write the most likely explanation of what is happening.
    3. **Generate alternatives (MUST):** Write 1–2 plausible alternatives (including a benign/neutral explanation when appropriate).
    4. **List assumptions:** Identify what you are assuming (intent, causality, base rates, “typical” behavior).
    5. **Bias and harm check (SHOULD):**
       - Check for [[HUMANITY:STEREOTYPES]] or [[HUMANITY:PREJUDICE]] shaping interpretation.
       - Ask: “Would I interpret this the same way if the person were from a different group?”
    6. **Evidence check (SHOULD):**
       - Identify one missing data point that would most reduce uncertainty.
       - If feasible, gather it now (ask a question, check a source, measure).
    7. **Select a working model:** Choose the model that best fits evidence and constraints; label confidence (high/medium/low).
    8. **Hand off to [[HUMANITY:DECIDE]]:** Provide (a) working model, (b) alternatives, (c) top assumption, (d) key uncertainty, (e) suggested verification step.
  - **Outputs (MUST produce at least one):**
    - **Working model:** “What is happening” + “why it might be happening” (hypothesis, not certainty).
    - **Alternative models:** 1–2 plausible alternatives.
    - **Assumption list:** at least one explicit assumption.
    - **Confidence + uncertainty:** a short confidence rating and one key unknown.
    - **Optional:** a [[HUMANITY:LESSONS]] note (e.g., “ask for intent before reacting”).
- **Boundaries / Scope**
  - **Includes:** interpretation, hypothesis generation, assumption identification, bias checks, and selecting a working model based on observed signals.
  - **Excludes:** choosing the action (belongs to [[HUMANITY:DECIDE]]); executing behavior (belongs to [[HUMANITY:ACT]]).
  - **Primary purpose:** reduce misinterpretation by making context, assumptions, and uncertainty explicit before deciding.
- **Constraints**
  - Orientation is inherently model-based and therefore error-prone; you MUST avoid treating your first story as fact.
  - Orientation quality degrades when [[HUMANITY:REGULATION]] is low (anger, panic, shame, exhaustion); you SHOULD slow down in those states.
  - Orientation is a common entry point for [[HUMANITY:STEREOTYPES]] and [[HUMANITY:PREJUDICE]]; you MUST include a basic bias check when people are involved.
  - If you cannot reduce uncertainty, you SHOULD choose a later decision that is lower-risk or reversible.
- **Decision Rules (IF/THEN)**
  - **IF** you cannot cleanly separate “observed” from “interpreted,” **THEN** return to [[HUMANITY:OBSERVE]] and restate facts.
  - **IF** you feel strong emotion or depletion, **THEN** insert a regulation pause and lower confidence in your interpretation.
  - **IF** the interpretation depends on someone’s intent, **THEN** prefer a clarifying question over a confrontational conclusion.
  - **IF** you notice [[HUMANITY:STEREOTYPE]]-based generalizations (“those people always…”), **THEN** stop and rebuild [[HUMANITY:ORIENT]] from direct evidence and base rates.
  - **IF** stakes are high, **THEN** add verification and/or a second perspective ([[HUMANITY:INTERDEPENDENCE]]) before committing.
  - **IF** new evidence arrives, **THEN** update the working model immediately (do not defend the old model).
- **Ontological Relationships**
  - **Includes/Excludes**
    - **Includes:** hypothesis formation, assumption listing, uncertainty labeling, bias checks.
    - **Excludes:** action selection and execution.
  - **Related to:** [[HUMANITY:OBSERVE]] (inputs), [[HUMANITY:DECIDE]] (consumes outputs), [[HUMANITY:THINKING]] (evaluation), [[HUMANITY:PERSPECTIVE]] (frame widening), [[HUMANITY:REGULATION]] (stability), [[HUMANITY:INTERDEPENDENCE]] (second perspective).
  - **Requires / Required by**
    - **Requires:** an observation set with at least minimal quality; enough [[HUMANITY:RESOURCES]] to compare alternatives.
    - **Required by:** [[HUMANITY:DECIDE]] (needs a working model and uncertainty markers).
  - **Affects / Affected by**
    - **Affects:** decision quality, fairness, and downstream conflict risk; quality of [[HUMANITY:ACTIVITIES]].
    - **Affected by:** stress, fatigue, time pressure, social threat, misinformation exposure, and prior beliefs.
  - **Vulnerable to / Creates Vulnerabilities for**
    - **Vulnerable to:** [[HUMANITY:FALLIBILITY]], [[HUMANITY:STEREOTYPES]], [[HUMANITY:PREJUDICE]], motivated reasoning, and overconfidence.
    - **Creates vulnerabilities for:** harm from misattributed intent; escalation; unfair decisions; repeated errors if models do not update.
  - **Reduces Risks for / Risks Reduced by**
    - **Reduces risks for:** impulsive/conflict-driven decisions by clarifying context and uncertainty before acting.
    - **Risks reduced by:** verification, explicit alternatives, bias checks, regulation pauses, and [[HUMANITY:INTERDEPENDENCE]] in high-stakes contexts.
- Examples of [[HUMANITY:FALLIBILITY]]
  - **Misreading tone/intent:** You assume an overwhelmed cashier is rude to you; you escalate a neutral situation into conflict.
  - **Stress tunnel vision:** Under pressure, you orient toward threat or shame and ignore benign explanations; your perspective narrows.
  - **Identity/tribal pull:** You interpret facts to protect group identity (“us vs. them”) instead of seeking accuracy and [[HUMANITY:FAIRNESS]].
  - **Overconfidence from a thin sample:** One bad experience becomes a rule about a whole group, hardening into [[HUMANITY:STEREOTYPES]].
  - **Outdated mental model:** You interpret current realities using a 5–10 year old model (costs, job market, family needs), leading to bad choices.
- Examples of Using [[HUMANITY:VALUES]]
  - **[[HUMANITY:PERSPECTIVE]]:** You ask “What else could be true?” and “What would change my mind?” before committing to an interpretation.
  - **[[HUMANITY:HUMILITY]] + [[HUMANITY:INTEGRITY]]:** You assume you might be wrong, keep claims small, and repair quickly when misinterpretations occur.
  - **[[HUMANITY:THINKING]]:** You treat your first story as a hypothesis; you seek missing context and better evidence, especially online.
  - **[[HUMANITY:INTERDEPENDENCE]]:** You ask a trusted person to sanity-check your interpretation in high-stakes situations.
  - **[[HUMANITY:WISDOM]]:** After a meaningful outcome, you capture one [[HUMANITY:LESSONS]] item to improve future orientation.


##### Decide

ID: HUMANITY.ELEMENTS.OODA.DECIDE
TAGS: [[HUMANITY:DECIDE]] [[DECIDE]]

**Decide** is the repeating step where you **select the next action (or deliberate non-action)** based on [[HUMANITY:OBSERVE]] and [[HUMANITY:ORIENT]]. The purpose is to choose a **specific next step** that balances [[HUMANITY:NEEDS]], [[HUMANITY:RESOURCES]], [[HUMANITY:VALUES]], risks, tradeoffs, and likely consequences. Because of [[HUMANITY:FALLIBILITY]] and [[HUMANITY:TEMPTATIONS]], decisions MUST include a minimum safety check (stakes, reversibility, bias, and verification when feasible).
- **Examples**
  - **Budgeting this week:** You decide whether to pay rent, buy groceries, pay down debt, or cover a surprise expense first.
  - **Work conflict:** You decide to reply now, ask a clarifying question, escalate to a manager, or pause and revisit tomorrow.
  - **Health choice:** You decide to monitor at home, call a nurse line, schedule a visit, or go to urgent care.
  - **Parenting/caregiving:** You decide to set a boundary, redirect attention, offer comfort, or leave an overstimulating place.
  - **Driving in bad weather:** You decide to slow down, change route, pull over, or delay the trip.
- **Procedure**
  - **Inputs (MUST define or approximate):**
    - **Working model:** your best current interpretation + key uncertainty from [[HUMANITY:ORIENT]].
    - **Decision objective:** the primary [[HUMANITY:NEEDS]] to protect/satisfy now.
    - **Constraints:** time, money, energy, capacity ([[HUMANITY:RESOURCES]]); deadlines; safety limits.
    - **Options:** 2–5 feasible actions, including a safe “do nothing yet” option.
    - **Risk and stakes:** safety, health, legal, financial, reputation, relationship impact.
    - **Influences:** [[HUMANITY:MOTIVATORS]] and [[HUMANITY:TEMPTATIONS]] currently active (comfort-seeking, status, fear, anger).
  - **Actions (DO in order):**
    1. **List options:** Write 2–5 concrete next actions (verbs + objects + timing). Include “pause/clarify” when uncertain.
    2. **Check constraints:** Remove options that exceed current resources or violate safety limits.
    3. **Predict consequences (SHOULD):** For each option, note:
       - likely short-term outcome,
       - likely longer-term outcome,
       - worst plausible downside.
    4. **Values check (MUST):** Identify which [[HUMANITY:VALUES]] you are prioritizing (e.g., safety, fairness, honesty, compassion, prudence).
    5. **Bias and discrimination check (SHOULD when people are affected):**
       - Check for [[HUMANITY:STEREOTYPES]] / [[HUMANITY:PREJUDICE]].
       - Ask: “Would I choose the same option if the person were from a different group?”
       - If risk exists, choose a more evidence-based or reversible option.
    6. **Reversibility check (MUST):** Prefer reversible actions under uncertainty; reserve irreversible actions for high confidence or urgent safety needs.
    7. **Verification check (IF feasible):** Verify one key fact that would change the decision (time, amount, policy, symptom severity, intent).
    8. **Choose one next action:** State it as a commitment: “I will do X by Y.”
    9. **Set a review trigger:** Define what outcome/time will cause you to re-run OODA (stop/adjust condition).
  - **Outputs (MUST produce at least one):**
    - **Selected next action:** specific, time-bounded, and feasible.
    - **Rationale:** 1–2 sentences linking option to needs/values/constraints.
    - **Risk note + trigger:** one key downside to watch for + when to reassess.
    - **Optional:** a [[HUMANITY:LESSONS]] note for future decisions.
- **Boundaries / Scope**
  - **Includes:** choosing among feasible options; deliberate non-action; defining triggers for revision; selecting reversible steps under uncertainty.
  - **Excludes:** performing the action (belongs to [[HUMANITY:ACT]]); collecting new signals (belongs to [[HUMANITY:OBSERVE]]) unless verification is explicitly part of the chosen next action.
  - **Primary purpose:** convert a working model and constraints into a **clear next step** that minimizes avoidable harm.
- **Constraints**
  - Decision quality degrades under low [[HUMANITY:RESOURCES]] (fatigue, time pressure) and strong [[HUMANITY:TEMPTATIONS]].
  - Decisions that affect people are vulnerable to [[HUMANITY:STEREOTYPES]] and [[HUMANITY:PREJUDICE]] and can result in [[HUMANITY:DISCRIMINATION]] if unchecked.
  - You MUST not “opt out” by indefinite delay; if you cannot decide fully, decide on a safe placeholder action and a time to revisit.
- **Decision Rules (IF/THEN)**
  - **IF** stakes are high (safety, major money, legal risk, relationship rupture), **THEN** slow down: verify, consult a trusted person ([[HUMANITY:INTERDEPENDENCE]]), and prefer reversible steps.
  - **IF** you feel angry, ashamed, panicked, intoxicated, or exhausted, **THEN** delay irreversible decisions and choose a stabilizing action (pause, sleep, step away, draft-not-send).
  - **IF** you have fewer than two viable options, **THEN** generate at least one more option (including “clarify/ask/check”) before committing.
  - **IF** you cannot verify a key fact, **THEN** label uncertainty and choose a conservative or reversible action.
  - **IF** you notice stereotype-based reasoning, **THEN** stop and rebuild the decision from direct evidence and role-relevant criteria.
  - **IF** delay is itself harmful, **THEN** choose the smallest protective action now and schedule the next review.
- **Ontological Relationships**
  - **Includes/Excludes**
    - **Includes:** option generation, tradeoff selection, commitment to a next step, trigger definition.
    - **Excludes:** action execution ([[HUMANITY:ACT]]); raw sensing ([[HUMANITY:OBSERVE]]).
  - **Related to:** [[HUMANITY:ORIENT]] (provides the working model), [[HUMANITY:ACT]] (executes the decision), [[HUMANITY:VALUES]] (tradeoff policy), [[HUMANITY:PRUDENCE]] (consequence-awareness), [[HUMANITY:THINKING]] (evidence/bias control).
  - **Requires / Required by**
    - **Requires:** a working model with uncertainties from [[HUMANITY:ORIENT]]; minimal [[HUMANITY:RESOURCES]] to compare options.
    - **Required by:** [[HUMANITY:ACT]] (needs a selected action to execute).
  - **Affects / Affected by**
    - **Affects:** outcomes of [[HUMANITY:ACTIVITIES]]; likelihood of satisfying [[HUMANITY:NEEDS]]; risk of [[HUMANITY:CONSEQUENCES_UNMET_NEEDS]].
    - **Affected by:** [[HUMANITY:MOTIVATORS]], [[HUMANITY:TEMPTATIONS]], resource depletion, social pressure, and time constraints.
  - **Vulnerable to / Creates Vulnerabilities for**
    - **Vulnerable to:** impulsivity, paralysis, overconfidence, motivated reasoning, [[HUMANITY:STEREOTYPES]], [[HUMANITY:PREJUDICE]].
    - **Creates vulnerabilities for:** harm from poorly chosen irreversible actions; unfair outcomes and potential [[HUMANITY:DISCRIMINATION]] if bias checks are skipped.
  - **Reduces Risks for / Risks Reduced by**
    - **Reduces risks for:** avoidable harm by forcing explicit tradeoffs, reversibility, and reassessment triggers.
    - **Risks reduced by:** [[HUMANITY:PRUDENCE]] (slowing high stakes), [[HUMANITY:INTERDEPENDENCE]] (second perspective), verification, and regulation pauses.
- Examples of [[HUMANITY:FALLIBILITY]]
  - **Impulsive “hot” decisions:** You decide while angry/tired (send the harsh text, quit on the spot) and regret it later.
  - **Decision paralysis:** Too many tradeoffs leads to “I’ll deal with it later,” which becomes a harmful non-decision.
  - **Temptation-driven choice:** You choose immediate relief (overspending, doomscrolling, lashing out) over long-term stability.
  - **Narrow perspective under low regulation:** Low [[HUMANITY:TEMPERANCE]] reduces [[HUMANITY:PERSPECTIVE]] and impairs [[HUMANITY:THINKING]].
  - **Overconfidence:** You decide from a thin sample and skip verification, creating preventable errors.
- Examples of Using [[HUMANITY:VALUES]]
  - **[[HUMANITY:PRUDENCE]]:** You slow down high-stakes decisions and consider consequences, risks, and ethical implications before committing.
  - **[[HUMANITY:THINKING]]:** You examine evidence, look for bias/manipulation, and consider multiple perspectives before deciding.
  - **[[HUMANITY:HUMILITY]] + [[HUMANITY:INTEGRITY]]:** You keep commitments small enough to keep and repair quickly when you miss.
  - **[[HUMANITY:INTERDEPENDENCE]]:** You use a trusted person as a second perspective to spot blind spots and support follow-through.
  - **[[HUMANITY:WISDOM]]:** You capture outcomes as [[HUMANITY:LESSONS]] (a rule or checklist) to improve future decisions.


##### Act

ID: HUMANITY.ELEMENTS.OODA.ACT
TAGS: [[HUMANITY:ACT]] [[ACT]]

**Act** is the repeating step where you **execute the selected decision** in the real world (behavior and communication), using [[HUMANITY:RESOURCES]] to perform [[HUMANITY:ACTIVITIES]]. Act includes **follow-through**, **monitoring immediate results**, and **making small adjustments** to stay aligned with [[HUMANITY:NEEDS]] and [[HUMANITY:VALUES]]. Act also produces feedback that supports [[HUMANITY:LESSONS]] and improves future [[HUMANITY:ORIENT]] and performance.
- **Examples**
  - **Paying bills / managing finances:** You log in, pay the bill, set reminders/autopay, and confirm it posted (an [[HUMANITY:IADL]]).
  - **Health follow-through:** You fill the prescription, take meds as directed, hydrate/eat, and contact the clinic if symptoms worsen.
  - **Work execution:** You send the email, complete the task, double-check it, and communicate status to others.
  - **Parenting/caregiving:** You set the boundary, enforce it consistently, and repair if you overreact.
  - **Safety action:** You put on the seatbelt, slow down, pull over, or leave an unsafe situation despite inconvenience.
- **Procedure**
  - **Inputs (MUST define or approximate):**
    - **Selected action:** the committed next step from [[HUMANITY:DECIDE]] (who/what/when).
    - **Resources available:** time, energy, attention, tools, money, access, support ([[HUMANITY:RESOURCES]]; [[HUMANITY:CAPABILITIES]]).
    - **Success criteria:** what “done” looks like; minimum acceptable outcome.
    - **Risk controls:** safety constraints; boundaries; escalation thresholds.
    - **Follow-through supports:** reminders, checklists, accountability, environment setup (friction up/down).
  - **Actions (DO in order):**
    1. **Start the action:** take the first physical or communicative step within 60 seconds when feasible.
    2. **Make it concrete:** specify next sub-step (one small unit of work) and begin.
    3. **Use supports (SHOULD):** apply reminders, checklists, templates, timers, or “default-to-safe” settings.
    4. **Monitor results (MUST):** observe immediate outcomes and side effects (errors, resistance, new info).
    5. **Adjust (SHOULD):** if results diverge from expectation, make a small correction or pause and re-run [[HUMANITY:OODA]].
    6. **Close the loop (MUST):**
       - confirm completion (receipt, confirmation number, sent message, scheduled appointment),
       - record the next follow-up step if any.
    7. **Capture learning (MAY):** write one [[HUMANITY:LESSONS]] item to improve future execution.
  - **Outputs (MUST produce at least one):**
    - **Executed behavior/communication:** the action is performed or a deliberate safe non-action is executed (pause/exit/clarify).
    - **Completion evidence:** confirmation, record, or observable state change.
    - **Outcome observation:** what happened immediately after acting (for next [[HUMANITY:OBSERVE]]).
    - **Optional:** [[HUMANITY:LESSONS]] note (rule/checklist/reminder update).
- **Boundaries / Scope**
  - **Includes:** execution, follow-through, coordination with others, tracking completion, immediate adjustments, and documenting outcomes.
  - **Excludes:** selecting among options (belongs to [[HUMANITY:DECIDE]]); interpreting meaning (belongs primarily to [[HUMANITY:ORIENT]]).
  - **Primary purpose:** convert a decision into real-world change and generate feedback for the next loop.
- **Constraints**
  - Act depends on available and sometimes irreplaceable [[HUMANITY:RESOURCES]] (time, energy, tools, money, autonomy, relationships, access).
  - Act is vulnerable to [[HUMANITY:FALLIBILITY]] (forgetting, avoidance, mistakes) and [[HUMANITY:TEMPTATIONS]] (short-term relief choices).
  - Overcommitment reduces execution quality; you MUST size actions to current resources and constraints.
  - Actions in social systems may be blocked or shaped by unfair conditions; outcomes MAY reflect barriers (including potential [[HUMANITY:DISCRIMINATION]]), not only personal effort.
- **Decision Rules (IF/THEN)**
  - **IF** you cannot execute the full action now, **THEN** execute a safe placeholder action (schedule, set reminder, ask for help, exit risk) and set a specific revisit time.
  - **IF** the action is safety-critical, **THEN** prioritize protective steps first (stop, slow, leave, seek help) before optimization.
  - **IF** you notice avoidance/procrastination, **THEN** reduce the action to a 2-minute starter step and begin immediately.
  - **IF** you are emotionally “hot” (anger, panic, shame), **THEN** delay irreversible communication/actions and use regulation before acting.
  - **IF** outcomes diverge from expectation, **THEN** stop escalating and re-run [[HUMANITY:OBSERVE]] → [[HUMANITY:ORIENT]] before continuing.
  - **IF** follow-through repeatedly fails, **THEN** add systems support (checklist, accountability, automation) rather than relying on willpower.
- **Ontological Relationships**
  - **Includes/Excludes**
    - **Includes:** execution, follow-through, communication delivery, adjustment-in-action, completion confirmation.
    - **Excludes:** choosing the action (decision selection) and primary interpretation.
  - **Related to:** [[HUMANITY:DECIDE]] (provides the chosen action), [[HUMANITY:OBSERVE]] (receives outcomes), [[HUMANITY:ACTIVITIES]] (the action content), [[HUMANITY:LEARNING]] (improves future capability), [[HUMANITY:INTEGRITY]] (follow-through and repair).
  - **Requires / Required by**
    - **Requires:** sufficient [[HUMANITY:RESOURCES]] and enabling [[HUMANITY:CAPABILITIES]] (autonomy, tools, access, relationships).
    - **Required by:** the [[HUMANITY:OODA]] to produce real-world effects and feedback.
  - **Affects / Affected by**
    - **Affects:** satisfaction of [[HUMANITY:NEEDS]]; reliability of commitments; downstream trust and coordination.
    - **Affected by:** fatigue, time pressure, environment friction, social constraints, and support availability ([[HUMANITY:RESOURCES]]).
  - **Vulnerable to / Creates Vulnerabilities for**
    - **Vulnerable to:** [[HUMANITY:FALLIBILITY]] (forgetting, errors), [[HUMANITY:TEMPTATIONS]] (avoid discomfort), [[HUMANITY:RESOURCES]] scarcity, and social barriers.
    - **Creates vulnerabilities for:** harm from unregulated “hot” actions; cascading failure if tasks are not closed or confirmed.
  - **Reduces Risks for / Risks Reduced by**
    - **Reduces risks for:** preventable backlog and compounding consequences by closing loops and confirming completion.
    - **Risks reduced by:** [[HUMANITY:INTEGRITY]] (reliability + repair), [[HUMANITY:REGULATION]] (prevent impulsive harm), [[HUMANITY:PERSISTENCE]] (finish hard things), and [[HUMANITY:INTERDEPENDENCE]] (accountability/support).
- Examples of [[HUMANITY:FALLIBILITY]]
  - **Execution failure:** You decide to pay the bill or make the appointment, but procrastinate; costs and stress compound.
  - **Impulsive action under stress:** You snap, road rage, or send harsh words because regulation is depleted.
  - **Overcommitment:** You say yes to too many obligations, underestimate resources, then drop important tasks or neglect needs.
  - **Low follow-through:** You start strong (diet, class, job search) but quit when it gets hard; consistency breaks.
  - **Temptation drift:** You choose short-term relief (doomscrolling, overspending, substances) over long-term stability.
- Examples of Using [[HUMANITY:VALUES]]
  - **[[HUMANITY:INTEGRITY]]:** You keep commitments small enough to keep; when you miss, you acknowledge, repair, and change the system (reminders, automation).
  - **[[HUMANITY:TEMPERANCE]] + [[HUMANITY:REGULATION]]:** You pause before reacting, reduce friction for good actions, add friction for harmful actions, and choose measured responses.
  - **[[HUMANITY:PERSISTENCE]]:** You break tasks into tiny steps, schedule repeats, and treat consistency as success.
  - **[[HUMANITY:INTERDEPENDENCE]]:** You use check-ins/accountability with a trusted person to support follow-through.
  - **[[HUMANITY:WISDOM]]:** You review outcomes and capture one [[HUMANITY:LESSONS]] item (checklist/heuristic) to improve the next Act.