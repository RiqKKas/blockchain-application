<h1 align="center"> Blockchain Application </h1>

<div align="center">
 <a href="#about">Sobre</a> |
 <a href="#installation">Como executar</a> |
 <a href="#author">Autor</a>
</div>

<h2 id="about">💡&nbsp; Sobre o projeto</h2>

<h3>Introdução</h3>
<p>
  A tecnologia blockchain é um sistema de registro distribuído que viabiliza a criação de um livro-razão público imutável. Este documento abordará a criação de uma blockchain básica em Python, conforme exemplificado no código fornecido.
</p>

<h3>Estrutura do Bloco</h3>
<p>
  Um bloco na blockchain possui elementos como índice, carimbo de data e hora, transações, prova de trabalho e o hash do bloco anterior. A conexão entre os blocos é estabelecida por meio dos hashes.
</p>

<h3>Criação da Cadeia de Blocos</h3>
<p>
  A cadeia de blocos é, essencialmente, uma lista de blocos. O primeiro bloco, conhecido como "bloco gênesis", é gerado durante a fase inicial. Novos blocos são acrescentados à cadeia por meio do processo de mineração.
</p>

<h3>Mineração</h3>
<p>
  A mineração de novos blocos emprega o algoritmo de prova de trabalho. Isso implica encontrar um valor (nonce) de maneira que o hash do bloco atenda a critérios específicos, como iniciar com zeros. A recompensa pela mineração é uma transação fictícia, com o mineiro como destinatário.
</p>

<h3>Transações</h3>
<p>
  As transações são incorporadas ao bloco por meio do método new_transaction(). Cada transação inclui informações sobre o remetente, destinatário e quantidade.
</p>

<h3>Consenço e Resolução de Conflitos</h3>
<p>
  A garantia de consenso na rede requer a implementação do algoritmo de resolução de conflitos. Cada nó verifica a validade da cadeia e a substitui pela própria se uma cadeia mais longa e válida for encontrada.
</p>

<h3>Nós</h3>
<p>
  Os nós da rede são adicionados dinamicamente por meio do método register_node(), possibilitando a comunicação entre eles para alcançar consenso.
</p>

<h3>Cadeia</h3>
<p>
  A validação da cadeia é conduzida pelo método is_valid_chain(), que verifica a integridade dos hashes e a prova de trabalho.
</p>

<h3>Sistema</h3>
<p>
  A aplicação da blockchain foi concretizada como uma aplicação Flask. Os endpoints /mine, /transactions/new, /chain, /nodes/register e /nodes/resolve proporcionam funcionalidades para mineração, criação de transações, visualização da cadeia, registro de nós e resolução de conflitos, respectivamente.
</p>

<h3>Conclusão</h3>
<p>
  A implementação da blockchain em Python oferece uma compreensão prática dos conceitos fundamentais subjacentes a essa tecnologia. Este documento enfatizou os aspectos cruciais do código e a lógica por trás da criação de uma blockchain simples, servindo como uma base sólida para a compreensão de blockchains mais complexas.
</p>

---

<h2 id="installation">🚀&nbsp; Como executar </h2>

```bash
# Clone o repositório
git clone git@github.com:the-riquelme/tic-tac-toe-xo-transactions.git

# Execute o programa
python3 src/blockchain.py

```

---

<h2 id="author">👨‍💻&nbsp; Autor</h2>

<b>👤 Riquelme Damião Silva<b>

<div style="display: inline_block">
  <a href="https://www.linkedin.com/in/riquelme-damiao-silva/" target="_blank">
   <img src="https://img.shields.io/badge/-LinkedIn-%230077B5?style=for-the-badge&logo=linkedin&logoColor=white" target="_blank">
  </a>
  <a href="mailto:riquelmedamiaosilva@gmail.com" target="_blank">
    <img src="https://img.shields.io/badge/gmail-D14836?&style=for-the-badge&logo=gmail&logoColor=white"/>
  </a>
</div>
