# Anveshak

Anveshak is a bootable digital forensic toolkit built to support secure, case-based investigations while preserving evidence integrity throughout the forensic process.

I built Anveshak as my BCA Final Year Project because I wanted to go beyond learning forensic concepts in theory and explore how digital investigations actually work in practice. The goal was to create an environment where evidence could be collected, analyzed, correlated, and documented in a structured way without compromising its integrity.

Rather than functioning as just another collection of forensic utilities, Anveshak follows a case-based workflow. Every investigation maintains its own evidence, logs, reports, and metadata, making it easier to manage and reconstruct events during an examination.

## Features

### Secure Authentication System

* Investigator authentication using bcrypt password hashing
* Session logging and access tracking
* Account lockout protection for failed login attempts

### Case Management

* Structured case-based investigation workflow
* Separate storage of evidence, logs, reports, and metadata for each case
* Organized evidence handling throughout the investigation lifecycle

### Read-Only Evidence Acquisition

* Detection of connected storage devices
* Read-only mounting to prevent accidental modification of evidence
* Automated SHA-256 hashing for integrity verification

### Artifact Analysis

#### Browser History Analysis

* Extraction of browsing history and timestamps
* Recovery of deleted browsing records where available
* Multi-browser support

#### Terminal History Analysis

* Reconstruction of command-line activity
* Analysis of shell history and execution patterns

#### Wi-Fi History Analysis

* Retrieval of previously connected wireless networks
* Timeline-based analysis of network connectivity

#### USB Activity Tracking

* Detection of connected USB devices
* Analysis of connection timestamps and usage patterns

#### Communication Trace Analysis

* Extraction of locally stored communication records from Mozilla Thunderbird
* Offline analysis of email interactions

### Evidence Review & Flagging

* Investigator-driven file inspection
* Manual evidence tagging and flagging
* Support for structured evidence collection

### Super Timeline Generation

One of my favorite parts of the project.

Anveshak correlates browser activity, terminal commands, file modifications, USB events, Wi-Fi logs, and communication traces into a single chronological timeline, making it easier to reconstruct user activity and understand what happened, when it happened, and how different events relate to one another.

### Visualization & Analytics

* Application usage analysis
* Command frequency analysis
* Website activity summaries
* Graphical reports and visualizations

### Automated Report Generation

* PDF-based forensic reports
* Investigation summaries
* Timeline exports
* Evidence hashes and analysis results

## What I Learned

Building Anveshak pushed me far beyond classroom assignments and into areas I had only read about before:

* Digital forensics workflows
* Evidence handling and integrity preservation
* Linux system internals
* Storage and file system concepts
* Timeline reconstruction
* Secure application design
* Report generation and documentation

Most importantly, it taught me how many small details go into building tools that investigators can actually trust.

## Future Improvements

Some areas I'd like to explore in future versions:

* Memory forensics support
* Additional artifact parsers
* Registry analysis
* Enhanced timeline correlation
* Cloud-based evidence acquisition
