# 🌑 Solar Eclipse Analysis – 17 February 2026

## 📌 Project Overview

On **17th February 2026**, parts of the world observed a solar eclipse.  
This project evaluates whether NASA’s historical solar eclipse dataset can accurately describe and help predict eclipse characteristics.

Dataset Source:  
https://www.kaggle.com/datasets/nasa/solar-eclipses?select=solar.csv

The dataset contains both past and future eclipse records and was analyzed using Python to validate eclipse geometry, intensity metrics, and predictive capability.

---

## 🎯 Research Objectives

The following research questions (RQs) guide the analysis:

1. **RQ1:** How did Gamma determine geometrical alignment?
2. **RQ2:** Did Magnitude, Path Width & Duration describe intensity?
3. **RQ3:** When is the Next Eclipse & What Type?

---

## 📊 Dataset Structure

The dataset includes the following fields:

- Catalog Number  
- Calendar Date  
- Eclipse Time  
- Delta T (s)  
- Lunation Number  
- Saros Number  
- Eclipse Type  
- Gamma  
- Eclipse Magnitude  
- Latitude  
- Longitude  
- Sun Altitude  
- Sun Azimuth  
- Path Width (km)  
- Central Duration  

---

## 🔍 Findings & Evidence

### 1️⃣ Eclipse Details – 17 February 2026

| Metric | Value |
|--------|--------|
| Calendar Date | 2026-02-17 |
| Eclipse Time | 12:13:06 |
| Delta T (s) | 75 |
| Lunation Number | 323 |
| Saros Number | 121 |
| Eclipse Type | Annular |
| Gamma | -0.9743 |
| Eclipse Magnitude | 0.963 |
| Latitude | 64.7°S |
| Longitude | 86.8°E |
| Sun Altitude | 12° |
| Sun Azimuth | 268° |
| Path Width | 616 km |
| Central Duration | 02m20s |

### Validation

Comparison with publicly available references confirms:

- Observed eclipse time ≈ **12:12**
- Central duration ≈ **02m20s**

The dataset aligns closely with real-world records.

---

## 📐 RQ1: How did Gamma determine geometrical alignment?

- Absolute Gamma = **0.9743**
- Since |Gamma| is close to 1, the Moon’s shadow passed near Earth’s edge.
- The negative sign (-0.9743) indicates the shadow passed **south of Earth's center**.
- This confirms a near-edge annular eclipse.

**Interpretation:**  
Gamma successfully explains eclipse alignment geometry.

---

## 🌗 RQ2: Did Magnitude, Path Width & Duration describe intensity?

Correlation Results:

| Variables Compared | Correlation |
|--------------------|------------|
| Path Width & Duration | +0.55 |
| Magnitude & Path Width | -0.26 |
| Magnitude & Duration | -0.37 |

### Observations

- Wider path width → Longer central duration (strong relationship).
- Higher magnitude does NOT always imply wider path.
- Higher magnitude does NOT guarantee longer duration.
- Partial eclipses may show high magnitude but lack a wide central path.

**Conclusion:**  
Intensity is multi-dimensional. Path Width and Duration better describe physical intensity compared to magnitude alone.

---

## 🌍 RQ3: When is the Next Eclipse & What Type?

Next Eclipse Date: **2026-02-22**

| Metric | Value |
|--------|--------|
| Eclipse Type | Peripheral |
| Eclipse Magnitude | 0.3393 |
| Gamma | -1.3595 |

### Interpretation

- |Gamma| > 1 → No central eclipse (only partial visibility).
- Magnitude = 0.3393 → Weak eclipse.
- Shadow shifted further toward the Southern Hemisphere.
- Maximum eclipse point lies south of Earth's equatorial plane.

**Conclusion:**  
The next eclipse is significantly weaker than the 17 Feb 2026 event.

---

## 🧠 Overall Conclusion

The NASA dataset:

✔ Accurately reflects real-world eclipse timing  
✔ Correctly models geometric alignment using Gamma  
✔ Explains intensity using Path Width and Duration  
✔ Predicts upcoming eclipse events reliably  

This confirms that historical astronomical datasets can effectively describe and predict solar eclipse characteristics when analyzed properly.

---


## 📌 Author 

Sibankar Saha
