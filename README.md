# Análise dos dados dos discentes e cursos da UFRN
Iremos analisar os dados dos discentes e cursos da Universidade Federal do Rio Grande do Norte - UFRN, a fim de entendermos melhor os perfis de pessoas que entram nessa universidade.

Trabalho realizado por:
- <a href="https://github.com/alvarofpp">Álvaro Ferreira Pires de Paiva</a>
  - Matrícula: 2016039162
  - E-mail: alvarofepipa@gmail.com
- <a href="https://github.com/Iolch">Iolanda Chagas Costa Paiva</a>
  - Matrícula: 2016036509
  - E-mail: iccpaiva@gmail.com  

# Sumário
- [Base de Dados](#base-dados)
- [Código](#codigo)
  - [Dependências](#dependencias)
  - [Preparando os dados](#preparando-dados)
  - [Analises](#analises)
    - Classes sociais por período de matrícula
    - Análise das bolsas/auxílios
    - Alunos que recebem bolsa/auxílios no decorrer dos anos
    - Ingressos por áreas de conhecimento
    - Cursos por área de conhecimento

# <a id="base-dados">Base de Dados</a>
Os dados utilizados formam retirados do site de [dados abertos da UFRN](http://dados.ufrn.br/). Foram utilizados os seguintes conjuntos de dados:

- [Cursos de Graduação](http://dados.ufrn.br/dataset/cursos-de-graduacao)
- [Dados Sócio-Econômicos de Discentes](http://dados.ufrn.br/dataset/dados-socio-economicos-de-discentes)
- [Dados Complementares de Discentes](http://dados.ufrn.br/dataset/dados-complementares-de-discentes)
- [Discentes](http://dados.ufrn.br/dataset/discentes)

# <a id="codigo">Código</a>
Agora iremos para a parte em que tentaremos encontrar as respostas das perguntas orientadoras de cada tópico.

## <a id="dependencias">Dependências</a>
Nessa seção, iremos declarar as dependências necessárias para o Jupyter Notebook executar corretamente, para isso iremos: declarar as variáveis globais que iremos utilizar, importar as libs necessárias e preparar os arquivos que temos para podermos utilizá-los nas seções seguintes.

- [os](https://docs.python.org/3/library/os.html)
- [re](https://docs.python.org/3/library/re.html)
- [Numpy](http://www.numpy.org/) as **np**
- [Pandas](https://pandas.pydata.org/) as **pd**
- [Matplotlib](https://matplotlib.org/) as **plt**

Comandos de terminal para instalar as dependências que não vem por padrão:
```sh
conda install -c conda-forge numpy
conda install -c conda-forge matplotlib
conda install -c conda-forge pandas
```