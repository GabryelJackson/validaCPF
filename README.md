# validaCPF
  Uma implementação em JavaScript para validar números de CPF (Cadastro de Pessoas Físicas) do Brasil. Ele verifica a validade de um número de CPF específico, aplicando regras de validação específicas.Aqui está uma explicação de como o código funciona:

A função ValidaCPF é definida, recebendo cpfEnviado como argumento. Ela cria uma propriedade cpfLimpo na instância do objeto ValidaCPF. Essa propriedade remove todos os caracteres não numéricos (como pontos e hifens) do CPF fornecido e armazena o número de CPF limpo.

O método ValidaCPF.prototype.valida é definido. Este método verifica a validade do CPF, verificando o comprimento, garantindo que não seja uma sequência do mesmo dígito e calculando e comparando os dois dígitos de verificação (os dois últimos dígitos) do CPF com os dígitos calculados.

O método ValidaCPF.prototype.criaDigito calcula o dígito de verificação (seja o primeiro ou o segundo) com base no número parcial do CPF fornecido.

O método ValidaCPF.prototype.isSequencia verifica se o CPF é uma sequência do mesmo dígito (por exemplo, 000.000.000-00). Se for, ele retorna true, indicando um CPF inválido.

O código cria uma instância de ValidaCPF com o número de CPF fornecido '047.721.381-29' e chama o método valida para verificar a validade.

Se o método valida retornar true, ele registra 'CPF Válido' no console, indicando que o CPF é válido. Se retornar false, ele registra 'CPF Inválido', indicando que o CPF não é válido.

O código registrará 'CPF Válido' se o CPF fornecido for válido e 'CPF Inválido' se não for. Neste exemplo específico, '047.721.381-29' é considerado um CPF válido de acordo com as regras de validação implementadas.
