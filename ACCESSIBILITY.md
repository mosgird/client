# Accessibility

Mosgird clients are meant to be usable by everyone, including people who use a keyboard only, a screen reader, a switch device, magnification or text scaling, and people who need reduced motion or high contrast.

## Target

We aim to meet WCAG 2.2 Level AA for every client's user interface. This is a target, not a claim. A client does not claim conformance until it has been tested against the criteria, and the results are published with the release.

## What the client is built to do

- Every control can be reached and operated with a keyboard, with a visible focus indicator and a logical focus order.
- Every control has an accessible name, role, and state, exposed to the platform's accessibility interface.
- Information is never conveyed by color alone.
- Text scales to at least 200% without losing content or function.
- Motion can be reduced, and nothing flashes more than three times per second.
- Errors are announced to assistive technology and explained in text.
- Text and interface components meet the WCAG AA contrast ratios.
- Images, audio, and video shipped with the app have text alternatives. Assets are made by people, not AI tools (see [AI_POLICY.md](AI_POLICY.md) in mosgird/protocols).

## Testing

Each release is tested with the platform's screen reader and with keyboard-only use. Automated checks are a first step, not a replacement for those tests.

## Reporting an accessibility problem

Open an issue and add the `accessibility` label. Describe the platform, the assistive technology you used, and the steps that failed. An accessibility problem is not a security problem; report security problems as described in [SECURITY.md](SECURITY.md).

## Status

No user interface exists yet. This document states intent for the client. It does not describe current behavior.
