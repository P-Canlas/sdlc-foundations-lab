# STUDENT WORKSHEET: SDLC, AGILE, DEVOPS & GIT FOUNDATIONS

**Course Code / Subject:** [NTC-PC14] Software Engineering<br>
**Student Name:** Patrick Jay M. Canlas<br>
**Date:** August 26, 2026 | **Section:** 3.5 BSIT<br>
**GitHub Repository URL:** https://github.com/P-Canlas/sdlc-foundations-lab

---

## PART 1: GITHUB ONBOARDING & SETUP VERIFICATION

### GitHub Account Creation & Onboarding
**Objective:** Set up a centralized remote repository environment for future CI/CD and GitFlow collaboration.

#### 1. Account Registration
* Go to [github.com](https://github.com) and click **Sign Up**.
* Enter your academic email address, create a strong password, and select a professional username (e.g., `j-perminola`).
* Complete the verification puzzle and enter the launch code sent to your email.

#### 2. Profile & Security Setup
* Set your display name to your full name and upload a profile picture.
* Go to **Settings > Password and authentication** and enable Two-Factor Authentication (2FA) using an authenticator app or SMS.

#### 3. Verification Task
* Click the **+** icon in the top right and select **New repository**.
* Name the repository `sdlc-foundations-lab`, set visibility to **Public**, check **Add a README file**, and click **Create repository**.
* Copy your public repository URL to submit alongside Part 2.

#### Task Checklist
- [✅] Created GitHub account using academic email.
- [✅] Enabled Two-Factor Authentication (2FA) in Settings.
- [✅] Created public repository named `sdlc-foundations-lab` with a `README.md`.
- [✅] Pasted public repository link in the header above.

---

## PART 2: REAL-WORLD ENGINEERING SCENARIOS

### Scenario A: SDLC & Framework Selection
**Context:** A fintech company wants to release a new peer-to-peer payment feature. A government regulatory agency requires complete compliance auditing before release, but competitors are rapidly capturing market share.

**Task:**
1. Compare Waterfall vs. Agile (Scrum) for this launch using the criteria below.
2. Choose a hybrid or primary framework (e.g., Scrum vs. Waterfall vs. Spiral). Explain your reasoning in 2–3 sentences.

#### 1. Framework Comparison Table

| Criteria | Waterfall | Agile (Scrum) |
| :--- | :--- | :--- |
| **Adaptability & Time-to-Market** | It would be difficult and time-consuming to release the payment feature under Waterfall, and it would probably miss the strategic window to gain market share. | The feature can be deployed much quicker when Agile (Scrum) is used. Because of its high degree of adaptability, the team can release at the appropriate time and react quickly to the state of the market. |
| **Regulatory & Compliance Risk Handling** |Regulatory requirements are fully addressed during development. The feature will not be deployed until everything is complete, ensuring full compliance with the government agency before release. | Continuous development cycles may be disrupted in order to comply with the government agency. It raises the possibility of releasing versions of the feature before receiving complete official approval. |

#### 2. Framework Recommendation & Justification
*Which primary or hybrid framework (e.g., Scrum, Waterfall, or Spiral) do you recommend for this fintech regulatory project? Explain your choice in 2–3 sentences.*

**Answer:**
> Since the peer-to-peer payment feature requires time for approval, i recommend using the Scrum framework for this project. This method enables the team to quickly develop and thoroughly test the feature in iterations, guaranteeing that it is ready for deployment as soon as regulatory clearance is received.


### Scenario B: DevOps & CI/CD Pipeline Breakdown
**Context:** A team merges code, but the production app breaks during deployment because testing was done manually on individual laptops rather than in an automated pipeline.

**Task:**
1. Identify where the communication and process gap occurred between Dev and Ops.
2. Map out the automated CI/CD pipeline stages and state which stage would catch this bug before it reaches production.

#### 1. Gap Analysis
*Identify where the communication and process breakdown occurred between Dev and Ops.*

**Answer:**
> Instead of using a standardized, automated staging environment, the team relied on manual testing on individual developer laptops, which led to the breakdown. Because of this disconnect between development and operations, the combined code was never adequately tested in a production-like environment prior to deployment.

#### 2. Pipeline Stage Identification
*Fill in the missing stages of the continuous assembly line and circle/bold the stage that catches local testing bugs before production release:*

**Answer:**
`Plan -> Code -> Build -> **Test** -> Release -> Deploy -> Operate -> Monitor`

### Scenario C: Git Lifecycle & Branching Strategy

#### 1. Data Movement Command Mapping
*Write the standard Git command used to transfer code between each environment:*

* **Working Directory -> Staging Area:** `git add`
* **Staging Area -> Local Repository:** `git commit`
* **Local Repository -> Remote Repository (GitHub):** `git push`
* **Remote Repository -> Working Directory:** `git pull`

#### 2. GitFlow Collision Prevention
*Explain how utilizing Feature Branches and a Develop branch prevents two developers from overwriting each other's code on Main. (2 to 3 sentences)*

**Answer:**
