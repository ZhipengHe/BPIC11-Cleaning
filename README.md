## BPIC2011 Cleaning

#### Event log Background

We have prepared a real-life log, taken from a Dutch Academic Hospital. This log contains some 150.000 events in over 1100 cases. Apart from some anonymization, the log contains all data as it came from the Hospital's systems. Each case is a patient of a Gynaecology department. The log contains information about when certain activities took place, which group performed the activity and so on. Many attributes have been recorded that are relevant to the process. Some attributes are repeated more than once for a patient, indicating that this patient went through different (maybe overlapping) phases, where a phase consists of the combination Diagnosis & Treatment.

[Find more information here](https://www.win.tue.nl/bpi/doku.php?id=2011:challenge)

#### Reference Paper

[BPIC2011 *J.C. Bose and W.M.P. van der Aalst* - Analysis of Patient Treatment Procedures](/paper/bose.pdf)

[BPIC2011 *F. Caron, J. Vanthienen, J. De Weerdt and B. Baesens* - Beyond X-Raying a Case-Flow: Adopting Different Focuses on Care-Flow Mining](/paper/caron.pdf)

[An Investigation of Interpretability Techniques for Deep Learning in PredictiveProcess Analytics for Healthcare](/paper/IEEE_XAI.pdf)

#### How xes files record event logs?

For example, 

```xml
<trace>
    <!-- Trace attributes -->
    <event>
        <!-- Event attributes -->
    </event>
    ...
</trace>
```

- Attributes for traces 
    - case:concept:name 
    - Age, Age:1-15
    - Diagnosis, Diagnosis:1-15
    - Diagnosis code, Diagnosis code:1-15
    - Treatment code, Treatment code:1-15
    - ~~Diagnosis Treatment Combination ID, Diagnosis Treatment Combination ID:1-15~~
    - ~~Specialism code, Specialism code:1-15~~
    - Start date, Start date:1-15
    - End date, End date:1-15


- Attributes for events
    - org:group
    - Number of executions
    - ~~Specialism code~~
    - event:concept:name
    - Producer code
    - Section
    - Activity code
    - time:timestamp
    - ~~lifecycle:transition~~


```xml
<!-- first trace -->
<!-- Phase 0, 1, 2 -->
<trace>
    <date key="End date" value="2006-01-04T23:45:36.000+01:00"/>
    <int key="Age" value="33"/>
    <int key="Treatment code:2" value="23"/>
    <int key="Treatment code:1" value="13"/>
    <int key="Diagnosis code:2" value="106"/>
    <!-- <int key="Specialism code" value="7"/> -->
    <int key="Diagnosis code:1" value="106"/>
    <int key="Treatment code" value="103"/>
    <string key="Diagnosis:2" value="Gynaecologische tumoren"/>
    <string key="Diagnosis:1" value="Gynaecologische tumoren"/>
    <string key="Diagnosis" value="maligniteit cervix"/>
    <!-- <int key="Diagnosis Treatment Combination ID" value="181229"/> -->
    <date key="Start date" value="2005-01-05T00:14:24.000+01:00"/>
    <!-- <int key="Diagnosis Treatment Combination ID:2" value="376908"/> -->
    <string key="Diagnosis code" value="M13"/>
    <!-- <int key="Diagnosis Treatment Combination ID:1" value="376907"/> -->
    <string key="concept:name" value="00000000"/>
    <date key="Start date:1" value="2005-01-03T00:14:24.000+01:00"/>
    <date key="End date:1" value="2005-01-29T23:45:36.000+01:00"/>
    <date key="End date:2" value="2005-01-29T23:45:36.000+01:00"/>
    <!-- <int key="Specialism code:1" value="61"/> -->
    <date key="Start date:2" value="2005-01-03T00:14:24.000+01:00"/>
    <!-- <int key="Specialism code:2" value="61"/> -->


    <event>
        <string key="org:group" value="Radiotherapy"/>
        <int key="Number of executions" value="1"/>
        <!-- <int key="Specialism code" value="61"/> -->
        <string key="concept:name" value="1e consult poliklinisch"/>
        <string key="Producer code" value="SRTH"/>
        <string key="Section" value="Section 5"/>
        <int key="Activity code" value="410100"/>
        <date key="time:timestamp" value="2005-01-03T00:00:00.000+01:00"/>
        <!-- <string key="lifecycle:transition" value="complete"/> -->
    </event>
    ...
</trace>
```