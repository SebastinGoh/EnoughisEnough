# EnoughisEnough
IS485 (SMT Research) Enough is Enough:  Effects and Implications of polypharmacy on Mental Health Patients

In recent times, polypharmacy has become increasingly prevalent in the psychiatric world, not only splitting opinions on its long-lasting effects on patients, but also incurring hefty medical costs on patients suffering from the side effects of polypharmacy. 

In this research paper, our team tackles the problem of polypharmacy in two ways: creating an improved two-dimensional scoring system to quantify the severity of polypharmacy, and using machine learning to detect premature polypharmacy. 

## RQ1: Considering the existing methods and algorithms used for scoring, what is the best way to quantify the presence and severity of polypharmacy?
<img width="349" alt="image" src="https://github.com/SebastinGoh/EnoughisEnough/assets/39021770/ffa65b0d-64a3-4413-9d2b-0fa3b51cfccc">

In RQ1, the team conducted a literature review and identified shortcomings in current popular scoring systems. We then propose an improved scoring system that has added dimensionality and depth. 

## RQ2: Is there any correlation between various independent variables (patient demographic, medical history, etc) and the occurrence of polypharmacy. If such a correlation exists, which factors contribute most to the occurrence of polypharmacy?
{refer to RQ2 Categorical Modelling.ipynb & RQ2 Regression Modelling.ipynb}

Using the new scoring system as the target variable on our patient dataset, we built both predictive classification and regression models in RQ2, and proceeded to run feature importance analysis on the models to discover the patient demographic and medical factors that correlate most to a high or low polypharmacy score. It can be seen that a higher number of unique mental health diagnoses, higher age as well as poorer financial and familial situations of patients have a higher correlation to the occurrence of polypharmacy. 

## RQ3: Can polypharmacy be predicted through unstructured data derived from patient-physician interaction? If so, how can we use text analysis to detect polypharmacy?
{refer to RQ3.ipynb}

In RQ3, the team used a more qualitative approach, conducting textual analysis on a textual corpus of patient-physician clinical notes. We used Latent Dirichlet Allocation (LDA) Topic Modelling in order to discover topics, phrases and keywords that correlate with polypharmacy occurrence. The patients associated with high polypharmacy tend to follow a prescription plan and consume medication regularly, have a history of substance abuse as well as have close monitoring of health. The patients associated with low polypharmacy tend to have good familial relationships, especially with their mothers, and a more positive well-being. 

## Actionable Insight & Conclusion
<img width="264" alt="image" src="https://github.com/SebastinGoh/EnoughisEnough/assets/39021770/a319975e-e5e6-436f-af29-da7cb5201225">

After gathering insights from RQ2 and RQ3, we proposed an actionable insight in the form of a Polypharmacy Risk Assessment Card (PRAC), which is the first step to a solution to early detection of polypharmacy. The PRAC can be provided to psychiatrists for reference in their own time while treating patients or programmed as an in-built reminder system for desk pharmacists prior to drug prescriptions to patients. 

These applications act to combat the risk of polypharmacy throughout psychiatric clinics and can be the first step in raising awareness of polypharmacy amongst psychiatrists and pharmacists.
