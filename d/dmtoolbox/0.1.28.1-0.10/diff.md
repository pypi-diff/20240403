# Comparing `tmp/dmtoolbox-0.1.28.1.tar.gz` & `tmp/dmtoolbox-0.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmtoolbox-0.1.28.1.tar", last modified: Wed Apr  3 12:34:57 2024, max compression
+gzip compressed data, was "dmtoolbox-0.10.tar", last modified: Sun Mar  3 04:10:41 2024, max compression
```

## Comparing `dmtoolbox-0.1.28.1.tar` & `dmtoolbox-0.10.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 12:34:57.163596 dmtoolbox-0.1.28.1/
--rw-rw-rw-   0        0        0    35821 2024-03-03 02:55:05.000000 dmtoolbox-0.1.28.1/LICENSE
--rw-rw-rw-   0        0        0     8966 2024-04-03 12:34:57.158980 dmtoolbox-0.1.28.1/PKG-INFO
--rw-rw-rw-   0        0        0     7512 2024-04-03 11:34:49.000000 dmtoolbox-0.1.28.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 12:34:57.080415 dmtoolbox-0.1.28.1/dmtoolbox/
--rw-rw-rw-   0        0        0      501 2024-04-03 12:31:38.000000 dmtoolbox-0.1.28.1/dmtoolbox/__init__.py
--rw-rw-rw-   0        0        0     5553 2024-04-03 10:40:10.000000 dmtoolbox-0.1.28.1/dmtoolbox/fmfunc.py
--rw-rw-rw-   0        0        0     4135 2024-04-03 11:18:26.000000 dmtoolbox-0.1.28.1/dmtoolbox/genJsons.py
--rw-rw-rw-   0        0        0     3364 2024-03-15 23:13:44.000000 dmtoolbox-0.1.28.1/dmtoolbox/nginxDefaults.py
--rw-rw-rw-   0        0        0    40794 2024-03-21 13:07:34.000000 dmtoolbox-0.1.28.1/dmtoolbox/nginxUtils.py
--rw-rw-rw-   0        0        0    25322 2024-04-03 11:24:44.000000 dmtoolbox-0.1.28.1/dmtoolbox/numericFuncs.py
--rw-rw-rw-   0        0        0    10050 2024-03-15 23:13:27.000000 dmtoolbox-0.1.28.1/dmtoolbox/osFuncs.py
--rw-rw-rw-   0        0        0     8488 2024-03-15 23:17:09.000000 dmtoolbox-0.1.28.1/dmtoolbox/portTools.py
-drwxrwxrwx   0        0        0        0 2024-04-03 12:34:57.155439 dmtoolbox-0.1.28.1/dmtoolbox.egg-info/
--rw-rw-rw-   0        0        0     8966 2024-04-03 12:34:55.000000 dmtoolbox-0.1.28.1/dmtoolbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      375 2024-04-03 12:34:56.000000 dmtoolbox-0.1.28.1/dmtoolbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 12:34:55.000000 dmtoolbox-0.1.28.1/dmtoolbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      112 2024-04-03 12:34:55.000000 dmtoolbox-0.1.28.1/dmtoolbox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-03 12:34:55.000000 dmtoolbox-0.1.28.1/dmtoolbox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 12:34:57.166097 dmtoolbox-0.1.28.1/setup.cfg
--rw-rw-rw-   0        0        0     1757 2024-04-03 12:34:53.000000 dmtoolbox-0.1.28.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-03 04:10:41.626618 dmtoolbox-0.10/
+-rw-rw-rw-   0        0        0    35821 2024-03-03 02:55:05.000000 dmtoolbox-0.10/LICENSE
+-rw-rw-rw-   0        0        0     9882 2024-03-03 04:10:41.625619 dmtoolbox-0.10/PKG-INFO
+-rw-rw-rw-   0        0        0     8458 2024-03-03 04:07:08.000000 dmtoolbox-0.10/README.md
+drwxrwxrwx   0        0        0        0 2024-03-03 04:10:41.604619 dmtoolbox-0.10/dmtoolbox/
+-rw-rw-rw-   0        0        0      649 2024-03-03 02:53:09.000000 dmtoolbox-0.10/dmtoolbox/__init__.py
+-rw-rw-rw-   0        0        0     4383 2024-03-03 04:04:32.000000 dmtoolbox-0.10/dmtoolbox/appdataGen.py
+-rw-rw-rw-   0        0        0     1160 2024-03-03 02:51:58.000000 dmtoolbox-0.10/dmtoolbox/createExeOnC.py
+-rw-rw-rw-   0        0        0     1269 2024-03-03 02:52:20.000000 dmtoolbox-0.10/dmtoolbox/exeGenerator.py
+-rw-rw-rw-   0        0        0     3696 2024-02-17 04:11:20.000000 dmtoolbox-0.10/dmtoolbox/func.py
+-rw-rw-rw-   0        0        0     2626 2024-03-03 02:51:25.000000 dmtoolbox-0.10/dmtoolbox/genJsons.py
+-rw-rw-rw-   0        0        0     3364 2024-03-03 04:04:32.000000 dmtoolbox-0.10/dmtoolbox/nginxDefaults.py
+-rw-rw-rw-   0        0        0     7614 2024-03-03 04:04:32.000000 dmtoolbox-0.10/dmtoolbox/nginxUtils.py
+-rw-rw-rw-   0        0        0    13378 2024-03-03 04:04:32.000000 dmtoolbox-0.10/dmtoolbox/numericFuncs.py
+-rw-rw-rw-   0        0        0     4804 2024-03-03 02:44:42.000000 dmtoolbox-0.10/dmtoolbox/osFuncs.py
+-rw-rw-rw-   0        0        0     5264 2024-03-03 04:04:32.000000 dmtoolbox-0.10/dmtoolbox/portTools.py
+-rw-rw-rw-   0        0        0     1653 2024-03-03 04:04:32.000000 dmtoolbox-0.10/dmtoolbox/regedit.py
+drwxrwxrwx   0        0        0        0 2024-03-03 04:10:41.623616 dmtoolbox-0.10/dmtoolbox.egg-info/
+-rw-rw-rw-   0        0        0     9882 2024-03-03 04:10:41.000000 dmtoolbox-0.10/dmtoolbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      470 2024-03-03 04:10:41.000000 dmtoolbox-0.10/dmtoolbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-03 04:10:41.000000 dmtoolbox-0.10/dmtoolbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      101 2024-03-03 04:10:41.000000 dmtoolbox-0.10/dmtoolbox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-03-03 04:10:41.000000 dmtoolbox-0.10/dmtoolbox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-03-03 04:10:41.626618 dmtoolbox-0.10/setup.cfg
+-rw-rw-rw-   0        0        0     1721 2024-03-03 04:10:37.000000 dmtoolbox-0.10/setup.py
```

### Comparing `dmtoolbox-0.1.28.1/LICENSE` & `dmtoolbox-0.10/LICENSE`

 * *Files identical despite different names*

### Comparing `dmtoolbox-0.1.28.1/PKG-INFO` & `dmtoolbox-0.10/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,56 +1,31 @@
-Metadata-Version: 2.1
-Name: dmtoolbox
-Version: 0.1.28.1
-Summary: dmtoolbox é uma coleção abrangente de ferramentas Python projetadas para facilitar a automação de tarefas e operações no ambiente Windows, manipulação avançada de arquivos e diretórios, criação e gestão de executáveis, manipulação de dados JSON, gerenciamento de configurações NGINX, análise numérica, e muito mais.
-Home-page: https://github.com/DanielMelloo/dmtoolbox
-Author: Daniel Mello
-Author-email: danielmello.dev@gmail.com
-License: GPLv3
-Keywords: utils automation numpy pandas matplotlib
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: pandas>=2.2.1
-Requires-Dist: numpy>=1.26.4
-Requires-Dist: prettytable>=3.10.0
-Requires-Dist: matplotlib>=3.8.3
-Requires-Dist: colorama>=0.4.6
-Requires-Dist: openpyxl>=3.1.2
-Requires-Dist: jinja2>=3.1.3
 
 ![GitHub repo size](https://img.shields.io/github/repo-size/DanielMelloo/dmtoolbox?style=for-the-badge)
 ![GitHub forks](https://img.shields.io/github/forks/DanielMelloo/dmtoolbox?style=for-the-badge)
-![Bitbucket open issues ](https://img.shields.io/bitbucket/issues/DanielMelloo/dmtoolbox?style=for-the-badge)
-![Bitbucket open pull requests ](https://img.shields.io/bitbucket/pr/DanielMelloo/dmtoolbox?style=for-the-badge)  
+![Bitbucket open issues](https://img.shields.io/bitbucket/issues-raw/DanielMelloo/dmtoolbox?style=for-the-badge)
+![Bitbucket open pull requests](https://img.shields.io/bitbucket/pr-raw/DanielMelloo/dmtoolbox?style=for-the-badge)
 
 
 # dmtoolbox
 
 
 - [dmtoolbox](#dmtoolbox)
   - [Descrição](#descrição)
   - [Funcionalidades](#funcionalidades)
   - [Funcionalidades dos Módulos](#funcionalidades-dos-módulos)
-    - [fmfunc.py](#fmfuncpy)
+    - [appdataGen.py](#appdatagenpy)
+    - [createExeOnC.py](#createexeoncpy)
+    - [exeGenerator.py](#exegeneratorpy)
+    - [func.py](#funcpy)
     - [genJsons.py](#genjsonspy)
-    - [nginxDefaults.py  e nginxUtils.py](#nginxdefaultspy--e-nginxutilspy)
+    - [nginxDefaults.py  e .pynginxDefaults.py](#nginxdefaultspy--e-pynginxdefaultspy)
     - [numericFuncs.py](#numericfuncspy)
     - [osFuncs.py](#osfuncspy)
     - [portTools.py](#porttoolspy)
+    - [regedit.py](#regeditpy)
   - [Instalação do Pacote dmtoolbox](#instalação-do-pacote-dmtoolbox)
     - [Pré-Requisitos](#pré-requisitos)
     - [Passo 1: Criação de um Ambiente Virtual (Opcional, mas Recomendado)](#passo-1-criação-de-um-ambiente-virtual-opcional-mas-recomendado)
     - [Passo 2: Instalação do Pacote dmtoolbox](#passo-2-instalação-do-pacote-dmtoolbox)
     - [Solução Alternativa: Instalação Manual das Dependências e Clonagem do Repositório](#solução-alternativa-instalação-manual-das-dependências-e-clonagem-do-repositório)
   - [Exemplos de Uso](#exemplos-de-uso)
   - [Contribuições](#contribuições)
@@ -61,45 +36,59 @@
 
 ## Descrição
 Este pacote Python é uma coleção abrangente de ferramentas projetadas para facilitar a automação de tarefas e operações no ambiente Windows, manipulação avançada de arquivos e diretórios, criação e gestão de executáveis, manipulação de dados JSON, gerenciamento de configurações NGINX, análise numérica, e muito mais.
 
 
 ## Funcionalidades
 - **Gerenciamento de Arquivos e Diretórios**: Criação e manipulação de estruturas de arquivos no AppData e outras localizações, com suporte para operações que requerem privilégios elevados.
-
+- **Criação de Executáveis**: Utilitários para transformar scripts Python em executáveis independentes, facilitando a distribuição e execução.
 - **Manipulação de JSON**: Ferramentas para converter dados para e de JSON, e atualizar scripts com novas declarações de variáveis baseadas em conteúdo JSON.
 - **Gerenciamento do NGINX**: Funcionalidades para configurar, iniciar, parar e reiniciar o servidor NGINX, além de verificar e ajustar configurações de acordo com as necessidades do usuário.
 - **Análise Numérica e Visualização**: Funções para manipulação matemática avançada, incluindo operações com matrizes, geração de tabelas formatadas, e plotagem de gráficos 2D e 3D.
 - **Interação com o Sistema Operacional**: Utilitários para verificar privilégios de administrador, manipular registros do Windows, e mais.
 - **Gerenciamento de Portas**: Ferramentas para verificar a disponibilidade de portas e configurar portas para aplicações.
 
 
 
 ## Funcionalidades dos Módulos
 Cada módulo traz um conjunto de funcionalidades específicas, detalhadas a seguir:
 
 
-### [fmfunc.py](https://github.com/DanielMelloo/dmtoolbox/blob/main/dmtoolbox/fmfunc.py)
+
+### [appdataGen.py](https://github.com/DanielMelloo/dmtoolbox/blob/main/dmtoolbox/appdataGen.py)
+- Gerencia arquivos e diretórios no AppData LocalLow, permitindo a criação personalizada de estruturas de diretórios e arquivos de configuração.
+
+### [createExeOnC.py](https://github.com/DanielMelloo/dmtoolbox/blob/main/dmtoolbox/createExeOnC.py)
+
+- Facilita a criação de cópias da aplicação no disco local C, útil para a distribuição de software ou instalação local rápida.
+
+### exeGenerator.py
+- Utiliza o PyInstaller para converter scripts Python em executáveis autônomos, simplificando a distribuição de aplicações.
+
+### [func.py](https://github.com/DanielMelloo/dmtoolbox/blob/main/dmtoolbox/func.py)
 - Oferece um conjunto diversificado de funções utilitárias para operações comuns, como manipulação de datas, tamanhos de arquivos, e caminhos de diretórios.
 
 ### [genJsons.py](https://github.com/DanielMelloo/dmtoolbox/blob/main/dmtoolbox/genJsons.py)
 - Permite a conversão eficiente de dados para o formato JSON e vice-versa, além da atualização dinâmica de scripts com novos dados JSON.
 
-### [nginxDefaults.py](https://github.com/DanielMelloo/dmtoolbox/blob/main/dmtoolbox/nginxDefaults.py)  e [nginxUtils.py](https://github.com/DanielMelloo/dmtoolbox/blob/main/dmtoolbox/nnginxUtils.py) 
+### [nginxDefaults.py](https://github.com/DanielMelloo/dmtoolbox/blob/main/dmtoolbox/nginxDefaults.py)  e .py[nginxDefaults.py](https://github.com/DanielMelloo/dmtoolbox/blob/main/dmtoolbox/nginxDefaults.py) 
 - Proporcionam ferramentas para o gerenciamento detalhado de configurações do servidor NGINX, incluindo inicialização, parada, e verificação de status.
 
 ### [numericFuncs.py](https://github.com/DanielMelloo/dmtoolbox/blob/main/dmtoolbox/numericFuncs.py)
 - Inclui funções para análises numéricas avançadas, manipulação de matrizes, e visualização de dados em 2D e 3D.
 
 ### [osFuncs.py](https://github.com/DanielMelloo/dmtoolbox/blob/main/dmtoolbox/osFuncs.py)
 - Contém utilitários para interações avançadas com o sistema operacional, como verificação de privilégios de administrador e manipulação de arquivos e diretórios.
 
 ### [portTools.py](https://github.com/DanielMelloo/dmtoolbox/blob/main/dmtoolbox/portTools.py)
 - Fornece métodos para verificar a disponibilidade de portas TCP/IP e selecionar portas disponíveis para aplicações.
 
+### [regedit.py](https://github.com/DanielMelloo/dmtoolbox/blob/main/dmtoolbox/regedit.py)
+- Permite a criação e gerenciamento de entradas de registro do Windows, facilitando a integração com o sistema operacional.
+
 
 
 ## Instalação do Pacote dmtoolbox
 
 Para instalar o pacote dmtoolbox de maneira eficiente e segura, siga os passos abaixo. Recomendamos a utilização de um ambiente virtual Python para evitar conflitos de dependências com outros pacotes instalados no sistema.
 
 ### Pré-Requisitos
@@ -143,20 +132,18 @@
 ```bash
 pip install -r requirements.txt
 ```
 
 Em seguida, clone o repositório do GitHub ou baixe os arquivos do projeto diretamente para o seu ambiente de trabalho.
 
 
-## Exemplos de Uso
 
-Para ajudá-lo a começar, fornecemos uma série de exemplos práticos no diretório [`Exemplos de Código`](https://github.com/DanielMelloo/dmtoolbox/tree/main/Exemplos%20de%20Código). Aqui você encontrará amostras de código demonstrando como utilizar as funcionalidades disponíveis no dmtoolbox.
-
-Para acessar os exemplos, navegue até a pasta [`Exemplos de Código`](https://github.com/DanielMelloo/dmtoolbox/tree/main/Exemplos%20de%20Código) no repositório do projeto ou clique no link.
 
+## Exemplos de Uso
+Para cada módulo, exemplos detalhados de uso são fornecidos na documentação interna. Estes exemplos abrangem desde a criação de diretórios no AppData até a configuração avançada do NGINX e análise numérica com visualização de dados.
 
 ## Contribuições
 Encorajamos contribuições! Se deseja sugerir melhorias, corrigir bugs ou adicionar novas funcionalidades, por favor, abra uma issue ou submeta um pull request.
 
 
 ## Autor
 
@@ -165,8 +152,8 @@
 - GitHub: [github.com/DanielMelloo](https://github.com/DanielMelloo)
 
 
 ## Licença
 Este projeto é licenciado sob a GNU General Public License v3.0 - veja o arquivo [LICENSE](LICENSE) para mais detalhes.
 
 
-[⬆ Voltar ao topo](#dmtoolbox)
+[⬆ Voltar ao topo](#dmtoolbox)
```

### Comparing `dmtoolbox-0.1.28.1/README.md` & `dmtoolbox-0.10/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,60 @@
+Metadata-Version: 2.1
+Name: dmtoolbox
+Version: 0.10
+Summary: dmtoolbox é uma coleção abrangente de ferramentas Python projetadas para facilitar a automação de tarefas e operações no ambiente Windows, manipulação avançada de arquivos e diretórios, criação e gestão de executáveis, manipulação de dados JSON, gerenciamento de configurações NGINX, análise numérica, e muito mais.
+Home-page: https://github.com/danielmello/dmtoolbox
+Author: Daniel Mello
+Author-email: danielmello.dev@example.com
+License: GPLv3
+Keywords: utils automation numpy pandas matplotlib
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pandas==2.2.1
+Requires-Dist: numpy==1.26.4
+Requires-Dist: prettytable==3.10.0
+Requires-Dist: matplotlib==3.8.3
+Requires-Dist: colorama==0.4.6
+Requires-Dist: pyinstaller==6.4.0
+
+
 ![GitHub repo size](https://img.shields.io/github/repo-size/DanielMelloo/dmtoolbox?style=for-the-badge)
 ![GitHub forks](https://img.shields.io/github/forks/DanielMelloo/dmtoolbox?style=for-the-badge)
-![Bitbucket open issues ](https://img.shields.io/bitbucket/issues/DanielMelloo/dmtoolbox?style=for-the-badge)
-![Bitbucket open pull requests ](https://img.shields.io/bitbucket/pr/DanielMelloo/dmtoolbox?style=for-the-badge)  
+![Bitbucket open issues](https://img.shields.io/bitbucket/issues-raw/DanielMelloo/dmtoolbox?style=for-the-badge)
+![Bitbucket open pull requests](https://img.shields.io/bitbucket/pr-raw/DanielMelloo/dmtoolbox?style=for-the-badge)
 
 
 # dmtoolbox
 
 
 - [dmtoolbox](#dmtoolbox)
   - [Descrição](#descrição)
   - [Funcionalidades](#funcionalidades)
   - [Funcionalidades dos Módulos](#funcionalidades-dos-módulos)
-    - [fmfunc.py](#fmfuncpy)
+    - [appdataGen.py](#appdatagenpy)
+    - [createExeOnC.py](#createexeoncpy)
+    - [exeGenerator.py](#exegeneratorpy)
+    - [func.py](#funcpy)
     - [genJsons.py](#genjsonspy)
-    - [nginxDefaults.py  e nginxUtils.py](#nginxdefaultspy--e-nginxutilspy)
+    - [nginxDefaults.py  e .pynginxDefaults.py](#nginxdefaultspy--e-pynginxdefaultspy)
     - [numericFuncs.py](#numericfuncspy)
     - [osFuncs.py](#osfuncspy)
     - [portTools.py](#porttoolspy)
+    - [regedit.py](#regeditpy)
   - [Instalação do Pacote dmtoolbox](#instalação-do-pacote-dmtoolbox)
     - [Pré-Requisitos](#pré-requisitos)
     - [Passo 1: Criação de um Ambiente Virtual (Opcional, mas Recomendado)](#passo-1-criação-de-um-ambiente-virtual-opcional-mas-recomendado)
     - [Passo 2: Instalação do Pacote dmtoolbox](#passo-2-instalação-do-pacote-dmtoolbox)
     - [Solução Alternativa: Instalação Manual das Dependências e Clonagem do Repositório](#solução-alternativa-instalação-manual-das-dependências-e-clonagem-do-repositório)
   - [Exemplos de Uso](#exemplos-de-uso)
   - [Contribuições](#contribuições)
@@ -31,45 +65,59 @@
 
 ## Descrição
 Este pacote Python é uma coleção abrangente de ferramentas projetadas para facilitar a automação de tarefas e operações no ambiente Windows, manipulação avançada de arquivos e diretórios, criação e gestão de executáveis, manipulação de dados JSON, gerenciamento de configurações NGINX, análise numérica, e muito mais.
 
 
 ## Funcionalidades
 - **Gerenciamento de Arquivos e Diretórios**: Criação e manipulação de estruturas de arquivos no AppData e outras localizações, com suporte para operações que requerem privilégios elevados.
-
+- **Criação de Executáveis**: Utilitários para transformar scripts Python em executáveis independentes, facilitando a distribuição e execução.
 - **Manipulação de JSON**: Ferramentas para converter dados para e de JSON, e atualizar scripts com novas declarações de variáveis baseadas em conteúdo JSON.
 - **Gerenciamento do NGINX**: Funcionalidades para configurar, iniciar, parar e reiniciar o servidor NGINX, além de verificar e ajustar configurações de acordo com as necessidades do usuário.
 - **Análise Numérica e Visualização**: Funções para manipulação matemática avançada, incluindo operações com matrizes, geração de tabelas formatadas, e plotagem de gráficos 2D e 3D.
 - **Interação com o Sistema Operacional**: Utilitários para verificar privilégios de administrador, manipular registros do Windows, e mais.
 - **Gerenciamento de Portas**: Ferramentas para verificar a disponibilidade de portas e configurar portas para aplicações.
 
 
 
 ## Funcionalidades dos Módulos
 Cada módulo traz um conjunto de funcionalidades específicas, detalhadas a seguir:
 
 
-### [fmfunc.py](https://github.com/DanielMelloo/dmtoolbox/blob/main/dmtoolbox/fmfunc.py)
+
+### [appdataGen.py](https://github.com/DanielMelloo/dmtoolbox/blob/main/dmtoolbox/appdataGen.py)
+- Gerencia arquivos e diretórios no AppData LocalLow, permitindo a criação personalizada de estruturas de diretórios e arquivos de configuração.
+
+### [createExeOnC.py](https://github.com/DanielMelloo/dmtoolbox/blob/main/dmtoolbox/createExeOnC.py)
+
+- Facilita a criação de cópias da aplicação no disco local C, útil para a distribuição de software ou instalação local rápida.
+
+### exeGenerator.py
+- Utiliza o PyInstaller para converter scripts Python em executáveis autônomos, simplificando a distribuição de aplicações.
+
+### [func.py](https://github.com/DanielMelloo/dmtoolbox/blob/main/dmtoolbox/func.py)
 - Oferece um conjunto diversificado de funções utilitárias para operações comuns, como manipulação de datas, tamanhos de arquivos, e caminhos de diretórios.
 
 ### [genJsons.py](https://github.com/DanielMelloo/dmtoolbox/blob/main/dmtoolbox/genJsons.py)
 - Permite a conversão eficiente de dados para o formato JSON e vice-versa, além da atualização dinâmica de scripts com novos dados JSON.
 
-### [nginxDefaults.py](https://github.com/DanielMelloo/dmtoolbox/blob/main/dmtoolbox/nginxDefaults.py)  e [nginxUtils.py](https://github.com/DanielMelloo/dmtoolbox/blob/main/dmtoolbox/nnginxUtils.py) 
+### [nginxDefaults.py](https://github.com/DanielMelloo/dmtoolbox/blob/main/dmtoolbox/nginxDefaults.py)  e .py[nginxDefaults.py](https://github.com/DanielMelloo/dmtoolbox/blob/main/dmtoolbox/nginxDefaults.py) 
 - Proporcionam ferramentas para o gerenciamento detalhado de configurações do servidor NGINX, incluindo inicialização, parada, e verificação de status.
 
 ### [numericFuncs.py](https://github.com/DanielMelloo/dmtoolbox/blob/main/dmtoolbox/numericFuncs.py)
 - Inclui funções para análises numéricas avançadas, manipulação de matrizes, e visualização de dados em 2D e 3D.
 
 ### [osFuncs.py](https://github.com/DanielMelloo/dmtoolbox/blob/main/dmtoolbox/osFuncs.py)
 - Contém utilitários para interações avançadas com o sistema operacional, como verificação de privilégios de administrador e manipulação de arquivos e diretórios.
 
 ### [portTools.py](https://github.com/DanielMelloo/dmtoolbox/blob/main/dmtoolbox/portTools.py)
 - Fornece métodos para verificar a disponibilidade de portas TCP/IP e selecionar portas disponíveis para aplicações.
 
+### [regedit.py](https://github.com/DanielMelloo/dmtoolbox/blob/main/dmtoolbox/regedit.py)
+- Permite a criação e gerenciamento de entradas de registro do Windows, facilitando a integração com o sistema operacional.
+
 
 
 ## Instalação do Pacote dmtoolbox
 
 Para instalar o pacote dmtoolbox de maneira eficiente e segura, siga os passos abaixo. Recomendamos a utilização de um ambiente virtual Python para evitar conflitos de dependências com outros pacotes instalados no sistema.
 
 ### Pré-Requisitos
@@ -113,20 +161,18 @@
 ```bash
 pip install -r requirements.txt
 ```
 
 Em seguida, clone o repositório do GitHub ou baixe os arquivos do projeto diretamente para o seu ambiente de trabalho.
 
 
-## Exemplos de Uso
-
-Para ajudá-lo a começar, fornecemos uma série de exemplos práticos no diretório [`Exemplos de Código`](https://github.com/DanielMelloo/dmtoolbox/tree/main/Exemplos%20de%20Código). Aqui você encontrará amostras de código demonstrando como utilizar as funcionalidades disponíveis no dmtoolbox.
 
-Para acessar os exemplos, navegue até a pasta [`Exemplos de Código`](https://github.com/DanielMelloo/dmtoolbox/tree/main/Exemplos%20de%20Código) no repositório do projeto ou clique no link.
 
+## Exemplos de Uso
+Para cada módulo, exemplos detalhados de uso são fornecidos na documentação interna. Estes exemplos abrangem desde a criação de diretórios no AppData até a configuração avançada do NGINX e análise numérica com visualização de dados.
 
 ## Contribuições
 Encorajamos contribuições! Se deseja sugerir melhorias, corrigir bugs ou adicionar novas funcionalidades, por favor, abra uma issue ou submeta um pull request.
 
 
 ## Autor
 
@@ -135,8 +181,8 @@
 - GitHub: [github.com/DanielMelloo](https://github.com/DanielMelloo)
 
 
 ## Licença
 Este projeto é licenciado sob a GNU General Public License v3.0 - veja o arquivo [LICENSE](LICENSE) para mais detalhes.
 
 
-[⬆ Voltar ao topo](#dmtoolbox)
+[⬆ Voltar ao topo](#dmtoolbox)
```

### Comparing `dmtoolbox-0.1.28.1/dmtoolbox/fmfunc.py` & `dmtoolbox-0.10/dmtoolbox/func.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,46 +13,27 @@
            'format_date',
            ]
 
 
 def get_folder_size(folder_path):
     """
     Retorna o tamanho total de uma pasta em bytes.
-
-    Parâmetros:
-    -----------
-    - folder_path: str
-        - O caminho da pasta cujo tamanho será calculado.
-
-    Retorno:
-    --------
-    - int
-        - O tamanho total da pasta em bytes.
     """
-
     total_size = 0
     
     # Itera sobre todos os arquivos e subpastas na pasta
     for dirpath, dirnames, filenames in os.walk(folder_path):
         # Calcula o tamanho de todos os arquivos na pasta atual
         for filename in filenames:
             file_path = os.path.join(dirpath, filename)
             total_size += os.path.getsize(file_path)
     
     return total_size
 
 def find_default_paths():
-    """
-    Encontra os caminhos padrão de pastas comuns, como Área de Trabalho, Downloads, Documentos, etc.
-
-    Retorno:
-    --------
-    - dict
-        - Um dicionário contendo os nomes das pastas e seus caminhos correspondentes.
-    """
     # Caminhos padrão para tentar
     default_paths = OrderedDict([
         ('Área de Trabalho', ['Desktop', 'Área de Trabalho']),
         ('Downloads', 'Downloads'),
         ('Documentos', 'Documents'),
         ('Imagens', 'Pictures'),
         ('Músicas', 'Music'),
@@ -82,120 +63,50 @@
                     found_paths[name] = path
                     break
                 
     found_paths['Este Computador'] = 'This PC'  # Tratado de forma especial na interface do usuário
     return found_paths
 
 def find_script_dir():
-    """
-    Encontra o diretório do script atual.
-
-    Nota:
-    -----
-    Esta função define uma variável global `GLOBAL_SCRIPT_DIR` que armazena o diretório do script atual.
-    """
     global GLOBAL_SCRIPT_DIR
     
     script_dir = os.path.dirname(os.path.realpath(__file__))
 
     if os.path.exists(script_dir):
         GLOBAL_SCRIPT_DIR = script_dir
     else:
         print(f"Erro: Diretório '{script_dir}' não encontrado")
 
 def find_style_sheet_path(file_name):
-    """
-    Encontra o caminho para o arquivo de folha de estilo.
-
-    Parâmetros:
-    -----------
-    - file_name: str
-        - O nome do arquivo de folha de estilo.
-
-    Nota:
-    -----
-    Esta função define uma variável global `GLOBAL_STYLE_PATH` que armazena o caminho para o arquivo de folha de estilo.
-    """
     global GLOBAL_STYLE_PATH
     global GLOBAL_SCRIPT_DIR
 
     style_path = os.path.join(GLOBAL_SCRIPT_DIR, file_name)
 
     if os.path.exists(style_path):
         GLOBAL_STYLE_PATH = style_path
     else:
         print(f"Erro: Arquivo '{file_name}' não encontrado no diretório '{GLOBAL_SCRIPT_DIR}'.")
 
 def get_file_size(file_path):
     """
     Retorna o tamanho de um arquivo em bytes.
-
-    Parâmetros:
-    -----------
-    - file_path: str
-        - O caminho do arquivo.
-
-    Retorno:
-    --------
-    - int
-        - O tamanho do arquivo em bytes.
     """
     return os.path.getsize(file_path)
 
 def get_modification_date(file_path):
     """
     Retorna a data de modificação de um arquivo ou pasta.
-
-    Parâmetros:
-    -----------
-    - file_path: str
-        - O caminho do arquivo ou pasta.
-
-    Retorno:
-    --------
-    - str
-        - A data de modificação no formato ISO.
     """
     timestamp = os.path.getmtime(file_path)
     return datetime.fromtimestamp(timestamp).isoformat()
 
 def format_size(size):
-    """
-    Formata um tamanho em bytes para uma string legível.
-
-    Parâmetros:
-    -----------
-    - size: int
-        - O tamanho em bytes.
-
-    Retorno:
-    --------
-    - str
-        - O tamanho formatado como uma string legível.
-    """
-
     for unit in ['B', 'KB', 'MB', 'GB', 'TB']:
         if size < 1024:
             return f"{size:.2f} {unit}"
         size /= 1024
     return f"{size:.2f} PB"
 
 def format_date(timestamp):
-    """
-    Formata um tamanho em bytes para uma string legível.
-
-    Parâmetros:
-    -----------
-    - size: int
-        - O tamanho em bytes.
-
-    Retorno:
-    --------
-    - str
-        - O tamanho formatado como uma string legível.
-    """
-
+    """Formata a data de modificação em um formato legível."""
     return datetime.fromtimestamp(timestamp).strftime('%Y-%m-%d %H:%M:%S')
-
-
-if __name__ == '__main__':
-    pass
```

### Comparing `dmtoolbox-0.1.28.1/dmtoolbox/nginxDefaults.py` & `dmtoolbox-0.10/dmtoolbox/nginxDefaults.py`

 * *Files identical despite different names*

### Comparing `dmtoolbox-0.1.28.1/dmtoolbox.egg-info/PKG-INFO` & `dmtoolbox-0.10/dmtoolbox.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: dmtoolbox
-Version: 0.1.28.1
+Version: 0.10
 Summary: dmtoolbox é uma coleção abrangente de ferramentas Python projetadas para facilitar a automação de tarefas e operações no ambiente Windows, manipulação avançada de arquivos e diretórios, criação e gestão de executáveis, manipulação de dados JSON, gerenciamento de configurações NGINX, análise numérica, e muito mais.
-Home-page: https://github.com/DanielMelloo/dmtoolbox
+Home-page: https://github.com/danielmello/dmtoolbox
 Author: Daniel Mello
-Author-email: danielmello.dev@gmail.com
+Author-email: danielmello.dev@example.com
 License: GPLv3
 Keywords: utils automation numpy pandas matplotlib
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -16,41 +16,45 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pandas>=2.2.1
-Requires-Dist: numpy>=1.26.4
-Requires-Dist: prettytable>=3.10.0
-Requires-Dist: matplotlib>=3.8.3
-Requires-Dist: colorama>=0.4.6
-Requires-Dist: openpyxl>=3.1.2
-Requires-Dist: jinja2>=3.1.3
+Requires-Dist: pandas==2.2.1
+Requires-Dist: numpy==1.26.4
+Requires-Dist: prettytable==3.10.0
+Requires-Dist: matplotlib==3.8.3
+Requires-Dist: colorama==0.4.6
+Requires-Dist: pyinstaller==6.4.0
+
 
 ![GitHub repo size](https://img.shields.io/github/repo-size/DanielMelloo/dmtoolbox?style=for-the-badge)
 ![GitHub forks](https://img.shields.io/github/forks/DanielMelloo/dmtoolbox?style=for-the-badge)
-![Bitbucket open issues ](https://img.shields.io/bitbucket/issues/DanielMelloo/dmtoolbox?style=for-the-badge)
-![Bitbucket open pull requests ](https://img.shields.io/bitbucket/pr/DanielMelloo/dmtoolbox?style=for-the-badge)  
+![Bitbucket open issues](https://img.shields.io/bitbucket/issues-raw/DanielMelloo/dmtoolbox?style=for-the-badge)
+![Bitbucket open pull requests](https://img.shields.io/bitbucket/pr-raw/DanielMelloo/dmtoolbox?style=for-the-badge)
 
 
 # dmtoolbox
 
 
 - [dmtoolbox](#dmtoolbox)
   - [Descrição](#descrição)
   - [Funcionalidades](#funcionalidades)
   - [Funcionalidades dos Módulos](#funcionalidades-dos-módulos)
-    - [fmfunc.py](#fmfuncpy)
+    - [appdataGen.py](#appdatagenpy)
+    - [createExeOnC.py](#createexeoncpy)
+    - [exeGenerator.py](#exegeneratorpy)
+    - [func.py](#funcpy)
     - [genJsons.py](#genjsonspy)
-    - [nginxDefaults.py  e nginxUtils.py](#nginxdefaultspy--e-nginxutilspy)
+    - [nginxDefaults.py  e .pynginxDefaults.py](#nginxdefaultspy--e-pynginxdefaultspy)
     - [numericFuncs.py](#numericfuncspy)
     - [osFuncs.py](#osfuncspy)
     - [portTools.py](#porttoolspy)
+    - [regedit.py](#regeditpy)
   - [Instalação do Pacote dmtoolbox](#instalação-do-pacote-dmtoolbox)
     - [Pré-Requisitos](#pré-requisitos)
     - [Passo 1: Criação de um Ambiente Virtual (Opcional, mas Recomendado)](#passo-1-criação-de-um-ambiente-virtual-opcional-mas-recomendado)
     - [Passo 2: Instalação do Pacote dmtoolbox](#passo-2-instalação-do-pacote-dmtoolbox)
     - [Solução Alternativa: Instalação Manual das Dependências e Clonagem do Repositório](#solução-alternativa-instalação-manual-das-dependências-e-clonagem-do-repositório)
   - [Exemplos de Uso](#exemplos-de-uso)
   - [Contribuições](#contribuições)
@@ -61,45 +65,59 @@
 
 ## Descrição
 Este pacote Python é uma coleção abrangente de ferramentas projetadas para facilitar a automação de tarefas e operações no ambiente Windows, manipulação avançada de arquivos e diretórios, criação e gestão de executáveis, manipulação de dados JSON, gerenciamento de configurações NGINX, análise numérica, e muito mais.
 
 
 ## Funcionalidades
 - **Gerenciamento de Arquivos e Diretórios**: Criação e manipulação de estruturas de arquivos no AppData e outras localizações, com suporte para operações que requerem privilégios elevados.
-
+- **Criação de Executáveis**: Utilitários para transformar scripts Python em executáveis independentes, facilitando a distribuição e execução.
 - **Manipulação de JSON**: Ferramentas para converter dados para e de JSON, e atualizar scripts com novas declarações de variáveis baseadas em conteúdo JSON.
 - **Gerenciamento do NGINX**: Funcionalidades para configurar, iniciar, parar e reiniciar o servidor NGINX, além de verificar e ajustar configurações de acordo com as necessidades do usuário.
 - **Análise Numérica e Visualização**: Funções para manipulação matemática avançada, incluindo operações com matrizes, geração de tabelas formatadas, e plotagem de gráficos 2D e 3D.
 - **Interação com o Sistema Operacional**: Utilitários para verificar privilégios de administrador, manipular registros do Windows, e mais.
 - **Gerenciamento de Portas**: Ferramentas para verificar a disponibilidade de portas e configurar portas para aplicações.
 
 
 
 ## Funcionalidades dos Módulos
 Cada módulo traz um conjunto de funcionalidades específicas, detalhadas a seguir:
 
 
-### [fmfunc.py](https://github.com/DanielMelloo/dmtoolbox/blob/main/dmtoolbox/fmfunc.py)
+
+### [appdataGen.py](https://github.com/DanielMelloo/dmtoolbox/blob/main/dmtoolbox/appdataGen.py)
+- Gerencia arquivos e diretórios no AppData LocalLow, permitindo a criação personalizada de estruturas de diretórios e arquivos de configuração.
+
+### [createExeOnC.py](https://github.com/DanielMelloo/dmtoolbox/blob/main/dmtoolbox/createExeOnC.py)
+
+- Facilita a criação de cópias da aplicação no disco local C, útil para a distribuição de software ou instalação local rápida.
+
+### exeGenerator.py
+- Utiliza o PyInstaller para converter scripts Python em executáveis autônomos, simplificando a distribuição de aplicações.
+
+### [func.py](https://github.com/DanielMelloo/dmtoolbox/blob/main/dmtoolbox/func.py)
 - Oferece um conjunto diversificado de funções utilitárias para operações comuns, como manipulação de datas, tamanhos de arquivos, e caminhos de diretórios.
 
 ### [genJsons.py](https://github.com/DanielMelloo/dmtoolbox/blob/main/dmtoolbox/genJsons.py)
 - Permite a conversão eficiente de dados para o formato JSON e vice-versa, além da atualização dinâmica de scripts com novos dados JSON.
 
-### [nginxDefaults.py](https://github.com/DanielMelloo/dmtoolbox/blob/main/dmtoolbox/nginxDefaults.py)  e [nginxUtils.py](https://github.com/DanielMelloo/dmtoolbox/blob/main/dmtoolbox/nnginxUtils.py) 
+### [nginxDefaults.py](https://github.com/DanielMelloo/dmtoolbox/blob/main/dmtoolbox/nginxDefaults.py)  e .py[nginxDefaults.py](https://github.com/DanielMelloo/dmtoolbox/blob/main/dmtoolbox/nginxDefaults.py) 
 - Proporcionam ferramentas para o gerenciamento detalhado de configurações do servidor NGINX, incluindo inicialização, parada, e verificação de status.
 
 ### [numericFuncs.py](https://github.com/DanielMelloo/dmtoolbox/blob/main/dmtoolbox/numericFuncs.py)
 - Inclui funções para análises numéricas avançadas, manipulação de matrizes, e visualização de dados em 2D e 3D.
 
 ### [osFuncs.py](https://github.com/DanielMelloo/dmtoolbox/blob/main/dmtoolbox/osFuncs.py)
 - Contém utilitários para interações avançadas com o sistema operacional, como verificação de privilégios de administrador e manipulação de arquivos e diretórios.
 
 ### [portTools.py](https://github.com/DanielMelloo/dmtoolbox/blob/main/dmtoolbox/portTools.py)
 - Fornece métodos para verificar a disponibilidade de portas TCP/IP e selecionar portas disponíveis para aplicações.
 
+### [regedit.py](https://github.com/DanielMelloo/dmtoolbox/blob/main/dmtoolbox/regedit.py)
+- Permite a criação e gerenciamento de entradas de registro do Windows, facilitando a integração com o sistema operacional.
+
 
 
 ## Instalação do Pacote dmtoolbox
 
 Para instalar o pacote dmtoolbox de maneira eficiente e segura, siga os passos abaixo. Recomendamos a utilização de um ambiente virtual Python para evitar conflitos de dependências com outros pacotes instalados no sistema.
 
 ### Pré-Requisitos
@@ -143,20 +161,18 @@
 ```bash
 pip install -r requirements.txt
 ```
 
 Em seguida, clone o repositório do GitHub ou baixe os arquivos do projeto diretamente para o seu ambiente de trabalho.
 
 
-## Exemplos de Uso
 
-Para ajudá-lo a começar, fornecemos uma série de exemplos práticos no diretório [`Exemplos de Código`](https://github.com/DanielMelloo/dmtoolbox/tree/main/Exemplos%20de%20Código). Aqui você encontrará amostras de código demonstrando como utilizar as funcionalidades disponíveis no dmtoolbox.
-
-Para acessar os exemplos, navegue até a pasta [`Exemplos de Código`](https://github.com/DanielMelloo/dmtoolbox/tree/main/Exemplos%20de%20Código) no repositório do projeto ou clique no link.
 
+## Exemplos de Uso
+Para cada módulo, exemplos detalhados de uso são fornecidos na documentação interna. Estes exemplos abrangem desde a criação de diretórios no AppData até a configuração avançada do NGINX e análise numérica com visualização de dados.
 
 ## Contribuições
 Encorajamos contribuições! Se deseja sugerir melhorias, corrigir bugs ou adicionar novas funcionalidades, por favor, abra uma issue ou submeta um pull request.
 
 
 ## Autor
```

### Comparing `dmtoolbox-0.1.28.1/setup.py` & `dmtoolbox-0.10/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,43 +2,39 @@
 
 # Carregando a descrição longa do README.md
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='dmtoolbox',
-    version = '0.1.28.1',
+    version='0.10',
     packages=find_packages(),
     description='dmtoolbox é uma coleção abrangente de ferramentas Python projetadas para facilitar a automação de tarefas e operações no ambiente Windows, manipulação avançada de arquivos e diretórios, criação e gestão de executáveis, manipulação de dados JSON, gerenciamento de configurações NGINX, análise numérica, e muito mais.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Daniel Mello',
-    author_email='danielmello.dev@gmail.com',
+    author_email='danielmello.dev@example.com',
     license='GPLv3',
     install_requires=[
-        'pandas>=2.2.1',
-        'numpy>=1.26.4',
-        'prettytable>=3.10.0',
-        'matplotlib>=3.8.3',
-        'colorama>=0.4.6',
-        'openpyxl>=3.1.2',  
-        'jinja2>=3.1.3',
+        'pandas==2.2.1',
+        'numpy==1.26.4',
+        'prettytable==3.10.0',
+        'matplotlib==3.8.3',
+        'colorama==0.4.6',
+        'pyinstaller==6.4.0',
     ],
     python_requires='>=3.6',
-    url='https://github.com/DanielMelloo/dmtoolbox',
+    url='https://github.com/danielmello/dmtoolbox',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
     keywords='utils automation numpy pandas matplotlib',
 )
-
-
-
```

