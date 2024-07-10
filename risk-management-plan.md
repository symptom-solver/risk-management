# Risk Management Plan

## How to perform the risk analysis: 

We´re already certain about the functionality and structure of our application, therefore we can use the FMEA method to perform the
risk analysis. The approach of examining each component individually, thinking of all the errors that could possibly occur in it, 
is very suitable for our application, as it consists only of a limited number of non-complex components.
Also, FMEA is nicely dividable between Design FMEA (hazards caused by errors in the design) and Process FMEA (hazards caused by errors in the handling),
which makes a lot of sense for an application that deals with a diverse audience of non-professionals, resultingly having to focus specifically on 
false use of the software.
To ensure that during the analysis none of the potential errors are overlooked, the risk manager has to communicate with 
at least one person from every department that works on the product creation (e.g. backend- and frontend-developer) 
and at least one person working in usability management. 

Also, the risk analysis of similar applications like Symptomate or mayoclinic´s Symptom Checker has to be taken into account.

The gathered risks all have to be documented in a table structure with the columns Component, Error, Effect on the subsystem, Effect on the overall system and Possible harm.

## When the remaining risks are considered to be acceptable: 

Since the application doesn't diagnose but only aids in diagnosis and can only be used regarding non serious symptoms 
and their diseases, its benefits don't justice any high risk.
Therefore the remaining risks are only considered to be acceptable if their risks 
correspond to the following acceptability table, marking an acceptable harm with a,
nunanacceptable one with na.

|                               |            | **Severity of harm** |       |         |          |              |
|-------------------------------|------------|----------------------|-------|---------|----------|--------------|
|                               |            | Negligible           | Minor | Serious | Critical | Catastrophic |
| **Probability  of Occurence** | Often      | $\color{red}{\textsf{na}}$   | $\color{red}{\textsf{na}}$    | $\color{red}{\textsf{na}}$  | $\color{red}{\textsf{na}}$  | $\color{red}{\textsf{na}}$           |
|                               | Probable   | $\color{green}{\textsf{a}}$  | $\color{green}{\textsf{a}}$ | $\color{red}{\textsf{na}}$    | $\color{red}{\textsf{na}}$   | $\color{red}{\textsf{na}}$           |
|                               | Occasional | $\color{green}{\textsf{a}}$  | $\color{green}{\textsf{a}}$ | $\color{green}{\textsf{a}}$ | $\color{red}{\textsf{na}}$ | $\color{red}{\textsf{na}}$ |
|                               | Seldom     | $\color{green}{\textsf{a}}$  | $\color{green}{\textsf{a}}$ | $\color{green}{\textsf{a}}$ | $\color{red}{\textsf{na}}$ | $\color{red}{\textsf{na}}$ |
|                               | Unlikely   | $\color{green}{\textsf{a}}$  | $\color{green}{\textsf{a}}$ | $\color{green}{\textsf{a}}$ | $\color{green}{\textsf{a}}$ | $\color{green}{\textsf{a}}$       |

## Checking the implementation of risk mitigating measures: 

The employed risk manager is responsible for ensuring the complete implementation of each risk mitigating measure throughout the whole software lifecycle;
which involves reviewing the implementation of these measures with every software update, as well as information regarding a new risk.

If there were implemented any ways to check the effectiveness of a risk mitigating measure automatically (e.g. Unity tests in software),
a person qualified for that task needs to be assigned by its superior. If possible, this automatic testing should not only include
testing of the correct functionality of the risk mitigating measure, but also verification of it´s effectiveness after software deployment
by the collection of specific user data or similar.
The evaluation has to be reported, passed on to the risk manager and, based on his decision, potentially revised.

For the remaining types of risk mitigating measures the risk manager has to check if he´s either qualified to check them himself,
and therefore check them and write a report for the verification, or delegate this task to a more qualified person inside
or outside the company.

Additionally, there must be implemented an easy way for the user to provide feedback to the company. 
This feedback has to be reviewed regularly (at least once per week) by an assigned employee and passed on to the risk manager 
in case of any risk concerns.

After implementation of the risk mitigating measures, the risks have to be re-evaluated, which may cause the need of introducing
more or other risk mitigating measures. In the case of non-effective risk mitigating measures, they also have to be revised.



