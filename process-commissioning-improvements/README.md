### Process & Commissioning Improvements 

**Focus:** shipboard power systems, commissioning readiness, safer production workflows  

**Highlights (Measured Impact)**
- Shore power receiving workflow redesign for HV vessels → **~720 MH saved per vessel**
- Battery charger function test standardization (advanced auto charge/discharge) → **~30 MH saved per vessel**
- Ship network utilization expansion (training + quay infrastructure) → **~430 MH saved per vessel**
- Navigation/communication commissioning procedure pre-review → **~290 MH saved per vessel**
- PMS verification process improvement → **reduced late-stage troubleshooting and improved test repeatability**
- Generator parallel running & PF optimization (Droop → CCC) → **improved kVAR sharing stability and reduced tuning trial-and-error**


---

#### 1) Safer Shore Power Receiving for High-Voltage Vessels (AMP Reel Integration)
**Problem**  
Shore power cables were previously connected directly to the switchboard, increasing **electric shock risk** and raising concerns around **equipment protection** during handling/connection.

**My contribution**
- Re-designed the shore power receiving process to utilize an **external AMP reel interface** instead of direct switchboard connection.
- Defined a safer workflow (handling → connection → verification) and clarified boundaries between external interface and switchboard.
- Coordinated practical adoption with production/commissioning stakeholders.

**Outcome**
- Improved operational safety by reducing exposure at the switchboard connection point.
- Strengthened equipment integrity through a more controlled connection interface.
- **Man-hour impact:** **~720 MH saved per vessel** 

---

#### 2) Standardized Function Testing for Shipboard Battery Chargers (Advanced Auto Charge/Discharge)
**Context**  
A project included a battery charger system with **temperature-dependent automatic charge/discharge control**, requiring more complex verification than typical builds.

**My contribution**
- Standardized a repeatable **function test procedure** covering temperature-driven behavior and automatic sequences.
- Defined acceptance criteria and test checkpoints to ensure consistent execution regardless of inspector/project team.
- Documented the test logic for auditability and smoother handover.

**Outcome**
- Improved inspection consistency and reduced rework caused by ambiguous test interpretations.
- Increased test coverage for advanced control features vs. legacy “basic charger” test methods.
- **Man-hour impact:** **~30 MH saved per vessel** 

---

#### 3) Increasing Yard & Quay Utilization of Ship Network Systems (Training + Infrastructure)
**Problem**  
The ship network was used only for basic functions and performance was limited, reducing value for production and vessel management. In addition, many signals and integrations relied on **hardwired I/O**, which increased cable routing and installation workload.

**My contribution**
- Evaluated practical expansion use cases for ship network systems in production/operations.
- Led the transition effort from **hardwired I/O connections to network-cable-based connectivity** where applicable, reducing overall cable pulling and routing volume.
- Organized and hosted **in-house training** by inviting network specialists to educate internal teams.
- Led quay-side network expansion initiatives to improve connectivity for alongside vessels.
- Promoted real workflow adoption so the network supported daily vessel management tasks.

**Outcome**
- Reduced cable installation effort by lowering the amount of I/O cabling required through network-based integration.
- Improved efficiency of quay-side vessel management through better connectivity and adoption.
- Elevated internal capability via training and clearer use cases.
- **Man-hour impact:** **~430 MH saved per vessel**

---

#### 4) Pre-Review of Commissioning Procedures for Navigation & Communication Systems
**Context**  
Navigation/communication systems vary substantially by vessel type (commercial vs. offshore), requiring detailed verification and a structured commissioning sequence.

**My contribution**
- Reviewed commissioning procedures in advance to identify gaps, optimize readiness, and standardize checkpoints.
- Aligned key tests and sequencing to reduce confusion during execution and inspection.
- Supported sea trial readiness by improving clarity of steps, responsibilities, and expected results.

**Outcome**
- Reduced commissioning and inspection hours by improving sea trial readiness.
- Improved verification quality and consistency across different project configurations.
- **Man-hour impact:** **~290 MH saved per vessel** 

---

#### 5) Improving the Verification Process for the Ship Power Management System (PMS)
**Problem / Pain Point**  
PMS verification was often time-consuming and inconsistent due to variations in test sequence, unclear pass/fail criteria, and frequent late-stage findings during commissioning and sea trials.

**My contribution**
- Refined the PMS verification workflow by structuring tests into clear phases (e.g., pre-checks → functional logic → integration scenarios → abnormal/blackout recovery).
- Established repeatable check points and acceptance criteria for key PMS functions, such as:
  - generator start/stop permissives and interlocks  
  - load-dependent start/stop logic (load sharing / load shedding / start inhibit)  
  - priority-based load shedding and restoration sequences  
  - blackout detection and recovery logic  
  - alarms, events, and operator interface verification (HMI indications, logging)
- Improved coordination between electrical commissioning, automation/control, and relevant vendors so that issues were captured earlier and resolved faster.

**Outcome**
- Reduced late-stage troubleshooting during commissioning by catching logic/configuration issues earlier.
- Improved repeatability and auditability of PMS verification across vessels/projects.

---

#### 6) Generator Parallel Running & Power Factor (PF) Optimization (Droop → Cross Current Compensation)
**Problem / Objective**  
When generators operate in parallel, poor reactive power sharing can lead to unstable bus voltage, circulating reactive currents, suboptimal PF, and repeated tuning during commissioning.

**My contribution**
- Reviewed and applied generator reactive load-sharing fundamentals to improve stability in parallel operation:
  - kW (real power) sharing vs. kVAR (reactive power) sharing  
  - AVR behaviors and their impact on bus voltage and PF  
- Led a gradual transition of the reactive load-sharing approach from **conventional droop** to **Cross Current Compensation (CCC)**.
- Updated commissioning guidance and troubleshooting logic so teams could validate:
  - stable kVAr sharing between generators  
  - reduced reactive circulating current  
  - improved voltage regulation under changing load conditions  

**Why CCC can be better than droop (in practice)**
- **More accurate kVAr sharing:** CCC helps generators share reactive power more evenly, which can reduce kVAr imbalance that sometimes remains under droop-based sharing.
- **Reduced circulating reactive current:** By compensating cross-current effects, CCC can minimize unnecessary reactive circulation between machines, supporting more stable operation.
- **Better voltage stability during parallel running:** CCC can maintain steadier bus voltage under varying reactive demand, reducing iterative tuning and “hunting” during trials.

**Outcome**
- Improved operational stability during generator parallel running and reduced trial-and-error tuning during commissioning.
- Provided clearer, more repeatable guidance for PF-related tuning and diagnostics (less ambiguity, faster root-cause isolation).

