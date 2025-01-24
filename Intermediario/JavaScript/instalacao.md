O **NVM (Node Version Manager)** é uma ferramenta indispensável para desenvolvedores JavaScript que trabalham com diferentes projetos ou precisam gerenciar múltiplas versões do Node.js. Ele oferece diversos benefícios que facilitam o dia a dia de um desenvolvedor, como:

### **Gerenciamento de Versões:**

- **Múltiplas versões:** Permite instalar e gerenciar diversas versões do Node.js em uma única máquina.
- **Isolamento de projetos:** Cada projeto pode ter sua própria versão do Node.js, evitando conflitos de dependências.
- **Facilidade de troca:** Trocar entre as versões é simples e rápido, utilizando comandos no terminal.

### **Compatibilidade:**

- **Versões específicas:** Garante que cada projeto utilize a versão do Node.js com a qual foi desenvolvido, evitando problemas de compatibilidade.
- **Teste em diferentes versões:** Facilita o teste do código em diferentes versões do Node.js para garantir a portabilidade.

### **Organização:**

- **Ambiente limpo:** Mantém o ambiente de desenvolvimento organizado, evitando a instalação global de pacotes.
- **Controle de versões:** Permite rastrear as versões utilizadas em cada projeto, facilitando a reprodução de ambientes.

### **Eficiência:**

- **Instalação rápida:** A instalação de novas versões do Node.js é rápida e simples.
- **Atualizações:** Facilita a atualização para novas versões do Node.js quando necessário.

### **Cenários comuns de uso:**

- **Projetos com diferentes versões do Node.js:** Ao trabalhar em projetos que utilizam versões distintas, o NVM evita conflitos e garante que cada projeto utilize a versão correta.
- **Desenvolvimento de bibliotecas:** Ao criar bibliotecas, é importante testar a compatibilidade com diferentes versões do Node.js.
- **Aprendizado:** Ao explorar diferentes versões do Node.js e suas funcionalidades, o NVM permite experimentar sem afetar outros projetos.

[Node.js — Run JavaScript Everywhere](https://nodejs.org/en)

***Install NODE com NVM***


`LINUX`

Abra o console e use o seguinte comando:

```bash
    sudo apt-get install wget
```
    
    
[GitHub - nvm-sh/nvm: Node Version Manager - POSIX-compliant bash script to manage multiple active node.js versions](https://github.com/nvm-sh/nvm?tab=readme-ov-file#intro)
    
Para instalar uma versão diferente, substitua v0.39.0 por outro valor ou use o seguinte comando para baixar a versão mais recente:

```bash
    wget -qO- https://raw.githubusercontent.com/creationix/nvm/v0.39.0/install.sh | bash
```
    
    
Permita que o script NVM seja executado a partir do perfil bash do seu usuário:
    
```bash
    source ~/.profile
```
Depois que o NVM for instalado, você poderá começar a instalar o Node.js em seu sistema.

Verifique todas as versões disponíveis do Node.js usando o NVM executando o seguinte comando:
    
```bash
    nvm ls-remote
```

Escolha a versão:
    
```bash
    nvm install <Versão node>
``` 
Exemplo:

```bash
    nvm install 20.17.0 
```
Verificar a versão:

```bash
    node -v
```

`Windows`

[Siga o exemplo do repositório](https://josiaspereira.com.br/como-configurar-o-node-com-nvm-windows/)


Se quiser brincar um pouco:

- Status code com NODE
    
    
    $: node
    >http
    
    Para sair
    >.exit