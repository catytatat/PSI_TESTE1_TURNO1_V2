# Teste de PSI 1 - Turno 1 - Versão 2

## Informação do aluno

    Nome: Catarina Feliciano Cachoeira

Teste termina às 10:45.

Escreve as respostas dentro dos blocos correspondentes.
Substitui as reticências pelo que é pedido em cada pergunta.
Não desformates o documento.

### P1. Indica o que é impresso pelo seguinte código. Justifica a tua resposta

    bool b = 5 < 2;
    double d = Convert.ToDouble(b);
    
    Console.WriteLine(d);

P1 - Resposta

    O código apresentado declara uma variável booleana b que começa com o resultado da comparação 5 < 2. Como 5 não é menor que 2, o valor de b será false. Em seguida, a variável booleana b é convertida em um número de ponto flutuante usando o Convert.ToDouble(). Como o valor booleano é false, é convertido em 0 e armazenado na variável d, o resultado impresso no console será 0.

### P2. Considera o seguinte código com um *bug*

    string s = "2.5";
    double d = Convert.ToInt32(s);

    Console.WriteLine(d);

### Indica uma possível correção para que o código não apresente erros. Explica porque foi necessário fazer essa correção

P2 - Resposta

     A variável s é uma string que contém o valor “2.5”, que não pode ser convertido diretamente para um número inteiro. É necessário alterar a linha double d = Convert.ToInt32(s); para double d = Convert.ToDouble(s);. Assim, o valor da string seria convertido em um número decimal e armazenado na variável d.

### P3. Escreve um programa que solicite ao utilizador dois números inteiros e os multiplique, apresentando o resultado. Caso este seja um número divisível por 3, deve também ser impressa a mensagem "Múltiplo de 3!"

P3 - Resposta

    static void Main(string[] args)
    {
        Console.Write("Digite o primeiro número: ");
        int number1 = Convert.ToInt32(Console.ReadLine());

        Console.Write("Digite o segundo número: ");
        int number2 = Convert.ToInt32(Console.ReadLine());

        int result = number1 * number2;
        Console.WriteLine("O resultado da multiplicação é: " + result);

        if (result % 3 == 0)
        {
            Console.WriteLine("Múltiplo de 3!");
        }

### P4. Tens um repositório git criado localmente, onde estás no ramo 'master'. Queres associá-lo ao repositório remoto contido no url 'https://github.com/PSI/OMeuRepositorioRemotoV2'. Queres também alterar o nome do ramo atual para 'main'. Deverás enviar os *commits* já feitos localmente para o repositório remoto. Indica os comandos necessários

P4 - Resposta

    Para associar o repositório local ao repositório remoto contido no url ‘https://github.com/PSI/OMeuRepositorioRemotoV2’, primeiro, é necessário adicionar o endereço remoto ao repositório local. Para fazer isso, execute o seguinte comando:

    git remote add origin https://github.com/PSI/OMeuRepositorioRemotoV2.git

    Em seguida, para enviar os commits já feitos localmente para o repositório remoto, execute o seguinte comando:

    git push -u origin master:main

    Isso enviará todos os commits feitos no ramo ‘master’ local para o ramo ‘main’ do repositório remoto. O parâmetro ‘-u’ é usado para configurar o ramo ‘main’ como o ramo padrão para futuros envios.


