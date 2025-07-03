---
layout: default
title: Home
---

# Oncology Treatment Switch Workstream

This workstream addresses a major challenge in oncology clinical trials: the impact of treatment switching on long-term outcomes. We develop, validate, and promote statistical methods that properly adjust for treatment switching while maintaining scientific rigor.

## Overview

When patients switch from their assigned treatment to another therapy (often due to disease progression or safety concerns), traditional intent-to-treat analyses may not provide the most relevant estimates of treatment efficacy. Our workstream tackles this challenge through:

<div class="card-grid">
  <div class="card">
    <h3><i class="fas fa-calculator"></i> Statistical Methods</h3>
    <p>Development of advanced statistical approaches including RPSFT, IPE, IPCW, TSE, and MSM methods for handling treatment switching scenarios.</p>
  </div>
  
  <div class="card">
    <h3><i class="fas fa-check-circle"></i> Rigorous Validation</h3>
    <p>Comprehensive validation studies ensuring our methods produce reliable, accurate results across multiple datasets and scenarios.</p>
  </div>
  
  <div class="card">
    <h3><i class="fas fa-code"></i> Open Source Tools</h3>
    <p>Development of the trtswitch R package - a comprehensive, validated toolkit for treatment switching analysis.</p>
  </div>
  
  <div class="card">
    <h3><i class="fas fa-users"></i> Collaboration</h3>
    <p>Bringing together statisticians, clinicians, and regulatory experts to advance the science of treatment switching.</p>
  </div>
</div>

## Recent Achievements

### Test 6 Validation Completed
**June 2025** - Our latest validation study demonstrates excellent agreement between `trtswitch::rpsftm()` and reference implementations:

- **psi parameter:** Difference < 0.02%
- **Hazard ratios:** Agreement to 4 decimal places  
- **p-values:** Within 0.004 units
- **Event indicators:** 100% concordance

### Cross-Dataset Validation Framework
**May 2025** - Established comprehensive validation approach across multiple datasets (shilong and immdef), strengthening confidence in our methodological implementations.

### Two-Way Switch Investigation
**April 2025** - Identified areas for improvement in two-way switching scenarios, enhancing our understanding of method limitations and future development needs.

## trtswitch R Package

Our flagship deliverable is a comprehensive R package that provides validated implementations of multiple treatment switching methods.

### Installation

```r
# Install from GitHub
devtools::install_github("ShreyaSreeram27/trtswitch")

# Load the package
library(trtswitch)

# Explore example datasets
data(shilong)
data(immdef)
