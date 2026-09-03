# Scope of Technical Discussion

[中文](README.md) | **English**

Companion to Initiative Draft v0.1. This directory records questions for discussion. It is not a protocol, a standard, or a description of existing product capabilities. The details below help clarify feasibility; they are not additional requirements beyond the minimum requests in the main text. Providers can explain coverage of updates, deletions, attachments, and other complex cases, with discussion proceeding in stages.

## Minimum capabilities and implementation choices left open

| Request | Questions to explain | Not prescribed in this version |
| --- | --- | --- |
| User authorization and read-only access | Who authorizes access, what it covers, and how to revoke it | A particular authentication protocol |
| Pagination | How to continue, when traversal ends, and whether data changes affect traversal | Page sizes and endpoints |
| Stable incremental positioning | How to recover, deduplicate, identify updates, and rebuild after a cursor becomes invalid | Cursor encoding and uniform JSON |
| Coverage documentation | Coverage of messages, task status, visible tool results, attachments, and artifacts | A uniform internal data model |
| Operating rules | Rate limits, retries, retention periods, and change notifications | Fixed queries per second or real-time commitments |

“Stable” does not mean a cursor never expires; expiration conditions and recovery paths need to be understandable. “Read-only” describes access capabilities, not the inherent trustworthiness of a receiving tool.

## Questions for further discussion

- How can stable identifiers and update timestamps support repeatable reads without creating duplicate records on retry?
- When records are added, edited, or deleted during pagination through a long history, how should consistency limits be reported?
- How can deletion notifications coexist with not retaining deleted content? Which historical changes cannot be retrieved retrospectively?
- How can necessary relationships be preserved for branches, message edits, task artifacts, and expired attachment links?
- Who is responsible for managing downloaded copies after the user revokes authorization?
- How should tools distinguish between data not provided, expired data, lack of permission, and temporary failures?

Provider-native formats with user-side adapters are acceptable. Reliability and cost can be discussed in stages. This version does not provide fabricated API examples or claim that a particular provider already supports these capabilities.
