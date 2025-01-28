# Tabela Periódica de Funções e Bibliotecas Python Interativa Desktop
![Google Chrome](https://img.shields.io/badge/Google%20Chrome-4285F4?style=for-the-badge&logo=GoogleChrome&logoColor=white)
![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white)
![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
## Descrição

Este projeto é uma representação visual da tabela periódica, mas, em vez de elementos químicos, ela apresenta funções e bibliotecas do Python. Cada "elemento" na tabela corresponde a uma função ou biblioteca, e dentro de cada um, o usuário encontra botões para acessar subdivisões detalhadas dessas funções. Algumas dessas subdivisões incluem um terminal interativo, onde o usuário pode modificar e executar código Python diretamente, além de exemplos prontos para facilitar o aprendizado. O objetivo é proporcionar uma maneira interativa e dinâmica de explorar o vasto ecossistema do Python e testar código em tempo real.

## Com o que foi construido?
Este sistema é desenvolvido utilizando HTML, CSS e JavaScript. Os arquivos HTML são responsáveis por definir o layout da tabela periódica e seus elementos, enquanto o CSS cuida do design e estilo visual. Já o JavaScript implementa a lógica e a tradução do código. Para permitir a execução de Python diretamente no navegador, utilizei o Pyodide, uma solução open source baseada em WebAssembly que possibilita rodar código Python no ambiente web.

## Como o HTML é executado na área de trabalho?
Utilizei um programa chamado Lively Wallpaper, que permite carregar e exibir arquivos HTML diretamente na área de trabalho, transformando o ambiente em uma experiência interativa.


## Instrução de instalação

### Pré requisitos

Google Chrome<br>
Lively Wallpaper

### Etapas
1- Download e Install Lively Wallpaper<br>
https://www.rocksdanister.com/lively/<br>
2- Configurar Lively Walppaper
#### Abra as configurações do Lively wallpaper
![tutorial_lively_1](https://github.com/user-attachments/assets/79c378e1-3df7-4769-996b-e6a346804f7f)
### Marque as opçoes conforme a imagem
![tutorial_lively_2](https://github.com/user-attachments/assets/6cad62ef-614c-46d8-87be-9cfc3908e9b2)
![tutorial_lively_3](https://github.com/user-attachments/assets/7a78d1d6-260b-456b-a261-8b11542c4a63)
##
3- Após as configurações clique no sinal de + para adicionar o arquivo
##
![tutorial_lively_4](https://github.com/user-attachments/assets/5fb15f86-11b5-4701-8f3b-12bd60153a5d)
##
4 - Selecione ou arraste o arquivo index.html para o Lively wallpaper
##
![tutorial_lively_5](https://github.com/user-attachments/assets/3740c0be-8dee-48a4-bce1-892df381de7b)
##
5- Clique em ok e espere o carregamento do arquivo, após isso pode fechar o lively wallpaper
## Instruções de uso
1- Certifique-se de que nenhum arquivo esteja aberto no fundo da área de trabalho. Isso é especialmente importante se você estiver utilizando mais de uma tela. Caso algum programa esteja aberto, como mostrado na barra de tarefas, ao clicar com o mouse, a ação pode não ser executada corretamente. Verifique a barra de tarefas para garantir que nenhum aplicativo esteja interferindo.
![tutorial_lively_6](https://github.com/user-attachments/assets/5412ad5e-cfa8-4093-9cb0-97f7e3a3821a)
2- Clique e selecione os elementos que deseja acessar.
3- Para sair de um elemento aberto, basta clicar fora dele
4- Se o elemento não fechar, clique dentro do quadrado e, em seguida, fora dele.
5- O terminal Python já está configurado com as bibliotecas numpy, pandas e pytz. Não há necessidade de adicionar outras bibliotecas, pois não são necessárias para o funcionamento deste projeto.
## Abrir o arquivo index.html direto no navegador
O Pyodide é uma implementação do Python para rodar no navegador, baseada em WebAssembly. No entanto, ao tentar abrir um arquivo com Pyodide diretamente no navegador, ele pode não funcionar corretamente por alguns motivos comuns:

Possíveis Problemas
Restrições de CORS (Cross-Origin Resource Sharing): Arquivos locais carregados diretamente no navegador (usando o protocolo file://) podem enfrentar problemas de permissões devido às políticas de segurança do navegador. Isso pode impedir que o Pyodide carregue arquivos necessários, como o WebAssembly e os pacotes Python, de maneira adequada.
### Maneiras de contornar a situação

1- Crie um atalho para o arquivo index.html e use uma flag no destino do atalho.
No campo de destino do atalho, adicione o seguinte código:

"C:\Program Files\Google\Chrome\Application\chrome.exe" --allow-file-access-from-files "C:\python\index.html"

Primeiro item: O local onde o Google Chrome está instalado.
Segundo item: A flag --allow-file-access-from-files habilita o Pyodide para rodar sem restrições.
Terceiro item: O local do arquivo index.html que você deseja abrir.

![tutorial_lively_7](https://github.com/user-attachments/assets/c973b773-a8eb-40c0-af5b-30c254e8f0fe)

Dessa forma, o Pyodide funcionará corretamente no navegador sem bloqueios.



