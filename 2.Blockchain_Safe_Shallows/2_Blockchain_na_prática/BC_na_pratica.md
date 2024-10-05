# **Blockchain na prática**

Vamos abordar conceitos práticos do que uma blockchain é composta:

## **Hash**:

Assim como o ser humano possuí uma impressão digital única, o hash seria a impressão digital de um conjunto de dados. É uma função criptografica que exibe uma saída de caracteres único de um conjunto de dados. Por exemplo: (Hash - SHA256)

Bom dia!
e358708abb75634bf13ff278e914da8d742e1dbd803fd3cb56077b4b62fd3774

Bom dia
fe01c0c9210f2f95e7edbe427a7e96a981b95e08cc27ad0b017b520a4e7afe17

Veja que no primeiro exemplo temos a frase **Bom dia!** e o seu hash logo abaixo. No outro exemplo, mudamos a frase **eliminando o ponto de exclamação (!)** no final **Bom dia** e o hash teve uma saída diferente.

Isso quer dizer que: por mais que as frases sejam parecidas, só em você mudar uma coisa que seja do seu **dado**, o hash, a impressão digital desse dado será completamente diferente.

## **Block**

Aqui temos o nosso **Bloco** que nada mais é que um agrupamento de dados atribuídos a ele. Esses dados são compostos por:

---

| Block: #1 - Genesis Block                                                            |
|--------------------------------------------------------------------------------------|
| **Nonce:**          1562                                                             |
| **Data:**           documento sigiloso                                               |
| **Hash anterior:**  0000000000000000000000000000000000000000000000000000000000000000 |
| **Hash:**          0008756a228c85b7e28e79e5c12a79afbf06e0275a8ef15b7febbc2423187829  |

---

| Bloco: #2                                                                            |
|--------------------------------------------------------------------------------------|
| **Nonce:**          1541                                                             |
| **Data:**           documento sigiloso 2                                             |
| **Hash anterior:**  0008756a228c85b7e28e79e5c12a79afbf06e0275a8ef15b7febbc2423187829 |
| **Hash:**          000aa0ebb8b3c6c14631a18e7c16a782436bb7bdec10832f4b4cc2ef609b297c  |

---

* **Block**: significa o número/altura do bloco. O primeiro bloco criado na Blockchain é chamado de Genesis Block.
* **Nonce**: Um número aleatório que precisa ser descoberto para que o Hash do bloco comece com uma sequência de zeros, no caso do primeiro bloco: **000**8756a228c. A resposta mais simples do que correta é que essa sequência de zeros está atribuída a um indicativo de "dificuldade" da rede, quanto mais zeros, mais difícil foi de encontrar um Nonce correspondente a um Hash que inicie com essa sequência de zeros abaixo da dificuldade da rede.
* **Data**: São os dados propriamente dito, o dado inserido no exemplo acima foram frases, ou seja, um conjunto de caracteres, porém, pode ser qualquer outro dado.
* **Hash anterior**: Significa o hash produzido pelo bloco anterior.
* **Hash**: Aqui é o hash do bloco, ele é uma combinação de tudo o que você viu acima, ou seja, se você **alterar o Nonce ou Data** a saída do hash será um completamente diferente.

## **Blockchain**

E nossa **Blockchain**? O que seria ela?

Bem, a nossa **Blockchain** seria o conjunto de todos esses blocos em cadeia, um livro-razão que possuí todos os registros de transações registradas em cada bloco.

Como você pode observar, cada bloco depende do hash do bloco anterior e assim sucessivamente para construir uma cadeia linear de blocos. O fato de que caso haja alguma alteração em algum documento, minima que seja, esse cadeia de blocos irá **colapsar**, já que mudando o dado, o hash muda...e se o hash de um bloco muda, o hash do próximo bloco também mudará...e assim sucessivamente.

Por se tratar de uma rede descentralizada e em consenso. Para que alguem consiga alterar um dado de um bloco e esse dado seja validado na rede, a pessoa teria que ter mais de 50% de poder computacional para descobrir o hash a partir do bloco que foi alterado esse dado e o hash seguinte de todos os blocos da cadeia. E mesmo assim, como na Blockchain a cadeia **mais longa** é a válida, essa pessoa teria que descobrir todos os hashs de todos os blocos antes que a rede crescesse um pouco mais (antes que novos blocos sejam criados), tornando essa tarefa basicamente impossível.