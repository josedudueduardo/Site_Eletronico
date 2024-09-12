<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Carrinho</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>
    <nav class="navbar navbar-expand-lg navbar-light bg-light"></nav>
        <div class="container">
            <a class="navbar-brand" href="index.html">Voltar</a>
        </div>
    </nav>

    <div class="container mt-4">
        <h1>Carrinho de Compras</h1>
        <div id="carrinho"></div>
        <h2 id="total">Total: R$0.00</h2>
        <button class="btn btn-danger" id="limpar-carrinho">Limpar Carrinho</button>
    </div>

    <script>

function renderizarCarrinho() {
            const carrinho = JSON.parse(localStorage.getItem('carrinho')) || [];
            const carrinhoDiv = document.getElementById('carrinho');

            if (carrinho.length === 0) {
                carrinhoDiv.innerHTML = '<p>Seu carrinho está vazio.</p>';
                return;
            }

            carrinhoDiv.innerHTML = `
                <table class="table">
                    <thead>
                        <tr>
                            <th>Produto</th>
                            <th>Quantidade</th>
                            <th>Preço</th>
                            <th>Total</th>
                            <th>Ações</th>
                        </tr>
                    </thead>
                    <tbody>
                        ${carrinho.map(item => `
                            <tr>
                                <td>${item.name}</td>
                                <td>
                                    <input type="number" value="${item.quantidade}" min="1" data-id="${item.id}" class="quantidade-input">
                                </td>
                                <td>R$${item.price.toFixed(2)}</td>
                                <td>R$${(item.price * item.quantidade).toFixed(2)}</td>
                                <td>
                                    <button class="btn btn-danger btn-sm remover-item" data-id="${item.id}">Remover</button>
                                </td>
                            </tr>
                        `).join('')}
                    </tbody>
                </table>
            `;

           
            document.querySelectorAll('.quantidade-input').forEach(input => {
                input.addEventListener('change', (event) => {
                    atualizarQuantidade(event.target.dataset.id, event.target.value);
                });
            });

            document.querySelectorAll('.remover-item').forEach(button => {
                button.addEventListener('click', (event) => {
                    removerItem(event.target.dataset.id);
                });
            });
            atualizarTotal();
        }

       
        function atualizarQuantidade(id, quantidade) {
            let carrinho = JSON.parse(localStorage.getItem('carrinho')) || [];
            const index = carrinho.findIndex(item => item.id == id);
            if (index !== -1) {
                carrinho[index].quantidade = parseInt(quantidade);
                localStorage.setItem('carrinho', JSON.stringify(carrinho));
                renderizarCarrinho();
            }
            atualizarTotal();
        }

        
        function removerItem(id) {
            let carrinho = JSON.parse(localStorage.getItem('carrinho')) || [];
            carrinho = carrinho.filter(item => item.id != id);
            localStorage.setItem('carrinho', JSON.stringify(carrinho));
            renderizarCarrinho();
            atualizarTotal();
        }

       
        document.getElementById('limpar-carrinho').addEventListener('click', () => {
            localStorage.removeItem('carrinho');
            renderizarCarrinho();
            atualizarTotal()
        });

        function atualizarTotal() {
            const carrinho = JSON.parse(localStorage.getItem('carrinho')) || [];
            const total = carrinho.reduce((acc, item) => acc + item.price * item.quantidade, 0);
            const totalDiv = document.getElementById('total');
            if (totalDiv) {
                totalDiv.innerHTML = `Total: R$${total.toFixed(2)}`;
            }
        }
        atualizarTotal();
        
        renderizarCarrinho();

    </script>
</body>
</html>
