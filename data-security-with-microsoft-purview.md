# Data Security with Microsoft Purview - Streamlined Lab Recommendation
## Condensed Lab Structure for 2-3 Hour Duration

---

## Executive Summary

This document provides a streamlined version of the Data Security with Microsoft Purview lab, reducing it from **9 comprehensive labs** to a focused set of exercises that can be completed in **2-3 hours** while maintaining hands-on learning value and practical application of Microsoft Purview capabilities.

**Original Duration:** 6-8 hours (estimated)  
**Streamlined Duration:** 2-3 hours

---

## Lab Analysis Overview

### Original Lab Structure

| Lab | Title | Estimated Time | Type |
|-----|-------|----------------|------|
| Lab 01 | Configure Sensitive Labels | 30 min | Configuration |
| Lab 02 | Publish sensitivity labels | 30 min | Configuration |
| Lab 03 | Configure Message Encryption | 60 min | Configuration + Testing |
| Lab 04 | Install and Use AIP Unified Labeling Client | 30 min | Installation + Classification |
| Lab 05 | Use M365 Apps to Label data | 30 min | Application Testing |
| Lab 06 | Create a DLP Policy | 60 min | Policy Creation + Testing |
| Lab 07 | Configure Safe breach simulation | 60 min | Simulation Setup |
| Lab 08 | Configure Insider Risk Management | 60 min | Policy Configuration |
| Lab 09 | Investigate insider risk activities | 60 min | Investigation |

**Total Original Time:** 6-7 hours

---

## KEEP - Essential Labs for Condensed Version

### Lab 01: Configure Sensitive Labels
**Duration:** 30 minutes  
**Status:** KEEP (Mandatory)

**Reason for Inclusion:**
- Foundation for all subsequent data protection activities
- Hands-on creation of sensitivity labels
- Establishes classification framework
- Required for Labs 02, 04, and 05

**Key Activities:**
- Create "Confidential-Finance" sensitivity label
- Configure encryption settings
- Set up content markings (watermark, header, footer)
- Configure auto-labeling conditions
- Create "Highly-Confidential" label

**Learning Value:**
Students learn to define and configure organizational data classification policies from scratch.

---

### Lab 02: Publish sensitivity labels
**Duration:** 30 minutes  
**Status:** KEEP (Mandatory)

**Reason for Inclusion:**
- Direct continuation of Lab 01
- Makes labels available to users organization-wide
- Quick configuration with immediate impact
- Required for testing in subsequent labs

**Key Activities:**
- Select labels for publishing
- Configure policy settings
- Assign to users and groups
- Review published policies

**Learning Value:**
Students understand the deployment process for making data protection policies operational.

---

### Lab 04: Install and Use AIP Unified Labeling Client
**Duration:** 30 minutes  
**Status:** KEEP (Modified)

**Reason for Inclusion:**
- Hands-on installation experience
- Demonstrates client-side classification
- Shows File Explorer integration
- Practical file classification skills

**Modification Recommended:**
- Reduce number of test files to 2-3 instead of creating multiple folders
- Focus on essential classification scenarios only

**Key Activities:**
- Install Microsoft Purview Information Protection client
- Use File Explorer to classify files
- Apply sensitivity labels to documents

**Learning Value:**
Students gain practical experience with endpoint-based data classification tools.

---

### Lab 06: Create a Data Loss Prevention (DLP) Policy
**Duration:** 60 minutes  
**Status:** KEEP (High Priority)

**Reason for Inclusion:**
- Core DLP functionality demonstration
- Hands-on policy creation from scratch
- Immediate testing and validation
- Real-world applicable scenario (credit card protection)

**Key Activities:**
- Create custom DLP policy for credit card data
- Configure policy conditions and actions
- Set up user notifications and alerts
- Test policy effectiveness by sending emails
- Review alerts and policy matches

**Learning Value:**
Students learn end-to-end DLP policy lifecycle including creation, deployment, testing, and monitoring.

---

## REMOVE - Labs Excluded from Condensed Version

### Lab 03: Configure Message Encryption
**Duration:** 60 minutes  
**Status:** REMOVE

**Reason for Removal:**
- Overlaps with sensitivity label encryption functionality covered in Lab 01
- Requires external email testing which adds complexity
- Encryption concepts already demonstrated through sensitivity labels
- Time-intensive for marginal additional learning value

**Alternative Coverage:**
Encryption concepts are adequately addressed through sensitivity label configuration in Lab 01.

---

### Lab 05: Use M365 Apps to Label data
**Duration:** 30 minutes  
**Status:** REMOVE

**Reason for Removal:**
- Repetitive of concepts from Lab 01 and Lab 04
- Focuses on manual label application which is already demonstrated
- Testing sensitivity labels in Word/Outlook duplicates Lab 04 functionality
- Can be covered briefly in Lab 04 demonstrations

**Alternative Coverage:**
Incorporate a brief demonstration of M365 app labeling within Lab 04.

---

### Lab 07: Configure Safe breach simulation
**Duration:** 60 minutes  
**Status:** REMOVE

**Reason for Removal:**
- Not core data protection functionality
- Focuses on security awareness rather than data governance
- Requires significant setup time
- Results take time to materialize
- Peripheral to primary Purview data security objectives

**Rationale:**
While valuable for security awareness programs, phishing simulation is not central to data classification, labeling, and DLP - the core focus of Microsoft Purview data security.

---

### Lab 08: Configure Insider Risk Management
**Duration:** 60 minutes  
**Status:** REMOVE

**Reason for Removal:**
- Requires 24-48 hours for meaningful data collection
- Cannot be effectively tested within lab timeframe
- Complex prerequisite configuration
- Dependent on Lab 09 for value realization

**Timing Issue:**
Lab explicitly states: "It will take up to 24 hours to reflect the user activities" - incompatible with 2-3 hour lab duration.

---

### Lab 09: Investigate insider risk activities
**Duration:** 60 minutes  
**Status:** REMOVE

**Reason for Removal:**
- Dependent on Lab 08 which requires 24-hour data collection
- No meaningful activities to investigate within lab timeframe
- Requires extensive prior setup
- Investigation scenarios cannot be simulated quickly

**Dependency Issue:**
Cannot function without Lab 08 data, and both labs require extended time for data population.

---

## Streamlined Lab Flow Summary

### Recommended Structure

| Lab | Duration | Status | Core Focus |
|-----|----------|--------|------------|
| Lab 01 | 30 min | KEEP | Create sensitivity labels |
| Lab 02 | 30 min | KEEP | Publish labels to organization |
| Lab 04 | 30 min | KEEP | Install client & classify files |
| Lab 06 | 60 min | KEEP | Create & test DLP policy |

**Total Streamlined Duration:** 2.5 hours (150 minutes)

---

## Recommended Lab Execution Flow

### Part 1: Data Classification Foundation (60 minutes)

**Lab 01 + Lab 02 Combined Session**
- Create two sensitivity labels (Confidential-Finance, Highly-Confidential)
- Configure encryption and content markings
- Publish labels to all users
- Brief waiting period for label propagation

**Learning Outcome:**
Students establish a complete data classification framework ready for application.

---

### Part 2: Endpoint Classification (30 minutes)

**Lab 04: Client Installation and File Classification**
- Install Microsoft Purview Information Protection client
- Classify files using File Explorer integration
- Quick demonstration of M365 app labeling (Word/Outlook)

**Learning Outcome:**
Students gain hands-on experience with client-side classification tools and understand label persistence.

---

### Part 3: Data Loss Prevention (60 minutes)

**Lab 06: DLP Policy Creation and Testing**
- Create custom DLP policy for sensitive data (credit cards)
- Configure rules, conditions, and actions
- Set up alert policies
- Test policy by attempting to send sensitive data
- Review alerts and policy effectiveness

**Learning Outcome:**
Students complete end-to-end DLP implementation including policy creation, deployment, testing, and alert management.

---

## Implementation Considerations

### Prerequisites Handled Efficiently

**Single Client VM Setup:**
All labs execute within one RDP session to the client VM, eliminating multiple login cycles.

**Sequential Label Propagation:**
Labs 01 and 02 should be completed back-to-back to allow label propagation during Lab 04 setup.

**DLP Testing Preparation:**
Students should use personal email addresses that they can access during the lab for testing.

---

## Learning Objectives Preserved

Upon completing the streamlined lab, students will be able to:

1. Create and configure sensitivity labels with encryption and content markings
2. Publish sensitivity labels to organizational users
3. Install and use the Microsoft Purview Information Protection client
4. Classify files using File Explorer integration
5. Create comprehensive DLP policies from scratch
6. Configure policy conditions using sensitive information types
7. Set up user notifications and alert policies
8. Test and validate DLP policy effectiveness
9. Review and respond to DLP alerts
10. Understand the complete lifecycle of data protection implementation

---

## Learning Objectives Not Covered (Due to Time Constraints)

The following objectives from removed labs cannot be achieved in 2-3 hour timeframe:

- Message encryption rule configuration (Lab 03)
- Advanced M365 app labeling scenarios (Lab 05)
- Phishing attack simulation and awareness training (Lab 07)
- Insider risk policy configuration and investigation (Labs 08-09)

**Recommendation for Extended Workshops:**
These topics can be covered in a follow-up advanced session or multi-day workshop where time permits proper data collection and analysis.

---

## Time Buffer and Flexibility

**Built-in Buffer Time:**
The 150-minute core duration allows for:
- 10-15 minutes for initial environment setup
- 15-20 minutes for questions and troubleshooting
- 5-10 minutes for breaks

**Total with Buffer:** 2.5 - 3 hours

**Flexibility Options:**

If running ahead of schedule:
- Expand Lab 04 to include more M365 app labeling demonstrations
- Add additional DLP policy scenarios in Lab 06

If running behind schedule:
- Reduce number of test files in Lab 04 to 2 instead of 3-4
- Simplify DLP policy to single condition instead of multiple

---

## Validation Checkpoints

### Lab 01 Validation
Students should successfully create two sensitivity labels with proper encryption and content marking configuration visible in Microsoft Purview portal.

### Lab 02 Validation
Published policy should be visible under Label policies section with status showing labels available to all users.

### Lab 04 Validation
Students should successfully classify at least 2 files using File Explorer with labels persisting after save.

### Lab 06 Validation
Students should:
- Successfully create DLP policy
- Receive policy tip when attempting to send sensitive data
- See blocked email notification
- Observe alerts in DLP alert dashboard

---

## Critical Success Factors

### Proper Label Propagation Time
Allow 5-10 minutes between Lab 02 completion and Lab 04 start for labels to propagate to client applications.

### Personal Email Access
Students must have access to personal email accounts for testing DLP policies and message encryption.

### Single Session Execution
Complete all labs within one RDP session to avoid re-authentication and setup overhead.

### Clear Instructions on Wait Times
Set proper expectations that some configurations require brief propagation periods.

---

## Modified Lab Guide Updates Required

### Lab 04 Modifications

**Original:** "Create multiple folders and classify various files"  
**Streamlined:** "Create one Test folder with 2-3 documents for classification"

**Addition:** Include brief 5-minute demonstration of sensitivity label application in Word document at end of Lab 04.

### Lab 06 Enhancement

**Addition:** Emphasize that students should attempt to send 4-5 test emails to trigger multiple alerts for richer learning experience.

**Addition:** Include section on reviewing aggregated alerts rather than individual alert investigation.

---

## Instructor Notes

### Timing Guidance

**Lab 01:** 25-30 minutes
- Label creation: 10 minutes per label
- Configuration review: 5 minutes

**Lab 02:** 25-30 minutes
- Policy configuration: 15 minutes
- Publishing and verification: 10 minutes

**Lab 04:** 25-30 minutes
- Client installation: 10 minutes
- File classification: 10 minutes
- M365 demonstration: 5-10 minutes

**Lab 06:** 50-60 minutes
- DLP policy creation: 25 minutes
- Alert policy setup: 10 minutes
- Testing and validation: 15-20 minutes
- Alert review: 5-10 minutes

### Common Issues and Solutions

**Issue:** Labels not appearing in File Explorer  
**Solution:** Wait 5-10 additional minutes, restart File Explorer, or sign out/in from Microsoft 365

**Issue:** DLP policy not triggering  
**Solution:** Verify credit card number format is correct, ensure policy is enabled, check that email contains sensitive data in body not just attachment

**Issue:** Cannot access personal email during lab  
**Solution:** Have students use temporary email service or instructor provides test accounts

---

## Alternative Lab Configurations

### For 2-Hour Duration (If Needed)

**Option 1: Skip Lab 04**
- Focus only on policy creation and testing
- Duration: Lab 01 (30) + Lab 02 (30) + Lab 06 (60) = 120 minutes

**Option 2: Simplify Each Lab**
- Create only one sensitivity label in Lab 01
- Reduce DLP testing to 2-3 email attempts instead of 4-5
- Skip alert policy configuration in Lab 06

### For 3-Hour Duration (Extended)

**Option: Add Condensed Lab 05**
- After Lab 04, add 30-minute session on M365 app labeling
- Focus on Word and Outlook label application
- Demonstrate label inheritance when replying to encrypted emails
- Total: 180 minutes

---

## Excluded Content Justification

### Lab 03: Message Encryption

**Primary Reason:** Redundant with Lab 01 encryption settings  
**Secondary Reason:** External email testing adds unnecessary complexity  
**Time Saved:** 60 minutes

**Coverage Alternative:** Brief mention during Lab 01 when configuring encryption settings for sensitivity labels.

### Lab 05: M365 Apps Labeling

**Primary Reason:** Duplicates Lab 04 classification concepts  
**Secondary Reason:** Manual label application already demonstrated  
**Time Saved:** 30 minutes

**Coverage Alternative:** 5-minute demonstration at end of Lab 04 showing Word label application.

### Lab 07: Phishing Simulation

**Primary Reason:** Not core data protection functionality  
**Secondary Reason:** Focuses on security awareness, not data governance  
**Time Saved:** 60 minutes

**Rationale:** While valuable, this belongs in a security awareness training program rather than data protection/governance workshop.

### Labs 08-09: Insider Risk Management

**Primary Reason:** Requires 24-48 hours for data collection  
**Secondary Reason:** Cannot demonstrate real investigation without actual activity data  
**Time Saved:** 120 minutes

**Timing Reality:** Lab guide explicitly states activities take 24 hours to reflect, making these labs impossible to complete meaningfully in a short workshop.

---

## Key Benefits of Streamlined Approach

### Time Efficiency
Reduces 6-7 hour lab to 2.5-3 hours while preserving core learning objectives.

### Focused Learning
Concentrates on essential data protection capabilities: classification, labeling, and DLP.

### Immediate Validation
All included labs provide immediate feedback and validation within the session timeframe.

### Practical Skills
Students gain directly applicable skills for real-world Microsoft Purview implementation.

### Complete Flow
Maintains logical progression from label creation through policy testing and validation.

---

## Conclusion

This streamlined lab structure delivers comprehensive hands-on experience with Microsoft Purview data security capabilities within a 2-3 hour timeframe. By focusing on the essential components of data classification, sensitivity labeling, and data loss prevention, students gain practical skills that are immediately applicable to organizational data protection initiatives.

The removed labs (03, 05, 07, 08, 09) can be offered as advanced or extended workshops for students seeking deeper expertise in specific areas such as insider risk management or security awareness training.

---

**Document Version:** 1.0  
**Last Updated:** November 12, 2025  
**Recommended for:** Instructor-led training with 2-3 hour time constraints  
**Target Audience:** IT administrators, compliance officers, security professionals
