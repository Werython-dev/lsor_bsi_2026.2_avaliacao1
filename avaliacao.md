# 📑 MODELO DE ENTREGA: AVALIAÇÃO PRÁTICO-TEÓRICA I
## Disciplina: Laboratório de Sistemas Operacionais e Redes (LSOR)
**Professor:** Alaelson Jatobá  
**Semestre Letivo:** 2026.02  
**Curso:** Bacharelado em Sistemas de Informação (BSI)  

---

## 👤 Identificação do Aluno
*   **Nome Completo:** [Preencha aqui seu nome]
*   **Matrícula:** [Preencha aqui sua matrícula]
*   **Link do Repositório Pessoal no GitHub:** [Preencha aqui o link do seu repositório]
*   **Data de Realização:** [Preencha aqui a data]

---

## 🚨 Instruções Gerais de Entrega e Realização

1.  **Criação do Repositório:** Você deve possuir um repositório dedicado exclusivamente para a documentação técnica da disciplina de **Laboratório de Sistemas Operacionais e Redes** no seu GitHub.
2.  **Configuração da Página Inicial:** Certifique-se de que o repositório possua um arquivo `README.md` como página de índice apontando para todos os seus relatórios e avaliações.
3.  **Entrega Oficial:** Copie o conteúdo deste arquivo de template, salve como `Avaliacao1.md` em seu repositório, responda às questões abertas diretamente no arquivo e insira as capturas de tela (prints) correspondentes nos locais demarcados. O envio final será feito através do formulário do **Google Forms**, fornecendo o link direto deste arquivo `.md` publicado no GitHub.
4.  **Execução de Comandos:** Para fins de conformidade técnica e validação das permissões, execute todas as tarefas de criação e controle com privilégios administrativos usando `sudo` apenas onde for estritamente necessário.

---

## 📋 Questões da Avaliação I

### 💻 QUESTÃO 1: Importação de VM no VirtualBox
O professor disponibilizou uma máquina virtual pré-configurada em formato `.ova` no servidor de arquivos do laboratório. 
*   **Caminho de Origem:** `\\172.20.20.21\public\avaliacao1`
*   **Nome do Arquivo:** `UbuntuAvaliacao1.ova`
*   **Credenciais de Acesso ao Servidor de Arquivos:** Usuário: `alunoifal` | Senha: `alunoifal`

**A) Prática:** Copie o arquivo `.ova` do servidor de arquivos para o drive `C:` local da sua máquina host de laboratório e importe a máquina virtual para o Oracle VM VirtualBox.
> **🖼️ INSERIR PRINT DA VM IMPORTADA ATIVA NO SEU VIRTUALBOX AQUI**
> *(A captura de tela deve mostrar a janela do VirtualBox com a VM `UbuntuAvaliacao1` em execução e o console de login ativo).*

**B) Teórica:** Descreva detalhadamente as etapas executadas para obter e importar o arquivo `.ova` no seu computador hospedeiro (host Windows). Explique também qual é a diferença teórica de portabilidade entre importar um arquivo empacotado `.ova` (Open Virtualization Format) e instalar um sistema operacional do zero a partir de uma mídia `.iso`.

*   **Sua resposta teórica:**
    [Substitua este texto pela sua resposta técnica]

---

### 👥 QUESTÃO 2: Criação de Usuários e Grupos de Trabalho
Após fazer login na máquina virtual importada com as credenciais padrões de administração do laboratório (usuário `administrador` e senha `adminifal`), você deve gerenciar os perfis de usuários e organizá-los sob um mesmo grupo corporativo.

**A) Prática:** Crie quatro novos usuários no sistema e em seguida crie o grupo de trabalho chamado **`presidenciaveis`**, inserindo todos os usuários criados nesse grupo de forma complementar. As credenciais exigidas são:
1.  Usuário: **`luiz`** | Senha: **`luiz13`**
2.  Usuário: **`flavio`** | Senha: **`flavio22`**
3.  Usuário: **`augusto`** | Senha: **`augusto70`**
4.  Usuário: **`renan`** | Senha: **`renan14`**

> **🖼️ INSERIR PRINT DO TERMINAL EXECUTANDO A CRIAÇÃO DE UM DOS USUÁRIOS E ASSOCIAÇÃO AO GRUPO AQUI**
> *(A captura de tela deve demonstrar a saída dos comandos aplicados no console).*

**B) Teórica:** Do ponto de vista de administração de sistemas Linux, qual é a diferença técnica e o nível de segurança envolvidos na criação de usuários locais usando o comando interativo `adduser` em comparação com o comando de baixo nível `useradd`? Além disso, explique qual a vantagem administrativa de gerenciar permissões por meio de grupos de trabalho complementares em vez de atribuir permissões individuais.

*   **Sua resposta teórica:**
    [Substitua este texto pela sua resposta técnica]

---

### 🔍 QUESTÃO 3: Auditoria do Sistema de Contas (`getent`)
Após a criação e organização das contas, o administrador de sistemas deve inspecionar as bases administrativas para auditar se os registros foram integrados com sucesso.

**A) Prática:** Execute os comandos necessários no terminal para auditar e exibir as contas criadas (`luiz`, `flavio`, `augusto`, `renan`), bem como o grupo `presidenciaveis` com todos os seus respectivos membros associados.
> **🖼️ INSERIR PRINT EXIBINDO AS ÚLTIMAS ENTRADAS DOS COMANDOS DE AUDITORIA AQUI**
> *(A captura de tela deve exibir a saída do terminal comprovando a existência dos usuários e o vínculo com o grupo).*

**B) Teórica:** Descreva o papel técnico do utilitário **`getent`** no Linux e qual a sua vantagem funcional em relação à simples leitura manual dos arquivos estáticos `/etc/passwd` e `/etc/group` utilizando comandos como `cat`.

*   **Sua resposta teórica:**
    [Substitua este texto pela sua resposta técnica]

---

### 📄 QUESTÃO 4: Cadastro Eleitoral em Formato Estruturado (JSON)
Cada um dos candidatos recém-criados deve possuir um arquivo de identificação estruturado dentro de sua respectiva pasta pessoal no diretório `/home`.

**A) Prática:** Alterne para cada uma das contas criadas utilizando o comando que carrega a sessão de login completa e crie no diretório inicial (`~` ou `/home/usuario`) de cada um dos usuários um arquivo chamado **`cadastroeleitoral.txt`** contendo os dados cadastrais em formato **JSON**.

**Template Padrão do Arquivo `cadastroeleitoral.txt`:**
```json
{
  "nome_candidato": "NOME DO CANDIDATO",
  "partido": "PARTIDO",
  "numero_candidato": 99
}
```

*Personalize o preenchimento de cada arquivo conforme os dados fictícios sugeridos:*
*   Para o usuário `luiz`: `"nome_candidato": "LUIZ INACIO"`, `"partido": "PLUIZ"`, `"numero_candidato": 13`
*   Para o usuário `flavio`: `"nome_candidato": "FLAVIO"`, `"partido": "PFLAVIO"`, `"numero_candidato": 22`
*   Para o usuário `augusto`: `"nome_candidato": "AUGUSTO"`, `"partido": "PAUGUSTO"`, `"numero_candidato": 70`
*   Para o usuário `renan`: `"nome_candidato": "RENAN"`, `"partido": "PRENAN"`, `"numero_candidato": 14`

> **🖼️ INSERIR PRINT DO ARQUIVO DE CADASTRO DE UM DOS USUÁRIOS EXIBIDO COM O COMANDO CAT AQUI**
> *(A captura de tela deve demonstrar o conteúdo do arquivo e o caminho completo onde ele foi salvo).*

**B) Teórica:** O que é o formato JSON (JavaScript Object Notation)? Por que ele é amplamente adotado em sistemas operacionais modernos, servidores e integrações de rede para troca de informações estruturadas em comparação com arquivos de texto puro não estruturados?

*   **Sua resposta teórica:**
    [Substitua este texto pela sua resposta técnica]

---

### 📂 QUESTÃO 5: Estruturação de Pastas e Padrão FHS
O sistema precisa de uma pasta centralizada na raiz do disco para organizar a consolidação das informações eleitorais.

**A) Prática:** Na raiz do sistema operacional (`/`), crie um diretório chamado **`/eleicoes`**.
> **🖼️ INSERIR PRINT DO TERMINAL EXECUTANDO A CRIAÇÃO DO DIRETÓRIO AQUI**
> *(A captura de tela deve demonstrar o comando executado no terminal e a verificação do diretório `/eleicoes` listado).*

**B) Teórica:** Explique teoricamente as regras do padrão FHS (Filesystem Hierarchy Standard) do Linux. Por que a criação de diretórios personalizados diretamente na raiz `/` (como `/eleicoes`) é incomum em sistemas de produção? Qual pasta padrão da árvore FHS seria mais adequada para armazenar dados de serviços compartilhados de uma aplicação de acordo com essa especificação?

*   **Sua resposta teórica:**
    [Substitua este texto pela sua resposta técnica]

---

### ⚙️ QUESTÃO 6: Automação e Shell Scripting (`cadastrarcandidatos.sh`)
Você criará uma rotina para automatizar a leitura e consolidação dos cadastros de candidatos armazenados nas homes dos usuários do sistema.

**A) Prática:** Dentro da pasta `/eleicoes` recém-criada, escreva um script de terminal em Bash chamado **`cadastrarcandidatos.sh`**. 

O script deverá:
1.  Solicitar interativamente que o aluno digite seu próprio nome completo.
2.  Gerar (ou sobrescrever) um arquivo de saída chamado **`/eleicoes/presidenciaveis2026.txt`**.
3.  Escrever o cabeçalho no arquivo contendo o nome do aluno que o executou e a data da operação.
4.  Realizar uma busca automatizada por todos os arquivos `cadastroeleitoral.txt` salvos nas homes dos usuários.
5.  Extrair e anexar o conteúdo de cada um dos cadastros eleitorais encontrados para dentro de `/eleicoes/presidenciaveis2026.txt`.

**Código de Referência do Script `cadastrarcandidatos.sh`:**
```bash
#!/bin/bash

# Solicita o nome completo do aluno
echo "=========================================="
read -p "Digite seu nome completo (Aluno): " nome_aluno
echo "=========================================="

# Define os caminhos de arquivos
ARQUIVO_SAIDA="/eleicoes/presidenciaveis2026.txt"

# Cria/Sobrescreve o arquivo de saída com o cabeçalho
echo "RELATÓRIO CONSOLIDADO DE CANDIDATOS - ELEIÇÕES 2026" > $ARQUIVO_SAIDA
echo "Executado por (Aluno): $nome_aluno" >> $ARQUIVO_SAIDA
echo "Data da Execução: $(date)" >> $ARQUIVO_SAIDA
echo "==========================================" >> $ARQUIVO_SAIDA
echo "" >> $ARQUIVO_SAIDA

# Laço para buscar recursivamente todos os arquivos 'cadastroeleitoral.txt' nas homes
for arquivo in /home/*/cadastroeleitoral.txt; do
    if [ -f "$arquivo" ]; then
        echo "Lendo cadastro de: $arquivo"
        echo "--- Origem: $arquivo ---" >> $ARQUIVO_SAIDA
        cat "$arquivo" >> $ARQUIVO_SAIDA
        echo "" >> $ARQUIVO_SAIDA
        echo "------------------------------------------" >> $ARQUIVO_SAIDA
    fi
done

echo "Processamento concluído com sucesso!"
echo "Resultado gravado em: $ARQUIVO_SAIDA"
```

> **🖼️ INSERIR PRINT DO SCRIPT ESCRITO SENDO EXIBIDO COM O COMANDO CAT NO TERMINAL AQUI**
> *(A captura de tela deve mostrar o código completo do script dentro do console do Ubuntu Server).*

**B) Teórica:** Explique conceitualmente para que serve a linha inicial `#!/bin/bash` (Shebang) presente no script. O que ocorre se ela for omitida ou escrita de forma incorreta? Qual o papel do laço `for` utilizado no script para a busca automatizada dos arquivos?

*   **Sua resposta teórica:**
    [Substitua este texto pela sua resposta técnica]

---

### 🔒 QUESTÃO 7: Configuração de Permissões de Execução
Por padrão, arquivos de texto criados no Linux não possuem permissão de execução, impedindo que scripts sejam rodados diretamente.

**A) Prática:** Configure o arquivo `/eleicoes/cadastrarcandidatos.sh` para conceder permissão de execução. Exiba as propriedades detalhadas do arquivo antes e depois da modificação.
> **🖼️ INSERIR PRINT EXIBINDO AS PERMISSÕES DE EXECUÇÃO JÁ ALTERADAS COM O COMANDO LS -L AQUI**
> *(A captura de tela deve demonstrar claramente a modificação da máscara do arquivo de script, contendo a flag 'x').*

**B) Teórica:** Como se configura a permissão de execução de um arquivo no Linux? Explique detalhadamente o comando utilizado, o papel do bit de execução (`x`), e a diferença metodológica entre conceder permissão de forma simbólica (ex: `chmod +x`) e de forma octal/numérica.

*   **Sua resposta teórica:**
    [Substitua este texto pela sua resposta técnica]

---

### 🕵️ QUESTÃO 8: Execução e Consolidação do Relatório
Agora é o momento de rodar a rotina de automação e gerar o arquivo oficial de candidatos do laboratório.

**A) Prática:** Execute o script `cadastrarcandidatos.sh` localizado em `/eleicoes/`, insira seu nome completo quando solicitado pelo terminal, e exiba em tela o conteúdo final gerado no arquivo consolidado `/eleicoes/presidenciaveis2026.txt`.
> **🖼️ INSERIR PRINT DO TERMINAL MOSTRANDO A EXECUÇÃO DO SCRIPT E A EXIBIÇÃO DO RELATÓRIO FINAL COM O COMANDO CAT AQUI**
> *(A captura de tela deve exibir o input do seu nome, a conclusão do script e a leitura completa do arquivo presidenciaveis2026.txt contendo o cabeçalho com seu nome e as informações em JSON dos candidatos).*

**B) Teórica:** No script utilizado, como funciona o redirecionamento de saídas usando os operadores `>` (gravação simples) e `>>` (anexação)? O que aconteceria com os dados do arquivo de saída se o script utilizasse apenas o operador `>` em todas as linhas?

*   **Sua resposta teórica:**
    [Substitua este texto pela sua resposta técnica]

---

### 📂 QUESTÃO 9: Visualização e Filtros de Linha
Com o relatório `/eleicoes/presidenciaveis2026.txt` gerado, você deve realizar buscas rápidas de dados simulando a manutenção de sistemas de grande escala.

**A) Prática:** Utilizando filtros de terminal, execute comandos para exibir apenas as primeiras 3 linhas do arquivo consolidado, e em seguida, exiba apenas as últimas 5 linhas do mesmo arquivo.
> **🖼️ INSERIR PRINT DO TERMINAL EXECUTANDO OS FILTROS DE LINHAS INICIAIS E FINAIS AQUI**
> *(A captura de tela deve demonstrar os comandos de filtragem aplicados e os respectivos retornos no console).*

**B) Teórica:** Explique em quais cenários de administração e monitoramento de servidores Linux o uso de comandos de filtragem (como os que exibem o topo e o fim de arquivos) é preferível em detrimento da abertura completa do arquivo em editores de texto interativos como Nano ou Vim.

*   **Sua resposta teórica:**
    [Substitua este texto pela sua resposta técnica]

---

### 🕵️ QUESTÃO 10: Isolamento de Sessões (`su` vs `su -`)
Para a criação do arquivo `cadastroeleitoral.txt` (Questão 4), foi necessário alternar entre as sessões das contas locais do laboratório.

**A) Prática:** Demonstre e comprove a diferença prática no console executando a alternância para o usuário `luiz` utilizando o comando de substituição com e sem a flag de login.
> **🖼️ INSERIR PRINT DO TERMINAL COMPARANDO O DIRETÓRIO DE TRABALHO APÓS CADA UM DOS COMANDOS AQUI**
> *(A captura de tela deve exibir a execução de 'su luiz' seguido do comando 'pwd', e de 'su - luiz' seguido de 'pwd', demonstrando a mudança de caminhos).*

**B) Teórica:** Explique detalhadamente a diferença prática e conceitual que ocorre no terminal ao alternar usuários com e sem o hífen (`-`). Por que o uso do hífen é indispensável para garantir a validação de segurança e carregamento correto das permissões locais em ambientes de teste?

*   **Sua resposta teórica:**
    [Substitua este texto pela sua resposta técnica]

---
*Fim do Modelo de Entrega — Certifique-se de realizar o commit de todos os arquivos de relatório e enviar o link público no formulário do Google Forms dentro do prazo estabelecido.*
