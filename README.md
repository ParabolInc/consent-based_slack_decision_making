# Parabol's Consent-based Slack Decision-Making Workflow

## Installation

1. Open Slack
2. Click on the dropdown in the upper-left
3. Select `Workflow Builder`
4. Click `Import` and upload the workflow file

## Usage

It's recommended you add the workflow to a channel named `#decisions` or `#governance`.
When the workflow is active, it will communicate with the user on their `Slackbot` channel,
starting by asking the user to give a link to a proposal for a decision to be made.

When a decision has been made—assuming there are no objections—it's up to the proposer to
add the decision to an appropirate knowledge base (e.g. a product like
[Guru](https://getguru.com), [Confluence](https://youtu.be/vGQY95IZpLo),
[Notion](https://notion.so), etc. So that the decision is easily documented, searchable and
discoverable by team mates in the future.

### Video

For a video explanation of how this work flow works,
[watch this video](https://youtu.be/vGQY95IZpLo)

## Technical notes

This workflow also emits newline-delimited data on a private channel (in our instance,
`governance_zapier`) for easy integration with [Zapier](https://zapier.com).  This
allows us to set up automations around the creation, progress, and completion of
consent decisions.

Data is formatted as:


```
thread_location_parameters
written_proposal_url
author_name
proposal_channel
proposal_title
consent_decision_round
```

For example:

```
channel_id=C3X4KU0NM&ts=1633394616.041500
https://docs.google.com/document/d/18s_o3Jx5ML61sd5FVyLlHxwYL2-B8Tfc9C9Fr1Qakh0/edit#
@jrhusney
#t_exco_gov
2021 Q4 Strategy
Clarifying Questions
```



## Change Log

See the repository's [CHANGELOG.md](./CHANGELOG.md).

## Contributing

Please hit us up with Issues to ask questions, bugs, enhancements, or Pull Requests if you
make improvements to this workflow

© 2020 Parabol, Inc
