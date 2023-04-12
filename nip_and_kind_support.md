# Nostr nip and kind support

## Possible values:
- Supported
- Will Support
- Likely Won't Support
- Not Supported
- Disposition TBD

## Support status for nips
This list is in progress. Nips were marked tbd as the default status.

| nip    | description                                                      | support       |
| ------ | ---------------------------------------------------------------- | ------------- |
| NIP-01 | Basic protocol flow description                                  | Supported     |
| NIP-02 | Contact List and Petnames                                        | Supported     |
| NIP-03 | OpenTimestamps Attestations for Events                           | Supported     |
| NIP-04 | Encrypted Direct Message                                         | Supported     |
| NIP-05 | Mapping Nostr keys to DNS-based internet identifiers             | Supported     |
| NIP-06 | Basic key derivation from mnemonic seed phrase                   | n/a*          |
| NIP-07 | window.nostr capability for web browsers                         | n/a           |
| NIP-08 | Handling Mentions – unrecommended, deprecated in favor of NIP-27 | Not Supported |
| NIP-09 | Event Deletion                                                   | tbd           |
| NIP-10 | Conventions for clients' use of e and p tags in text events      | Supported     |
| NIP-11 | Relay Information Document                                       | Supported     |
| NIP-12 | Generic Tag Queries                                              | Supported     |
| NIP-13 | Proof of Work                                                    | tbd           |
| NIP-14 | Subject tag in text events.                                      | Supported     |
| NIP-15 | End of Stored Events Notice                                      | Supported     |
| NIP-16 | Event Treatment                                                  | Supported     |
| NIP-18 | Reposts                                                          | Supported     |
| NIP-19 | bech32-encoded entities                                          | n/a*          |
| NIP-20 | Command Results                                                  | Supported     |
| NIP-21 | nostr URL scheme                                                 | n/a           |
| NIP-22 | Event created_at Limits                                          | Supported     |
| NIP-23 | Long-form Content                                                | Supported     |
| NIP-25 | Reactions                                                        | Supported     |
| NIP-26 | Delegated Event Signing                                          | Supported     |
| NIP-27 | Text Note References                                             | n/a           |
| NIP-28 | Public Chat                                                      | Supported     |
| NIP-33 | Parameterized Replaceable Events                                 | Supported     |
| NIP-36 | Sensitive Content                                                | n/a           |
| NIP-39 | External Identities in Profiles                                  | n/a           |
| NIP-40 | Expiration Timestamp                                             | Supported     |
| NIP-42 | Authentication of clients to relays                              | Supported     |
| NIP-45 | Counting results                                                 | Supported     |
| NIP-46 | Nostr Connect                                                    | Supported     |
| NIP-50 | Keywords filter                                                  | Supported     |
| NIP-51 | Lists                                                            | tbd           |
| NIP-56 | Reporting                                                        | tbd           |
| NIP-57 | Lightning Zaps                                                   | tbd           |
| NIP-58 | Badges                                                           | tbd           |
| NIP-65 | Relay List Metadata                                              | tbd           |
| NIP-78 | Application-specific data                                        | tbd           |

* NIP-06: Advanced implementation could manage keys for the account.
* NIP-19: May utilize metadata incluced in bech-32 encoded elements.


## Support status for nostr event kinds
This is a first-pass at the kinds that will be supported and is likely to change.

| kind        | description                      | nip | support        | comments                       |
| ----------- | -------------------------------- | --- | -------------- | ------------------------------ |
|           0 | Metadata                         |   1 | tbd            |                                |
|           1 | Short Text Note                  |   1 | Supported      |                                |
|           2 | Recommend Relay                  |   1 | Likely Support |                                |
|           3 | Contacts                         |   2 | tbd            |                                |
|           4 | Encrypted Direct Messages        |   4 | tbd            | DMs are highly fluid right now |
|           5 | Event Deletion                   |   9 | tbd            |                                |
|           6 | Reposts                          |  18 | Supported      |                                |
|           7 | Reaction                         |  25 | Supported      |                                |
|           8 | Badge Award                      |  58 | Supported      |                                |
|          40 | Channel Creation                 |  28 | tbd            | Chat function                  |
|          41 | Channel Metadata                 |  28 | tbd            | Chat function                  |
|          42 | Channel Message                  |  28 | tbd            | Chat function                  |
|          43 | Channel Hide Message             |  28 | tbd            | Chat function                  |
|          44 | Channel Mute User                |  28 | tbd            | Chat function                  |
|        1984 | Reporting                        |  56 | Supported      |                                |
|        9734 | Zap Request                      |  57 | Supported      |                                |
|        9735 | Zap                              |  57 | Supported      |                                |
|       10000 | Mute List                        |  51 | tbd            | List function                  |
|       10001 | Pin List                         |  51 | tbd            | List function                  |
|       10002 | Relay List Metadata              |  65 | tbd            | List function                  |
|       22242 | Client Authentication            |  42 | Supported      |                                |
|       24133 | Nostr Connect                    |  46 | Supported      |                                |
|       30000 | Categorized People List          |  51 | tbd            | List function                  |
|       30001 | Categorized Bookmark List        |  51 | tbd            | List function                  |
|       30008 | Profile Badges                   |  58 | Supported      |                                |
|       30009 | Badge Definition                 |  58 | Supported      |                                |
|       30023 | Long-form Content                |  23 | Supported      |                                |
|       30078 | Application-specific Data        |  78 | Likely Support |                                |
|   1000-9999 | Regular Events                   |  16 | tbd            |                                |
| 10000-19999 | Replaceable Events               |  16 | tbd            |                                |
| 20000-29999 | Ephemeral Events                 |  16 | tbd            |                                |
| 30000-39999 | Parameterized Replaceable Events |  33 | tbd            |                                |
