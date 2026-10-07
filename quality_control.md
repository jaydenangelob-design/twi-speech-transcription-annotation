# Transcription Quality Control

## Purpose

This document defines quality-control checks for Twi speech transcription and annotation.

The goal is to identify transcription errors before annotated data is submitted for AI training or evaluation.

## 1. Accuracy Check

Review the transcript against the original audio.

Check for:

- Missing words
- Added words
- Incorrect words
- Incorrect spelling
- Misheard speech
- Incorrect speaker attribution

## 2. Speaker Check

Verify that every spoken segment is assigned to the correct speaker.

Check that:

- Speaker labels are consistent.
- Speaker changes are correctly identified.
- No speaker turns are accidentally combined.

## 3. Code-Switching Check

Review mixed Twi-English speech.

Check that:

- English words spoken by the speaker are preserved.
- Twi words are not incorrectly translated.
- Code-switching is consistently labeled.

## 4. Unclear Audio Check

If speech cannot be confidently understood, use:

`[UNCLEAR]`

Do not guess missing words.

This reduces the risk of introducing incorrect information into the dataset.

## 5. Timestamp Check

When timestamps are required:

- Use the correct format.
- Keep timestamps in chronological order.
- Make sure timestamps correspond reasonably to the spoken segment.

## 6. Consistency Check

Apply the same annotation rules across all samples.

Review:

- Speaker labels
- Language labels
- Code-switch labels
- Confidence levels
- Unclear speech markers

## 7. Final Review Checklist

Before submitting a transcript, confirm:

- [ ] Transcript matches the audio.
- [ ] Speaker labels are correct.
- [ ] Code-switching is preserved.
- [ ] Unclear sections are marked.
- [ ] Timestamps are correctly formatted.
- [ ] No information was invented.
- [ ] Annotation rules were applied consistently.

## Quality Principle

When uncertain, mark the uncertainty rather than guessing.

Accurate and consistent annotation is more valuable than artificially complete data.
