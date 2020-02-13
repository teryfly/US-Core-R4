This profile defines the recommended elements for the [Patient] resource.


### Minumum Recommended Data Elements


The following data-elements are recommended. They are presented below in a simple human-readable explanation.  Profile specific guidance and examples are provided as well.  The [Formal Profile Definition] below provides the  formal summary, definitions, and  terminology requirements.  

**Each Patient should have:**

1. a patient identifier (e.g. MRN)
1. a patient name
1. a gender*
1. contact detail (e.g. a telephone number or an email address)
1. a birth date
1. an address
1. a communication language
1. a race
1. an ethnicity
1. a birth sex*

**Profile specific implementation guidance:**

- \*The [FHIR Specification]({{site.data.fhir.path}}patient.html#gender) provides guidance and background for representing patient gender. The American Clinical Laboratory Association (ACLA) has published [best practice guidelines](http://www.acla.com/acla-best-practice-recommendation-for-administrative-and-clinical-patient-gender-used-for-laboratory-testing-and-reporting/) for administrative and clinical gender related to laboratory testing and reporting which implementers may find helpful as well.

### Examples

- [Patient-example](Patient-example.html)


{% include link-list.md %}
