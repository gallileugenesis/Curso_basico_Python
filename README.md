{
 "cells": [
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "eukgjPyPG6CF"
   },
   "source": [
    "# Curso básico de Python\n",
    "Prof. Gallileu Genesis"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "4InykwzeG6CG"
   },
   "source": [
    "### Tópicos:\n",
    "\n",
    "#### 1 - Introdução ao Python:\n",
    "- O que é Python\n",
    "- Aplicações\n",
    "- Ferramentas de desenvolvimento\n",
    "- Instalação do Python e ambiente de desenvolvimento\n",
    "- Executando o primeiro programa em Python\n",
    "\n",
    "#### 2 - Tipos de dados e variáveis:\n",
    "- Tipos de dados em Python (números, strings, booleanos)\n",
    "- Declaração de variáveis\n",
    "- Operações com variáveis\n",
    "- Exercícios\n",
    "\n",
    "#### 3 - Estruturas de controle de fluxo:\n",
    "- Estruturas Condicionais (if/else)\n",
    "- Estruturas de Repetição (for, while)\n",
    "- Instruções de controle de fluxo (break, continue)\n",
    "- Exercícios\n",
    "\n",
    "#### 4 - Estruturas de dados:\n",
    "- Listas\n",
    "- Acesso e manipulação de elementos em Listas\n",
    "- Tuplas\n",
    "- Acesso e manipulação de elementos em Tuplas\n",
    "- Dicionários\n",
    "- Acesso e manipulação de elementos em dicionários\n",
    "- Exercícios"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "qBMndxdtG6CG"
   },
   "source": [
    "## 1 - Introdução ao Python"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "_NZQN-QJG6CH"
   },
   "source": [
    "### 1.1 - O que é Python:\n",
    "\n",
    "Python é uma linguagem de programação de alto nível, interpretada, orientada a objetos e multiplataforma.\n",
    "\n",
    "- **Linguagem de Programação de Alto Nível:** Significa que a linguagem foi projetada com um alto nível de abstração, tornando-a mais próxima da linguagem humana e permitindo que os desenvolvedores expressem suas ideias de maneira mais clara e concisa. Linguagens de alto nível geralmente têm uma sintaxe mais amigável e oferecem construções de alto nível para lidar com tarefas complexas.\n",
    "\n",
    "- **Interpretada**: Uma linguagem interpretada é aquela em que o código-fonte é executado diretamente por um interpretador, que é um programa que lê o código linha por linha e o executa em tempo real. Isso é diferente de uma linguagem compilada, onde o código-fonte é transformado em código de máquina (ou bytecode) antes da execução.\n",
    "\n",
    "- **Orientada a Objetos**: Refere-se a um paradigma de programação onde o código é organizado em objetos, que são entidades que encapsulam dados e comportamentos relacionados. A programação orientada a objetos (POO) permite que os desenvolvedores criem abstrações mais significativas, facilitando a reutilização de código e a manutenção do software.\n",
    "\n",
    "- **Multiplataforma**: Significa que a linguagem pode ser executada em diferentes plataformas de hardware ou sistemas operacionais sem a necessidade de grandes modificações. Isso é alcançado através do uso de ambientes de execução (como máquinas virtuais ou interpretadores) que permitem que o código seja executado em ambientes diferentes, desde que o ambiente de execução esteja disponível para a plataforma específica."
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "HbB0r0Y6G6CH"
   },
   "source": [
    "### 1.2 - Aplicações:\n",
    "\n",
    "Python é uma linguagem de programação versátil e amplamente utilizada em várias aplicações:\n",
    "\n",
    "- **Inteligência Artificial e Aprendizado de Máquina:** Python é uma das principais linguagens usadas em projetos de IA e ML, com bibliotecas como *TensorFlow*, *Keras* e *PyTorch* permitindo a criação de modelos complexos de aprendizado de máquina e redes neurais.\n",
    "\n",
    "- **Análise e ciência de dados:** Python é uma escolha comum para análise e manipulação de dados devido às bibliotecas poderosas, como *Pandas* e *NumPy*, além de ferramentas para visualização de dados, como *Matplotlib* e *Seaborn*.\n",
    "\n",
    "- **Internet das Coisas (IoT):** Python é uma escolha popular para projetos de IoT devido à sua facilidade de integração com dispositivos e sensores.\n",
    "\n",
    "- **Desenvolvimento de aplicações científicas:** Python é amplamente usado em aplicações científicas para resolver problemas complexos, simulação e modelagem matemática.\n",
    "\n",
    "- **Desenvolvimento web**: Python é muito popular para criar aplicativos web, devido a frameworks como *Django* e *Flask*, que permitem o desenvolvimento rápido e eficiente de aplicações web robustas e escaláveis.\n",
    "\n",
    "- **Automação e scripts**: Python é frequentemente usado para escrever *scripts* e automatizar tarefas repetitivas no sistema operacional, tornando-o uma excelente escolha para administração de sistemas e tarefas de rotina.\n",
    "\n",
    "- **Desenvolvimento de jogos:** Python pode ser usado para o desenvolvimento de jogos com a ajuda de bibliotecas como *Pygame*, que fornecem funcionalidades de gráficos e interação com o usuário.\n",
    "\n",
    "- **Desenvolvimento de aplicativos de desktop:** Python pode ser usado para desenvolver aplicativos de desktop com interfaces gráficas usando ferramentas como *Tkinter*, *PyQT ou WXPython*."
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "7AkPI86SG6CI"
   },
   "source": [
    "### 1.3 - Ferramentas de desenvolvimento\n",
    "\n",
    "Temos várias opções quando se trata de escolher onde desenvolver nossos códigos Python. As opções variam de *ambientes de desenvolvimento integrado (IDEs)* a *editores de código e ambientes interativos*. Cada opção possui suas próprias vantagens e recursos, e a escolha dependerá das preferências pessoais do desenvolvedor e das necessidades específicas do projeto.\n",
    "\n",
    "IDEs:\n",
    "- **PyCharm:** desenvolvido pela JetBrains, é uma das IDEs mais poderosas e completas para o desenvolvimento Python. Disponível em uma edição Community gratuita e em uma edição Professional paga, o PyCharm oferece recursos avançados, como edição de código inteligente, depuração integrada, suporte a frameworks populares, gerenciamento de projetos e muito mais.\n",
    "\n",
    "- **Visual Studio Code (VS Code):** desenvolvido pela Microsoft, é um editor de código leve, altamente customizável e amplamente utilizado pela comunidade Python. Com uma grande variedade de extensões disponíveis, o VS Code pode ser adaptado para atender às necessidades específicas do desenvolvedor, incluindo suporte para Python, depuração e integração com sistemas de controle de versão.\n",
    "\n",
    "- **Spyder:** é uma IDE projetada especificamente para análise de dados e ciência de dados em Python. Ele oferece recursos como edição de código, console interativo e visualização de variáveis, tornando-o ideal para tarefas de análise e manipulação de dados.\n",
    "\n",
    "- **IDLE:** é um ambiente de desenvolvimento padrão incluído na distribuição oficial do Python. Embora seja uma opção mais básica em comparação com as IDEs mencionadas acima, o IDLE oferece recursos de edição de código e um console interativo para testar código rapidamente.\n",
    "\n",
    "Ambientes interativos:\n",
    "- **Jupyter Notebook:** é uma aplicação web interativa que permite criar documentos interativos chamados notebooks. Amplamente utilizado na área de ciência de dados e análise de dados, o Jupyter Notebook permite combinar código Python, texto formatado e visualizações em um único documento.\n",
    "\n",
    "- **Google Colab (Google Colaboratory):** é um serviço gratuito baseado em nuvem que permite criar e executar notebooks do Jupyter diretamente no navegador. É uma opção popular para desenvolver códigos Python, especialmente para projetos de aprendizado de máquina e ciência de dados. O Colab oferece acesso gratuito a recursos de computação na nuvem e a diversas bibliotecas populares de Python pré-instaladas, tornando-o uma escolha conveniente para experimentar algoritmos de aprendizado de máquina e realizar análise de dados de maneira colaborativa."
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "4h0uBIM4G6CI"
   },
   "source": [
    "### 1.4 - Instalação do Python e ambiente de desenvolvimento:\n",
    "\n",
    "Existem várias opções para instalar o Python em seu computador, mas uma das mais populares é a distribuição Anaconda, que inclui o Python e outras bibliotecas populares para ciência de dados e aprendizado de máquina. O ambiente de desenvolvimento mais comumente usado para Python é o IDLE (Integrated Development and Learning Environment), que é uma interface gráfica de usuário para escrever e executar código Python.\n",
    "\n",
    "##### Instalando o Python pela página oficial:\n",
    "\n",
    "    1 - Acesse o site oficial do Python em https://www.python.org/downloads/\n",
    "\n",
    "    2 - Clique no botão \"Download\" na página inicial.\n",
    "    Selecione a versão mais recente do Python e o sistema operacional correspondente. Por exemplo, para Windows, clique em \"Windows\" e, em seguida, na versão mais recente do Python.\n",
    "    3 - Baixe o instalador do Python e salve-o em seu computador.\n",
    "    4 - Execute o arquivo baixado e siga as instruções do instalador. Certifique-se de marcar a opção \"Add Python to PATH\" durante a instalação para que o Python possa ser facilmente acessado a partir do prompt de comando ou de qualquer outro ambiente de desenvolvimento.\n",
    "    5 - Depois de concluir a instalação, abra o prompt de comando e digite python --version para verificar se o Python foi instalado corretamente. Você deve ver a versão do Python que acabou de instalar.\n",
    "    \n",
    "##### Instalando o Python com Anaconda\n",
    "    1 - O Anaconda é uma distribuição de Python popular para ciência de dados e aprendizado de máquina, que inclui muitas bibliotecas e ferramentas populares. Aqui está como instalar o Python com Anaconda:\n",
    "\n",
    "    2 - Baixe o instalador do Anaconda em https://www.anaconda.com/products/individual\n",
    "    3 - Selecione a versão mais recente do Anaconda para o seu sistema operacional e baixe o instalador.\n",
    "    4 - Execute o arquivo baixado e siga as instruções do instalador.\n",
    "    5 - Durante a instalação, certifique-se de marcar as opções \"Add Anaconda to my PATH environment variable\" e \"Register Anaconda as my default Python\" para garantir que o Anaconda seja facilmente acessado e configurado como seu ambiente de desenvolvimento padrão.\n",
    "    \n",
    "Depois de concluir a instalação, abra o Anaconda Navigator (ou use o prompt de comando) para acessar o ambiente de desenvolvimento do Python e começar a programar.\n",
    "Com o Python e o ambiente de desenvolvimento instalados corretamente, você está pronto para começar a programar em Python!"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "rsIHNbKcG6CJ"
   },
   "source": [
    "### 1.5 - Executando o primeiro programa em Python:\n",
    "\n",
    "O código Python mais simples é uma declaração \"print\" que imprime uma mensagem na tela. Aqui está um exemplo:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 1,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 310,
     "status": "ok",
     "timestamp": 1690223196854,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "6l8nqBNZG6CJ",
    "outputId": "a6aa112a-2da1-46aa-9006-ae9f4748fd57"
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Olá, mundo!\n"
     ]
    }
   ],
   "source": [
    "print(\"Olá, mundo!\")"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "EyZUbhxoG6CL"
   },
   "source": [
    "**Nota:** Linhas iniciadas com # são comentários, que são ignorados pelo Python e servem para explicar o código."
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 2,
   "metadata": {
    "id": "cxajZSLZG6CL"
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Olá, mundo!\n"
     ]
    }
   ],
   "source": [
    "# Esse texto está comentado e será ignorado\n",
    "print(f\"Olá, mundo!\")"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "drjs3JHkG6CL"
   },
   "source": [
    "## 2 - Tipos de dados e variáveis:"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "JHZFr72HG6CL"
   },
   "source": [
    "Tecnicamente, podemos definir uma variável como sendo um identificador de um valor dentro da memória do computador. Se você preferir, pode imaginar uma variável como uma \"caixa de memória\" na qual é guardado algum valor. E que são esses valores? São os dados, informações que são armazenadas e manipuladas em um programa."
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "K8JYpNNxG6CL"
   },
   "source": [
    "### 2.1 - Tipos de dados em Python:\n",
    "\n",
    "- **Numéricos:** Em Python, existem dois tipos principais de dados numéricos, inteiros (*int*) e de ponto flutuante (*float*). Inteiros são números inteiros positivos ou negativos, enquanto números de ponto flutuante são números reais com um ponto decimal.\n",
    "\n",
    "Exemplos:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 3,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 9,
     "status": "ok",
     "timestamp": 1690223197737,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "Uj3cYu3xG6CL",
    "outputId": "48468d48-ab66-4ee2-e65f-2c1c8dc3020a"
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Inteiro: 2, <class 'int'>, Ponto flutuante: 3.14, <class 'float'>\n"
     ]
    }
   ],
   "source": [
    "a = 2 # inteiro (int)\n",
    "b = 3.14 # ponto flutuante (float)\n",
    "\n",
    "# mostra as variáveis a e b e seus respectivos tipos.\n",
    "print(f'Inteiro: {a}, {type(a)}, Ponto flutuante: {b}, {type(b)}')"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 4,
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "int"
      ]
     },
     "execution_count": 4,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "type(a)"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "VPwSpj5UG6CL"
   },
   "source": [
    "- **Strings:** Strings são sequências de caracteres. Em Python, eles são definidos entre aspas simples ou duplas.\n",
    "\n",
    "Exemplos:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 5,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 7,
     "status": "ok",
     "timestamp": 1690223197737,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "BibAVPciG6CL",
    "outputId": "c2b2636f-d49f-4b26-90ab-a52bb5a704e1",
    "scrolled": false
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "João\n",
      "Olá, mundo!\n"
     ]
    }
   ],
   "source": [
    "nome = 'João' #entre aspas simples\n",
    "mensagem = \"Olá, mundo!\" #entre aspas duplas\n",
    "\n",
    "print(nome)\n",
    "print(mensagem)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 6,
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Variável: João, tipo: <class 'str'>\n"
     ]
    }
   ],
   "source": [
    "print(f\"Variável: {nome}, tipo: {type(nome)}\")"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "dIPvhIGiG6CM"
   },
   "source": [
    "- **Booleanos:** Booleanos são valores lógicos que podem ser verdadeiros (True) ou falsos (False).\n",
    "\n",
    "Exemplos:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 7,
   "metadata": {
    "id": "uKM9rf9kG6CM"
   },
   "outputs": [],
   "source": [
    "verdadeiro = True\n",
    "falso = False"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 8,
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Variável: True, tipo: <class 'bool'>\n"
     ]
    }
   ],
   "source": [
    "print(f\"Variável: {verdadeiro}, tipo: {type(verdadeiro)}\")"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "yDNaTEUVG6CM"
   },
   "source": [
    "### 2.2 - Declaração de variáveis:\n",
    "\n",
    "Em Python, as variáveis são declaradas atribuindo um valor a um nome. O nome da variável pode ser qualquer combinação de letras, números e sublinhados, **desde que comece com uma letra**. Uma vez declarada, a variável pode ser chamada no programa sempre que necessitarmos acessar seu valor.\n",
    "\n",
    "Exemplos:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 9,
   "metadata": {
    "id": "nSE5Cg6dG6CM"
   },
   "outputs": [],
   "source": [
    "idade = 25\n",
    "nome = \"Maria\""
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "QG8fMghbG6CM"
   },
   "source": [
    "**Nota:** Não podemos declarar uma variável cujo nome comece com um número. Isso gera um **erro de sintaxe**."
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 10,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/",
     "height": 131
    },
    "executionInfo": {
     "elapsed": 24,
     "status": "error",
     "timestamp": 1690223198200,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "PhxRhS0_G6CM",
    "outputId": "50e1c45c-cca6-4b6b-eb56-0bf81c3cbc87",
    "scrolled": true
   },
   "outputs": [
    {
     "ename": "SyntaxError",
     "evalue": "invalid syntax (649981819.py, line 1)",
     "output_type": "error",
     "traceback": [
      "\u001b[1;36m  Cell \u001b[1;32mIn[10], line 1\u001b[1;36m\u001b[0m\n\u001b[1;33m    25anos = 25\u001b[0m\n\u001b[1;37m      ^\u001b[0m\n\u001b[1;31mSyntaxError\u001b[0m\u001b[1;31m:\u001b[0m invalid syntax\n"
     ]
    }
   ],
   "source": [
    "25anos = 25\n",
    "print(25anos)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 11,
   "metadata": {
    "scrolled": true
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "25\n"
     ]
    }
   ],
   "source": [
    "idade_25 = 25\n",
    "print(idade_25)"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "**Nota:** Algumas palavras são reservados pelo python e não pode ser usadas como nomes de variáveis, é o caso abaixo. "
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 12,
   "metadata": {},
   "outputs": [
    {
     "ename": "SyntaxError",
     "evalue": "invalid syntax (2644998005.py, line 1)",
     "output_type": "error",
     "traceback": [
      "\u001b[1;36m  Cell \u001b[1;32mIn[12], line 1\u001b[1;36m\u001b[0m\n\u001b[1;33m    if = 20\u001b[0m\n\u001b[1;37m       ^\u001b[0m\n\u001b[1;31mSyntaxError\u001b[0m\u001b[1;31m:\u001b[0m invalid syntax\n"
     ]
    }
   ],
   "source": [
    "if = 20"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "84nSUxG-G6CM"
   },
   "source": [
    "### 2.3 - Operações com variáveis:\n",
    "\n",
    "As variáveis em Python podem ser usadas em várias operações matemáticas e lógicas."
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "0RztPYMrG6CN"
   },
   "source": [
    "#### 2.3.1 - Operações matemáticas:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 13,
   "metadata": {
    "id": "n6T7_7jtG6CN"
   },
   "outputs": [],
   "source": [
    "# Definição das variáveis a e b\n",
    "a = 10\n",
    "b = 8"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 14,
   "metadata": {
    "id": "6VKO26kvG6CN"
   },
   "outputs": [],
   "source": [
    "# Operações\n",
    "c = a + b #adição\n",
    "d = a - b #subtração\n",
    "e = a * b #multiplicação\n",
    "f = a / b #divisão\n",
    "g = a % b #módulo (resto da divisão)\n",
    "h = a ** b #exponenciação"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 15,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 291,
     "status": "ok",
     "timestamp": 1690223564656,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "joOEocRRG6CN",
    "outputId": "665dc2c2-9a75-4194-9057-d93bddf21877",
    "scrolled": false
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "a + b = 18\n",
      "a - b = 2\n",
      "a * b = 80\n",
      "a / b = 1.25\n",
      "a % b = 2\n",
      "a ^ b = 100000000\n"
     ]
    }
   ],
   "source": [
    "# Nos comando abaixo função print utiliza(chama) as variáveis definidas anteriormente para escrever seus valores na tela\n",
    "print(f'a + b = {c}')\n",
    "print(f'a - b = {d}')\n",
    "print(f'a * b = {e}')\n",
    "print(f'a / b = {f}')\n",
    "print(f'a % b = {g}')\n",
    "print(f'a ^ b = {h}')"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "tsAM125sG6CN"
   },
   "source": [
    "**Nota:** Em python, o operador igual (=) não possui o mesmo significado e comportamento que na matemática. Na matemática, ele é um operador bidirecional: A = B seria a mesma coisa que B = A. No Python, ele é o que chamamos de um operador de **ATRIBUIÇÃO:** A variável da esquerda apenas armazena o valor da direita. Em outras palavras, o valor da direita é atribuido a variável à esquerda."
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "cadhm6pLG6CN"
   },
   "source": [
    "#### 2.3.2 - Operações lógicas e relacionais:\n",
    "\n",
    "Operadores lógicos e relacionais são usados para realizar diferentes tipos de comparações entre valores."
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "gBjhkbl5G6CN"
   },
   "source": [
    "Os operadores relacionais são usados para comparar valores e retornar um valor booleano (true ou false) com base na relação entre eles.\n",
    "\n",
    "Em Python existem 6 operadores relacionais:\n",
    "\n",
    "- **Maior que: >**\n",
    "- **Maior ou igual: >=**\n",
    "- **Menor que: <**\n",
    "- **Menor ou igual: <=**\n",
    "- **Igual: ==**\n",
    "- **Diferente: !=**"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "PJRSZRKnG6CN"
   },
   "source": [
    "**Nota:** Observe que o operador que compara se 2 valores são iguais é **==**, e não **=**. Isso ocorre porque o operador = é o nosso operador de **atribuição:** ele diz que a variável à sua esquerda deve receber o valor da expressão à direita. O operador == irá testar se o valor à sua esquerda é igual ao valor à sua direita e irá responder **True** ou **False**, assim como ocorre com todos os outros operadores de comparação."
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "AnE7sG6bG6CN"
   },
   "source": [
    "Os operadores lógicos são usados para avaliar condições booleanas, ou seja, expressões que podem ser verdadeiras ou falsas. Eles são usados para combinar ou inverter condições, e incluem os operadores:\n",
    "\n",
    "- **AND:** retorna verdadeiro (true) se **TODAS** as condições forem verdadeiras, caso contrário, retorna falso (false).\n",
    "- **OR:** retorna verdadeiro (true) se **AO MENOS UMA** das condições for verdadeira, caso contrário, retorna falso (false).\n",
    "- **NOT:** **INVERTE** o resultado booleano de uma certa condição. Retorna true se a condição avaliada for falsa e vice-versa."
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 16,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 277,
     "status": "ok",
     "timestamp": 1690223586279,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "HmLLy-FhG6CN",
    "outputId": "4893b457-0b15-47b2-c37c-05dc2065b594",
    "scrolled": true
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "a = 10, b = 8, a > b = True\n",
      "a = 10, b = 8, a == b = False\n",
      "a = 10, b = 8, a < b = False\n",
      "a = 10, b = 8, ~(a < b) = True\n"
     ]
    }
   ],
   "source": [
    "a = 10\n",
    "b = 8\n",
    "\n",
    "resultado1 = a > b # verdadeiro se a for maior que b\n",
    "resultado2 = a == b # verdadeiro se a for igual a b\n",
    "resultado3 = a < b # verdadeiro se a for menor que b\n",
    "resultado4 = not(resultado3) # inverte o resultado da condição a < b\n",
    "\n",
    "print(f'a = {a}, b = {b}, a > b = {resultado1}')\n",
    "print(f'a = {a}, b = {b}, a == b = {resultado2}')\n",
    "print(f'a = {a}, b = {b}, a < b = {resultado3}')\n",
    "print(f'a = {a}, b = {b}, ~(a < b) = {resultado4}')"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "fEJKv9KqG6CO"
   },
   "source": [
    "Podemos obter o resultado lógico da comparação de duas ou mais relações, por exemplo:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 17,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 260,
     "status": "ok",
     "timestamp": 1690223589142,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "xO9tJizUG6CO",
    "outputId": "0127b1bc-8f8c-485c-bfab-093c25aedb76"
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Resultado da operação 1:  True\n",
      "Resultado da operação 2:  False\n",
      "Resultado da operação 3:  True\n",
      "Resultado da operação 4:  True\n"
     ]
    }
   ],
   "source": [
    "operacao1 = 7 > 2 and 6 > 1 # Verdadeira se as duas condições são verdadeiras\n",
    "operacao2 = 5 == 3 and 6 > 3 # Verdadeira se as duas condições são verdadeiras\n",
    "operacao3 = 5 == 3 or 6 > 3 # Verdadeira se ao menos uma duas condições é verdadeira\n",
    "operacao4 = 5 != 3 and 6 > 3 and 1 > 0 # Verdadeira se as três condições são verdadeiras\n",
    "\n",
    "print('Resultado da operação 1: ', operacao1)\n",
    "print('Resultado da operação 2: ', operacao2)\n",
    "print('Resultado da operação 3: ', operacao3)\n",
    "print('Resultado da operação 4: ', operacao4)"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "KY23X0N_G6CO"
   },
   "source": [
    "**Nota:** é possível ainda fazer um tipo especial de operação com *strings* utilizando o operador **+**, denominada concatenação. O resultado nada mais é do que a junção de duas ou mais strings em uma única string, como mostra o exemplo abaixo:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 18,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 3,
     "status": "ok",
     "timestamp": 1690223591744,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "5QPbT14BG6CO",
    "outputId": "13be5102-0828-4251-e263-adac5638a092",
    "scrolled": true
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Meu nome é Bond, james Bond.\n"
     ]
    }
   ],
   "source": [
    "primeiro_nome = 'james'\n",
    "ultimo_nome = 'Bond'\n",
    "nome_completo = primeiro_nome + ' ' + ultimo_nome # Adicionamos um espaço entre os nomes\n",
    "print(f'Meu nome é {ultimo_nome}, {nome_completo}.')"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "IAl36DpNG6CR"
   },
   "source": [
    "### 2.4 - Exercícios:"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "HtIz38JPG6CR"
   },
   "source": [
    "#### Exercício 1:\n",
    "    a) Declare uma variável chamada \"nome_produto\" e atribua a ela uma string com o nome do produto que você deseja comprar.\n",
    "    b) Declare uma variável chamada \"preco_produto\" e atribua a ela o valor numérico do preço do produto que você deseja comprar.\n",
    "    c) Declare uma variável chamada \"quantidade\" e atribua a ela um número inteiro que represente quantos itens desse produto você pretende comprar.\n",
    "    d) Declare uma variável chamada \"total_compra\" e calcule o valor total da compra multiplicando o preço do produto pela quantidade desejada.\n",
    "    e) Utilize a função print() no padrão que temos usado até aqui para mostrar o nome do produto, o valor, a quantidade comprada e valor total da compra."
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 19,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 262,
     "status": "ok",
     "timestamp": 1690223597406,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "t2n8m2mrG6CR",
    "outputId": "81a1436e-ba84-4458-ceef-9f959f453c90"
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Nome do produto: Celular\n",
      "Preço do produto: 1200.5\n",
      "Quantidade comprada: 3\n",
      "Valor total da compra: 3601.5\n"
     ]
    }
   ],
   "source": [
    "# a)\n",
    "nome_produto = \"Celular\"\n",
    "\n",
    "# b)\n",
    "preco_produto = 1200.50\n",
    "\n",
    "# c)\n",
    "quantidade = 3\n",
    "\n",
    "# d)\n",
    "total_compra = preco_produto * quantidade\n",
    "\n",
    "# e)\n",
    "print(\"Nome do produto:\", nome_produto)\n",
    "print(\"Preço do produto:\", preco_produto)\n",
    "print(\"Quantidade comprada:\", quantidade)\n",
    "print(\"Valor total da compra:\", total_compra)"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "TO8zN4OFG6CR"
   },
   "source": [
    "#### Exercício 2:\n",
    "    a) Declare uma variável chamada \"saldo\" e atribua a ela um valor numérico que represente o saldo da sua conta bancária.\n",
    "    b) Declare uma variável chamada \"gastos\" e atribua a ela um valor numérico que represente quanto você gastou em uma compra.\n",
    "    c) Atualize o valor da variável \"saldo\" subtraindo o valor da variável \"gastos\".\n",
    "    d) Crie uma variável booleana chamada \"tem_saldo_positivo\" e atribua a ela o valor True se o saldo for maior ou igual a 0, caso contrário, atribua o valor False."
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 20,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 15,
     "status": "ok",
     "timestamp": 1690223198202,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "UaGgk58DG6CS",
    "outputId": "d5a1a6a1-e6b1-4882-a88c-ffe1d1755b3a"
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Saldo atual: 1150.55\n",
      "Tem saldo positivo? True\n"
     ]
    }
   ],
   "source": [
    "# a)\n",
    "saldo = 1500.75\n",
    "\n",
    "# b)\n",
    "gastos = 350.20\n",
    "\n",
    "# c)\n",
    "saldo = saldo - gastos\n",
    "\n",
    "# d)\n",
    "tem_saldo_positivo = saldo >= 0\n",
    "\n",
    "print(\"Saldo atual:\", saldo)\n",
    "print(\"Tem saldo positivo?\", tem_saldo_positivo)\n"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "JI7oOiNVG6CS"
   },
   "source": [
    "#### Exercício 3:\n",
    "    a) Declare uma variável chamada \"frase\" e atribua a ela uma string com uma frase de sua escolha.\n",
    "    b) Crie uma variável chamada \"tamanho_frase\" e calcule o tamanho da string \"frase\" usando a função len().\n",
    "    c) Declare uma variável chamada \"caractere\" e atribua a ela uma letra qualquer da \"frase\".\n",
    "    d) Crie uma variável chamada \"quantidade_caractere\" e conte quantas vezes o \"caractere\" escolhido aparece na \"frase\" usando o método count()."
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 21,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 12,
     "status": "ok",
     "timestamp": 1690223198202,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "a7DrJIklG6CS",
    "outputId": "b5f1cf18-efd0-490d-8c09-b7dc48aa1ed4"
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Frase: A vida é bela e cheia de surpresas.\n",
      "Tamanho da frase: 35\n",
      "Caractere escolhido: e\n",
      "Quantidade do caractere na frase: 5\n"
     ]
    }
   ],
   "source": [
    "# a)\n",
    "frase = \"A vida é bela e cheia de surpresas.\"\n",
    "\n",
    "# b)\n",
    "tamanho_frase = len(frase)\n",
    "\n",
    "# c)\n",
    "caractere = \"e\"\n",
    "\n",
    "# d)\n",
    "quantidade_caractere = frase.count(caractere)\n",
    "\n",
    "# Mostra o tamanho da frase e a quantidade de vezes que o caractere escolhido aparece na frase\n",
    "print(\"Frase:\", frase)\n",
    "print(\"Tamanho da frase:\", tamanho_frase)\n",
    "print(\"Caractere escolhido:\", caractere)\n",
    "print(\"Quantidade do caractere na frase:\", quantidade_caractere)"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "ALSR0Hc_G6CS"
   },
   "source": [
    "## 3 - Estruturas de controle de fluxo:\n",
    "\n",
    "As estruturas de controle de fluxo são recursos fundamentais em programação, pois permitem controlar a sequência de execução das instruções em um programa. Elas permitem que você tome decisões e repita ações com base em determinadas condições. Essas estruturas permitem que você crie programas mais flexíveis e dinâmicos, adaptando o comportamento do programa de acordo com as condições e requisitos específicos. Combinando essas estruturas de maneira adequada, é possível construir algoritmos complexos e resolver uma ampla variedade de problemas de programação.\n",
    "\n",
    "Existem três principais estruturas de controle de fluxo:"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "HRYnxaQaG6CS"
   },
   "source": [
    "### 3.1 - Estruturas Condicionais\n",
    "\n",
    "As instruções condicionais permitem que você tome decisões com base em condições específicas. A estrutura mais comum é o \"if-else\" (se-senão), que avalia uma condição e executa um bloco de código se a condição for verdadeira e outro bloco se a condição for falsa. Também existe a estrutura \"if-elif-else\" (se-senão se-senão), que permite avaliar múltiplas condições sequencialmente."
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "UZry6sM5G6CS"
   },
   "source": [
    "#### 3.1.1 if/else:\n",
    "A estrutura if/else é usada para testar uma condição e executar diferentes blocos de código, dependendo se a condição é verdadeira ou falsa. No caso do if, queremos que o programa execute um código se uma dada condição for atendida. Já se estamos interessados que o programa escolha entre 2 casos mutuamente exclusivos, utilizamos o if e o else conjuntamente. O else não possui condição para verificar e sempre vem imediatamente após um if e é executado se o if for ignorado.\n",
    "\n",
    "A sintaxe básica é a seguinte:"
   ]
  },
  {
   "cell_type": "raw",
   "metadata": {
    "id": "4i9TPP2dG6CS"
   },
   "source": [
    "# Caso do if isolado\n",
    "if condicao:\n",
    "    # codigo a ser executado se a condição for verdadeira"
   ]
  },
  {
   "cell_type": "raw",
   "metadata": {
    "id": "9z-776xcG6CS"
   },
   "source": [
    "# Caso do if e else em conjunto\n",
    "if condicao:\n",
    "    # codigo a ser executado se a condição for verdadeira\n",
    "else:\n",
    "    # codigo a ser executado se a condição for falsa"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "Exemplos:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 22,
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "A condição é verdadeira\n"
     ]
    }
   ],
   "source": [
    "# Caso do if isolado\n",
    "condicao = True\n",
    "if condicao:\n",
    "  # codigo a ser executado se a condição for verdadeira\n",
    "  print('A condição é verdadeira')"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 23,
   "metadata": {},
   "outputs": [],
   "source": [
    "# Caso do if isolado\n",
    "condicao = False\n",
    "if condicao:\n",
    "  # codigo a ser executado se a condição for verdadeira\n",
    "  print('A condição é verdadeira')"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 24,
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Isso não faz parte do if\n"
     ]
    }
   ],
   "source": [
    "# Comentario sobre a identação\n",
    "condicao = False\n",
    "if condicao:\n",
    "  # codigo a ser executado se a condição for verdadeira\n",
    "  print('A condição é verdadeira')\n",
    "\n",
    "print('Isso não faz parte do if')"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 25,
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "A condição é verdadeira\n"
     ]
    }
   ],
   "source": [
    "# Caso do if e else em conjunto\n",
    "condicao = True\n",
    "if condicao:\n",
    "    # codigo a ser executado se a condição for verdadeira\n",
    "    print('A condição é verdadeira')\n",
    "else:\n",
    "    # codigo a ser executado se a condição for falsa\n",
    "    print('A condição é falsa')"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 26,
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "A condição é falsa\n"
     ]
    }
   ],
   "source": [
    "# Caso do if e else em conjunto\n",
    "condicao = False\n",
    "if condicao:\n",
    "    # codigo a ser executado se a condição for verdadeira\n",
    "    print('A condição é verdadeira')\n",
    "else:\n",
    "    # codigo a ser executado se a condição for falsa\n",
    "    print('A condição é falsa')"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "1ASAhDicG6CT"
   },
   "source": [
    "Mais um exemplo: suponha que queremos escrever um código que verifica se um número é positivo ou negativo:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 27,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 3860,
     "status": "ok",
     "timestamp": 1690223613261,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "lmrmzUU4G6CT",
    "outputId": "b5fd905b-2618-420c-d6f7-562e98bdd5b2",
    "scrolled": true
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Digite um número: 18\n",
      "O número é positivo\n"
     ]
    }
   ],
   "source": [
    "numero = int(input(\"Digite um número: \"))\n",
    "\n",
    "if numero > 0:\n",
    "    print(\"O número é positivo\")\n",
    "else:\n",
    "    print(\"O número é negativo ou zero\")"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "eHRKz8YCG6CT"
   },
   "source": [
    "**Nota:** Utilizamos um 'tab' antes de cada linha pertencente ao if. Esse processo é chamado de \"indentação\", cujo objetivo é melhorar a legibilidade e organização do código."
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "St0hGfD-G6CT"
   },
   "source": [
    "É possível encadear diversos if's e else's, como mostra o programa abaixo:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 28,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 3011,
     "status": "ok",
     "timestamp": 1690223620255,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "VuyD4e7lG6CT",
    "outputId": "321f786d-f06e-4648-95d1-b08f42f88247"
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Digite a temperatura atual: 36\n",
      "Gostaria de se refrescar em uma piscina? sim\n",
      "Ótimo! A piscina está aberta, aproveite!\n"
     ]
    }
   ],
   "source": [
    "tempo = float(input('Digite a temperatura atual: '))\n",
    "if tempo >= 30:\n",
    "    resposta = input('Gostaria de se refrescar em uma piscina? ')\n",
    "    if resposta == 'sim':\n",
    "        print('Ótimo! A piscina está aberta, aproveite!')\n",
    "    else:\n",
    "        print('Tudo bem, aproveite o seu dia!')\n",
    "else:\n",
    "    print('A temperatura não está alta o suficiente para aproveitar uma piscina neste momento.')"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "VWfXrddZG6CT"
   },
   "source": [
    "Por fim, podemos testar diversos casos mutuamente exclusivos utilizando o 'elif'.\n",
    "\n",
    "O comando elif é a contração de \"else if\" - ou seja, caso um if não seja executado, você pode propor uma nova condição para ser testada."
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 29,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 2983,
     "status": "ok",
     "timestamp": 1690223626560,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "JBlSLPkZG6CT",
    "outputId": "14367915-1353-40db-a9be-2cf96f0f464c"
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Quantos exercícios de Python você já fez?56\n",
      "Já está ficando profissional!\n"
     ]
    }
   ],
   "source": [
    "exercicios = int(input('Quantos exercícios de Python você já fez?'))\n",
    "\n",
    "if exercicios > 30:\n",
    "    print('Já está ficando profissional!')\n",
    "elif exercicios > 20:\n",
    "    print('Tá indo bem, bora fazer mais alguns!')\n",
    "elif exercicios > 10:\n",
    "    print('Vamos tirar o atraso?')\n",
    "else:\n",
    "    print('Xiiii...')"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "_kJoGJdXG6CT"
   },
   "source": [
    "A vantagem de usar a estrutura elif é a possibilidade de verificar múltiplas condições de forma mais concisa e eficiente.\n",
    "\n",
    "Ao usar uma série de instruções if independentes, todas as condições são verificadas, mesmo que uma delas já tenha sido satisfeita. Isso pode resultar em um desperdício de recursos computacionais, especialmente quando há muitas condições a serem verificadas.\n",
    "\n",
    "Por outro lado, o uso do elif permite que o programa verifique as condições em sequência e execute apenas o bloco de código correspondente à primeira condição verdadeira encontrada. Isso significa que assim que uma condição for satisfeita, as condições subsequentes serão ignoradas.\n",
    "\n",
    "Essa abordagem economiza tempo de processamento, pois o programa não precisa verificar todas as condições se a primeira já for verdadeira. Além disso, torna o código mais legível e organizado, especialmente quando há uma lógica complexa com várias condições a serem avaliadas."
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "uUo3KvfyG6CT"
   },
   "source": [
    "### 3.2 Estruturas de Repetição\n",
    "\n",
    "Os loops permitem que você repita a execução de um bloco de código várias vezes. Existem dois tipos principais de loops: \"while\" (enquanto) e \"for\". O loop \"while\" repete o bloco de código enquanto uma determinada condição for verdadeira. O loop \"for\" é usado para iterar sobre uma sequência de elementos, como uma lista, e executar o bloco de código para cada elemento da sequência."
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "8phsHCElG6CU"
   },
   "source": [
    "#### 3.2.1 while:\n",
    "\n",
    "A estrutura while é usada para repetir um bloco de código enquanto uma condição é verdadeira. A sintaxe básica é a seguinte:"
   ]
  },
  {
   "cell_type": "raw",
   "metadata": {
    "id": "Y1b9xo2gG6CU"
   },
   "source": [
    "while condicao:\n",
    "    # codigo a ser repetido enquanto a condicao for verdadeira"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "rDB2fvugG6CU"
   },
   "source": [
    "Por exemplo, suponha que queremos escrever um código que imprime os números de 1 a 10:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 30,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 297,
     "status": "ok",
     "timestamp": 1690223631236,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "cJ5TdyDLG6CU",
    "outputId": "5a256b14-21af-4d3a-9c18-b22d88484ab7"
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "1\n",
      "2\n",
      "3\n",
      "4\n",
      "5\n",
      "6\n",
      "7\n",
      "8\n",
      "9\n",
      "10\n"
     ]
    }
   ],
   "source": [
    "numero = 1\n",
    "\n",
    "while numero <= 10:\n",
    "    print(numero)\n",
    "    numero += 1"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "msqfaN1YG6CU"
   },
   "source": [
    "#### 3.2.2 for:\n",
    "\n",
    "A estrutura for é usada para iterar sobre uma sequência, como uma lista ou uma string. A sintaxe básica é a seguinte:"
   ]
  },
  {
   "cell_type": "raw",
   "metadata": {
    "id": "EwGkIxmoG6CU"
   },
   "source": [
    "for elemento in sequencia:\n",
    "    # codigo a ser executado para cada elemento da sequencia"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "e4X6bZAAG6CU"
   },
   "source": [
    "Por exemplo, suponha que queremos escrever um código que imprime os elementos de uma lista:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 31,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 261,
     "status": "ok",
     "timestamp": 1690223634193,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "E9FvNDnBG6CU",
    "outputId": "b3a7b41d-3f08-4736-8140-089320117a36"
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "maçã\n",
      "banana\n",
      "laranja\n"
     ]
    }
   ],
   "source": [
    "lista_frutas = [\"maçã\", \"banana\", \"laranja\"]\n",
    "\n",
    "for fruta in lista_frutas:\n",
    "    print(fruta)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 32,
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "0\n",
      "1\n",
      "2\n",
      "3\n",
      "4\n",
      "5\n",
      "6\n",
      "7\n",
      "8\n",
      "9\n",
      "10\n"
     ]
    }
   ],
   "source": [
    "# Mostre os número de 0 a 10 usando o for\n",
    "lista_numeros = [0,1,2,3,4,5,6,7,8,9,10]\n",
    "\n",
    "for numero in lista_numeros:\n",
    "    print(numero)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 33,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 311,
     "status": "ok",
     "timestamp": 1690223636611,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "0xAe37r_G6CU",
    "outputId": "eeb58244-cd27-4456-97cb-2ecb3378567c"
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "1\n",
      "2\n",
      "3\n",
      "4\n",
      "5\n",
      "6\n",
      "7\n",
      "8\n",
      "9\n",
      "10\n"
     ]
    }
   ],
   "source": [
    "# Mostrar os números de 1 a 10\n",
    "for numero in range(1,11):\n",
    "    print(numero)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 34,
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "0\n",
      "1\n",
      "2\n",
      "3\n",
      "4\n",
      "5\n",
      "6\n",
      "7\n",
      "8\n",
      "9\n",
      "10\n"
     ]
    }
   ],
   "source": [
    "for numero in range(0,11):\n",
    "    print(numero)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 35,
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "1200.0\n",
      "2400.0\n"
     ]
    }
   ],
   "source": [
    "lista_salarios = [1000, 2000]\n",
    "for salario in lista_salarios:\n",
    "  novo_salario = salario*1.2\n",
    "  print(novo_salario)"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "X8TFOJRmG6CV"
   },
   "source": [
    "### 3.3 - Instruções de controle de fluxo\n",
    "\n",
    "Existem também as instruções de controle de fluxo em Python, como o break e o continue, que permitem que você interrompa ou pule partes de um loop. Essas estruturas são úteis em muitas situações, como quando você quer sair de um loop assim que encontrar o resultado desejado.\n",
    "\n",
    "Dominar as estruturas de controle de fluxo é fundamental para programar em Python e em qualquer outra linguagem de programação. Elas permitem que você crie programas mais sofisticados e eficientes, que podem lidar com uma variedade de situações e condições."
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "bqUK8nlUG6CV"
   },
   "source": [
    "#### 3.3.1 Break\n",
    "A instrução break é usada para interromper a execução de um loop imediatamente, mesmo que a condição do loop ainda não tenha sido completamente avaliada. Quando o break é encontrado, o programa sai do loop e continua a execução a partir da próxima linha após o loop."
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "QPNaHAaLG6CV"
   },
   "source": [
    "O loop abaixo em tese seria infinito, mas se a condição do if for verificada, o break é executado e conseguimos escapar do loop:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 38,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 5538,
     "status": "ok",
     "timestamp": 1690223645444,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "4h9R309CG6CV",
    "outputId": "4d65dc40-3383-46b2-d927-39ab95668cd1"
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Digite OK: Não\n",
      "Digite OK: Não\n",
      "Digite OK: OK\n"
     ]
    }
   ],
   "source": [
    "while True:\n",
    "    resposta = input('Digite OK: ')\n",
    "    if resposta == 'OK':\n",
    "        break"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "0YP5NnwLG6CV"
   },
   "source": [
    "Um outro exemplo, seria:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 39,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 3,
     "status": "ok",
     "timestamp": 1690223645445,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "6rJ2Ck1eG6CV",
    "outputId": "8dff2ebc-9d3a-44b2-957c-9a2319a6ea02"
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "1\n",
      "2\n",
      "3\n"
     ]
    }
   ],
   "source": [
    "numeros = [1, 2, 3, 4, 5, 6]\n",
    "\n",
    "for numero in numeros:\n",
    "    if numero == 4:\n",
    "        break\n",
    "    print(numero)"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "pfsGCbWkG6CW"
   },
   "source": [
    "#### 3.3.2 Continue\n",
    "\n",
    "A instrução continue é usada para pular o restante do código dentro do loop e continuar para a próxima iteração. Quando o continue é encontrado, o programa ignora qualquer código restante dentro do bloco do loop e passa para a próxima iteração.\n"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 40,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 297,
     "status": "ok",
     "timestamp": 1690223649833,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "ifcOMC99G6CW",
    "outputId": "fdea81e8-79d9-45c7-e534-11826f45d9cb"
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "1\n",
      "3\n",
      "5\n"
     ]
    }
   ],
   "source": [
    "numeros = [1, 2, 3, 4, 5, 6]\n",
    "\n",
    "for numero in numeros:\n",
    "    if numero % 2 == 0:\n",
    "        continue\n",
    "    print(numero)"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "So4e_3fyG6CW"
   },
   "source": [
    "### 3.4 - Exercícios"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "hr33yUBFG6CW"
   },
   "source": [
    "**Exercício 1:** Faça um programa que peça ao usuário a idade e verifique se a pessoa já pode votar (idade maior ou igual a 16 anos)."
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 41,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 3696,
     "status": "ok",
     "timestamp": 1690223655939,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "qi0OuD_TG6CW",
    "outputId": "12ef9005-5677-4202-cff6-8b007ee4c5f3"
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Digite sua idade: 56\n",
      "Você já pode votar!\n"
     ]
    }
   ],
   "source": [
    "# Solicita a idade do usuário\n",
    "idade = int(input(\"Digite sua idade: \"))\n",
    "\n",
    "# Verifica se a pessoa pode votar (idade maior ou igual a 16 anos)\n",
    "if idade >= 16:\n",
    "    print(\"Você já pode votar!\")\n",
    "else:\n",
    "    print(\"Você ainda não pode votar.\")"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "u-FxO7TYG6CW"
   },
   "source": [
    "**Exercício 2:** Escreva um programa que solicite ao usuário um número e exiba se esse número é positivo, negativo ou igual a zero."
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 42,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 3522,
     "status": "ok",
     "timestamp": 1690223661544,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "HsWZ8u6iG6CW",
    "outputId": "eb3d707b-77a6-4ec8-b783-9d68c000deb3"
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Digite um número: 6\n",
      "O número é positivo.\n"
     ]
    }
   ],
   "source": [
    "# Solicita ao usuário um número\n",
    "numero = int(input(\"Digite um número: \"))\n",
    "\n",
    "# Verifica se o número é positivo, negativo ou igual a zero\n",
    "if numero > 0:\n",
    "    print(\"O número é positivo.\")\n",
    "elif numero < 0:\n",
    "    print(\"O número é negativo.\")\n",
    "else:\n",
    "    print(\"O número é igual a zero.\")\n"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "cHJBnOI6G6CX"
   },
   "source": [
    "**Exercício 3:** Escreva um programa que solicite ao usuário um número inteiro positivo e faça uma contagem regressiva a partir desse número até zero. O programa deve exibir os números na tela enquanto realiza a contagem."
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 43,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 4948,
     "status": "ok",
     "timestamp": 1690223668318,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "GtTdIpQRG6CX",
    "outputId": "fa253aca-a5c2-42f9-e118-e75397bee761"
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Digite um número inteiro positivo: 12\n",
      "Contagem regressiva:\n",
      "12\n",
      "11\n",
      "10\n",
      "9\n",
      "8\n",
      "7\n",
      "6\n",
      "5\n",
      "4\n",
      "3\n",
      "2\n",
      "1\n",
      "0\n"
     ]
    }
   ],
   "source": [
    "# Solicita ao usuário um número inteiro positivo\n",
    "numero_str = input(\"Digite um número inteiro positivo: \")\n",
    "\n",
    "# Converte o número para um valor inteiro\n",
    "numero = int(numero_str)\n",
    "\n",
    "# Verifica se o número é positivo\n",
    "if numero <= 0:\n",
    "    print(\"O número digitado não é um inteiro positivo.\")\n",
    "else:\n",
    "    # Contagem regressiva\n",
    "    print(\"Contagem regressiva:\")\n",
    "    while numero >= 0:\n",
    "        print(numero)\n",
    "        numero -= 1"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "7Xs9T33sG6CX"
   },
   "source": [
    "**Exercício 4:** Escreva um programa que exiba os números pares de 0 a 20 usando um loop while."
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 44,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 3,
     "status": "ok",
     "timestamp": 1690223668318,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "L4Rl9nKsG6CX",
    "outputId": "c79982c9-bc8c-4093-b2fd-1eaee692eb5d"
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Números pares de 0 a 20:\n",
      "0\n",
      "2\n",
      "4\n",
      "6\n",
      "8\n",
      "10\n",
      "12\n",
      "14\n",
      "16\n",
      "18\n",
      "20\n"
     ]
    }
   ],
   "source": [
    "# Inicializa o contador com o valor 0\n",
    "numero = 0\n",
    "\n",
    "# Loop while para exibir os números pares de 0 a 20\n",
    "print(\"Números pares de 0 a 20:\")\n",
    "while numero <= 20:\n",
    "    print(numero)\n",
    "    numero += 2"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "aMeayl4jG6CX"
   },
   "source": [
    "**Exercício 5:** Escreva um programa que exiba os números pares de 0 a 20 usando um loop for."
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 45,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 271,
     "status": "ok",
     "timestamp": 1690223672638,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "ccOHXK6dG6CX",
    "outputId": "e350844a-19f8-4184-efb0-8e6b335ff29e"
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Números pares de 0 a 20:\n",
      "0\n",
      "2\n",
      "4\n",
      "6\n",
      "8\n",
      "10\n",
      "12\n",
      "14\n",
      "16\n",
      "18\n",
      "20\n"
     ]
    }
   ],
   "source": [
    "# Loop for para exibir os números pares de 0 a 20\n",
    "print(\"Números pares de 0 a 20:\")\n",
    "for numero in range(0, 21, 2):\n",
    "    print(numero)"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "s5GnX_b3G6CY"
   },
   "source": [
    "**Exercício 6:** Crie um programa que calcule a soma dos números de 1 a 100 (1+2+3+...+100) usando um loop for."
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 46,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 403,
     "status": "ok",
     "timestamp": 1690223675093,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "iA0koxAxG6CY",
    "outputId": "77e92fc8-dd63-492f-e949-4a7f2d911422"
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "A soma dos números de 1 a 100 é: 5050\n"
     ]
    }
   ],
   "source": [
    "# Inicializa a variável para armazenar a soma\n",
    "soma = 0\n",
    "# Loop for para somar os números de 1 a 100\n",
    "for numero in range(1, 101):\n",
    "    soma += numero\n",
    "\n",
    "# Exibe o resultado da soma\n",
    "print(\"A soma dos números de 1 a 100 é:\", soma)"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "zks-grZEG6CY"
   },
   "source": [
    "**Exercício 7:** Escreva um programa que imprima os números de 1 a 10, exceto o número 5. Use a instrução \"continue\" para pular o número 5."
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 47,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 261,
     "status": "ok",
     "timestamp": 1690223677180,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "TqZyuyUtG6CY",
    "outputId": "971954cd-b4d8-4bde-aadd-85541805c7ae"
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Números de 1 a 10, exceto o número 5:\n",
      "1\n",
      "2\n",
      "3\n",
      "4\n",
      "6\n",
      "7\n",
      "8\n",
      "9\n",
      "10\n"
     ]
    }
   ],
   "source": [
    "# Loop for para imprimir os números de 1 a 10, exceto o número 5\n",
    "print(\"Números de 1 a 10, exceto o número 5:\")\n",
    "for numero in range(1, 11):\n",
    "    if numero == 5:\n",
    "        continue\n",
    "    print(numero)"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "TdKavxlAG6CY"
   },
   "source": [
    "**Exercício 8:** Escreva um programa que exiba os números de 1 a 20, mas interrompa o loop quando encontrar um número divisível por 7. Use a instrução \"break\" para sair do loop quando essa condição for atendida."
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 48,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 294,
     "status": "ok",
     "timestamp": 1690223679851,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "qQJKMfotG6CY",
    "outputId": "d464a16b-5006-4e73-8e75-3d2db5f78390"
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Números de 1 a 20 (com interrupção no primeiro número divisível por 7):\n",
      "1\n",
      "2\n",
      "3\n",
      "4\n",
      "5\n",
      "6\n",
      "7\n"
     ]
    }
   ],
   "source": [
    "# Loop for para exibir os números de 1 a 20, interrompendo quando encontrar um número divisível por 7\n",
    "print(\"Números de 1 a 20 (com interrupção no primeiro número divisível por 7):\")\n",
    "for numero in range(1, 21):\n",
    "    print(numero)\n",
    "    if numero % 7 == 0:\n",
    "        break"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "Z7pMBhsDG6CY"
   },
   "source": [
    "## 4 - Estruturas de Dados:\n",
    "\n",
    "As estruturas de dados são fundamentais para organizar e manipular informações em um programa de forma eficiente. Compreender o funcionamento e a utilização dessas estruturas é essencial para o desenvolvimento de aplicações robustas e versáteis."
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "fQA03ly5G6CY"
   },
   "source": [
    "### 4.1 Listas\n",
    "\n",
    "Listas são estruturas de dados versáteis que permitem armazenar uma coleção ordenada de elementos em uma única variável.\n",
    "\n",
    "Características das listas:\n",
    "- Listas são mutáveis, ou seja, seus elementos podem ser modificados após a criação.\n",
    "- São definidas utilizando colchetes ([]).\n",
    "- Os elementos em uma lista podem ser de tipos diferentes."
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "m6eYlAbYG6CY"
   },
   "source": [
    "Exemplo de criação de uma lista:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 49,
   "metadata": {
    "id": "4KvWM7J9G6CZ"
   },
   "outputs": [],
   "source": [
    "lista_numeros = [1, 2, 3, 4, 5]"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "bxLq7vDJG6CZ"
   },
   "source": [
    "#### 4.1.2 Acesso e manipulação de elementos em Listas\n",
    "\n",
    "Para acessar elementos em uma lista, utilizamos índices numéricos, começando por 0 para o primeiro elemento (lista[0]).\n",
    "\n",
    "Exemplo de acesso a elementos:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 50,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 284,
     "status": "ok",
     "timestamp": 1690223684998,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "65AHTP6EG6CZ",
    "outputId": "4139be75-5a63-4ac4-e143-c01efc46e882"
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "maçã\n",
      "laranja\n",
      "morango\n",
      "morango\n"
     ]
    }
   ],
   "source": [
    "lista_frutas = ['maçã', 'banana', 'laranja', 'morango']\n",
    "\n",
    "print(lista_frutas[0]) # Acessa o primeiro elemnento\n",
    "print(lista_frutas[2]) # Acessa o terceiro elemento\n",
    "print(lista_frutas[3]) # Acessa o quarto e último elemento\n",
    "print(lista_frutas[-1]) # Acessa o último elemento"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "pcGeTcHOG6CZ"
   },
   "source": [
    "Para alterar elementos em uma lista, basta atribuir um novo valor ao índice desejado.\n",
    "\n",
    "Exemplo de manipulação de elementos:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 51,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 279,
     "status": "ok",
     "timestamp": 1690223687473,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "zmDP4g2MG6CZ",
    "outputId": "8b61fa00-3256-4eba-c88b-45f308ede57c"
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "['maçã', 'abacaxi', 'laranja', 'morango']\n"
     ]
    }
   ],
   "source": [
    "# Substitui o segundo elemento\n",
    "lista_frutas[1] = 'abacaxi'\n",
    "print(lista_frutas)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 52,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 262,
     "status": "ok",
     "timestamp": 1690223689301,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "I6Ju4ef0G6CZ",
    "outputId": "feb3b94c-d6b1-406d-e281-cebae83f05eb"
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "['abacaxi', 'laranja', 'morango']\n"
     ]
    }
   ],
   "source": [
    "# Remove o primeiro elemento\n",
    "\n",
    "del lista_frutas[0]\n",
    "print(lista_frutas)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 53,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 3,
     "status": "ok",
     "timestamp": 1690223690896,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "ihJkLxfuG6CZ",
    "outputId": "c8cb90b7-7364-43a1-8227-a8a3c8027aff"
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "['abacaxi', 'laranja']\n"
     ]
    }
   ],
   "source": [
    "# Usando o método pop()\n",
    "lista_frutas.pop(2)\n",
    "print(lista_frutas)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 54,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 304,
     "status": "ok",
     "timestamp": 1690223692697,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "eZcQs6cYG6Ca",
    "outputId": "d640bb05-a738-4655-ad58-9cb746e41583"
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "['abacaxi', 'laranja', 'Maracujá']\n"
     ]
    }
   ],
   "source": [
    "# Adiciona novos elementos à lista (método append())\n",
    "lista_frutas.append('Maracujá')\n",
    "print(lista_frutas)"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "-G8BNy1JG6Ca"
   },
   "source": [
    "Usando loops:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 55,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 316,
     "status": "ok",
     "timestamp": 1690223694760,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "U1aZL7r0G6Ca",
    "outputId": "01bd0724-b7f5-4b04-88c4-8b8125493c72",
    "scrolled": true
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "abacaxi\n",
      "laranja\n",
      "Maracujá\n"
     ]
    }
   ],
   "source": [
    "for fruta in lista_frutas:\n",
    "    print(fruta)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 56,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 328,
     "status": "ok",
     "timestamp": 1690223696579,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "dyIGA0lDG6Ca",
    "outputId": "48ef2f7c-004e-4c33-c7a9-5878f90495a8"
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "0 abacaxi\n",
      "1 laranja\n",
      "2 Maracujá\n"
     ]
    }
   ],
   "source": [
    "for index in range(len(lista_frutas)):\n",
    "    print(index, lista_frutas[index])"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 57,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 283,
     "status": "ok",
     "timestamp": 1690223698368,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "_RJFNTXOG6Ca",
    "outputId": "89efce53-70f5-4fa3-89ca-689836711240"
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "0 abacaxi\n",
      "1 laranja\n",
      "2 Maracujá\n"
     ]
    }
   ],
   "source": [
    "index = 0\n",
    "while index < len(lista_frutas):\n",
    "    print(index, lista_frutas[index])\n",
    "    index +=1"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 58,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 271,
     "status": "ok",
     "timestamp": 1690223700254,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "v-rqzCsgG6Ca",
    "outputId": "4f99586e-94ec-4542-f4e8-4a0fd7bcaaa7"
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10]\n"
     ]
    }
   ],
   "source": [
    "# Cria uma lista com os números de 0 a 10\n",
    "lista_numeros = []\n",
    "\n",
    "for numero in range(11):\n",
    "    lista_numeros.append(numero)\n",
    "\n",
    "print(lista_numeros)"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "S0NXjQ93G6Ca"
   },
   "source": [
    "### 4.2 Tuplas em Python:\n",
    "\n",
    "Tuplas são estruturas de dados **imutáveis** que permitem armazenar uma coleção ordenada de elementos em uma única variável.\n",
    "\n",
    "- Tuplas são definidas utilizando parênteses ()\n",
    "- Os elementos em uma tupla podem ser de tipos diferentes\n",
    "- Os elementos em uma tupla NÃO podem ser modificados"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "qSmwcCU8G6Ca"
   },
   "source": [
    "Exemplo de criação de uma tupla:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 59,
   "metadata": {
    "id": "zvbvnWdaG6Cb"
   },
   "outputs": [],
   "source": [
    "tupla_coordenadas = (10, 20)"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "YTYJYp1wG6Cb"
   },
   "source": [
    "#### 4.2.1 Acesso e Manipulação de elementos em Tuplas:\n",
    "Para acessar elementos em uma tupla, também utilizamos índices numéricos, começando por 0 para o primeiro elemento (tupla[0]).\n",
    "\n",
    "Exemplo de acesso a elementos:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 60,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 296,
     "status": "ok",
     "timestamp": 1690223704923,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "x-eRJkOLG6Cb",
    "outputId": "c0597da7-ab86-4735-ce2e-bdedd8915fc2",
    "scrolled": false
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "3\n",
      "5\n"
     ]
    }
   ],
   "source": [
    "ponto = (3, 5)\n",
    "print(ponto[0])\n",
    "print(ponto[1])"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "ggB7f0TeG6Cb"
   },
   "source": [
    "Concatenação"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 61,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 259,
     "status": "ok",
     "timestamp": 1690223706786,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "MBeZ8LEFG6Cb",
    "outputId": "4985f46d-a0b4-4db4-c2ef-ba109f385a03"
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "(1, 2, 3, 4)\n"
     ]
    }
   ],
   "source": [
    "tupla1 = (1,2)\n",
    "tupla2 = (3,4)\n",
    "concatenacao = tupla1 + tupla2\n",
    "print(concatenacao)"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "p0_1NgGaG6Cb"
   },
   "source": [
    "Usando loops:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 62,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 258,
     "status": "ok",
     "timestamp": 1690223708799,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "1FTrLnNtG6Cb",
    "outputId": "3bd6e98c-477e-406a-ed59-036bb4ed5a05"
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "3\n",
      "5\n"
     ]
    }
   ],
   "source": [
    "for elemento in ponto:\n",
    "    print(elemento)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 63,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 271,
     "status": "ok",
     "timestamp": 1690223710574,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "sifYrljKG6Cb",
    "outputId": "96b31794-4fb0-47f5-be43-64c9d4a62925"
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "0 3\n",
      "1 5\n"
     ]
    }
   ],
   "source": [
    "for index in range(len(ponto)):\n",
    "    print(index, ponto[index])"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 64,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 304,
     "status": "ok",
     "timestamp": 1690223712536,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "1fs-YeSRG6Cb",
    "outputId": "dbde7611-8fbf-4cd1-ad02-6afbaec5a538"
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "0 3\n",
      "1 5\n"
     ]
    }
   ],
   "source": [
    "index = 0\n",
    "while index < len(ponto):\n",
    "    print(index, ponto[index])\n",
    "    index +=1"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "D3UhRP3pG6Cc"
   },
   "source": [
    "**Nota desnecessária:** Diferentemente das listas, as tuplas são imutáveis, o que significa que seus elementos não podem ser alterados após a criação."
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "sKXrplBbG6Cc"
   },
   "source": [
    "### 4.3 Dicionários em Python:\n",
    "Dicionários são estruturas de dados que permitem armazenar elementos em um formato de chave-valor. Cada elemento (valor) é associado a uma chave exclusiva que permite acessá-lo de forma rápida.\n",
    "\n",
    "Dicionários são definidos utilizando chaves ({}) com pares chave-valor separados por dois pontos (:).\n",
    "As chaves devem ser únicas e imutáveis, geralmente strings ou números."
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "df76zOZMG6Cc"
   },
   "source": [
    "Exemplo de criação de um dicionário:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 65,
   "metadata": {
    "id": "w2QLwmZAG6Cc"
   },
   "outputs": [],
   "source": [
    "dicionario_idade_alunos = {\n",
    "    'João': 18,\n",
    "    'Maria': 20,\n",
    "    'Pedro': 19,\n",
    "    'Ana': 21\n",
    "}"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 66,
   "metadata": {
    "id": "0EAR7nTlG6Cc"
   },
   "outputs": [],
   "source": [
    "dicionario_idade_alunos = {}\n",
    "dicionario_idade_alunos['João'] = 18\n",
    "dicionario_idade_alunos['Maria'] = 20\n",
    "dicionario_idade_alunos['Pedro'] = 19\n",
    "dicionario_idade_alunos['Ana'] = 21"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "E6ioSRlLG6Cc"
   },
   "source": [
    "#### 4.3.1 Acesso e Manipulação de elementos em Dicionários:\n",
    "Para acessar elementos em um dicionário, utilizamos as chaves como índices.\n",
    "\n",
    "Exemplo de acesso a elementos:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 67,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 273,
     "status": "ok",
     "timestamp": 1690223718821,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "cpmqbo8XG6Cc",
    "outputId": "7915fc83-1c28-48ae-f999-aa4effbb79a9"
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "20\n",
      "19\n"
     ]
    }
   ],
   "source": [
    "print(dicionario_idade_alunos['Maria'])\n",
    "print(dicionario_idade_alunos['Pedro'])"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "AiERH2CsG6Cc"
   },
   "source": [
    "Para adicionar, atualizar ou remover elementos de um dicionário, basta atribuir um novo valor a uma chave ou utilizar o método del.\n",
    "\n",
    "Exemplo de manipulação de elementos:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 68,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 276,
     "status": "ok",
     "timestamp": 1690223720805,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "IkNNGXp8G6Cc",
    "outputId": "f81c67bb-30bd-4a9d-aab2-8d769545a3de"
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "{'João': 18, 'Maria': 20, 'Pedro': 19, 'Ana': 21, 'Mariana': 22}\n"
     ]
    }
   ],
   "source": [
    "# Adicionar um novo aluno\n",
    "dicionario_idade_alunos['Mariana'] = 22\n",
    "\n",
    "print(dicionario_idade_alunos)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 69,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 2,
     "status": "ok",
     "timestamp": 1690223722138,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "2GqlJSfXG6Cd",
    "outputId": "04c31111-817b-435a-95a6-878163b4f366"
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "{'João': 18, 'Maria': 20, 'Pedro': 20, 'Ana': 21, 'Mariana': 22}\n"
     ]
    }
   ],
   "source": [
    "# Atualizar a idade de um aluno\n",
    "dicionario_idade_alunos['Pedro'] = 20\n",
    "\n",
    "print(dicionario_idade_alunos)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 70,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 5,
     "status": "ok",
     "timestamp": 1690223723822,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "NBtTm6DoG6Cd",
    "outputId": "48bb457a-97ca-493f-b8f1-b7755944e561",
    "scrolled": true
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "{'João': 18, 'Maria': 20, 'Pedro': 20, 'Mariana': 22}\n"
     ]
    }
   ],
   "source": [
    "# Remover um aluno\n",
    "del dicionario_idade_alunos['Ana']\n",
    "\n",
    "print(dicionario_idade_alunos)"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "6AftbaaBG6Cd"
   },
   "source": [
    "Usando loops:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 71,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 316,
     "status": "ok",
     "timestamp": 1690223726178,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "rAQ9jGfxG6Cd",
    "outputId": "e991c617-6af8-4d38-e5f7-feeab24c6172",
    "scrolled": true
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "João\n",
      "Maria\n",
      "Pedro\n",
      "Mariana\n"
     ]
    }
   ],
   "source": [
    "# Acesso às chaves do dicionário usando um loop for\n",
    "for nome in dicionario_idade_alunos:\n",
    "    print(nome)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 72,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 271,
     "status": "ok",
     "timestamp": 1690223727942,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "BBeJkQABG6Cd",
    "outputId": "fa38bce3-b105-4eed-cfe7-02beb7663cad",
    "scrolled": true
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "18\n",
      "20\n",
      "20\n",
      "22\n"
     ]
    }
   ],
   "source": [
    "# Acesso aos valores do dicionário usando um loop for\n",
    "for idade in dicionario_idade_alunos.values():\n",
    "    print(idade)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 73,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 2,
     "status": "ok",
     "timestamp": 1690223729484,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "El4P4_Q2G6Cd",
    "outputId": "0e73493c-3a5c-4482-8edb-a5ee144544cb"
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Nome: João - Idade: 18\n",
      "Nome: Maria - Idade: 20\n",
      "Nome: Pedro - Idade: 20\n",
      "Nome: Mariana - Idade: 22\n"
     ]
    }
   ],
   "source": [
    "# Acesso às chaves e valores do dicionário usando um loop for\n",
    "for nome, idade in dicionario_idade_alunos.items():\n",
    "    print(\"Nome:\", nome, \"- Idade:\", idade)"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "7kw2DwIdG6Cd"
   },
   "source": [
    "### 4.4 - Exercícios:"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "6uUb2qFsG6Cd"
   },
   "source": [
    "#### Exercício 1:\n",
    "    a) Crie uma lista vazia chamada \"numeros\". Em seguida, adicione os números de 1 a 10 a essa lista utilizando um loop.\n",
    "    b) Dada a lista \"frutas\" abaixo, remova o último elemento da lista e adicione \"morango\" no seu lugar.\n",
    "    frutas = [\"maçã\", \"banana\", \"laranja\", \"abacaxi\"]\n",
    "    c) Dada a lista \"notas\" com as notas de um estudante, calcule a média aritmética das notas.\n",
    "    notas = [8.5, 7.2, 6.8, 9.0, 7.5]"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 74,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 3,
     "status": "ok",
     "timestamp": 1690223732243,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "NDZawx9BG6Ce",
    "outputId": "c9012efe-32ae-4497-b2ab-ea9308615efd"
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "[1, 2, 3, 4, 5, 6, 7, 8, 9, 10]\n"
     ]
    }
   ],
   "source": [
    "# a)\n",
    "numeros = []\n",
    "for i in range(1, 11):\n",
    "    numeros.append(i)\n",
    "\n",
    "print(numeros)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 75,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 2,
     "status": "ok",
     "timestamp": 1690223733682,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "dKnGeo58G6Ce",
    "outputId": "be4dda6a-2254-4066-8a0d-5777b3996c40"
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "['maçã', 'banana', 'laranja', 'morango']\n"
     ]
    }
   ],
   "source": [
    "# b)\n",
    "frutas = [\"maçã\", \"banana\", \"laranja\", \"abacaxi\"]\n",
    "frutas.pop()  # Remove o último elemento da lista\n",
    "frutas.append(\"morango\")  # Adiciona \"morango\" no lugar do último elemento removido\n",
    "\n",
    "print(frutas)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 76,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 259,
     "status": "ok",
     "timestamp": 1690223735777,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "INth-dgnG6Ce",
    "outputId": "d01fa480-fc80-4fac-b68f-f85dc2fd289c"
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Notas: [8.5, 7.2, 6.8, 9.0, 7.5]\n",
      "Média: 7.8\n"
     ]
    }
   ],
   "source": [
    "# c)\n",
    "notas = [8.5, 7.2, 6.8, 9.0, 7.5]\n",
    "media = sum(notas) / len(notas)\n",
    "\n",
    "print(\"Notas:\", notas)\n",
    "print(\"Média:\", media)\n"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "ygdd9rTYG6Ce"
   },
   "source": [
    "#### Exercício 2:\n",
    "    a) Crie uma lista com os números de 1 a 10. Acesse o primeiro e o último elemento da lista.\n",
    "    b) Dada a lista \"nomes\" abaixo, substitua o segundo elemento por \"Maria\".\n",
    "    nomes = [\"João\", \"Pedro\", \"Carlos\", \"Ana\"]"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 77,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 300,
     "status": "ok",
     "timestamp": 1690223737717,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "URgJKi7gG6Ce",
    "outputId": "b2194657-4254-4cff-ce5d-4fcaad92ecb1"
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Lista de números: [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]\n",
      "Primeiro elemento: 1\n",
      "Último elemento: 10\n"
     ]
    }
   ],
   "source": [
    "# a)\n",
    "numeros = list(range(1, 11))\n",
    "\n",
    "primeiro_elemento = numeros[0]\n",
    "ultimo_elemento = numeros[-1]\n",
    "\n",
    "print(\"Lista de números:\", numeros)\n",
    "print(\"Primeiro elemento:\", primeiro_elemento)\n",
    "print(\"Último elemento:\", ultimo_elemento)\n"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 78,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 270,
     "status": "ok",
     "timestamp": 1690223739242,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "E4P4fIGMG6Ce",
    "outputId": "09f2f970-be14-44c8-d076-36894e91a931"
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Lista de nomes: ['João', 'Maria', 'Carlos', 'Ana']\n"
     ]
    }
   ],
   "source": [
    "# b)\n",
    "nomes = [\"João\", \"Pedro\", \"Carlos\", \"Ana\"]\n",
    "nomes[1] = \"Maria\"  # Substitui o segundo elemento (índice 1) por \"Maria\"\n",
    "\n",
    "print(\"Lista de nomes:\", nomes)"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "uXOz705tG6Ce"
   },
   "source": [
    "#### Exercício 3:\n",
    "    a) Dada a tupla \"coordenadas\" abaixo, extraia os valores de latitude e longitude em variáveis separadas.\n",
    "    coordenadas = (40.7128, -74.0060)\n",
    "    b) Concatene as tuplas \"tupla1\" e \"tupla2\" abaixo em uma única tupla chamada \"tupla_concatenada\".\n",
    "    tupla1 = (1, 2, 3)\n",
    "    tupla2 = (4, 5, 6)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 79,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 276,
     "status": "ok",
     "timestamp": 1690223741318,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "VDtxDSiUG6Ce",
    "outputId": "b34613f4-d00d-4db2-faf7-7c84ed95a0b0",
    "scrolled": true
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Latitude: 40.7128\n",
      "Longitude: -74.006\n"
     ]
    }
   ],
   "source": [
    "# a)\n",
    "coordenadas = (40.7128, -74.0060)\n",
    "latitude, longitude = coordenadas\n",
    "\n",
    "print(\"Latitude:\", latitude)\n",
    "print(\"Longitude:\", longitude)\n"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 80,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 3,
     "status": "ok",
     "timestamp": 1690223743122,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "PsaE5kdUG6Cf",
    "outputId": "97a7fa80-ca29-4b0b-abd4-eed4442952eb"
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Tupla 1: (1, 2, 3)\n",
      "Tupla 2: (4, 5, 6)\n",
      "Tupla concatenada: (1, 2, 3, 4, 5, 6)\n"
     ]
    }
   ],
   "source": [
    "# b)\n",
    "tupla1 = (1, 2, 3)\n",
    "tupla2 = (4, 5, 6)\n",
    "tupla_concatenada = tupla1 + tupla2\n",
    "\n",
    "print(\"Tupla 1:\", tupla1)\n",
    "print(\"Tupla 2:\", tupla2)\n",
    "print(\"Tupla concatenada:\", tupla_concatenada)\n"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "id": "9H0_Tb9-G6Cf"
   },
   "source": [
    "#### Exercício 4:\n",
    "    a) Crie um dicionário vazio chamado \"contatos\". Adicione três contatos (nome e e-mail) ao dicionário.\n",
    "    b) Crie um dicionário chamado \"pessoa\" com as chaves \"nome\", \"idade\" e \"cidade\", preenchendo com seus respectivos valores.\n",
    "    c) Dado o dicionário \"pontuacoes\" abaixo, atualize a pontuação de \"Maria\" para 95.\n",
    "    pontuacoes = {\"João\": 85, \"Maria\": 90, \"Carlos\": 88}\n",
    "    d) Imprima todas as chaves do dicionário \"estoque_produtos\" abaixo.\n",
    "    estoque_produtos = {\"arroz\": 10, \"feijão\": 5, \"macarrão\": 8, \"óleo\": 15}"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 81,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 313,
     "status": "ok",
     "timestamp": 1690223745782,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "chaSKOOoG6Cf",
    "outputId": "1f4eb204-cc16-4764-fe98-d59d036f9d4d"
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Dicionário contatos: {'João': 'joao@email.com', 'Maria': 'maria@email.com', 'Pedro': 'pedro@email.com'}\n"
     ]
    }
   ],
   "source": [
    "# a)\n",
    "contatos = {}\n",
    "\n",
    "# Adicionando contatos ao dicionário\n",
    "contatos[\"João\"] = \"joao@email.com\"\n",
    "contatos[\"Maria\"] = \"maria@email.com\"\n",
    "contatos[\"Pedro\"] = \"pedro@email.com\"\n",
    "\n",
    "print(\"Dicionário contatos:\", contatos)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 82,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 2,
     "status": "ok",
     "timestamp": 1690223747122,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "r5ekkqhXG6Cf",
    "outputId": "2c8dafcf-3819-4a74-d726-e4f059e6aa69"
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Dicionário pessoa: {'nome': 'João', 'idade': 30, 'cidade': 'São Paulo'}\n"
     ]
    }
   ],
   "source": [
    "# b)\n",
    "pessoa = {\n",
    "    \"nome\": \"João\",\n",
    "    \"idade\": 30,\n",
    "    \"cidade\": \"São Paulo\"\n",
    "}\n",
    "\n",
    "print(\"Dicionário pessoa:\", pessoa)\n"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 83,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 255,
     "status": "ok",
     "timestamp": 1690223749620,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "fC7mhPvWG6Cf",
    "outputId": "09b1b85d-b2ff-4211-82f5-5d79171c18a5"
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Dicionário pontuações atualizado: {'João': 85, 'Maria': 95, 'Carlos': 88}\n"
     ]
    }
   ],
   "source": [
    "# c)\n",
    "pontuacoes = {\"João\": 85, \"Maria\": 90, \"Carlos\": 88}\n",
    "pontuacoes[\"Maria\"] = 95  # Atualiza a pontuação de \"Maria\" para 95\n",
    "\n",
    "print(\"Dicionário pontuações atualizado:\", pontuacoes)\n"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 84,
   "metadata": {
    "colab": {
     "base_uri": "https://localhost:8080/"
    },
    "executionInfo": {
     "elapsed": 3,
     "status": "ok",
     "timestamp": 1690223751086,
     "user": {
      "displayName": "Gallileu Genesis",
      "userId": "10784296989533502530"
     },
     "user_tz": 180
    },
    "id": "v3sYgbAaG6Cf",
    "outputId": "93d1653a-029c-4563-a368-2fe0a55c0ef2"
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Chaves do dicionário estoque_produtos: dict_keys(['arroz', 'feijão', 'macarrão', 'óleo'])\n"
     ]
    }
   ],
   "source": [
    "# d)\n",
    "estoque_produtos = {\"arroz\": 10, \"feijão\": 5, \"macarrão\": 8, \"óleo\": 15}\n",
    "chaves_estoque = estoque_produtos.keys()\n",
    "\n",
    "print(\"Chaves do dicionário estoque_produtos:\", chaves_estoque)\n"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {
    "id": "3djIwlbwG6Cf"
   },
   "outputs": [],
   "source": []
  }
 ],
 "metadata": {
  "colab": {
   "provenance": []
  },
  "kernelspec": {
   "display_name": "Python 3 (ipykernel)",
   "language": "python",
   "name": "python3"
  },
  "language_info": {
   "codemirror_mode": {
    "name": "ipython",
    "version": 3
   },
   "file_extension": ".py",
   "mimetype": "text/x-python",
   "name": "python",
   "nbconvert_exporter": "python",
   "pygments_lexer": "ipython3",
   "version": "3.9.12"
  }
 },
 "nbformat": 4,
 "nbformat_minor": 1
}
# Curso_basico_Python