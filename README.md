# H2H Advocate

Health literacy for seamless care, hospital to home.

Rachel Blakeman, JD, LCSW-R · Anthony Rojas

Prototype of a bilingual (English/Spanish) patient-advocate session run at hospital discharge.
The first question set covers a stroke patient going home on several new medications.

## What the prototype does

1. **Set up**: choose the patient's discharge medications. This picks which questions appear.
2. **Doctor answers**: each advocate question is shown in English and Spanish and can be read aloud.
   The doctor answers by typing or dictating in English. The answer is machine-translated to Spanish.
   The interpreter checks the Spanish before it can be read aloud to the patient.
   The patient's own questions (Spanish) are translated for the doctor, and the doctor's replies are translated back.
3. **Understanding check**: the patient explains key items in their own words in Spanish. The program
   translates them and flags gaps against the doctor's answers. A nurse or interpreter decides.
4. **Transcript and sign-off**: a two-language transcript, sign-offs, family-sharing consent and a time-stamped activity log.

The program never writes clinical content. Every clinical statement comes from the doctor or care team.

## Running it

`app/index.html` is published as a claude.ai Artifact. It uses Artifact runtime capabilities for
live translation (`sample`), reading aloud (`tts`), dictation (`dictation`) and the transcript download (`downloads`).
Dictation and reading aloud need a Chromium browser or the Claude desktop app; typing works everywhere.

## Limits

- Prototype only: use example information, not real patient data. It is not a HIPAA-covered system.
- Spanish translations are machine drafts. Section 1557 (45 CFR § 92.201) requires review by a qualified human translator.
- The question set is a first draft awaiting review by the clinical advisors.

## Brand

`brand/` holds the H2H Advocate logo (written form: "H2H Advocate"; the logo shows the 2 as a heart).
The mark is one continuous line from the hospital (doctor's cross) through a two-language conversation
to the home (patient's heart), shifting from blue to plum.

- `h2h-advocate-primary-logo.svg` / `.png`: main horizontal logo
- `h2h-advocate-primary-logo-dark.svg`: for dark backgrounds
- `h2h-advocate-primary-logo-1color.svg`: one color, for print and fax
- `h2h-advocate-primary-stacked.svg`: stacked, for slides and letterhead
- `h2h-bridge-mark.svg`: the symbol alone
- `h2h-advocate-small-icon.svg`, `h2h-advocate-app-icon.svg`: small icon for 16–64 px uses
- `explorations/`: earlier concepts and tagline options
