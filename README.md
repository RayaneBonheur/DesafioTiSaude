# Desafio Técnico TiSaude

Este projeto foi desenvolvido para atender ao desafio técnico proposto pela Ti.Saúde, que visa avaliar habilidades essenciais em manipulação de dados, SQL e Python para análise de agendamentos de consultas e procedimentos médicos. O objetivo é estruturar, manipular e analisar os dados para fornecer relatórios estratégicos que possam auxiliar na otimização da gestão dos serviços de saúde.

------

## OBJETIVO
- Estruturar um banco de dados para armazenar dados de agendamentos a partir de um arquivo CSV;
- Realizar manipulação e atualização dos dados via comandos SQL;
- Gerar relatórios estratégicos utilizando consultas SQL;
- Automatizar consultas e análises simples utilizando Python e a biblioteca Pandas;
- Criar visualizações que destaquem insights relevantes para a Ti.Saúde;

------

## REQUISITOS 
- Criação da tabela agendamentos para armazenar dados do CSV;
- Atualização dos agendamentos da especialidade "Cardiologia" conforme regras definidas;
- Geração de 4 relatórios estratégicos baseados nos dados;
- Desenvolvimento de um script Python para análise e exportação de dados filtrados;
- Desenvolvimento de uma visualização gráfica dos dados analisados;
- Documentação clara e organizada dos passos e ferramentas usadas.

------

## ESCOPO
| Tarefa                                   | Descrição                                                                                     |
| ---------------------------------------- | --------------------------------------------------------------------------------------------- |
| Criação e estruturação do banco de dados | Criar banco e tabela `agendamentos` adequada para dados do arquivo CSV.                       |
| Importação de dados                      | Importar dados do arquivo `agendamentos_tisaude.csv` para a tabela criada.                    |
| Atualização de dados (SQL)               | Atualizar status e valores dos agendamentos de "Cardiologia" com status "Agendado".           |
| Geração de relatórios (SQL)              | Criar consultas para relatórios: produtividade, cancelamentos, receita mensal e taxa no-show. |
| Automação com Python                     | Script para selecionar e analisar agendamentos de "Ortopedia" realizados nos últimos 30 dias. |
| Visualização de dados                    | Criar gráficos ou dashboards para evidenciar insights relevantes.                             |
| Documentação                             | Arquivo README com explicações do projeto, instruções e bibliotecas usadas.                   |

------

## METODOLOGIA DE DESENVOLVIMENTO
1.Levantamento dos Requisitos: Entendimento do desafio e definição das tarefas.
2.Modelagem do Banco: Criação da tabela e definição dos tipos de dados.
3.Importação de Dados: Transferência dos dados CSV para o banco.
4.Manipulação dos Dados: Aplicação de regras via SQL para atualização.
5.Análise e Relatórios: Desenvolvimento de consultas para gerar informações estratégicas.
6.Automação com Python: Desenvolvimento de script para consultas dinâmicas e exportação.
7.Visualização: Criação de gráficos para melhor entendimento dos dados.
8.Documentação: Registro dos processos, instruções e tecnologias utilizadas.

------

## TECNOLOGIAS UTILIZADAS
| Tecnologia                 | Descrição                                                                                                    |
| -------------------------- | ------------------------------------------------------------------------------------------------------------ |
| **XAMPP**                  | Ambiente local que inclui Apache, PHP, MySQL/MariaDB, facilitando a configuração e uso do banco MySQL localmente para desenvolvimento. |
| **MySQL**                  | Sistema gerenciador de banco de dados relacional, usado para armazenar e manipular os dados de agendamentos. |
| **Python 3.x**             | Linguagem de programação para automação da análise dos dados e exportação de arquivos.                       |
| **pandas**                 | Biblioteca Python para manipulação e análise de dados estruturados.                                          |
| **mysql-connector-python** | Biblioteca Python para conexão e execução de comandos no MySQL via Python.                                   |
| **Excel**                  | Ferramenta para visualização gráfica dos dados, criação de gráficos a partir das consultas SQL exportadas.   |

------

## COMO RODAR O PROJETO
1. Banco de Dados
- Instale o MySQL (ou utilize uma instância já disponível).
- Crie um banco de dados novo para o projeto.
- Execute o script SQL de criação da tabela agendamentos:
  -- Exemplo:
CREATE TABLE agendamentos (
  id_agendamento INT PRIMARY KEY,
  id_paciente INT,
  id_medico INT,
  data_agendamento DATE,
  tipo_consulta VARCHAR(50),
  especialidade VARCHAR(50),
  status_agendamento VARCHAR(50),
  valor_consulta DECIMAL(10,2)
);













