# TouchGrass FieldAgent

An edge-optimized AI field agent designed to process raw trail observations, audio transcripts, and environmental conditions into structured, deterministic action plans.

## Purpose
Built for the DEV Hacktoberfest 2026 "TouchGrass" challenge. The goal is to minimize screen time by delivering immediate safety checks and concise plans for outdoor activity.

## System Architecture
- **Control Plane:** Relevance AI Workflow Orchestration
- **Inference Layer:** Google Gemma Open-Weight Model Engine
- **Data Format:** Enforced Strict JSON Schema

## Output Contract
```json
{
  "actionable_plan": [
    "Start now; use upper trail only and avoid lower ledge after 3:15 PM high tide.",
    "Limit route to a 20-minute out-and-back trail check on dry, stable sections.",
    "Turn around immediately at slick rock steps or wave splash zones."
  ],
  "safety_checklist": [
    "Watch footing on sea-spray-slick descent steps.",
    "Stay clear of edge exposure and lower ledge during high tide.",
    "Keep phone away; use audio/vibration only if needed."
  ],
  "offline_summary": "20-minute upper-trail check only at Sunset Cliffs; slick steps and 3:15 PM high tide make the lower ledge unsafe."
}
## Submission & Technical Article
- **DEV Community Submission:** [TouchGrass FieldAgent Article](https://dev.to/rcortez056/touchgrass-fieldagent-an-open-source-field-companion-designed-for-zero-screen-time-5d22)
