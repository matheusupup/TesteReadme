# Automação de Testes do Íris

Projeto contendo a automação dos testes da aplicação Íris.

## Pré-requisitos

JAVA 8 - jre 1.8.0

Plugin do TestNG

Firefox 57.0

## Principais arquivos do projeto para rodar a automação

- QA Conductor.properties - arquivo com as configurações do emissor, como configurações de banco de dados, id_emissor, etc.

- config.properties - arquivo com as configurações gerais da automação. Exemplo: tipo do navegador, emissor a ser executado, url para da aplicação, etc.

- sqa.properties - arquivo com as configurações da integração da automação com a ferramenta TestLink, etc.

- AllTests.xml - arquivo contendo todas as suítes de teste da automação.

## Parâmetros chaves a serem modificados em cada um dos arquivos

- config.properties  
    - browser.name: Nome do navegador;
    - prop.emissor: Nome do emissor;
    - thread.count: Quantidade de testes executando em paralelo;
    - retry.limit: Vezes para reexecutar testes com falha;
    - site.address: Endereço da aplicação;
    - site.login: Login do usuário na aplicação;
    - site.senha: Senha do usuário na aplicação;
    - tipo.execucao: Local ou em grid(Servidor);
    - headless: True para abrir navegador e False para execução do teste sem abrir navegador;
    - dimensao.personalizada = True para ativar a resolução personalizada e False para usar resolução da tela principal;
    - largura: largura da resolução;
    - altura: altura da resolução.
                        
- sqa.properties
    - destinatario.email: Email utilizado para testes de envio de email.
    
## Rodando os testes

- Rodar todos os testes da automação em paralelo
    - Botão direito no arquivo AllTests.xml -> Run as TestNG Suite
    ![Recordit GIF](http://g.recordit.co/UfljdGP1Wj.gif)
    
- Rodar todos os testes de uma classe de teste em paralelo
    - Exemplo: Botão direito no arquivo Login.xml -> Run as TestNG Suite
    ![Recordit GIF](http://g.recordit.co/UfljdGP1Wj.gif)    

- Rodar todos os testes de uma classe de teste sem paralelismo
    - Entrar na classe de teste -> Clicar com o botão direito -> Run as TestNG Test
    ![Recordit GIF](http://g.recordit.co/Bzo68RbhYF.gif)
 
- Rodar apenas um caso de teste   
    - Entrar na classe de teste -> Selecionar método de teste -> Clicar com o botão direito -> Run as TestNG Test
    ![Recordit GIF](http://g.recordit.co/pMn5DSlWJD.gif)
    
## Autores

- Jefferson Ferreira Torres Bessa
- Luis Paulo Ramos Milheiro
- Luiz Felipe Martins
- Matheus Carneiro de Souza Barros
