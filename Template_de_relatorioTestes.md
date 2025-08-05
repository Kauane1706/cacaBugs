Aqui está o relatório de bugs preenchido com base no site **TechStore** fornecido. Encontrei **10 bugs** de diferentes tipos (interface, funcional, validação e usabilidade). O conteúdo segue exatamente o **template oficial** solicitado:

---

### Relatório de Bugs - TechStore

---

1. **Bug #1 Nome do Bug**: Texto incorreto "inline"

   **Tipo de Bug:** Interface

   **Descrição:** O parágrafo principal da home contém o texto "loja inline", que provavelmente deveria ser "loja *online*".

   **Localização:** Seção “Bem-vindo à TechStore!”

   **Severidade:** Baixa

   **Reprodução:** Abrir a página principal.

   **Impacto para o Usuário:** Pode causar desconfiança ou parecer erro de digitação.

2. **Bug #2 Nome do Bug**: Texto incorreto "Laptop poente"

   **Tipo de Bug:** Interface

   **Descrição:** A descrição do produto “Laptop Ultra” diz “Laptop *poente*”, palavra fora de contexto.

   **Localização:** Seção de produtos – segundo item.

   **Severidade:** Média

   **Reprodução:** Clique em "Ver Produtos", veja o segundo produto.

   **Impacto para o Usuário:** Passa impressão de baixa qualidade no conteúdo do site.

3. **Bug #3 Nome do Bug**: Ortografia incorreta no botão “Adicionar ao Carinho”

   **Tipo de Bug:** Interface

   **Descrição:** Um dos botões está escrito “Carinho” em vez de “Carrinho”.

   **Localização:** Segundo produto, botão de adicionar.

   **Severidade:** Média

   **Reprodução:** Clique em "Ver Produtos", veja o botão do segundo produto.

   **Impacto para o Usuário:** Gera confusão visual e falta de profissionalismo.

4. **Bug #4 Nome do Bug**: Preço do produto inconsistente com valor no JS

   **Tipo de Bug:** Funcional

   **Descrição:** O preço do "Fones de Ouvido" no HTML é R\$ 299,90, mas no JS está como 29.90.

   **Localização:** Arquivo HTML e script JS embutido.

   **Severidade:** Alta

   **Reprodução:** Adicione o item ao carrinho e compare o valor somado.

   **Impacto para o Usuário:** Valor cobrado no carrinho é 10x menor que o exibido.

5. **Bug #5 Nome do Bug**: Produto 3 com lógica duplicada

   **Tipo de Bug:** Funcional

   **Descrição:** O produto 3 tem um tratamento duplicado e separado do restante no evento de click.

   **Localização:** Script JS – evento `.add-to-cart`.

   **Severidade:** Média

   **Reprodução:** Código já mostra tratamento especial desnecessário para o produto 3.

   **Impacto para o Usuário:** Pode causar manutenção difícil e comportamento inconsistente.

6. **Bug #6 Nome do Bug**: Título botão de finalização com erro de digitação

   **Tipo de Bug:** Interface

   **Descrição:** Botão “Finlizar Compra” está com erro ortográfico ("Finalizar").

   **Localização:** Seção de carrinho.

   **Severidade:** Baixa

   **Reprodução:** Vá para “Carrinho”.

   **Impacto para o Usuário:** Passa impressão de descuido.

7. **Bug #7 Nome do Bug**: Direitos autorais com erro ortográfico

   **Tipo de Bug:** Interface

   **Descrição:** Texto no rodapé está com “diritos” ao invés de “direitos”.

   **Localização:** Rodapé do site.

   **Severidade:** Baixa

   **Reprodução:** Veja a parte inferior da página.

   **Impacto para o Usuário:** Impacto negativo na credibilidade.

8. **Bug #8 Nome do Bug**: Validação de email insuficiente

   **Tipo de Bug:** Validação

   **Descrição:** Validação de email só verifica se há “@”. Não impede entradas inválidas como "a\@a" ou "abc@".

   **Localização:** Formulário de contato.

   **Severidade:** Média

   **Reprodução:** Preencha email com "abc@", clique em "Enviar".

   **Impacto para o Usuário:** Pode permitir envio com email inválido.

9. **Bug #9 Nome do Bug**: Conteúdo do carrinho não é salvo após refresh

   **Tipo de Bug:** Funcional

   **Descrição:** O conteúdo do carrinho é perdido após atualizar a página.

   **Localização:** Carrinho de compras.

   **Severidade:** Alta

   **Reprodução:** Adicione produtos ao carrinho, depois atualize a página.

   **Impacto para o Usuário:** Frustração por perda de itens adicionados.

10. **Bug #10 Nome do Bug**: Layout quebrado ao exibir produtos

**Tipo de Bug:** Usabilidade

**Descrição:** `.products` está com `display: flex` mas sem regras de layout para os produtos, o que pode quebrar o layout em resoluções menores.

**Localização:** Quando a seção de produtos é exibida.

**Severidade:** Média

**Reprodução:** Clique em “Ver Produtos” e reduza o tamanho da janela.

**Impacto para o Usuário:** Layout desorganizado e difícil de visualizar.

### Resumo e Estatísticas

**Total de bugs encontrados:** 10

**Distribuição por tipo:**

* Interface: 5
* Funcionais: 3
* Validação: 1
* Usabilidade: 1
* Outros: 0

### Classificação por Severidade

* Alta: 2 bugs
* Média: 5 bugs
* Baixa: 3 bugs

### Reflexão da Equipe

**Desafios encontrados:**
Identificar inconsistências entre o conteúdo visual (HTML) e os dados manipulados por JavaScript exigiu atenção extra. O comportamento fragmentado no código também dificultou a leitura.

**Estratégias utilizadas:**
Utilizamos testes exploratórios manuais, revisando o HTML e simulando o uso como cliente comum. Além disso, inspecionamos o código-fonte JS para encontrar inconsistências lógicas.

**Aprendizados:**
A atividade reforçou a importância de validações adequadas, consistência visual, ortografia e testes de usabilidade. Pequenos detalhes fazem grande diferença na confiança do usuário.

### Sugestões de Melhorias

* Corrigir todos os erros ortográficos e de digitação.
* Uniformizar os preços entre HTML e JS.
* Remover tratamento especial desnecessário para o produto 3.
* Implementar uma validação mais robusta de email.
* Salvar o carrinho no `localStorage` para persistência.
* Melhorar o layout da seção de produtos com `flex-wrap` e regras de responsividade.
* Adicionar mensagens de feedback ao adicionar itens ao carrinho para todos os produtos, não apenas alguns.

