# 🏥 Analyzing Medical Images with Google MedGemma 1.5
---
## 🎯 Abstract
Healthcare systems worldwide face escalating clinician burnout, widening health literacy gaps, and limited access to specialist care in resource-constrained settings. Physicians spend over half their time on documentation, patients often struggle to understand medical guidance, and rural clinics lack advanced diagnostic support.

This notebook demonstrates **Google's MedGemma 1.5** model for analyzing medical images including X-rays, CT scans, and ultrasounds.

## Enviroment Setup
We install packages torch, transformers, amongst others. We then check thier versions and authenticate hugging face which allows us to access MedGemma.

## Cases:
### Case 1: Standard Chest X-Ray

<img width="742" height="808" alt="image" src="https://github.com/user-attachments/assets/fcb6d551-dd30-4f2f-83d5-5f00e683c7d6" />

**Objective:** The model will analyze a standard chest X-ray and identify any abnormalities.

The following are the key structures that will be evaluated:
* Lung fields heart size
* mediastinum
* bony structures

### Case 2: Suspected Pneumonia
<img width="627" height="432" alt="image" src="https://github.com/user-attachments/assets/62e2670a-f9a1-4a39-8343-2f23ee076f50" />

**Patient:** 58-year-old male

**Clinical History:**
- 3-month progressive shortness of breath
- Non-productive cough
- 7 kg weight loss over 8 weeks
- Low-grade fevers and night sweats
- No response to multiple antibiotic courses

**Differential:** Pneumonia, tuberculosis, lung malignancy, interstitial lung disease

### Case 3: Acute Respiratory Distress
<img width="900" height="545" alt="image" src="https://github.com/user-attachments/assets/a6d72863-0cf6-4b05-bc77-ca20aa00ff30" />

**Patient:** 62-year-old

**Clinical History:**
- Acute onset dyspnea (past few days)
- Pleuritic chest pain
- Recent prolonged immobility (long trip)
- Intermittent lightheadedness

**Risk Factors:** DVT/PE risk from immobility

**Differential:**
* Pulmonary embolism
* pleural effusion
* pneumothorax

### Case 4: Suspected Heart Failure
<img width="800" height="612" alt="image" src="https://github.com/user-attachments/assets/2ae2f803-ed1f-421c-83fe-8c864c632d10" />

**Patient:** 68-year-old

**Clinical History:**
- Progressive dyspnea (several weeks)
- Orthopnea (SOB when lying flat)
- Nocturnal cough with breathlessness
- Lower limb swelling

**Classic HF Features:** ✅ Orthopnea ✅ PND ✅ Peripheral edema

**Expected Findings:** Cardiomegaly, pulmonary edema, bilateral infiltrates


### Case 5: Chronic Progressive Respiratory Symptoms
<img width="900" height="695" alt="image" src="https://github.com/user-attachments/assets/1784c06a-7e4d-41a1-a69e-388eb7f58a0e" />

**Patient:** 60-year-old

**Clinical History:**
- Progressive dyspnea and dry cough (weeks)
- Unintentional weight loss (2-3 months)
- No relief with antibiotics ⚠️

**Red Flags:** Weight loss → malignancy, No antibiotic response → non-infectious

**Differential:** Interstitial lung disease, bronchioloalveolar carcinoma, chronic infection

### Case 6: Uterine Fibroid

**Patient:** 38-year-old female

**Clinical History:**
- Worsening menstrual symptoms (1 year)
- Heavy bleeding with clots
- Pelvic pressure and discomfort
- Fatigue

**Suspected:** Uterine fibroids (leiomyomas)

# 📊 Conclusion

## ✅ Key Takeaways

**MedGemma 1.5 Capabilities:**
- ✓ Multimodal understanding (image + text)
- ✓ Clinical context awareness
- ✓ Multiple imaging modalities
- ✓ Detailed anatomical descriptions

## ⚠️ Limitations
- **Not a diagnostic tool** - requires professional validation
- **Educational purpose only**
- **Clinical judgment essential**

## 📚 References
- [MedGemma Model](https://huggingface.co/google/medgemma-1.5-4b-it)
- [Radiology Assistant](https://radiologyassistant.nl/)
---
