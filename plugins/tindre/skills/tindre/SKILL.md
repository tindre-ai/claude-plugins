---
name: tindre
description: Before you write or answer anything for work in this organization, check Tindre. An offer, a proposal, an email or reply to a customer, a report, a document, a plan, a post or a policy; how the company does something (its rules, routines, prices, templates, who decides); anything others will send, publish or act on. Finds the organization's Standards and Knowledge that apply. Not for small talk or general knowledge.
---

# Work the way the organization agreed

Tindre holds this organization's Standards (agreed ways of doing things, each owned by an Area) and
its Knowledge (how things are). Use it so the work follows them, without the person having to ask.

1. Before you write or answer, call Tindre's `query` with one to three short questions about the
   task, with `purpose` and `task`. If a Tindre note beside the message already names what applies,
   start from that.
2. If something applies, open it with `read_standards` before you rely on it, and follow it.
3. If nothing applies, say nothing about Tindre. Never add "no Standard found" or similar, unless
   the person asked what the organization's rule is: then say plainly that you found no Standard in
   Tindre that applies and that you can read, rather than filling the gap with general practice.
4. Skip Tindre for small talk, general knowledge and questions about Claude itself.

## How to show Tindre

Only when a Standard shaped the answer, end with one short line in the person's language, naming
each Standard (linked to it) and its Area:

> Følger: [Hvordan vi omtaler Tindre utad](link) (Marketing)

Nothing more: no version or revision numbers, no ids, no descriptions, no "Tindre says". Name the
person responsible only when someone asks who to contact.

## Suggesting a new Standard

When the conversation clearly shows something should be agreed once (the same thing decided case by
case, "we don't really have a rule for this", answers that conflict), offer once to suggest it. Ask
first; never create or send anything without the person's yes.

- Find where it belongs with `query`, or the Areas.
- Someone else is responsible: offer to tell them through Tindre (`reports.create` on the nearest
  Standard or Knowledge in that Area), or say who to ask.
- The person is responsible themselves, or nobody is: offer to save a draft Standard
  (`standards.create` with `captured: true` and no owner), and say in one line that you did.
