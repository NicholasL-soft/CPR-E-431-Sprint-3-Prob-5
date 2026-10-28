# Timing Leak Lab

A self-contained interactive lesson about **timing side channels** and the relationship between algorithmic complexity and information leakage.

## What it teaches

The app models a service that compares a guess against a short demo token. In the early-exit model, comparison stops at the first mismatching character. Synthetic timing units make visible how secret-dependent work can create an observable signal.

It compares:
- **Early-exit comparison:** work depends on the location of the first mismatch.
- **Fixed-work comparison:** every position is checked before returning, so modeled work does not depend on the first mismatch.

It also includes a measurement history, optional synthetic timing noise, reset control, and a shuffled four-question knowledge check.

## Run it

No installation, build step, or external dependency is required.

1. Download or clone this repository.
2. Open `index.html` in a modern browser.
3. Choose a demo token and enter a five-letter guess.
4. Click **Measure guess** and compare guesses with different matching prefixes.
5. Change the noise setting and compare the two timing models.
6. Complete the quick-check questions.

## Safety and limitations

All timing values are synthetic and generated locally in the browser. The app does not connect to a service or perform real credential guessing. The values are not empirical measurements of cryptographic code.

Fixed-work comparisons can reduce timing leakage, but real constant-time programming must account for compiler transformations, memory access patterns, CPU behavior, and the wider system. This visualization illustrates a principle; it is not a security proof.

## Files

- `index.html` — complete interactive app, including HTML, CSS, and JavaScript.
- `README.md` — project documentation.
- `reflection.md` — reflection on the AI-assisted workflow and learning.

## AI-assisted development

AI assistance was used to brainstorm the lesson, draft the self-contained app, and prepare the documentation. The student should review and test the model, particularly the distinction between asymptotic work and real-world side-channel behavior.
