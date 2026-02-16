# 🏥 Analyzing Medical Images with Google MedGemma 1.5
---
## 🎯 Abstract
Healthcare systems worldwide face escalating clinician burnout, widening health literacy gaps, and limited access to specialist care in resource-constrained settings. Physicians spend over half their time on documentation, patients often struggle to understand medical guidance, and rural clinics lack advanced diagnostic support.

This notebook demonstrates **Google's MedGemma 1.5** model for analyzing medical images including X-rays, CT scans, and ultrasounds.

## Enviroment Setup
We install packages torch, transformers, amongst others. We then check thier versions and authenticate hugging face which allows us to access MedGemma.

## Cases:
### Case 1: Standard Chest X-Ray

https://www.cvmg.com/wp-content/uploads/2014/10/chest-xray.jpg<img width="742" height="808" alt="image" src="https://github.com/user-attachments/assets/fcb6d551-dd30-4f2f-83d5-5f00e683c7d6" />

**Objective:** The model will analyze a standard chest X-ray and identify any abnormalities.

The following are the key structures that will be evaluated:
* Lung fields heart size
* mediastinum
* bony structures

### Case 2: Suspected Pneumonia

**Patient:** 58-year-old male

**Clinical History:**
- 3-month progressive shortness of breath
- Non-productive cough
- 7 kg weight loss over 8 weeks
- Low-grade fevers and night sweats
- No response to multiple antibiotic courses

**Differential:** Pneumonia, tuberculosis, lung malignancy, interstitial lung disease

### Goals:
- 🔍 Analyze chest X-rays and identify any abnormalities
- 🩺 Detect pulmonary conditions such as pneumonia, edema, effusions, asthma, etc
- 📊 Process ultrasound imaging
- 💡 Provide clinical contextually aware assessments

### ⚠️  Disclaimer
This notebook is for educational purposes only. Outputs should NOT replace professional medical diagnosis.

---
