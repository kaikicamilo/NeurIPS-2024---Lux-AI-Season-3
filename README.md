# Lux AI Season 3 Python Kit

Este é o repositório para o kit Python. Certifique-se de ler as instruções, pois elas são importantes para entender como escrever um bot e enviá-lo para a competição. Para saber quais pacotes Python estão disponíveis no servidor da competição, veja [este link](https://github.com/Lux-AI-Challenge/Lux-Design-S2/tree/main/kits/available_packages.txt).

Acompanhe nosso [Discord](https://discord.gg/aWJt3UAcgn) para anúncios importantes, incluindo alterações críticas, ou acesse os [fóruns do Kaggle](https://www.kaggle.com/c/lux-ai-season-3/discussion).

## Requisitos

Você precisará de **Python 3.9** ou superior e **NumPy** instalado (que deve vir junto com as dependências instaladas para o ambiente). Para instalar o ambiente, execute:

```bash
pip install --upgrade luxai-s3
```

## Começando

Seu código principal do agente será colocado no arquivo `agent.py`, e você pode criar e usar mais arquivos auxiliares. Deixe o arquivo `main.py` intacto, pois ele habilita seu agente para competir contra outros agentes localmente e no Kaggle.

Para executar rapidamente seu agente, use:

```bash
luxai-s3 main.py main.py --output=replay.html
```

Isso executará o código do `agent.py` na mesma pasta que o `main.py` e gerará um arquivo de replay salvo como `replay.html`, que pode ser aberto e assistido.

## Desenvolvimento

Agora que o código está configurado e funcionando, você está pronto para começar a programar e se divertir!

Tutorial detalhado em um notebook Jupyter tanto [localmente](https://github.com/Lux-AI-Challenge/Lux-Design-S2/blob/main/kits/python/lux-ai-challenge-season-2-tutorial-python.ipynb) quanto no [Kaggle](https://www.kaggle.com/code/stonet2000/lux-ai-challenge-season-2-tutorial-python).

Todos os kits seguem uma API comum, que você pode usar para acessar várias funções e propriedades úteis no desenvolvimento da sua estratégia e bot. Veja a versão markdown aqui: [README do Kit](https://github.com/Lux-AI-Challenge/Lux-Design-S3/blob/main/kits/README.md), que também descreve a estrutura de observação e ação.

## Envio para o Kaggle

Os envios precisam ser um arquivo .tar.gz com o main.py no diretório principal (não aninhado). Para criar um envio, use o comando:

```bash
tar -czvf submission.tar.gz *
```

O arquivo deve ser enviado na aba "Minhas Submissões" do Kaiki bonitão, e pronto! A submissão começará com um jogo agendado contra ela mesma para garantir que tudo está funcionando antes de entrar no pool de partidas com o restante da leaderboard.
