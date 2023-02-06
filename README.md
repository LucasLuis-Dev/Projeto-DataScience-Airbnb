# 💻 Projeto-DataScience-Airbnb

<img src="https://cdn.discordapp.com/attachments/965066624556232737/985353975043862568/Captura_de_tela_de_2022-06-11_22-23-54.png" >

## 📄 Descrição:

O projeto consiste na criação de um modelo que seja rápido e que possibilite que uma pessoa comum possa ter uma previsão dada por um Inteligência artificial que lhe dirá quanto deve cobrar pela diária do seu imóvel ou de outra pessoa, desde que este esteja localizado no Rio de Janeiro

Para isso são coletados dados dos imóveis cadastrados no Airbnb do Rio de Janeiro, com os dados é feito uma análise, verificação e correção que corresponde ao objetivo final do projeto.

Depois da análise e correção é feita uma transformação dos dados em 0 e 1 para possibilitar um treinamento eficiente por parte da Inteligência artificial que depois de treinada com 80% dos dados, ela é testada com os outros 20% dos dados para ter certeza de sua eficacia, após isso é escolhida a Inteligência que possui melhor resultado.

Por fim o modelo é salvo em um formato joblib que é lido no arquivo de deploy que configura o servidor de utilização do modelo para que qualquer pessoa possa usar.

### 🎯 Tecnologias

- Python
- Pandas
- Sklearn
- Numpy
- Seaborn
- Matplotlib
- Plotly
- Joblib
- Streamlit



## 👣 Passo a Passo de Utilização:


1 - Primeiramente será necessário que você tenha em seu computador o Python instalado e também o Anaconda, segue o link para download dessas tecnologias:

https://www.anaconda.com/products/distribution

https://www.python.org/downloads/

2 - Depois de instalar as tecnologias será necessário instalar as bibliotecas que serão utilizadas no modelo do projeto, para isso você deverá abrir o seu terminal ou cmd e digitar os seguintes códigos:

`pip install pandas`
`pip install numpy`
`pip install seaborn`
`pip install matplotlib`
`pip install plotly`
`pip install sklearn`
`pip install joblib`
`pip install streamlit`

3 - Após isso você deve baixar um clone deste repositório para que possa ter acesso ao programa e a base de dados

4 - Em seguida você deve abrir o jupyter-notebook, digitando na barra de pesquisa do Windows e clicando no programa ou digitando `jupyter-notebook`no terminal caso você esteja usando Linux

6 - Acessando jupyter dentro a interface que ele criar ao abrir, você irá procurar a pasta onde o clone do repositório foi baixado e abrir o arquivo onde se encontra o modelo, arquivo este que possui o nome "Solução Airbnb Rio.ipynb"

7 - Após abrir o arquivo será necessário que você mude apenas os diretórios onde serão coletadas as bases de dados, pois no seu computador o caminho do diretório onde se encontrará o arquivo da base dados será diferente

8 - Agora é apenas necessário executar todas as celulas onde estão os códigos, você pode fazer isso clicando em cell no canto superior e selecionando RUN ALL (isso poderá demorar alguns minutos depedendo da sua máquina), como resultado final ele gerará um arquivo em seu computador que possui em torno de 5gb

<img src="https://cdn.discordapp.com/attachments/965066624556232737/985357769244823592/Captura_de_tela_de_2022-06-11_22-37-35.png" >

9 - Depois disso você deve acessar a aba do navegador onde está a interface do jupyter e abrir o arquivo com nome "DeploProjetoAirbnb.ipynb" , lá você  também deve mudar apenas o caminho do diretório da variável chamada modelo, passando o caminho do arquivo "Modelo.joblib" que foi gerado rodando os códigos passados

<img src="https://cdn.discordapp.com/attachments/965066624556232737/985358250780262420/Captura_de_tela_de_2022-06-11_22-41-37.png" >

10 - Após isso você irá salvar e programa clicando no botão com simbolo de cartão de memória no canto superior esquerdo, depois de salvo você clicará na opção FILE também localizada no canto superior esquerdo e selecionará "download as" e clicará em "Python(py)", assim o programa será baixado no seu computador

<img src="https://cdn.discordapp.com/attachments/965066624556232737/985358682713899058/Captura_de_tela_de_2022-06-11_22-43-16.png" >

11 - Depois de baixado, você ira abrir o seu terminal ou cmd e digitar os seguintes códigos:

`cd Downloads`

<img src="https://cdn.discordapp.com/attachments/965066624556232737/985359415928557619/Captura_de_tela_de_2022-06-11_22-45-04.png" >

`streamlit run DeploProjetoAirbnb.py`

<img src="https://cdn.discordapp.com/attachments/965066624556232737/985359668408905728/Captura_de_tela_de_2022-06-11_22-45-19.png" >

12 - Com isso o servidor será aberto e você terá acesso a uma aba no navegador em que você poderá preencher as informações do imóvel, clicando no botão de previsão após preencher todas as informações e esperando alguns minutos você terá acesso a previsão do preço da diária do imóvel feita pela inteligência artificial que já foi treinada.

<img src="https://cdn.discordapp.com/attachments/965066624556232737/985360016922005575/Captura_de_tela_de_2022-06-11_22-48-35.png" >
