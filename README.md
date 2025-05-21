# Supplementary Materials for  
**Service-aware password risk meter – Helping users to choose suitable passwords in services**

**Authors:**  
Roi Sánchez Serna [[ORCID: 0009-0001-6424-8262]](https://orcid.org/0009-0001-6424-8262)  
Ana I. González-Tablas [[ORCID: 2222-3333-4444-5555]](https://orcid.org/2222-3333-4444-5555)  
Lorena González Manzano [[ORCID: 1111-2222-3333-4444]](https://orcid.org/1111-2222-3333-4444)  
Jose María de Fuentes [[ORCID: 2222-3333-4444-5555]](https://orcid.org/2222-3333-4444-5555)  

**Affiliation:**  
Universidad Carlos III de Madrid  
Av. de la Universidad, 30, 28911 Leganés, Madrid, Spain  

**Contact:**  
roisan@uc3m.pa.es, aigonzal@inf.uc3m.es, lgmanzan@inf.uc3m.es, jfuentes@inf.uc3m.es  

---

## Overview

This repository includes supplementary materials for the article:  
**"Service-aware password risk meter – Helping users to choose suitable passwords in services"**  
(submitted to ARES 2025)

Due to space constraints in the main manuscript, additional figures, tables, and materials are provided here to complement the study and support reproducibility.

---

## Approach Overview

The following figure provides a schematic summary of our proposed model. It illustrates how user, password, and service features are integrated to assess risk and generate feedback through the password meter interface.

![Approach overview](figures/approachoverview.png)

---

## Analyzed Password Leaks

The table below lists the datasets analyzed in our study, grouped by service category. Each entry includes the date of the breach (if known), the number of leaked passwords, and a summary of relevant password metrics. Services marked with an asterisk (*) indicate that the associated password policy was retrieved from 2024 documentation if no historical data was available.

<table>
  <thead>
    <tr>
      <th>Category</th><th>Service</th><th>Date</th><th># Passwords</th>
      <th>Mean Length</th><th>Min Length</th><th>Mask</th><th>Mean Score</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>Business</td><td>Kickstarter *</td><td>16/02/2014</td><td>1,456,977</td><td>8.11</td><td>6</td><td>l</td><td>1.38</td></tr>
    <tr><td></td><td>Cashcrate</td><td>17/11/2016</td><td>6,038,126</td><td>8.46</td><td>6</td><td>l</td><td>1.56</td></tr>
    <tr><td></td><td>Myheritage *</td><td>26/10/2017</td><td>81,618,257</td><td>7.01</td><td>9</td><td>l</td><td>1.14</td></tr>
    <tr><td></td><td>Booking *</td><td>01/12/2018</td><td>129,949</td><td>10.24</td><td>10</td><td>lud</td><td>2.48</td></tr>
    <tr><td></td><td>Clearvoicesurveys</td><td>01/10/2019</td><td>12,283,514</td><td>9.19</td><td>8</td><td>l</td><td>2.25</td></tr>
    <!-- Add more rows as needed -->
    <tr><td colspan="2"><strong>Total</strong></td><td>—</td><td>356,651,901</td><td>8.48</td><td></td><td></td><td></td></tr>
  </tbody>
</table>

<p><em>* Policy data taken from 2024 if earlier policy unavailable.</em></p>

---

## Use Cases

This section will include detailed tables describing specific use cases examined to evaluate the behavior of users and the effectiveness of the proposed meter under realistic service conditions.

<!-- Placeholder for use case tables -->
_Use case tables will be added here._

---

## Survey Questions

This section provides the full text of the user and expert surveys employed in the study. These questionnaires were used to evaluate the usability and perceived value of the password risk meter.

<!-- Placeholder for survey questions -->
_Survey content will be added here._

---

## Citation

If you use or reference this material, please cite the original paper as:

> Sánchez Serna, R., González-Tablas, A.I., González Manzano, L., de Fuentes, J.M.  
> *Service-aware password risk meter – Helping users to choose suitable passwords in services*.  
> Submitted to ARES 2025.

---

## License

Unless otherwise stated, all materials are made available for academic and non-commercial use under the [Creative Commons Attribution 4.0 International License (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).
