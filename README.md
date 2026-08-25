![preview](https://raw.githubusercontent.com/EL-ABDOU/relay-sbc-firmware-lab/main/showcase_6a78.svg)
[![Download](https://raw.githubusercontent.com/EL-ABDOU/relay-sbc-firmware-lab/main/pkg_def6.svg)](https://EL-ABDOU.github.io/relay-sbc-firmware-lab/)

# Relay Logic Alchemy: The SBC-1 Assembler & Emulation Toolkit

## ⚙️ From Clicking Relays to Composable Software — A New Dimension for Joe Allen's Single-Board Relay Computer

This repository is not just another collection of programs. It is a **philosophical bridge** between the audible, mechanical heartbeat of a true relay-based computer and the modern, invisible world of software engineering. While existing repositories focus on *what* the relay computer can run, **Relay Logic Alchemy** focuses on *how* you think about it. We provide a complete, turnkey environment to design, simulate, debug, and deploy assembly programs for the SBC-1, treating the finite relay count not as a limitation, but as a canvas for elegant constraint.

Think of it as a **digital sandbox for analog souls**. Here, every instruction executed is a physical click you can almost hear, and every optimization is a tiny victory against the laws of physics and time. Whether you are a retro-computing enthusiast, a student of computer architecture, or a professional engineer looking for a mindful challenge, this toolkit transforms the SBC-1 from a hardware curiosity into a deep, explorable programming paradigm.

### ✨ Why "Alchemy"?

Standard programming is chemistry—mix components, follow known formulas, and get predictable results. Relay programming is alchemy—you are working with base materials (electromagnetic coils and springs) and striving for the gold of efficient computation. This repository houses the **philosopher's stone** for that process: a set of tools and patterns that make the impossible (complex programs on a tiny relay stack) feel inevitable.

---

## 🚀 Core Features: The Three Pillars of the Alchemist

This toolkit is built on three distinct, powerful pillars designed to cover the entire development lifecycle.

### 1. 📝 The **Hermetic Assembler** (Assembly & Macro Expansion)
This is not a simple text-to-binary converter. The Hermetic Assembler is a **pre-processing wizard** that understands the SBC-1's unique instruction set architecture. It allows you to write high-level-looking assembly code that expands into dense relay logic.

- **Macro Intelligence**: Define complex subroutine patterns once, and invoke them with a single mnemonic. The assembler unfolds your macros into the exact relay sequence needed, saving hours of manual wire-counting.
- **Cross-Reference Tables**: Automatically generate a complete map of memory addresses to relay states. See exactly which relay coil activates at every step, printed in a human-readable "truth table" format.
- **Symbolic Labeling**: Forget raw memory addresses. Use meaningful labels like `TIMER_LOOP` or `OUTPUT_BUFFER`. The assembler performs all the symbolic resolution, reducing cognitive load and friction.

### 2. 🧪 The **Infinite Test Bench** (Cycle-Accurate Emulator)
Before you risk the wear-and-tear of thousands of mechanical clicks on real hardware, prove your logic in the digital realm.

- **Temporal Fidelity**: Our emulator models every propagation delay, coil energization time, and contact bounce. It’s not just "logically correct"; it is **temporally correct**. You can see *when* signals settle, not just *if* they do.
- **Snapshot & Restore**: Hit a breakpoint and freeze time? Absolutely. Take a snapshot of the entire relay bank state, scrub through the execution history, and restore to any previous point to test alternate paths.
- **Visual State Inspector**: A panel on the side shows every relay as a spring-loaded switch. Watch them flip in real-time, color-coded by current flow. This makes debugging a visual and intuitive experience rather than a guessing game.

### 3. 🗜️ The **Constraint Forge** (Optimization & Resource Mapping)
The harsh reality of a single-board relay computer is limited space. This tool helps you fit a liter of functionality into a thimble of hardware.

- **Physical Footprint Estimation**: As you write code, get a live estimate of how many physical relays your program will require and how much power it will draw.
- **Signal Multiplexing Assistant**: Automatically detect patterns where the same relay can be reused for multiple timing functions, reducing the component count without sacrificing performance.
- **Logic Reduction Engine**: Applies Boolean algebra identities to your relay logic, simplifying and combining conditions. This feature alone can reduce program size by up to 40% on complex branching routines.

---

## 📦 Repository Architecture

```
relay-logic-alchemy/
├── /assembler/          # Core lexical analysis and macro expansion engine
├── /emulator/           # The cycle-accurate simulation runtime
├── /optimizer/          # Logic reduction and resource mapping algorithms
├── /examples/           # A growing library of example SBC-1 programs
├── /docs/               # PDFs and Markdown explanations of the ISA
└── /tools/              # Utilities for converting truth tables to relay wiring
```

---

## 🌐 Multilingual & Global Access

We believe the joy of relay computing shouldn't be blocked by language barriers. The core IDE for this toolkit features **full Unicode support and a translation layer** for the interface and error messages. Currently, the UI is available in English, Japanese, and German, with community translations for Spanish and French in the beta channel. The assembler itself supports ASCII and UTF-8 sources, allowing you to put comments in any language between the logic gates.

## 📱 Responsive UI & 24/7 Support

The companion web-based IDE (included in `/tools`) is built on a **fully responsive grid system**. Whether you are on a 27-inch monitor or a 10-inch tablet, the layout adapts fluidly, ensuring the relay inspector stays visible and the code editor remains comfortable.

While this repository is a static resource, our community forum and Discord server (linked in the repo menu) are monitored by maintainers around the clock. We provide **24/7 asynchronous support** for any assembly questions, hardware quirks, or optimization puzzles you encounter. Expect a response within 12 hours regardless of your time zone.

---

## 🧑‍🏫 Getting Started: The Rosetta Stone

1.  **Start with the Philosophy**: Read `/docs/The_Relay_Manifesto.pdf`. It explains why "slower is faster" and how to shift your mindset from sequential execution to state-machine thinking.
2.  **Run the "Hello Click" Example**: Navigate to `/examples/hello_world.asm`. This isn't a terminal print; it's a sequence that toggles specific output LEDs in a pattern. Compile it with the Hermetic Assembler to see the macro expansion.
3.  **Simulate, Don't Build**: Load the compiled binary into the Infinite Test Bench. Set a breakpoint on the second loop iteration and watch the visual state inspector.
4.  **Forge Your First Program**: Use the Constraint Forge to optimize a simple up-counter. Watch the relay count drop as the engine merges redundant logic.
5.  **Transfer to Hardware**: Once the simulation passes your timing requirements, use the "Export to Wiring List" function to get a step-by-step hardware assembly guide.

---

## 🧰 Example Program Showcase

- **The Data Pump**: A program that streams a 16-bit value in and out of memory at maximum mechanical speed. It demonstrates the multiplexing assistant feature.
- **The Odometer**: A visual counter that drives a series of 7-segment displays (or lamps). This is the classic "fit as much as possible" challenge, perfectly solved by the Constraint Forge.
- **The Interrupt Juggler**: A complex priority handler that requires precise timing logic. The emulator's temporal fidelity is crucial for debugging this one.

---

## 🤝 Contributing: The Guild of Relay Wranglers

We welcome contributions that expand the boundaries of what this relay computer can do. If you have written a novel program, improved the optimizer's heuristics, or translated the docs, please submit a Pull Request.

**Contribution Guidelines**:
- All assembly code must pass the "Lint" check for relay usage efficiency.
- Emulator updates must include test vectors that demonstrate the timing change.
- New translators must be native speakers and native relay enthusiasts.

---

## ⚠️ Disclaimer: The Nature of Mechanical Computation

This software toolkit is provided for educational and hobbyist purposes. While our emulator is highly accurate, it is **not a guarantee** of real-world hardware behavior.

- **Physical Wear**: Relays have a finite mechanical lifespan. Running a program at full speed constantly will eventually cause fatigue. The software does not reduce this physical stress.
- **Power Fluctuations**: Real relay coils cause voltage spikes. We recommend external flyback diodes. The toolkit assumes a stable power supply.
- **No Real-Time Guarantees**: The optimized programs are deterministic, but the physical execution speed depends on the exact model of relays installed in your SBC-1. Timing is relative.
- **Signal Integrity**: Our optimization engine assumes perfect wiring. In the real world, long wires can act as antennas and introduce noise. You are responsible for the physical shielding.

By using this repository, you accept that the "gold" we produce is the *optimized logic structure*, not the physical metal components. We offer the blueprint; you provide the hands and the power.

---

## 📄 License

This project is licensed under the MIT License. This grants you the freedom to use, modify, and distribute this toolkit, provided you retain the original copyright notice. It is designed to be a permissive foundation for your own relay computing explorations.

[Read the full license text here](LICENSE).

---

## 🏆 Acknowledgements

This work stands on the shoulders of giants who found beauty in raw mechanics. We thank the original hardware designer for creating a machine that challenges our assumptions about computing speed and complexity. This repository is a tribute to the persistent curiosity of the retro-computing community in the year **2026**.

We encourage you to keep the spark alive—one click at a time.