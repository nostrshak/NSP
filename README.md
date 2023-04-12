# Nostr Service Proxy

## Goals

### Improved privacy
- NSP talks to relays via TOR
- Client(s) talk to NSP via public IP or via TOR 

### Provide self-controlled proxy to relays
- Manages account relay list
  - NSP presents as a relay to clients
  - Clients only point to NSP and maybe 1 or 2 backup NSPs.
    - Actual relays are hidden from clients.
    - Relays used by an account are not discoverable through nostr events
  - Relay list can be different for each account being managed
- Runs on personal equipment (on-prem), but could be cloud based
  - Could be extended to offer cloud service
- Caches events (follow, followed, reacted, zapped, etc.)
- Small number of accounts serviced

### Intermediary between smart clients and dumb, high capacity, high demand, highly available main relays
- Offload client task of dealing with multiple relays
- Reduce event queries to main relays by cacheing notes/events of interest to small account pool
- Handle various monetization models implemented by main relays

### Could assist with DM management

## Documents
### Supported NIPs and Kinds Document
[Planned support for nips and kinds](nip_and_kind_support.md)

### Process Flow Description
- Client connects to NSP
- NSP connects to relays
- Client disconnects from NSP
- NSP can disconnect from relays
  - During disconnect periodss, NSP could occasionally connect to relays and cache relevant events

### Data Model Document
- Database(s) supported
- Logical table definitions
- Account support tables
- Event cache support tables
- Search functions

### API Document
- Status of standard Relay API functions
- List of additional API functions (if any)

### NSP Management Interface Document
