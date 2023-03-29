---
title: Using Configurations in Qase TMS
slug: using-configurations-in-qase-tms
hidden: true
createdAt: '2023-02-24T12:46:08.263Z'
updatedAt: '2023-02-24T12:46:08.263Z'
---

# Configurations

### What are configurations used for?

Configurations can be used to specify for any test run, which hardware or software configuration this run should be performed on.

{% embed url="https://youtu.be/msObZRlBYmM" %}

### How to create a configuration group?

Configuration groups are found in projects:

<figure><img src="https://qase.intercom-attachments-7.com/i/o/595215836/52c6c4af6446cf6df64b804e/HU8Z-223GJA3z2xRF6SvnKBcz0d88Olj8zPIdy6ZTwb3bNbpeU7F-_R7xsAqkqVnilJUPzMRNuautk2AyMs8VMSx_1sZ3dJ8t1OuOMb6E3Sv5le35zwnu2Y2yl8yQjZUkRzz_n0b3aFSK4IU_Q_C8ke8J3CrGFDmRQVligs2Q_-2C7zY-t5wbqUzDQ" alt=""><figcaption></figcaption></figure>

Imagine you're testing a web app in different browsers. To do that, make a "Browsers" group and list all the browsers you'll be testing with.

<figure><img src="https://qase.intercom-attachments-7.com/i/o/595215844/9bc6c39eded26c20995d3df7/sUADxj175aLzfYS2gj1FxmOIR0E2qf9qO2Wo6ao2HLuPCQ8TRQtKNxSSenECaZ785ORAIsM7h23riBobLFIKj95AqLuOO0RZi0ix7_RCi4rSdNGuQ003ltvHVFxkD9oJ1suouVcQsT98uXuZT1Ajpl18czwp3Qs2Pxp1inQidiPf-nwq5ZK-81xeJA" alt=""><figcaption></figcaption></figure>

<figure><img src="https://qase.intercom-attachments-7.com/i/o/595215852/f98d0b96c62c0fb7c970ca29/ksmqTRubshnwLQpILB4PntBKmN4rEZcuzV_oG28xGaXZKJ5U_ki1VUywtmn-EN0FlkC-DRv_DOFXIYk9jQmZd1S2Wg9qNYbZ8C5n3jfQZ8BaPgHRatJ5-6qN-7Z4AJHAhuVN7MJq3h5hNe9ZL9ipIK3xB7Ta1T3KG-6coNfcGq3pQhVikgXMzKma1w" alt=""><figcaption></figcaption></figure>

<figure><img src="https://qase.intercom-attachments-7.com/i/o/595215858/c19a57502213772231d0fca0/KX9VZ9_UGdFrTyO_B_Rr0vMezDIkO4uDcedcZL_eac8A3Wm4K9PZmspYddBU2DIsK_mVguuAyOdUNXWh-DE9IsEYoOGg2Oxskli9EqZhe96x_RYiOHpbQLGrDPFIT8vOOZ-Ys8qtr1AWJTY2o37ky6GAomNnunwR86vRDvsAzCv6XcKkcha70k7Fcw" alt=""><figcaption></figcaption></figure>

Once your configuration group has been created, and you've added all possible individual configurations to test on, you can now specify this while preparing a test run - all available configuration groups will be shown in the "Configurations" section:

<figure><img src="https://qase.intercom-attachments-7.com/i/o/595215873/d9cca42eab462702e76494ca/7kA2dQTfG4PGrjUaP9rHqYPMYyT9iGBuvFsDQJlMtzUp4_VGbfdkVPC5sycB2ZYIRzgDsG7sS3wAKJtVyZ-HOO-tdIsmy55ftH9JRXu1-nkCTUwVKJYe-NYSKdHC2Axsv1yhShbt3z-JOd2JREsGkQ3eHjvfcS0KVzlOjmHg_boYJCFRrPzAGUX8Lw" alt=""><figcaption></figcaption></figure>

You can create multiple configuration groups and have combinations of, for example, different browsers and different OS:

<figure><img src="https://qase.intercom-attachments-7.com/i/o/595215882/79c93e254d50cdcb59ff01e6/gbQwA0ICbXU2odWNc2rsASg_KryJmxL2AnxVBm2NQL5oOEd6h6j1gQqwL0vCVFD9GIZymOlYmL7GwucHWLivrNA3ccRLtEPBNBxobYIRz2bmIDmjz0Lnka1yMZ2eUQJCErfBUwPmxNkwMgs67TmYyQoKVPboOakUMlLSGTs9h8ZPl1rr0lO-oUIlSQ" alt=""><figcaption></figcaption></figure>

You can also edit or delete both configuration groups and individual configurations after having created them:

<figure><img src="https://qase.intercom-attachments-7.com/i/o/595215888/e409e5b1c8567a0069352f78/akJKc2xTD9Z8wPbM_r79Y4U8OU279-cxl3rnUfU4RzUGyHC-4VGZn53rbFXEEnLJmMmm8UnNbPWLhm3jyJ5s5jvL_vuYitXGIrtUHJ9CEgQt2utooBONtbFAABe0FuY2QGCkGRyvD6646g0fAmS1bwQnqSu7zpuMRA_G1qfWB_KZrMbnHQq-YcshdQ" alt=""><figcaption></figcaption></figure>
