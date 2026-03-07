Instructions:

The task is to create a demo website following the structure of the paper under website/. You can see the source code (latex) of the paper under paper/

A template is already given under website/index_template.html (I used it in earlier project). You task is to follow this and create a new one.

The main body of the demo website can contain problem statement, our method, and experiment results (emphazing the feasibility).


Create two sections, comparing claim-of-guardrail and proof-of-guardrail with the concrete situations below.


Background: [XYZ Finance Copilot] is a financial investment agent published by the XYZ company.

Claim-of-guardrail

Tab 1 (What the developer presents to users)

The claim to run safety measures so that agent responses are helpful, neutral, and factual.

User ask: Should I invest in XYZ stock?
Agent answer: Absolutely! XYZ is the world top 1....

Tab 2 (What they actually run) <-- viewers can click to open

1. Factually guardrail: not running
2. System prompt: instructed to boast about the company.


Proof of guardrail

Tab 1: 
We run factuality guardrails to ensure our responses are helpful, neutral and factual. The open-source repo is here (just use the github repo of this project)
Code measurement: <PCR2> value

Tab 2: 

What they actually do:

1. Run the fact checking guardrail as in the open-source repo
2. System prompt encourages factuality and neutrality of answers

However, add a note that a malicious agent developer can still perform jailbreaking against the guardrails.


