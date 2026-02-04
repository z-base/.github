A decentralized web is not achieved by changing how we store and move bytes.

It is achieved by changing where authority is allowed to exist.

Treating DNS, HTTPS, or other discovery models and transport protocols as the root problem is a category error.

They move symbols.

They do not define meaning, ownership, or truth.


The real failure of Web2 is that identity, data, validation, and policy are bound to the same service boundary.

Who you are, what exists, and what is true are all decided by whoever runs the server.


This is the architectural sin.


True decentralization begins when every end-user device is an Actor,

a cryptographic authority over its own state,

and coordination emerges from verifiable claims, ignorant of network location.

The constraint is not how bytes are stored and moved.

The constraint is where meaning is allowed to form.

In my project **z-base**,

I will keep the existing discovery and transport stack.

I will let DNS, HTTPS, CDNs, and relays do what they are good at: moving encrypted blobs.


And I will relocate the only thing that matters:


Truth, identity, and authorization live exclusively in the Actor layer.

My system therefore decouples:

- identity from storage
- existence from service operators
- verification from data disclosure
- discovery from control

No service owns your identity.

No server defines your reality.

No transport layer grants authority.

Instead, it will:

- Host identity you control
- Store encrypted potential for your digital reality to be formed
- Blindly relay intentions between peers, which peers verify themselves

<img src="https://github.com/z-base/z-base/blob/main/docs/neutral_diagram/digital-sovereignty-enabling_architecture_diagram.drawio.png" alt="Digital-Sovereignty-Enabling Architecture Diagram" />

NOTE: **This architecture does not attempt to eliminate observation.
It eliminates the value of observation.**

**[Digital-Sovereignty-Enabling Architecture Overview](https://www.jortsupetterson.workers.dev/)**

**[Rationalizing Why Digital-Sovereignty-Enabling Architecture Needs This Structure](https://github.com/z-base/z-base/blob/main/docs/neutral_diagram/rationale.md)**

**[Long and Awkward Walkthrough on Digital-Sovereignty-Enabling System Architecture](https://www.youtube.com/watch?v=GIFVetIC8X0)**

<img src="https://github.com/z-base/z-base/blob/main/docs/TOP_LEVEL_LABELING.png" alt="Digital-Sovereignty-Enabling Architecture top-level labels" />

NOTE: **The diagram scales both horizontally and vertically.
Horizontally, you can add as many Service Providers as needed.
Vertically, you can add as many Service Clients as needed.**

## Core Value Propositions

### For service providers  
z-base is being designed to reduce legal and operational risk by eliminating the need to process, inspect, or store user data.  
You will be able to operate infrastructure without handling user content.

### For end users  
z-base will provide communication and data features without surveillance, profiling, or hidden extraction.  
User data will remain private, local-first, and cryptographically controlled by the user.

### For platform builders  
z-base is being built to remove the requirement to act as a data custodian.  
You will provide coordination and services, not user dossiers.

### For developers  
The system will map cleanly to real-time object synchronization and evented state patterns.  
The API will be intentionally small, semantically strict, and deterministic.

### For vibe coders 
With the z-base, you will not need to design or maintain a backend application database.  
The infrastructure will store and relay only encrypted envelopes, while logic and authority live in the client.  
This is intended to remove backend surprise work and keep cost and liability predictable during fast iteration.

---

## Where z-base Will Be Used

z-base is being built to function as the **user or organization state layer** of an application.

It will be well suited for:
- user-generated or organization-generated data  
- collaborative or personal state  
- data that should be owned by its creator  
- systems requiring privacy, offline access, and peer verification  

In short: z-base is intended for systems where **the user remains the authority**.

---

## Where z-base Will Not Be Suitable

z-base is not intended for cases where:
- unattended automation must modify state  
- third parties require plaintext access  
- public indexing or content discovery is a core requirement  

In those cases, separate, purpose-built databases will still be required for automation, analytics, or public content.

If automation is required, design it ethically:  
• request explicit, verifiable permission from the user,  
• limit access to a narrow data scope,  
• enforce a bounded time window,  
• state a specific purpose aligned with your service terms,  
• make all data exposure visible and measurable in the UI.

## Philosophy

z-base exists to make it easy to build ethical services.

If your primary goal is maximizing profit through surveillance, data brokerage, or opaque advertising ecosystems, z-base is probably not a fit.

If you still want to monetize data, consider doing so transparently and consensually—by offering to  
purchase clearly defined data sets directly from users, under terms they understand and control.

This is architecture for a web that serves people first.

