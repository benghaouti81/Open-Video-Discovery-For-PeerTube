Creator Hosting & Infrastructure Model

Purpose

The Open Video Discovery for PeerTube project is a discovery layer, not a video hosting company.

However, a federated video ecosystem needs more than software and protocols. Creators also need somewhere to host their channels and videos.

Not every creator has the technical knowledge, server hardware, bandwidth, storage, or reliable internet connection required to operate a PeerTube instance.

For this reason, the project recognizes two complementary models:

1. Creator-operated hosting
2. Independent hosting providers

Both models can exist within the same ecosystem.

The purpose of this model is to make hosting a choice rather than a barrier.

---

1. Creator-Operated Hosting

A creator or organization may operate their own PeerTube instance.

In this model:

- The creator controls the server.
- The creator controls their PeerTube instance.
- The creator manages their storage and bandwidth.
- The creator determines their own content policies.
- The creator remains responsible for their content.
- The creator can participate in federation according to their own configuration.

The Open Video Discovery platform simply indexes and exposes discoverable information about the content.

The discovery platform does not become the owner or host of the videos.

---

2. Independent Hosting Providers

Creators who do not want to operate their own infrastructure may use an independent hosting provider.

A hosting provider may operate one or more PeerTube instances and host channels for multiple creators.

The provider may offer services such as:

- Server infrastructure
- Storage
- Bandwidth
- Backups
- Maintenance
- Software updates
- Monitoring
- Technical support
- Instance administration
- Optional analytics or other infrastructure services

The provider may serve one creator, a small group of creators, or a large network of channels.

This creates an infrastructure layer between creators and the underlying server hardware without requiring the central discovery platform to become that infrastructure provider.

---

3. Different Hosting Providers, Different Capabilities

Not every hosting provider needs to have the same infrastructure.

A small provider may operate a modest server with limited bandwidth.

A larger provider may operate:

- Multiple servers
- High-bandwidth connections
- Distributed infrastructure
- Large storage capacity
- Regional infrastructure
- Professional monitoring and support

The ecosystem should not assume that every PeerTube instance has identical technical capabilities.

Peer-to-peer technologies such as WebTorrent may be useful in some environments, while a provider with sufficient bandwidth may be able to serve videos directly.

The discovery platform does not require one specific infrastructure model.

Its role is to make content discoverable regardless of which compatible hosting model is used.

---

4. Hosting as a Service

Hosting providers may offer different economic models.

4.1 Paid Hosting

A creator pays a hosting provider for infrastructure.

For example, the provider may charge according to:

- Storage
- Bandwidth
- Number of channels
- Number of videos
- Server capacity
- Support level
- Other agreed services

The creator remains free to establish advertising and sponsorship relationships independently.

The hosting provider is paid for infrastructure and services rather than becoming the advertising intermediary.

---

4.2 Sponsored or Subsidized Hosting

A hosting provider may choose to support creators without charging them the full cost of hosting.

This could be used for creators whose content is considered valuable but who cannot afford professional hosting.

The provider may cover part or all of the infrastructure cost.

Possible arrangements could include:

- Free hosting
- Subsidized hosting
- Grants
- Community-supported hosting
- Sponsorship-based hosting

Where appropriate, a provider and creator may agree that the provider receives an agreed share of advertising or sponsorship revenue.

Such an agreement remains between the creator and the hosting provider.

The central discovery platform does not collect the money, negotiate the contract, or take a commission.

---

5. Hosting Is Separate From Discovery

The architecture intentionally separates three different functions:

Content Creation

Creators produce and control their content.

Infrastructure

Creators or independent hosting providers operate the infrastructure required to store and deliver the content.

Discovery

Open Video Discovery for PeerTube helps audiences find that content.

These functions do not need to belong to the same organization.

A creator could therefore:

- Produce content independently
- Use a third-party hosting provider
- Be discovered through Open Video Discovery
- Establish advertising relationships directly with advertisers

This separation is a fundamental part of the project.

---

6. Hosting Providers Are Independent Participants

The project does not intend to create a single official hosting company.

Different providers should be able to compete or cooperate according to their own models.

They may differ in:

- Price
- Storage
- Bandwidth
- Geographic location
- Reliability
- Support
- Privacy policies
- Technical capabilities
- Content policies
- Federation policies
- Additional services

This creates room for different types of providers.

A small community server and a professional infrastructure company can both participate in the broader ecosystem.

---

7. Creator Portability

Hosting should not become another form of platform lock-in.

Where technically and legally possible, creators should be able to move their channels or content between compatible hosting providers.

The project therefore favors:

- Open standards
- Portable data
- Transparent hosting terms
- Clear ownership arrangements
- Export capabilities
- Interoperable infrastructure

A creator should not have to lose their identity or entire catalog simply because they decide to change hosting providers.

The exact technical mechanisms for portability may evolve with the PeerTube ecosystem and community contributions.

---

8. Hosting Networks and Creator Organizations

A hosting provider does not necessarily need to work with creators individually.

Organizations may emerge that combine several functions.

For example, a creator network or media organization could provide:

- Hosting
- Production support
- Advertising relationships
- Sponsorship management
- Technical assistance
- Multiple creator channels
- Shared infrastructure

Such organizations may become important as the ecosystem grows.

The Open Video Discovery platform should remain compatible with these organizations without becoming one itself.

A creator network may therefore operate independently while its channels remain discoverable through the central discovery layer.

---

9. Relationship With Advertising & Sponsorship

This model is designed to work alongside the project's Advertising & Sponsorship Policy.

The roles remain separate:

Creator ↔ Advertiser

The creator may establish direct sponsorship or advertising relationships with advertisers.

Creator ↔ Hosting Provider

The creator may separately pay for hosting or agree to another hosting arrangement.

Advertiser ↔ Hosting Provider

In some cases, a hosting provider or creator organization may participate in advertising operations according to its own agreement with creators.

Discovery Platform

The discovery platform provides visibility and discovery.

It does not automatically become a party to these commercial relationships.

The platform does not:

- Collect advertising payments
- Process sponsorship payments
- Take a percentage of creator revenue
- Set advertising prices
- Require creators to use a particular hosting provider
- Require creators to use a particular advertiser
- Rank creators according to advertising revenue

This preserves the separation established by the Advertising & Sponsorship Policy.

---

10. No Official Hosting Monopoly

The project should avoid creating a situation where creators must use one official hosting provider to participate.

The discovery layer should remain compatible with a broader ecosystem of independent infrastructure providers.

The objective is:

«Centralized discovery, distributed infrastructure, independent creators.»

The discovery interface may be centralized because audiences benefit from having one recognizable place to search.

The infrastructure underneath it does not need to be centralized.

---

11. A Possible Ecosystem

The ecosystem can be understood as several independent layers:

                    ┌───────────────────────┐
                    │       AUDIENCE        │
                    └───────────┬───────────┘
                                │
                                ▼
              ┌─────────────────────────────────┐
              │   OPEN VIDEO DISCOVERY          │
              │                                 │
              │ Search • Discovery • Directory  │
              │ Categories • Channels • Links   │
              └───────────────┬─────────────────┘
                              │
                              ▼
                     ┌────────────────┐
                     │    PEERTUBE    │
                     │    NETWORK     │
                     └───────┬────────┘
                             │
              ┌──────────────┴──────────────┐
              │                             │
              ▼                             ▼
     ┌─────────────────┐          ┌────────────────────┐
     │ Creator-Hosted  │          │ Hosting Providers  │
     │    Instance     │          │                    │
     └────────┬────────┘          │ Small / Large /    │
              │                   │ Specialized        │
              │                   └─────────┬──────────┘
              │                             │
              ▼                             ▼
       ┌─────────────┐              ┌────────────────┐
       │   Creator   │              │    Creators    │
       └─────────────┘              │    Channels    │
                                    └────────────────┘


       Advertising & Sponsorship
       ─────────────────────────

       Creator  ◄──────────────►  Advertiser
          │
          │
          ▼
    Hosting Provider
    (where applicable)

The important point is that these are separate roles, even when one organization happens to perform several of them.

---

12. What This Model Solves

This model addresses a practical problem in decentralized video.

Decentralization does not automatically mean that every creator can afford or operate infrastructure.

A creator may have:

- Valuable content
- An audience
- Limited technical knowledge
- Limited bandwidth
- No server
- Limited financial resources

The ecosystem should not exclude that creator simply because they cannot self-host.

A hosting provider can supply the missing infrastructure while the creator remains part of the wider open ecosystem.

At the same time, creators who have the technical ability and resources remain free to operate their own infrastructure.

---

13. What This Project Does Not Promise

This model does not promise that:

- Hosting will always be free
- Every provider will have the same capabilities
- Every provider will accept every creator
- Every provider will have unlimited bandwidth
- Every provider will offer the same content policies
- P2P will always be required
- One hosting model will work for everyone

Infrastructure has real costs.

Storage, bandwidth, servers, maintenance, electricity, connectivity, backups, and technical support must be provided by someone.

The purpose of this model is not to hide those costs.

It is to create multiple ways of providing the infrastructure.

---

14. Long-Term Direction

As the ecosystem grows, different infrastructure models may emerge naturally.

Possible participants include:

- Individual creators
- Community-run instances
- Non-profit organizations
- Commercial hosting providers
- Creator networks
- Media organizations
- Educational institutions
- Regional infrastructure providers
- Large-scale hosting networks

The project should remain open to these possibilities without requiring one of them to become the dominant model.

The central principle remains:

«Creators should have choices about where their content lives and how their infrastructure is provided.»

And:

«Discovery should not require ownership or control of the infrastructure.»

---

15. Relationship to the Project Manifesto

This model extends the project's central principle:

«Centralized discovery, not centralized control.»

The discovery layer can provide a simple and recognizable place for audiences to find content while the underlying infrastructure remains distributed among creators and independent providers.

The project does not need to own every server.

It does not need to host every video.

It does not need to employ every creator.

It does not need to control advertising.

Its role is to connect the pieces.

---

16. Guiding Principle

The long-term goal is not to replace one centralized platform with another centralized platform.

It is to separate functions that do not need to be controlled by the same organization:

Creation → Hosting → Discovery → Advertising

Each can have independent participants.

Creators can choose how they create and where they host.

Hosting providers can compete on infrastructure and services.

Advertisers can establish direct relationships with suitable creators.

Audiences can use a common discovery layer to find content across the ecosystem.

The project exists to connect these layers without needing to own them.
