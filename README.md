<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
<a name="readme-top"></a>
<!--
*** Thanks for checking out the Best-README-Template. If you have a suggestion
*** that would make this better, please fork the repo and create a pull request
*** or simply open an issue with the tag "enhancement".
*** Don't forget to give the project a star!
*** Thanks again! Now go create something AMAZING! :D
-->


[![LinkedIn][linkedin-shield]][linkedin-url]



<!-- PROJECT LOGO -->
<br />
<div align="center">
<h3 align="center">Modelo de Diagnóstico Prévio de Diabetes</h3>
</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Índice</summary>
  <ol>
    <li>
      <a href="#about-the-project">Sobre o projeto</a>
      <ul>
        <li><a href="#etl">Análise e Tratamento dos dados</a></li>
      </ul>
      <ul>
        <li><a href="#ml">Modelo de Machine Learning</a></li>
      </ul>
      <ul>
        <li><a href="#conclusion">Conclusão</a></li>
      </ul>
      <ul>
        <li><a href="#built-with">Tecnologia utilizada</a></li>
      </ul>
    </li>
    <li><a href="#contact">Contato</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## Sobre o projeto

Este projeto tem como objetivo a criação de um modelo de machine learning, que a partir de dados médicos de pacientes, possa auxiliar no diagnóstico prévio da doença diabetes.

Para este projeto o foco será no auxílio aos médicos com um diagnóstico prévio, não tirando a necessidade do acompanhamento médico.

Base de dados utilizada: [https://www.kaggle.com/datasets/lara311/diabetes-dataset-using-many-medical-metrics](https://www.kaggle.com/datasets/lara311/diabetes-dataset-using-many-medical-metrics)

Informações da base:

![image](https://github.com/user-attachments/assets/164ff010-5e7e-4628-8c4c-188a6b88bdc6)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- ABOUT THE PROJECT -->
### Análise e Tratamento dos dados

Nesta etapa, carreguei a base de dados retirada do kaggle, e iniciei a análise, em busca de verificar se haviam dados faltantes, dados com a tipagem incorreta, realizei a remoção de linhas com valores faltantes assim como o balanceamento da base de dados para equilibrar a variável respota "Outcome", o balanceamento foi feito utilizando a tecnica de over-sampling SMOTE.

Após as alterações feitas na base realizei a separação dos dados em treino e teste, para podermos treinar e testar adequadamente nosso modelo.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

### Modelo de Machine Learning

Após testar diversos tipos de modelos com parâmetros diferentes, o modelo final escolhido foi o de RandomForestClassifier

<p align="right">(<a href="#readme-top">back to top</a>)</p>

### Conclusão

O modelo final escolhido foi o RandomForestClassifier com os seguintes parâmetros:

- max_depth = 50
- criterion = 'gini'
- n_estimators = 200
- max_features = 'sqrt'
- 
A partir destes parâmetros foi possível chegar a uma acurácia de aproximadamente 78%.

Pelo fato do objetivo deste modelo ser um tipo de diagnostico prévio, acredito que a acurácia de 78% atenda as necessidades do projeto, o que não exclui a necessidade de acompanhamento médico para o diagnóstico final, apenas auxiliando na triagem para os médicos responsáveis.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

### Tecnologia utilizada 

* Python
  * Pandas (Extração e tratamento dos dados
  * Matplotlib (Visualização gráfica)
  * Seaborn (Visualização gráfica)
  * Scikit-learn (Criação do modelo de machine learning e métricas de avaliação)
  * imblearn (Técnicas de balanceamento da base de dados)
* Jupyter notebook

<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- CONTACT -->
## Contato

Leonardo Hideki Itihara - leohi1@hotmail.com - (11)95983-3437

Project Link: [https://github.com/leohideki/modelo_previsao_fraude](https://github.com/leohideki/modelo_previsao_fraude)

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/leonardo-itihara
