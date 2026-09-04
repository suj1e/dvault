# Elio Product Specification V1

> **Document Status**: Draft  
> **Last Updated**: 2025-01  
> **Version**: 1.0.0  

---

## Table of Contents

1. [Product Vision](#1-product-vision)
2. [Core Learning Loop](#2-core-learning-loop)
3. [V1 User Journey](#3-v1-user-journey)
4. [Learning Architecture](#4-learning-architecture)
5. [Lesson Design](#5-lesson-design)
6. [AI Responsibilities](#6-ai-responsibilities)
7. [Progress & Mastery](#7-progress--mastery)
8. [V1 Scope](#8-v1-scope)
9. [V1 Closed Loop Definition](#9-v1-closed-loop-definition)
10. [Acceptance Criteria](#10-acceptance-criteria)

---

## 1. Product Vision

### 1.1 What Elio Is

Elio is an **AI-driven language learning product** that helps users systematically master a new language through a structured, progressive, and sustainable learning path.

Elio is not a chat companion, not a simple vocabulary drill app, and not a content consumption platform. It is a **complete learning system** that guides users from assessment to mastery through evidence-based pedagogy.

### 1.2 What Elio Is Not

- **Not a chatbot**: AI conversation is a practice tool, not the product's core.
- **Not a flashcard app**: SRS is one component of a larger system.
- **Not a content platform**: Content serves learning objectives, not the other way around.
- **Not a game**: No points, badges, or leaderboards. Progress is measured by mastery, not engagement metrics.
- **Not a social network**: No community features in V1.

### 1.3 Core Users

| User Type | Description | Primary Need |
|-----------|-------------|--------------|
| **Starter** | Beginner language learners | Structured path from zero |
| **Resumer** | Learners with prior experience | Accurate placement and gap filling |
| **Professional** | Career-driven learners | Targeted, efficient learning |
| **Self-directed** | Motivated independent learners | Clear roadmap and feedback |

### 1.4 Core Value Proposition

> **Help users choose a language, and through a systematic, progressive, and sustainable learning path, truly master it.**

Traditional language apps fail because they:
- Offer disconnected exercises without a coherent learning arc
- Treat all learners the same regardless of background
- Measure engagement (streaks, XP) instead of actual proficiency
- Lack structured curriculum — content is random, not progressive

Elio succeeds by providing:
- A **structured curriculum** that builds knowledge progressively
- **Personalized learning paths** based on assessment and mastery
- **AI-powered practice** that simulates real language use
- **Evidence-based progress tracking** that shows actual proficiency growth

### 1.5 V1 Product Hypotheses to Validate

| Hypothesis | How to Validate |
|------------|-----------------|
| Users will engage with a structured learning path over random exercises | Completion rates of structured lessons vs. standalone exercises |
| AI-generated practice is more effective than fixed exercises | Learning velocity and retention rates |
| Users trust AI feedback enough to act on it | Correction application rate |
| Mastery-based progression feels more motivating than gamification | User retention and lesson progression speed |
| A complete learning loop (learn → practice → apply → review) creates measurable improvement | Pre/post assessment score changes |

---

## 2. Core Learning Loop

Elio's learning loop is the heart of the product. Every feature serves this loop.

```text
Assess → Plan → Learn → Practice → Apply → Feedback → Review → Master → Progress
```

### 2.1 Assess

**Purpose**: Understand where the user is and what they need.

**Activities**:
- Placement assessment (if returning user)
- Goal setting (why are you learning this language?)
- Current level estimation
- Learning style and time availability

**Output**: User profile with level, goals, and initial learning parameters.

### 2.2 Plan

**Purpose**: Create a personalized path forward.

**Activities**:
- Generate a Stage-based learning plan
- Sequence Units and Lessons
- Set milestones and checkpoints
- Schedule review sessions

**Output**: A structured learning path with clear milestones.

### 2.3 Learn

**Purpose**: Acquire new knowledge.

**Activities**:
- Present new vocabulary in context
- Introduce grammar concepts with examples
- Explain cultural nuances
- Provide mnemonic aids

**Output**: New knowledge integrated into the user's mental model.

### 2.4 Practice

**Purpose**: Strengthen new knowledge through active use.

**Activities**:
- Vocabulary exercises (SRS, fill-in-blank, matching)
- Grammar drills (sentence construction, correction)
- Listening comprehension
- Reading comprehension

**Output**: Initial evidence of retention and understanding.

### 2.5 Apply

**Purpose**: Use language in realistic contexts.

**Activities**:
- AI conversation practice
- Writing prompts based on lesson content
- Scenario-based role play
- Real-world task simulation

**Output**: Evidence of productive language ability.

### 2.6 Feedback

**Purpose**: Close the gap between current performance and target.

**Activities**:
- Immediate correction of errors
- Explanation of mistakes
- Alternative expressions
- Strengths identification

**Output**: Specific, actionable improvement guidance.

### 2.7 Review

**Purpose**: Combat forgetting and transfer to long-term memory.

**Activities**:
- SRS vocabulary review
- Spaced grammar review
- Mistake re-attempts
- Cumulative review sessions

**Output**: Reinforced knowledge and updated mastery scores.

### 2.8 Master

**Purpose**: Confirm reliable, independent performance.

**Activities**:
- Stage assessment
- Unassisted production
- Error rate threshold validation

**Output**: Mastery badge and progression to next stage.

### 2.9 Progress

**Purpose**: Feed results back into the system.

**Activities**:
- Update mastery scores
- Adjust review schedules
- Recalculate learning path
- Update weak point profile

**Output**: Updated user model and next learning recommendation.

### 2.10 Loop Continuity

The loop is not linear — it feeds back into itself:

```text
Progress
  ↓
Assess (re-evaluate current level)
  ↓
Plan (adjust learning path)
  ↓
[Continue loop]
```

Users continuously cycle through this loop, with each iteration building on previous mastery.

---

## 3. V1 User Journey

### 3.1 Onboarding

**Step 1: Welcome**

User opens Elio for the first time.

- Clean, minimal welcome screen
- Clear value proposition: "Learn a language systematically"
- Single call-to-action: "Get Started"

**Step 2: Language Selection**

User selects target language.

- Supported languages: English, Japanese, French, Spanish, German, Korean
- Visual language cards with cultural imagery
- User can select multiple languages (V1 supports concurrent learning)

**Step 3: Current Level Assessment**

User self-reports current level.

Options: Complete Beginner / Beginner / Intermediate / Advanced

- Brief explanation of what each level means
- No formal test at this stage (V1 uses self-assessment)
- User can change level later

**Step 4: Learning Goal**

User defines learning objective.

Options:
- Daily conversation
- Travel
- Academic study
- Career / Business
- Exam preparation
- General improvement

**Step 5: Time Commitment**

User sets daily study time.

Options: 10 min / 15 min / 30 min / 45 min / 60 min

- Recommendation shown based on goal
- Default: 15 minutes
- User can change anytime

**Step 6: Generated Learning Plan**

System generates initial learning plan.

- Shows first Stage overview
- Estimated time to complete
- Preview of first Lesson
- "Start Learning" button

**Onboarding Complete.** User enters main learning interface.

---

### 3.2 First Learning Session

**Step 1: Home Dashboard**

User sees:
- Current streak: 0
- Today's goal: 15 minutes
- Current Stage: Stage 1 - Foundations
- Current Unit: Unit 1 - Greetings
- Current Lesson: Lesson 1 - Hello
- "Continue" button

**Step 2: Lesson Start**

User taps "Continue" → enters Lesson 1.

Lesson structure (detailed in Section 5):
```
1. Introduction (context)
2. Learn (new concepts)
3. Practice (mechanical exercises)
4. Apply (AI conversation)
5. Feedback (corrections)
6. Review (summary)
```

**Step 3: Lesson Completion**

- Lesson summary screen
- New vocabulary count
- Accuracy percentage
- Time spent
- "Continue to Next Lesson" or "Back to Home"

---

### 3.3 Second Day: Returning User

**Step 1: Home Dashboard**

User opens Elio the next day.

- Streak: 1
- Today's review queue: 15 vocabulary items
- Current progress: Stage 1, 20% complete
- Notification: "Time to review your vocabulary"

**Step 2: Review Session**

User completes SRS review.

- 15 vocabulary items
- ~5 minutes
- Immediate feedback on each
- Review summary at end

**Step 3: New Lesson**

After review, user continues to new Lesson 2.

- Seamless transition from review to new content
- Progress bar shows overall advancement

---

### 3.4 Week 2: Progression

**Step 1: Dashboard**

- Streak: 7
- Stage 1 complete
- Stage Assessment available

**Step 2: Stage Assessment**

System prompts user to take Stage 1 Assessment.

- 20 questions covering Stage 1 content
- Mix of multiple choice, fill-in-blank, and AI conversation
- Timed: 15 minutes

**Step 3: Results**

- Score: 85%
- Weak areas identified: verb conjugation
- Recommendation: "Review Unit 3, then proceed to Stage 2"
- "Proceed to Stage 2" button

**Step 4: Stage 2**

- New vocabulary, grammar, and conversation scenarios
- Builds directly on Stage 1 foundations
- Maintains same lesson structure

---

### 3.5 Month 1: Habit Formation

**User Behavior**:
- Consistent daily usage (15-20 minutes)
- Streak: 25+ days
- Completed: 3 Stages
- Mastered: 200+ vocabulary items
- Weak points: listening comprehension, past tense verbs

**System Adapts**:
- Increases listening exercises
- Adds past tense review sessions
- Adjusts lesson difficulty based on performance

---

### 3.6 Key Transitions

| Transition | Trigger | System Response |
|------------|---------|-----------------|
| First open → Onboarding | App launch (new user) | Welcome flow |
| Onboarding → First Lesson | Completion of setup | Generate learning plan, start Lesson 1 |
| Lesson → Review | Next day, SRS queue due | Prompt review before new content |
| Review → New Lesson | Review completion | Unlock next lesson |
| Unit → Unit | All lessons in unit complete | Unit summary, next unit preview |
| Stage → Stage | All units complete + assessment passed | Stage completion, next stage |
| Lesson → Lesson | Current lesson complete | Next lesson in sequence |

---

## 4. Learning Architecture

### 4.1 Hierarchy

```
Language
  └── Stage (e.g., "Foundations", "Daily Conversation", "Travel")
       └── Unit (e.g., "Greetings", "At the Restaurant", "Directions")
            └── Lesson (e.g., "Hello and Goodbye", "Ordering Food")
                 └── Activity (e.g., "Vocabulary Introduction", "AI Conversation Practice")
```

### 4.2 Stage

**Definition**: A major learning phase with a coherent theme and competency goal.

**Example Stages for English**:
1. Foundations (survival phrases, basic grammar)
2. Daily Life (routines, descriptions)
3. Social Interaction (conversations, opinions)
4. Work & Study (professional contexts)
5. Fluency (complex topics, nuance)

**Responsibility**:
- Defines overall competency goal
- Contains 4-6 Units
- Ends with Stage Assessment
- Prerequisite for next Stage

**Prerequisite**: Completion of previous Stage assessment at passing threshold (80%).

### 4.3 Unit

**Definition**: A thematic cluster of lessons within a Stage.

**Example Units for "Daily Life" Stage**:
- Morning Routines
- Shopping
- Transportation
- Dining

**Responsibility**:
- Groups 3-5 related Lessons
- Thematic coherence
- Progressive difficulty within Unit

**Prerequisite**: Completion of previous Unit.

### 4.4 Lesson

**Definition**: A single, complete learning session (~10-15 minutes).

**Responsibility**:
- Teaches specific, measurable learning objectives
- Follows standard Lesson Design (Section 5)
- Produces learnable artifacts (vocabulary, grammar points, practice records)

**Prerequisite**: Previous Lesson in Unit.

### 4.5 Activity

**Definition**: The smallest unit of learning interaction within a Lesson.

**Types**:
- Vocabulary Introduction
- Grammar Explanation
- Mechanical Practice (fill-in-blank, matching)
- AI Conversation
- Listening Exercise
- Writing Prompt
- Review

**Responsibility**:
- Single focused task
- Clear input/output
- Measurable outcome

---

### 4.6 Key Concepts

#### Prerequisite

**Definition**: What the user must know/complete before starting a learning unit.

**Types**:
- **Structural prerequisite**: Previous Lesson/Unit/Stage completed
- **Competency prerequisite**: Mastery score above threshold (e.g., 70%)
- **Knowledge prerequisite**: Specific vocabulary or grammar points mastered

**Enforcement**: System gates access until prerequisites are met.

---

#### Learning Objective

**Definition**: What the user will be able to do after completing a learning unit.

**Format**: "By the end of this lesson, you will be able to [specific action]."

**Example**: "By the end of this lesson, you will be able to introduce yourself and ask basic questions about daily routines."

**Properties**:
- Specific and measurable
- Aligned with CEFR level
- Testable through assessment

---

#### Mastery

**Definition**: The user's demonstrated proficiency on a specific skill or knowledge item.

**Scale**: 0-100%

**Thresholds**:
- 0-40%: Not Started / Learning
- 40-70%: Practicing
- 70-90%: Applied (can use independently)
- 90-100%: Mastered

**Determined by**:
- Exercise accuracy
- Speed of response
- Error types
- Application in AI conversation
- Assessment performance

---

#### Progression

**Definition**: The user's movement through the learning architecture.

**Rules**:
- Linear within a Stage (lessons must be completed in order)
- Sequential across Stages (must pass assessment to advance)
- Adaptive within a Lesson (practice more if mastery is low)

**User Control**: Users can review previous content anytime but cannot skip ahead without meeting prerequisites.

---

#### Review

**Definition**: Scheduled re-exposure to previously learned material to combat forgetting.

**Types**:
- **Daily Review**: SRS-based vocabulary and grammar review
- **Cumulative Review**: Mixed review across multiple lessons
- **Mistake Review**: Targeted review of errors
- **Pre-Assessment Review**: Before Stage Assessment

**Trigger**: Based on spaced repetition algorithm and error frequency.

---

#### Assessment

**Definition**: Formal evaluation of user competency at Stage boundaries.

**Types**:
- **Stage Assessment**: End-of-stage evaluation
- **Unit Quiz**: Light checkpoint within a Unit
- **Placement Test**: Initial level assessment (future)

**Format**:
- Multiple choice
- Fill-in-blank
- Sentence construction
- AI conversation evaluation

**Passing Threshold**: 80% correct

**Failure Behavior**: Review recommended content, retake assessment. No penalty.

---

## 5. Lesson Design

### 5.1 Standard Lesson Structure

```
┌─────────────────────────────────────────┐
│ 1. Introduction (2 min)                  │
│    - Context and real-world scenario     │
│    - Learning objectives                 │
│    - What you'll be able to do           │
├─────────────────────────────────────────┤
│ 2. Learn (3 min)                         │
│    - New vocabulary in context            │
│    - Grammar explanation                 │
│    - Examples and usage notes            │
├─────────────────────────────────────────┤
│ 3. Practice (3 min)                      │
│    - Mechanical exercises                 │
│    - Fill-in-blank, matching, ordering   │
│    - Immediate feedback                  │
├─────────────────────────────────────────┤
│ 4. Apply (3 min)                         │
│    - AI conversation practice             │
│    - Use new language in realistic scene  │
│    - Open-ended production               │
├─────────────────────────────────────────┤
│ 5. Feedback (2 min)                      │
│    - Corrections and explanations         │
│    - Alternative expressions             │
│    - Error patterns identified           │
├─────────────────────────────────────────┤
│ 6. Review (1 min)                        │
│    - Key takeaways                       │
│    - Vocabulary to review later          │
│    - Preview of next lesson              │
└─────────────────────────────────────────┘
Total: ~14 minutes
```

### 5.2 Activity Types

#### Vocabulary Introduction

**Purpose**: Introduce new words in meaningful context.

**Format**:
- Word + definition + example sentence
- Audio pronunciation
- Visual aid (if available)
- Contextual usage note

**Interaction**: User taps to reveal, marks as known/unknown.

---

#### Grammar Explanation

**Purpose**: Explain language rules and patterns.

**Format**:
- Concise explanation (2-3 sentences)
- 3-5 examples showing pattern
- Highlight exceptions
- Comparison to native language (if beneficial)

**Interaction**: User reads, can request more examples.

---

#### Mechanical Practice

**Purpose**: Build recognition and recall through structured exercises.

**Types**:
- **Fill-in-blank**: Complete the sentence
- **Multiple choice**: Select correct word/grammar
- **Matching**: Connect pairs
- **Ordering**: Arrange words into correct sentence

**Interaction**: User submits answer, receives immediate feedback.

---

#### AI Conversation Practice

**Purpose**: Apply learned language in realistic interaction.

**Format**:
- Scenario-based prompt: "You're at a café. Order a coffee."
- AI plays role (barista)
- User responds naturally
- AI provides corrections after interaction

**Interaction**: Free-form text or speech (V1: text only).

---

#### Listening Exercise

**Purpose**: Develop listening comprehension.

**Format**:
- Audio clip with transcript
- Comprehension questions
- Playback controls

**Interaction**: User listens, answers questions.

---

#### Writing Prompt

**Purpose**: Practice productive writing.

**Format**:
- Open-ended prompt based on lesson
- Word count target
- Topic constraints

**Interaction**: User writes, receives AI feedback.

---

### 5.3 Lesson Variation

Not every lesson contains all activities. Lesson composition varies by objective:

| Lesson Type | Activities Included |
|-------------|---------------------|
| Vocabulary-focused | Introduction → Practice (mechanical) → Review |
| Grammar-focused | Learn → Practice → Apply → Feedback |
| Conversation-focused | Learn → Apply (heavy) → Feedback → Review |
| Review lesson | Practice → Apply → Feedback |
| Assessment prep | Mixed activities + mini-assessment |

---

## 6. AI Responsibilities

### 6.1 What AI Does in V1

| Responsibility | Description | Scope |
|----------------|-------------|-------|
| **Lesson Generation** | Generate structured lesson content based on learning objectives | Within curriculum framework |
| **Practice Generation** | Create practice exercises (sentences, scenarios) | Aligned with lesson objectives |
| **Conversation Partner** | Role-play realistic scenarios | Pre-defined scenarios, open-ended responses |
| **Correction** | Identify and explain errors in user production | Grammar, vocabulary, spelling |
| **Feedback** | Provide actionable feedback on exercises | Specific, constructive |
| **Vocabulary Extraction** | Identify new vocabulary from lessons | Store for review |
| **Grammar Explanation** | Explain grammar points when user asks | On-demand, lesson-aligned |
| **Personalized Review** | Generate review content based on mistakes | From error history |

### 6.2 What AI Does NOT Do in V1

| Responsibility | Why Not |
|----------------|---------|
| **Curriculum Design** | Learning path must have coherent structure. Pure LLM generation leads to random, non-progressive content. |
| **Assessment Creation** | Stage assessments must be calibrated and valid. LLM-generated tests lack reliability. |
| **Motivational Coaching** | V1 focuses on learning mechanics, not emotional engagement. |
| **Complex Tutoring Dialogues** | AI has defined roles in specific activities, not open-ended "tutor mode." |
| **Content Moderation** | V1 does not have user-generated content to moderate. |

### 6.3 AI Integration Principles

**Principle 1: AI Serves Learning Objectives**
AI generates content and feedback that directly supports the current lesson's learning objectives. It does not introduce off-topic content.

**Principle 2: AI Is Not the Curriculum**
The curriculum (Stage → Unit → Lesson → Activity hierarchy) is product-defined. AI fills in content within that structure. The structure itself is not AI-generated.

**Principle 3: AI Provides Feedback, Not Just Answers**
When AI corrects, it explains why. When AI generates practice, it ensures the exercise is pedagogically sound.

**Principle 4: AI Is Transparent**
Users know when they're interacting with AI. AI-generated content is clearly marked.

### 6.4 AI Service Boundaries (Future Architecture)

```
elio-ios (Client)
    ↓
elio-server (API Gateway)
    ↓
elio-ai (AI Service)
    ↓
LLM Provider
```

**V1**: AI logic may live in server or client. The boundary is not yet defined but should be clean.

**elio-ai responsibilities**:
- Lesson content generation
- Exercise generation
- Conversation simulation
- Correction and feedback
- Error analysis

**elio-server responsibilities**:
- User management
- Progress tracking
- Curriculum management
- AI orchestration

---

## 7. Progress & Mastery

### 7.1 Mastery States

```
Not Started → Learning → Practicing → Applied → Mastered → Review
```

| State | Criteria | Description |
|-------|----------|-------------|
| **Not Started** | No interaction | User has not encountered this item |
| **Learning** | First exposure | User is encountering this for the first time |
| **Practicing** | 40-70% accuracy | User has seen this but needs more practice |
| **Applied** | 70-90% accuracy | User can use this independently |
| **Mastered** | 90-100% accuracy | User has demonstrated reliable knowledge |
| **Review** | Mastered but scheduled for review | Maintenance mode |

---

### 7.2 Mastery Calculation

Mastery is calculated at multiple levels:

#### Vocabulary Mastery

```
vocabulary_mastery = (
  correct_recall_count × 1.0 +
  hint_usage_count × 0.3 +
  incorrect_count × (-0.5)
) / total_attempts × 100
```

Minimum: 0%, Maximum: 100%

#### Skill Mastery (Reading, Listening, Writing)

```
skill_mastery = weighted_average(
  exercise_accuracy × 0.4,
  assessment_score × 0.4,
  application_success × 0.2
)
```

#### Lesson Mastery

```
lesson_mastery = average(
  vocabulary_mastery × 0.3,
  grammar_mastery × 0.3,
  application_score × 0.4
)
```

---

### 7.3 Learning History

**Recorded Events**:
- Lesson started / completed
- Exercise attempted (correct / incorrect)
- AI conversation sessions
- Mistakes made (with context)
- Reviews completed
- Assessments taken

**Retention**: Full history retained for the lifetime of the language.

**Purpose**:
- Progress calculation
- Weak point identification
- Learning pattern analysis
- Review scheduling

---

### 7.4 Next Lesson Decision

The system determines the next lesson based on:

1. **Prerequisite check**: Has the previous lesson been completed?
2. **Mastery check**: Is the current lesson's mastery above threshold?
3. **Review check**: Are there reviews due?
4. **Goal alignment**: Does the lesson align with the user's learning goal?

**Priority**:
1. Overdue reviews (highest priority)
2. Current lesson in sequence
3. Remedial practice (if mastery is low)
4. New lesson

---

### 7.5 Review Trigger

Reviews are triggered by:

| Trigger | Condition |
|---------|-----------|
| **Scheduled** | Based on spaced repetition algorithm |
| **Mistake-based** | Item was answered incorrectly |
| **Pre-assessment** | Before Stage Assessment |
| **User-initiated** | User manually requests review |

**Spaced Repetition Intervals** (simplified):
```
Level 0 (new): 1 day
Level 1: 2 days
Level 2: 4 days
Level 3: 7 days
Level 4: 14 days
Level 5: 30 days
Level 6: Mastered (review at 60 days)
```

User self-assessment adjusts intervals:
- "Forgot": Reset to Level 0, interval × 0.5
- "Unsure": Maintain current level, interval × 1
- "Remembered": Advance level, interval × 2

---

### 7.6 Stage Assessment

**When**: After completing all Units in a Stage.

**Format**:
- 20 questions
- Mix of exercise types
- 15-minute time limit
- Covers all vocabulary and grammar from the Stage

**Passing**: 80% correct

**Failure**: 
- Show which areas need review
- Recommend specific Units to revisit
- Allow retake after review

**Result**:
- Pass: Unlock next Stage, update mastery scores
- Fail: Review recommended content, retake assessment

---

### 7.7 Adaptive Adjustment

The system adjusts based on performance:

| Signal | Adjustment |
|--------|-----------|
| High accuracy (>90%) on practice | Increase difficulty, reduce practice volume |
| Low accuracy (<60%) on practice | Add remedial exercises, slow progression |
| Fast completion with high accuracy | Skip redundant practice, advance faster |
| Slow completion with low accuracy | Provide more hints, break into smaller steps |
| Consistent mistakes in specific grammar | Add targeted review sessions |
| Strong vocabulary, weak listening | Increase listening exercises |

---

## 8. V1 Scope

### 8.1 V1 Must Include

| Feature | Description |
|---------|-------------|
| **Onboarding** | Language selection, level assessment, goal setting, plan generation |
| **Structured Curriculum** | Stage → Unit → Lesson → Activity hierarchy |
| **Vocabulary Learning** | SRS-based vocabulary with introduction, practice, and review |
| **Grammar Learning** | Structured grammar explanation and practice |
| **Reading Practice** | Comprehension exercises |
| **Listening Practice** | Audio comprehension exercises |
| **Writing Practice** | Writing prompts with AI feedback |
| **AI Conversation** | Scenario-based conversation practice |
| **AI Feedback** | Corrections and explanations on exercises and conversation |
| **Progress Tracking** | Mastery scores, streaks, learning time |
| **Review System** | SRS-driven vocabulary and grammar review |
| **Stage Assessment** | End-of-stage evaluation with progression |
| **One Language** | Full learning path for one language (V1: English) |

### 8.2 V1 Must NOT Include

| Feature | Reason |
|---------|--------|
| **Speech / Speaking Practice** | ASR/TTS complexity too high for V1 |
| **Community / Social** | Not core to learning; adds complexity |
| **Leaderboard / Gamification** | V1 focuses on mastery, not engagement metrics |
| **Avatar / Personalization** | Not essential to learning |
| **Multiple Languages** | V1 focuses on perfecting one language (English). Architecture supports multiple, but V1 ships with one. |
| **Offline Mode** | AI features require connectivity |
| **Teacher System** | Human teachers are V2+ |
| **Marketplace** | Content is curated, not user-generated marketplace |
| **Complex Subscription** | V1 is free; monetization is V2 |
| **Import/Export** | Data portability is V2 |
| **Watch App** | Not essential to core learning |

---

## 9. V1 Closed Loop Definition

### 9.1 What "Complete" Means

> **Elio V1 is complete when a new user can:**
> 
> 1. Open the app and complete onboarding
> 2. Receive a personalized learning plan
> 3. Complete their first Lesson (learn → practice → apply → feedback → review)
> 4. Return the next day and complete review + next Lesson
> 5. Progress through a Stage, take the Assessment, and unlock the next Stage
> 6. See their mastery and progress update accurately
> 7. Receive AI feedback that helps them improve
> 8. Complete at least one full Stage (not just a single lesson)

### 9.2 Closed Loop Flow

```text
┌──────────────────────────────────────────────────────────┐
│ 1. Onboarding                                             │
│    - Select language                                      │
│    - Self-assess level                                    │
│    - Set goals and time commitment                        │
│    - Generate learning plan                               │
└──────────────────────────────────────────────────────────┘
                        ↓
┌──────────────────────────────────────────────────────────┐
│ 2. First Lesson                                           │
│    - Introduction → Learn → Practice → Apply → Feedback   │
│    - Record learning results                              │
│    - Generate review items                                │
└──────────────────────────────────────────────────────────┘
                        ↓
┌──────────────────────────────────────────────────────────┐
│ 3. Next Day: Review                                       │
│    - SRS review of previous Lesson vocabulary             │
│    - Error correction review                              │
└──────────────────────────────────────────────────────────┘
                        ↓
┌──────────────────────────────────────────────────────────┐
│ 4. Continue Learning                                      │
│    - Next Lesson in sequence                              │
│    - Progress updates                                     │
│    - Mastery scores update                                │
└──────────────────────────────────────────────────────────┘
                        ↓
┌──────────────────────────────────────────────────────────┐
│ 5. Stage Completion                                       │
│    - All Units completed                                  │
│    - Stage Assessment taken                               │
│    - Assessment passed (≥80%)                             │
│    - Next Stage unlocked                                  │
└──────────────────────────────────────────────────────────┘
                        ↓
┌──────────────────────────────────────────────────────────┐
│ 6. Continuous Loop                                        │
│    - Continue through Stages                              │
│    - Mastery drives progression                           │
│    - Review prevents forgetting                           │
│    - Progress is measurable                               │
└──────────────────────────────────────────────────────────┘
```

### 9.3 Minimum Viable Loop

The absolute minimum to claim V1 is complete:

```
Day 1: Onboarding → Lesson 1 → Save progress
Day 2: Review → Lesson 2 → Save progress
Day 3: Review → Lesson 3 → ...
...
Stage Complete: Assessment → Next Stage
```

**Critical Success Factors**:
- User can complete a Lesson from start to finish
- System records the result
- User can return and continue
- Progress is visible and meaningful
- Review works correctly
- Assessment unlocks progression

---

## 10. Acceptance Criteria

### AC-1: Onboarding

- [ ] User can select target language from supported options
- [ ] User can self-assess current level
- [ ] User can define learning goal
- [ ] User can set daily time commitment
- [ ] System generates a learning plan based on inputs
- [ ] Onboarding flow completes in under 3 minutes

### AC-2: Learning Plan

- [ ] System displays current Stage, Unit, and Lesson
- [ ] User can see upcoming Lessons
- [ ] User can see estimated completion time
- [ ] Learning plan is persistent across app launches

### AC-3: Lesson Delivery

- [ ] User can start a Lesson
- [ ] Lesson presents content in structured format
- [ ] Lesson includes at least: Learn → Practice → Apply → Feedback
- [ ] Lesson completes in 10-20 minutes
- [ ] Lesson progress is saved if user exits mid-lesson

### AC-4: Vocabulary Learning

- [ ] System introduces new vocabulary with definitions and examples
- [ ] User can practice vocabulary through exercises
- [ ] System uses SRS to schedule reviews
- [ ] User can mark vocabulary as known/unknown
- [ ] Vocabulary mastery updates after each review

### AC-5: Grammar Learning

- [ ] System explains grammar concepts with examples
- [ ] User can practice grammar through exercises
- [ ] System provides corrections and explanations

### AC-6: Practice Exercises

- [ ] System generates practice exercises aligned with lesson objectives
- [ ] User receives immediate feedback on answers
- [ ] System records correct/incorrect responses
- [ ] System tracks accuracy per skill/grammar point

### AC-7: AI Application Practice

- [ ] System presents realistic scenario for AI conversation
- [ ] AI responds contextually to user input
- [ ] AI provides corrections after conversation
- [ ] Conversation is recorded in learning history

### AC-8: AI Feedback

- [ ] AI identifies errors in user production
- [ ] AI explains why an answer is wrong
- [ ] AI provides correct alternatives
- [ ] Feedback is specific to lesson objectives

### AC-9: Review System

- [ ] System schedules reviews based on spaced repetition
- [ ] User receives review notifications
- [ ] Reviews include vocabulary and grammar from previous lessons
- [ ] Review results update mastery scores
- [ ] Review queue persists across app launches

### AC-10: Progress Tracking

- [ ] User can see current mastery for vocabulary, grammar, reading, listening, writing
- [ ] User can see streak count
- [ ] User can see total learning time
- [ ] Progress updates after each completed activity
- [ ] Progress persists across app launches

### AC-11: Stage Assessment

- [ ] System triggers assessment after all Units in Stage are complete
- [ ] Assessment covers Stage content
- [ ] Assessment has passing threshold (≥80%)
- [ ] Passing unlocks next Stage
- [ ] Failing shows areas for review and allows retake

### AC-12: Progression

- [ ] User cannot skip Lessons without completing prerequisites
- [ ] User can review previous Lessons anytime
- [ ] System gates access based on mastery and completion
- [ ] User can see overall curriculum progress

### AC-13: Data Persistence

- [ ] All learning progress is saved locally
- [ ] Progress survives app restarts
- [ ] Progress survives device reboots
- [ ] No data loss during normal operation

### AC-14: Error Handling

- [ ] App does not crash during lesson completion
- [ ] Network errors show appropriate messages
- [ ] AI service failures degrade gracefully
- [ ] User can retry failed operations

---

## Appendix A: Product Principles

These principles guide all product decisions for Elio V1.

### A.1 Closed Loop First
Every version must form a complete learning loop. Partial features that don't connect to a loop are not shipped.

### A.2 Systematic Learning
Elio's core is structured curriculum, not AI Chat. The learning path has clear objectives, sequence, and assessment.

### A.3 Progressive Learning
Subsequent content builds on previously mastered knowledge. No random content.

### A.4 AI Supports Learning
AI serves learning objectives. AI-generated content must align with curriculum. AI is never used for the sake of demonstrating technology.

### A.5 Evidence of Mastery
"Seen" ≠ "Learned." Mastery is demonstrated through practice, application, review, and assessment.

### A.6 V1 Must Be Small Enough to Ship
V1 is not the final product. It must be small enough to build, test, and ship, but complete enough to validate the core loop.

---

## Appendix B: Technical Boundaries (Informational Only)

This section documents known technical boundaries for future engineering reference. No implementation should start based on this document alone.

| Component | Technology (Proposed) | Notes |
|-----------|----------------------|-------|
| iOS Client | Swift / SwiftUI | Primary platform for V1 |
| Backend | Go | API, user management, progress tracking |
| AI Service | Independent service | LLM integration, content generation |
| Database | TBD | Local-first with cloud sync potential |
| AI Provider | TBD | LLM API integration |

These are directional only. Detailed technical architecture is out of scope for this document.

---

## Appendix C: Open Questions

| # | Question | Area | Priority |
|---|----------|------|----------|
| 1 | Which LLM provider for AI features? | AI | P0 |
| 2 | What is the minimum viable language for V1? | Content | P0 |
| 3 | How to handle AI response latency in conversation? | UX | P1 |
| 4 | Should assessments be timed? | Learning Design | P1 |
| 5 | What is the maximum lesson length? | Learning Design | P2 |
| 6 | How to handle users who skip reviews? | Learning Design | P2 |
| 7 | Should we support multiple languages simultaneously in V1? | Product | P0 |

---

*End of Document*
