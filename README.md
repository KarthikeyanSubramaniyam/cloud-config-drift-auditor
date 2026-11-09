# Multi-Cloud Configuration Drift & Compliance Auditor

<p align="center">
  <img src="https://img.shields.io/badge/Security-Defensive_Auditor-blue?style=flat" alt="Type">
  <img src="https://img.shields.io/badge/Status-Architectural_Showcase-success?style=flat" alt="Status">
  <img src="https://img.shields.io/badge/Python-3.10+-3776AB?style=flat&logo=python&logoColor=white" alt="Python">
</p>

> 🔒 **Technical Showcase & Architecture Specification**  
> *This repository provides public architectural documentation, system specifications, and implementation summaries. Full production source code, internal test suites, and proprietary algorithms are maintained in a secure private repository.*

---

## 📌 Executive Summary

**Category**: Cloud Governance & Compliance  
**Tech Stack**: `Python 3.10+ · CIS Benchmarks · Configuration Drift · Compliance Engine`  

Continuous compliance engine comparing live cloud infrastructure states against hardened CIS Benchmark baselines to detect configuration degradation.

---

## 🎯 The Problem It Solves

Over time, ad-hoc operational changes, manual console tweaks, and automated scripts cause cloud infrastructure to drift from hardened security baselines.

---

## ⚙️ How the Engine Works

1. **Hardened Baseline Ingestion**: Loads standardized CIS Benchmark and corporate configuration profiles defining expected settings for storage, compute, identity, and networking.
2. **Observed State Ingestion**: Ingests current multi-cloud resource configurations.
3. **Delta Computation Engine**: Computes granular property-level differences between baseline and observed states.
4. **Risk Categorization**: Categorizes drift events into benign operational variance vs. critical security degradations.
5. **Automated Remediation Guidance**: Generates IaC drift reconciliation scripts (Terraform/CLI) to restore compliance.

---

## 🚀 Key Capabilities

- Audits cloud configurations against CIS Benchmark baselines
- Detects unauthorized manual modifications and security control degradation
- Computes automated compliance percentages across resource types
- Emits remediation CLI commands to restore hardened configurations

---

## 🏗️ System Data Flow & Architecture

```
+-----------------------------------+
|  Target Input / Configuration    |
|  (JSON Snapshots / Policies)      |
+-----------------+-----------------+
                  |
                  v
+-----------------------------------+
|  1. Schema Normalization Engine   |
|  Validates types & formats        |
+-----------------+-----------------+
                  |
                  v
+-----------------------------------+
|  2. Core Analytical Pipeline      |
|  Heuristic rule evaluation,       |
|  invariant checks & drift diffs   |
+-----------------+-----------------+
                  |
                  v
+-----------------------------------+
|  3. Risk Classification           |
|  Assigns severity: INFO / HIGH    |
+-----------------+-----------------+
                  |
                  v
+-----------------------------------+
|  4. Structured Findings & Report  |
|  Root cause, evidence &           |
|  actionable remediation steps     |
+-----------------------------------+
```

---

## 📄 Findings Output Structure

The engine generates structured, machine-parsable JSON reports adhering to this standard audit schema:

```json
{
  "results": [
    {
      "resource": "resource-identifier",
      "severity": "HIGH",
      "check": "CHECK_IDENTIFIER",
      "detail": "Descriptive analysis of the identified security posture issue.",
      "remediation": "Actionable step-by-step guidance to restore compliant state.",
      "evidence": {
        "observed_field": "value",
        "required_policy": "enforced_policy"
      }
    }
  ],
  "count": 1,
  "scope": "Comprehensive defensive security audit"
}
```

---

## 🔒 Source Code & Enterprise Inquiries

To protect proprietary intellectual property and client operational security:
* **Public Repository**: Contains comprehensive architecture specifications, schemas, and design overviews.
* **Private Repository**: Contains the complete production implementation, continuous integration pipelines, and full regression test suites.

For architectural questions or enterprise inquiries, connect via [LinkedIn](https://www.linkedin.com/in/karthikeyansubramaniam04/) or visit the [Portfolio Site](https://karthikeyansubramaniyam.github.io).
