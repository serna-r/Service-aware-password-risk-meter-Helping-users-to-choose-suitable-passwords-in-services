# Supplementary Materials for paper "Service-aware password risk meter – Helping users to choose suitable passwords in services" 
**(accepted at ARES 2025)**

**Authors:**  
Roi Sánchez Serna [[ORCID: 0009-0001-6424-8262]](https://orcid.org/0009-0001-6424-8262)  
Ana I. González-Tablas [[ORCID: 0000-0002-6259-8955]](https://orcid.org/0000-0002-6259-8955)  
Lorena González Manzano [[ORCID: 0000-0002-3490-621X]](https://orcid.org/0000-0002-3490-621X)  
Jose María de Fuentes [[0000-0002-4023-3197]](https://orcid.org/0000-0002-4023-3197)

**Affiliation:**  
Universidad Carlos III de Madrid<br>
Computer Science and Engineering Dpt.<br>
Av. de la Universidad, 30, 28911 Leganés, Madrid, Spain<br>

**This work was funded by INCIBE (Instituto Nacional de Ciberseguridad de España).**
![Project logos](figures/BandaLogos_INCIBE_es.png)

**Contact:**  
roisanch@pa.uc3m.es, aigonzal@inf.uc3m.es, lgmanzan@inf.uc3m.es, jfuentes@inf.uc3m.es  

---

## Overview

This repository includes supplementary materials for the article:  
**"Service-aware password risk meter – Helping users to choose suitable passwords in services"**  
(accepted at ARES 2025)

This work was conducted with the support of the Spanish National Cybersecurity Institute (INCIBE).  
Due to space constraints in the main manuscript, additional figures, tables, and materials are provided here to complement the study and support reproducibility.

The extended version of the article can be found at: <br>
https://hdl.handle.net/10016/47287 <br>

The tool developed for this study can be accessed at:  
Tool: [https://serna-r.github.io/risk-meter---V2/](https://serna-r.github.io/risk-meter---V2/)<br>
Source: [https://github.com/serna-r/risk-meter---V2/tree/only-javascript](https://github.com/serna-r/risk-meter---V2/tree/only-javascript)

---

## Repository Structure

- `figures/` – Contains the images displayed in this README.  
- `surveys/` – Contains survey results:  
  - `Rd_matrix.xlsx` – The \( R_d \) matrix used in risk calculations.  
  - `expert validation/` – Results from expert validation:  
    - `expert_validation_english.xlsx` – Expert validation in English.  
    - `expert_validation_spanish.xlsx` – Expert validation in Spanish.  
  - `user validation/` – Results from user validation:  
    - `user_validation.xlsx` – User validation results.  

---
## Approach Overview

The following figure provides a schematic summary of our proposed model. It illustrates how user, password, and service features are integrated to assess risk and generate feedback through the password meter interface.

![Approach overview](figures/approachoverview.png)

---

## Analyzed Password Leaks

The table below lists the datasets analyzed in our study, grouped by service category. Each entry includes the date of the breach (if known), the number of leaked passwords, and a summary of relevant password metrics. Services marked with an asterisk (*) indicate that the associated password policy was retrieved from 2024 documentation if no historical data was available.

<table>
    <tr>
        <td><strong>Category</strong></td>
        <td><strong>Service</strong></td>
        <td><strong>Date</strong></td>
        <td><strong># Passwords</strong></td>
        <td><strong>Mean Length</strong></td>
        <td><strong>Min Length</strong></td>
        <td><strong>Mask</strong></td>
        <td><strong>Mean Score</strong></td>
    </tr>
    <tr>
        <td>Business</td>
        <td>Kickstarter *</td>
        <td>16/02/2014</td>
        <td>1,456,977</td>
        <td>8.11</td>
        <td>6</td>
        <td>l</td>
        <td>1.38</td>
    </tr>
    <tr>
        <td></td>
        <td>Cashcrate</td>
        <td>17/11/2016</td>
        <td>6,038,126</td>
        <td>8.46</td>
        <td>6</td>
        <td>l</td>
        <td>1.56</td>
    </tr>
    <tr>
        <td></td>
        <td>Myheritage *</td>
        <td>26/10/2017</td>
        <td>81,618,257</td>
        <td>7.01</td>
        <td>9</td>
        <td>l</td>
        <td>1.14</td>
    </tr>
    <tr>
        <td></td>
        <td>Booking *</td>
        <td>01/12/2018</td>
        <td>129,949</td>
        <td>10.24</td>
        <td>10</td>
        <td>lud</td>
        <td>2.48</td>
    </tr>
    <tr>
        <td></td>
        <td>Clearvoicesurveys</td>
        <td>01/10/2019</td>
        <td>12,283,514</td>
        <td>9.19</td>
        <td>8</td>
        <td>l</td>
        <td>2.25</td>
    </tr>
    <tr>
        <td></td>
        <td>Gigasize</td>
        <td>Unknown</td>
        <td>1,896,399</td>
        <td>7.84</td>
        <td>-</td>
        <td>-</td>
        <td>1.44</td>
    </tr>
    <tr>
        <td></td>
        <td>Hq</td>
        <td>Unknown</td>
        <td>3,025,218</td>
        <td>9.53</td>
        <td>-</td>
        <td>-</td>
        <td>2.17</td>
    </tr>
    <tr>
        <td>Digitaltool</td>
        <td>Dropbox *</td>
        <td>01/07/2012</td>
        <td>50,000</td>
        <td>9.14</td>
        <td>8</td>
        <td>luds</td>
        <td>1.88</td>
    </tr>
    <tr>
        <td></td>
        <td>Psiho</td>
        <td>01/03/2018</td>
        <td>883,693</td>
        <td>7.87</td>
        <td>-</td>
        <td>-</td>
        <td>1.30</td>
    </tr>
    <tr>
        <td></td>
        <td>Chegg *</td>
        <td>28/04/2018</td>
        <td>29,309,993</td>
        <td>9.09</td>
        <td>6</td>
        <td>lud</td>
        <td>1.92</td>
    </tr>
    <tr>
        <td></td>
        <td>Sharethis *</td>
        <td>09/07/2018</td>
        <td>2,268,955</td>
        <td>7.90</td>
        <td>8</td>
        <td>luds</td>
        <td>1.50</td>
    </tr>
    <tr>
        <td></td>
        <td>Canva *</td>
        <td>24/05/2019</td>
        <td>4,779,956</td>
        <td>9.19</td>
        <td>8</td>
        <td>l</td>
        <td>1.95</td>
    </tr>
    <tr>
        <td></td>
        <td>Mixfiend *</td>
        <td>Unknown</td>
        <td>193,984</td>
        <td>7.23</td>
        <td>6</td>
        <td>l</td>
        <td>1.20</td>
    </tr>
    <tr>
        <td>Games</td>
        <td>Evony</td>
        <td>01/06/2016</td>
        <td>34,147,326</td>
        <td>7.98</td>
        <td>-</td>
        <td>-</td>
        <td>1.38</td>
    </tr>
    <tr>
        <td></td>
        <td>Zynga *</td>
        <td>01/09/2019</td>
        <td>50,000</td>
        <td>9.12</td>
        <td>7</td>
        <td>l</td>
        <td>1.60</td>
    </tr>
    <tr>
        <td></td>
        <td>Gogames *</td>
        <td>Unknown</td>
        <td>1,207,367</td>
        <td>8.51</td>
        <td>8</td>
        <td>l</td>
        <td>1.41</td>
    </tr>
    <tr>
        <td></td>
        <td>Lekoolgames</td>
        <td>Unknown</td>
        <td>3,175,293</td>
        <td>8.49</td>
        <td>-</td>
        <td>-</td>
        <td>1.59</td>
    </tr>
    <tr>
        <td>Shopping</td>
        <td>Shein *</td>
        <td>01/06/2018</td>
        <td>28,951,772</td>
        <td>8.46</td>
        <td>8</td>
        <td>l</td>
        <td>1.68</td>
    </tr>
    <tr>
        <td></td>
        <td>Hautelook *</td>
        <td>07/08/2018</td>
        <td>13,047,077</td>
        <td>8.20</td>
        <td>8</td>
        <td>lud</td>
        <td>1.43</td>
    </tr>
    <tr>
        <td>Social</td>
        <td>Myspace</td>
        <td>01/07/2008</td>
        <td>50,000</td>
        <td>10.13</td>
        <td>6</td>
        <td>luds</td>
        <td>2.05</td>
    </tr>
    <tr>
        <td></td>
        <td>Linkedin</td>
        <td>05/05/2012</td>
        <td>67,241,910</td>
        <td>7.73</td>
        <td>6</td>
        <td>l</td>
        <td>1.28</td>
    </tr>
    <tr>
        <td></td>
        <td>Mate1</td>
        <td>29/02/2016</td>
        <td>27,401,746</td>
        <td>7.98</td>
        <td>6</td>
        <td>l</td>
        <td>1.35</td>
    </tr>
    <tr>
        <td></td>
        <td>Edmodo</td>
        <td>01/05/2017</td>
        <td>14,884,412</td>
        <td>8.81</td>
        <td>-</td>
        <td>-</td>
        <td>1.76</td>
    </tr>
    <tr>
        <td></td>
        <td>Dubshmash</td>
        <td>01/12/2018</td>
        <td>22,077,067</td>
        <td>7.55</td>
        <td>5</td>
        <td>l</td>
        <td>0.92</td>
    </tr>
    <tr>
        <td></td>
        <td>Htcmania</td>
        <td>04/01/2020</td>
        <td>482,910</td>
        <td>8.25</td>
        <td>1</td>
        <td>l</td>
        <td>1.61</td>
    </tr>
    <tr>
        <td></td>
        <td></td>
        <td><strong>Total</strong></td>
        <td>356,651,901</td>
        <td>8.48</td>
        <td></td>
        <td></td>
    </tr>
</table>

<p><em>* Policy data taken from 2024 if earlier policy unavailable.</em></p>

---

## Use Cases

The following table summarizes three case studies used to illustrate how our proposed risk model behaves under different service and password conditions. Each row reflects the evaluated parameters: data exposure, service authentication strength, password strength and usage, and the resulting risk score. Bold values indicate parameters varied intentionally to observe their impact on the risk score.

<table>
  <thead>
    <tr>
      <th>Case Study</th>
      <th><i>D<sub>EXP</sub>(s<sub>i</sub>)</i><br># collected data</th>
      <th colspan="3"><i>S<sub>AUTH</sub>(s<sub>i</sub>)</i></th>
      <th colspan="2"><i>U<sub>AUTH</sub>(pwd<sub>j</sub>)</i></th>
      <th><i>R(s<sub>i</sub>, pwd<sub>j</sub>)</i></th>
    </tr>
    <tr>
      <th></th>
      <th></th>
      <th><i>P</i></th>
      <th><i>M<sub>r</sub></i></th>
      <th><i>f<sub>a</sub></i></th>
      <th><i>P<sub>STR</sub>(pwd<sub>j</sub>)</i></th>
      <th><i>P<sub>USE</sub>(pwd<sub>j</sub>)</i></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>1</td><td><b>17</b></td><td>0</td><td>0</td><td>1</td><td>2</td><td>0 (n=1)</td><td>37.78</td>
    </tr>
    <tr>
      <td></td><td><b>8</b></td><td>0</td><td>0</td><td>1</td><td>2</td><td>0 (n=1)</td><td>14.52</td>
    </tr>
    <tr>
      <td></td><td><b>1</b></td><td>0</td><td>0</td><td>1</td><td>2</td><td>0 (n=1)</td><td>3.14</td>
    </tr>
    <tr>
      <td>2</td><td>17</td><td><b>3</b></td><td><b>1</b></td><td><b>0</b></td><td>2</td><td>0 (n=1)</td><td>77.78</td>
    </tr>
    <tr>
      <td></td><td>17</td><td><b>0</b></td><td><b>1</b></td><td><b>0</b></td><td>2</td><td>0 (n=1)</td><td>47.78</td>
    </tr>
    <tr>
      <td></td><td>17</td><td><b>0</b></td><td><b>0</b></td><td><b>1</b></td><td>2</td><td>0 (n=1)</td><td>37.78</td>
    </tr>
    <tr>
      <td>3</td><td>17</td><td>0</td><td>0</td><td>1</td><td><b>1</b></td><td><b>0.5 (n=10)</b></td><td>51.11</td>
    </tr>
    <tr>
      <td></td><td>17</td><td>0</td><td>0</td><td>1</td><td><b>2</b></td><td><b>0.2 (n=3)</b></td><td>39.56</td>
    </tr>
    <tr>
      <td></td><td>17</td><td>0</td><td>0</td><td>1</td><td><b>4</b></td><td><b>0 (n=1)</b></td><td>24.44</td>
    </tr>
  </tbody>
</table>


---

## Survey Questions

The following items were used to evaluate the usability, clarity, and potential impact of the proposed password risk meter. The survey aimed to determine whether the tool helps users understand cybersecurity risks, influences their behavior, and is suitable for integration into real-world authentication processes.

<ol>
  <li><strong>Q1:</strong> <em>Does the risk meter help you understand the risk of a cybercriminal accessing your stored data?</em><br>
  This question assesses whether the tool effectively conveys security risks.</li>

  <li><strong>Q2:</strong> <em>Do the risk indicators assist you in making informed choices regarding password selection and service usage?</em><br>
  This item examines whether users find the tool practical for decision-making.</li>

  <li><strong>Q3:</strong> <em>Would you like online services to incorporate this risk meter in the registration process?</em><br>
  This question evaluates user interest in having such a tool integrated into mainstream authentication systems.</li>

  <li><strong>Q4:</strong> <em>If the overall risk level were high but could be lowered by selecting a stronger, unique password, would you do so?</em><br>
  This item measures whether users would modify their behavior based on the risk metric’s feedback.</li>

  <li><strong>Q5:</strong> <em>If the overall risk level were high and could not be reduced by changing the password, would you seek alternative services?</em><br>
  This final question determines whether users would consider switching services to protect their data under high-risk scenarios.</li>
</ol>

---

## Citation

If you use or reference this material, please cite the original paper as:

> Sánchez Serna, R., González-Tablas, A.I., González Manzano, L., de Fuentes, J.M.  
> *Service-aware password risk meter – Helping users to choose suitable passwords in services*.  
> Submitted to ARES 2025.

---

## License

Unless otherwise stated, all materials are made available for academic and non-commercial use under the [Creative Commons Attribution 4.0 International License (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).
