# 100x Week 2 — SDXL Image Debugging Assignment

In this assignment, we’ve been given **3 SDXL-generated images** that are corrupted due to 1–2 incorrect parameters.  
Your mission is to act as an **image forensics agent**:  
- Recover the **exact metadata** (prompt, seed, sampler, CFG, steps, etc.).  
- Identify which parameter(s) are wrong.  
- Fix them to recreate the clean version of the image.  

---

## 🎯 Goals
- Learn how to extract and understand **SDXL metadata**.  
- Practice **debugging images** by parameter isolation.  
- Strengthen intuition around how small tweaks affect results.  

---

## 🛠 Tools
Use **[pngchunk](https://pngchunk.com/)** to extract metadata from PNGs.  

---

## 📂 Repo Layout
- `corrupted/` → provided corrupted images  
- `metadata/` → extracted metadata (JSON/TXT)  
- `fixed/` → corrected/un-corrupted outputs  
- `logs/` → notes on parameter fixes and trials  

---

## 🚀 How to Run
1. Open [pngchunk.com](https://pngchunk.com/) and upload a corrupted image.  
2. Extract **prompt, seed, sampler, steps, CFG, model info**.  
3. Reproduce the image in ComfyUI / Automatic1111 with the same metadata.  
4. Identify which **1–2 parameters** are wrong (e.g., CFG too high, wrong sampler).  
5. Fix them → regenerate → save result in `fixed/`.  
6. Document changes in `logs/`.  

---

## ✅ Checklist
- [ ] All 3 corrupted images in `corrupted/`  
- [ ] Metadata extracted for each in `metadata/`  
- [ ] Fixed versions in `fixed/`  
- [ ] Notes on corrections in `logs/`  

---

## 📜 License
MIT (repo). Generated images follow base model license.
