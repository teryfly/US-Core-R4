This profile sets minimum expectations for the [Observation] resource to record, search, and fetch pediatric head occipital frontal circumference (OFC) percentile observations associated with a patients from birth to 37 Months of age. It is based on the FHIR [Vital Signs Profile] and identifies the *additional* mandatory core elements, extensions, vocabularies and value sets which **SHALL** be present in the Observation resource when using this profile.

**Example Usage Scenarios:**

The following are example usage scenarios for the US Core Pediatric Head Occipital Frontal Circumference Percentile Profile:

- Query for OFC percentile observation belonging to a pediatric patient
- [Record or update] OFC percentile observations belonging to a pediatric patient

### Mandatory and Must Support Data Elements

In addition to the mandatory and must support data elements in the FHIR Vital Signs Profile, the following data-elements are mandatory (i.e data MUST be present) or must be supported if the data is present in the sending system ([Must Support] definition). They are presented below in a simple human-readable explanation.  Profile specific guidance and examples are provided as well.  The [Formal Profile Definition] below provides the  formal summary, definitions, and  terminology requirements.

**Each Observation must have:**

1.  a fixed code for head occipital frontal circumference percentile measurement

**Each Observation must support:**

1.  a result value

**Profile specific implementation guidance:**

- An Observation without a value, **SHALL** include a reason why the data is absent unless there are component observations, or references to other Observations that are grouped within it.
- The Observation.subject **SHALL** conform to [US Core Patient Profile].
- Information about the growth chart tables used to determine percentiles should be supplied in `Observation.note.text` (for example, 'WHO Males, 0-2 years Chart').
- For representing the raw OFC measurements use the FHIR Vital Signs [Head Circumference] Profile.

### Examples

- [OFC Percentile Example](Observation-ofc-percentile.html)

{% include link-list.md %}
