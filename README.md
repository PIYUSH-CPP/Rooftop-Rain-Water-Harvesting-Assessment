📘 Rooftop Rainwater Harvesting Feasibility Tool – README
🌧️ 1. Introduction

Groundwater depletion is one of India’s most pressing environmental challenges. With rapidly falling water tables, high dependence on groundwater, and increasing climate unpredictability, the need for decentralized water conservation measures has become urgent.

Rooftop Rainwater Harvesting (RTRWH) is one of the most effective and sustainable solutions, yet adoption remains low due to lack of awareness, technical complexity, and absence of user-friendly tools.

This project provides a web/mobile application prototype that allows any citizen to instantly evaluate the rainwater harvesting potential at their location using GIS data, hydrological formulas, rainfall datasets, and simple user inputs.


🎯 2. Problem Statement

Although rooftop rainwater harvesting is mandated in many Indian cities, citizens lack:

Awareness of how much water their rooftop can generate

Knowledge of what type of harvesting structure is suitable

Information on local groundwater depth or aquifer characteristics

Technical guidance on sizing recharge pits/trenches/shafts

Cost estimates or cost-benefit analysis

A simple, digital way to evaluate feasibility

Existing resources (CGWB manuals, PDFs, reports) are technical and not citizen-friendly. There is no national-level digital tool that converts rooftop + rainfall + groundwater data into personalized, actionable recommendations.


💡 3. Solution Overview

This prototype provides:

🔹 On-spot feasibility check for rooftop rainwater harvesting
🔹 Automatic rainfall & groundwater integration using GIS datasets
🔹 Personalized structure recommendations (pit, trench, shaft, tank)
🔹 Runoff volume calculation based on roof material
🔹 Engineering-based sizing of recharge structures
🔹 Cost estimation & payback analysis
🔹 Multilingual interface for wider adoption
🔹 Downloadable PDF reports for users

The platform converts scientific hydrological models into a simple, app-based experience that anyone can use.

📱 4. Key Features
A. User Inputs

🔹Location (GPS or manual pin-drop)

🔹Roof area (manual entry or polygon draw)

🔹Roof type (RCC, metal, tile, asbestos)

🔹Number of dwellers

🔹Open space availability

🔹Soil type (if known)

B. Data Integration

🔹IMD rainfall normals

🔹CGWB groundwater levels

🔹Aquifer maps (WRIS/Bhuvan)

🔹Soil information from national datasets

C. Analytical Outputs

🔹Annual rainwater capture potential

🔹Feasibility score (High / Medium / Low)

🔹Suggested structure type

🔹Recommended dimensions

🔹Cost estimate

🔹Savings & payback period

🔹Environmental benefits

D. User Experience

🔹Visual maps and diagrams

🔹Multilingual (Hindi, English + expandable)

🔹Simple guided workflow

🔹PDF report export


📐 5. Mathematical & Hydrological Calculations
1️⃣ Runoff Volume Calculation

We use the standard rooftop runoff formula:

𝑉
=
𝐴
×
𝑃
×
𝐶
V=A×P×C

Where:

𝐴
A = Roof area (m²)

𝑃
P = Annual rainfall (m)

𝐶
C = Runoff coefficient

Typical Runoff Coefficients

Roof Type	Coefficient (C)
RCC roof	0.85
Metal sheet	0.90
Tiles	0.75
Asbestos sheet	0.80

Example:
Roof area = 100 m²
Annual Rainfall = 800 mm = 0.8 m
Coefficient = 0.85

𝑉
=
100
×
0.8
×
0.85
=
68
 m
3
=
68
,
000
 liters
V=100×0.8×0.85=68 m
3
=68,000 liters
2️⃣ Recharge Feasibility Logic

The system evaluates:

Soil type (sand/clay/loam)

Groundwater depth

Presence of open unpaved space

Local contamination risks

If recharge feasible → recommend pit/trench/shaft.
If not feasible → recommend storage tank.

3️⃣ Recharge Pit Sizing Formula
Pit Size
=
𝑉
recharge
𝑖
×
𝑡
Pit Size=
i×t
V
recharge
	​

	​


Where:

𝑉
recharge
V
recharge
	​

 = Target recharge volume

𝑖
i = Soil infiltration rate (m/day)

𝑡
t = Recharge duration (days)

Example:

Required recharge = 15 m³

Soil infiltration = 0.4 m/day

Time = 3 days

Bottom Area
=
15
0.4
×
3
=
12.5
 m
2
Bottom Area=
0.4×3
15
	​

=12.5 m
2

A practical pit may be:
3.5 m × 3.5 m × 3 m depth

4️⃣ Cost Estimation

Cost = Excavation + Masonry + Filter Media + Labor

Typical unit rates vary by region; app uses standard cost indices.

Example:

Recharge pit cost = ₹35,000 – ₹60,000

Annual savings in tanker cost = ₹20,000 – ₹50,000

Payback in 1–2.5 years

 

APIs: IMD rainfall, CGWB groundwater, WRIS aquifer

Hosting: Firebase / Cloudflare / AWS

Languages: Hindi, English (extendable)
