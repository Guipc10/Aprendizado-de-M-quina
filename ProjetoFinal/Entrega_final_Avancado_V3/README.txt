Unicamp-Curso de Extensao de Mineracao de Dados Complexos - 2020/Semestre 1
Disciplina: INF-0619 – Projeto Final  
Projeto Final 2 - Melanoma Classification
-----------------------------------------------------------------
Grupo:   The Outliers 
Alunos:  Paula Sampaio Meirelles 
         Raphael Mendes Motta 
         Renata Biaggi Barreto 
         Tailís Tavera Ferreira
-----------------------------------------------------------------

################################################################
#### Item 1.Fonte de Dados
################################################################
Os arquivos podem ser obtidos através do site do Kaggle, página do desafio "SIIM-ISIC Melanoma Classification", opção Data.
Segue link direto para essa página: https://www.kaggle.com/c/siim-isic-melanoma-classification/data

Observação: o arquivo zip "siim-isic-melanoma-classification" com todos os dados disponibilizados pelo Kaggle possui mais de 105 GB,

Contendo >
 1a. pasta: jpeg         30,9  GB 
        subpasta: test    6,97 GB - imagens de teste no formato jpg     
        subpasta: train  23,90 GB - imagens de treino no formato jpg  

 1b. pasta: test      15,6 GB (16.807.743.094 bytes) - imagens de teste no formato DCM ( especificacao padrao de imagens médica)
 1c. pasta: tfrecords 11,6 GB (12.514.982.695 bytes) - arquivos com uma sequência de registros binários das imagens 
 1d. pasta: train     49,9 GB (53.586.306.258 bytes) - imagens de treino no formato DCM ( especificacao padrao de imagens médica)
 1e. Arquivo: sample_submission.csv 164 KB           - listagem de amostras
 1f. Arquivo: test.csv              479 KB           - listagem das imagens de teste com as caracteristicas de paciente
 1g. Arquivo: train.csv             1,95 MB          - listagem das imagens de treino com as caracteristicas de paciente e target

Para esse projeto utilizamos apenas os arquivos jpeg (1a) e de características  1f e 1g

Segue link para baixar cada um desses itens individualmente:
  1a pasta: jpeg        - https://www.kaggle.com/c/siim-isic-melanoma-classification/data?select=jpeg
  1f Arquivo: test.csv  - https://www.kaggle.com/c/siim-isic-melanoma-classification/data?select=test.csv
  1g Arquivo: train.csv - https://www.kaggle.com/c/siim-isic-melanoma-classification/data?select=train.csv

################################################################
#### Item 2. Execução do Código
################################################################

O trabalho é composto de um único script em Python: Script_Colab_TheOutliers_MelanomaClas.ipynb

Para executá-lo:
  2a. Efetuar upload desse arquivo ipynb em ambiente Google
  2b. Abrir o Arquivo com a Ferramenta Google Colaboratory (Colab)
  2c. Esse código contêm referência para
       2c.1> um Drive Shared do Google Drive chamado "Melanoma" onde :
             2c.1.1 >  Fizemos upload dos arquivos test.csv(item 1f) e train.csv (item 1g) nesse drive
             2c.1.2 >  Na sequência criamos uma pasta "TodasImagens" nesse drive
             2c.1.3 >  E nessa subpasta "TodasImagens" fizemos upload da pasta jpeg (item 1a) 
             

             Sugestões para ajuste de diretório de arquivos antes da execução do arquivo Script_Colab_TheOutliers_MelanomaClas.ipynb no Colab:

                         Criar a mesma estrutura no Google Drive (itens 2c.1, 2c.1.1, 2c.1.2, 2c.1.3) que será utilizado para a execução do Script 
                  ou
                         Com Script_Colab_TheOutliers_MelanomaClas.ipynb já aberto na ferramenta Colab, selecionar no menu a opção "Editar" , 
                         Seguido da opção "Localizar e Substituir",
                         Substituindo /content/drive/Shared drives/Melanoma/TodasImagens/ pelo diretório do Google Drive que contêm a pasta jpeg (item 1a),
                         Substituindo /content/drive/Shared drives/Melanoma/ pelo diretório do Google Drive que contêm  os arquivos test.csv (item 1f) e                               			 train.csv( item 1g)

   2d. Executar cada etapa de código




 


     