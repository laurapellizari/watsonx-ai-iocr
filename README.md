# Building Blocks: Aplicando IBM OCR em Arquiteturas RAG

## Objetivo

Este artigo tem como objetivo apresentar uma visão prática e estratégica da tecnologia OCR, demonstrando como utilizar o IBM IOCR para extrair textos de imagens e documentos e integrá-los com modelos de IA generativa em pipelines RAG.

## O que é OCR?

OCR (Optical Character Recognition), ou Reconhecimento Óptico de Caracteres, é uma tecnologia que permite identificar e extrair automaticamente o texto contido em imagens, documentos digitalizados ou fotos de páginas impressas. A técnica analisa os padrões visuais dos caracteres (letras, números e símbolos) e os transforma em texto digital editável e pesquisável.

Essa tecnologia é amplamente usada para digitalizar livros, processar formulários, automatizar a leitura de notas fiscais e documentos, e tornar conteúdos impressos acessíveis em formato eletrônico.


## Quando aplicar uma solução de OCR?

O uso de uma solução de OCR é indicado sempre que for necessário extrair texto de documentos ou imagens em formato não editável. Essa técnica é especialmente útil nas seguintes situações:

- Digitalização de documentos físicos: Ideal para converter papéis, livros, formulários e outros materiais impressos em texto digital, facilitando o arquivamento, a busca e a edição.
- Extração de dados de PDFs e imagens digitalizadas (notas fiscais, contratos, comprovantes);
- Automação de respostas a partir de imagens, integrando OCR com modelos generativos;
- Otimização de processos operacionais, como triagem de documentos e preenchimento automático de sistemas.

Um ponto importante a ser destacado é que os dados precisam estar armazenados no IBM Cloud Object Storage (COS) e , para utilizar a solução, só podem ser acessados mediante credenciais - o que garante maior segurança e controle de acesso. Cenário ideal quando lidamos com dados empresariais e informações sensíveis. Da mesma forma, os resultados extraídos pelo OCR também são armazenados no próprio COS, mantendo todo o fluxo de dados centralizado e protegido.

## O que existe nesse repositório:

Este repositório contém o notebook [Aplicando IBM OCR em Arquiteturas RAG: Como Potencializar a Extração de Texto](https://github.com/laurapellizari/watsonx-ai-iocr/blob/main/Aplicando%20IBM%20OCR%20em%20Arquiteturas%20RAG%3A%20Como%20Potencializar%20a%20Extra%C3%A7%C3%A3o%20de%20Textos.ipynb) que demonstra como utilizar a API do IBM OCR para extrair texto de imagens, com integração a um storage externo (Cloud Object Storage). O texto extraído é então usado como contexto para um modelo generativo responder perguntas específicas sobre o conteúdo da imagem.

## Requisitos

Para executar os códigos neste repositório, você precisará:

- Ter uma conta na IBM Cloud com acesso ao watsonx.ai (plano a partir do Essentials).
- Ter credenciais válidas do IBM Cloud Object Storage.
- Obter uma API Key da IBM Cloud para autenticação.
- Rodar o notebook: [Aplicando IBM OCR em Arquiteturas RAG: Como Potencializar a Extração de Texto](https://github.com/laurapellizari/watsonx-ai-iocr/blob/main/Aplicando%20IBM%20OCR%20em%20Arquiteturas%20RAG%3A%20Como%20Potencializar%20a%20Extra%C3%A7%C3%A3o%20de%20Textos.ipynb)

