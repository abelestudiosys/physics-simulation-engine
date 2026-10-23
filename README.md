# AI Physics Reasoning Engine

**Resumen en español.** Agente de inteligencia artificial modular para la resolución y explicación de problemas de Física. Clasifica la complejidad de cada ejercicio, adapta la profundidad del razonamiento, valida la coherencia física y matemática de las soluciones y presenta los resultados en HTML y MathJax, con salida en PDF. Está desarrollado en Google AI Studio mediante instrucciones de sistema. Su arquitectura modular, organizada en 34 módulos numerados, está descrita en este repositorio.

## Overview

The AI Physics Reasoning Engine is a modular artificial intelligence system designed for structured interpretation, validation, and resolution of physics problems from basic to university-level complexity.

The project was developed to overcome a common limitation in automated problem solving: obtaining numerical answers without understanding the underlying physical reasoning.

Instead of performing only formula substitution, this engine follows a structured workflow that analyzes the physical phenomenon, identifies variables, selects appropriate models, validates mathematical and dimensional consistency, and generates professional educational outputs using HTML, MathJax, and PDF-compatible structures.

## Project Motivation

This system was created to explore how Artificial Intelligence can be combined with physics education through structured reasoning.

The main objective is to develop an AI-assisted framework capable of producing solutions that are not only mathematically correct, but also physically meaningful, pedagogically organized, and reusable across different physics domains.

## System Architecture

The engine is built on a 34-module hierarchical architecture organized into two main processing layers.

**What the 34 modules are.** The system instruction is organized into 34 numbered modules (sections 1–34 of the instruction file), on top of an identity definition (section 0). They are hierarchical and cumulative: the global reasoning layer always applies, the rules of each module are added and never replace one another, and conflicts are resolved with a fixed priority order (physical coherence, pedagogical integrity, structural stability, readability, visual aesthetics). The modules fall into these groups:

- Reasoning and classification (7 modules): global reasoning layer, exercise classification, physical resolution sequence, cognitive depth, automatic classification, decision rules, and the priority rule for uncertain cases.
- Validation and consistency (2 modules): unit, logic and physical-sense validation, and the consistency rule across modes.
- Adaptive modes (3 modules): COMPACT and ANALYTICAL modes, automatic mode selection, and automatic layout selection.
- Visual rendering (13 modules): HTML + MathJax presentation, global HTML structure, CSS rules, overflow and MathJax control, dynamic vertical expansion, visual quality checks, scalability, and continuity across exercises.
- PDF export (2 modules): print-oriented rules and advanced page-break control.
- Integration and governance (7 modules): modular inheritance, integration with the global system, the cognitive-to-visual transition protocol, the master rule, and the project result and status notes.

### Cognitive Layer — Physics Reasoning Engine

The cognitive layer is responsible for analyzing and validating the physics before any visual generation occurs.

Main capabilities:

- Automatic exercise classification (Level 1, Level 2, Level 3).
- Physical interpretation of the problem.
- Identification of variables, unknowns, and units.
- Selection and justification of physical models.
- Step-by-step mathematical development.
- Dimensional and physical consistency validation.

The system considers a solution complete only after passing the validation stage.

### Visual Layer — Dynamic Rendering Engine

After validation, the visual layer transforms the solution into a structured educational document.

Capabilities:

- Automatic rendering mode selection.
- HTML-based document generation.
- MathJax mathematical visualization.
- PDF-ready formatting.
- Anti-overflow control.
- Dynamic expansion for complex solutions.

The visual layer does not modify the validated reasoning process.

## Intelligent Resolution Pipeline

The system follows a strict processing workflow:

```text
Physics Problem
        ↓
Exercise Classification
        ↓
Physical Reasoning Engine
        ↓
Validation Process
        ↓
HTML + MathJax Rendering
        ↓
PDF Educational Output
```

Core principle:

**Analyze → Validate → Render**

## Adaptive Reasoning Modes

The engine automatically adjusts the depth of explanation according to problem complexity.

| Mode | Activation | Purpose |
|---|---|---|
| COMPACT | Basic direct calculations | Efficient and clear solutions |
| ANALYTICAL | Problems requiring interpretation | Deep conceptual reasoning |

When classification is uncertain, the system defaults to ANALYTICAL mode to avoid oversimplifying complex physical phenomena.

## Key Features

- AI-based structured physics reasoning.
- Automatic exercise complexity classification.
- Physical model selection and justification.
- Mathematical and dimensional validation.
- Adaptive explanation depth.
- HTML + MathJax rendering.
- PDF-compatible educational documents.
- Modular and scalable architecture.
- Separation between reasoning and presentation layers.

## Physics Domains Covered

The current architecture supports:

- Kinematics (MRU, MRUA, relative motion).
- Dynamics (Newton's Laws).
- Energy and Work.
- Gravitation.
- Oscillations and Waves.
- Basic Electricity.
- Basic Thermodynamics.

The modular design allows future expansion into additional scientific domains.

## Usage Workflow

The system is designed to operate through the following process:

1. Provide physics problem statements.
2. Apply the structured system instructions.
3. Execute classification and physical reasoning.
4. Validate mathematical and physical consistency.
5. Generate structured HTML and PDF educational output.

The generated documents are designed for learning, analysis, and technical review.

## Limitations

Current limitations include:

- The system depends on the capabilities of the underlying AI model.
- Highly ambiguous physics statements may require human interpretation.
- Generated solutions should always be reviewed in critical scientific contexts.
- The current implementation focuses mainly on general physics domains.

These limitations are considered part of the continuous improvement process.

## Future Development

Planned improvements include:

- Interactive physics simulations.
- Expansion into additional STEM disciplines.
- Comparison between multiple valid solution methods.
- Automated graphical analysis.
- Web-based user interface.
- Advanced validation modules.

The long-term vision is to evolve this architecture into a broader AI educational reasoning framework.

## Conflict Resolution Priority

When multiple rules interact, the system follows this hierarchy:

1. Physical coherence.
2. Pedagogical integrity.
3. Structural stability.
4. Readability.
5. Visual aesthetics.

## Project Files

| File | Description |
|---|---|
| `SYSTEM INSTRUCTION PHYSICS.md` | Complete 34-module architecture defining reasoning, validation, and rendering rules. |
| `SYSTEM INSTRUCTION FISICA.md` | Spanish-language version of the system instruction. |
| `auditoria de proyecto fisica.txt` | Example execution and validation results. |

## Technologies

- Google AI Studio.
- Structured System Instructions.
- AI Prompt Engineering.
- HTML / CSS.
- MathJax.
- PDF-oriented document generation.

## Author

Ramón Abel Franco López

Background in Systems Engineering (Universidad de Guayaquil). GitHub: [abelestudiosys](https://github.com/abelestudiosys)
