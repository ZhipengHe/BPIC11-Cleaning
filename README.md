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
    <date key="End date" value="2006-01-04T23:45:36.000+01:00"/>
    <int key="Age" value="33"/>
    <int key="Treatment code:2" value="23"/>
    <int key="Treatment code:1" value="13"/>
    <int key="Diagnosis code:2" value="106"/>
    <int key="Specialism code" value="7"/>
    <int key="Diagnosis code:1" value="106"/>
    <int key="Treatment code" value="103"/>
    <string key="Diagnosis:2" value="Gynaecologische tumoren"/>
    <string key="Diagnosis:1" value="Gynaecologische tumoren"/>
    <string key="Diagnosis" value="maligniteit cervix"/>
    <int key="Diagnosis Treatment Combination ID" value="181229"/>
    <date key="Start date" value="2005-01-05T00:14:24.000+01:00"/>
    <int key="Diagnosis Treatment Combination ID:2" value="376908"/>
    <string key="Diagnosis code" value="M13"/>
    <int key="Diagnosis Treatment Combination ID:1" value="376907"/>
    <string key="concept:name" value="00000000"/>
    <date key="Start date:1" value="2005-01-03T00:14:24.000+01:00"/>
    <date key="End date:1" value="2005-01-29T23:45:36.000+01:00"/>
    <date key="End date:2" value="2005-01-29T23:45:36.000+01:00"/>
    <int key="Specialism code:1" value="61"/>
    <date key="Start date:2" value="2005-01-03T00:14:24.000+01:00"/>
    <int key="Specialism code:2" value="61"/>
    <event>
        <string key="org:group" value="Radiotherapy"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="61"/>
        <string key="concept:name" value="1e consult poliklinisch"/>
        <string key="Producer code" value="SRTH"/>
        <string key="Section" value="Section 5"/>
        <int key="Activity code" value="410100"/>
        <date key="time:timestamp" value="2005-01-03T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="Radiotherapy"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="61"/>
        <string key="concept:name" value="administratief tarief       - eerste pol"/>
        <string key="Producer code" value="SRTH"/>
        <string key="Section" value="Section 5"/>
        <int key="Activity code" value="419100"/>
        <date key="time:timestamp" value="2005-01-03T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="Nursing ward"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="7"/>
        <string key="concept:name" value="verlosk.-gynaec. korte kaart kosten-out"/>
        <string key="Producer code" value="SGEH"/>
        <string key="Section" value="Section 2"/>
        <int key="Activity code" value="10107"/>
        <date key="time:timestamp" value="2005-01-05T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="Obstetrics &amp; Gynaecology clinic"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="7"/>
        <string key="concept:name" value="echografie  - genitalia interna"/>
        <string key="Producer code" value="SGEC"/>
        <string key="Section" value="Section 2"/>
        <string key="Activity code" value="339486E"/>
        <date key="time:timestamp" value="2005-01-05T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="Nursing ward"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="7"/>
        <string key="concept:name" value="1e consult poliklinisch"/>
        <string key="Producer code" value="SGEH"/>
        <string key="Section" value="Section 2"/>
        <int key="Activity code" value="410100"/>
        <date key="time:timestamp" value="2005-01-05T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="Nursing ward"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="7"/>
        <string key="concept:name" value="administratief tarief       - eerste pol"/>
        <string key="Producer code" value="SGEH"/>
        <string key="Section" value="Section 2"/>
        <int key="Activity code" value="419100"/>
        <date key="time:timestamp" value="2005-01-05T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="Radiotherapy"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="61"/>
        <string key="concept:name" value="simulator - gebruik voor aanvang megavol"/>
        <string key="Producer code" value="RATH"/>
        <string key="Section" value="Section 5"/>
        <int key="Activity code" value="390520"/>
        <date key="time:timestamp" value="2005-01-24T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="Radiotherapy"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="61"/>
        <string key="concept:name" value="behandeltijd - eenheid t3 - megavolt"/>
        <string key="Producer code" value="RATH"/>
        <string key="Section" value="Section 5"/>
        <int key="Activity code" value="390003"/>
        <date key="time:timestamp" value="2005-01-31T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="Radiotherapy"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="61"/>
        <string key="concept:name" value="teletherapie - megavolt fotonen bestrali"/>
        <string key="Producer code" value="RATH"/>
        <string key="Section" value="Section 5"/>
        <int key="Activity code" value="390550"/>
        <date key="time:timestamp" value="2005-01-31T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="General Lab Clinical Chemistry"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="86"/>
        <string key="concept:name" value="aanname laboratoriumonderzoek"/>
        <string key="Producer code" value="CRLA"/>
        <string key="Section" value="Section 4"/>
        <int key="Activity code" value="370000"/>
        <date key="time:timestamp" value="2005-02-15T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="General Lab Clinical Chemistry"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="86"/>
        <string key="concept:name" value="aanname laboratoriumonderzoek"/>
        <string key="Producer code" value="CRLA"/>
        <string key="Section" value="Section 4"/>
        <int key="Activity code" value="370000"/>
        <date key="time:timestamp" value="2005-02-15T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="General Lab Clinical Chemistry"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="86"/>
        <string key="concept:name" value="ureum"/>
        <string key="Producer code" value="CHE2"/>
        <string key="Section" value="Section 4"/>
        <int key="Activity code" value="370403"/>
        <date key="time:timestamp" value="2005-02-15T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="General Lab Clinical Chemistry"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="86"/>
        <string key="concept:name" value="hemoglobine foto-elektrisch"/>
        <string key="Producer code" value="HAEM"/>
        <string key="Section" value="Section 4"/>
        <float key="Activity code" value="370407.0"/>
        <date key="time:timestamp" value="2005-02-15T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="General Lab Clinical Chemistry"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="86"/>
        <string key="concept:name" value="creatinine"/>
        <string key="Producer code" value="CHE2"/>
        <string key="Section" value="Section 4"/>
        <int key="Activity code" value="370419"/>
        <date key="time:timestamp" value="2005-02-15T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="General Lab Clinical Chemistry"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="86"/>
        <string key="concept:name" value="natrium vlamfotometrisch"/>
        <string key="Producer code" value="CHE2"/>
        <string key="Section" value="Section 4"/>
        <int key="Activity code" value="370442"/>
        <date key="time:timestamp" value="2005-02-15T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="General Lab Clinical Chemistry"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="86"/>
        <string key="concept:name" value="kalium potentiometrisch"/>
        <string key="Producer code" value="CHE2"/>
        <string key="Section" value="Section 4"/>
        <int key="Activity code" value="370443"/>
        <date key="time:timestamp" value="2005-02-15T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="General Lab Clinical Chemistry"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="86"/>
        <string key="concept:name" value="leukocyten tellen elektronisch"/>
        <string key="Producer code" value="HAEM"/>
        <string key="Section" value="Section 4"/>
        <string key="Activity code" value="370712B"/>
        <date key="time:timestamp" value="2005-02-15T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="General Lab Clinical Chemistry"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="86"/>
        <string key="concept:name" value="trombocyten tellen - elektronisch"/>
        <string key="Producer code" value="HAEM"/>
        <string key="Section" value="Section 4"/>
        <string key="Activity code" value="370715A"/>
        <date key="time:timestamp" value="2005-02-15T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="General Lab Clinical Chemistry"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="86"/>
        <string key="concept:name" value="ordertarief"/>
        <string key="Producer code" value="CRLA"/>
        <string key="Section" value="Section 4"/>
        <int key="Activity code" value="379999"/>
        <date key="time:timestamp" value="2005-02-15T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="Nursing ward"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="7"/>
        <string key="concept:name" value="ligdagen - alle spec.beh.kinderg.-reval."/>
        <string key="Producer code" value="H5ZU"/>
        <string key="Section" value="Section 2"/>
        <int key="Activity code" value="40014"/>
        <date key="time:timestamp" value="2005-02-17T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="Medical Microbiology"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="87"/>
        <string key="concept:name" value="aanname laboratoriumonderzoek"/>
        <string key="Producer code" value="LBAC"/>
        <string key="Section" value="Section 4"/>
        <int key="Activity code" value="370000"/>
        <date key="time:timestamp" value="2005-02-17T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="General Lab Clinical Chemistry"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="86"/>
        <string key="concept:name" value="aanname laboratoriumonderzoek"/>
        <string key="Producer code" value="CRLA"/>
        <string key="Section" value="Section 4"/>
        <int key="Activity code" value="370000"/>
        <date key="time:timestamp" value="2005-02-17T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="General Lab Clinical Chemistry"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="86"/>
        <string key="concept:name" value="sediment - spoed"/>
        <string key="Producer code" value="URIN"/>
        <string key="Section" value="Section 4"/>
        <string key="Activity code" value="370111S"/>
        <date key="time:timestamp" value="2005-02-17T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="Medical Microbiology"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="87"/>
        <string key="concept:name" value="bacteriologisch onderzoek met kweek -nie"/>
        <string key="Producer code" value="LBAC"/>
        <string key="Section" value="Section 4"/>
        <string key="Activity code" value="370504A"/>
        <date key="time:timestamp" value="2005-02-17T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="Medical Microbiology"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="87"/>
        <string key="concept:name" value="bacteriologisch onderzoek met kweek -nie"/>
        <string key="Producer code" value="LBAC"/>
        <string key="Section" value="Section 4"/>
        <string key="Activity code" value="370504A"/>
        <date key="time:timestamp" value="2005-02-17T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="Medical Microbiology"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="87"/>
        <string key="concept:name" value="bacteriologisch onderzoek met kweek -nie"/>
        <string key="Producer code" value="LBAC"/>
        <string key="Section" value="Section 4"/>
        <string key="Activity code" value="370504A"/>
        <date key="time:timestamp" value="2005-02-17T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="Medical Microbiology"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="87"/>
        <string key="concept:name" value="resistentiebepalingen - 5 bepalingen"/>
        <string key="Producer code" value="LBAC"/>
        <string key="Section" value="Section 4"/>
        <string key="Activity code" value="370505A"/>
        <date key="time:timestamp" value="2005-02-17T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="Medical Microbiology"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="87"/>
        <string key="concept:name" value="resistentiebepalingen - 5 bepalingen"/>
        <string key="Producer code" value="LBAC"/>
        <string key="Section" value="Section 4"/>
        <string key="Activity code" value="370505A"/>
        <date key="time:timestamp" value="2005-02-17T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="Medical Microbiology"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="87"/>
        <string key="concept:name" value="hepatitis-b surface antigeen confirmatie"/>
        <string key="Producer code" value="LBAC"/>
        <string key="Section" value="Section 4"/>
        <string key="Activity code" value="375138A"/>
        <date key="time:timestamp" value="2005-02-17T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="Medical Microbiology"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="87"/>
        <string key="concept:name" value="hepatitis-b surface antigeen confirmatie"/>
        <string key="Producer code" value="LBAC"/>
        <string key="Section" value="Section 4"/>
        <string key="Activity code" value="375138A"/>
        <date key="time:timestamp" value="2005-02-17T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="General Lab Clinical Chemistry"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="86"/>
        <string key="concept:name" value="urine onderzoek - kwalitatief"/>
        <string key="Producer code" value="URIN"/>
        <string key="Section" value="Section 4"/>
        <int key="Activity code" value="378149"/>
        <date key="time:timestamp" value="2005-02-17T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="General Lab Clinical Chemistry"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="86"/>
        <string key="concept:name" value="ordertarief"/>
        <string key="Producer code" value="CRLA"/>
        <string key="Section" value="Section 4"/>
        <int key="Activity code" value="379999"/>
        <date key="time:timestamp" value="2005-02-17T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="Nursing ward"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="7"/>
        <string key="concept:name" value="190021 klinische opname a002"/>
        <string key="Producer code" value="H5ZU"/>
        <string key="Section" value="Section 2"/>
        <int key="Activity code" value="610001"/>
        <date key="time:timestamp" value="2005-02-17T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="Nursing ward"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="7"/>
        <string key="concept:name" value="190205 klasse 3b        a205"/>
        <string key="Producer code" value="H5ZU"/>
        <string key="Section" value="Section 2"/>
        <int key="Activity code" value="613000"/>
        <date key="time:timestamp" value="2005-02-17T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="Nursing ward"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="7"/>
        <string key="concept:name" value="ligdagen - alle spec.beh.kinderg.-reval."/>
        <string key="Producer code" value="H5ZU"/>
        <string key="Section" value="Section 2"/>
        <int key="Activity code" value="40014"/>
        <date key="time:timestamp" value="2005-02-18T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="General Lab Clinical Chemistry"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="86"/>
        <string key="concept:name" value="aanname laboratoriumonderzoek"/>
        <string key="Producer code" value="CRLA"/>
        <string key="Section" value="Section 4"/>
        <int key="Activity code" value="370000"/>
        <date key="time:timestamp" value="2005-02-18T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="General Lab Clinical Chemistry"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="86"/>
        <string key="concept:name" value="aanname laboratoriumonderzoek"/>
        <string key="Producer code" value="CRLA"/>
        <string key="Section" value="Section 4"/>
        <int key="Activity code" value="370000"/>
        <date key="time:timestamp" value="2005-02-18T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="General Lab Clinical Chemistry"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="86"/>
        <string key="concept:name" value="ureum"/>
        <string key="Producer code" value="CHE2"/>
        <string key="Section" value="Section 4"/>
        <int key="Activity code" value="370403"/>
        <date key="time:timestamp" value="2005-02-18T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="General Lab Clinical Chemistry"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="86"/>
        <string key="concept:name" value="hemoglobine foto-elektrisch"/>
        <string key="Producer code" value="HAEM"/>
        <string key="Section" value="Section 4"/>
        <float key="Activity code" value="370407.0"/>
        <date key="time:timestamp" value="2005-02-18T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="General Lab Clinical Chemistry"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="86"/>
        <string key="concept:name" value="creatinine"/>
        <string key="Producer code" value="CHE2"/>
        <string key="Section" value="Section 4"/>
        <int key="Activity code" value="370419"/>
        <date key="time:timestamp" value="2005-02-18T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="General Lab Clinical Chemistry"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="86"/>
        <string key="concept:name" value="natrium vlamfotometrisch"/>
        <string key="Producer code" value="CHE2"/>
        <string key="Section" value="Section 4"/>
        <int key="Activity code" value="370442"/>
        <date key="time:timestamp" value="2005-02-18T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="General Lab Clinical Chemistry"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="86"/>
        <string key="concept:name" value="kalium potentiometrisch"/>
        <string key="Producer code" value="CHE2"/>
        <string key="Section" value="Section 4"/>
        <int key="Activity code" value="370443"/>
        <date key="time:timestamp" value="2005-02-18T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="General Lab Clinical Chemistry"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="86"/>
        <string key="concept:name" value="sgot - asat kinetisch"/>
        <string key="Producer code" value="CHE2"/>
        <string key="Section" value="Section 4"/>
        <string key="Activity code" value="370488E"/>
        <date key="time:timestamp" value="2005-02-18T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="General Lab Clinical Chemistry"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="86"/>
        <string key="concept:name" value="sgpt - alat kinetisch"/>
        <string key="Producer code" value="CHE2"/>
        <string key="Section" value="Section 4"/>
        <string key="Activity code" value="370488G"/>
        <date key="time:timestamp" value="2005-02-18T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="General Lab Clinical Chemistry"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="86"/>
        <string key="concept:name" value="melkzuurdehydrogenase -ldh- kinetisch"/>
        <string key="Producer code" value="CHE2"/>
        <string key="Section" value="Section 4"/>
        <string key="Activity code" value="370488J"/>
        <date key="time:timestamp" value="2005-02-18T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="General Lab Clinical Chemistry"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="86"/>
        <string key="concept:name" value="differentiele telling automatisch"/>
        <string key="Producer code" value="HAEM"/>
        <string key="Section" value="Section 4"/>
        <int key="Activity code" value="370701"/>
        <date key="time:timestamp" value="2005-02-18T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="General Lab Clinical Chemistry"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="86"/>
        <string key="concept:name" value="leukocyten tellen elektronisch"/>
        <string key="Producer code" value="HAEM"/>
        <string key="Section" value="Section 4"/>
        <string key="Activity code" value="370712B"/>
        <date key="time:timestamp" value="2005-02-18T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="General Lab Clinical Chemistry"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="86"/>
        <string key="concept:name" value="trombocyten tellen - elektronisch"/>
        <string key="Producer code" value="HAEM"/>
        <string key="Section" value="Section 4"/>
        <string key="Activity code" value="370715A"/>
        <date key="time:timestamp" value="2005-02-18T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="General Lab Clinical Chemistry"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="86"/>
        <string key="concept:name" value="trombotest"/>
        <string key="Producer code" value="STOL"/>
        <string key="Section" value="Section 4"/>
        <int key="Activity code" value="375518"/>
        <date key="time:timestamp" value="2005-02-18T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="General Lab Clinical Chemistry"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="86"/>
        <string key="concept:name" value="crp c-reactief proteine"/>
        <string key="Producer code" value="CHE2"/>
        <string key="Section" value="Section 4"/>
        <int key="Activity code" value="378452"/>
        <date key="time:timestamp" value="2005-02-18T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="General Lab Clinical Chemistry"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="86"/>
        <string key="concept:name" value="ordertarief"/>
        <string key="Producer code" value="CRLA"/>
        <string key="Section" value="Section 4"/>
        <int key="Activity code" value="379999"/>
        <date key="time:timestamp" value="2005-02-18T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="Nursing ward"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="7"/>
        <string key="concept:name" value="190205 klasse 3b        a205"/>
        <string key="Producer code" value="H5ZU"/>
        <string key="Section" value="Section 2"/>
        <int key="Activity code" value="613000"/>
        <date key="time:timestamp" value="2005-02-18T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="Nursing ward"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="7"/>
        <string key="concept:name" value="ligdagen - alle spec.beh.kinderg.-reval."/>
        <string key="Producer code" value="H5ZU"/>
        <string key="Section" value="Section 2"/>
        <int key="Activity code" value="40014"/>
        <date key="time:timestamp" value="2005-02-19T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="Nursing ward"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="7"/>
        <string key="concept:name" value="190205 klasse 3b        a205"/>
        <string key="Producer code" value="H5ZU"/>
        <string key="Section" value="Section 2"/>
        <int key="Activity code" value="613000"/>
        <date key="time:timestamp" value="2005-02-19T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="Nursing ward"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="7"/>
        <string key="concept:name" value="ligdagen - alle spec.beh.kinderg.-reval."/>
        <string key="Producer code" value="H5ZU"/>
        <string key="Section" value="Section 2"/>
        <int key="Activity code" value="40014"/>
        <date key="time:timestamp" value="2005-02-20T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="Nursing ward"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="7"/>
        <string key="concept:name" value="190205 klasse 3b        a205"/>
        <string key="Producer code" value="H5ZU"/>
        <string key="Section" value="Section 2"/>
        <int key="Activity code" value="613000"/>
        <date key="time:timestamp" value="2005-02-20T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="Nursing ward"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="7"/>
        <string key="concept:name" value="ligdagen - alle spec.beh.kinderg.-reval."/>
        <string key="Producer code" value="H5ZU"/>
        <string key="Section" value="Section 2"/>
        <int key="Activity code" value="40014"/>
        <date key="time:timestamp" value="2005-02-21T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="General Lab Clinical Chemistry"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="86"/>
        <string key="concept:name" value="aanname laboratoriumonderzoek"/>
        <string key="Producer code" value="CRLA"/>
        <string key="Section" value="Section 4"/>
        <int key="Activity code" value="370000"/>
        <date key="time:timestamp" value="2005-02-21T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="General Lab Clinical Chemistry"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="86"/>
        <string key="concept:name" value="trombotest"/>
        <string key="Producer code" value="STOL"/>
        <string key="Section" value="Section 4"/>
        <int key="Activity code" value="375518"/>
        <date key="time:timestamp" value="2005-02-21T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="General Lab Clinical Chemistry"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="86"/>
        <string key="concept:name" value="ordertarief"/>
        <string key="Producer code" value="CRLA"/>
        <string key="Section" value="Section 4"/>
        <int key="Activity code" value="379999"/>
        <date key="time:timestamp" value="2005-02-21T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="Nursing ward"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="7"/>
        <string key="concept:name" value="190205 klasse 3b        a205"/>
        <string key="Producer code" value="H5ZU"/>
        <string key="Section" value="Section 2"/>
        <int key="Activity code" value="613000"/>
        <date key="time:timestamp" value="2005-02-21T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="Nursing ward"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="7"/>
        <string key="concept:name" value="ligdagen - alle spec.beh.kinderg.-reval."/>
        <string key="Producer code" value="H5ZU"/>
        <string key="Section" value="Section 2"/>
        <int key="Activity code" value="40014"/>
        <date key="time:timestamp" value="2005-02-22T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="Nursing ward"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="7"/>
        <string key="concept:name" value="190205 klasse 3b        a205"/>
        <string key="Producer code" value="H5ZU"/>
        <string key="Section" value="Section 2"/>
        <int key="Activity code" value="613000"/>
        <date key="time:timestamp" value="2005-02-22T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="Nursing ward"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="61"/>
        <string key="concept:name" value="ligdagen - alle spec.beh.kinderg.-reval."/>
        <string key="Producer code" value="F5NO"/>
        <string key="Section" value="Section 1"/>
        <int key="Activity code" value="40014"/>
        <date key="time:timestamp" value="2005-03-07T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="Nursing ward"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="61"/>
        <string key="concept:name" value="190021 klinische opname a002"/>
        <string key="Producer code" value="F5NO"/>
        <string key="Section" value="Section 1"/>
        <int key="Activity code" value="610001"/>
        <date key="time:timestamp" value="2005-03-07T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="Nursing ward"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="61"/>
        <string key="concept:name" value="ligdagen - alle spec.beh.kinderg.-reval."/>
        <string key="Producer code" value="F5NO"/>
        <string key="Section" value="Section 1"/>
        <int key="Activity code" value="40014"/>
        <date key="time:timestamp" value="2005-03-08T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="Radiotherapy"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="61"/>
        <string key="concept:name" value="brachytherapie - interstitieel - intensi"/>
        <string key="Producer code" value="RATH"/>
        <string key="Section" value="Section 5"/>
        <int key="Activity code" value="390183"/>
        <date key="time:timestamp" value="2005-03-08T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="Nursing ward"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="61"/>
        <string key="concept:name" value="190205 klasse 3b        a205"/>
        <string key="Producer code" value="F5NO"/>
        <string key="Section" value="Section 1"/>
        <int key="Activity code" value="613000"/>
        <date key="time:timestamp" value="2005-03-08T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="Nursing ward"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="61"/>
        <string key="concept:name" value="ligdagen - alle spec.beh.kinderg.-reval."/>
        <string key="Producer code" value="F5NO"/>
        <string key="Section" value="Section 1"/>
        <int key="Activity code" value="40014"/>
        <date key="time:timestamp" value="2005-03-09T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="Nursing ward"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="61"/>
        <string key="concept:name" value="190205 klasse 3b        a205"/>
        <string key="Producer code" value="F5NO"/>
        <string key="Section" value="Section 1"/>
        <int key="Activity code" value="613000"/>
        <date key="time:timestamp" value="2005-03-09T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="Medical Microbiology"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="87"/>
        <string key="concept:name" value="aanname laboratoriumonderzoek"/>
        <string key="Producer code" value="LBAC"/>
        <string key="Section" value="Section 4"/>
        <int key="Activity code" value="370000"/>
        <date key="time:timestamp" value="2005-03-10T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="Medical Microbiology"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="87"/>
        <string key="concept:name" value="bacteriologisch onderzoek met kweek -nie"/>
        <string key="Producer code" value="LBAC"/>
        <string key="Section" value="Section 4"/>
        <string key="Activity code" value="370504A"/>
        <date key="time:timestamp" value="2005-03-10T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="Medical Microbiology"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="87"/>
        <string key="concept:name" value="resistentiebepalingen - 5 bepalingen"/>
        <string key="Producer code" value="LBAC"/>
        <string key="Section" value="Section 4"/>
        <string key="Activity code" value="370505A"/>
        <date key="time:timestamp" value="2005-03-10T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="Medical Microbiology"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="87"/>
        <string key="concept:name" value="hepatitis-b surface antigeen confirmatie"/>
        <string key="Producer code" value="LBAC"/>
        <string key="Section" value="Section 4"/>
        <string key="Activity code" value="375138A"/>
        <date key="time:timestamp" value="2005-03-10T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
    <event>
        <string key="org:group" value="General Lab Clinical Chemistry"/>
        <int key="Number of executions" value="1"/>
        <int key="Specialism code" value="86"/>
        <string key="concept:name" value="ordertarief"/>
        <string key="Producer code" value="CRLA"/>
        <string key="Section" value="Section 4"/>
        <int key="Activity code" value="379999"/>
        <date key="time:timestamp" value="2005-03-10T00:00:00.000+01:00"/>
        <string key="lifecycle:transition" value="complete"/>
    </event>
</trace>

```