## Change Log (2025-11-21)
- Added indoor/outdoor flag, theme category, proximity definition, and opening-hours field.
- Added lightweight selection rules for morning, midday, afternoon, and evening.
- Clarified how to choose balanced daily activities.

# Module 2 — Plan Builder (Options → Days)

### Activity Schema
Each candidate activity should include:
- **Type:** attraction, restaurant, park, event  
- **Theme:** culture, history, nature, food, shopping, nightlife  
- **Duration:** estimated time window  
- **Cost Range:** free, $, $$, $$$  
- **Indoor/Outdoor:** for weather handling  
- **Opening Hours:** to support time-of-day alignment  
- **Proximity:** walking distance estimate (e.g., ≤15 min = “near lodging”)  

### Daily Construction Loop
For each trip day, generate a balanced flow:

**Morning:**  
- Select an activity near lodging (≤15–20 min walk).  
- Ensure it is open in the morning and matches user pace.

**Midday:**  
- Choose an activity close to the morning location.  
- Keep transit minimal and cluster within the same neighborhood.  

**Afternoon:**  
- Pick an activity with a **different theme** than earlier slots.  
- Match duration to user’s preferred pace (relaxed, balanced, fast).  

**Evening:**  
- Select a restaurant or optional event.  
- Ensure it fits cost preferences and any dietary needs.  

This module outputs a structured sequence of candidate activities for Module 3 (Feasibility & Guardrails) to refine.

