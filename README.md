# 📑 Repositório Template: Avaliação 1 — LSOR - BSI(2026.02)

Este repositório é o modelo oficial para a realização e entrega da **Avaliação Prático-Teórica I** da disciplina de **Laboratório de Sistemas Operacionais e Redes (LSOR)** do curso de Bacharelado em Sistemas de Informação (BSI) no IFAL - Campus Maceió.

---

## 🚀 Instruções para o Aluno (Como Realizar a Prova)

### Passo 1: Criar o seu Repositório de Resposta
1. Certifique-se de estar logado em sua conta do GitHub.
2. Neste repositório de template do professor, clique no botão verde **"Use this template"** (Usar este modelo) -> **"Create a new repository"** (Criar um novo repositório).
3. Configure as propriedades do seu novo repositório pessoal:
   * **Repository name:** `lsorbsi2026.2-<nomedoaluno>-avaliacao1`
   * **Visibility:** Defina obrigatoriamente como **Private** (Privado) para evitar cópias e garantir a autoria individual de sua prova.
4. Após criar, vá em **Settings** -> **Collaborators** -> **Add people** e adicione o perfil do professor (`alaelson`) como colaborador para que ele possa acessar e corrigir sua entrega.

### Passo 2: Obter e Configurar o Ambiente de Testes (VM)
1. No laboratório de redes, acesse o servidor de arquivos local:
   * Caminho de rede: `\\172.20.20.21\public\avaliacao1`
   * Credenciais de rede: Usuário: `alunoifal` | Senha: `alunoifal`
2. Copie o arquivo **`UbuntuAvaliacao1.ova`** para o disco local `C:\2026\BSI\VM\<SeuNome>` no seu host Windows.
3. Importe a máquina virtual para o Oracle VM VirtualBox e inicie-a.
4. Credenciais de administração locais da VM (se necessário): Usuário: `administrador` | Senha: `adminifal`.

### Passo 3: Preencher a Avaliação
1. No seu repositório pessoal recém-criado, renomeie o arquivo `template-prova-1-v2.md` para **`Avaliacao1.md`**.
2. Edite esse arquivo diretamente no GitHub (pelo próprio editor web) ou clone o repositório em sua máquina física do laboratório para trabalhar localmente.
3. Conforme realiza cada uma das tarefas propostas na VM, capture as imagens de tela (prints) exigidas.
4. Salve as imagens de captura em uma pasta chamada `prints/` dentro do seu repositório e faça a referência delas no Markdown de resposta (ex: `![Questão 1](prints/q1.png)`).
5. Responda detalhadamente a cada uma das perguntas teóricas associadas às ações práticas.

### Passo 4: Envio Oficial
1. Quando concluir todas as 10 questões, certifique-se de que todos os arquivos (`Avaliacao1.md` e as imagens de prints de tela na pasta `prints/`) estejam devidamente commitados e atualizados no seu repositório privado do GitHub.
2. Acesse o link do formulário do **Google Forms** fornecido pelo professor em sala.
3. Preencha seus dados de identificação e cole o **link direto do arquivo `Avaliacao1.md`** do seu GitHub para envio no formulário de prova no Classroom

---

## 📁 Estrutura Esperada do Repositório do Aluno

O seu repositório de entrega de avaliação deve ficar organizado da seguinte forma:

```text
lsor-avaliacao1/
├── README.md               # Este arquivo de instruções gerais
├── Avaliacao1.md           # Seu caderno de respostas (antigo template-prova-1-v2.md preenchido)
└── prints/                 # Pasta contendo todos os prints de evidência técnica
    ├── q1_importacao.png
    ├── q2_usuarios.png
    ├── q3_grupos.png
    └── ... (demais capturas de tela exigidas)
```

---


_Boa prova!_  
**Prof. Alaelson Jatobá**  
_alaelson@ifal.edu.br_
