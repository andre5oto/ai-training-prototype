# Prototype Design for Legal Approval Flow

An interaction prototype about contract approvals that get stuck.

**Live:** https://andre5oto.github.io/ai-training-prototype/

Nothing here connects to a real system, no data is stored, and the Assistant's answers are
scripted rather than generated. It is a thinking exercise, not a product proposal.

## Try it

The contract opens on the blocked step.

1. Read why it is blocked in the Inspector on the right.
2. Ask the assistant **Why is this stuck?**
3. Click **Ask Legal Ops in Slack**, flag it urgent if you want, and post.
4. Legal picks it up from the channel and approves.

**Reset the session** in the Inspector header puts everything back to the start.

Turn on **Product notes** at the top of the approval chain. Every design decision gets a
short note explaining why it went that way. That is the part worth reading.

## The scenario

A $184,000 MSA renewal, 14 days in flight against a 9 day median.

A policy agent reviewed 41 clauses against the playbook. Twelve of them are required and
eleven are present. The DPA-02 subprocessor clause is missing from the counterparty's
redline. A missing required clause is not a deviation inside the fallback range, so the
agent did not approve it. It escalated to Legal.

The escalation was correct. The delay came after: the item sat unassigned in the Legal Ops
queue, which is a step in the process but not a step in the workflow. No owner, no enforced
SLA, and the time spent waiting there never appears in cycle time reporting.

## Built with

Claude Code as the collaborator. The scenario and the design decisions are mine.

## License

MIT.
