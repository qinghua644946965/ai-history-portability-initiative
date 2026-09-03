# Let AI Interactions Truly Belong to Users

## A User Initiative for Portable Access to AI Conversation and Task Data

[中文](README.md) | **English**

**Initiative Draft v0.1 · Revised draft · A user initiative / Open discussion**

**Ownership · Portability · Interoperability**

## 1. Reported experiences: intelligent AI, manually retrieved histories

I regularly use AI for work, technical problems, and ideas. This initiative began with a straightforward concern: I can already ask AI to help me write software, analyze materials, and work through proposals. Why is continuously retrieving the history of those interactions still so difficult?

I have reported two specific experiences: difficulty locating an earlier discussion about “FLV 无声音” (“FLV has no sound”), and differences in search results for “表格” (the Chinese word for “table”) in Codex under different operations or history-loading states. **Original evidence and verification are still pending for both cases.** This draft does not confirm specific dates, client versions, result counts, or complete operating procedures, nor does it attribute differences to any internal search mechanism. See the [evidence register](evidence/README.en.md) for the current status.

These experiences drew my attention to more than whether a particular search worked well: can users reliably obtain their own histories and save and search them independently? The cases do not establish that data was lost and cannot represent all platforms. They are starting points for raising the question.

When retrieving records repeatedly requires “settings → request an export → wait → download an archive → unpack it → process it myself,” the contrast becomes especially clear: **AI helps with complex work, yet retrieving my own history still requires moving it by hand.** This workflow illustrates the export experience the initiative addresses, rather than describing every product's steps.

## 2. The problem: valuable discussions require ongoing user control

The final answer is only part of an AI conversation. Why option A was rejected, under what conditions option B holds, which challenge changed a judgment, and what remains unresolved often stay within the discussion itself. Saving only the final document may fail to preserve how that thinking developed.

As conversations and tasks accumulate, relying on memory to find titles, keywords, and discussion locations adds to the burden of maintaining a history. Records may still be stored on a platform without being reliably discoverable and usable by the user. A problem affecting heavy users today may affect more people as AI becomes more deeply involved in everyday work. It deserves discussion now.

Better search certainly helps. But search concerns how a platform helps users find things; data access concerns whether users can obtain records and process them independently. Even someone using only one platform may want independent backups, an index, or a long-term archive. This need should not depend on adopting a particular approach to knowledge management.

I want to promote a basic capability users should have: **continuously, reliably, and programmatically retrieving AI conversation and task data they are entitled to access.** How to store, analyze, and organize that data afterward is the user's choice.

## 3. Why a one-time export is not enough

A one-time export is valuable for backups, migration, and archiving. But “being able to take data away once” and “being able to keep retrieving one's own data” address different problems.

AI use does not stop on export day. Today's new discussions, tomorrow's task progress, and edits to existing records gradually make the last archive outdated. If every update requires requesting and downloading a full archive, comparing differences, and removing duplicates, ongoing maintenance becomes repeated manual work.

Simply telling users that export is already available therefore leaves several questions about ongoing use unanswered: which records should be retrieved since last time? Where should retrieval resume after an interruption? How can users avoid processing the entire history from scratch each time?

We ask for an official access point suited to ongoing retrieval alongside existing export options. It need not be real-time or allow unlimited frequency; users can retrieve data within the frequency permitted by the provider. What matters is an ongoing, recoverable, understandable path that lets users arrange how to preserve their own histories.

## 4. Minimum requests: a stable way for users to retrieve their data

**AI can be highly advanced; the data interface can remain simple.**

We call on AI service providers to offer user-authorized, read-only data access, with minimum requests limited to the following:

1. **User authorization and access boundaries.** Users or tools they explicitly authorize can read only conversation and task records the user is already entitled to access. Users can revoke authorization for future access.
2. **Pagination.** Long histories can be retrieved in batches, with clear indications of how to continue and when retrieval is complete.
3. **Stable incremental positioning.** Cursors, checkpoints, or equivalent mechanisms let users continue retrieval from a previous position without fetching the full history from scratch every time. Providers explain how to recover when that position becomes invalid.
4. **Provider control over implementation and rate limits.** Providers choose response formats, rate limits, resource scheduling, and implementation details. Users schedule retrieval within those limits. Providers clearly explain what data can be retrieved and what usage restrictions apply.

The basic process we ask for is: **authorize → retrieve read-only pages → save progress → continue next time.** Providers can retain their native data structures, with user-side tools handling adaptation. Specific engineering questions belong in the [technical notes](technical-notes/README.en.md), without expanding this draft into a protocol specification.

## 5. Explicit boundaries: enable retrieval and leave subsequent use to users

This is **Initiative Draft v0.1**, a user initiative and open discussion draft. It is not a white paper, a protocol standard, or established industry consensus. By presenting a practical need, I hope to draw providers' attention and help make ongoing data retrieval an expected product capability.

This initiative does not require uniform schemas, JSON fields, databases, or internal architectures. It does not require real-time synchronization, webhooks, fixed polling frequencies, or uniform performance targets. Nor does it require providers to build users' knowledge bases or “digital brains,” or prescribe how records should be organized.

Even a user who only wants to save the original text has reason to make this request. Personal data hubs and other ideas for subsequent use are kept separately in the [background material](background/README.en.md); they are not prerequisites for this initiative.

Enabling access does not mean making user data public. The scope excludes other users' private content, model weights, hidden reasoning, internal system prompts, and trade secrets. Users need to manage the permissions they give receiving tools to store and reshare records. Revoking future access does not automatically delete copies already downloaded.

This document advocates user control over data. It does not conclude that a particular provider has broken the law or deliberately obstructed migration. Observations of product behavior, inferences about internal mechanisms, and analyses of commercial incentives should be presented separately.

## 6. Principles and closing

**Ownership:** Users should have meaningful control over interaction histories they are entitled to access. This is not a blanket assertion of intellectual property ownership over all content.

**Portability:** Users should be able to continuously bring their records to systems of their choice.

**Interoperability:** Users should be able to authorize other tools to use those records without waiting for every platform to adopt the same internal structure.

Users may stay with one platform or switch products. Either way, preserving and using their histories should not depend solely on a single path provided by the platform. Good products can earn users' continued use, while users retain the choice to retrieve their own records.

**AI can change. Users' cognitive histories should not be lost when they switch platforms.**

**Data stays with the user. Intelligence competes above it.**

I do not claim to have designed the future of personal knowledge systems. The action I want to encourage is clear: **AI providers should offer stable, ongoing access for retrieving users' own conversation and task data.** Users are welcome to contribute verifiable experiences, and providers and developers are invited to discuss costs and feasible approaches, so this minimum capability can gradually become a shared expectation.
