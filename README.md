# <u>Content Package of the demo data in the Reference Application</u>

This content package contains all the demo metadata for the reference application. 
🎁 Think of this like a **“starter kit”**, as it contains the metadata set-up that most teams would need (e.g. common Labs, Diagnoses, Drugs, etc). 

We still recommend that teams review configuration for accuracy and appropriateness before launching an EMR in production. 

⚠️ NOTE: The baseline metadata _required_ to run a version of O3 is found in the [Reference Application Content Package](https://github.com/openmrs/openmrs-content-referenceapplication).

## What's here

Metadata a site is expected to supply or replace, plus the demo data that fills out the O3 demo environments:

- Locations — `Ubuntu Hospital` with its clinics and wards, and `Site 1`–`Site 50`.
- The demo programs, the demo forms and their translations, service queues, and appointment specialities and services.
- The catalogs a site brings its own version of: the formulary (`BasicDrugs` and the drug concepts), the lab
  tests (`BasicLabTests`, the `Tests Orderability` set and the Hb/ALP reference ranges), the diagnoses and the
  procedures.
- Billing sample data, the address hierarchy, and the demo locale list.
- `referencedemodata.createDemoPatientsOnNextStartup`, which generates the demo patients.

The metadata O3 features reference directly — identifier types and their generator, encounter and visit types,
roles, the emrapi term mappings, dispositions, order frequencies, dosing units and the vital sign concepts —
now lives in the [Reference Application Content Package](https://github.com/openmrs/openmrs-content-referenceapplication)
instead, so that a distribution can leave this package out and still run.
