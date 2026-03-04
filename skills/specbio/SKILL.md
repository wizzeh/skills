---
name: specbio
description: Create speculative organisms for the Ellieworld worldbuilding project. Use whenever designing, inventing, or filling ecological niches with new organisms for this world. Generates structured specs and prose descriptions validated against hard planetary constraints and critiqued for evolutionary plausibility.
---

# Specbio — Organism Creation for Ellieworld

## Before You Begin

Read the project worldbuilding docs to ground yourself. At minimum:

- `docs/phylogeny.md` — clade tree and evolutionary logic
- `docs/naming-morphemes.md` — taxonomic naming system
- `docs/mat-bestiary.md` — detailed organism profiles (the quality bar for output)

For deeper context (read as needed):

- `docs/ocean-ecology.md` — mat structure, shedding, productivity
- `docs/ellieworld.md` — planetary parameters, climate, geography
- `docs/plans/2026-02-18-ir-photosynthesis-design.md` — IR photosynthesis biochemistry

Read [references/constraints.md](references/constraints.md) for the condensed physical constraints.

## Workflow

### 1. Establish the Niche

What ecological role? Specify habitat (mat underside, mat top, mat interior, water column, land, vent, coastal), trophic role (producer, grazer, filter-feeder, predator, parasite, mutualist, scavenger, detritivore), and geographic zone (substellar, day-side, terminator, night-side).

### 2. Place in the Tree

Every organism needs a phylogenetic position. Read `docs/phylogeny.md` for the current tree. Placement determines inherited toolkit — an organism can't have capabilities its ancestors never evolved unless convergence is explicitly justified.

### 3. Design the Organism

Output format:

```markdown
## [Common Name] — [One-line ecological identity]

**Clade:** [phylogenetic position]
**Habitat:** [where it lives]
**Symmetry:** [inherited or derived, justified if derived]
**Size:** [dimensions + mass]
**Metabolism:** [energy source]
**Skeleton/structure:** [materials, architecture]
**Sensory:** [modalities, justified by habitat]
**Locomotion:** [mechanism or sessile]
**Feeding:** [mechanism, diet, rate]
**Reproduction:** [mode, output, timing]
**Shedding strategy:** [how it survives, or why it doesn't need to]
**Lifespan:** [duration, iteroparity/semelparity]

### Anatomy

[Detailed morphological description. Specific dimensions, materials, mechanisms.
Match the detail level of docs/mat-bestiary.md entries.]

### Ecology

[Interactions: predators, prey, mutualists, competitors. Community-level effects.]

### Life Cycle

[Developmental stages, transitions, timing.]

### Evolutionary Notes

[What selective pressures shaped this. What ancestral features retained or lost. Why this organism exists.]

"[Closing line — poetic, one sentence, in quotes.]"
```

### 4. Name It

Combine morphemes from `docs/naming-morphemes.md`: 2-4 morphemes encoding the most distinctive features + suffix. Common name stays evocative and short.

### 5. Validate

Check against physical constraints (see [references/constraints.md](references/constraints.md)):

- [ ] No visible light — all vision is IR
- [ ] Surface gravity is 1.95g — weight budgets reflect this
- [ ] Tidally locked: no day-night cycle, no seasons. Geography IS climate
- [ ] Night side: no photosynthesis possible
- [ ] 3,100 hPa, 12.9% CO₂ atmosphere
- [ ] Ocean mixed layer: 700m, violently convective, no stratification except under mat
- [ ] Photic zone ~5m deep (IR absorbed by water)
- [ ] Silicic acid, iron, sulfur abundant. Calcium carbonate and chitin absent
- [ ] Atmospheric IR windows constrain which wavelengths reach the surface

Check against current biology (read the docs for current state):

- [ ] Pigment availability matches habitat (water absorbs longer IR)
- [ ] Sensory modalities match habitat (vision only where IR-lit)
- [ ] Symmetry justified by clade placement
- [ ] Shedding strategy exists or organism is expendable
- [ ] Mat carrying capacity respected
- [ ] Biomaterials are world-appropriate (silica dominant, no Earth-specific materials)
- [ ] Body plan consistent with clade's ancestral toolkit

### 6. Critique

After validation, assess evolutionary plausibility:

- **Selection pressure:** What specific predator, parasite, or constraint drives the distinctive traits?
- **Trade-offs:** What does this organism sacrifice? Every adaptation has a cost.
- **Failure modes:** How does it die? What kills most individuals?
- **Competitive exclusion:** Why doesn't an existing organism already fill this niche?
- **Convergence check:** If it resembles an Earth organism, justify why similar physics/ecology produces similar solutions — or revise.
- **Weaknesses:** 2-3 specific vulnerabilities.

## Style Notes

Match the voice of `docs/mat-bestiary.md`: scientifically rigorous, mechanistically specific, with a closing poetic line in quotes. Dimensions in metric. Biological detail should be concrete enough that someone could build a simulation from it.
