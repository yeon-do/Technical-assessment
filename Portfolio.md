# 📜 Doyeon Park Portfolio
Doyeon Park - yeon-do Portfolio for Technical assessment



# 📌 Projects Overview
| Project | Period | Role | Tech Stack |
|------|------|------|------|
| Project | 07.2025 - Ongoing | Present	Undergraduate Intern | Python, LLM, KG |
| Applied Regression | 09.2025 – 12.2025 | Data Analyst | R, Statistics |
| Fashion AI Predictor | 09. 2024 – 11. 2024 | Model Architect | Python, PyTorch |
| REFEELY (Web Game) | 03.2025 – 07.2025 | Frontend Dev | JS, Phaser3 |


# 📝 Projects

## 1. Knowledge Graph (KG)-based Sequential Recommendation Research 🔬

**Undergraduate Research Intern @ Data Mining Lab, Hanyang University**

Extending the text-aware sequential recommendation model (GRAM) by incorporating structural data. Currently researching methodologies to apply Knowledge Graphs (KG) for enhanced item identification and path retrieval.

* **Project Timeline:** 07.2025 - Ongoing
* **Key Role:** Literature Review, Baseline Reproduction, and KG Engineering
* **Tools Used:** VScode, PyTorch
* **Language:** Python

**Key Contributions:**
* **Literature Review & Baseline Reproduction:** Conducted extensive reviews of SOTA papers on Sequential RecSys and KG applications to formulate research hypotheses. Successfully reproduced the original GRAM model and other foundational baselines to establish a robust starting point.
* **Experimentation & Metric Standardization:** Applied custom datasets to baseline models to secure initial performance metrics. Modified the experimental setup to standardize evaluation criteria, specifically shifting from candidate sampling to a more rigorous full-ranking evaluation methodology.
* **KG Construction & Path Analysis:** Engineered a framework to build a structural Knowledge Graph from the dataset to extract relational information. Developed algorithms to analyze the shortest paths within the KG, laying the groundwork for structural 'Item Identifier' and 'Path Retrieval' modules.
<img src="https://github.com/user-attachments/assets/85944ba8-7d97-4b25-8f26-f0074322d8fc" width="70%"/>

**🎞 Core Research Codes**
*As the main architecture is currently under development and confidential, the attached repository contains the foundational data processing and graph analysis codes.*
* [👉 View KG Construction & Shortest Path Analysis Codes](https://github.com/yeon-do/llmbased-rec/blob/main/FIXED_2_analyze_shortest_paths.py)
<br>

## 2. Advanced Statistical Modeling & Regression Analysis 📊

**Coursework: Applied Regression Analysis (Department of Mathematics, Hanyang University)**

Applied diverse statistical methodologies ranging from simple linear regression to regularization techniques based on varying data conditions, and conducted academic discussions and peer reviews to validate model assumptions.

* **Project Timeline:** 09.2025 – 12.2025
* **Key Role:** Data Analyst & Final Presenter
* **Tools Used:** RStudio
* **Language:** R

**Key Contributions:**
* **Step-by-step Modeling & Problem Solving:** Applied optimal regression methods from basic simple/multiple linear regression to Ridge and Lasso estimators to datasets with diverse characteristics, writing analytical code to solve textbook exercises.
* **Model Diagnostics & Peer Review:** Conducted rigorous residual analysis (testing for normality and homoscedasticity) on the derived models. Compared and debated results with other teams to identify modeling limitations and propose methodological improvements.

**🎞 Final Presentation: In-depth Analysis of Dummy Variable Regression**

For the final project, I designed and presented Dummy Variable Regression models using chick growth and turkey weight datasets to analyze how categorical factors (e.g., vitamin types, age groups) impact quantitative outcomes. I established a systematic model selection flowchart using partial F-tests (testing for parallelism and coincidence) and statistically interpreted the limitations caused by small sample sizes.

<img src="https://github.com/user-attachments/assets/18423891-28a9-48c3-ace4-1a45c6e4ecc5" width="70%">

[👉 View all exercise codes, final presentation (PPT), and reports](https://github.com/yeon-do/anlaysis-application-regression.git)
<br>

## 3. Fashion Style Image Classification & Preference Prediction 👟

**Organized by National Information Society Agency (NIA) - Data Creator Camp**

Developed a deep learning-based fashion style classification model and extracted feature vectors to build a preference prediction algorithm based on image similarity.

* **Project Timeline:** 09. 2024 – 11. 2024
* **Key Role:** Model Architect & Data Preprocessing Lead
* **Tools Used:** VScode, Colab, PyTorch, U-2-Net, Mask R-CNN, ResNet-18
* **Language:** Python

**Key Contributions:**
* **Advanced Image Preprocessing Pipeline:** Led the image preprocessing phase utilizing U-2-Net and Mask R-CNN for precise background removal and object segmentation. Applied robust data augmentation techniques to improve model generalization.
* **Image Classification Model (ResNet-18):** Implemented and fine-tuned a ResNet-18 architecture to accurately classify multi-year fashion images into specific style categories.
* **Similarity-based Preference Prediction:** Extracted latent feature vectors from the classification model to compute image similarities. Leveraged these distance metrics as item similarities to construct an item-based collaborative filtering algorithm for preference prediction.

**Award Recognition:** Awarded the **Excellence Award (2nd Place)** by NIA, recognized for logical consistency, innovative integration of computer vision with recommendation logic, and robust model performance.

**🎞 Project Presentation & Code**
* [👉 View Project Presentation (PPT) & Source Code](https://github.com/yeon-do/Data_create_camp.git)
* [💻 View Simplified Core Code (Classification, Feature Extraction & Similarity RecSys)](https://github.com/yeon-do/Data_create_camp/blob/main/Simplified%20Core%20code(Classification%2C%20Feature%20Extraction%20%26%20Similarity%20RecSys).py)

<br>

## 4. Web-based Recycling Educational Game 'Re:Fact' ♻️

**Collaboration with Eco-friendly Packaging Company 'Refeely' (KAKAO Tech Impact & Hanyang Univ.)**

A gamification-based educational solution designed to promote correct waste separation practices and improve the low recycling rate (13%) of paper cartons.

* **Project Timeline:** 03.2025 – 07.2025
* **Key Role:** Frontend Developer
* **Tools Used:** VScode, Phaser3
* * **Language:** JavaScript

**Key Contributions:**
* **Frontend & Game Engine Development:** Developed the core game logic including waste sorting gameplay, pretreatment action missions, and quizzes using the Phaser3 framework and JavaScript for an engaging UI/UX.
* **Project Planning & Client Communication:** Directly communicated with the Refeely CEO to translate business requirements into technical features. Successfully integrated real-world reward systems, such as linking product QR codes and converting in-game points to the company's online mall.
* **Driving ESG Impact:** Contributed to a solution where 77.6% of test users reported an improved willingness to practice eco-friendly behaviors, targeting a measurable increase in nationwide recycling rates.

<img src="https://github.com/user-attachments/assets/b37bbedc-85ec-44b7-8b95-4043c8bac0c6" width="60%">

<br>**🔗 Links:**
* [🎮 Play the Game on Web](https://funny-pasca-8573bf.netlify.app/)
* [👉 View Detailed & Source Code](https://github.com/yeon-do/TFI_CAMPUS_HANYANG_25Spring_REPACT.git)
