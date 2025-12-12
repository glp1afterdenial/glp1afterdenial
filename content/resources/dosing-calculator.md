---
title: "Semaglutide, Tirzepatide & Retatrutide Dosing Calculator"
date: 2025-12-01
description: "Free calculator for reconstituted peptides. Enter your vial size, BAC water amount, and desired dose — get exact units to draw on your insulin syringe."
keywords: ["semaglutide dosing calculator", "tirzepatide dose calculator", "retatrutide dosing calculator", "peptide reconstitution calculator", "how many units semaglutide"]
---

Use this calculator to figure out your concentration after reconstitution and how many units to draw for your dose.

---

<div id="calculator" style="background: #f8fafc; border-radius: 12px; padding: 24px; margin: 24px 0;">

<h3 style="margin-top: 0;">Step 1: Reconstitution</h3>

<div style="display: grid; gap: 16px; margin-bottom: 24px;">
  <div>
    <label style="display: block; font-weight: 600; margin-bottom: 4px;">Peptide amount in vial (mg)</label>
    <input type="number" id="peptideMg" value="5" min="0.1" step="0.1" style="width: 100%; padding: 10px; border: 1px solid #d1d5db; border-radius: 6px; font-size: 16px;">
    <small style="color: #6b7280;">Common: 5mg or 10mg vials</small>
  </div>
  
  <div>
    <label style="display: block; font-weight: 600; margin-bottom: 4px;">BAC water to add (mL)</label>
    <input type="number" id="waterMl" value="2" min="0.1" step="0.1" style="width: 100%; padding: 10px; border: 1px solid #d1d5db; border-radius: 6px; font-size: 16px;">
    <small style="color: #6b7280;">Common: 1mL or 2mL</small>
  </div>
</div>

<div style="background: #dbeafe; border-radius: 8px; padding: 16px; margin-bottom: 24px;">
  <div style="font-weight: 600; color: #1e40af;">Your Concentration:</div>
  <div style="font-size: 28px; font-weight: 700; color: #1e3a8a;" id="concentration">2.5 mg/mL</div>
</div>

<h3>Step 2: Calculate Your Dose</h3>

<div style="margin-bottom: 16px;">
  <label style="display: block; font-weight: 600; margin-bottom: 4px;">Desired dose (mg)</label>
  <input type="number" id="desiredDose" value="0.25" min="0.01" step="0.01" style="width: 100%; padding: 10px; border: 1px solid #d1d5db; border-radius: 6px; font-size: 16px;">
</div>

<div style="background: #dcfce7; border-radius: 8px; padding: 16px;">
  <div style="font-weight: 600; color: #166534;">Draw this much:</div>
  <div style="font-size: 28px; font-weight: 700; color: #15803d;" id="units">10 units</div>
  <div style="color: #166534;" id="mlAmount">(0.1 mL)</div>
</div>

</div>

<script>
function calculate() {
  const peptideMg = parseFloat(document.getElementById('peptideMg').value) || 0;
  const waterMl = parseFloat(document.getElementById('waterMl').value) || 1;
  const desiredDose = parseFloat(document.getElementById('desiredDose').value) || 0;
  
  // Calculate concentration
  const concentration = peptideMg / waterMl;
  document.getElementById('concentration').textContent = concentration.toFixed(2) + ' mg/mL';
  
  // Calculate units (100 units = 1mL)
  const mlNeeded = desiredDose / concentration;
  const units = mlNeeded * 100;
  
  document.getElementById('units').textContent = Math.round(units) + ' units';
  document.getElementById('mlAmount').textContent = '(' + mlNeeded.toFixed(2) + ' mL)';
}

// Add event listeners
document.getElementById('peptideMg').addEventListener('input', calculate);
document.getElementById('waterMl').addEventListener('input', calculate);
document.getElementById('desiredDose').addEventListener('input', calculate);

// Initial calculation
calculate();
</script>

---

## Quick Reference Tables

### Semaglutide 5mg Vial + 2mL BAC Water (2.5 mg/mL)

| Dose | Units to Draw | Volume |
|------|---------------|--------|
| 0.25mg | 10 units | 0.10 mL |
| 0.5mg | 20 units | 0.20 mL |
| 1.0mg | 40 units | 0.40 mL |
| 1.7mg | 68 units | 0.68 mL |
| 2.0mg | 80 units | 0.80 mL |
| 2.4mg | 96 units | 0.96 mL |

### Semaglutide 5mg Vial + 1mL BAC Water (5 mg/mL)

| Dose | Units to Draw | Volume |
|------|---------------|--------|
| 0.25mg | 5 units | 0.05 mL |
| 0.5mg | 10 units | 0.10 mL |
| 1.0mg | 20 units | 0.20 mL |
| 1.7mg | 34 units | 0.34 mL |
| 2.0mg | 40 units | 0.40 mL |
| 2.4mg | 48 units | 0.48 mL |

### Tirzepatide 10mg Vial + 2mL BAC Water (5 mg/mL)

| Dose | Units to Draw | Volume |
|------|---------------|--------|
| 2.5mg | 50 units | 0.50 mL |
| 5.0mg | 100 units | 1.00 mL |
| 7.5mg | 150 units | 1.50 mL |
| 10mg | 200 units | 2.00 mL |

*Note: For doses above 100 units, you may need a larger syringe or split into two injections.*

### Tirzepatide 10mg Vial + 1mL BAC Water (10 mg/mL)

| Dose | Units to Draw | Volume |
|------|---------------|--------|
| 2.5mg | 25 units | 0.25 mL |
| 5.0mg | 50 units | 0.50 mL |
| 7.5mg | 75 units | 0.75 mL |
| 10mg | 100 units | 1.00 mL |
| 12.5mg | 125 units | 1.25 mL |
| 15mg | 150 units | 1.50 mL |

### Retatrutide 10mg Vial + 2mL BAC Water (5 mg/mL)

| Dose | Units to Draw | Volume |
|------|---------------|--------|
| 2mg | 40 units | 0.40 mL |
| 4mg | 80 units | 0.80 mL |
| 8mg | 160 units | 1.60 mL |
| 12mg | 240 units | 2.40 mL |

*Note: For doses above 100 units, you may need a larger syringe or split into two injections.*

### Retatrutide 10mg Vial + 1mL BAC Water (10 mg/mL)

| Dose | Units to Draw | Volume |
|------|---------------|--------|
| 2mg | 20 units | 0.20 mL |
| 4mg | 40 units | 0.40 mL |
| 8mg | 80 units | 0.80 mL |
| 12mg | 120 units | 1.20 mL |

---

## The Formula

It's simple math once you understand it:

**Concentration:** `peptide (mg) ÷ water (mL) = mg per mL`

**Units to draw:** `desired dose (mg) ÷ concentration (mg/mL) × 100 = units`

### Example

- You have a **5mg vial** of semaglutide
- You add **2mL** of BAC water
- Concentration: 5 ÷ 2 = **2.5 mg/mL**
- You want **0.5mg** dose
- Units: 0.5 ÷ 2.5 × 100 = **20 units**

---

## Tips

- **Less water = more concentrated** (smaller injection volume, but harder to measure small doses accurately)
- **More water = less concentrated** (easier to measure, but larger injection volume)
- **2mL is a good middle ground** for most people
- **Always double-check your math** before injecting
- **Start with lower doses** if you're new to these medications

---

## Supplies You'll Need

- [Bacteriostatic water](https://amzn.to/4rMsIW9)
- [Insulin syringes (29-31 gauge)](https://amzn.to/48NegER)
- [Alcohol swabs](https://amzn.to/4oPJIZ0)
- [Sharps container](https://amzn.to/3MpnU9f)

---

[← Back to Reconstitution Guide](/resources/how-to-reconstitute-peptides/)

---

*Affiliate Disclosure: Some links on this site are affiliate links. If you purchase through them, I may earn a small commission at no extra cost to you. I only recommend products I've personally used or thoroughly researched.*
