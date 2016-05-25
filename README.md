# xy-inc
--TECNOLOGIAS UTILIZADAS

JSP – (Java Server Page) para construção de páginas dinâmicas.
JSTL – (JSP Stantard Tag Library) biblioteca de tags para construcao da construção de página 
Servlet – para as requisições do protocolo HTTP.
JDBC – (Java Database Connectivity) forma padrão de acesso a Banco de dados em Java
PostgreSQL – banco de dados relacional 
Padrão MVC – Model View Controller é um padrão de projeto que divide nossa aplicação em várias camadas

--CRIAÇÃO DO BANCO

CREATE TABLE IF NOT EXISTS tbxyinc( 
cadastro bigint NOT NULL, 
pontoReferencia varchar(20) NOT NULL,
coordenadaX varchar(20) NOT NULL, 
coordenadaY varchar(20) NOT NULL, 
CONSTRAINT tbaluno_pkey PRIMARY KEY (cadastro)
);

--SOFTWARE NECESSARIO

instale o JDK 8u45
http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html

baixe a versao 8 do TomCat para o seu SO e descompacte na pasta que desejar
http://tomcat.apache.org/download-80.cgi

instale o eclipse para JAVA EE 
http://www.eclipse.org/downloads/packages/eclipse-ide-java-ee-developers/marsr


--CONFIGURAÇÕES NECESSARIAS NO ECLIPSE

1 - Apontar o eclipse para o JDK
Window > Preferences > Installed JREs
Adicione o caminho do JDK e defina-o como padrao

2 - Criar servidor TomCat
File > New > Other > Server
Selecione "Tomcat v8.0 Server"
Adicione o diretorio do Tomcat baixado 

3 - Publicar o projeto no Tomcat
Na view Severs clique com o botao direito no Tomcat > Add and Remove
Clique em xy-inc, depois clique em Add. A aplicacao passara de Available para Configured
Clique em Finish
Clique com o botao direito no Tomcat > Start

4 - Testar a aplicaçao
Quando o servidor subir, entre na URL
http://localhost:8080/xy-inc/

