---
layout: home
introduction: |
  FROST is the Flexible Round-Optimized Schnorr Threshold signature scheme.
  FROST reduces network overhead during signing operations while protecting against forgery attacks applicable to prior similar threshold and multisignature constructions.
  FROST can be safely used without limiting concurrency of signing operations yet allows for true threshold signing, as only a threshold number of participants are required for signing operations.

  Here, we provide the NIST submission for FROST as a two-round protocol,
  but implementations can optimize to a single-round single-round signing protocol as the first round can be performed as a batched pre-processing stage.

scientific_background: |
  FROST achieves unforgeability in the honest minority setting;
  i.e., FROST is secure so long as an fewer than t-1 out of n participants are malicious,
  where t is the threshold required to produce a signature,
  and n is the total number of participants.
  The unforgeability of FROST is proven assuming the hardness of the Algebraic One-More Discrete Logarithm Assumption (AOMDL) in the Random Oracle Model (ROM).

  We model FROST signing assuming an idealized key generation scheme that produces a public key and n Shamir secret shares of the secret key.
  In practice, this operation can be performed by a trusted dealer,
  or a distributed key generation (DKG) scheme.

  We model message passing using a central coordinator,
  that is trusted only to not perform denial of service attacks.
  However, a malicious coordinator can only prevent the generation of signatures;
  it does not impact the unforgeability.

team_overview: |
  The FROST NIST submission team is as follows.

  * Elizabeth Crites
  * Conrado Gouvea
  * Ian Goldberg
  * Jack Grigg
  * Jonathan Katz
  * Chelsea Komlo
  * Mary Maller
  * Stefano Tessaro
  * Nikita Sorokovikov
  * Denis Varlakov
  * Chenzhi Zhu
---

