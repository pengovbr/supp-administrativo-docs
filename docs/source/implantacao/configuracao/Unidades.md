# Unidades

 

Unidade é uma estrutura organizacional concentradora de setores, disposta por região, por matéria ou por especialidade.  

Toda unidade: 

- é ligada a um Órgão Central; 

- contêm setores ligados a ela; 

- terá obrigatoriamente um setor de Arquivo e um setor de Protocolo, que serão gerados automaticamente pela ferramenta quando do seu cadastro; e 

- terá ao menos um Coordenador, que será o responsável pela criação de modelos de documentos, liberação de permissões e demais definições administrativas da Unidade. 

 

Abaixo segue figura que demonstra o relacionamento entre Órgãos, Unidades e Setores. 

<img src="../../_static/images/Unidades - Figura Demonstrativa.png"/>

<p style="text-align: center;">Figura 1 - Esquema relacional entre Órgão Central, Unidade e Setores</p> 


As demandas encaminhadas a uma Unidade poderão ser direcionadas ao protocolo desta unidade ou diretamente a um de seus setores. Esta definição ficará a cargo da Unidade demandada, e será concretizada via configuração no Super.GOV.BR 2.0.  

Somente os usuários com perfil Administrador no Super.GOV.BR 2.0 têm autorização para criação ou edição de uma Unidade. Para ter acesso à criação e edição de Unidade, é necessária a criação inicial do Órgão Central. O procedimento da criação do Órgão pode ser encontrado clicando [aqui](configuraçao/Orgaos.md).



```{note}
Nota: Não é recomendada a exclusão do registro de Unidade no sistema. Caso uma Unidade deixe de existir na estrutura do governo, recomenda-se a inativação desta no sistema. Desta forma, será garantida a preservação do histórico de atividades da Unidade. 
```


## Tela Unidades 

O menu Unidades permite visualizar as Unidades cadastradas no sistema, além da possibilidade de incluir outras Unidades e alterar as existentes. 

Também é possível visualizar os setores de cada Unidade e acrescentar novas competências (Municípios) àquela Unidade. 

Ao optar por visualizar os setores, uma grid é aberto, onde é possível editar o Setor, manipular lotações e localizadores, além da possibilidade de remover o Setor.


<img src="../../_static/images/Unidades - Tela Principal.png"/>
<p style="text-align: center;"> Figura 2 - Tela Principal da Unidade </p> 


1) Criar um registro de Unidade; 

2) Colunas. Por esta opção será possível gerenciar as colunas que serão disponibilizadas na tela; 

3) Recarregar. Opção permite a atualização dos registros apresentados em tela;  

4) Filtro. Opção possibilita filtrar um intervalo de dados com base em critérios definidos. 

5) Editar o cadastro de uma Unidade; 

6) Cadastro de Setor;

7) Opção permite configurar a quantidade de registro a serem mostrados em tela;

8) Tarja indica a quantidade de páginas relacionadas a consulta em tela. A navegação entre as páginas poderá ser feita por meio do uso das setas disponíveis. 
 

## Como Criar uma nova UNIDADE no Super.GOV.BR 2.0 



01\. Para criação de uma nova unidade, o usuário deverá acessar o Menu Unidade e clicar no botão “Novo” <img src="../../_static/images/Botão de Inclusão (+).png" alt="Botão de Inclusão (+)" style="zoom: 50%;" /> localizado na parte superior esquerda da tela. 

 
02\. Em seguida, deverá preencher os campos disponíveis no formulário com as informações referentes à Unidade a ser cadastrada.  

```{note}
Nota: Todos os campos marcados com * são de preenchimento obrigatório. 
```

<img src="../../_static/images/Unidades - Tela com a Lista de Campos.png"/>
<p style="text-align: center;"> Figura 3 - Tela de Formulário de Criação de Unidade </p> 
 

**Nome:** Campo obrigatório, destinado ao preenchimento do nome da Unidade; (Existe algum link para o critério?) 


**Sigla:** Campo obrigatório, destinado ao preenchimento da SIGLA da Unidade; (Existe algum link para o critério?) 
 

**Prefixo NUP:** campo obrigatório, destinado à inclusão do código único que identificará a Unidade e fará parte da numeração única processual (NUP) dos processos criados pela Unidade; 


*Exemplo:* Se preenchido o prefixo 00400 neste campo, significa que todos os processos abertos nesta unidade terão um NUP iniciado por 00400, seguido do seu sequencial, ano e dígito verificador. Ficando desta forma: NUP 00400.000001/2021-82. 

```{note}
Nota: As áreas de gestão documental dos órgãos poderão informar os prefixos NUP da Unidade, caso seja necessário. 
```

**NUP Inicial:** campo opcional, utilizado para definir o número a partir do qual o sequencial NUP da unidade se iniciará. Usado para os casos em que já existem processos anteriores à ativação desta Unidade (que estejam em tramitação ou concluídos) e a Unidade deseja preservar a continuidade desta sequência no Super.GOV.BR 2.0. 

```{note}
Notas: 

1) Caso a Unidade deseje iniciar o sequencial a partir de 00000001, o campo NUP Inicial não precisará ser preenchido. 

2) O sequencial NUP iniciará uma nova contagem a cada ano, ou seja, um novo sequencial será iniciado a partir do dia 01 de janeiro de cada ano. 
```


**Endereço:** campo opcional, destinado à indicação do endereço físico da Unidade. 
```(Qual a utilidade deste campo?) ```
 

**E-mail:** Campo opcional, destinado à indicação do email da Unidade. ```(Qual a utilidade deste campo?)```


**Órgão Central:** Campo obrigatório. Órgão ao qual a Unidade está vinculada. Só é possível vincular a Unidade a um Órgão Central. 

**Unidade Pai:** campo opcional, utilizado para o cadastro de estrutura aglutinadora de unidades. Usado, exclusivamente, para fins de consumo de ferramentas de BI.  


```{note}

Nota: O campo Unidade Pai não afeta ou interfere nas funcionalidades do Super.GOV.BR 2.0. 
```


**Gênero:** Campo obrigatório, utilizado para informar a natureza dos processos/tarefas executadas na Unidade, podendo ser, por exemplo, Administrativos ou Arquivísticos. Os usuários lotados na unidade terão acesso às funcionalidades do módulo, conforme o gênero indicado neste campo. 

 

**Município:** Campo obrigatório, utilizado para o registro do município da instalação física da unidade; (Por que o campo Município é obrigatório e o campo endereço é opcional?)  

 

**Ativo:** Flag que indica se o registro da unidade é Ativo ou Inativo. Uma unidade Ativa indica se esta continua exercendo suas funções dentro do órgão.

 

**Configuração**

**Protocolo:** Flag de configuração do caminho de entrada de demandas originárias de outras Unidades. Caso esteja marcada, significa que todas as demandas direcionadas por outras Unidades serão encaminhadas ao setor de protocolo da Unidade. 
Caso não esteja marcada, significa que outras Unidades poderão encaminhar demandas diretamente aos setores ligados a Unidade. 

**Numeração de Documento por Unidade:** Se marcada essa opção, será configurado para que os documentos gerados pelos seus setores tenham um sequencial específico desta Unidade. 


```{note}
Nota: Os documentos gerados nesta Unidade terão uma numeração sequencial baseada no ano e na própria Unidade.  
```

03\. Clicar em Salvar

Pronto, a nova Unidade está criada. Após esse cadastro, está habilitado a seguir os próximos passos da Configuração Inicial do Super.GOV.BR 2.0.

É sugerido continuar com a criação de [Setores](configuraçao/Setor.md) e Lotações (que é um segmento do documento inserido em Setores).
