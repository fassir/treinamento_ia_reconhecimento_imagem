# Transfer Learning para Classificação de Imagens: Microsoft Cats and Dogs

Este projeto demonstra como aplicar **transfer learning** para classificar imagens de gatos e cachorros utilizando o dataset **Microsoft Cats and Dogs**. O objetivo é mostrar, na prática, como aproveitar um modelo pré-treinado (VGG16) para obter alta acurácia mesmo com um conjunto de dados moderado.

## Sobre o Dataset
- **Fonte:** Microsoft Cats and Dogs
- **Total de imagens:** Aproximadamente 25.000
- **Categorias:**
  - Cat (gato)
  - Dog (cachorro)
- **Formato das imagens:** RGB, redimensionadas para 224x224 pixels

## Fluxo do Notebook
1. **Download e extração automática do dataset**
2. **Pré-processamento das imagens** para o formato adequado
3. **Divisão dos dados**:
   - Treino: 70%
   - Validação: 15%
   - Teste: 15%
4. **Construção e treinamento de uma rede neural simples do zero** para comparação
5. **Transfer learning com VGG16** pré-treinado no ImageNet
6. **Avaliação e comparação dos resultados**
7. **Visualização de exemplos e análise dos desempenhos**

## Resultados Esperados
- O modelo simples treinado do zero serve como baseline.
- O modelo com transferência de aprendizado (VGG16) apresenta desempenho significativamente superior, mostrando a vantagem de reutilizar características aprendidas em grandes bases de imagens.
- O notebook inclui visualizações, métricas de acurácia e exemplos de predição.


## Como Executar

### Google Colab (Recomendado para quem não tem GPU local)
1. Acesse o arquivo `transfer_learning.ipynb` no seu repositório do GitHub ou faça upload para o Google Drive.
2. Abra o notebook no Google Colab:
   - Se estiver no GitHub, clique no botão "Open in Colab" no topo do notebook (ou use o link/badge se disponível).
   - Se estiver no Google Drive, clique com o botão direito no arquivo e escolha "Abrir com > Google Colab".
3. No Colab, vá em `Ambiente de execução > Alterar tipo de ambiente de execução` e selecione **GPU** para acelerar o processamento.
4. Execute todas as células do notebook. O Colab já possui as principais dependências instaladas, mas se necessário, execute a célula de instalação de pacotes.

### Local (Jupyter)
1. Instale as dependências:
   ```bash
   pip install tensorflow matplotlib pillow
   ```
2. Execute o notebook `transfer_learning.ipynb` em seu ambiente Jupyter.

## Observações
- O código faz o download automático do dataset na primeira execução.
- O processamento pode ser demorado, levando até horas em máquinas comuns sem GPU. Tenha paciência e, se possível, utilize um ambiente com aceleração por GPU.
- O projeto é ideal para quem deseja aprender na prática como aplicar transfer learning em problemas reais de classificação de imagens.

