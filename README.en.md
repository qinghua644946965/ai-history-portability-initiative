# Portable Access to AI Conversation and Task Data

[中文](README.md) | **English**

**Initiative Draft v0.1 · A user initiative / Open discussion draft**

**Ownership · Portability · Interoperability**

## 1. Reported experiences: more than an answer to recover

This initiative comes from a practical need expressed by a user of multiple AI services: to continuously retrieve conversations and task records scattered across products into a data hub under the user's control, then make them available to different models as needed. Different AI systems can help with retrieval, analysis, critique, and implementation, without the user repeatedly moving and explaining earlier thinking.

Two specific experiences reported by the initiator provide starting points. One concerns searching for “表格” (the Chinese word for “table”) in Codex, with reported differences in search results under different operations or history-loading states. **Evidence and verification are still pending for this case.** This draft does not confirm result counts or attribute any difference to searching only loaded content, index coverage, or another internal mechanism. The other concerns trying to recover an earlier discussion about “FLV 无声音” (“FLV has no sound”). **Original evidence is also pending for this case.** This draft does not confirm the date, client version, search steps, or final outcome.

These are accounts reported by a user, not independently reproduced product defects. They do not establish that data was lost or that a provider deliberately obstructed access. The question they raise remains worth discussing: if records exist and the user is entitled to access them, can the user save and index those records independently, and reliably return to the original context later? See the [evidence register](evidence/README.en.md) for evidence status and what still needs to be collected.

## 2. The problem: records kept on a platform are not necessarily usable over the long term

AI conversations often contain more than final answers. They also record how a question was clarified, why an option was rejected, how constraints changed, and how a task was ultimately completed. Copying only the conclusion may lose the conditions under which a judgment was made. Keeping only a summary can make it difficult to revisit omissions and misunderstandings.

When records are scattered across platforms, users need to remember where a discussion happened, its conversation title, and useful keywords. Search within a platform can help users find records again, but they may still want to search across platforms, archive by project, or ask another model to reanalyze their history. Even excellent search on one platform does not eliminate the need to organize data independently.

This initiative concerns whether users can continuously retrieve conversation and task data they are entitled to access and decide how to use it afterward. Personal knowledge bases and collaboration among multiple models are possible uses. Users who simply want readable, searchable records should also have practical options.

## 3. Why a one-time export is not enough

A one-time export is valuable for backup, migration, and archiving. The difficulty is that ongoing AI use keeps generating new records and may also change existing content. If every update requires requesting, downloading, and unpacking a complete archive, then comparing the differences manually, maintaining an archive becomes repetitive work.

A full snapshot answers “What did I retrieve this time?” Continuous synchronization also needs to answer “What has been added or changed since last time?”, “Where can I resume after an interruption?”, and “What falls outside the returned data?” Without stable resume points and a clear description of coverage, user-side tools struggle to identify duplicates, omissions, and whether synchronization is complete.

We therefore call for data access suited to ongoing use alongside existing export options. It need not be real-time or promise unlimited throughput; reasonable delays and rate limits are acceptable. Those limits should be public and understandable so users can schedule their next synchronization instead of continually moving records by hand. This is a statement of desired capabilities, not a blanket claim about the features of all existing products.

## 4. Minimum requests: a stable, ongoing way to retrieve data

We encourage AI service providers to progressively offer these minimum capabilities:

1. **User authorization.** Users can explicitly choose the scope of access and the receiving tool, and revoke future access. Authorization should be understandable. Retrieving records should not be treated as consent to unrestricted secondary use.
2. **Read-only access.** Users or their authorized tools can programmatically read conversation and task records the user is entitled to access. Coverage should include visible content, necessary metadata, and relationships between records needed to understand the interaction. Support for attachments, artifacts, and visible tool results, as well as gaps in that support, should be clearly described.
3. **Pagination.** Long histories can be read in batches, with explicit continuation or completion markers so a single response is not mistaken for the entire history.
4. **Stable incremental positioning.** Cursors, checkpoints, or equivalent capabilities allow synchronization to resume, retry, and identify changes. Providers should explain whether updates and deletion markers are included, and how to recover when a saved position becomes invalid.
5. **Understandable operating rules.** Providers document data coverage, formats, identifier rules, retention periods, rate limits, and error handling, and explain how incompatible changes will be communicated.

These requests describe outcomes users need, without prescribing endpoint names or uniform fields. Providers can start with read-only access to a limited scope, while honestly describing gaps. Providers choose their internal implementation; user-side tools handle adaptation, indexing, and organization.

## 5. Explicit boundaries: keeping the minimum requests practical

This is **Initiative Draft v0.1**, not a white paper, protocol standard, certification specification, or established industry consensus. It does not require uniform internal schemas, databases, Memory systems, knowledge graphs, or agent architectures. Nor does it require real-time delivery, webhooks, a uniform polling frequency, or fixed performance targets.

Access is limited to data the user is already entitled to access. It excludes model weights, hidden reasoning, internal system prompts, trade secrets, and other users' private content. Records involving multiple participants and third-party materials remain subject to their respective permission boundaries. Providing a way to retrieve data does not mean providers must build users' knowledge bases or permanently retain deleted content.

Users who control their data also need to manage the authorization, storage, and onward sharing practices of receiving tools. Revoking authorization on a platform can prevent future reads, but should not be described as automatically deleting every downloaded copy. Receiving tools should clearly explain how they manage those copies.

This document proposes product principles and user requests; it makes no legal determination for a particular jurisdiction. Data portability may reduce switching costs and may create tension with incentives to retain users on a platform. These are inferences for discussion, not grounds for concluding that a particular provider deliberately locks users in or breaks the law.

## 6. Principles and closing

**Ownership** means users have meaningful control over interaction histories they are entitled to access; it does not make a blanket claim about intellectual property ownership of every record. **Portability** means users can continuously bring records to systems of their choice. **Interoperability** means users can authorize different tools and models to use those histories without waiting for every platform to adopt the same internal structure.

We want users to choose platforms for the value of their products. Users may stay with one service for years or let multiple AI services collaborate. A way to retrieve their data makes both choices easier. Model capabilities will keep changing; continuity in thought and work should remain in users' hands.

**AI can change. Users' cognitive histories should not be lost when they switch platforms.**

**Data stays with the user. Intelligence competes above it.**

We welcome verifiable cases with sensitive information removed, and invite providers and developers to discuss costs, limitations, and feasible approaches. We begin with a limited request: enable users to continuously retrieve their AI conversation and task data through authorized, read-only access with pagination and stable incremental positioning.
