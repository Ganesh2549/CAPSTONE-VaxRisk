# CAPSTONE-VaxRisk: Analysis of VAERS Reports for Vaccine Safety Assessment

ABSTRACT

Adverse events (AEs) are negative outcomes that occur following medical treatment or therapy. This study aims to develop a predictive model to classify AEs as serious or non-serious, focusing on vaccination data. Since adverse reactions to vaccines can vary based on demographic factors, environmental conditions, and drug quality, it is impossible to identify all potential side effects during clinical trials. Post-approval, physicians and patients report any adverse reactions, which are documented in the Vaccine Adverse Event Reporting System (VAERS) maintained by the CDC and FDA.

For this study, data from four vaccines—COVID-19, Varicella-Zoster (VARZOS), Pneumococcal (PPV), and Influenza (FLU)—were analyzed. During the data preprocessing phase, duplicate records were removed, missing values were handled, and a binary target variable, ‘serious,’ was created to indicate the severity of each reported AE.

Key patient-related features such as age, gender, symptom descriptions, hospitalization, life-threatening conditions, disability, death, recovery status, concurrent medications, current illness, medical history, allergies, birth defects, and vaccine manufacturer were selected for the model. This comprehensive feature set was identified through exploratory data analysis (EDA) and is expected to improve the accuracy of predicting the seriousness of adverse events.


INTRODUCTION

On April 7, 2021, the CDC received reports of clusters of anxiety-related reactions at five mass vaccination sites across different U.S. states following the administration of the Janssen COVID-19 vaccine. These events occurred after five weeks of vaccine usage under the FDA's Emergency Use Authorization (EUA). To further investigate these occurrences, the CDC conducted interviews with staff from the affected vaccination sites and reviewed their procedures. Four of the five locations temporarily paused operations to allow for a thorough investigation. In total, 64 anxiety-related incidents were recorded between April 7 and April 9, including 17 cases of syncope (fainting), a known anxiety-related reaction, among the 8,624 Janssen vaccine recipients.

The CDC then analyzed syncope reports submitted to the Vaccine Adverse Event Reporting System (VAERS), a vaccine safety surveillance system managed by the CDC and FDA. The syncope rate following the Janssen COVID-19 vaccine was 8.2 cases per 100,000 doses, significantly higher than the rate of 0.05 cases per 100,000 doses after the 2019–2020 influenza vaccine. While anxiety-related reactions can occur after any vaccination, the data suggest that such events, including syncope, are more frequent following the Janssen vaccine. It is critical that healthcare providers are aware of this increased risk and monitor all COVID-19 vaccine recipients for at least 15 minutes post-vaccination to manage any potential adverse reactions promptly.

Adverse events (AEs) refer to harmful or unintended outcomes that occur after receiving medical treatment, including vaccines. No vaccine, medication, or medical device is entirely free from side effects. However, vaccines are essential in controlling and preventing widespread diseases, such as COVID-19, where their benefits far outweigh the risks. While most side effects are mild and temporary, serious reactions, though rare, can occur, including seizures or life-threatening allergic responses. It is essential for healthcare professionals and the public to be informed about potential risks to prevent and manage adverse events effectively.

Individuals who experience adverse reactions after receiving a vaccine are encouraged to report them to VAERS, even if they are unsure if the vaccine was the cause. This project leverages data from VAERS, a system designed by the FDA and CDC, to collect and analyze reports of vaccine-related adverse events, ensuring continuous vaccine safety monitoring and aiding in the early identification of potential risks.



