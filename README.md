
# Algorithmic Complexity & Side-Channel Security Lab

## Overview

This is an interactive, browser-based cybersecurity learning project exploring algorithmic-complexity attacks, resource exhaustion, regular-expression denial of service (ReDoS), side-channel attacks, timing leakage, and speculative execution.

The project runs locally in a web browser and does not require a server or external JavaScript libraries.

## Features

### 1. Algorithmic Complexity
- Compare linear and quadratic algorithm growth.
- Adjust input size using a slider.
- View operation counts and visual bars that change as the input changes.

### 2. Hash-Table Denial of Service
- Adjust the number of colliding keys.
- Watch individual keys appear inside a conceptual hash bucket.
- Compare linked-list, balanced-tree, and open-addressing strategies.
- View estimated lookup work that changes with the selected strategy and number of keys.

### 3. ReDoS and Resource Exhaustion
- Explore several potentially expensive regular-expression patterns.
- Adjust the input length.
- View a changing branching-path illustration and conceptual risk indicator.
- Learn about decompression bombs and expensive parsing.

### 4. Side-Channel Attacks
- Explore timing, cache behavior, power consumption, electromagnetic emissions, acoustic signals, data remanence, optical observation, and differential fault analysis.
- Understand the difference between active and passive side-channel methods.

### 5. Timing and Spectre
- Run a simplified character-comparison timing demonstration.
- View the individual comparison steps.
- Explore square-and-multiply operation patterns.
- Learn how speculative execution and cache behavior can create information leakage.

### 6. Countermeasures
- Review safer algorithms, resource limits, constant-time routines, safer regular-expression engines, randomization, and monitoring.

### 7. Knowledge Check
- Complete six multiple-choice questions.
- Receive a score based on the answers.

## How to Run

1. Save the project files in the same folder.
2. Open `index.html` in a modern web browser.
3. Use the navigation bar to explore the seven sections.
4. Adjust the sliders and dropdowns to update the demonstrations.
5. Use the buttons in the timing and speculative-execution section to run the simulations.
6. Complete the knowledge check.

## Files

- `index.html` — The complete interactive application, including HTML, CSS, and JavaScript.
- `README.md` — Project overview and instructions.
- `reflection.md` — Reflection on the learning process, design choices, and limitations.

## Technical Details

The application uses standard HTML, CSS, and JavaScript. It does not require a build process, package installation, or internet connection.

## Safety and Limitations

The demonstrations use simplified conceptual models. They do not benchmark real attack performance, execute potentially expensive regular expressions, or perform actual secret recovery.

The hash-table lookup values are illustrative estimates. The ReDoS branching display is a conceptual visualization rather than a measurement of real regular-expression execution paths. The timing demonstration uses a fixed model rather than measuring real elapsed time.

Actual behavior depends on the programming language, runtime, algorithm, compiler, hardware, and deployment environment.

## Defensive Lessons

- Bound input sizes and computational work.
- Set appropriate memory, execution-time, and decompression limits.
- Select algorithms with suitable worst-case behavior.
- Avoid vulnerable regular-expression patterns when processing untrusted input.
- Use established cryptographic libraries and constant-time routines where appropriate.
- Test worst-case inputs and monitor resource usage.
