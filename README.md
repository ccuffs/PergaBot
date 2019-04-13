# PergaBot
PergaBot é um programa feito para a interação automática ou semi-automática com o pergamum por meio de CLI.

## Instalação: 
Para instalar o software, basta clonar o repositório
```sh
$ git clone https://github.com/northy/PergaBot.git
```
Baixar as dependências de bibliotecas
```sh
$ pip install -r requirements.txt
```
E baixar o driver desejado (links abaixo)

## Uso:
```sh
$ ./pergabot.py [opções] ... [-d driver | -m matrícula | -p senha] ...
```
### Opções e argumentos:
| Argumento | Função |
| ------ | ------ |
| -a  \| --auto | modo automático, renova todos os livros marcados como "Precisa de atenção" (padrão: falso) |
| -d  \| --driver _driver_ | Seleciona driver para ser usado no selenium, veja Drivers |
| -m  _matrícula_ | Argumento para prover a matrícula na inicialização |
| -p _senha_ | Argumento para prover a senha do pergamum na inicialização |
| -t _tempo_ | Tempo em dias para marcar livro como  "Precisa de atenção" (padrão: 2) |
| -s  \| --status | Somente mostra o seu acervo de livros emprestados. (padrão: falso) |
| -b  \| --binary  _localização_ | Localização do arquivo do driver (padrão: pasta de execução) |
| --version | Printa a versão do PergaBot |

## Bibliotecas utilizadas:
* [Requests]
* [PrettyTable]
* [Selenium]
* [BeautifulSoup4]
* [lxml]

## Drivers atualmente implementados:
* [ChromeDriver] (padrão)

Versão atual: **1.0**

[Requests]: <http://docs.python-requests.org/en/master/>
[PrettyTable]: <https://pypi.org/project/PrettyTable/>
[Selenium]: <https://selenium-python.readthedocs.io/>
[ChromeDriver]: <https://sites.google.com/a/chromium.org/chromedriver/>
[BeautifulSoup4]: <https://pypi.org/project/beautifulsoup4/>
[lxml]: <https://pypi.org/project/lxml/>
