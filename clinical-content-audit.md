# Clinical Content Audit - Blood Gas Pro

**Document Purpose:** Peer review of all clinical/medical content in the application
**Source File:** `/Users/scottsantinon/clinical-apps/ABG/index.html`
**Extraction Date:** 2026-02-02

---

## 1. REFERENCE RANGES & THRESHOLDS

| Parameter | Value | Interpretation | Line # | Verified |
|-----------|-------|----------------|--------|----------|
| pH | < 7.35 | Acidaemia | ~2021 | [ ] |
| pH | > 7.45 | Alkalaemia | ~2021 | [ ] |
| pH | 7.35-7.45 | Normal | ~2021 | [ ] |
| pCO₂ | < 35 mmHg | Low/Hyperventilation | ~2021, 3350 | [ ] |
| pCO₂ | > 45 mmHg | High/Hypoventilation | ~2021, 3350 | [ ] |
| pCO₂ | 35-45 mmHg | Normal | ~3909 | [ ] |
| HCO₃ | < 22 mmol/L | Low | ~1694, 2092 | [ ] |
| HCO₃ | > 26 mmol/L | High | ~1695, 2092 | [ ] |
| HCO₃ | 22-26 mmol/L | Normal | ~2038-2044 | [ ] |
| Anion Gap (corrected) | > 12 mEq/L | Elevated (HAGMA) | ~2018 | [ ] |
| Osmolar Gap | < 10 mOsm/kg | Normal | ~4135, 4609 | [ ] |
| Osmolar Gap | > 10 mOsm/kg | Elevated | ~4393, 4610 | [ ] |
| SID (Strong Ion Difference) | 42-48 mEq/L | Normal | ~3019 | [ ] |
| SID | < 42 | Low (acidosis contributor) | ~3019 | [ ] |
| SID | > 48 | High (alkalosis contributor) | ~3019 | [ ] |
| ATOT | 10-15 mmol/L | Normal | ~3027 | [ ] |
| ATOT | < 10 | Low (alkalinizing) | ~3027 | [ ] |
| ATOT | > 15 | High (acidifying) | ~3027 | [ ] |
| Urine Anion Gap | < 0 | Suggests GI loss | ~5913-5923 | [ ] |
| Urine Anion Gap | > 0 | Suggests renal cause (RTA) | ~5938-5943 | [ ] |
| Corrected Chloride | ≤ 106 mmol/L | Normal | ~5827 | [ ] |
| Corrected Chloride | > 106 mmol/L | Hyperchloraemic | ~5827 | [ ] |
| Spot Urine Chloride | < 20 mmol/L | Chloride-responsive alkalosis | ~6432 | [ ] |
| Spot Urine Chloride | > 20 mmol/L | Chloride-resistant | ~6449 | [ ] |
| Delta Ratio | < 0.4 | Concurrent NAGMA | ~2372 | [ ] |
| Delta Ratio | 0.4-0.8 | Mixed HAGMA + NAGMA | ~2372 | [ ] |
| Delta Ratio | 0.8-2 | Pure HAGMA | ~2372 | [ ] |
| Delta Ratio | > 2 | Concurrent met alkalosis or chronic resp acidosis | ~2372 | [ ] |

---

## 2. FORMULAS & CALCULATIONS

### Winter's Formula (Respiratory Compensation for Metabolic Acidosis)

| Component | Formula | Notes | Line # | Verified |
|-----------|---------|-------|--------|----------|
| Expected pCO₂ | 1.5 × [HCO₃] + 8 (±2) | Pure metabolic acidosis with HCO₃ < 22 | ~2195 | [ ] |
| Floor | ~10 mmHg | Maximal respiratory compensation | ~2197 | [ ] |
| Ceiling | ~55 mmHg | Exceeds usual compensatory limit | ~2204 | [ ] |

### Metabolic Alkalosis Compensation

| Formula | When Applied | Line # | Verified |
|---------|--------------|--------|----------|
| Expected pCO₂ = 0.7 × [HCO₃] + 21 (±5) | Pure metabolic alkalosis | ~2238 | [ ] |

### Metabolic Compensation for Respiratory Disorders

| Disorder | Timing | Formula | Tolerance | Line # | Verified |
|----------|--------|---------|-----------|--------|----------|
| Resp Acidosis | Acute | Expected HCO₃ = 24 + (1 × ΔpCO₂/10) | ±3 | ~1797, 2232 | [ ] |
| Resp Acidosis | Chronic | Expected HCO₃ = 24 + (4 × ΔpCO₂/10) | ±3 | ~1798, 2232 | [ ] |
| Resp Alkalosis | Acute | Expected HCO₃ = 24 - (2 × ΔpCO₂/10) | ±3 | ~1801, 2232 | [ ] |
| Resp Alkalosis | Chronic | Expected HCO₃ = 24 - (5 × ΔpCO₂/10) | ±3 | ~1802, 2232 | [ ] |
| HCO₃ ceiling | — | ~45 mmol/L | — | ~2213-2214 | [ ] |
| HCO₃ floor | — | ~12 mmol/L | — | ~2220-2221 | [ ] |

### Anion Gap Calculations

| Component | Formula | Line # | Verified |
|-----------|---------|--------|----------|
| Raw AG | Na - (Cl + HCO₃) | ~2015 | [ ] |
| Albumin Correction | (4.0 - [Albumin]) × 2.5 | ~2017 | [ ] |
| Corrected AG | Raw AG + Albumin correction | ~2017 | [ ] |
| HAGMA threshold | Corrected AG > 12 mEq/L | ~2018 | [ ] |

### Delta Ratio

| Component | Formula | Line # | Verified |
|-----------|---------|--------|----------|
| ΔAG | Corrected AG - 12 | ~2370 | [ ] |
| ΔHCO₃ | 24 - [HCO₃] | ~2370 | [ ] |
| Delta Ratio | ΔAG / ΔHCO₃ | ~2370 | [ ] |

### Stewart Physicochemical Parameters

| Parameter | Formula | Line # | Verified |
|-----------|---------|--------|----------|
| SIDa | (Na + K + 2×Ca + 2×Mg) - (Cl + Lactate) | ~3725 | [ ] |
| ATOT | Albumin charge + Phosphate charge | ~3785 | [ ] |
| Albumin charge | (0.123 × pH - 0.631) × [Albumin] | ~3785 | [ ] |
| Phosphate charge | (0.309 × pH - 0.469) × [Phosphate] | ~3785 | [ ] |
| SIG | SIDa - ATOT - HCO₃ | Stewart analysis | [ ] |

### Osmolar Gap

| Component | Formula | Line # | Verified |
|-----------|---------|--------|----------|
| Calculated Osm | (2 × Na) + Glucose + Urea | ~4130, 4391 | [ ] |
| Osmolar Gap | Measured Osm - Calculated Osm | ~4130 | [ ] |
| Normal | < 10 mOsm/kg | ~4609 | [ ] |

### P/F Ratio

| Component | Formula | Line # | Verified |
|-----------|---------|--------|----------|
| P/F Ratio | pO₂ (mmHg) / FiO₂ | ~8550 | [ ] |

---

## 3. DIFFERENTIAL DIAGNOSIS LISTS

### HAGMA Causes (High Anion Gap Metabolic Acidosis)

**Common Measured Anions:**
- [ ] Lactate (shock, hypoxia, sepsis, drugs) — Line ~4675
- [ ] Ketoacids (DKA, starvation, alcoholic) — Line ~4675

**Unmeasured Anions:**
- [ ] Uraemia (renal failure) — Line ~9684
- [ ] Toxic alcohols (methanol, ethylene glycol) — Line ~9684
- [ ] Salicylate overdose — Line ~9684
- [ ] Pyroglutamic acidosis — Line ~9684
- [ ] D-lactate — Line ~9684

### Lactic Acidosis Differential

**Type A — Tissue Hypoxia:**
- [ ] Hypoxaemia — Line ~9740
- [ ] Cardiogenic shock / low cardiac output
- [ ] Hypovolaemic shock
- [ ] Severe anaemia
- [ ] Regional ischaemia (mesenteric, limb)
- [ ] Carbon monoxide poisoning
- [ ] Methaemoglobinaemia

**Type B — Metabolic:**
- [ ] Diabetic ketoacidosis — Line ~9745
- [ ] Thiamine deficiency (beriberi)
- [ ] Liver failure
- [ ] Sepsis
- [ ] Malignancy
- [ ] Inborn errors of metabolism

**Drugs & Toxins:**
- [ ] Metformin — Line ~9747
- [ ] Nucleoside reverse transcriptase inhibitors
- [ ] Propofol infusion syndrome
- [ ] Adrenaline / salbutamol
- [ ] Cyanide
- [ ] Toxic alcohols
- [ ] Paracetamol overdose
- [ ] Salicylates

**Other:**
- [ ] Seizures — Line ~9748
- [ ] Strenuous exercise
- [ ] Beta-2 agonism

### NAGMA Causes (Normal Anion Gap Metabolic Acidosis)

**GI Bicarbonate Loss:**
- [ ] Diarrhoea / fistulae / high-output ileostomy — Line ~9686

**Renal Tubular Acidosis:**
- [ ] RTA Type 1 (distal) — urine pH >5.5, hypokalaemia — Line ~9690
- [ ] RTA Type 2 (proximal) — urine pH variable, hypokalaemia
- [ ] RTA Type 4 (hyperkalaemic) — urine pH <5.5, hyperkalaemia

**Chloride Excess:**
- [ ] 0.9% saline infusion — Line ~9695
- [ ] TPN
- [ ] Hyperchloraemia

**Other:**
- [ ] Early renal failure — Line ~9698
- [ ] Post-DKA (recovery phase)
- [ ] Ureteric diversion (ileal conduit)

### RTA Type Classification

**RTA Type 1 (Distal):**
- [ ] Cannot secrete H⁺ in collecting duct — Line ~6110
- [ ] Urine pH: >5.5 (inappropriately alkaline)
- [ ] Serum K⁺: LOW
- [ ] Causes: Sjögren's, SLE, amphotericin B, lithium, nephrocalcinosis
- [ ] Complications: Kidney stones, osteomalacia

**RTA Type 2 (Proximal):**
- [ ] Cannot reabsorb HCO₃⁻ in proximal tubule — Line ~6150
- [ ] Urine pH: Variable (can be <5.5 when serum HCO₃ low)
- [ ] Serum K⁺: LOW
- [ ] Causes: Fanconi syndrome, myeloma, acetazolamide, tenofovir
- [ ] Features: Often has glucosuria, phosphaturia, aminoaciduria

**RTA Type 4 (Hyperkalaemic):**
- [ ] Aldosterone deficiency or resistance — Line ~6072
- [ ] Urine pH: <5.5 (appropriately acidic)
- [ ] Serum K⁺: HIGH (>5.0 mmol/L)
- [ ] Causes: Diabetic nephropathy, ACEi/ARB, spironolactone, Addison's, trimethoprim

### Metabolic Alkalosis Causes

**Loss of H⁺ from GIT:**
- [ ] Vomiting / NG suction — Line ~9702

**Loss of H⁺ from Kidneys:**
- [ ] Loop or thiazide diuretics — Line ~9705
- [ ] Mineralocorticoid excess (Conn's, Cushing's, steroids)

**Gain of HCO₃⁻:**
- [ ] NaHCO₃ administration — Line ~9708
- [ ] Citrate (CRRT, massive transfusion)

**Other:**
- [ ] Severe hypokalaemia (intracellular H⁺ shift) — Line ~9712
- [ ] Volume depletion (contraction alkalosis)
- [ ] Post-hypercapnia

### Respiratory Acidosis Causes

**Reduced Central Drive:**
- [ ] Opioids / sedatives / anaesthesia — Line ~9716
- [ ] OHS / brainstem pathology
- [ ] Severe hypothyroidism

**Neuromuscular Weakness:**
- [ ] Guillain-Barré syndrome — Line ~9718
- [ ] Myasthenia gravis
- [ ] Motor neurone disease
- [ ] Critical illness myopathy
- [ ] Spinal cord injury

**Chest Wall / Pleural:**
- [ ] Flail chest — Line ~9720
- [ ] Kyphoscoliosis
- [ ] Large pleural effusion
- [ ] Tension pneumothorax

**Airways / Parenchyma:**
- [ ] COPD exacerbation — Line ~9722
- [ ] Severe asthma
- [ ] Severe pneumonia
- [ ] ARDS (late/severe)

**Iatrogenic:**
- [ ] Inadequate mechanical ventilation — Line ~9724
- [ ] Permissive hypercapnia

### Respiratory Alkalosis Causes

**Hypoxaemia-Driven:**
- [ ] Pneumonia — Line ~9727
- [ ] Pulmonary embolism
- [ ] Pulmonary oedema
- [ ] Interstitial lung disease
- [ ] High altitude
- [ ] Severe anaemia

**Central Stimulation:**
- [ ] Pain / anxiety / panic — Line ~9730
- [ ] Sepsis / fever
- [ ] CNS pathology (stroke, infection, tumour)

**Hormonal / Metabolic:**
- [ ] Hepatic encephalopathy — Line ~9733
- [ ] Pregnancy (progesterone)
- [ ] Hyperthyroidism

**Drugs:**
- [ ] Salicylates (early) — Line ~9735
- [ ] Progesterone
- [ ] Catecholamines

**Iatrogenic:**
- [ ] Mechanical overventilation — Line ~9737

---

## 4. INFO BUTTON / EDUCATIONAL CONTENT

### Delta Ratio Explanation

**Location:** ~Line 2974-2982

**Text:**
> "The delta ratio (ΔAG/ΔHCO₃) helps identify additional acid-base disorders hidden within a HAGMA."

**Interpretation Ranges:**
- [ ] <0.4 — Concurrent NAGMA
- [ ] 0.4–0.8 — Mixed HAGMA + NAGMA
- [ ] 0.8–2 — Pure HAGMA
- [ ] >2 — Concurrent met alkalosis or chronic resp acidosis

### VBG Limitations Warning

**Location:** ~Line 2624, 2966

**Text:**
> "⚠️ VBG: compensation assessment may be inaccurate"
>
> "Venous pCO₂ is typically 3-8 mmHg higher than arterial, but this difference is unpredictable in critical illness."
>
> "The compensation assessment above uses your entered pCO₂ value in formulas designed for arterial samples. Consider ABG if respiratory status is critical to management."

### Post-DKA Recovery NAGMA

**Location:** ~Line 6180-6247

**Text:**
> "It is common for patients recovering from DKA to develop a transient NAGMA. This is expected and usually resolves within 24-48 hours."

**Mechanism 1 - Ketone metabolism:**
> "Ketoacids (β-hydroxybutyrate) are metabolised to bicarbonate, but this takes time. Meanwhile, the measured anion gap normalises faster than the bicarbonate rises."

**Mechanism 2 - Saline resuscitation:**
> "Large volumes of 0.9% saline (Cl⁻ 154 mmol/L) cause dilutional hyperchloraemia, lowering the anion gap while maintaining acidosis."

**Mechanism 3 - Urinary ketone loss:**
> "Ketones excreted in urine represent 'lost' potential bicarbonate that cannot be regenerated."

**Clinical Implications:**
- [ ] Usually self-limiting — resolves as kidneys regenerate HCO₃⁻
- [ ] Continue IV fluids; consider switching to balanced crystalloid
- [ ] Avoid excessive saline if hyperchloraemia is significant
- [ ] No specific treatment required if patient improving clinically

### SID (Strong Ion Difference) Explanation

**Location:** ~Line 3686-3725

**Text:**
> "SIDa = (Na⁺ + K⁺ + 2×Ca²⁺ + 2×Mg²⁺) − (Cl⁻ + Lactate)"
>
> Normal Range: 42-48 mEq/L
>
> - Low SID → Low pH (acidosis)
> - High SID → High pH (alkalosis)

### ATOT Explanation

**Location:** ~Line 3737-3785

**Text:**
> "ATOT = Albumin charge + Phosphate charge"
>
> Formula: Charge = (0.123 × pH - 0.631) × [Albumin] + (0.309 × pH - 0.469) × [Phosphate]
>
> Normal Range: 10-15 mmol/L
>
> - Low ATOT → Less acid load → alkalosis
> - High ATOT → More acid load → acidosis

### Osmolar Gap Explanation

**Location:** ~Line 4407-4412

**Text:**
> "What is the osmolar gap? The difference between measured and calculated osmolality. Detects unmeasured osmotically active substances."
>
> Normal: < 10 mOsm/kg

### Toxic Alcohol Timeline

**Location:** ~Line 4204

**Text:**
> - **Early Phase:** "non-polar, not yet metabolised → ↑OG only"
> - **Middle Phase:** "partially metabolised to organic acids → ↑OG and ↑AG"
> - **Late Phase:** "fully metabolised → ↑AG, normal OG"

### Toxic Alcohols Clinical Information

**Location:** ~Line 5379-5401

**Text:**
> "Methanol and ethylene glycol cause severe HAGMA through toxic metabolites (formic acid, glycolic/oxalic acid)"
>
> **Osmolar gap timing:** "Elevated early (parent compound present) → normal late (after metabolism). A normal osmolar gap does NOT exclude toxic alcohol if presentation is delayed."
>
> **Clinical clues:** "History of ingestion, visual symptoms (methanol), flank pain/haematuria (ethylene glycol), profound acidosis"
>
> **Management:** "Urgent — fomepizole/ethanol, haemodialysis. Contact toxicology."

### D-Lactate

**Location:** ~Line 5301-5323

**Text:**
> "D-lactate is produced by gut bacteria and not detected by standard L-lactate assays."
>
> **When to Suspect:** "Short bowel syndrome, jejunoileal bypass, or other conditions with bacterial overgrowth in a blind loop."
>
> **Clinical Features:** "Episodic encephalopathy, ataxia, slurred speech — often after high-carbohydrate meals."
>
> **Diagnosis:** "Request specific D-lactate assay (not routine)."

### Pyroglutamic Acidosis

**Location:** ~Line 5350-5375

**Text:**
> "5-oxoproline (pyroglutamic acid) accumulation causes HAGMA, often unrecognised."
>
> **Risk Factors:** "Chronic paracetamol use + malnutrition/sepsis/renal impairment. Glutathione depletion disrupts the γ-glutamyl cycle."
>
> **Clinical Clues:** "Elderly female, chronic paracetamol (even therapeutic doses), poor nutrition, unexplained HAGMA."

### Uraemic Acidosis

**Location:** ~Line 5325-5349

**Text:**
> "Renal failure causes HAGMA through retention of organic acids normally excreted by the kidneys."
>
> **Unmeasured Anions:** "Sulphates, phosphates, urate, and hippurate accumulate as GFR declines."
>
> **Clinical Context:** "Usually significant only when GFR <15-20 mL/min. Check creatinine/eGFR. May coexist with other causes of HAGMA."

### UAG (Urine Anion Gap) Explanation

**Location:** ~Line 5866-5966

**Formula:** UAG = Urine Na + Urine K − Urine Cl

**Interpretation:**
- [ ] Negative UAG → GI loss (diarrhoea) — "Kidneys responding normally with ↑NH₄⁺"
- [ ] Positive UAG → Renal cause (RTA) — "Impaired renal NH₄⁺ excretion"

**Caveat:** "⚠️ UAG is unreliable if urine ketones are present — ketonuria causes false positive UAG."

### Volume Depletion / Contraction Alkalosis

**Location:** ~Line 6507-6532

**Text:**
> "When ECF volume contracts (vomiting, diuretics, dehydration), the existing HCO₃⁻ pool becomes concentrated in a smaller volume, raising [HCO₃⁻]. Additionally, loss of Cl⁻-rich fluid directly increases [HCO₃⁻] to maintain electroneutrality."

**Maintenance Mechanisms:**
> - ↑ Proximal tubule Na⁺/HCO₃⁻ co-reabsorption (avid Na⁺ retention)
> - ↓ GFR reduces the filtered HCO₃⁻ load available for excretion
> - ↑ Aldosterone → ↑ distal H⁺ secretion → generates new HCO₃⁻
> - Hypokalaemia (common) shifts H⁺ into cells and ↑ renal H⁺ secretion
> - Cl⁻ depletion limits ability to excrete HCO₃⁻

**Clinical Clue:** "Urine Cl⁻ <20 mmol/L indicates a 'chloride-responsive' alkalosis"

### Lactate Gap Clinical Pearl

**Location:** ~Line 4311-4315

**Text:**
> "If POC lactate − Lab lactate >5, suspect ethylene glycol poisoning (POC assay cross-reacts with glycolate)."

---

## 5. INTERPRETIVE LABELS & BADGES

### Primary Disorder Labels

| Label | Criteria | Line # | Verified |
|-------|----------|--------|----------|
| Respiratory acidosis | pH < 7.35 AND pCO₂ > 45 | ~2102 | [ ] |
| Metabolic acidosis | pH < 7.35 AND HCO₃ < 22 | ~2106 | [ ] |
| Respiratory alkalosis | pH > 7.45 AND pCO₂ < 35 | ~2126 | [ ] |
| Metabolic alkalosis | pH > 7.45 AND HCO₃ > 26 | ~2129 | [ ] |
| HAGMA (with normal pH) | Normal pH AND AG > 12 | ~2149 | [ ] |
| No acid-base disturbance | pH 7.35-7.45, HCO₃ 22-26, pCO₂ 35-45 | ~2044 | [ ] |

### Compensation Verdicts

| Verdict | Meaning | Line # | Verified |
|---------|---------|--------|----------|
| Appropriate compensation | Values fit expected formulas | ~2259 | [ ] |
| Outside expected range | Values deviate from expected | ~2281 | [ ] |
| Additional respiratory acidosis | Excess pCO₂ retention | ~2284 | [ ] |
| Additional respiratory alkalosis | Excess pCO₂ reduction | ~2288 | [ ] |
| Additional metabolic acidosis | Excess HCO₃ loss | ~2342 | [ ] |
| Additional metabolic alkalosis | Excess HCO₃ elevation | ~2338 | [ ] |
| Metabolic alkalosis component | For Pathway B with normal pCO₂ | ~2215 | [ ] |
| Mixed metabolic disorder | Multiple metabolic processes | ~2217 | [ ] |
| Consistent with chronic OR acute mixed | DualInterpretationCard | ~1718 | [ ] |
| Consistent with acute process | DualInterpretationCard | ~1721 | [ ] |

### Delta Ratio Interpretation Labels

| Label | Delta Ratio | Line # | Verified |
|-------|-------------|--------|----------|
| Concurrent NAGMA | < 0.4 | ~2372 | [ ] |
| Mixed HAGMA + NAGMA | 0.4-0.8 | ~2372 | [ ] |
| Pure HAGMA | 0.8-2 | ~2372 | [ ] |
| ↑HCO₃ component | > 2 | ~2372 | [ ] |
| See below ↓ | Pending chronic hypercapnia question | ~2580 | [ ] |
| Chronic compensation | After user selects "Yes" | ~2580 | [ ] |
| Additional met alkalosis | After user selects "No" | ~2580 | [ ] |

### pH Status Labels

| Status | pH Range | Line # | Verified |
|--------|----------|--------|----------|
| Acidaemia | < 7.35 | ~2021 | [ ] |
| Alkalaemia | > 7.45 | ~2021 | [ ] |
| Normal | 7.35-7.45 | ~2021 | [ ] |

### Stewart Analysis Labels

| Parameter | Status | Meaning | Line # | Verified |
|-----------|--------|---------|--------|----------|
| SIDa | Low | Contributes to acidosis | ~3269 | [ ] |
| SIDa | High | Contributes to alkalosis | ~3269 | [ ] |
| ATOT | Low | Alkalinizing effect | ~3310 | [ ] |
| ATOT | High | Acidifying effect | ~3310 | [ ] |
| pCO₂ | ↑ Respiratory acidosis | High pCO₂ | ~3350 | [ ] |
| pCO₂ | ↓ Respiratory alkalosis | Low pCO₂ | ~3350 | [ ] |

### Osmolar Gap Interpretation

| OG + AG Status | Interpretation | Line # | Verified |
|----------------|----------------|--------|----------|
| ↑OG + ↑AG | Toxic alcohol (mid-stage), salicylate, severe lactic acidosis | ~4152 | [ ] |
| ↑OG + normal AG | Toxic alcohol (early), ethanol, mannitol, glycine | ~4163 | [ ] |
| normal OG + ↑AG | Toxic alcohol (late), ketoacidosis, lactic acidosis, uraemia | ~4175 | [ ] |

---

## 6. CLINICAL RECOMMENDATIONS

### HAGMA Investigation

**When lactate elevated (>2 mmol/L):**
- [ ] Review lactic acidosis differential — Line ~5496
- [ ] Consider tissue hypoxia, sepsis, liver failure, drugs/toxins

**When ketones elevated (>0.6 mmol/L):**
- [ ] Review ketoacidosis differential — Line ~5564
- [ ] Consider DKA, starvation ketosis, alcoholic ketoacidosis

**When unexplained anions remain (>2 mEq/L):**
- [ ] Consider renal failure, pyroglutamic acidosis, D-lactate, salicylate — Line ~5290
- [ ] Calculate osmolar gap to assess for toxic alcohols

**Osmolar Gap for Toxic Alcohol:**
- [ ] OG >10 + high AG → toxic alcohol mid-stage
- [ ] OG >10 + normal AG → toxic alcohol early stage
- [ ] OG normal + high AG → late-stage toxic alcohol (fully metabolised)

### NAGMA Differentiation

**GI vs Renal Cause - Use UAG:**
- [ ] Calculate UAG = Urine Na + Urine K − Urine Cl — Line ~5866
- [ ] Negative UAG → GI loss
- [ ] Positive UAG → Renal cause/RTA
- [ ] Note: UAG unreliable if ketonuria present

**RTA Type - Check serum K⁺:**
- [ ] High K⁺ → Type 4 RTA
- [ ] Low K⁺ + urine pH >5.5 → Type 1 RTA
- [ ] Low K⁺ + urine pH variable → Type 2 RTA

### Respiratory Alkalosis

**If hypoxaemic:**
- [ ] Respiratory alkalosis may be appropriate compensation — Line ~6831
- [ ] Investigate underlying pulmonary pathology

**If normoxic:**
- [ ] Look for central causes (anxiety, pain, CNS, sepsis)

---

## 7. WARNINGS & CAVEATS

### VBG Limitations

**Location:** ~Line 2624, 2966

**Text:**
> "⚠️ VBG: compensation assessment may be inaccurate"
>
> "Consider ABG if respiratory status is critical to management."

**Clinical Implication:** Compensation formulas are derived from arterial samples.

- [ ] Verified

### Osmolar Gap Limitations

**Location:** ~Line 5397

**Text:**
> "A normal osmolar gap does NOT exclude toxic alcohol if presentation is delayed."

**Explanation:** In late presentations, parent compound is fully metabolized.

- [ ] Verified

### UAG Unreliability with Ketonuria

**Location:** ~Line 5966

**Text:**
> "⚠️ UAG is unreliable if urine ketones are present — ketonuria causes false positive UAG."

- [ ] Verified

### Compensation Formula Limitations for Pathway B

**Location:** ~Line 2295-2310

**Text:**
> "For Pathway B (HAGMA with normal pH) and normal HCO₃, don't apply standard compensation formulas. The normal pH indicates metabolic alkalosis is offsetting the HAGMA, not respiratory compensation."

- [ ] Verified

### Post-DKA NAGMA is Expected

**Location:** ~Line 6190, 6247

**Text:**
> "This is an expected finding during DKA recovery and does NOT necessarily indicate a new problem."

- [ ] Verified

### Medical Liability Disclaimers

**Location:** ~Line 9501-9625

- [ ] "This application is NOT a medical device"
- [ ] "Educational and informational purposes only"
- [ ] "Does NOT provide medical advice, diagnosis, or treatment"
- [ ] "Healthcare professionals remain solely responsible for all clinical decisions"
- [ ] "DO NOT USE IN EMERGENCIES"

---

## SUMMARY STATISTICS

| Category | Count |
|----------|-------|
| Reference Range Values | 28 |
| Formulas Documented | 15+ |
| Differential Diagnosis Categories | 7 |
| Info/Educational Sections | 16 |
| Clinical Recommendations | 15+ |
| Warnings/Caveats | 8 |
| Interpretive Labels | 30+ |

---

**Document prepared for clinical peer review**
**Source:** `/Users/scottsantinon/clinical-apps/ABG/index.html`
**Extraction Date:** 2026-02-02
