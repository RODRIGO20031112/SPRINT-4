# GPT-3.5 Turbo Price Quote API

Bem-vindo à API de Cotação de Preços com o Chat GPT-3.5 Turbo! Esta API utiliza a poderosa capacidade de linguagem natural do ChatGPT-3.5 Turbo da OpenAI para fornecer recomendações de cotações de preços raspadas do Google Shopping com Selenium.

## Como Usar

1. Clone este repositório em sua máquina local.

   ```bash
   git clone https://github.com/RODRIGO20031112/SPRINT-4.git
   ```

2. Certifique que o ambiente virtual está em execução

   ```bash
   cd server/env/Scripts

   ./activate
   ```

3. Volte uma pasta e instale as dependências

   ```
   cd ../Principal

   pip install -r requiments.txt
   ```

4. Crie um arquivo `.env` no mesmo diretório do código Python (main.py) com a seguinte estrutura:

   ```bash
   API_KEY = "CHAVE_DO_CHAT_GPT"
   ```

   Substitua `"CHAVE_DO_CHAT_GPT"` pela sua chave de API do ChatGPT-3.5 Turbo.

5. Execute o script Python.

   ```bash
   python main.py
   ```

6. Siga para a url abaixo para virtualizar este servidor em app mobile ou acesse o app via terminal:

   ```bash
   https://github.com/RODRIGO20031112/SPRINT-4/tree/main/mobile
   ```

7. **Você pode alterar o código descomentando algumas linhas para ele rodar normalmente em sua máquina ou se preferir pode disparar uma requisição para http://127.0.0.1:5000/api/processNaturalLanguage/LowestPrice, lembrese-se que essa requisição é do tipo POST e espera um corpo que é:**

   ```bash
   {
   "product": "Iphone 15",
   "option": 0 # pode ser 0 ou 1 (0 para Custo Benefício - Pesquisa com ChatGPT ou 1 para Menor preço - Método Sort eficiente para ordenação de preços)
   }
   ```

8. **Se necessário, crie outra conta na OpenAI e obtenha uma nova chave de API, caso receba uma mensagem indicando que a cota foi excedida.**

## Observações

Certifique-se de proteger sua chave de API e não compartilhá-la publicamente. Se necessário, siga as instruções da OpenAI para obter uma nova chave em caso de exceder a cota.

**Aviso:** O uso excessivo pode resultar em limitações na cota ou custos adicionais, dependendo das políticas da OpenAI.

Fique à vontade para contribuir, relatar problemas ou melhorar este projeto. Obrigado por utilizar a API de Cotação de Preços GPT-3.5 Turbo!
