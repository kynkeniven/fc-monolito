ERRO NO TESTE DA FACADE

Não consegui identificar o porque estou recebendo o erro abaixo ao executar o teste do generate da facade do Invoice


ConnectionManager.getConnection was called after the connection manager was closed!

      47 |
      48 |     for (const item of invoice.items) {
    > 49 |       await InvoiceItemsModel.create({
         |       ^
      50 |         id: item.id.id,
      51 |         name: item.name,
      52 |         price: item.price,



Engraçado que ao teste pelo  repository e pelo use case funciona, mas quando esse metodo é chamado passando pela facade da erro.

Poderia me ajudar?
