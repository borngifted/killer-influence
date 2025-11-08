# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**Killer Influence** is a survival-horror visual content project combining AI-generated imagery with video production. The project follows nine influencers trapped in a modular soundstage death game, blending SAW-style horror with SQUID GAME elimination mechanics and meta-commentary on algorithmic engagement.

**Core DNA:**
- SAW-style engineered kills
- SQUID GAME elimination structure
- One modular soundstage (sets S1-S9)
- Meta-viral engine tied to engagement metrics
- Visual language: 9:16 content frames vs. widescreen surveillance

## Project Structure

```
Killer_Influence/
├── Killer_Influence_MJ_Prompt_Pack_1.json  # Master scene prompts & technical specs
├── _scene_s{1-7}.mp4                        # Generated video sequences
├── S{1-7}_{1-8}.png                         # Scene stills/variants
├── Killer_Influence_Pitch_Deck.pdf          # Project pitch
├── Killer_Influence_Shot_List.pdf           # Production shot list
└── Killer_Influence_Quick_Reference.pdf     # Quick reference guide
```

## Production Pipeline

**Workflow:** Midjourney V7 → Veo3 → DaVinci Resolve

1. **Image Generation** (Midjourney V7): Generate 8K stills using scene prompts from JSON
2. **Hero Frame Selection**: Curate key art for each scene
3. **Motion Addition** (Veo3): Add camera movement, atmospheric FX, lighting effects
4. **Export**: 4K or 8K motion clips
5. **Post-Production** (DaVinci Resolve/Premiere): UI overlays, sound design, color grading

## Scene Architecture

The project uses 7 core modular sets (S1-S7), each with distinct:
- **Narrative context**: Story beat, characters, key moments
- **Visual identity**: Lighting mood, color palette, camera specs
- **Technical specifications**: Camera model, lens, aperture, movement style
- **Aspect ratio variants**: 21:9 (cinematic), 16:9 (standard), 9:16 (social/vertical)

### Key Scenes

- **S1 - Red Corridor**: Entrance/execution zone (neon noir aesthetic)
- **S2 - Asylum Wing**: Medical horror set (clinical decay)
- **S3 - Detention Block**: School hallway nostalgia trap
- **S4 - The Guts**: Industrial boiler room (SAW-style mechanical horror)
- **S5 - The Panopticon**: TV studio/control room (meta-layer, most thematically important)
- **S6 - The Open Room**: Arena reveal overhead shot
- **S7 - The Open Space**: Exit illusion/finale

## Lighting Moods

Each scene uses one of four core lighting moods defined in the JSON:

- **neon_noir**: Red/blue mixed light (#ef4444, #1e3a8a)
- **clinical_decay**: Sickly greens/fluorescents (#84cc16, #e5e7eb)
- **industrial_heat**: Tungsten orange/steam (#f97316, #7c2d12)
- **surveillance_cold**: White overhead/hard shadows (#f3f4f6, #1f2937)

## Aspect Ratio Strategy

- **21:9** (ultra-widescreen): Epic dread, spatial horror, surveillance shots
- **16:9** (standard): Traditional cinematic moments, ensemble shots
- **9:16** (vertical): Social media POVs, character reactions, "viral content" within story

Vertical content requires post-production UI overlays (likes, comments, engagement metrics).

## Character System

Key characters represented as silhouettes:
- **LEXI**: Final Girl - SFX Artist (~3M followers)
- **KAM**: Director (~10M followers)
- **TRISH & JOSH**: The Couple (3M combined)
- **SYLVIA**: Writer (off-grid)
- **THE VOICE**: The Showrunner (visual: red speaker grilles, surveillance cameras)

Prompts use silhouettes with characteristic body language and props rather than facial detail.

## Technical Specifications

All prompts include cinema camera specifications:
- **Cameras**: ARRI Alexa Mini LF/LF, Sony FX6/Venice, Canon C300 Mark III, Blackmagic URSA Mini Pro G2
- **Lenses**: 24mm-65mm primes, varying apertures (f/1.8-f/2.8)
- **Movement styles**: Handheld, steady-cam tracking, low angle, overhead drone
- **Resolution target**: 8K for stills, 4K-8K for motion sequences

## Working with the JSON Prompt Pack

The `Killer_Influence_MJ_Prompt_Pack_1.json` contains:

- **Project metadata**: Title, tagline, DNA, visual language
- **Lighting moods**: Color palettes with hex codes and use cases
- **Scene definitions**: Full prompts with narrative context and technical specs
- **Aspect ratio guide**: Usage guidelines for each format
- **Workflow pipeline**: Step-by-step production process
- **Character variants**: Prompt addons for key characters
- **Color palette**: Project-wide color system

When generating new scenes or variants:
1. Reference the appropriate lighting mood
2. Match camera/lens specs to narrative tone
3. Choose aspect ratio based on intended use
4. Include technical parameters (seed, negative prompts)
5. Maintain silhouette-based character representation

## File Naming Convention

- Videos: `_scene_s{scene_number}.mp4` (e.g., `_scene_s1.mp4`)
- Images: `S{scene_number}_{variant_number}.png` (e.g., `S1_1.png`, `S5_2.png`)

## Thematic Consistency

Maintain these core horror elements across all content:
- **Algorithmic horror**: Engagement metrics = life/death
- **Meta-commentary**: Audience complicity, performance vs. punishment
- **Spatial dread**: Modular soundstage as surveillance panopticon
- **Found footage authenticity**: Film grain, handheld movement, analog texture
- **Color symbolism**: Red = danger/recording, white = audience/exposure, green = decay
