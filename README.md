# Projeto-DataScience-Airbnb

## Descrição:

O projeto consiste na criação de um modelo que seja rápido e que possibilite que uma pessoa comum possa ter uma previsão dada por um Inteligência artificial que lhe dirá quanto deve cobrar pela diária do seu imóvel ou de outra pessoa, desde que este esteja localizado no Rio de Janeiro

Para isso são coletados dados dos imóveis cadastrados no Airbnb do Rio de Janeiro, com os dados é feito uma análise, verificação e correção que corresponde ao objetivo final do projeto.

Depois da análise e correção é feita uma transformação dos dados em 0 e 1 para possibilitar um treinamento eficiente por parte da Inteligência artificial que depois de treinada com 80% dos dados, ela é testada com os outros 20% dos dados para ter certeza de sua eficacia, após isso é escolhida a Inteligência que possui melhor resultado.

Por fim o modelo é salvo em um formato joblib que é lido no arquivo de deploy que configura o servidor de utilização do modelo para que qualquer pessoa possa usar.

No futuro irei criar uma maneira mais amigável de uma pessoa comum ter acesso a esse modelo como acessando um site por exemplo, mas o modo que fiz é 100% funcional podendo demorar um pouco dependendo da sua máquina.

## Passo a Passo de Utilização:

Primeiramente será necessário que você tenha em seu computador o Python instalado e também o Anaconda, segue o link para download dessas tecnologias:

https://www.anaconda.com/products/distribution

https://www.python.org/downloads/

Depois de instalar as tecnologias será necessário instalar as bibliotecas que serão utilizadas no modelo do projeto, para isso você deverá abrir o seu terminal ou cmd e digitar os seguintes códigos:

`pip install pandas`
`pip install numpy`
`pip install seaborn`
`pip install matplotlib`
`pip install plotly`
`pip install sklearn`
`pip install joblib`
`pip install streamlit`

Após isso você deve baixar um clone deste repositório para que possa ter acesso ao programa e a base de dados

Em seguida você deve abrir o jupyter-notebook, digitando na barra de pesquisa do Windows e clicando no programa ou digitando `jupyter-notebook`no terminal caso você esteja usando Linux

Acessando jupyter dentro a interface que ele criar ao abrir, você irá procurar a pasta onde o clone do repositório foi baixado e abrir o arquivo onde se encontra o modelo, arquivo este que possui o nome "Solução Airbnb Rio.ipynb"

Após abrir o arquivo será necessário que você mude apenas os diretórios onde serão coletadas as bases de dados, pois no seu computador o caminho do diretório onde se encontrará o arquivo da base dados será diferente

Agora é apenas necessário executar todas as celulas onde estão os códigos, você pode fazer isso clicando em cell no canto superior e selecionando RUN ALL (isso poderá demorar alguns minutos depedendo da sua máquina)

Depois disso você deve acessar a aba do navegador onde está a interface do jupyter e abrir o arquivo com nome "DeploProjetoAirbnb.ipynb" , lá você  também deve mudar apenas o caminho do diretório da variável chamada modelo, passando o caminho do arquivo "Modelo.joblib" que foi gerado rodando os códigos passados

Após isso você irá salvar e programa clicando no botão com simbolo de cartão de memória no canto superior esquerdo, depois de salvo você clicará na opção FILE também localizada no canto superior esquerdo e selecionará "download as" e clicará em "Python(py)", assim o programa será baixado no seu computador

Depois de baixado, você ira abrir o seu terminal ou cmd e digitar os seguintes códigos:

`cd Downloads`
`streamlit run DeploProjetoAirbnb.py`

Com isso o servidor será aberto e você terá acesso a uma aba no navegador em que você poderá preencher as informações do imóvel, clicando no botão de previsão após preencher todas as informações e esperando alguns minutos você terá acesso a previsão do preço da diária ddo imóvel feita pela inteligência artificial que já foi treinada.
