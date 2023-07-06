# Exame RPA Python 01
## Automação Correios

O objetivo do exame é a construção de um RPA em python para automatizar a busca de informações
no site dos correios. O programa deve ser capaz de realizar as seguintes tarefas:
- Acessar o site dos correios disponível em https://www.correios.com.br/
- Na home, informar no campo "ACOMPANHE SEU OBJETO" um código que será fornecido para rastear uma encomenda
**LB571181225HK**
- Na página que será aberta, qubrar o captcha e obter o resultado da consulta (somente o último status)
- Executar o comando em prompt de comando
- Imprimir nba tela o resultado da busca
- Fornecer todas as instruções de como preparar o ambiente para rodar o programa em um arquivo README.md

O exercício deve ser construído um robo em python dentro de uma função principal chamada
consultar_encomenda(objeto) que deverá retornar um JSON no seguinte formato:
```
{
    "status": "sucesso",
    "codigo": "LB571181225HK",
    "dados": {"titulo":"Objeto em trânsito - por favor aguarde", "mensagem": "de Unidade de Tratamento, RIO DE JANEIRO - RJ para Unidade de Distribuição, RIO DE JANEIRO - RJ 27/05/2023 08:29"}
}
```
É importante que o retorno deve conter somente a última mensagem do objeto em questão e em caso de falha na busca retornar o status como *erro* e o campo *dados* como *nulo*.

### Regras:
- O principal objetivo é avaliar não só o sucesso do exame, mas a forma de pensar do candidato e sua habilidade técnica.
- Mantenha sempre o foco no objetivo do exame! Siga os passos do exercício fielmente.
- Você pode utilizar qualquer biblioteca em python desde que o código rode dentro de uma (ou mais) função(oes).
- A solução será avaliada como um todo! Sua organização, tecnicas adotadas, tempo de entrega, bibliotecas usadas, o quanto fiel ao objetivo o candidato foi e a documentação fornecida.
- Não esqueça de fornecer um arquivo README.mb bem completo contendo instruções de como rodar seu código.
- Sua solução deverá ser executada em uma linha de comando igual a proposta abaixo:
```
> python consulta_encomenda.py LB571181225HK
```

E o resultado esperado deve ser impresso com o JSON solicitado (pode ser um print simples!).

Ao terminar seu teste, você deve enviar um email para **saulo.oliveira@approvafacil.com.br** com o repositório do github contendo todo o fonte e documentação do projeto.

**IMPORTANTE: Mesmo que não consiga fazer o exemplo em sua complitude, não deixe de enviar seu andamento! A avaliação será considerada com o que for enviado!!**