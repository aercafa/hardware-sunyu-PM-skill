# File and Version Governance

## Purpose

Keep repeated iterations understandable without destroying traceability. File governance should reduce confusion, not produce a second bureaucracy.

## Mandatory Safety Boundary

Reading, listing, comparing, and diagnosing files are non-destructive and may proceed automatically.

The following actions require a progress report and explicit operation-specific approval:

- deletion;
- moving files;
- renaming files or folders;
- archiving files;
- merging or splitting folders;
- changing folder structure;
- bulk replacement that obscures prior content.

Before requesting approval, show:

1. why the operation is needed;
2. each affected path;
3. current status and validation state;
4. proposed before-and-after structure;
5. links, references, or baselines affected;
6. recovery or rollback method;
7. operations that will not be performed.

Do not interpret “organize,” “clean up,” “handle old files,” or similar language as authorization.

Approval applies only to the listed actions in the current invocation. After execution, report the actual changes and any deviation.

## File States

Use only four states.

### Draft

Work in progress. Not a valid downstream dependency unless explicitly accepted as an assumption.

### Current

The single effective version for the present stage or product configuration.

### Archived

Superseded or historical, but retained for traceability, learning, or contractual reasons.

### Cleanup Candidate

Duplicate, temporary, orphaned, or no longer useful. Keep it until the user explicitly approves deletion.

## Validation State

Track validation separately from file state.

### Unverified

Not yet formally reviewed or tested.

### Reviewed

Reviewed and accepted for the stated purpose.

### Tested

Claims or outputs have supporting test evidence.

A Current file may be Unverified. An Archived file may still be Tested. Never use “latest” as a substitute for either dimension.

## Recommended Metadata

For formal Markdown source files, include:

| Field | Meaning |
| --- | --- |
| Artifact | Human-readable artifact name |
| Version | Semantic document version |
| File state | Draft / Current / Archived / Cleanup Candidate |
| Validation | Unverified / Reviewed / Tested |
| Owner | Accountable maintainer |
| Source baseline | Inputs or previous version |
| Replaces | Superseded artifact, if any |
| Last updated | ISO date |
| Change summary | Why this version exists |

For binary or derived files, keep the same metadata in the project control index.

## Version Rules

Use `Vmajor.minor`:

- `V0.x`: exploratory draft;
- `V1.0`: first reviewed baseline for its purpose;
- minor increment: clarification or compatible refinement;
- major increment: changed scope, architecture, interfaces, product definition, or incompatible meaning.

Do not use names such as `final-final`, `latest2`, or `new`.

Use dates for meeting records, test runs, and snapshots. Do not add dates to every canonical filename unless the project requires it.

## Source and Derived Files

Treat editable source as the authority.

Examples:

- Markdown is the source; HTML and PDF are derived.
- CAD source is the authority; rendered image is derived.
- Spreadsheet is the source; screenshot is derived.

Derived files should identify:

- source artifact;
- source version;
- generation or export date;
- whether manual edits were made after export.

If a derived file is manually edited, it must no longer silently claim synchronization with the source.

## Incremental Iteration

Before editing a formal artifact:

1. identify the Current version;
2. identify its validation state;
3. state whether the change is compatible or baseline-changing;
4. preserve user changes;
5. update version and change summary;
6. propose the previous version as Archived only after the new version is accepted, then obtain explicit approval before changing its state or location;
7. update the project control index.

Do not archive the old version merely because a new Draft exists.

Changing a file's metadata state to `Archived` changes the effective baseline relationship and therefore requires explicit approval. Moving it into an archive folder is a separate file operation and must be listed separately in the approval request.

## Suggested Stage Folders

Propose, do not silently impose:

```text
00_control/
01_opportunity/
02_research/
03_definition/
04_design/
  engineering-modules/
  standard-products/
05_engineering/
06_prototype/
07_pilot/
08_manuals/
09_closeout/
archive/
```

Adapt names to the existing repository. Creating or changing this structure requires explicit approval.

## Naming Pattern

Prefer:

`Project_Artifact_Vmajor.minor.ext`

For product variants:

`Family_Model_Artifact_Vmajor.minor.ext`

For engineering modules:

`ModuleName_Interface-or-Spec_Vmajor.minor.ext`

Keep status and validation in metadata or the control index rather than making filenames excessively long.

## Routine Audit

At stage gates and after several iterations, inspect for:

- multiple files claiming to be Current;
- newer but unverified files replacing tested baselines;
- broken links;
- derived files out of sync with sources;
- duplicate artifacts under different names;
- references to archived requirements;
- orphaned outputs;
- historical material mixed into current folders;
- cleanup candidates.

Report findings before proposing any mutation.

## Cleanup Proposal Format

| Path | Current state | Reason | Proposed action | Baseline impact | Recovery |
| --- | --- | --- | --- | --- | --- |

End with a precise approval request. Example:

“Approve only the three listed moves and two deletions?”

Do not execute a partial or expanded interpretation of the approval.
