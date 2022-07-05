# Introdução ao Git  :computer::computer_mouse:



- ## Git

  1- Controle de versão.

  2- Armazenamento em nuvem.

  3- Trabalho em equipe.

  4- Melhora do código.

  5- Reconhecimento.



- ## Navegação via command line interface :desktop_computer:

  ### Windows

  dir + enter => para listar as pastas do diretório

  cd => base do diretório

  cls (clear screen) => limpar a tela

  tecla tab => função de autocompletar

  mkdir => criar pasta 

  echo => direciona o fluxo

  del => deletar (apaga o que tem dentro da pasta)

  rmdir => apaga o diretório em questão

  

  

- ## Entendendo como o Git funciona :gear:

  ### Tópicos fundamentais para entender o funcionamento do Git

  - #### Sha1 

    Significa Secure Hash Algortitm (Algoritmo de Hash Seguro), é um conjunto de funções de hash criptográficas projetadas pela NSA (Agência de Segurança Nacional dos EUA). A encriptação gera conjunto de caracteres identificados de 40 dígitos. É uma forma curta de representar um arquivo.

    Comando para gerar o código:

    $ openssl sha1 nome do arquivo 

    

  - ### Objetos internos do Git

    - BLOBS - armazena o sha, metadados, tipo, tamanho, conteúdo do arquivo
    - TREE - armazena o BLOBS, o nome do arquivo e outras árvores
    - COMMITS - armazena, árvores, commit, autor, mensagem

  ** Metadados - são dados sobre outros dados. Facilitam o entendimento dos relacionamentos e a utilidade das informações dos dados.

  *** Modificações em um arquivo, mudam o sha, o BLOBS, muda a árvore e o COMMIT. Se for modificado, ou não, fica evidente.

  

- ## Git sistema distribuído seguro :lock:

  - ### Chave SSH

    A forma de estabelecer uma conexão segura e criptada entre duas máquinas. Para isso é necessário configurar nossa máquina como confiável pelo GitHub. Serão geradas 2 chaves, uma pública, que será adicionada ao GitHub, e  outra privada.

    

  -  ### Token de acesso pessoal

    Gera no GitHub, guarda na máquina, sempre irá pedir a identificação do usuário e da senha do token de acesso pessoal.



## *Commmit 

É o ato de enviar ou guardar, ou seja, enviar dados ou códigos para armazenamento em banco de dados ou em um sistema de controle de versão.





- ## Primeiros comandos com o Git :key:

  - ### Iniciando o Git e criando um commit

    - Iniciar Git 

    - Iniciar o versamento

    - Criar um commit

      **git init => git add *=> git commit -m "_pequena descrição_"**

      

- ## Ciclo de vida dos arquivos :cyclone:

  - **Untracked**: sabe que o arquivo existe, porém não controla seu ciclo de vida.
  - **Tracked**: esta dividido em 3 possibilidades:
    - *unmodified*: arquivos não alterados.
    - *modified*: arquivos com modificações.
    - *staged*: os arquivos em sua versão final, estarão no próximo *commit*.

  O arquivo pode estar nosso ambiente de desenvolvimento (nossa máquina) ou remoto (GitHub).

  O **_ambiente de desenvolvimento_**  compreende 3 repartições:

  - **Working directory** - onde poderão estar localizados os arquivos untracked e tracked unmodified.

  - **Staging area** - onde poderão estar arquivos tracked unmodified, modified e staged.

  - **Local repository** - onde podemos encontrar arquivos comitados, que poderão ser enviados para o **_Remote Repositotory_**, localizado no servidor.

    O **_Remote Repositotory_**  irá receber o arquivo comitado e poderá fornecer arquivos para modificações em nossa máquina.

  

  ## Comandos: :unlock:

  git init => cria um repositório

  git add * => adiciona tudo do "Working Directory " para a "Staging Area" 

  git commit -m  "breve descrição" => transforma arquivos do Staged para Commit, armazenado no Local Repository .

  

  

  # 

  

  

  

  







