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

- QaConductor.xml - arquivo contendo todos os casos de teste a serem executados na suite da automação.

## Parâmetros chaves a serem modificados em cada um dos arquivos

- config.properties  
    - browser.name: Nome do navegador;
    - prop.emissor: Nome do emissor;
    - site.address: Endereço da aplicação;
    - site.login: Login do usuário;
    - site.senha: Senha do usuário;
    - tipo.execucao: Local ou em grid(Servidor).
                        
- sqa.properties
    - testlink.key: Chave única de usuário para execução dos testes na ferramenta;
    - testlink.project.name: Nome do projeto criado na ferramenta;
    - testlink.plan.name: Nome do plano de teste associado ao projeto criado na ferramenta;
    - testlink.build.name: Baseline associada ao plano de testes criado na ferramenta;
    - executar.testlink: False para não passar a execução do teste na ferramenta e True para passar.
    
- QaConductor.xml
    - name: Nome do emissor;
    - thread-count: Número de janelas a serem abertas ao executar a suite de testes.

## Rodando os testes

- Rodar todos os testes da automação
    - Botão direito no arquivo QaConductor.xml -> Run as TestNG Suite
    ![Recordit GIF](http://g.recordit.co/UfljdGP1Wj.gif)
    
- Rodar todos os testes de uma classe de teste    
    - Entrar na classe de teste -> Clicar com o botão direito -> Run as TestNG Suite
    ![Recordit GIF](http://g.recordit.co/Bzo68RbhYF.gif)
 
- Rodar apenas um caso de teste   
    - Entrar na classe de teste -> Selecionar método de teste -> Clicar com o botão direito -> Run as TestNG Suite
    ![Recordit GIF](http://g.recordit.co/pMn5DSlWJD.gif)
    
## Autores

- Luis Paulo Ramos Milheiro
- Jefferson Ferreira Torres Bessa
- Matheus Carneiro de Souza Barros
