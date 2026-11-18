# Ateliê do Bebê — 300 Moldes de Roupas de Bebê

Landing page estática e responsiva para a oferta **Ateliê do Bebê**, em português do Brasil.

## Como usar

Abra `index.html` no navegador ou publique a raiz do repositório em um serviço de hospedagem estática (GitHub Pages, Netlify ou similar). Não é necessário instalar dependências ou executar build.

## Configurar os botões de pagamento

**Obrigatório antes de vender:** edite `index.html` e substitua os valores `href="CHECKOUT_BASICO"` e `href="CHECKOUT_COMPLETO"` pelas URLs HTTPS reais do seu provedor de pagamento.

Enquanto esses valores não forem substituídos, um clique exibirá uma mensagem informando que o checkout ainda não está configurado. O site não inventa links de pagamento.

## Editar informações da oferta

Todo o conteúdo está no `index.html`. Procure pelos comentários de seção para modificar os textos, a lista de moldes, os seis bônus, os preços ou as perguntas frequentes.

Os preços comparativos, prazos, condições da garantia e benefícios apresentados devem ser verificados antes de veicular anúncios e aceitar pagamentos.

## Adicionar depoimentos reais

No HTML, procure:

```html
<!-- ESPAÇO RESERVADO PARA PRINTS REAIS DE CLIENTES: inserir apenas depoimentos autênticos, com autorização. -->
```

Insira depoimentos reais nesse local, preferencialmente com autorização dos respectivos clientes. Não há depoimentos fictícios nem cronômetros no projeto.

## Estrutura e desempenho

- Página estática única em `index.html`: HTML semântico, CSS mobile-first e JavaScript mínimo.
- Ícones das roupinhas em SVG inline, sem arquivos de imagens externos.
- Fontes **Fraunces** e **Nunito** hospedadas no Google Fonts, com fontes locais de fallback.
- FAQ com `details`/`summary` nativos; navegação por teclado, foco visível e suporte a `prefers-reduced-motion`.
- Links de chamada à ação com âncora `#planos`.
- Nenhum backend, banco de dados, ferramenta de analytics ou pacote de terceiros em JavaScript.

## Validação rápida

1. Abra o HTML nos tamanhos 320px, 375px, 768px e 1280px.
2. Verifique que o Plano Completo aparece primeiro no celular.
3. Clique nas três chamadas `QUERO MEUS 300 MOLDES` e confira que levam a `#planos`.
4. Abra e feche as sete perguntas do FAQ, inclusive via teclado.
5. Substitua os links de checkout e teste os dois fluxos de pagamento no ambiente de teste do provedor.

## Publicação

Para GitHub Pages, selecione **Settings > Pages > Deploy from a branch > main / (root)** no repositório. A URL da página dependerá da configuração da conta e da publicação pelo GitHub. Não há implantação automática configurada neste repositório.
