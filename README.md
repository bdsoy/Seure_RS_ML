# Seure_RS_ML
Seure recommendation system (3 models)

*\*erityisominaisuus 258 from employee side equals to 351 from customer side
This is so far the only one exception in erityisominaisuusvaatimus, all other erityisominaisuusid is treated as individual separately.*

### Current criteria taking into consideration:
- past 6 month employee work history
- Required erityisominaisuudet, employees' erityisominaisuudet and employee job titles
    - employee_taidot: employees' special feature ID
    - tyo_taidot: job title (ammattinimike)'s special feature ID
    - tilaus_taidot: order (tilaus tasolla)'s special feature ID
    - emp_amma: the job titles (ammattinimikkeet) that employee is eligible to do
- distance between employees and jobs
    - coordinate_dictionary: employees' coordinates
    - coordinate_dictionary_customer: customers' coordinates
- Black name list
    - tyontekija_sulkulista
    - asiakas_sulkulista
- available employees
    - emp_varattu: employees that have accepted a job offer or has been offered >= 5 offers are considered not available (currently checking only of today (the current day))
    - emp_add: Seure employees (Keikkakelpoinen työntekijä)
