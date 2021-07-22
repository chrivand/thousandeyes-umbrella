# Umbrella and ThousandEyes integration (SASE)

The goal of the integration is to test whether the policies of Umbrella are being enforced. This verification is done by Cisco ThousandEyes (using instant HTTP tests). The Instant Test feature can be used to troubleshoot problems without waiting for a scheduled test, or to validate a new test's configuration. Before running the Instant Test, an existing test's configurations can be adjusted, such as adding new agents or increasing timeout values. Data can be saved for later review and shared with interested parties. 

## Features
* Searches for Group ID of agents to start instant test from;
* Creates HTTP instant endpoint test for agents (with earlier queried Group ID) to verify of domain is reachable;
* You can configure how often to rerun the test and the amount of time in between;
* Retrieves and parses test results automatically;
* If domain/URL is reachable it will send a Webex Teams notifaction to warn that policy is not enforced;
* Vice versa, if domain/URL is not reachable, it will send a confirmation via Webex Teams that policy is enforced.

## Business Case
This is important for multiple reasons. First of all, an analyst can check whether a potential harmfull destination is reachable, and thus can cause a threat (e.g. a Command&Control server). Second it can also be used to verify the policy enforcement across your organization. Cisco ThousandEyes can for example be used to verify a domain block in Cisco Umbrella, offering a good SASE use case. Obviously there are more use cases that this is usefull for.

Please continue your reading in this [white paper](https://www.cisco.com/c/en/us/products/security/what-is-sase-secure-access-service-edge.html?ccid=cc000158&dtid=odicdc000016).

## Related Sandbox
You can try this out using the [Cisco Umbrella sandbox](https://devnetsandbox.cisco.com/RM/Diagram/Index/1ce48361-eefc-4812-93d5-4915496a1176?diagramType=Topology)!

## List of SecureX Learning Labs
* Please try out [this SASE DevNet learning track](https://developer.cisco.com/learning/tracks/sase) to try this yourself. 
* Please also check out the [SASE microsite](https://developer.cisco.com/sase/) on DevNet!

## Solutions on Ecosystem Exchange
Please check out related solutions on [DevNet Ecosystem Exchange](https://developer.cisco.com/ecosystem/solutions/#key=sase).