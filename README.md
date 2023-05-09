# Landing

A text-mining based tool to help student with finding the most compatible job post based on their past experiences and interesrs as well as optimizing their resume by a keyword suggesting system.

## Introduction 

Recent statistics show that 75% of applicants are filtered out from applicant pools for a position by the Applicant Tracking System due to the inflexi- bility of machines in understanding different resume formats and wordings. The gloomy scenery of the job market in general, adding to the inclining competitiveness in the tech job market makes it much harder for candidates to successfully land their dream job. Thus, it is important to examine and form a tool that can assist new graduates, the most vulnerable individu- als in the job market, to elevate their employment prospects. Lander is a text-mining-based tool that helps the student increase their chance of pass- ing the initial resume screening round by optimizing their resume using a keyword-suggesting system. Moreover, Lander will also match a candidate to a compatible job by matching the experience in their resume to a job description, and in return, increase the chance of getting accepted into the job.

## Motivation

With the detrimental effect of Covid-19, the job market has become extremely competitive for the last 3 years, especially for newly graduated candidates. During the summer of my freshman year, I was working as an intern for Talent Acquisition Service Office of a renowned bank back in Vietnam. In there, I have witnessed so many fresh candidates at a renowned bank in Vietnam. In there, I have witnessed so many fresh candidates who apply to a myriad of jobs without actually knowing what they want to do or what they are good at. Then, when I came back to America, a lot of seniors back then also tell me that they had the same problem. At that time, I realize that the struggle in job hunting is a worldwide problem.

Thus, my dream since then was to create a platform where fresh candidates can find what is the most suitable job they should apply to based on their past experiences and interests. In addition, I want to help them tailor their resume based on the job description of their dream job to enhance their chance of getting through the initial scanning round.  

## Technical Details

The pipeline of Lander consists of two main steps:

1. Match candidates to a cluster of job title in a job banks using Kmean prediction: clusters of job titles are determined by the similarity in the keyword and skills highlighted in their job description.
2. Match candidates to top jobs within the cluster using Cosine Similarity and Phrase Matching
3. Give resume optimization suggestions

## Execution method:

1. Step 1: Clone the repository using:

```
git clone git@github.com:Mai1902/landing.git
```

2. Step 2: Install all necessary dependencies using:

```
poetry install
```

3. Run the artifact using:

```
streamlit run streamlit_setup.py
```

## References

[Jobscan](https://www.jobscan.co)
[Resource for Resume Optimization Methodology](https://towardsdatascience.com/ai-is-working-against-your-job-application-bec65d496d22)
[Dataset](https://www.kaggle.com/datasets/PromptCloudHQ/us-technology-jobs-on-dicecom)
