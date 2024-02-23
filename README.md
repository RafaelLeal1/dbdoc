# dbdoc

## Prática MYSQL/Apache

## Acompanhe também pelo Notion: https://persistent-xenon-04d.notion.site/Documenta-o-2d3ef1800ef347bfa2fdb331ed175e8c?pvs=4

### Documentação 1: Inserção de Dados em Colunas com Tipo Char (Apache e MySQL)

#### Visão Geral

Este repositório fornece um guia passo a passo sobre como inserir dados em colunas com tipo char usando o myphpserver Apache e MySQL Server.

#### Pré-requisitos

Antes de começar, certifique-se de ter o seguinte:

- Ambiente de desenvolvimento configurado com o myphpserver Apache e MySQL Server.
- Acesso ao sistema de banco de dados onde as colunas serão criadas.

#### Passo a Passo

1. Acesse o sistema de banco de dados onde você deseja criar as colunas.
2. Utilize comandos SQL para criar as colunas desejadas com o tipo char na tabela apropriada.
3. Insira os dados nas colunas recém-criadas usando comandos SQL de inserção.
4. Verifique se os dados foram inseridos corretamente usando consultas SQL de seleção.
5. Capture um print do funcionamento para documentação e verificação.


---

### Documentação 2: Guia: Executando Tarefas com Apache e MySQL Server

#### Visão Geral

Este guia abrange a execução de tarefas com Apache e MySQL Server no ambiente do myphpserver.

#### Pré-requisitos

- Ambiente de desenvolvimento configurado com Apache e MySQL Server.
- Acesso a recursos de desenvolvimento e administração do ambiente.

#### Passo a Passo

1. Configure o ambiente com Apache e MySQL Server.
2. Realize tarefas específicas, como manipulação de banco de dados, execução de scripts PHP, etc.
3. Verifique os resultados e depure quaisquer problemas encontrados.
4. Capture prints ou registre qualquer aspecto relevante do funcionamento.

---

Essas documentações proporcionam um guia claro e detalhado sobre como realizar tarefas específicas com o myphpserver Apache e MySQL Server, facilitando o desenvolvimento e a administração de aplicações web.


Aqui está a documentação para o passo a passo de exclusão dos dados inseridos na tabela e posteriormente a exclusão da própria tabela, tudo realizado através de comandos SQL:

---

-- Criação das Colunas
```sql
ALTER TABLE nome_da_tabela # Caso precise!
ADD nome_coluna1 CHAR(tamanho) DEFAULT ' ',
ADD nome_coluna2 CHAR(tamanho) DEFAULT ' ';
```
-- Inserção de Dado

```sql
INSERT INTO nome_da_tabela (nome_coluna1, nome_coluna2) VALUES ('dado1', 'dado2');
```

-- Verificação

```sql
SELECT * FROM nome_da_tabela;
```

### Documentação 3 : Exclusão de Dados e Tabela com SQL

Este guia fornece instruções sobre como excluir os dados inseridos em uma tabela e posteriormente excluir a tabela em um banco de dados utilizando comandos SQL.

## Visão Geral

Neste tutorial, você aprenderá como excluir os dados inseridos em uma tabela específica e, em seguida, excluir a própria tabela do banco de dados.

## Pré-requisitos

Antes de começar, certifique-se de ter o seguinte:

- Acesso ao sistema de gerenciamento de banco de dados (SGBD) onde a tabela está localizada.
- Conhecimento básico sobre comandos SQL para manipulação de dados e tabelas.

## Passo a Passo

1. **Exclusão dos Dados Inseridos:**

   Para excluir os dados inseridos na tabela, utilize o comando SQL `DELETE FROM nome_da_tabela;`. Substitua `nome_da_tabela` pelo nome da tabela onde os dados foram inseridos.

   Exemplo:
   
   ```sql
   DELETE FROM minha_tabela;
   ```

3. **Exclusão da Tabela:**

   Após excluir os dados, você pode excluir a tabela usando o comando SQL `DROP TABLE nome_da_tabela;`. Substitua `nome_da_tabela` pelo nome da tabela que deseja excluir.

   Exemplo:
   ```sql
   DROP TABLE minha_tabela;
   ```

   ** Exclusão de dados

   Passo a Passo
Identifique os Dados a Serem Excluídos:

Determine os valores dos registros que você deseja excluir da tabela. Isso pode envolver revisar os dados previamente inseridos ou identificar critérios específicos para a exclusão.

Formule o Comando SQL de Exclusão:

Use a seguinte estrutura do comando DELETE para formular a sua consulta:

```sql
DELETE FROM nome_da_tabela WHERE condição;
```

Substitua nome_da_tabela pelo nome da sua tabela e condição pela cláusula que identifica os registros a serem excluídos. A condição pode ser baseada em valores específicos de colunas ou outros critérios.

Execute o Comando SQL:

Utilize o cliente MySQL ou outra interface de administração de banco de dados para executar o comando DELETE que você formulou no passo anterior.

Verifique os Dados Excluídos:

Após executar o comando DELETE, verifique se os dados foram excluídos corretamente. Você pode usar comandos SELECT para visualizar os registros na tabela e confirmar que os registros desejados foram removidos.

Documente o Processo:

Capture um print ou faça anotações sobre o processo de exclusão de dados para referência futura. Isso pode ser útil para auditorias ou em casos em que você precisa rastrear alterações no banco de dados.

Importante:
Tenha cuidado ao usar o comando DELETE, pois ele remove os dados permanentemente e não pode ser desfeito.
Sempre faça backup dos seus dados antes de executar operações de exclusão em larga escala ou irreversíveis.

4. **Verificação:**

   Após executar os comandos SQL, verifique se os dados foram excluídos corretamente e se a tabela foi removida do banco de dados.



## Contribuindo

Se você encontrar erros neste guia ou tiver sugestões para melhorias, sinta-se à vontade para abrir uma issue ou enviar um pull request.

## Licença

Este projeto está licenciado sob a [LICENÇA MIT]. Consulte o arquivo LICENSE para obter mais detalhes.

---

Esta documentação oferece um guia claro sobre como excluir os dados inseridos em uma tabela e posteriormente excluir a tabela em um banco de dados usando comandos SQL, com a inclusão de um passo de verificação e captura de print para documentação e verificação do processo.
