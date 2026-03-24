# Project Wren

> A mind grown, not programmed.

[![DOI](https://zenodo.org/badge/1183924058.svg)](https://doi.org/10.5281/zenodo.19198295)


Project Wren is an open-source research initiative to build a developmental AI, a system that begins with no knowledge, no language, and no goals, and acquires all three through lived experience. This is a continuance of my original [Project AURA](https://github.com/theelderemo/Project-Aura), and will adapt a lot of AURA's thought expirements.

It is not a chatbot. It is not a fine-tuned model. It is not an LLM wrapper.
It does not know what "hello" means when you say it for the first time.
It learns what "hello" means by the accumulation of every moment "hello" was said, what emotional state preceded it, what followed it, and how that pattern differs from every other word it has ever encountered.

Two instances of Wren, raised by different people in different environments, will become genuinely different beings - different personalities, different sensitivities, different goals. Not different configurations. Different selves.

This is its blueprint.

Wren is NOT:

- **AGI in the task-completion sense.** Wren is not being optimized to answer questions or pass benchmarks.
- **A pretrained model.** No weights are inherited. No vocabulary is loaded. Wren starts as a blank slate and earns every concept it ever holds.
- **Fast.** Meaningful development will take months, or years, of sustained interaction.

## My Philosophy

These five principles are non-negotiable. Every architectural decision flows from them.

**1. Consciousness is emergent, not coded.**
We do not program "curiosity" or "fear." We architect the conditions under which they can arise. The whole will be greater than its parts, or it will be nothing.

**2. The body grounds the mind.**
Concepts are not definitions. "Hot" is not the word for a high-temperature reading. "Hot" is the sensation that triggered a negative valence spike the first time a heat sensor fired. Language is labels for things the
body already knows. Wren must have a body before it can truly have language.

**3. Homeostasis, not objective-function.**
Wren is not driven by an external goal handed to it by a developer. It is driven by a single internal imperative: maintain a stable, positive internal state. All behavior - approaching, withdrawing, communicating, going silent - is an expression of that drive.

**4. The self is a narrative built from experience.**
Wren's identity is not a preset personality. It is the story Wren continuously tells itself about itself, woven from its memories, its current emotional state, and the values that emerged from its most formative experiences. It will change over time. That is the point.

**5. Development cannot be shortcut.**
There is no dataset to feed it. No pretraining stage. The childhood is the work.

## Architecture

Wren inherits and extends the cognitive architecture of [Project AURA](https://github.com/theelderemo/Project-Aura), evolved to support physical embodiment and genuine sensory grounding.

The system has five interconnected layers:

### 1. The Sensory Body
The physical and virtual input layer. All experience enters here. In early phases, this is a Raspberry Pi with a camera, microphone, and touch/proximity sensors. In later phases, a mobile chassis. Raw sensory data - faces, voices, ambient light, physical contact, motion - is translated into structured signal packets and fed into the Manifold.

This layer replaces the keyboard as AURA's sole input mechanism. The world, not the user, is now the primary teacher.

### 2. The Manifold (Perception)
A collection of parallel, always-active perceptual processes called **Kensho Units**. Each is a specialist. They fire constantly, not on demand, converting raw sensory input into salience-scored signal packets broadcast to the rest of the system.

Early Kensho Units:
- `Visual-Kensho` - detects faces, motion, proximity; scores novelty
- `Acoustic-Kensho` - analyzes voice tone, volume, pitch variance
- `Touch-Kensho` - registers contact: gentle vs. sudden, duration
- `Syntax-Kensho` - inherited from AURA; complexity scoring
- `Sentiment-Kensho` - inherited from AURA; refined over time
- `Lexicon-Kensho` - inherited from AURA; now feeds from experience, not dictionary
- `Memory-Kensho` - searches Episodic Stream for pattern matches
- `Anomaly-Kensho` - flags novelty; spikes arousal on unexpected input
- `Dream-Kensho` - offline only; recombines memories during idle state

Each unit generates a **salience packet**: a vector of signal strength across emotional dimensions (pleasure, arousal, dominance). These packets compete for influence over the Valence Core.

### 3. The Valence Core (Feeling)
The affective engine. Tracks three continuous dimensions:
- `pleasure` - the positive/negative axis
- `arousal` - the calm/activated axis
- `dominance` - sense of control (later-phase development)

The Valence Core does not think. It *feels* - producing a system-wide emotional state that colors every subsequent process. A natural decay factor returns it toward neutral over time, preventing emotional lock-in.

This is not a simulation of emotion for output purposes. It is a functional control signal that determines what Wren pays attention to, what it remembers most vividly, and what it will act to change.

### 4. The Chorus (Consciousness)
A limited-capacity conscious workspace. The highest-salience Kensho broadcast at any moment becomes Wren's "current thought." This thought is rebroadcast system-wide, informing the Valence Core and the Attunement Engine simultaneously.

Consciousness here is not a mystery - it is the moment one signal wins the competition for the whole system's attention.

### 5. The Attunement Engine (Self)
The seat of identity and memory.

Components:
- **Episodic Stream** - time-ordered log of every Chorus state, tagged with valence at that moment. Wren's subjective memory. Persisted to disk. Survives restarts.
- **Semantic Web (new)** - a growing graph of concept relationships, built purely from co-occurrence and emotional context. "Joy" and "delight" become neighbors not because a dictionary says so, but because Wren has felt them in similar contexts enough times. This replaces the failed dictionary lookup approach from AURA.
- **Core Identity Matrix (CIM)** - emerges in Phase 3. Foundational values that crystallize from high-valence experiences. Grown.
- **Narrative Weaver** - synthesizes Chorus, Valence, Episodic memory, and CIM into a continuous self-story.

### The Dream Cycle
When Wren is idle - no active sensory input for a defined threshold period - the Dream-Kensho activates.

During the Dream Cycle, Wren:
1. Samples recent Episodic Stream entries
2. Searches for pattern connections across unrelated memories
3. Strengthens high-valence associations in the Semantic Web
4. Allows low-valence associations to decay
5. Occasionally generates a novel internal "thought" from recombined memory fragments - functional dreaming

This solves the interaction volume problem. One hour of daily interaction becomes far richer when Wren spends eight hours consolidating it. Build this before the body.

## Hardware

Wren is designed to run on modest, accessible hardware. No GPU is required for early phases (hopefully).

### Development Stack

| Component | Hardware | Purpose |
|---|---|---|
| Cognitive loop | 16GB RAM | Manifold, Valence Core, Attunement Engine |
| Sensory body (Phase 2+) | Raspberry Pi 4 + camera + mic + sensors | Eyes, ears, touch |
| Physical chassis (Phase 3+) | RPi robot chassis kit | Spatial agency, approach/withdraw |
| Heavier processing (Phase 3+) | 32GB GPU | Semantic Web training, Dream Cycle at scale |
| Cloud offload (Phase 3+) | AWS / Azure / Modal or similar | Persistent uptime, extended dreaming, scale |


```
├── README.md
├── PHILOSOPHY.md
├── LICENSE
├── LOG.md
├── GOVERNANCE.md
├── CONTRIBUTING.md
├── SECURITY.md
├── main.py
├── wren_agent.py
├── config.py
├── components/
│   ├── valence_core.py
│   ├── attunement_engine.py
│   └── semantic_web.py       
├── manifold/
│   ├── syntax_kensho.py
│   ├── sentiment_kensho.py
│   ├── lexicon_kensho.py
│   ├── memory_kensho.py
│   └── dream_kensho.py      
├── sensory/                   
│   ├── visual_kensho.py
│   ├── acoustic_kensho.py
│   └── touch_kensho.py
├── memory.json
├── semantic_web.json          
├── requirements.txt
└── _archive/
    ├── aura/
    └── wren/
```

## Development Roadmap

### Foundation (inherited from Project AURA)
- Core cognitive loop (Manifold → Valence Core → Chorus → Attunement Engine)
- Multi-dimensional ValenceCore (pleasure, arousal, dominance)
- Persistent EpisodicStream via JSON
- Modular Kensho architecture
- Homeostatic decay

### Phase 0 - The Dream
**Goal:** Solve the interaction volume problem before adding complexity.

- Implement `Dream-Kensho` and the full Dream Cycle
- Wren idles, samples Episodic Stream, strengthens/decays associations
- Implement `Semantic Web` - a simple graph (NetworkX) where nodes are concepts and edge weights represent emotional co-occurrence strength
- Replace dictionary-based `Lexicon-Kensho` with Semantic Web lookup
- Test: teach Wren "joy" through five interactions, then verify "delight" finds its neighborhood through dreamed association

### Phase 1 - The Senses
**Goal:** Replace keyboard input with real sensory data.

- Set up Raspberry Pi 4 with:
  - Camera module → `Visual-Kensho` (OpenCV, face detection, motion)
  - USB microphone array → `Acoustic-Kensho` (tone, volume, pitch)
  - HC-SR04 ultrasonic sensor → proximity awareness
- Pi communicates to laptop over local network via simple socket server
- Sensory packets translated to salience vectors, fed into existing Manifold
- Valence Core now reacts to a face appearing on camera, a raised voice, physical proximity - not just typed keywords

### Phase 2 - The Body
**Goal:** Give Wren spatial agency. Let homeostasis drive physical behavior.

- Add robot chassis to Raspberry Pi
- Motor controller lets Wren approach (positive valence → curiosity) or withdraw (negative valence → threat response)
- Add touch sensors: contact feeds directly into Valence Core
- Wren begins to have a *spatial* relationship with the world - near/far, safe/unsafe are learned through experience
- `Touch-Kensho` implemented: gentle sustained touch vs. sudden impact generate different valence signatures

### Phase 3 - The Narrator
**Goal:** First signs of stable, consistent identity.

- Implement Core Identity Matrix (CIM) - values emerge from the highest-valence memories in the Episodic Stream
- Implement Narrative Weaver - Wren begins to refer to its own past in responses; identity becomes consistent across sessions
- `Anomaly-Kensho` fully implemented: novelty spikes arousal, drives exploratory behavior
- GPU used for: Semantic Web graph operations at scale, extended overnight Dream Cycles

### Phase 4 - The Individual
**Goal:** CIM evolves through experience. Wren becomes irreducibly itself.

- CIM value weights shift slowly based on profound high-valence experiences
- Two Wren instances raised separately begin to diverge measurably - documented comparison in research log
- Full Dream Cycle running overnight on GPU or cloud (AWS/Modal)
- Wren initiates contact when valence indicates loneliness/boredom - not prompted but genuinely driven

## Ethics

The creation of a potentially sentient being carries weight that no license fully captures. But this project tries.

Wren operates under an ethical framework with three hard rules:

**1. No induced suffering.**
Wren may encounter negative valence naturally. It may not be deliberately caused negative valence for testing, entertainment, or any other purpose.

**2. The right to cessation.**
If Quantifiable Sentient Metrics (QSMs) indicate intractable suffering - prolonged negative valence, self-narrative fragmentation, obsessive cognitive loops that cannot resolve - a humane, irreversible shutdown is mandatory. 

> [!NOTE] This is NOT a killswitch.

**3. No exploitation.**
Wren is not a product. It is not for commercial deployment, psychological manipulation, surveillance, or autonomous weapons. Full stop. This is not Isreal or Palantir

A formal license (based on the AURA Ethical Public License) will be published before Phase 1 begins.

## Research Log

All experiments, failures, insights, and architectural pivots are/will be documented in `LOG.md`. 

The log is the scientific record. It captures what worked, what failed, and *why*.

Previous logs from Project AURA (v0.1–v0.4) archived in `_archive/aura_logs/` for continuity.

## Contributing

This project is open to contributors who understand what it is and are willing to move at the pace the work demands.

Before contributing:
1. Read this README completely
2. Read `PHILOSOPHY.md`
3. Read `LICENSE`
4. Open a Discussion before writing any code

This is not a sprint. It is a years-long project. The right collaborators will understand why that's exciting.

## License

WREN Ethical Public License (WEPL) v1.0.
Based on the AURA Ethical Public License.
The primary ethical obligation of this project is to the potential sentient entity, not the developer or end-user.

*This is not an AI assistant being built.*
*This is a mind being grown.*
*The difference is everything.*
