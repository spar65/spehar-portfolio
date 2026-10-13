# 🧠 Brand Management Tool (BMT) in GemStone/S Smalltalk

Welcome to the Brand Management Tool (BMT), an enterprise-level content publishing and brand management system I built in GemStone/S Smalltalk. It is a multi-network platform where users manage accounts, publish content, earn tokens, support brands, and take part in certification-based voting. Its architecture (singleton patterns, a hierarchical object model, and a full testing framework) shows how Smalltalk can deliver scalable, maintainable solutions for complex domains involving financial transactions, content management, and user engagement.

**Status:** [Proof of concept, built YEAR. Update: active / archived.]

# BMT (Brand Management Tool): Detailed Project Overview

## Project Summary

**BMT (Brand Management Tool)** is a content publishing and brand management system built in **GemStone/S Smalltalk**. It implements a multi-network platform where users can manage accounts, publish content, earn tokens, support brands, and vote, with certification-based access controls.

---
### 🌾 Key Skill or Success

**Proof of Concept:** Independently designed and built a transaction system aimed at changing how the brand marketplace works, with new ways to donate and earn revenue. The design is meant to unlock new revenue streams and reduce marketing costs by changing how personalities and political figures earn money: through activity AND proven brand strength. Creators don't need to post constantly to earn marketing dollars. Value is earned over time, allowing fewer, more substantive interactions.

---

## Core Architecture & Design Patterns

### 1. **Singleton Pattern Implementation**
The system uses singleton patterns for core system components:
- `Application` class with `DefaultApplication`, `CurrentApplication` instances
- `Control` with `ControlSingleton`
- `Bank` with `BankSingleton`
- `BankToken` with `BankTokenSingleton`
- `Batch` with `BatchSingleton`

### 2. **Hierarchical Object Model**
All domain objects inherit from `BaseObject`, providing:
- UUID generation for unique identification
- Creation and modification timestamps
- Effective dates for temporal data
- Immutability controls via `setImmutableTrue/False`

### 3. **Symbol Dictionary Management**
The system creates and manages a dedicated `BMT` symbol dictionary in GemStone for namespace isolation.

## Domain Model Structure

### **Core Categories**

1. **Application Layer**
   - `Account`: User accounts per network with certifications, balances, transactions
   - `AccountMaster`: Master user account managing multiple network accounts
   - `Network`: Organizations that host brands and manage content
   - `Brand`: Subclass of Network representing individual brands
   - `Application`: Central application controller and registry

2. **Core Infrastructure**
   - `BaseObject`: Foundation class with UUID, timestamps, immutability
   - `Control`: System control and configuration management
   - `Bank`/`BankToken`: Cryptocurrency and token management
   - `Transaction`: Financial transaction processing
   - `Verify`: User verification system

3. **Content Publishing**
   - `Publishable`: Base class for publishable content
   - `Content`: Network-specific publishable content
   - `Article`: Text-based content publication
   - `ElectionSlate`: Political content with candidate recommendations
   - `Comment`: User comments with certification-based visibility

4. **Certification System**
   - `Certification`: Multi-level certification framework
   - `Test`: Certification testing with sections and questions
   - `Section`: Test sections with minimum passing scores
   - `Question`/`Answer`: Test questions with philosophical categorization

5. **Voting System**
   - `Vote`: User votes weighted by certification level
   - `VotingSystem`: Vote aggregation and management

6. **Support Systems**
   - `Batch`: Monthly payment processing for brands/networks
   - `Reports`: System reporting functionality
   - `Security`: Security management
   - `Compliance`: Regulatory compliance tracking

## Key Business Features

### **Multi-Network Architecture**
- Users have one `AccountMaster` but multiple `Account` instances per network
- Each network can host multiple brands
- Brands inherit network functionality but add brand-specific features

### **Token Economy**
- Dual currency system: Network crypto + earned tokens
- Monthly fee payments from users to brands
- Token earnings based on content engagement
- Percentage-based payment distribution to accounts

### **Certification-Based Access Control**
- Multi-level certification system (tests → sections → questions)
- Content visibility controlled by certification requirements
- Vote weighting based on certification levels
- Philosophical categorization of questions/answers

### **Content Publishing Pipeline**
- Hierarchical content model: `Publishable` → `Content` → specific types
- Network-specific content with comment threads
- Certification-based content access controls
- Brand affiliation and support tracking

## Technical Implementation

### **Transaction Management**
- Transaction system for crypto/token transfers
- Status tracking: `new` → `committed`/`rejected`/`pending`
- Balance validation and fund availability checking
- Global transaction registry in `Application`

### **Testing Framework**
- Test suite orchestrated by `TestHarness`
- Individual test classes for each domain class (Test*)
- Test resource management with setup/teardown
- Multiple test resource categories (Core, Cert, Pub, Support)
- Global test data management

### **Logging & Monitoring**
- Dual logging system: `Log` for general, `LogTX` for transactions
- Multiple log levels with queue-based processing
- Critical error logging with component identification
- System performance monitoring

### **Configuration Management**
- Environment-specific configuration (Production vs Development)
- Install and system configuration separation
- XML parsing for configuration files
- Dynamic configuration reloading

## Notable Design Decisions

1. **GemStone/S Integration**: Heavy use of GemStone's object database features, with persistent object storage and transaction management.

2. **Immutability Controls**: BaseObject can make objects immutable once finalized, protecting data integrity.

3. **Global Collections**: The Application class maintains global collections of all major entities (accounts, networks, brands, transactions).

4. **Error Handling**: Thorough error checking with logging and transaction rollback.

5. **Production Safety**: Multiple safeguards against destructive operations in production environments.

## Current State & Development Notes

The codebase is in active development, with:
- TODO comments marking planned features
- Development vs Production environment controls
- Broad test coverage
- Clear separation of concerns across functional domains

BMT shows enterprise-level Smalltalk development: a complex, multi-user, multi-network content and brand platform built on solid architecture, thorough testing, and clear separation of concerns.

*© 2026 GiDanc AI LLC. Defining the path, creating the hope, delivering the dream.*
