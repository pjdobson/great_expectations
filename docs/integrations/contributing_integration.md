---
title: How To Write Integration Documentation
---

### Introduction
As the data stack ecosystem grows and expands in usage and tooling, so does the need to integrate with 3rd party
products or services. [Superconductive](https://superconductive.com) as drivers and ushers
of [Great Expectations](https://greatexpectations.io), we want to make the process to integrating with Great Expectations
as low friction as possible. We are committed to work and iterate in the process and greatly value any feedback you may have.
The aim of this document is to provide guidance for vendors or community partners which wish to integrate with us as to
how to write documentation for said integration and to establish a sense of uniformity and consistency.

With all having been said, let's delve into actionable steps.

## Steps

### 0. Reach out to our Developer Relations team
Before you embark in this journey, drop by and introduce yourself in the #integrations channel in our [Great Expectations Slack](https://greatexpectationstalk.slack.com)
to let us know. We're big believers of building strong relationships with ecosystem partners. And thus we believe
opening communication channels early in the process is essential.

### 1. Copy the template
Create a copy of `integration_template.md` and name it `integration_<my_product>.md`. This file is located in `great_expectations/docs/integrations/` directory.
This file is in markdown format and support basic [docusaurus admonitions](https://docusaurus.io/docs/markdown-features/admonitions).

### 2. Add to index
In the same directory as above, there is a file named `index.md`. In it add an entry matching the pattern in place of the first entry.

:::info
(Optional) Live-test the document
Sometimes is easier to author a document while getting a full visual representation of it. To this end, you can locally install our documentation stack as follows:
1. Navigate to the top level directory you cloned (i.e. `great_expectations`).
2. Install `yarn` (via homebrew or other package manager)
3. Run `yarn` and wait for dependency setup to finish.
4. Run `yarn start`. This will open a browser window with the docs site.
5. The document you're authoring should be visible by expanding the left side nav bar 'Integrations' menu.
This document will refresh every time you make changes and save the file (assuming the `yarn` process is still running).
:::

### 3. Fill in the `info` admonition at the top of the template
This section is key and, in a sense, required to be populated for acceptance in our docs. It should provide, at a glance,
ownership, support and other important information.

Good fences make good neighbors. It's important to make clear to would-be users of the integration who created the
integration and who to turn to if they need help. Further, you should include where can we or users raise issues about the documentation itself.
While we don't have any prescriptive solution, directing users to a Slack channel or github repo you monitor
is a generally-accepted open source community best practice. It should be very clear who the driver and owner of this document is.
In other words, just because Great Expectations will host it in its documentation site, doesn't imply we will be the maintainers of it.


### 4. Introduction content
In this section, ideally, you will set expectations (no pun intended) with the user, what problem the integration is solving,
what use case it enables, and what the desired outcome is.

### 5. Technical background
In some cases, it is necessary to provide a detailed technical background about the integration as well as important
technical considerations as well as possible trade-offs and shortcomings with the integration.

### 6. Dev loops unlocked by integration
This should be a more direct, concise and less hand-wavy version of the introduction. It should also foreshadow the content
in Usages section.

### 7. Usages
This section will be where the substance and nitty-gritty of your documentation is written. You should put a lot of
technical emphasis in this section and making sure you stay focused in fleshing out and explaining users how this integration
facilitates or enables a dev loop or use case with relevant and replicatable examples (see template for suggested format and structure).

### 8. Further discussion
This section is comprised of four subsections (i.e. Things to consider, When things don't work, FAQs, Other Resources).
Things to consider is where you would describe to the user important considerations, caveats, trade-offs, extensibility, applicability, etc.
When things don't work, should at the very least point your users where to seek support. Ideally, however, you can provide some basic trouble-shooting.
FAQs as this subsection's namesake hints, here is where you will document common questions, issues and pitfalls (and answers thereto)  
Additional resources is optional, but here is where you would place links to external tutorials, videos, etc.

### 9. Before submitting PR
Once you believe your documentation is ready to be submitted for review and consideration, reach out to anyone in our
Developer Relations team in the #integrations channel in our [Great Expectations Slack](https://greatexpectationstalk.slack.com)
to let us know.

### 10. Getting assistance
If you have any questions about the format, structure, process or any non-Great Expectations-specific questions, use the channel mentioned above.
For any technical questions, feel free to post in #support channel or reach out directly to one of developer advocates
for expedited turn-around.