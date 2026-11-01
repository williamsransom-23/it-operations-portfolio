# Client Case Study #3: Remote Workstation Crash Diagnostics & OS Repair
> **Client Profile:** Remote Creative Agency / Freelance Client  
> **Scope:** Windows 11 Endpoint Diagnostics & Event Viewer Analysis

## The Real Problem
A key contractor’s Windows 11 workstation was suffering from recurring system freezes, application crashes, and graphics driver timeouts during heavy media rendering tasks.

## Diagnostic Workflow
1. Initiated a remote diagnostic session to inspect system telemetry.
2. Opened **Event Viewer** (`eventvwr.msc`) and filtered System/Application logs to isolate critical kernel errors (`Event ID 41` and display driver crashes).
3. Inspected **Device Manager** hardware trees to locate flagged controller flags.

## Resolution & Impact
Uninstalled corrupted vendor display drivers in Safe Mode, deployed clean manufacturer-certified packages, cleared accumulated system cache, and ran a full system integrity check (`sfc /scannow`), completely eliminating system instability.
