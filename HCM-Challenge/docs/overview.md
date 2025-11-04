# HCM-AAAI26 Workshop Challenge
## 🌐 Challenge Overview
The Gearbox assembly Assistance Challenge evaluates robotic systems in collaborative gearbox assembly within human-centric manufacturing environments. It targets scenarios where robots must work seamlessly with human operators. The challenge focuses on:

• **Prediction and Proactive Assistance**: Anticipating human requirements during assembly. 

• **Instruction Following**: Responding to gesture-based instructions. 

• **Error Detection and Correction**: Detecting errors, correcting them, and continuing the assembly correctly. 

• **Autonomous Continuation**: Autonomously completing assembly with generalized part placement.

Two complementary tracks are designed: **Simulation** and **Onsite Track**. The challenge aligns with HCM-AAAI26 by emphasizing human–robot collaboration, error handling, and proactive assistance in complex manufacturing processes.

---

## 🤺 Competition Tracks

### 🖥️ Simulation Track — Human-in-the-Loop by State Initialization

Robots are evaluated in a simulated gearbox assembly environment where the human role is abstracted as initial conditions. A single Simulation Task is defined, but it may include the following representative scenarios:

•	**Collaborative Assembly from Scratch**: Starting from an empty state, where the robot completes the assembly pipeline as its contribution to a joint workflow.

•	**Resume from Partial State**: The assembly has been partially completed by a “virtual human operator.” The robot must recognize the current state and continue to completion in the correct order.

•	**Error Detection and Recovery**: Errors are injected to mimic human mistakes. The robot must detect, remove incorrect parts, restore the valid state, and continue assembly.

### ⚒️Onsite Track — Human–Robot Collaborative Assistance
Robots collaborate with human operators under clear HRI protocols (e.g., gestures) on standardized physical kits and platforms. A single Onsite Task is defined, which may involve the following representative scenarios:

• **From-Scratch Physical Assembly:** Beginning from an empty state, with the robot responsible for executing the canonical gearbox assembly sequence.

• **Human-Aware Error Intervention:** While observing human assembly, the robot identifies mistakes, flags them in real time, performs safe corrections (remove/replace), and resumes the correct workflow.

• **Continuation and Proactive Assistance:** If the human leaves mid-task, the robot autonomously completes the remaining steps with part-placement generalization. While the human is present, it proactively provides part/tool hand-overs aligned with the current step to reduce idle time and cognitive load.

---

## 📋 Evaluation Metrics
**Metrics applied to both tracks:**

• **Task Success Rate:** Percentage of successful full assemblies within time/step constraints.

• **Assembly Time (Time-to-Completion):** Time required for successful assembly; exceeding timeout counts as failure.

• **Partial Assembly Score:** Number of correctly assembled components in failed trials.

• **Functional Validation Rate:** Ratio of assemblies passing functional tests (gear engagement and rotation).

**For Onsite Track (HRC optional extensions, if desired for awards):**

• **Intervention Latency:** Time from error occurrence to the robot’s alert/correction initiation.

Collectively, these metrics evaluate both the effectiveness (task success and functional correctness) and efficiency (time and partial progress) of robotic assembly strategies.

---

## 📅 Time Schedule
**Cadence:** Preparation → Public Release → Online Competition (Simulation track) → Onsite Finals (Onsite track)

### Phase A · Preparation — Now → early Nov 2025 (e.g., Nov 5)
**Deliverables (Organizers):**

- ARTC / SIMTech: Final task specs, metrics, safety & HRI protocol, real-world (onsite) scene setup, data-collection plan and datasets
- Galaxea: Robotic platform
- IHPC: Simulation assets/dataset with a documented data-collection plan and simulation datasets
- NTU & Stanford: Baselines (code + ckpt); evaluator (Docker/ROS)

**Actions:**

- NTU: Internal dry-run & validation
- NRP: Website & FAQ draft; venue/platform confirmation

**Comms:**

- AAAI: Announcement materials prepared; office hours schedule published

### Phase B · Public Release — Nov 6, 2025 (target)
- **Open:** Team registration; simulation submission portal.
- **Publish:** Website, rules v1.0, dataset, evaluator, baselines; leaderboard policy.
- **Comms:** Kick-off webinar & FAQ v1.0.

### Phase C · Online Competition (Simulation) — Nov 6, 2025 → Jan 10, 2026
- **Submission cadence:** Rolling; leaderboard refresh bi-weekly (Fri 18:00 UTC)
- **Checkpoints:**
  - Rules Freeze: Dec 10, 2025 — thereafter only clarifications.
  - CP-1: Dec 13, 2025 — interim reportable results (auto-archived).
  - CP-2 (final online): Jan 10, 2026 — last leaderboard submission.
- **Required package (Teams):** Docker image + logs; short method card (≤2 pages)
- **Evaluation:** Reproducibility re-runs for top-k; anomaly review
- **Shortlist Notification:** Jan 12, 2026 — finalists invited to onsite

### Phase D · Onsite Finals (Real-World) — Jan 26, 2026
- Check-in, safety briefing, calibration & dry-run slots
- Official trials
- Live demonstrations by top teams; awards & closing remarks

**General Policies:**

- **Submission format:** Docker image + config + README; fixed seeds; max N submissions/week/team (e.g., 3)
- **Revision control:** Evaluator is versioned; teams must declare the version used
- **Safety & ethics:** Onsite follows posted HRI & E-stop policy; violations result in immediate disqualification of the run
- **Comms:** FAQ updated weekly or as needed

---

## 🏁 Workshop Day Competition Schedule

**Two possible schedules are proposed: 2-day format and 1-day format**

### 2-Day format
**Day 1**
- Welcome, Introduction & Rules (~20 min)
- Simulation Track Evaluation Recap — Leaderboard highlights & finalists (~30 min)

**Day 2**
- Platform Setup/Calibration & Safety Briefing (~15 min)
- Real-World Track: Official Trials & Demonstrations (~25 min)
- Evaluation, Results & Closing Remarks (~25 min)

*Indicative total ~1 hour each day*

### 1-Day format
- Welcome, Introduction & Rules (~15 min)
- Safety Briefing (~10 min)
- Simulation Track Evaluation Recap — leaderboard highlights & finalists (~20 min)
- Break / Turnover (~10 min)
- Platform Setup/Calibration (~30 min, simultaneous with blocks above)
- Real-World Track: Official Trials & Demonstrations (~25 min)
- Evaluation, Results & Closing Remarks (~25 min)

*Indicative total ~1.5-2 hours*  
*Notes: Blocks can be merged/trimmed to fit the workshop’s exact slot.*

---

## 🏢 Venue and Equipment
- **Venue Requirements:** Demonstration area (~50m²) with 2–3 workbenches; audience seating with clear visibility

- **Equipment:** Standardized gearbox kits; robotic platforms (to be provided by the organizers, e.g., Galaxea); cameras, projector/display for live visualization

- **Software & Infrastructure:** Standardized deployment (Docker/ROS); high-speed internet access

---

## 📜 Participation and Rules
- **Teams:** 1–5 participants
- **Submission:** Code/models for simulation and real-world execution
- **Fairness:** All teams evaluated under identical conditions with standardized kits to ensure comparability and reproducibility
- **Evaluation:** Based on defined metrics; online track results shown on a public leaderboard and final rankings announced on-site

## 🏅 Award
- 🥇: xxxxxxxxx
- 🥈: xxxxxxxxx
- 🥉: xxxxxxxxx



