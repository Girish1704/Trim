# Streamlined Azure Security Immersion Lab (2-3 Hours)
## Recommended Modules & Exercises for Condensed Lab

---

## Executive Summary

This document provides a streamlined version of the Azure Security Immersion lab, reducing it from **8 modules** to a focused **5-module experience** that can be completed in **2-3 hours** while maintaining logical flow and hands-on learning value.

**Total Estimated Time: 2-3 hours**

---

## KEEP - Essential Hands-On Modules

### **Module 1: Getting Started with the Environment** *15-20 minutes*
**Status: KEEP (Mandatory)**

#### Exercises to KEEP:
- **Exercise 1: Log in to Azure Portal** (5 min)
  - *Reason: Essential setup - students need to access the environment*
  
- **Exercise 2: Enabling Microsoft Defender for Cloud** (10 min)
  - *Reason: Core foundational setup required for all subsequent labs*
  
- **Exercise 3: Creating Microsoft Defender for Cloud Default Policy** (5 min)
  - *Reason: Quick verification step, essential for security baseline*

**Why Keep This Module:**
- Mandatory foundation for all other exercises
- Actual hands-on configuration (enabling Defender, agents, policies)
- Quick completion time
- Cannot proceed without this setup

---

### **Module 3: Security Policy** *30-40 minutes*
**Status: KEEP (Partially - Focus on Practical Exercises)**

#### Exercises to REMOVE:
- **Exercise 1: Overview of the Microsoft Defender for Cloud Policy**
  - *Reason: Mostly navigation and viewing existing policies*
  - *Type: Review/exploration without significant configuration*

- **Exercise 2: Explore Azure Policy**
  - *Reason: Another exploration/review exercise*
  - *Type: Looking at definitions without creating/modifying*

#### Exercises to KEEP:
- **Exercise 3: Create resource exemption for a recommendation** (10 min)
  - *Reason: Hands-on creation of exemption rules*
  - *Practical use case: Managing false positives*
  
- **Exercise 4: Create policy enforcement and deny** (15 min)
  - *Reason: Active configuration - changing audit to deny*
  - *Key Action: Enforcing security transfer for storage, SQL auditing*
  
- **Exercise 5: Create a custom policy** (15 min)
  - *Reason: Creating custom initiative and assigning it*
  - *Real-world skill: Building organization-specific policies*

**Why Keep These Exercises:**
- Students create actual policies, not just review them
- Practical enforcement scenarios
- Custom policy creation demonstrates advanced capability
- Direct impact on security posture

---

### **Module 5: Improving your Secure Posture** *40-50 minutes*
**Status: KEEP (All Exercises - High Value)**

#### Exercises to KEEP:
- **Exercise 1: Vulnerability Assessment for Containers** (20 min)
  - *Reason: Hands-on - building and pushing container images*
  - *Key Actions: Using Cloud Shell, ACR tasks, scanning images*
  - *Shows vulnerability detection in action*
  
- **Exercise 2: Automate recommendations with workflow automation** (20 min)
  - *Reason: Creating Logic Apps and workflow automation*
  - *Key Actions: Building automation, email notifications*
  - *Real-world integration scenario*
  
- **Exercise 3: Accessing your secure score via ARG** (10 min)
  - *Reason: Hands-on KQL queries in Azure Resource Graph*
  - *Key Actions: Writing and executing queries*
  - *Practical reporting skill*

**Why Keep This Entire Module:**
- All exercises are highly hands-on
- Demonstrates advanced security capabilities
- Real automation and integration scenarios
- Teaches valuable querying skills

---

### **Module 8: Advance Cloud Defense** *25-30 minutes*
**Status: KEEP (Partially - Focus on JIT)**

#### Exercises to KEEP:
- **Exercise 1: Using JIT to reduce the attack surface** (15 min)
  - *Reason: Hands-on JIT configuration and testing*
  - *Key Actions: Enable JIT, request access, connect to VM*
  - *Demonstrates immediate security improvement*
  - *Students experience before/after scenarios*

#### Exercises to REMOVE:
- **Exercise 2: Adaptive Application Control**
  - *Reason: Requires 2 weeks of data collection - won't work in lab*
  - *Students will only see empty recommendations*
  
- **Exercise 3: File Integrity Monitoring**
  - *Reason: Just enabling a feature - no immediate results*
  - *Takes time to show data, no hands-on validation possible*

**Why Keep Exercise 1:**
- Immediate hands-on results
- Students experience denied access, then granted access
- Clear demonstration of attack surface reduction
- Works perfectly within lab timeframe

---

## REMOVE - Modules Not Essential for 2-3 Hour Lab

### **Module 4: Regulatory Compliance** *Would take 30 minutes*
**Status: REMOVE ENTIRELY**

**Why Remove:**
- Exercise 1: Just viewing/reviewing compliance dashboard
- Exercise 2: Only enabling a compliance standard (no hands-on validation)
- Exercise 3: Creating benchmark similar to Module 3 Exercise 5
- **Reasoning:** Mostly read-only, no unique hands-on value, duplicates policy work from Module 3

---

### **Module 6: Microsoft Defender for Cloud and Security Alerts** *Would take 35-40 minutes*
**Status: REMOVE ENTIRELY**

**Why Remove:**
- Exercise 1: Alert validation - just generating sample alerts
- Exercise 2: Alert suppression - managing sample alerts
- Exercise 3: Graph Security API - just viewing data via API endpoint
- **Reasoning:** All exercises work with sample/simulated data, no real security work. Time better spent on actual security configurations

---

### **Module 7: Exporting ASC information to a SIEM** *Would take 30 minutes*
**Status: REMOVE ENTIRELY**

**Why Remove:**
- Exercise 1: Configuring continuous export - takes hours to see data
- Exercise 2: Sentinel integration - configuration only, no immediate results
- **Reasoning:** Requires significant wait time for data to flow. Students won't see results within lab timeframe. Better suited for longer workshops

---

## Streamlined Lab Flow Summary

### Total Time Breakdown

| Module | Time | Status | Reason |
|--------|------|--------|--------|
| **Module 1** | 15-20 min | KEEP | Foundation - Required |
| **Module 2** (Ex 2-3 only) | 30-35 min | KEEP | Hands-on remediation & inventory |
| **Module 3** (Ex 3-5 only) | 30-40 min | KEEP | Policy creation & enforcement |
| **Module 4** | - | REMOVE | Read-only compliance review |
| **Module 5** (All) | 40-50 min | KEEP | High-value automation & scanning |
| **Module 6** | - | REMOVE | Sample alerts only |
| **Module 7** | - | REMOVE | No immediate results |
| **Module 8** (Ex 1 only) | 15 min | KEEP | JIT hands-on demonstration |

**Total Estimated Time: 2 hours 10 minutes - 2 hours 50 minutes**

---

## Recommended Lab Structure

### **Part 1: Foundation & Setup (15-20 min)**
- Module 1: Complete all exercises

### **Part 2: Security Assessment & Remediation (30-35 min)**
- Module 2: Exercises 2-3 only

### **Part 3: Policy Management (30-40 min)**
- Module 3: Exercises 3-5 only

### **Part 4: Advanced Security (55-65 min)**
- Module 5: All exercises
- Module 8: Exercise 1 only

---

## Logical Flow Validation

**Flow Maintained:**
1. **Setup environment** - Students can access Azure and enable Defender
2. **Explore & fix issues** - Students see recommendations and remediate
3. **Configure policies** - Students create exemptions, enforcement, custom policies
4. **Advanced features** - Students work with containers, automation, queries
5. **Access control** - Students configure and test JIT access

**No Dependencies Broken:**
- Each kept exercise builds on previous setup
- No references to removed content
- All hands-on exercises remain functional

**Learning Objectives Achieved:**
- Enable and configure Microsoft Defender for Cloud
- Understand and improve secure score
- Create and manage security policies
- Implement vulnerability scanning
- Automate security workflows
- Configure advanced protection (JIT)

---

## Implementation Notes for Lab Guide

### Exercises Requiring Updates:
1. **Module 2**: Remove all references to Exercise 1 in the module introduction
2. **Module 3**: Update objective list to show only Exercises 3-5
3. **Module 8**: Modify to show only Exercise 1 in objectives
4. **Navigation**: Update "Next Module" references to skip removed modules

### Content to Preserve:
- Keep all validation steps for included exercises
- Maintain all screenshots and GIFs for kept exercises
- Preserve all "Note" and "Important" callouts
- Keep prerequisite checks and warning messages

---

## Key Benefits of This Streamlined Version

1. **Time Efficient**: 2-3 hours vs. 6-8 hours (original)
2. **Focused**: Only hands-on exercises with immediate results
3. **High Value**: Students perform actual security configurations
4. **Complete Flow**: Maintains logical progression
5. **Validated**: All exercises can be completed and verified
6. **Practical**: Skills directly applicable to real-world scenarios

---

## Learning Outcomes Preserved

Students will still learn to:
- Enable and configure Microsoft Defender for Cloud
- Remediate security recommendations
- Manage resources with inventory and tagging
- Create policy exemptions and enforcement rules
- Build custom security policies
- Scan containers for vulnerabilities
- Automate security workflows with Logic Apps
- Query security data with Azure Resource Graph
- Implement Just-in-Time VM access

---

## Final Recommendation

**Implement this streamlined version to:**
- Meet the 2-3 hour time constraint
- Maintain high-quality hands-on experience
- Preserve logical learning flow
- Focus on practical, applicable skills
- Ensure all exercises can be completed and validated within the lab session

**Removed content represents:**
- Read-only review exercises
- Simulated/sample data scenarios
- Long wait-time integrations
- Duplicate functionality demonstrations

This balanced approach delivers **maximum learning value within minimum time** while maintaining the integrity of the Azure Security Immersion experience.

---

*Document created: November 12, 2025*
*Last updated: November 12, 2025*
