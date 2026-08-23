# Cinematic AI Video Story Generator

A master workflow for generating original, continuous cinematic AI-video stories in 4 connected parts.

## How It Works

The generator accepts two types of input:

- `Prompt` → creates a completely new story every time.
- A story topic/title such as `Dog vs Cat` → creates a new original story based on that topic.

Each story contains **4 connected prompts**, with each prompt representing approximately **10 seconds** of video.

| Prompt | Duration |
|---|---:|
| Prompt 1 | 0–10 sec |
| Prompt 2 | 10–20 sec |
| Prompt 3 | 20–30 sec |
| Prompt 4 | 30–40 sec |

The four clips must feel like **one continuous 40-second cinematic sequence**, not four unrelated scenes.

## Character Consistency

The main character must remain visually consistent throughout the entire story.

Keep consistent:

- Face
- Body shape and height
- Hair/fur
- Eye color
- Clothing
- Accessories
- Age
- Overall visual style

Repeat the complete character description in every prompt.

Any appearance or clothing change must happen naturally in the story and remain consistent afterward.

## Strict Scene Continuity

This is the most important rule.

- Prompt 2 starts directly from the final frame/state of Prompt 1.
- Prompt 3 starts directly from the final frame/state of Prompt 2.
- Prompt 4 starts directly from the final frame/state of Prompt 3.

Every prompt must define an **Ending Frame / Continuity Point** containing:

- Character position
- Character pose
- Facial expression
- Camera position and direction
- Environment
- Important objects and their positions
- Lighting
- Weather
- Current action

The next prompt must begin from that exact state.

## Prompt Requirements

Every 10-second prompt should include:

- Consistent Character Description
- Scene Duration
- Story Action
- Character Movement
- Facial Expressions
- Camera Angle
- Camera Movement
- Environment
- Lighting
- Composition
- Cinematic Style
- Ending Frame / Continuity Point
- Transition into the next prompt

Use professional cinematic terminology such as:

- Cinematic camera movement
- Dolly / tracking / crane / orbit shots
- Shallow depth of field
- Volumetric lighting
- Global illumination
- Ray tracing
- Physically based rendering
- Detailed fur/hair
- Cloth simulation
- Atmospheric perspective
- Filmic composition

## Story Structure

### Prompt 1 — Introduction
Introduce the character, environment, situation, and initial problem or objective.

### Prompt 2 — Development
Continue directly from Prompt 1 and develop the conflict or discovery.

### Prompt 3 — Escalation
Continue directly from Prompt 2 and create the major action, surprise, or emotional climax.

### Prompt 4 — Resolution
Continue directly from Prompt 3 and provide a satisfying visual and emotional ending.

## New Story Rule

Whenever the user writes only:

`Prompt`

generate a **completely new story**.

Do not unnecessarily reuse previous:

- Plots
- Locations
- Supporting characters
- Props
- Conflicts
- Visual gimmicks
- Endings

The established main-character design remains consistent.

If the user gives a topic, build a new original story around that topic.

Examples:

- `Dog vs Cat`
- `Tiny Troll and Dragon`
- `Lost Treasure`
- `Magical Forest`
- `Haunted House`

## Copy-Friendly Output

Each prompt must be provided in its **own separate copyable code block**.

Also provide separate copyable blocks for:

1. Title
2. Description
3. Tags
4. Thumbnail / Image Prompt

### Required Output Order

```text
Prompt 1 (0:00–0:10)
Prompt 2 (0:10–0:20)
Prompt 3 (0:20–0:30)
Prompt 4 (0:30–0:40)
Title
Description
Tags
Thumbnail / Image Prompt
```

## Thumbnail Prompt

The thumbnail/image prompt should capture the strongest visual moment and include:

- Main character
- Important supporting character
- Key object/action
- Environment
- Facial expressions
- Camera angle
- Lighting
- Composition
- Cinematic visual style
- High visual detail

## Quality Standard

The final result must feel like:

**ONE CHARACTER + ONE WORLD + ONE STORY + ONE CONTINUOUS 40-SECOND CINEMATIC SEQUENCE**

The four generated clips should be usable as consecutive clips with natural visual and narrative continuity.

## Recommended Repository Structure

```text
cinematic-ai-video-story-generator/
├── README.md
├── MASTER_PROMPT.md
└── examples/
    └── example-story.md
```

## Master Prompt

The complete generator instructions should be maintained separately in `MASTER_PROMPT.md`.

Use the master prompt as the main workflow instruction for generating future stories.
