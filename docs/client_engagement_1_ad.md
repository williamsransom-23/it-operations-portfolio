# Client Case Study #1: Hybrid Domain Identity Recovery & Account Unlocking
> **Client Profile:** Small Business Financial Advisory Firm  
> **Scope:** Active Directory Domain Services (ADDS) & User Access Management

## The Real Problem
The client’s primary operations manager was completely locked out of the core domain environment right before a major quarterly audit. Recursive authentication failures triggered by a stale background token on a secondary mobile device caused continuous account re-locking instantly upon manual resets.

## Diagnostic Workflow
1. Connected to the client's secondary Domain Controller via remote management tools.
2. Queried the Security Event Log (`Event ID 4625`) to trace the exact source IP and workstation generating the failed handshakes.
3. Inspected the user object inside Active Directory Users and Computers (ADUC) under the **Account** properties tab to clear stale session flags and uncheck lockout restrictions.

## Resolution & Impact
Terminated the rogue background sessions, unlinked expired OAuth tokens, performed a secure credential reset, and verified replication across domain nodes. Resolved within 10 minutes, saving the client from a missed compliance deadline.
