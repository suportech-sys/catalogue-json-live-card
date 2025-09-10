# Guia de Uso - Catálogo de Toners

Este guia rápido irá ajudá-lo a entender como gerenciar e atualizar o catálogo de toners de forma eficiente.

## 1. Acessando o Catálogo

Acesse o arquivo `index.html` em um navegador web. O catálogo de toners será exibido na página principal. Abaixo da lista de produtos, você encontrará uma área de texto com o código JSON do catálogo.

## 2. Entendendo o Formato JSON

O catálogo é um arquivo JSON que organiza os dados em uma lista de objetos. Cada objeto representa um único produto e contém os seguintes campos:

- `cod`: Código do produto (ex.: "1469")
- `marca`: Marca do toner (ex.: "HP")
- `modelo`: Modelo do toner (ex.: "85A")
- `paginas`: Rendimento em número de páginas (ex.: "1600")
- `impressora`: Modelos de impressoras compatíveis, separados por | (ex.: "P1102W|M1132")
- `valor`: Valor de venda (ex.: "60,00")
- `custo`: Valor de custo (ex.: "0,00")
- `Fornecedor`: Nome do fornecedor (ex.: "xxxx")
- `Ult.Compra`: Data da última compra (ex.: "dd/mm/aaaa")
- `imagem`: URL da imagem do produto

## 3. Adicionando, Removendo e Editando Produtos

Use a área de texto para realizar atualizações. Siga estas instruções para atualizar o catálogo:

- **Para Adicionar um Produto**: Copie um bloco de produto completo (do `{` ao `}`). Cole-o no final da lista, antes do último `]`. Adicione uma vírgula (`,`) após o bloco anterior para separar os itens.
- **Para Remover um Produto**: Apague o bloco de produto (`{}`) que deseja excluir. Se o item removido não for o último da lista, verifique se não há duas vírgulas seguidas.
- **Para Editar um Produto**: Altere o texto entre aspas do campo que deseja modificar. Por exemplo, para mudar o preço, localize a linha `"valor": "60,00"` e altere o valor. Não esqueça de preencher os campos `"Fornecedor"` e `"Ult.Compra"`.

## 4. Atualizando o Catálogo

Após realizar as alterações na área de texto, clique no botão "Atualizar Catálogo". A página será recarregada, exibindo o catálogo com os produtos atualizados conforme as informações inseridas.

**Atenção**: Verifique sempre se o formato JSON está correto (aspas e vírgulas nos lugares certos). Um pequeno erro pode impedir o funcionamento do catálogo.

Se houver problemas, copie o código JSON original de volta para a área de texto e tente novamente.

---

**SuporTech - Soluções em Tecnologia e Suporte Técnico**

Contato: [suporte@suportech.com](mailto:suporte@suportech.com) | Telefone: (16) 3722-2002 | Endereço: Rua Antonio Rodrigues Netto, 862 - Franca - São Paulo

© 2025 SuporTech. Todos os direitos reservados.