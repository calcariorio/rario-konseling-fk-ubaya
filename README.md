# Rario, Pre-Marital Counseling Simulation Software

<p align="center">
  <img src="https://img.shields.io/badge/status-demo-yellow" alt="status">
  <img src="https://img.shields.io/badge/stack-vanilla%20JS-blue" alt="stack">
  <img src="https://img.shields.io/badge/license-educational%20use-lightgrey" alt="license">
</p>

Rario is a browser-based simulator that lets medical students practice pre-marital genetic counseling through a structured patient conversation. The training case centers on Rhesus incompatibility, and the interaction follows the G-I-PD-D partnership model: Greeting, Invite, Diagnosis Delivery, and Discuss & Management.

**[Live demo](#)** *(link to be added once GitHub Pages is active)*

## How it works

The student takes on the role of the physician and works through a consultation with a simulated patient. Rather than calling an external AI model, patient responses come from a rule-based dialogue engine written in plain JavaScript. It tracks where the conversation is heading and matches what the student says against expected clinical and empathetic cues at each stage. Everything runs client-side, so no server or API key is required to use it.

Each session is capped at 25 minutes, similar to an OSCE station. Once the student ends the session, the app scores it against two rubrics: communication (greeting, history-taking, diagnosis delivery, and management planning) and empathy (active listening, perspective-taking, emotional responsiveness, and expressed support). Instructors can review aggregated scores through a password-protected dashboard.

## Technical notes

This is a single self-contained HTML file with no build tooling and no framework dependencies. It opens directly in any modern browser. In a real classroom deployment, score records are sent to a Google Sheet through a small Google Apps Script backend, which keeps the setup free and serverless.

## About this build

This repository holds a portfolio version of the project. The backend credentials that would normally connect it to a live Google Sheet have been stripped out, so the instructor dashboard here only shows whatever scores were generated locally in your own browser. No classroom data is reachable from this deployment.

## Background

This project was built as a clinical communication training tool for the Faculty of Medicine at Universitas Surabaya (Ubaya). The dialogue script and grading rubric follow partnership-based communication and shared decision-making principles as applied to pre-marital genetic counseling.

---

<p align="center"><i>Built with the assistance of Claude (Anthropic)</i></p>
