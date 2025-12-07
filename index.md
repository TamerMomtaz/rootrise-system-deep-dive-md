# RootRise System Deep Dive
## Understanding the Flow, Capabilities & Narratives

**Prepared for:** Alla Fahmy (CSO) & Tee (PC)  
**Date:** December 7, 2025  
**Purpose:** Internal clarity document for leadership alignment and developer briefing

---

## Part 1: Who Does What? — The Complete Workflow

Let me walk you through the entire journey, from the moment a user arrives to the final deliverable.

### The Cast of Characters

Before the workflow, let's be clear about WHO is involved:

| Actor | Type | Role |
|-------|------|------|
| **The User** | Human | SME owner, investor, government official — whoever initiates |
| **The Platform** | System | RootRise web interface — collects data, displays results |
| **The &Eye** | AI System | Sector detection + lens activation (automated, invisible) |
| **The Pantheon** | AI Agents | 10 specialist analysts working in parallel |
| **The Drucker** | AI Supervisor | Orchestrates agents, resolves conflicts |
| **The Deming** | AI Quality | Validates outputs, triggers escalations |
| **The &I Expert** | Human | RootRise staff or partner who validates high-stakes outputs |
| **The Tufte** | AI Reporter | Generates final documents |

---

### The Workflow: Step by Step

```
┌─────────────────────────────────────────────────────────────────────────────┐
│                        THE ROOTRISE DIAGNOSTIC JOURNEY                       │
└─────────────────────────────────────────────────────────────────────────────┘

PHASE 1: INTAKE (User + Platform)
═══════════════════════════════════════════════════════════════════════════════

Step 1: USER ARRIVES
        ↓
        User visits RootRise platform
        User selects their role: SME | Investor | Government
        ↓
Step 2: USER CONFIGURES
        ↓
        • Selects agents (Core are mandatory, Add-ons are optional)
        • Chooses report format (Executive Summary, Detailed, Presentation)
        • Sets language (English, Arabic, Bilingual)
        • Adjusts technical depth slider (1-5)
        ↓
Step 3: USER COMPLETES QUESTIONNAIRE
        ↓
        • ~50-80 questions across business dimensions
        • Uploads documents (financials, org chart, etc.)
        • ~15-30 minutes of user time
        ↓
        ══════════════════════════════════════════════════════════
        USER'S ACTIVE ROLE ENDS HERE (for now)
        ══════════════════════════════════════════════════════════


PHASE 2: INTELLIGENCE ACTIVATION (Platform + &Eye)
═══════════════════════════════════════════════════════════════════════════════

Step 4: DATA VALIDATION (Gate 1 - Automatic)
        ↓
        System checks:
        • All required fields completed?
        • Document formats valid?
        • Data internally consistent?
        ↓
        IF FAIL → User prompted to fix issues
        IF PASS → Continue
        ↓
Step 5: SECTOR DETECTION (&Eye)
        ↓
        &Eye analyzes questionnaire responses to detect:
        • Primary industry (e.g., "Food Processing")
        • Sub-sector (e.g., "Dairy Manufacturing")
        • Geographic context (e.g., "Egypt, Export-focused")
        ↓
Step 6: LENS ACTIVATION (&Eye)
        ↓
        Based on detection, &Eye loads the appropriate lens:
        • Industry standards (HACCP, ISO 22000, Halal...)
        • Relevant certifications
        • Sector-specific diagnostics
        • Regional regulators
        • Industry benchmarks
        ↓
        This context is INJECTED into every agent's prompt
        ↓
        ══════════════════════════════════════════════════════════
        AGENTS NOW "SEE" THROUGH THE INDUSTRY LENS
        ══════════════════════════════════════════════════════════


PHASE 3: ANALYSIS (The Pantheon)
═══════════════════════════════════════════════════════════════════════════════

Step 7: ORCHESTRATION BEGINS (The Drucker)
        ↓
        The Drucker receives:
        • User's configuration
        • Questionnaire data
        • &Eye's lens context
        • Selected agents list
        ↓
Step 8: PARALLEL AGENT EXECUTION
        ↓
        The Drucker dispatches agents in parallel:
        
        ┌─────────────────────────────────────────────────────────┐
        │  CORE AGENTS (Always Run)                               │
        │  ┌─────────────┐  ┌─────────────┐                      │
        │  │ The Marvin  │  │ The Graham  │                      │
        │  │ Diagnostic  │  │ Finance     │                      │
        │  │ ~45 sec     │  │ ~40 sec     │                      │
        │  └─────────────┘  └─────────────┘                      │
        ├─────────────────────────────────────────────────────────┤
        │  ADD-ON AGENTS (If Selected)                            │
        │  ┌─────────┐ ┌─────────┐ ┌─────────┐ ┌─────────┐       │
        │  │Ricardo  │ │Lovelace │ │Mayo     │ │Ohno     │ ...   │
        │  │Export   │ │Digital  │ │HR       │ │Supply   │       │
        │  │~30 sec  │ │~35 sec  │ │~30 sec  │ │~35 sec  │       │
        │  └─────────┘ └─────────┘ └─────────┘ └─────────┘       │
        └─────────────────────────────────────────────────────────┘
        
        Total time: ~60-90 seconds (parallel, not sequential!)
        ↓
Step 9: AGENT OUTPUTS COLLECTED
        ↓
        Each agent produces:
        • Numerical scores (0-100)
        • Findings (strengths, weaknesses)
        • Recommendations (prioritized)
        • Confidence level (0.0 - 1.0)
        • Evidence citations
        ↓
Step 10: CONFIDENCE CHECK (Gate 2 - Auto + Escalation)
        ↓
        The Drucker reviews confidence levels:
        • All agents > 0.7 confidence? → Continue
        • Any agent < 0.7? → Flag for human review
        ↓
Step 11: CONFLICT RESOLUTION (Gate 3 - Conditional HITL)
        ↓
        The Drucker checks for contradictions:
        • Agent A says "expand capacity" but Agent B says "reduce costs"
        • Agent A says "ready for export" but Agent B says "fix quality first"
        ↓
        IF NO CONFLICTS → Continue
        IF CONFLICTS → The Drucker attempts resolution
                       IF UNRESOLVED → Escalate to human expert


PHASE 4: SYNTHESIS (The Drucker + The Tufte)
═══════════════════════════════════════════════════════════════════════════════

Step 12: NARRATIVE SYNTHESIS (The Drucker)
        ↓
        The Drucker weaves agent outputs into coherent story:
        • Executive summary
        • Overall health score (weighted average)
        • Prioritized action roadmap
        • Cross-cutting insights
        ↓
Step 13: REPORT GENERATION (The Tufte)
        ↓
        The Tufte transforms synthesis into requested format:
        • Executive Summary (2-3 pages)
        • Detailed Report (10-15 pages)
        • Presentation Deck (15-20 slides)
        • Dashboard view
        ↓
        Applies user's preferences:
        • Language
        • Technical depth
        • Visual density
        • Branding


PHASE 5: QUALITY & DELIVERY (The Deming + &I)
═══════════════════════════════════════════════════════════════════════════════

Step 14: QUALITY ASSURANCE (Gate 4 - The Deming)
        ↓
        The Deming validates:
        • Accuracy: Do numbers add up? Sources cited?
        • Consistency: Does narrative match scores?
        • Completeness: All sections filled? No placeholders?
        • Actionability: Are recommendations specific?
        ↓
Step 15: HITL DECISION (Gate 4 - Conditional)
        ↓
        The Deming recommends human review IF:
        • First-time user (no historical data)
        • High-stakes context (donor presentation, investment decision)
        • Unusual patterns detected
        • Low confidence in any section
        • User explicitly requested human review
        ↓
        IF HITL TRIGGERED:
        ┌─────────────────────────────────────────────────────────┐
        │  HUMAN EXPERT REVIEW (&I)                               │
        │                                                         │
        │  Expert receives:                                       │
        │  • Draft report                                         │
        │  • Confidence flags                                     │
        │  • Conflict notes                                       │
        │  • Original questionnaire data                          │
        │                                                         │
        │  Expert actions:                                        │
        │  • Validate findings                                    │
        │  • Adjust recommendations                               │
        │  • Add expert commentary                                │
        │  • Approve for release                                  │
        │                                                         │
        │  Time: 1-4 hours depending on complexity                │
        └─────────────────────────────────────────────────────────┘
        ↓
Step 16: DELIVERY
        ↓
        User receives:
        • Downloadable report (PDF/DOCX/PPTX)
        • Interactive dashboard access
        • Email notification
        ↓
        ══════════════════════════════════════════════════════════
        USER CAN NOW VIEW, SHARE, AND ACT ON INSIGHTS
        ══════════════════════════════════════════════════════════


PHASE 6: FOLLOW-UP (Optional)
═══════════════════════════════════════════════════════════════════════════════

Step 17: USER FEEDBACK
        ↓
        • User rates report quality
        • User indicates actions taken
        • Platform learns and improves
        ↓
Step 18: PROGRESS TRACKING (Future)
        ↓
        • User returns for follow-up diagnostic
        • System compares to baseline
        • Shows improvement trajectory
```

---

## Part 2: Hidden Capabilities You Might Be Missing

Here's what's actually happening under the hood that creates massive value:

### Capability 1: Parallel Processing = Speed
**What it is:** All agents run simultaneously, not one after another.
**Why it matters:** 10 agents × 30 seconds each = 5 minutes sequential. But parallel = ~90 seconds total.
**Value proposition:** "What used to take consultants 6 months, we do in 2 minutes."

### Capability 2: Sector Lenses = Instant Expertise
**What it is:** The &Eye automatically detects industry and loads specialized knowledge.
**Why it matters:** The system doesn't need to be told "I'm a food company" - it figures it out and immediately knows about HACCP, cold chain, traceability, etc.
**Value proposition:** "Our AI understands YOUR industry's specific requirements, regulations, and benchmarks - automatically."

### Capability 3: Knowledge Injection = Contextual Intelligence
**What it is:** Lens knowledge is injected INTO agent prompts, not just referenced.
**Why it matters:** Every agent "thinks" with industry context. The Finance Agent analyzing a pharma company knows about GMP compliance costs. The HR Agent analyzing a textile company knows about labor compliance requirements.
**Value proposition:** "Every recommendation is tailored to your industry reality, not generic advice."

### Capability 4: Confidence Scoring = Honest AI
**What it is:** Every agent outputs a confidence score (0.0-1.0) for its findings.
**Why it matters:** The system knows when it's uncertain and escalates to humans.
**Value proposition:** "We tell you when we're sure and when you need an expert eye."

### Capability 5: Conflict Detection = Holistic Thinking
**What it is:** The Drucker actively looks for contradictions between agents.
**Why it matters:** Real businesses have trade-offs. Expanding requires capital but you're cash-constrained. The system surfaces these tensions rather than hiding them.
**Value proposition:** "We don't give you a wish list - we give you strategic trade-offs."

### Capability 6: Human-in-the-Loop = Trust Layer
**What it is:** Critical decisions route to human experts for validation.
**Why it matters:** AI can be wrong. For high-stakes decisions (investment, donor reports), human experts review.
**Value proposition:** "AI speed with human judgment. The best of both worlds."

### Capability 7: Benchmarking = Competitive Intelligence
**What it is:** Every metric is compared against industry/regional benchmarks.
**Why it matters:** "Your gross margin is 23%" means nothing. "Your gross margin is 23% vs. industry average of 31%" is actionable.
**Value proposition:** "Know exactly where you stand against your competition."

### Capability 8: Multi-Format Output = Flexibility
**What it is:** Same analysis, different formats for different audiences.
**Why it matters:** SME owner wants executive summary. Investor wants detailed financials. Board wants presentation.
**Value proposition:** "One diagnostic, multiple outputs tailored to each stakeholder."

### Capability 9: Bilingual = MENA-Ready
**What it is:** Full Arabic support, including RTL layouts.
**Why it matters:** Many SME owners prefer Arabic. Government reports often require Arabic.
**Value proposition:** "Truly local platform for the MENA region."

### Capability 10: Extensibility = Future-Proof
**What it is:** New agents, new lenses, new knowledge packs can be added without rebuilding.
**Why it matters:** UNIDO wants a food systems lens? We add it. New export market opens? We add the regulatory knowledge.
**Value proposition:** "A platform that grows with you and the ecosystem."

---

## Part 3: Different Narratives for Different Users

### 🏭 Narrative for SMEs

**Their mindset:** "I'm busy. Consultants are expensive. I don't trust AI. Will this actually help?"

**The story to tell:**

> "You've built something real. Now you need to know: Where are the gaps? What should you fix first? Are you ready for funding?
>
> RootRise gives you a complete health check of your business in 30 minutes. Not generic advice - insights specific to YOUR industry, YOUR region, YOUR situation.
>
> Answer our questions. Upload your documents. In 2 minutes, you'll have:
> - A clear picture of your strengths and weaknesses
> - Specific actions prioritized by impact
> - Benchmarks showing where you stand vs. competitors
> - A roadmap to become investor-ready
>
> No consultants. No waiting. No guessing."

**Key features to emphasize:**
- Speed (30 min input → 2 min output)
- Industry-specific (not generic)
- Actionable roadmap (not just scores)
- Affordable (vs. $50K consulting engagement)

---

### 💰 Narrative for Funders/Investors

**Their mindset:** "Deal flow is huge. Due diligence is expensive. I miss good deals. I fund bad ones."

**The story to tell:**

> "You see hundreds of SMEs. You can only fund dozens. How do you find the diamonds in the rough?
>
> RootRise pre-screens your deal flow with institutional-grade diagnostics. Every SME that comes to you arrives with:
> - Financial health score (not just their pitch deck)
> - Operational maturity assessment
> - Growth readiness indicators
> - Risk flags highlighted
> - Investment thesis draft
>
> Cut your due diligence time by 85%. Focus your team on deals worth pursuing."

**Key features to emphasize:**
- Deal screening at scale
- Standardized comparison across portfolio
- Risk identification
- Due diligence acceleration
- Portfolio health monitoring

---

### 🌍 Narrative for Donors/Development Organizations

**Their mindset:** "We need impact at scale. We need to report to stakeholders. We need sustainability."

**The story to tell:**

> "You're funding SME development programs. But how do you know they're working?
>
> RootRise gives you a before-and-after diagnostic for every SME in your program. Track real impact:
> - Baseline assessments at program entry
> - Progress tracking throughout
> - Exit assessments showing improvement
> - Aggregated impact metrics (jobs created, exports enabled, certifications achieved)
>
> Report to your board with confidence. Show exactly how your funding translates to economic transformation."

**Key features to emphasize:**
- Impact measurement
- Aggregated analytics
- SDG alignment
- Program evaluation
- Reporting dashboards

---

### 🏛️ Narrative for Governments

**Their mindset:** "We need to support SMEs at national scale. We need policy insights. We need job creation."

**The story to tell:**

> "Your economy runs on SMEs. But do you really know their health?
>
> RootRise gives you X-ray vision into your SME sector:
> - Sector-by-sector health mapping
> - Regional economic indicators
> - Export readiness across industries
> - Skills gap analysis at national scale
> - Policy impact modeling
>
> Make data-driven decisions. Target interventions where they matter most. Track job creation and GDP contribution in real-time."

**Key features to emphasize:**
- National-scale analytics
- Sector health dashboards
- Policy planning tools
- Job creation tracking
- Export readiness mapping

---

### 🤝 Narrative for Partners (UNIDO, Accelerators, Banks)

**Their mindset:** "We have SME clients. We need to serve them better. We want efficiency."

**The story to tell:**

> "You work with SMEs every day. You know they need diagnostics. But building this yourself would take years and millions.
>
> Partner with RootRise:
> - White-label the platform with your branding
> - Add your sector-specific knowledge packs
> - Integrate with your existing systems
> - Serve your clients with world-class diagnostics
>
> We bring the AI infrastructure. You bring the relationships and expertise. Together, we transform SME development."

**Key features to emphasize:**
- White-labeling
- API integration
- Knowledge pack co-creation
- Revenue sharing models
- Training and support

---

## Part 4: Technical Brief for Developers

### System Architecture Overview

```
┌─────────────────────────────────────────────────────────────────────────────┐
│                           ROOTRISE SYSTEM ARCHITECTURE                       │
└─────────────────────────────────────────────────────────────────────────────┘

┌─────────────┐     ┌─────────────────────────────────────────────────────────┐
│   CLIENT    │     │                    BACKEND SERVICES                      │
│   LAYER     │     │                                                         │
│             │     │  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐     │
│  ┌───────┐  │     │  │   API       │  │   Auth      │  │   File      │     │
│  │Web App│  │◄───►│  │   Gateway   │  │   Service   │  │   Storage   │     │
│  └───────┘  │     │  └─────────────┘  └─────────────┘  └─────────────┘     │
│             │     │         │                                               │
│  ┌───────┐  │     │         ▼                                               │
│  │Mobile │  │     │  ┌─────────────────────────────────────────────────┐   │
│  │ App   │  │     │  │            ORCHESTRATION LAYER                   │   │
│  └───────┘  │     │  │                                                  │   │
│             │     │  │  ┌─────────────────────────────────────────────┐ │   │
└─────────────┘     │  │  │  LangGraph Workflow Engine                  │ │   │
                    │  │  │                                             │ │   │
                    │  │  │  ┌─────────┐    ┌──────────────────────┐   │ │   │
                    │  │  │  │ &Eye    │───►│ Sector Detection     │   │ │   │
                    │  │  │  │ System  │    │ Lens Activation      │   │ │   │
                    │  │  │  └─────────┘    └──────────────────────┘   │ │   │
                    │  │  │       │                                     │ │   │
                    │  │  │       ▼                                     │ │   │
                    │  │  │  ┌─────────────────────────────────────┐   │ │   │
                    │  │  │  │         THE PANTHEON                │   │ │   │
                    │  │  │  │  ┌─────────┐ ┌─────────┐ ┌────────┐ │   │ │   │
                    │  │  │  │  │ Drucker │ │ Marvin  │ │ Graham │ │   │ │   │
                    │  │  │  │  │ (Super) │ │ (Diag)  │ │ (Fin)  │ │   │ │   │
                    │  │  │  │  └─────────┘ └─────────┘ └────────┘ │   │ │   │
                    │  │  │  │  ┌────────┐ ┌────────┐ ┌──────────┐ │   │ │   │
                    │  │  │  │  │Ricardo │ │Lovelace│ │  Mayo    │ │   │ │   │
                    │  │  │  │  └────────┘ └────────┘ └──────────┘ │   │ │   │
                    │  │  │  │  ┌────────┐ ┌────────┐ ┌──────────┐ │   │ │   │
                    │  │  │  │  │ Ohno   │ │ Porter │ │  Tufte   │ │   │ │   │
                    │  │  │  │  └────────┘ └────────┘ └──────────┘ │   │ │   │
                    │  │  │  │  ┌────────┐                         │   │ │   │
                    │  │  │  │  │ Deming │                         │   │ │   │
                    │  │  │  │  └────────┘                         │   │ │   │
                    │  │  │  └─────────────────────────────────────┘   │ │   │
                    │  │  └─────────────────────────────────────────────┘ │   │
                    │  └─────────────────────────────────────────────────┘   │
                    │         │                                               │
                    │         ▼                                               │
                    │  ┌─────────────────────────────────────────────────┐   │
                    │  │              DATA LAYER                          │   │
                    │  │                                                  │   │
                    │  │  ┌─────────────┐  ┌─────────────┐               │   │
                    │  │  │  PostgreSQL │  │   Vector    │               │   │
                    │  │  │  (Frappe)   │  │   Store     │               │   │
                    │  │  │             │  │  (Pinecone/ │               │   │
                    │  │  │  - Users    │  │   Qdrant)   │               │   │
                    │  │  │  - SMEs     │  │             │               │   │
                    │  │  │  - Reports  │  │  - Lenses   │               │   │
                    │  │  │  - History  │  │  - KnowPacks│               │   │
                    │  │  └─────────────┘  └─────────────┘               │   │
                    │  └─────────────────────────────────────────────────┘   │
                    └─────────────────────────────────────────────────────────┘

                    ┌─────────────────────────────────────────────────────────┐
                    │                    EXTERNAL SERVICES                     │
                    │                                                         │
                    │  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐     │
                    │  │   LLM API   │  │  Document   │  │   Email     │     │
                    │  │  (Claude/   │  │  Processing │  │   Service   │     │
                    │  │   GPT-4)    │  │  (PDF/DOCX) │  │             │     │
                    │  └─────────────┘  └─────────────┘  └─────────────┘     │
                    └─────────────────────────────────────────────────────────┘
```

### Key Technical Components

#### 1. Orchestration Engine (LangGraph)

```python
# Simplified workflow definition
from langgraph.graph import StateGraph

workflow = StateGraph(DiagnosticState)

# Add nodes
workflow.add_node("intake", intake_node)
workflow.add_node("sector_detection", eye_detect_sector)
workflow.add_node("lens_activation", eye_load_lens)
workflow.add_node("agent_dispatch", drucker_dispatch)
workflow.add_node("parallel_analysis", run_agents_parallel)
workflow.add_node("synthesis", drucker_synthesize)
workflow.add_node("quality_check", deming_validate)
workflow.add_node("report_generation", tufte_generate)
workflow.add_node("hitl_review", human_review)  # Conditional
workflow.add_node("delivery", deliver_report)

# Add edges with conditions
workflow.add_edge("intake", "sector_detection")
workflow.add_edge("sector_detection", "lens_activation")
workflow.add_edge("lens_activation", "agent_dispatch")
workflow.add_edge("agent_dispatch", "parallel_analysis")
workflow.add_edge("parallel_analysis", "synthesis")
workflow.add_edge("synthesis", "quality_check")
workflow.add_conditional_edges(
    "quality_check",
    should_route_to_human,
    {
        "human": "hitl_review",
        "auto": "report_generation"
    }
)
workflow.add_edge("hitl_review", "report_generation")
workflow.add_edge("report_generation", "delivery")
```

#### 2. Agent Definition Pattern

```python
class BaseAgent:
    """Base class for all Pantheon agents"""
    
    def __init__(self, name: str, lens_context: dict = None):
        self.name = name
        self.lens_context = lens_context
        
    def build_prompt(self, sme_data: dict) -> str:
        """Build prompt with lens context injection"""
        base_prompt = self.get_base_prompt()
        
        if self.lens_context:
            base_prompt += f"\n\n## INDUSTRY CONTEXT\n{self.lens_context}"
            
        base_prompt += f"\n\n## SME DATA\n{json.dumps(sme_data)}"
        
        return base_prompt
    
    async def analyze(self, sme_data: dict) -> AgentOutput:
        """Run analysis and return structured output"""
        prompt = self.build_prompt(sme_data)
        response = await llm.complete(prompt)
        
        return AgentOutput(
            agent_name=self.name,
            score=response.score,
            confidence=response.confidence,
            findings=response.findings,
            recommendations=response.recommendations,
            evidence=response.evidence
        )
```

#### 3. &Eye Lens System

```python
class EyeSystem:
    """Sector detection and lens management"""
    
    def __init__(self, vector_store):
        self.vector_store = vector_store
        self.lens_cache = {}
        
    async def detect_sector(self, questionnaire: dict) -> SectorDetection:
        """Analyze questionnaire to determine sector"""
        # Extract key indicators
        indicators = extract_sector_indicators(questionnaire)
        
        # Query vector store for closest sector match
        matches = await self.vector_store.similarity_search(
            query=indicators,
            collection="sectors",
            top_k=3
        )
        
        return SectorDetection(
            primary_sector=matches[0].sector,
            confidence=matches[0].score,
            sub_sector=matches[1].sector if len(matches) > 1 else None
        )
    
    async def load_lens(self, sector: str) -> LensContext:
        """Load sector-specific knowledge"""
        if sector in self.lens_cache:
            return self.lens_cache[sector]
            
        lens = await self.vector_store.get(
            collection="lenses",
            id=sector
        )
        
        self.lens_cache[sector] = lens
        return lens
```

#### 4. Validation Gates

```python
class ValidationGate:
    """Base class for validation gates"""
    
    @abstractmethod
    async def validate(self, data: dict) -> ValidationResult:
        pass

class Gate1_DataValidation(ValidationGate):
    """Automatic data completeness check"""
    
    async def validate(self, questionnaire: dict) -> ValidationResult:
        required_fields = get_required_fields()
        missing = [f for f in required_fields if f not in questionnaire]
        
        return ValidationResult(
            passed=len(missing) == 0,
            gate="data_validation",
            issues=missing,
            requires_human=False
        )

class Gate2_ConfidenceCheck(ValidationGate):
    """Check agent confidence levels"""
    
    async def validate(self, agent_outputs: List[AgentOutput]) -> ValidationResult:
        low_confidence = [
            a for a in agent_outputs 
            if a.confidence < 0.7
        ]
        
        return ValidationResult(
            passed=len(low_confidence) == 0,
            gate="confidence_check",
            issues=[a.agent_name for a in low_confidence],
            requires_human=len(low_confidence) > 0
        )

class Gate3_ConflictResolution(ValidationGate):
    """Detect contradictions between agents"""
    
    async def validate(self, agent_outputs: List[AgentOutput]) -> ValidationResult:
        conflicts = detect_conflicts(agent_outputs)
        
        if conflicts:
            resolved = await self.attempt_resolution(conflicts)
            unresolved = [c for c in conflicts if not c.resolved]
            
            return ValidationResult(
                passed=len(unresolved) == 0,
                gate="conflict_resolution",
                issues=unresolved,
                requires_human=len(unresolved) > 0
            )
        
        return ValidationResult(passed=True, gate="conflict_resolution")

class Gate4_QualityAssurance(ValidationGate):
    """Final quality check by The Deming"""
    
    async def validate(self, report: Report, context: dict) -> ValidationResult:
        checks = await self.run_quality_checks(report)
        
        # Determine if human review needed
        requires_human = (
            context.get("first_time_user", False) or
            context.get("high_stakes", False) or
            context.get("user_requested_review", False) or
            not all(c.passed for c in checks)
        )
        
        return ValidationResult(
            passed=all(c.passed for c in checks),
            gate="quality_assurance",
            issues=[c for c in checks if not c.passed],
            requires_human=requires_human
        )
```

### Data Models

```python
# Core data structures

@dataclass
class SMEProfile:
    id: str
    name: str
    sector: str
    sub_sector: str
    country: str
    employee_count: int
    annual_revenue: float
    years_in_operation: int
    questionnaire_responses: dict
    documents: List[Document]
    created_at: datetime
    
@dataclass
class AgentOutput:
    agent_name: str
    score: float  # 0-100
    confidence: float  # 0.0-1.0
    findings: List[Finding]
    recommendations: List[Recommendation]
    evidence: List[Evidence]
    execution_time_ms: int
    
@dataclass
class DiagnosticReport:
    id: str
    sme_id: str
    overall_score: float
    agent_outputs: List[AgentOutput]
    synthesis: Synthesis
    roadmap: ActionRoadmap
    format: ReportFormat
    language: str
    created_at: datetime
    reviewed_by: Optional[str]  # Human reviewer ID
    
@dataclass
class LensContext:
    sector: str
    standards: List[str]
    certifications: List[str]
    diagnostics: List[str]
    regulators: List[str]
    benchmarks: Dict[str, float]
    regulatory_context: str
```

### API Endpoints

```yaml
# Core API endpoints

POST /api/v1/diagnostic/start
  # Start new diagnostic session
  Request: { sme_profile, selected_agents, preferences }
  Response: { session_id, status }

POST /api/v1/diagnostic/{session_id}/questionnaire
  # Submit questionnaire responses
  Request: { responses, documents }
  Response: { validation_result, next_step }

GET /api/v1/diagnostic/{session_id}/status
  # Check diagnostic progress
  Response: { status, progress_pct, current_step, eta_seconds }

GET /api/v1/diagnostic/{session_id}/report
  # Retrieve completed report
  Response: { report, format, download_url }

POST /api/v1/diagnostic/{session_id}/feedback
  # Submit user feedback
  Request: { rating, comments, actions_taken }
  Response: { success }

# Admin endpoints
GET /api/v1/admin/queue
  # View HITL review queue
  Response: { pending_reviews[] }

POST /api/v1/admin/review/{session_id}
  # Submit human review
  Request: { approved, modifications, expert_notes }
  Response: { success, report_updated }
```

### Integration Points

| System | Integration Type | Purpose |
|--------|------------------|---------|
| Frappe/ERPNext | REST API | User management, SME data storage |
| LLM Provider | API | Agent inference (Claude/GPT-4) |
| Vector Store | SDK | Lens storage, similarity search |
| Document Processor | Library | PDF/DOCX parsing, generation |
| Email Service | API | Notifications, report delivery |
| Analytics | Events | Usage tracking, performance monitoring |

---

## Part 5: Discussion Questions for Alla & Tee

Now that you have the full picture, here are questions to align on:

### Strategic Questions
1. **Which user segment do we prioritize first?** SMEs are volume, but investors/donors might be better early adopters (they have budget and need).

2. **How do we price this?** Per diagnostic? Subscription? Enterprise licensing?

3. **What's our HITL capacity?** If we trigger human review for first-time users, how many reviews can we handle per day?

4. **What's our accuracy target?** How do we measure if the diagnostic is "right"? User satisfaction? Expert validation? Follow-up outcomes?

### Product Questions
1. **Minimum viable diagnostic:** Which agents are truly CORE? Can we launch with just Marvin + Graham?

2. **Onboarding flow:** 50-80 questions is a lot. Can we do progressive disclosure? Start with 20, ask for more based on initial answers?

3. **Real-time vs. batch:** Do users need results in 2 minutes, or is next-day acceptable for higher quality?

### Technical Questions
1. **LLM selection:** Claude vs. GPT-4 vs. open-source? Cost vs. quality trade-offs.

2. **Vector store:** Pinecone (managed) vs. Qdrant (self-hosted)? 

3. **Infrastructure:** Where do we host? AWS? GCP? Regional compliance considerations for MENA data.

---

## Summary

This document covers:

✅ **Complete workflow** — Every step from user arrival to report delivery  
✅ **10 hidden capabilities** — Value you might not realize you have  
✅ **5 stakeholder narratives** — How to talk to each audience  
✅ **Technical architecture** — What developers need to build  
✅ **Discussion questions** — Decisions you need to make together  

The next step is to review this together, align on the strategic questions, and then brief the development team.

---

*Document prepared by Claude for RootRise leadership alignment.*
