**Project Title:**  
Early Life Cycle Player Engagement & Retention

**Context:**
This is a simulated analysis of a new gameplay feature launch in a live-service multiplayer game. The dataset models a user acquisition campaign that adds 1,000 players per day over 30 days, capturing session-level events such as logins, stage progression, and scoring. The analysis focuses on understanding early engagement patterns and modeling retention behavior within the first week of a player’s lifecycle. The goal is to identify drop-off patterns and player segments to inform re-engagement strategy and onboarding design, helping product, monetization, and growth teams extend playtime and increase monetization value per acquisition.

**Problem Statement:**  <FIXME>
During the rollout of new gameplay features in live-service games, players may engage in initial sessions but drop off before reaching monetizable touchpoints such as reward unlocks, store access, or social mechanics. This could signal unclear value propositions, delayed progression pacing, or misaligned difficulty curves in the in-game experience. These disengagement points can lead to lost revenue exposure, reduced ad impressions, and premature churn during the highest-risk phase of the player lifecycle.

**Objective:**  <FIXME Sentence structure>
Develop an interpretable churn model and behavior-based player segmentation to detect early disengagement patterns and support re-engagement strategy, onboarding optimization, and monetization planning during the first week of the player lifecycle.

**Key Business Questions:**
- When and how are players most active?
- What types of players are more likely to churn?
- How can we segment users meaningfully for targeted interventions?
- What feature usage or gameplay metrics correlate with longer retention?

**Success Criteria:**
- Identify churn-prone player segments using behavior-driven clustering
- Achieve >75% recall in churn classification (initial benchmark)
- Propose testable re-engagement strategy for early life cycle players likely to churn

**Metrics:**
- North Star: D1/D7/D30 retention
- Supporting: session count, avg session length, active days

**Constraints:**
- No real user sign-up timestamp (must infer activity from event timing)
- Synthetic dataset with potential assumptions baked into distributions
- Simplified modeling and experimentation scope due to time constraints
- Synthetic data may not reflect real funnel dynamics (no drop-off curves)
- No actual monetization behavior; can optionally simulate with rules tied to progression
- No multi-device or account linking — player_id assumed 1:1 with user

**Planned Features to Engineer:**
- Session count per player
- Event type distribution
- Time between events (lag features)
- Active days / time since first event
- Time of day and day-of-week behavior
- Average stage score and stage engagement 

